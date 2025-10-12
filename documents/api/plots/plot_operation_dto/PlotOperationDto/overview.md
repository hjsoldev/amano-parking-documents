# Overview for `PlotOperationDto`

## Description

# 주차장 운영 정보

  |이름|타입|설명|
  |-|-|-|
  |fstMin|int?|주차요금 최초 1회차 분|
  |fstAmt|int?|주차요금 최초 1회차 금액|
  |addChrgMin|int?|주차요금 분|
  |addChrgAmt|int?|주차요금 분당 금액|
  |maxAmt|int?|주차요금 일 최대 금액|
  |rndMin|int?|회차시간(분)|
  |poutPpmMin|int?|출차유예시간(분)|
  |dtlGid|string?|주차장 특이 사항 정보|

## Dependencies

- _$PlotOperationDto

## Constructors

### Unnamed Constructor


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`
