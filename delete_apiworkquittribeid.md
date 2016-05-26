### DELETE /api/work/quit/:tribeId

#### Description
user quit the tribe
#### Resource
 > Please look forward to ☺

#### Authorization
must have user's session info,user must be login

#### Path Parameters
|Name|Type|Description| 
|----|---|---|
| tribeId |number| id of tribe| 


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
        creater_id:'number',
        isCreater:'boolean'
      }]
    }
}
```

|Name|Type|Description| 
|----|----|--- | 
| trbeList |   JSON  | details of tribe | 
| trbeList -> id |   Number  | id of tribe | 
| trbeList -> avatar |   String  | avatar of tribe | 
| trbeList -> create_time |   Number  | 创建部落时候的时间戳 | 
| trbeList -> works_sum |   Number  | 部落里面的所有作品数量 | 
| trbeList -> comment_sum |   Number  | 部落的留言数量| 
|trbeList -> creater_id  |  Number|  部落创建者的id   |
|trbeList -> isCreater  |  Boolean |   自己是不是部落的创建人true表示是  |
 