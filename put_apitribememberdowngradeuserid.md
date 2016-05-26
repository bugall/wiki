### 1. PUT /api/tribe/member/downgrade/:userId

#### Description
downgrade user one level

#### Resource
 > Please look forward to ☺

#### Authorization
must have user's session info,user must be login

#### Path Parameters
|Name|Type|Description| 
|----|---|---|
| userId |number| id of user who downgraded by tribe owner| 

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
 