# 엘라스틱 서치의 restClient를 사용 통신 방법
### restClient를 통해서 rest 통신을 할 수 있음 but 이 방법은 가장 원시적인 방법이라 잘 쓰이진 않는다

## 예시코드
```java
RestClient restClient = RestClient.builder(
        new HttpHost("엘라스틱 서치 주소", 9200, "http/https") // 엘라스틱 서치 주소와 포트를 지정합니다.
        ).build();
        //RestClient를 이용해 엘라스틱 서치에 연결합니다.
        
    Request request = new Request("GET", "/_search");
    
    request.setJsonEntity(
        "{\n" +
        "  \"query\": {\n" +
        "    \"match_all\": {}\n" +
        "  }\n" +
        "}"
    );
    
    
    Response response = restClient.performRequset(requset);
    // 요청을 수행하고 응답을 받습니다.

    String responseBody = EntityUtils.toString(response.getEntity());
    
    system.out.println("Response: " + responseBody);

)
```


