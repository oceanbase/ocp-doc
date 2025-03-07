# Clear added restore resources

## Purpose

You can call this operation to clear the paths of added restore resources.

## Call description

### Limitations

None.

### Request path

`POST /api/v2/ob/backup/restore/clearRestoreSource`

### Request parameters

| Parameter | Type | Required | Example value | Description |
| ----- | ----- | ----- | ----- | ----- |
| restoreClusterId | Integer | Yes | 1001 | The ID of the cluster to restore.  |

### Response parameters

| Parameter | Type | Description |
| ----- | ----- | ----- |
| successful | Boolean | Indicates whether the request is successful.  |
| timestamp | Datetime | The timestamp when the server completed the request.  |
| duration | Integer | The amount of time taken by the server to process the request, in milliseconds.  |
| status | Integer | The HTTP status code.  |
| traceId | String | The trace ID of the request. This trace ID is used for troubleshooting.  |
| server | String | The address of the application server that responds to the request.  |

## Examples

### Sample request

```json
restoreClusterId:14
```

### Sample response

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
