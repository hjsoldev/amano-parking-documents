# Method: `submitRefund`

## Description

# 환불 요청

 - POST /refund

 - 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |plotId|String|주차장 ID|
  |ticketId|String|주차권 ID|
  |refundDate|DateTime|환불 일자|
  |refundableAmount|int|환불 가능 금액|
  |refundReason|String|환불 사유|

 - 요청 파라미터 예시

 ```json
 {
   "plotId": "1",
   "ticketId": "1",
   "refundDate": "2025-01-01",
   "refundableAmount": 10000,
   "refundReason": "환불 사유",
 }
 ```

 # 환불 요청 응답

 - contents 결과값 사용

## Return Type
`Future<Either<AppException, WrapperDto<void>>>`

## Parameters

- `plotId`: `String`
- `ticketId`: `String`
- `refundDate`: `DateTime`
- `refundableAmount`: `int`
- `refundReason`: `String`
