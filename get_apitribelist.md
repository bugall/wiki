### GET /api/tribe/list

#### Description
get all tribe that i join
#### Resource
 > Please look forward to ☺

#### Authorization
must have user's session info,user must be login

#### Path Parameters


#### Response
Status-code: 200 OK

```json

{   
    code:200,
    msg:'ok',
    data:{
      trbeList:[{
        id:'number',
        avatar:'string',
        create_time:'number',
        works_sum:'number',
        comment_sum:'number',
        creater_id:'number'
      }]
    }
}
```
 