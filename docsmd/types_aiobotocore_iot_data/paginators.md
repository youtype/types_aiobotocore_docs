# Paginators

> [Index](../README.md) > [IoTDataPlane](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [IoTDataPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane)
    type annotations stubs module [types-aiobotocore-iot-data](https://pypi.org/project/types-aiobotocore-iot-data/).

## ListRetainedMessagesPaginator

Type annotations and code completion for `#!python session.create_client("iot-data").get_paginator("list_retained_messages")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#IoTDataPlane.Paginator.ListRetainedMessages)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_iot_data.paginator import ListRetainedMessagesPaginator

session = get_session()
async with session.create_client("iot-data") as client:
    client: IoTDataPlaneClient
    paginator: ListRetainedMessagesPaginator = client.get_paginator("list_retained_messages")
```


### paginate

Type annotations and code completion for `#!python ListRetainedMessagesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRetainedMessagesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRetainedMessagesResponseTypeDef](./type_defs.md#listretainedmessagesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRetainedMessagesRequestListRetainedMessagesPaginateTypeDef](./type_defs.md#listretainedmessagesrequestlistretainedmessagespaginatetypedef) 
