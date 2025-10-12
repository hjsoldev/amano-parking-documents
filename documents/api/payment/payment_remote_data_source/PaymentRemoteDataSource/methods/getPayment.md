# Method: `getPayment`

## Description

# 결제 정보 요청

 ## GET /payments/{id}

 ### 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |id|String|상품권 ID|

 ### 응답 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |ppOp|PlotProductOperationDto|상품 정보|
  |pleaseNotes|arr_String|안내 문구|
  |refundNotes|arr_String|환불 문구|

## Return Type
`Future<Either<AppException, PaymentDto>>`

## Parameters

- `ticketId`: `String`
