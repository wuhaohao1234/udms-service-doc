# 删除某个角色

#### ```GET /api/role/delete/:id```
##### ```v1.0.0```
删除某个角色，如果角色对应有某些权限也一起删除

<br />

## 请求格式
### ```Path Parameters```
* ```{integer} id``` 要删除的角色id

<br />

## 成功响应
无

<br />

## 错误代码
全局错误代码参考```global.md ```。

#### ```ERR_NOT_FOUND```
要删除角色没有找到时设置这个错误。