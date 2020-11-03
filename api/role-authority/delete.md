# 删除角色的权限

#### ```GET /api/role-authority/delete/:id```
##### ```v1.0.0```

删除某个角色与某个权限的关联关系

<br />

## 请求格式
### ```Path Parameters```
* ```{integer} role_id``` 要删除的角色id
* ```{integer} auth``` 权限值，参考权限标准文件

<br />

## 成功响应
无

<br />

## 错误代码
全局错误代码参考```global.md```。

#### ```ERR_NOT_FOUND```
要删除的角色和对应权限没有找到时设置这个错误。