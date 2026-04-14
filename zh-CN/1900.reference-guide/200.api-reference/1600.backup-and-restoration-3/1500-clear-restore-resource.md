|slug|1500-clear-restore-resource|
|---|---|

清空已添加的恢复资源
==============================


功能说明
-------------------------

该接口用于清空已添加的恢复资源路径。

调用说明
-------------------------

### 接口约束
无


### 请求路径
`POST /api/v2/ob/backup/restore/clearRestoreSource`


### 请求参数
| 参数 | 类型 | 必选 | 示例值 | 描述 |
| --- | --- | --- | --- | --- |
| restoreClusterId | Integer | 是 | 1001 | 恢复时的目标集群的 ID。 |



### 返回结果
| 参数 | 类型 | 说明 |
| --- | --- | --- |
| successful | Boolean | 请求是否成功。 |
| timestamp | Datetime | 服务端完成请求的时间戳。 |
| duration | Integer | 服务端处理请求的时间（毫秒）。 |
| status | Integer | 符合 HTTP Status 规范的编码。 |
| traceId | String | 请求的 Trace Id，用于排查问题。 |
| server | String | 响应请求的应用服务的地址。 |


示例
-----------------------

### 请求示例
```json
restoreClusterId:14
```


### 返回示例
```json
{
    "duration": 32,
    "server": "d21b8dbaea",
    "status": 200,
    "successful": true,
    "timestamp": "2024-04-25T19:27:01.66+08:00",
    "traceId": "a5f6ea4f0a294eb7"
}
```

