# Examples

> [Index](../README.md) > [IoTFleetHub](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IoTFleetHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#iotfleethub)
    type annotations stubs module [types-aiobotocore-iotfleethub](https://pypi.org/project/types-aiobotocore-iotfleethub/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[iotfleethub]` package installed.

Write your `IoTFleetHub` code as usual,
type checking and code completion should work out of the box.



```python
# IoTFleetHubClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("iotfleethub") as client:  # (1)
    result = await client.create_application()  # (2)
```

1. client: [IoTFleetHubClient](./client.md)
2. result: [:material-code-braces: CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef) 



```python
# ListApplicationsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("iotfleethub") as client:  # (1)
    paginator = client.get_paginator("list_applications")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [IoTFleetHubClient](./client.md)
2. paginator: [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
3. item: [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[iotfleethub]`
or a standalone `types_aiobotocore_iotfleethub` package, you have to explicitly specify
`client: IoTFleetHubClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# IoTFleetHubClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_iotfleethub.client import IoTFleetHubClient
from types_aiobotocore_iotfleethub.type_defs import CreateApplicationResponseTypeDef
from types_aiobotocore_iotfleethub.type_defs import CreateApplicationRequestTypeDef


session = get_session()

async with session.create_client("iotfleethub") as client:
    client: IoTFleetHubClient
    kwargs: CreateApplicationRequestTypeDef = {...}
    result: CreateApplicationResponseTypeDef = await client.create_application(**kwargs)
```



```python
# ListApplicationsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_iotfleethub.client import IoTFleetHubClient
from types_aiobotocore_iotfleethub.paginator import ListApplicationsPaginator
from types_aiobotocore_iotfleethub.type_defs import ListApplicationsResponseTypeDef


session = get_session()

async with session.create_client("iotfleethub") as client:
    client: IoTFleetHubClient
    paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
    async for item in paginator.paginate(...):
        item: ListApplicationsResponseTypeDef
        print(item)
```


