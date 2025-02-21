# Examples

> [Index](../README.md) > [SNS](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SNS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#sns)
    type annotations stubs module [types-aiobotocore-sns](https://pypi.org/project/types-aiobotocore-sns/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[sns]` package installed.

Write your `SNS` code as usual,
type checking and code completion should work out of the box.



```python
# SNSClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("sns") as client:  # (1)
    result = await client.add_permission()  # (2)
```

1. client: [SNSClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



```python
# ListEndpointsByPlatformApplicationPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("sns") as client:  # (1)
    paginator = client.get_paginator("list_endpoints_by_platform_application")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SNSClient](./client.md)
2. paginator: [ListEndpointsByPlatformApplicationPaginator](./paginators.md#listendpointsbyplatformapplicationpaginator)
3. item: [:material-code-braces: ListEndpointsByPlatformApplicationResponseTypeDef](./type_defs.md#listendpointsbyplatformapplicationresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[sns]`
or a standalone `types_aiobotocore_sns` package, you have to explicitly specify
`client: SNSClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# SNSClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_sns.client import SNSClient
from types_aiobotocore_sns.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_sns.type_defs import AddPermissionInputTypeDef


session = get_session()

async with session.create_client("sns") as client:
    client: SNSClient
    kwargs: AddPermissionInputTypeDef = {...}
    result: EmptyResponseMetadataTypeDef = await client.add_permission(**kwargs)
```



```python
# ListEndpointsByPlatformApplicationPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_sns.client import SNSClient
from types_aiobotocore_sns.paginator import ListEndpointsByPlatformApplicationPaginator
from types_aiobotocore_sns.type_defs import ListEndpointsByPlatformApplicationResponseTypeDef


session = get_session()

async with session.create_client("sns") as client:
    client: SNSClient
    paginator: ListEndpointsByPlatformApplicationPaginator = client.get_paginator("list_endpoints_by_platform_application")
    async for item in paginator.paginate(...):
        item: ListEndpointsByPlatformApplicationResponseTypeDef
        print(item)
```


