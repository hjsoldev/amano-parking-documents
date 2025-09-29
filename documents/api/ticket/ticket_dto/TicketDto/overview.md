# Overview for `TicketDto`

## Description

# 내부 정기권 목록 요청

 - GET /tickets/internal

 - 응답 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |id|String|내부 정기권 ID|
  |productName|String|상품명|
  |plotName|String|지점명|
  |dong|String|동|
  |ho|String|호|
  |status|String|상태|

 - status 값
   - completed: 완료
   - rejected: 거절
   - requested: 요청중

 - 요청 파라미터 예시

 ```json
 {
   [
   {
     "id": "1",
     "productName": "1시간권",
     "plotName": "이마트 성수점",
     "dong": "101",
     "ho": "101",
     "status": "completed"
   },
   {
     "id": "2",
     "productName": "1시간권",
     "plotName": "이마트 성수점",
     "dong": "101",
     "ho": "101",
     "status": "progress"
   },
   {
     "id": "3",
     "productName": "1시간권",
     "plotName": "이마트 성수점",
     "dong": "101",
     "ho": "101",
     "status": "rejected"
   }
 ]
 ```

 - status 값
   - completed: 승인완료
   - rejected: 승인거절
   - progress: 승인요청중

 # 내부 정기권 삭제 요청

 - DELETE /tickets/internal/{id}

 - 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |id|String|내부 정기권 ID|

 - 요청 파라미터 예시

 ```json
 {
   "id": "1",
 }
 ```

 - 응답 파라미터 설명

 - content 없음, 결과 값만 사용합니다.

## Dependencies

- _$TicketDto

## Constructors

### Unnamed Constructor


### _


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`
