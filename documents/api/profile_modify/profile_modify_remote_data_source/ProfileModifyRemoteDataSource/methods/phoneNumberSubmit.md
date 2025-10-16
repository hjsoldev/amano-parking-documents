# Method: `phoneNumberSubmit`

## Description

# 전화번호 변경 요청

 ## PUT /profile/modify/phone-number

 ### 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |phoneNumber|String|전화번호|

 ### 응답 파라미터 설명

 - content 없음, 결과 값만 사용합니다.

## Return Type
`Future<Either<AppException, WrapperDto<void>>>`

## Parameters

- `phoneNumber`: `String`
