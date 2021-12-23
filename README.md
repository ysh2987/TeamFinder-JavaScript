# TeamFinder

- 프로젝트 기간 : 2021/12/6 ~ 2021/12/23

<img src="./readmeImg/main.jpg">

<img src="./readmeImg/writing.jpg">

<img src="./readmeImg/setting.jpg">

<img src="./readmeImg/detail.jpg">

## 수정할 사항

- writing Page
  - 기능 구현에 초점이 맞춰져 있어 코드 개선 필요!
  - 이벤트 처리 부분과 서버 통신 코드 각 파일로 분리
- setting Page

  - 코드 리펙토링!!
  - 시간이 부족해 이미지 등록 / 수정 기능 추가
  - 회원 탈퇴시 users 데이터는 삭제되지만 posts 데이터 삭제 안되는 버그 수정 필요

- 공부가 필요한 부분
  - SPA 구축
  - component화
  - Routing
  - 목 서버 구현 express
  - 상태관리

## Memo

- 첫 팀 프로젝트
- 웹 페이지가아닌 웹 어플리케이션

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
