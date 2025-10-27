# Greenora

## 커밋 규칙
- 🎉init: 프로젝트 시작
- ✨feat: 새로운 기능 추가, 기존의 기능을 요구 사항에 맞추어 수정 커밋
- 🐛fix: 기능에 대한 버그 수정 커밋
- 🛠️refactor: 기능의 변화가 아닌 코드 리팩터링 ex) 변수 이름 변경
- ✏️chore: 패키지 매니저 수정, 그 외 기타 수정 ex) .gitignore
- 📄docs: 문서(주석) 수정
- 🥂release : 버전 릴리즈



## 브랜치 전략 - Git flow 

[참고 문헌](https://velog.io/@diduya/git-%ED%9A%A8%EC%9C%A8%EC%A0%81%EC%9D%B8-%ED%98%91%EC%97%85%EC%9D%84-%EC%9C%84%ED%95%9C-Git-Flow-%EC%9D%B4%ED%95%B4%ED%95%98%EA%B8%B0-git-branch-repository)

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
