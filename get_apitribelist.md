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

|Name|Type|Description| 
|----|----|--- | 
| trbeList |   JSON  | details of tribe | 
| workInfo -> workId |   Number  | id of work | 
| workInfo -> workName |   String  | name of work | 
| workInfo -> workPreview |   String  | preview of work(is a cdn url) | 
| workInfo -> viewTimes |   Number  | how many of user has been see the work| 
| workInfo -> attentionTimes |   Number  | how many of user attention the tribe| 
|workInfo -> praiseTimes  |  Number|  how many of user praise the work   |
|workInfo -> userId  |  Number |  user id of the work   |
|workInfo -> userName  |  String |  user name of the work   |
 