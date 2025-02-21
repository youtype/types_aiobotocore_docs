# Examples

> [Index](../README.md) > [AppIntegrationsService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AppIntegrationsService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#appintegrationsservice)
    type annotations stubs module [types-aiobotocore-appintegrations](https://pypi.org/project/types-aiobotocore-appintegrations/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[appintegrations]` package installed.

Write your `AppIntegrationsService` code as usual,
type checking and code completion should work out of the box.



```python
# AppIntegrationsServiceClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("appintegrations") as client:  # (1)
    result = await client.create_application()  # (2)
```

1. client: [AppIntegrationsServiceClient](./client.md)
2. result: [:material-code-braces: CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef) 



```python
# ListApplicationAssociationsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("appintegrations") as client:  # (1)
    paginator = client.get_paginator("list_application_associations")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [AppIntegrationsServiceClient](./client.md)
2. paginator: [ListApplicationAssociationsPaginator](./paginators.md#listapplicationassociationspaginator)
3. item: [:material-code-braces: ListApplicationAssociationsResponseTypeDef](./type_defs.md#listapplicationassociationsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[appintegrations]`
or a standalone `types_aiobotocore_appintegrations` package, you have to explicitly specify
`client: AppIntegrationsServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# AppIntegrationsServiceClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_appintegrations.client import AppIntegrationsServiceClient
from types_aiobotocore_appintegrations.type_defs import CreateApplicationResponseTypeDef
from types_aiobotocore_appintegrations.type_defs import CreateApplicationRequestTypeDef


session = get_session()

async with session.create_client("appintegrations") as client:
    client: AppIntegrationsServiceClient
    kwargs: CreateApplicationRequestTypeDef = {...}
    result: CreateApplicationResponseTypeDef = await client.create_application(**kwargs)
```



```python
# ListApplicationAssociationsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_appintegrations.client import AppIntegrationsServiceClient
from types_aiobotocore_appintegrations.paginator import ListApplicationAssociationsPaginator
from types_aiobotocore_appintegrations.type_defs import ListApplicationAssociationsResponseTypeDef


session = get_session()

async with session.create_client("appintegrations") as client:
    client: AppIntegrationsServiceClient
    paginator: ListApplicationAssociationsPaginator = client.get_paginator("list_application_associations")
    async for item in paginator.paginate(...):
        item: ListApplicationAssociationsResponseTypeDef
        print(item)
```


