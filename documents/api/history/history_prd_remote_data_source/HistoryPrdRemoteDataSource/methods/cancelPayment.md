# Method: `cancelPayment`

## Description

# 상품 구매 취소 요청

 ## POST /history/products/cancel/{id}

 ### 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |id|string|상품 ID|

 ### 응답 파라미터 설명

 - content 없음, 결과 값만 사용합니다.

## Return Type
`Future<Either<AppException, WrapperDto<void>>>`

## Parameters

- ``: `dynamic`
