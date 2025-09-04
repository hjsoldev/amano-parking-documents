# Overview for `CustomerDto`

## Description

# 고객센터 FAQ 데이터 요청

 - GET /faqs

 - 앱 실행시 서버에서 데이타를 받은 후 로컬에 파일 저장
   - 로컬 데이타 저장 파일명: customer_${type}.hashcode
   - 데이타가 변경될 수 있기 때문에 앱 실행시 매번 로컬에 파일 저장(버전 관리 필요?)
   - 검색시 로컬 데이타에서 조회

 # 고객센터 FAQ 데이터 응답

 - 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |id|string|고유 아이디|
 |title|string|타이틀|
 |type|string|타입(탭 메뉴)|
 |content|string|내용|
 |createAt|string|생성 날짜|

 - 응답 파라미터 예시

 ```json
 [
   {
     "id": "123e4567-e89b-12d3-a456-426614174000",
     "title": "이용한 주차 내역",
     "type": "app",
     "content": "이용한 주차 내역",
     "createAt": "2025-08-20T10:00:00Z"
   },
   {
     "id": "123e4567-e89b-12d3-a456-426614174000",
     "title": "이용한 주차 내역",
     "type": "app",
     "content": "이용한 주차 내역",
     "createAt": "2025-08-20T10:00:00Z"
   }
 ]
 ```

 - type 값
   - app: 앱
   - product: 상품
   - refund: 환불
   - member: 회원
   - plots: 주차장

## Dependencies

- _$CustomerDto

## Constructors

### Unnamed Constructor


### _


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`
