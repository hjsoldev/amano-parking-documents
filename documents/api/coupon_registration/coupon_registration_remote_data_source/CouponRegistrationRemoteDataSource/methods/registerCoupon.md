# Method: `registerCoupon`

## Description

# 쿠폰 등록 요청

 ## POST /coupons/register

 ### 요청 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |code|string|쿠폰 코드|

 ### 응답 파라미터 설명

 - content 없음, 결과 값만 사용합니다.

## Return Type
`Future<Either<AppException, WrapperDto<void>>>`

## Parameters

- `code`: `String`
