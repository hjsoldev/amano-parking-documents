# Overview for `LeaveDto`

## Description

# 탈퇴 요청

 - POST /leave

 # 탈퇴 요청 응답

 - 응답 파라미터 설명

  |이름|타입|설명|
  |-|-|-|
  |isSuccess|boolean|성공 여부|
  |message|string|메시지|

 - 응답 파라미터 예시

 ```json
 {
   "isSuccess": true,
   "message": "탈퇴 요청이 완료되었습니다."
 }
 ```

## Dependencies

- _$LeaveDto

## Constructors

### Unnamed Constructor


### fromJson


#### Parameters

- `json`: `Map<String, dynamic>`
