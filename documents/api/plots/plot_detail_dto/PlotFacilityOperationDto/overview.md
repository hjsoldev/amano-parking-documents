# Overview for `PlotFacilityOperationDto`

## Description

# 주차장 시설 운영 정보

 - 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |plotAliasNm|string|주차장 별칭|
 |bildNm|string|건물 이름|
 |bildForms|arr_string|건물 형태 목록|
 |plotForms|arr_string|주차장 형태 목록|
 |useDayWkVal|arr_string|주차장 이용 요일 목록|
 |usePsblCarKinds|arr_string|이용 가능 차량 목록|
 |totPakCnt|int|총 주차 가능 대수|
 |plotImageFls|arr_string|주차장 이미지 링크 목록|
 |plotAddtCtnts|arr_string|부가 사항 목록|

 - 응답 파라미터 예시
 ```json

   "plotAliasNm": "주차장 별칭",
   "bildNm": "건물 이름",
   "bildForms": ["건물형태1", "건물형태2"],
   "plotForms": ["주차형태1", "주차형태2"],
   "useDayWkVal": {"일": "09:00 ~ 18:00", "월": "09:00 ~ 18:00", "화": "09:00 ~ 23:00"},
   "usePsblCarKinds": ["차량종류1", "차량종류2"],
   "totPakCnt": 100,
   "plotImageFls": ["주차장이미지1", "주차장이미지2"],
   "plotAddtCtnts": ["추가정보1", "추가정보2"],
 }
 ```

## Dependencies

- _$PlotFacilityOperationDto

## Constructors

### Unnamed Constructor


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`
