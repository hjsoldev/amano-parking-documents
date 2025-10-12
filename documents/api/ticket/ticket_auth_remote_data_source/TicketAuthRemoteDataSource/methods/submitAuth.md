# Method: `submitAuth`

## Description

# 내부 정기권 승인 요청

 ## POST /tickets

 ### 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |plotId|String|주차장 ID|
  |dong|String|동|
  |ho|String|호|
  |attachments|arr_String|업로드 된 첨부파일 목록|

 ### 응답 파라미터 설명

 - content 없음, 결과 값만 사용합니다.

## Return Type
`Future<Either<AppException, WrapperDto<void>>>`

## Parameters

- `plotId`: `String`
- `dong`: `String?`
- `ho`: `String?`
- `attachments`: `List<String>`
