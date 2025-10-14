# Method: `updateRegisteredCar`

## Description

# 차량 대표 차량 설정 요청

 ## PUT /profile/registered-cars/{id}

 ### 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |id|String|차량 ID|

 ### 응답 파라미터 설명

 - content 없음, 결과 값만 사용합니다.

## Return Type
`Future<Either<AppException, WrapperDto<void>>>`

## Parameters

- `id`: `String`
- `carNumber`: `String`
