# Overview for `PlotFacilityOperationDto`

## Description

# 주차장 시설 운영 정보

  |이름|타입|설명|
  |-|-|-|
  |plotAliasNm|string?|주차장 별칭|
  |bildNm|string?|건물 이름|
  |bildForms|arr_string?|건물 형태 목록|
  |plotForms|arr_string?|주차장 형태 목록|
  |useDayWkVal|arr_string?|주차장 이용 요일 목록|
  |usePsblCarKinds|arr_string?|이용 가능 차량 목록|
  |totPakCnt|int?|총 주차 가능 대수|
  |plotImageFls|arr_string?|주차장 이미지 링크 목록|
  |plotAddtCtnts|arr_string?|부가 사항 목록|

 ### bildForms
 - amano: 아마노
 - public: 공공
 - private: 민간
 - mixed: 혼합
 - sub: 서브
 - .....

 ### plotForms
 - machine: 기계식
 - auto: 자동차
 - .....

## Dependencies

- _$PlotFacilityOperationDto

## Constructors

### Unnamed Constructor


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`
