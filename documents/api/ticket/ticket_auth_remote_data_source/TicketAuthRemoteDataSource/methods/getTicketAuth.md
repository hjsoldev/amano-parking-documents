# Method: `getTicketAuth`

## Description

# 내부 정기권 정보 요청

 ## GET /tickets/{plotId}

 ### 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |plotId|String|주차장 ID|

 ### 응답 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |plotId|String|주차장 ID|
  |plotName|String|주차장 이름|
  |plotAddress|String|주차장 주소|
  |status|String|상태|
  |dong|String|설정된 동|
  |ho|String|설정된 호|
  |dongList|arr_String|동 목록|
  |hoList|arr_String|호 목록|
  |documents|arr_String|문서 목록|
  |attachments|arr_String|업로드 된 첨부파일 목록|

 ### status 값
   - available: 승인 요청 가능
   - progress: 승인 요청중
   - completed: 승인 완료 - ?
   - rejected: 승인 거절 - ?

## Return Type
`Future<Either<AppException, WrapperDto<TicketAuthDto>>>`

## Parameters

- `plotId`: `String`
