### 1. PUT /api/tribe/member/downgrade/:userId

#### Description
downgrade user one level

#### Resource
 > Please look forward to ☺

#### Authorization
none

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
 