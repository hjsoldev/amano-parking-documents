# Method: `passwordCheck`

## Description

# 현재 비밀번호 확인 요청

 ## GET /profile/modify/password

 ### 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |password|String|비밀번호|

 ### 응답 파라미터 설명

 - content 없음, 결과 값만 사용합니다.

## Return Type
`Future<Either<AppException, WrapperDto<void>>>`

## Parameters

- `password`: `String`
