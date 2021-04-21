# 환경 설정
## JDK 설치 
* 버젼 : OpenJDK 11

# To Do List _ REST API

## 목표
* 로그인 기능
* 회원 가입기능
* 리스트 아이템 CRUD
* 리스트 아이템 회원 간 공유 기능

## 진행 상황
### 2021-04-14
* 멤버 CRUD 완료
> Response 구조 일반, 정형화 필요 있음...
>> 기능 별 Http Status 정리 필요
* Item CRUD 구현 필요

### 2021-04-15
* Response 구조 일반화
> 중복 코드 많아서 수정 필요
* Item CRUD 구현 시작
 
### 2021-04-20
* Item CRUD 구현 완료
* Item unit test 구현 완료
* Service Component에서 로직 상 문제가 있을 때 null을 return하던 부분을 예외를 throw하도록 수정
* CustomTooManyRequestsException 추가
> DB 상에서 생길 수 있는 예외 처리

### 2021-04-20
* 로그인한 member의 nick을 가져오는 코드를 controller -> service로 이동
* 로그인이 완료된 nick을 가져오기 때문에 usernick 체크하는 코드 삭제
* Follow CRUD 
