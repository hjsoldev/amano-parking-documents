# Method: `getBanner`

## Description

# 배너 목록 요청

 ## GET /home/banner/{type}

 ### 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |type|string|배너 타입|

 ### type 값
 - M00: 홈 화면에서 보여지는 큐브 배너
 - M01: 홈 화면에서 보여지는 프로모션 배너
 - M02: 홈 화면에서 보여지는 하단 가이드 배너
 - M03: 이벤트 목록 상단에 보여지는 배너

 ### 응답 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |id|string|배너 고유 아이디|
  |title|string|배너 타이틀|
  |subtitle|string|배너 서브타이틀|
  |imageUrl|string|배너 이미지 URL|
  |linkType|string|이동할 컨텐츠 타입|
  |linkId|string|이동할 컨텐츠 아이디|

 ### linkType
 - event: 이벤트
 - notice: 공지

 ### 확인 필요 사항
 - 배너를 클릭해서 이동할 컨텐츠가 어떤것이 있는지 확인 필요
 - title, subtitle 값은 가이드 배너에 필요 - 이미지라면 해당 컬럼은 삭제

## Return Type
`Future<Either<AppException, WrapperDto<BannerDto>>>`

## Parameters

- `type`: `String`
