# Overview for `HomeCubeDto`

## Description

# 홈 화면에서 보여지는 큐브 데이터 요청

 - GET /home/cube

 # 홈 화면에서 보여지는 큐브 데이터 응답

 - 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |id|string|큐브 고유 아이디|
 |title|string|큐브 타이틀|
 |imageUrl|string|큐브 이미지 URL|
 |createAt|string|큐브 생성 날짜|
 |status|string|큐브 상태(?)|

 - 응답 파라미터 예시

 ```json
 [
   {
     "id": "1",
     "title": "큐브 타이틀1",
     "imageUrl": "https://example.com/image.png",
     "createAt": "2025-08-20T10:00:00Z",
     "status": "completed"
   },
   {
     "id": "2",
     "title": "큐브 타이틀2",
     "imageUrl": "https://example.com/image.png",
     "createAt": "2025-08-20T10:00:00Z",
     "status": "completed"
   }
 ]
 ```

## Dependencies

- _$HomeCubeDto

## Constructors

### Unnamed Constructor


### _


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`
