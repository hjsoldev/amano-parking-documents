# Overview for `PlotOperationDto`

## Description

# 주차장 운영 정보 응답

 - 응답 파라미터 설명

 |이름|타입|설명|
 |-|-|-|
 |fstMin|int|첫 시간 최소 분|
 |fstAmt|int|첫 시간 요금|
 |addChrgMin|int|추가 시간 최소 분|
 |addChrgAmt|int|추가 시간 요금|
 |maxAmt|int|최대 요금|
 |rndMin|int|라운드 시간 최소 분|
 |poutPpmMin|int|출차 판매율 최소 분|
 |dtlGid|string|주차장 고유 아이디|

 - 응답 파라미터 예시
 ```json
 {
   "fstMin": 10,
   "fstAmt": 1000,
   "addChrgMin": 10,
   "addChrgAmt": 1000,
   "maxAmt": 10000,
   "rndMin": 10,
   "poutPpmMin": 10,
   "dtlGid": "1234567890",
 }

 ```

## Dependencies

- _$PlotOperationDto

## Constructors

### Unnamed Constructor


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`
