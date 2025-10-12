# Method: `changeCard`

## Description

# 구독 카드 변경 요청

 ## PUT /subscriptions/card

 ### 요청 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |id|string|아이디|
 |cardId|string|카드 아이디|

 ### 응답 파라미터 설명

 - content 없음, 결과 값만 사용합니다.

## Return Type
`Future<Either<AppException, WrapperDto<void>>>`

## Parameters

- `id`: `String`
- `cardId`: `String`
