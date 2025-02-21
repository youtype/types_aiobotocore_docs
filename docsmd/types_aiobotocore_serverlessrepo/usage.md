# Examples

> [Index](../README.md) > [ServerlessApplicationRepository](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ServerlessApplicationRepository](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#serverlessapplicationrepository)
    type annotations stubs module [types-aiobotocore-serverlessrepo](https://pypi.org/project/types-aiobotocore-serverlessrepo/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[serverlessrepo]` package installed.

Write your `ServerlessApplicationRepository` code as usual,
type checking and code completion should work out of the box.



```python
# ServerlessApplicationRepositoryClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("serverlessrepo") as client:  # (1)
    result = await client.create_application()  # (2)
```

1. client: [ServerlessApplicationRepositoryClient](./client.md)
2. result: [:material-code-braces: CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef) 



```python
# ListApplicationDependenciesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("serverlessrepo") as client:  # (1)
    paginator = client.get_paginator("list_application_dependencies")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ServerlessApplicationRepositoryClient](./client.md)
2. paginator: [ListApplicationDependenciesPaginator](./paginators.md#listapplicationdependenciespaginator)
3. item: [:material-code-braces: ListApplicationDependenciesResponseTypeDef](./type_defs.md#listapplicationdependenciesresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[serverlessrepo]`
or a standalone `types_aiobotocore_serverlessrepo` package, you have to explicitly specify
`client: ServerlessApplicationRepositoryClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ServerlessApplicationRepositoryClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_serverlessrepo.client import ServerlessApplicationRepositoryClient
from types_aiobotocore_serverlessrepo.type_defs import CreateApplicationResponseTypeDef
from types_aiobotocore_serverlessrepo.type_defs import CreateApplicationRequestTypeDef


session = get_session()

async with session.create_client("serverlessrepo") as client:
    client: ServerlessApplicationRepositoryClient
    kwargs: CreateApplicationRequestTypeDef = {...}
    result: CreateApplicationResponseTypeDef = await client.create_application(**kwargs)
```



```python
# ListApplicationDependenciesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_serverlessrepo.client import ServerlessApplicationRepositoryClient
from types_aiobotocore_serverlessrepo.paginator import ListApplicationDependenciesPaginator
from types_aiobotocore_serverlessrepo.type_defs import ListApplicationDependenciesResponseTypeDef


session = get_session()

async with session.create_client("serverlessrepo") as client:
    client: ServerlessApplicationRepositoryClient
    paginator: ListApplicationDependenciesPaginator = client.get_paginator("list_application_dependencies")
    async for item in paginator.paginate(...):
        item: ListApplicationDependenciesResponseTypeDef
        print(item)
```


