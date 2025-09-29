# Overview for `TicketAuthDto`

## Description

# 내부 정기권 정보 요청

 - GET /tickets/internal/{plotId}

 - 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |plotId|String|주차장 ID|

 - 요청 파라미터 예시

 ```json
 {
   "plotId": "1",
 }
 ```

 # 내부 정기권 정보 응답

 - 응답 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |plotId|String|주차장 ID|
  |plotName|String|주차장 이름|
  |plotAddress|String|주차장 주소|
  |dongList|arr_String|동 목록|
  |hoList|arr_String|호 목록|
  |documents|arr_String|문서 목록|

 - 응답 파라미터 예시

 ```json
 {
   "plotId": "1",
   "plotName": "주차장 이름",
   "plotAddress": "주차장 주소",
   "dongList": ["1", "2", "3"],
   "hoList": ["101", "102", "103"],
   "documents": ["임대차 계약서", "사업자 등록증", "자동차 등록증", "주민등록등본", "통장 사본", "신분증 사본"],
 }
 ```

 # 내부 정기권 등록 승인 요청

 - POST /tickets/internal

 - 요청 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |plotId|String|주차장 ID|
  |dong|String|동|
  |ho|String|호|
  |documents|arr_document|문서 목록|

 - 요청 파라미터 예시

 ```json
 {
   "plotId": "1",
   "dong": "1",
   "ho": "101",
   "documents":
   [
     {
        "name": "임대차 계약서",
        "file": "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAA..."
     },
     {
        "name": "주민등록등본",
        "file": "data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAAQABA..."
     }
   ]
 }
 ```

## Dependencies

- _$TicketAuthDto

## Constructors

### Unnamed Constructor


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`
