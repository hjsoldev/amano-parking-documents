# Method: `getFavorites`

## Description

# 즐겨찾기 목록 데이타 예시

 ```json
 {
   "success": true,
   "message": "success",
   "meta": {
     "total": 4,
     "page": 1,
     "size": 10
   },
   "contents": [
     {
       "plotId": "1",
       "plotNm": "카페",
       "addr": "서울특별시 강남구 역삼동 123-45",
       "lngt": 126.9779,
       "ltd": 37.5683,
       "pfOp": {
         "bildForms": ["amano", "auto"],
       }
     },
     ...
   ]
 }
 ```

## Return Type
`Future<Either<AppException, WrapperDto<PlotDto>>>`

