# Overview for `EventDetailDto`

## Description

# 이벤트 상세 요청

 - GET /event/{id}

 # 이벤트 상세 응답

 - 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |id|string|이벤트 ID|
 |title|string|이벤트 제목|
 |content|string|이벤트 내용|
 |status|string|이벤트 상태|
 |startAt|string|이벤트 시작 날짜|
 |endAt|string|이벤트 종료 날짜|
 |createAt|string|이벤트 생성 날짜|

 - 응답 파라미터 예시

 ```json
 [
   {
     "id": "1",
     "title": "이벤트 제목",
     "content": "이벤트 내용",
     "status": "progress",
     "startAt": "2025-07-11",
     "endAt": "2025-07-11",
     "createAt": "2025.07.11",
   }
 ]
 ```

## Dependencies

- _$EventDetailDto

## Constructors

### Unnamed Constructor


### _


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`
