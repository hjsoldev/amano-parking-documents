# Overview for `CustomerDto`

## Description

# 고객센터 FAQ 요청

 - GET /customers/{type}

 - type값은 /customers/tabs 요청 후 탭 타입 값으로 사용

 # 고객센터 FAQ 응답

 - 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |id|string|아이디|
 |title|string|타이틀|
 |type|string|타입|
 |content|string|내용|
 |createAt|string|생성 날짜|

 - 응답 파라미터 예시

 ```json
 [
   {
     "id": "1",
     "title": "이용한 주차 내역",
     "type": "app",
     "content": "이용한 주차 내역",
     "createAt": "2025-08-20T10:00:00Z"
   },
   {
     "id": "1",
     "title": "이용한 주차 내역",
     "type": "app",
     "content": "이용한 주차 내역",
     "createAt": "2025-08-20T10:00:00Z"
   }
 ]
 ```

## Dependencies

- _$CustomerDto

## Constructors

### Unnamed Constructor


### _


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`
