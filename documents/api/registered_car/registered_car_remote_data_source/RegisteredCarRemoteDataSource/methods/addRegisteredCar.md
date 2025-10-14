# Method: `addRegisteredCar`

## Description

# 차량 등록 요청

 ## POST /profile/registered-cars

 ### 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |carNumber|String|차량 번호|
  |carType|String|차량 타입|
  |nickname|String|차량 별칭|

 ### 응답 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |id|String|차량 ID|
  |carNumber|String|차량 번호|
  |carType|String|차량 타입|
  |nickname|String|차량 별칭|
  |isPrimary|bool|차량 대표 여부|
  |registeredAt|String|차량 등록 일자|

## Return Type
`Future<Either<AppException, WrapperDto<RegisteredCarDto>>>`

## Parameters

- ``: `dynamic`
- ``: `dynamic`
- ``: `dynamic`
