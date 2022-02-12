<a id="paginators-for-aiobotocore-iotdataplane-module"></a>

# Paginators for aiobotocore IoTDataPlane module

> [Index](..) > [IoTDataPlane](.) > Paginators

Auto-generated documentation for
[IoTDataPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane)
type annotations stubs module
[types-aiobotocore-iot-data](https://pypi.org/project/types-aiobotocore-iot-data/).

- [Paginators for aiobotocore IoTDataPlane module](#paginators-for-aiobotocore-iotdataplane-module)
  - [ListRetainedMessagesPaginator](#listretainedmessagespaginator)

<a id="listretainedmessagespaginator"></a>

## ListRetainedMessagesPaginator

Type annotations for
`session.create_client("iot-data").get_paginator("list_retained_messages")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot_data.paginator import ListRetainedMessagesPaginator

session = get_session()
async with session.create_client("iot-data") as client:
    client: IoTDataPlaneClient
    paginator: ListRetainedMessagesPaginator = client.get_paginator("list_retained_messages")
```

Boto3 documentation:
[IoTDataPlane.Paginator.ListRetainedMessages](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Paginator.ListRetainedMessages)

Arguments for `ListRetainedMessagesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRetainedMessagesPaginator.paginate` returns
`AsyncIterable`\[[ListRetainedMessagesResponseTypeDef](./type_defs.md#listretainedmessagesresponsetypedef)\].
