### POST /api/tribe/work/:tribeId

#### Description
add work to tribe
#### Resource
 > Please look forward to ☺

#### Authorization
must have user's session info,user must be login

#### Path Parameters
|Name|Type|Description| 
|----|---|---|
| tribeId |number| tribeId| 

#### POST Parameters
|Name|Type|Description| 
|----|---|---|
| workId |number| which work do you want to add|


#### Response
Status-code: 200 OK

```json

{   
    code:200,
    msg:'ok',
    data:{}
}
```
 