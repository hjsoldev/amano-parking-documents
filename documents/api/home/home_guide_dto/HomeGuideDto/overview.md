# Overview for `HomeGuideDto`

## Description

# 홈 화면에서 보여지는 가이드 데이터 요청

 - GET /api/home/guide

 # 홈 화면에서 보여지는 가이드 데이터 응답

 - 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |id|string|가이드 고유 아이디|
 |title|string|가이드 타이틀|
 |content|string|가이드 내용|
 |imageUrl|string|가이드 이미지 URL|
 |containerColor|string|가이드 색상(?)|
 |navigation|string|가이드 네비게이션(?)|
 |createAt|string|가이드 생성 날짜|

 - 응답 파라미터 예시

 ```json
 [
   {
     "id": "1",
     "title": "가이드 타이틀",
     "content": "가이드 내용",
     "imageUrl": "https://example.com/image.png",
     "containerColor": "#000000",
     "navigation": "https://example.com/navigation",
     "createAt": "2025-08-20T10:00:00Z"
   },
   {
     "id": "2",
     "title": "가이드 타이틀2",
     "content": "가이드 내용2",
     "imageUrl": "https://example.com/image.png",
     "containerColor": "#000000",
     "navigation": "https://example.com/navigation",
     "createAt": "2025-08-20T10:00:00Z"
   }
 ]
 ```

## Dependencies

- _$HomeGuideDto

## Constructors

### Unnamed Constructor


### _


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`
