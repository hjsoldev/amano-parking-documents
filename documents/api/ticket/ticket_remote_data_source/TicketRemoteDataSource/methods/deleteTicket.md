# Method: `deleteTicket`

## Description

# 내부 정기권 삭제 요청

 ## DELETE /tickets/{id}

 ### 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |id|String|내부 정기권 ID|

 ### 응답 파라미터 설명

 - content 없음, 결과 값만 사용합니다.

## Return Type
`Future<Either<AppException, WrapperDto<bool>>>`

## Parameters

- `id`: `String`
