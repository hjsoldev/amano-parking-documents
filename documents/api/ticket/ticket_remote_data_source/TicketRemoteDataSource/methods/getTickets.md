# Method: `getTickets`

## Description

# 내부 정기권 목록 요청

 ## GET /tickets

 ### 응답 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |id|String|내부 정기권 ID|
  |productName|String|상품명|
  |plotName|String|지점명|
  |dong|String|동|
  |ho|String|호|
  |lat|double|위도|
  |lng|double|경도|
  |status|String|상태|

 ### status 값
 - completed: 완료
 - rejected: 거절
 - requested: 요청중

## Return Type
`Future<Either<AppException, WrapperDto<TicketDto>>>`

