# Method: `emailCheck`

## Description

# 이메일 중복 확인 요청

 ## GET /profile/modify/email

 ### 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |email|String|이메일|

 ### 응답 파라미터 설명

 - content 없음, 결과 값만 사용합니다.

## Return Type
`Future<Either<AppException, WrapperDto<void>>>`

## Parameters

- `email`: `String`
