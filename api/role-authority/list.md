# 查询某个角色所具有的所有权限

#### ```GET /api/role-authority/list```
##### ```v1.0.0```

返回某个角色下的所有权限

<br />

## 请求格式
### ```Headers```
```Content-Type: application/json;charset=utf-8```

### ```Body```
* ```{object}```
  * ```{integer} role_id``` 角色id

## 成功响应
### ```Headers```
```Content-Type: application/json;charset=utf-8```

### ```Body```
* ```{integer[]}``` 没查到数据应返回空数组，其中元素代表权限

<br />

## 错误代码
全局错误代码参考```global.md```。