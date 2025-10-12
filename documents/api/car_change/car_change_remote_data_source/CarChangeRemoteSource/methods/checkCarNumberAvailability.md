# Method: `checkCarNumberAvailability`

## Description

# 차량 변경 가능 여부 조회 요청

 ## GET /car-change/check-availability

 ### 요청 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |carNumber|string|차량 번호|

 ### 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |available|bool|차량 변경 가능 여부|

## Return Type
`Future<Either<AppException, bool>>`

## Parameters

- `carNumber`: `String`
