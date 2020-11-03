# 添加一个组织层级

#### ```POST /api/hierarchy/add```
##### ```v1.0.0```
增加一个新的组织层级

<br />

## 请求格式
### ```Headers```
```Content-Type: application/json;charset=utf-8```

### ```Body```
* ```{object}```
  * ```{string} name``` 组织层级的名称
  * ```{string|null|undefined} parent_id``` 父层级ID，如果是```null```或```undefined```代表添加的是根层级

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