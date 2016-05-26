### 1. PUT /api/tribe/member/upgrade/:userId

#### Description
upgrade user one level

#### Resource
 > Please look forward to ☺

#### Authorization
must have user's session info,user must be login

#### Path Parameters
|Name|Type|Description| 
|----|---|---|
| userId |number| id of user who upgraded by tribe owner| 

#### PUT Parameters
|Name|Type|Description| 
|----|---|---|
| tribeId |number| tribeId.|

#### Response
Status-code: 200 OK

```json

{   
    code:200,
    msg:'ok',
    data:{}
}
```
 