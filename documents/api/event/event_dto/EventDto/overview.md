# Overview for `EventDto`

## Description

# 이벤트 목록 요청

 - GET /event

 # 이벤트 목록 응답

 - 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |id|string|이벤트 ID|
 |title|string|이벤트 제목|
 |status|string|이벤트 상태|
 |startAt|string|이벤트 시작 날짜|
 |endAt|string|이벤트 종료 날짜|
 |createAt|string|이벤트 생성 날짜|

 - 응답 파라미터 예시

 ```json
 [
 {

     "id": "1",
     "title": "이벤트 제목1",
     "status": "progress"
     "startAt": "2025-08-20T10:00:00Z",
     "endAt": "2025-08-20T10:00:00Z",
     "createAt": "2025-08-20T10:00:00Z",
   },
   {
     "id": "2",
     "title": "이벤트 제목2",
     "status": "closed"
     "startAt": "2025-08-20T10:00:00Z",
     "endAt": "2025-08-20T10:00:00Z",
     "createAt": "2025-08-20T10:00:00Z",
   },
 ]
 ```

 - status 값
   - progress: 진행중
   - closed: 종료
   - always: 상시

## Dependencies

- _$EventDto

## Constructors

### Unnamed Constructor


### _


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`
