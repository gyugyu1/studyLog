# 📘 Markdown 사용법 정리

개발 공부, TIL, 프로젝트 회고 등에 자주 사용하는 마크다운 문법 정리

---

## 📝 제목 (Heading)

```markdown
# 제목 1
## 제목 2
### 제목 3
```

결과:

# 제목 1  
## 제목 2  
### 제목 3

---

## 📋 목록 (List)

### 🔹 순서 없는 목록

```markdown
- 항목1
- 항목2
  - 하위 항목
```

### 🔸 순서 있는 목록

```markdown
1. 첫 번째
2. 두 번째
```

---

## ✨ 텍스트 강조

```markdown
**굵게**
*기울임*
~~취소선~~
```

결과:  
**굵게**  
*기울임*  
~~취소선~~

---

## 💻 코드 작성

### 🔹 인라인 코드
```markdown
`코드`
```

예: `console.log("Hello");`

### 🔸 코드 블록
\`\`\`javascript
function hello() {
  console.log("Hello!");
}
\`\`\`

---

## 🔗 링크와 이미지

```markdown
[링크텍스트](https://example.com)
![이미지설명](https://주소.com/image.png)
```

예:  
[Google](https://google.com)

---

## 🧾 수평선 (구분선)

```markdown
---
```

---

## 💬 인용문

```markdown
> 인용하고 싶은 문장
```

결과:
> 인용하고 싶은 문장

---

## ✅ 체크박스 (To-Do List)

```markdown
- [x] 완료된 항목
- [ ] 미완료 항목
```

결과:
- [x] 완료된 항목  
- [ ] 미완료 항목

---

## 📌 기타 팁

- 코드 블록 언어 지정 시 문법 강조됨 (예: `js`, `html`, `java`)
- 마크다운은 GitHub, Notion, Velog 등에서 대부분 동일하게 지원됨
- 이미지 경로는 GitHub에 올린 후 상대경로로 관리하면 편함

---

📂 마지막으로, 이 파일은 `markdown-guide.md` 로 저장하면 언제든 참고하기 좋아요!
