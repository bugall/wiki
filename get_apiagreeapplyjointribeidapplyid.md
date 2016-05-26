### GET /api/tribe/agree/apply/join/:tribeId/:applyId

#### Description
tribe manager agree user to join tribe
#### Resource
 > Please look forward to ☺

#### Authorization
must have user's session info,user must be login

#### Path Parameters
|Name|Type|Description| 
|----|---|---|
| tribeId |number| tribeId| 
| applyId |number| id of user who apply join the tribe| 


#### Response
Status-code: 200 OK

```json

{   
    code:200,
    msg:'ok',
    data:{}
}
```
 