# TeamFinder

- 프로젝트 기간 : 2021/12/13 ~ 2021/12/23

<img src="./readmeImg/main.jpg">

<img src="./readmeImg/writing.jpg">

<img src="./readmeImg/setting.jpg">

<img src="./readmeImg/detail.jpg">


## Git Commit Message Convention

- Feat: 새로운 기능 추가
- Fix: 버그 수정
- Modify: 기존 기능 변경
- Docs: 문서 내용 변경
- Style: 포맷, 세미콜론 수정 등 코드가 아닌 코드 스타일에 관련된 수정
- Refactor: 리팩토링 코드 (기존 기능 및 style 코드 수정)
- Test: 테스트 코드 추가 및 리팩토링 테스트 등
- Chore: build task 수정, package manager configs 수정 등

> Udacity의 깃 스타일 가이드를 참고했습니다. Udacity's git style guide

## API

### GET /api/postings

포스팅 정보 전부 취득

### POST /api/postings

포스팅 추가

**Payload**

```json
{
  "title": "축구 같이 할 사람",
  "city": ["경기도"],
  "sportsType": ["축구"],
  "content": "14:00에 축구 같이 할 사람 연락주세요.",
  "date": "2021-12-13"
}
```

### PATCH /api/postings/:id

특정 포스팅 수정

**Payload**

```json
{
  "title": "축구 같이 할 사람",
  "city": ["서울", "경기도"],
  "sportsType": ["축구"],
  "content": "서울 지역도 같이 구함!",
  "recruit": true
}
```

### DELETE /api/postings/:id

특정 포스팅 삭제

### POST /signin

로그인

**Payload**

```json
{
  "id": "",
  "password": ""
}
```

### POST /signup

회원가입

**Payload**

```json
{
  "id": "",
  "password": ""
}
```
