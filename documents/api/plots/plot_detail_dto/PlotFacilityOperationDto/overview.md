# Overview for `PlotFacilityOperationDto`

## Description

# 주차장 시설 운영 정보

 - 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |plotAliasNm|string|주차장 별칭|
 |bildNm|string|건물 이름|
 |bildForms|arr_string|건물 형태|
 |plotForms|arr_string|주차장 형태|
 |useDayWkVal|string|사용 요일 코드|
 |useStrTm|string|사용 시작 시간|
 |useEndTm|string|사용 종료 시간|
 |usePsblCarKinds|arr_string|사용 가능 차량 종류|
 |totPakCnt|int|총 주차 가능 차량 수|
 |plotImageFls|arr_string|주차장 이미지 파일 리스트|
 |plotAddtCtnts|arr_string|주차장 추가 정보|

 - 응답 파라미터 예시
 ```json

   "plotAliasNm": "주차장 별칭",
   "bildNm": "건물 이름",
   "bildForms": ["건물형태1", "건물형태2"],
   "plotForms": ["주차형태1", "주차형태2"],
   "useDayWkVal": "1",
   "useStrTm": "09:00",
   "useEndTm": "18:00",
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
