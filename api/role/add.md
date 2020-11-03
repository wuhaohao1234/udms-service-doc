# 添加一个角色

#### ```POST /api/role/add```
##### ```v1.0.0```
增加一个角色

<br />

## 请求格式
### ```Headers```
```Content-Type: application/json;charset=utf-8```

### ```Body```
* ```{object}```
  * ```{string} name``` 角色名称

<br />

## 成功响应
### ```Headers```
```Content-Type: application/json;charset=utf-8```

### ```Body```
* ```{object}```
  * ```{integer} id``` 后端分配的新ID

<br />

## 错误代码
全局错误代码参考```global.md```。