# Examples

> [Index](../README.md) > [DirectoryService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DirectoryService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#directoryservice)
    type annotations stubs module [types-aiobotocore-ds](https://pypi.org/project/types-aiobotocore-ds/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[ds]` package installed.

Write your `DirectoryService` code as usual,
type checking and code completion should work out of the box.



```python
# DirectoryServiceClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ds") as client:  # (1)
    result = await client.accept_shared_directory()  # (2)
```

1. client: [DirectoryServiceClient](./client.md)
2. result: [:material-code-braces: AcceptSharedDirectoryResultTypeDef](./type_defs.md#acceptshareddirectoryresulttypedef) 



```python
# DescribeClientAuthenticationSettingsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ds") as client:  # (1)
    paginator = client.get_paginator("describe_client_authentication_settings")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [DirectoryServiceClient](./client.md)
2. paginator: [DescribeClientAuthenticationSettingsPaginator](./paginators.md#describeclientauthenticationsettingspaginator)
3. item: [:material-code-braces: DescribeClientAuthenticationSettingsResultTypeDef](./type_defs.md#describeclientauthenticationsettingsresulttypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[ds]`
or a standalone `types_aiobotocore_ds` package, you have to explicitly specify
`client: DirectoryServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# DirectoryServiceClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ds.client import DirectoryServiceClient
from types_aiobotocore_ds.type_defs import AcceptSharedDirectoryResultTypeDef
from types_aiobotocore_ds.type_defs import AcceptSharedDirectoryRequestTypeDef


session = get_session()

async with session.create_client("ds") as client:
    client: DirectoryServiceClient
    kwargs: AcceptSharedDirectoryRequestTypeDef = {...}
    result: AcceptSharedDirectoryResultTypeDef = await client.accept_shared_directory(**kwargs)
```



```python
# DescribeClientAuthenticationSettingsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ds.client import DirectoryServiceClient
from types_aiobotocore_ds.paginator import DescribeClientAuthenticationSettingsPaginator
from types_aiobotocore_ds.type_defs import DescribeClientAuthenticationSettingsResultTypeDef


session = get_session()

async with session.create_client("ds") as client:
    client: DirectoryServiceClient
    paginator: DescribeClientAuthenticationSettingsPaginator = client.get_paginator("describe_client_authentication_settings")
    async for item in paginator.paginate(...):
        item: DescribeClientAuthenticationSettingsResultTypeDef
        print(item)
```


