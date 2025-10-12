# Method: `submitCancel`

## Description

# 내부 정기권 승인 취소 요청

 ## DELETE /tickets/cancel/{plotId}

 ### 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |plotId|String|주차장 ID|

 ### 응답 파라미터 설명

 - content 없음, 결과 값만 사용합니다.

## Return Type
`Future<Either<AppException, WrapperDto<void>>>`

## Parameters

- `plotId`: `String`
