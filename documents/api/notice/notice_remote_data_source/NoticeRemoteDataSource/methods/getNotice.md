# Method: `getNotice`

## Description

# 공지사항 목록 요청

 ## GET /notice

 ### 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |id|string|공지사항 ID|
 |title|string|공지사항 제목|
 |author|string|공지사항 작성자|
 |createAt|string|공지사항 생성 날짜|

## Return Type
`Future<Either<AppException, WrapperDto<NoticeDto>>>`

