# Culcom 회원 등록

## API 정보

Method : Post<br>
URL : /users/
Body : {
  "userId" : integer, <br>
  "userName" : string, <br>
  "address" : { <br>
      "country":  string, <br>
      "code" : integer <br>
  }<br>
}<br>

## Sample

Request : Post /users

body : {
 "userId" : 2,
 "userName" : "taerim",
 "address" : {
   "country" : "Japan",
   "code" : 200
 }
}

return 

| status code | 처리기준 |  |
|-------|-------|-------|
| 200   | 성공   |    |
| 400   | 클라이언트 메시지 에러   |    |
| 500   | 서버에러, 재시도   |    |
