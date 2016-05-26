### 1. POST /api/tribe/invita/:tribeId

#### Description
invita user to join tribe

#### Resource
 > Please look forward to ☺

#### Authorization
must have user's session info,user must be login

#### Path Parameters
|Name|Type|Description| 
|----|---|---|
| invitaId |number| id of user who invited by tribe manager| 

#### POST Parameters
|Name|Type|Description| 
|----|---|---|
| tribe_id |number| tribeId.|

#### Response
Status-code: 200 OK

```json

{   
    code:200,
    msg:'ok',
    data:{}
}
```
 
