# Method: `getEventDetail`

## Description

# 이벤트 상세 요청

 ## GET /event/{id}

 ### 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |id|string|이벤트 ID|
 |title|string|이벤트 제목|
 |content|string|이벤트 내용|
 |status|string|이벤트 상태|
 |startAt|string|이벤트 시작 날짜|
 |endAt|string|이벤트 종료 날짜|
 |createAt|string|이벤트 생성 날짜|

 ### status
 - progress: 진행중
 - closed: 종료
 - always: 상시

## Return Type
`Future<Either<AppException, WrapperDto<EventDetailDto>>>`

## Parameters

- `id`: `String`
