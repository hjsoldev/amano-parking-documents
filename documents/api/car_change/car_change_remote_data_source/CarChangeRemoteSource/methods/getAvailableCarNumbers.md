# Method: `getAvailableCarNumbers`

## Description

# 차량 변경 가능 차량 번호 조회 요청

 ## GET /car-change/available-cars

 ### 응답 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |carNumbers|string[]|차량 변경 가능 차량 번호 목록|

## Return Type
`Future<Either<AppException, List<String>>>`

