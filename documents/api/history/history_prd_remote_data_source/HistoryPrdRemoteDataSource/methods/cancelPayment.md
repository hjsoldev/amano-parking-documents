# Method: `cancelPayment`

## Description

# 주차권 구매 내역 취소 요청

 ## POST /history/products/cancel/{id}

 ### 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |id|string|주차권 ID|

 ### 응답 파라미터 설명

 - content 없음, 결과 값만 사용합니다.

## Return Type
`Future<Either<AppException, WrapperDto<void>>>`

## Parameters

- ``: `dynamic`
