# Method: `getNoticeDetail`

## Description

# 공지사항 상세 요청

 ## GET /notice/{id}

 ### 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |id|string|공지사항 ID|
 |title|string|공지사항 제목|
 |author|string|공지사항 작성자|
 |content|string|공지사항 내용|
 |createAt|string|공지사항 생성 날짜|

## Return Type
`Future<Either<AppException, WrapperDto<NoticeDetailDto>>>`

## Parameters

- `id`: `String`
