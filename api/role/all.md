# 查询所有角色

#### ```GET /api/role/all```
##### ```v1.0.0```
返回所有角色和角色id

<br />

## 成功响应
### ```Headers```
```Content-Type: application/json;charset=utf-8```

### ```Body```
* ```{object[]}``` 没查到数据应返回空数组
  * ```{integer} id``` 角色ID
  * ```{string} name``` 角色名称


<br />

## 错误代码
全局错误代码参考```global.md```。