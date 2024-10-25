# Examples

> [Index](../README.md) > [QBusiness](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [QBusiness](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#QBusiness)
    type annotations stubs module [types-aiobotocore-qbusiness](https://pypi.org/project/types-aiobotocore-qbusiness/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[qbusiness]` package installed.

Write your `QBusiness` code as usual,
type checking and code completion should work out of the box.



```python
# QBusinessClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("qbusiness") as client:  # (1)
    result = await client.batch_delete_document()  # (2)
```

1. client: [QBusinessClient](./client.md)
2. result: [:material-code-braces: BatchDeleteDocumentResponseTypeDef](./type_defs.md#batchdeletedocumentresponsetypedef) 



```python
# GetChatControlsConfigurationPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("qbusiness") as client:  # (1)
    paginator = client.get_paginator("get_chat_controls_configuration")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [QBusinessClient](./client.md)
2. paginator: [GetChatControlsConfigurationPaginator](./paginators.md#getchatcontrolsconfigurationpaginator)
3. item: [:material-code-braces: GetChatControlsConfigurationResponseTypeDef](./type_defs.md#getchatcontrolsconfigurationresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[qbusiness]`
or a standalone `types_aiobotocore_qbusiness` package, you have to explicitly specify
`client: QBusinessClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# QBusinessClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_qbusiness.client import QBusinessClient
from types_aiobotocore_qbusiness.type_defs import BatchDeleteDocumentResponseTypeDef
from types_aiobotocore_qbusiness.type_defs import BatchDeleteDocumentRequestRequestTypeDef


session = get_session()

async with session.create_client("qbusiness") as client:
    client: QBusinessClient
    kwargs: BatchDeleteDocumentRequestRequestTypeDef = {...}
    result: BatchDeleteDocumentResponseTypeDef = await client.batch_delete_document(**kwargs)
```



```python
# GetChatControlsConfigurationPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_qbusiness.client import QBusinessClient
from types_aiobotocore_qbusiness.paginator import GetChatControlsConfigurationPaginator
from types_aiobotocore_qbusiness.type_defs import GetChatControlsConfigurationResponseTypeDef


session = get_session()

async with session.create_client("qbusiness") as client:
    client: QBusinessClient
    paginator: GetChatControlsConfigurationPaginator = client.get_paginator("get_chat_controls_configuration")
    async for item in paginator.paginate(...):
        item: GetChatControlsConfigurationResponseTypeDef
        print(item)
```


