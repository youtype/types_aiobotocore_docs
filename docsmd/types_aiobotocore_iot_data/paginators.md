# Paginators

> [Index](../README.md) > [IoTDataPlane](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [IoTDataPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#iotdataplane)
    type annotations stubs module [types-aiobotocore-iot-data](https://pypi.org/project/types-aiobotocore-iot-data/).

## ListRetainedMessagesPaginator

Type annotations and code completion for `#!python session.create_client("iot-data").get_paginator("list_retained_messages")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data/paginator/ListRetainedMessages.html#IoTDataPlane.Paginator.ListRetainedMessages)

```python
# ListRetainedMessagesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot_data.paginator import ListRetainedMessagesPaginator

session = get_session()
async with session.create_client("iot-data") as client:  # (1)
    paginator: ListRetainedMessagesPaginator = client.get_paginator("list_retained_messages")  # (2)
    async for item in paginator.paginate(...):
        item: ListRetainedMessagesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTDataPlaneClient](./client.md)
2. paginator: [ListRetainedMessagesPaginator](./paginators.md#listretainedmessagespaginator)
3. item: [:material-code-braces: ListRetainedMessagesResponseTypeDef](./type_defs.md#listretainedmessagesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRetainedMessagesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListRetainedMessagesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRetainedMessagesResponseTypeDef](./type_defs.md#listretainedmessagesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRetainedMessagesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRetainedMessagesRequestPaginateTypeDef](./type_defs.md#listretainedmessagesrequestpaginatetypedef) 
