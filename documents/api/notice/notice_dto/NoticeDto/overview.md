# Overview for `NoticeDto`

## Description

# 공지사항 목록 요청

 - GET /notice

 # 공지사항 목록 응답

 - 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |id|string|공지사항 ID|
 |title|string|공지사항 제목|
 |author|string|공지사항 작성자|
 |createAt|string|공지사항 생성 날짜|

 - 응답 파라미터 예시

 ```json
 [
   {
     "id": "1",
     "title": "공지사항 제목",
     "author": "공지사항 작성자",
     "createAt": "2025-08-20T10:00:00Z"
   }
 ]
 ```

## Dependencies

- _$NoticeDto

## Constructors

### Unnamed Constructor


### _


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`
