# 查询所有组织层级

#### ```GET /api/hierarchy/all```
##### ```v1.0.0```
无差别的返回系统中的所有组织层级，由客户端自行建立层级结构。

<br />

## 成功响应
### ```Headers```
```Content-Type: application/json;charset=utf-8```

### ```Body```
* ```{object[]}``` 没查到数据应返回空数组
  * ```{integer} id``` 层级ID
  * ```{string} name``` 层级的名称
  * ```{string|null|undefined} parent_id``` 当前层级的父层级id，如果为```null```或```undefined```则代表它是根层

<br />

## 错误代码
全局错误代码参考```global.md```。