# Method: `getRefundableAmount`

## Description

# 환급 가능 금액 조회 요청

 - GET /refund/amount

 - 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |dateTime|String|날짜 시간|
  |ticketId|String|주차권 ID|

 - 요청 파라미터 예시

 ```json
 {
   "dateTime": "2025-01-01",
   "ticketId": "1",
 }
 ```

 # 환급 가능 금액 조회 응답

 ```json
 ['8000000']
 ```

## Return Type
`Future<Either<AppException, WrapperDto<int>>>`

## Parameters

- `dateTime`: `String`
- `ticketId`: `String`
