# Method: `submitCarChangeRequest`

## Description

# 차량 변경 요청(작업중)

 ## PUT /car-change/submit

 ### 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |currentCarNumber|string|현재 차량 번호|
  |newCarNumber|string|변경할 차량 번호|
  |changeDate|string|변경할 날짜 (YYYY-MM-DD)|

 ### 응답 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |id|string|차량 변경 요청 ID|
  |remainCount|int|남은 차량 변경 횟수|

## Return Type
`Future<Either<AppException, CarChangeDto>>`

## Parameters

- `currentCarNumber`: `String`
- `newCarNumber`: `String`
- `changeDate`: `DateTime`
