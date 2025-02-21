# Examples

> [Index](../README.md) > [SMS](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SMS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#sms)
    type annotations stubs module [types-aiobotocore-sms](https://pypi.org/project/types-aiobotocore-sms/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[sms]` package installed.

Write your `SMS` code as usual,
type checking and code completion should work out of the box.



```python
# SMSClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("sms") as client:  # (1)
    result = await client.create_app()  # (2)
```

1. client: [SMSClient](./client.md)
2. result: [:material-code-braces: CreateAppResponseTypeDef](./type_defs.md#createappresponsetypedef) 



```python
# GetConnectorsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("sms") as client:  # (1)
    paginator = client.get_paginator("get_connectors")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SMSClient](./client.md)
2. paginator: [GetConnectorsPaginator](./paginators.md#getconnectorspaginator)
3. item: [:material-code-braces: GetConnectorsResponseTypeDef](./type_defs.md#getconnectorsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[sms]`
or a standalone `types_aiobotocore_sms` package, you have to explicitly specify
`client: SMSClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# SMSClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_sms.client import SMSClient
from types_aiobotocore_sms.type_defs import CreateAppResponseTypeDef
from types_aiobotocore_sms.type_defs import CreateAppRequestTypeDef


session = get_session()

async with session.create_client("sms") as client:
    client: SMSClient
    kwargs: CreateAppRequestTypeDef = {...}
    result: CreateAppResponseTypeDef = await client.create_app(**kwargs)
```



```python
# GetConnectorsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_sms.client import SMSClient
from types_aiobotocore_sms.paginator import GetConnectorsPaginator
from types_aiobotocore_sms.type_defs import GetConnectorsResponseTypeDef


session = get_session()

async with session.create_client("sms") as client:
    client: SMSClient
    paginator: GetConnectorsPaginator = client.get_paginator("get_connectors")
    async for item in paginator.paginate(...):
        item: GetConnectorsResponseTypeDef
        print(item)
```


