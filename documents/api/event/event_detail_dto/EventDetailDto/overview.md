# Overview for `EventDetailDto`

## Description

# 이벤트 상세 페이지 데이터 요청

 - GET /event/{id}

 # 이벤트 상세 페이지 데이터 응답

 - 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |id|string|이벤트 ID|
 |content|string|이벤트 내용|

 - 응답 파라미터 예시

 ```json
 {
   "id": "123e4567-e89b-12d3-a456-426614174000",
   "content": "이벤트 내용"
 }
 ```

## Dependencies

- _$EventDetailDto

## Constructors

### Unnamed Constructor


### _


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`
