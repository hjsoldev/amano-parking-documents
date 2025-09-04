# Overview for `PlotInfoDto`

## Description

# 주차장 정보

 - 응답 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |plotId|string|주차장 ID|
  |plotNm|string|주차장 이름|
  |addr|string|주차장 주소|
  |plotClasGrpCd|string|현장 유형 코드 (판매, 운영, 렌탈, 기타) 공란시 전체 조회|
  |lngt|double|경도|
  |ltd|double|위도|
  |plotTicketName|string?|주차권 이름|
  |plotTicketPrice|int?|주차장 요금|
  |plotTicketType|string?|주차장 타입(주차권, 정기권)|
  |plotStatus|string?|주차장 상태(이용불가, 할인 이벤트, 쿠폰)|
  |plotTagList|string?|주차장 태그(일반, 기계식, 자주식, 리프트, 노상, 복합, 부설주, 전기차 충전)|

 - plotTicketType 값
    - regular:주차권
    - season:정기권
 - plotStatus 값
    - none:상태없음
    - unavailable:이용불가
    - discount:할인 이벤트
    - coupon:쿠폰
 - plotTagList 값
    - none:일반
    - machine:기계식
    - auto:자주식
    - lift:리프트
    - ground:노상
    - mixed:복합
    - sub:부설주
    - electric:전기차 충전

## Dependencies

- _$PlotInfoDto

## Constructors

### Unnamed Constructor


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`
