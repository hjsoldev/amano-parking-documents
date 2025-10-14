# Method: `submitCarChangeCancelRequest`

## Description

# 차량 변경 취소 요청(작업중)

 ## POST /car-change/cancel

 ### 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |requestId|string|차량 변경 요청 ID|

 ### 응답 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |id|string|차량 변경 요청 ID|

## Return Type
`Future<Either<AppException, CarChangeCancelDto>>`

## Parameters

- `requestId`: `String`
