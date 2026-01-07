# Greenora

## 📝 Gachimura Commit Convention
- ✨ feat : 새로운 기능 추가 (ex. ✨ feat: 로그인 기능 구현구
- 🐛 fix : 버그 수정 (ex. 🐛 fix: 무한 스크롤 오류 수정)
- 💄 design : CSS 등 사용자 UI 디자인 변경 (ex. 💄 design: 메인 버튼 색상 변경)
- ♻️ refactor : 코드 리팩토링 (기능 변경 없음) (ex. ♻️ refactor: 페이지 컴포넌트 분리)
- 📝 docs : 문서 수정 (README.md, 주석 등) (ex. 📝 docs: API 명세서 업데이트)
- ✏️ chore : 빌드 업무 수정, 패키지 매니저 설정 등 (코드 변경 없음) (ex. ✏️ chore: framer-motion 패키지 추가)
- 🔨 style : 코드 포맷팅, 세미콜론 누락 등 (코드 변경 없음) (ex. 🔨 style: 코드 들여쓰기 정리)



## 브랜치 전략 - Git flow 

[참고 문헌](https://velog.io/@diduya/git-%ED%9A%A8%EC%9C%A8%EC%A0%81%EC%9D%B8-%ED%98%91%EC%97%85%EC%9D%84-%EC%9C%84%ED%95%9C-Git-Flow-%EC%9D%B4%ED%95%B4%ED%95%98%EA%B8%B0-git-branch-repository)

```
GitHub
├── frontend-repo (Next.js)
│   ├── feature/*  ← 새로운 기능 개발
│   ├── develop    ← 통합 테스트용
│   ├── release/*  ← 릴리즈 준비
│   └── main       ← 실제 배포용
│
└── backend-repo (Nest.js)
    ├── feature/*
    ├── develop
    ├── release/*
    └── main
```

### 전략 설명
1. main 브랜치
2. main 을 소스로한 develop 브랜치
3. **develop 브랜치를 소스로 한 각 기능 별 feature 브랜치**
4. **완성된 feature 브랜치는 develop 브랜치로 merger**
5. 모든 기능이 merge 된 develop 브랜치를 소스로 한 release 브랜치 - release 브랜치에서는 직접 기능 추가 불가, bug fix만 가능
6. 버그 수정이 완료된 release 브랜치를 main 에 merge(버전 태그 달기)

- 볼드체로 처리된 부분만 수행


## 브랜치 이름 규칙
- 기능 브랜치 : feature/기능을 나타내는 이름
- 버그 수정 브랜치 : bug-fix/#이슈번호

## Docs
[Notion](https://www.notion.so/2025-2-Nest-294052ad29dc80b8a431c70bec1c7d46?source=copy_link)
[Figma](https://www.figma.com/design/AiMOEEkjsHNRulGMNYta4z/SoonEats?node-id=0-1&t=Kx0nFG2bgqm8GwZl-1)
