<a id="examples-for-aiobotocore-serverlessapplicationrepository-module"></a>

# Examples for aiobotocore ServerlessApplicationRepository module

> [Index](../README.md) > [ServerlessApplicationRepository](./README.md) >
> Examples

- [Examples for aiobotocore ServerlessApplicationRepository module](#examples-for-aiobotocore-serverlessapplicationrepository-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[serverlessrepo]` package installed.

Write your `ServerlessApplicationRepository` code as usual, type checking and
code completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ServerlessApplicationRepositoryClient
# and provides type checking and code completion
async with session.create_client("serverlessrepo") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListApplicationDependenciesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_application_dependencies")
    async for item in paginator.paginate(...):
        # item has type ListApplicationDependenciesResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[serverlessrepo]` or a standalone
`types_aiobotocore_serverlessrepo` package, you have to explicitly specify
`client: ServerlessApplicationRepositoryClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_serverlessrepo.client import ServerlessApplicationRepositoryClient
from types_aiobotocore_serverlessrepo.type_defs import bool
from types_aiobotocore_serverlessrepo.paginator import ListApplicationDependenciesPaginator

from types_aiobotocore_serverlessrepo.literals import PaginatorName



session = get_session()

async with session.create_client("serverlessrepo") as client:
    client: ServerlessApplicationRepositoryClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_application_dependencies"
    paginator: ListApplicationDependenciesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListApplicationDependenciesResponseTypeDef
        print(item)
    

    
```
