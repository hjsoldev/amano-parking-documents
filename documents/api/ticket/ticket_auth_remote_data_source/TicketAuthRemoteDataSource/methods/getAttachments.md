# Method: `getAttachments`

## Description

# 내부 정기권 첨부파일 목록 요청

 ## GET /tickets/attachments/{plotId}

 ### 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |plotId|String|주차장 ID|

 ### 응답 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |attachments|arr_String|업로드 된 첨부파일 목록|

## Return Type
`Future<Either<AppException, WrapperDto<String>>>`

## Parameters

- `plotId`: `String`
