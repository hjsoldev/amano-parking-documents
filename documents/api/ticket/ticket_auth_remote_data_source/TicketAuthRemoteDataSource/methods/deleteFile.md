# Method: `deleteFile`

## Description

# 내부 정기권 첨부파일 삭제 요청

 ## DELETE /tickets/attachments/{name}

 ### 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |name|String|첨부파일 이름|

 ### 응답 파라미터 설명

 - content 없음, 결과 값만 사용합니다.

## Return Type
`Future<Either<AppException, WrapperDto<void>>>`

## Parameters

- `name`: `String`
