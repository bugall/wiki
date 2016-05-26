### DELETE /api/tribe/:tribeId

#### Description
解散部落
#### Resource
 > Please look forward to ☺

#### Authorization
must have user's session info,user must be login
必须是创建人才能解散部落

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
    data:{}
}
```

### Appendix

部落解散会群发消息给关注部落的人和部落成员

 