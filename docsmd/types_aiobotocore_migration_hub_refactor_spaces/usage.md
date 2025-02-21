# Examples

> [Index](../README.md) > [MigrationHubRefactorSpaces](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [MigrationHubRefactorSpaces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#migrationhubrefactorspaces)
    type annotations stubs module [types-aiobotocore-migration-hub-refactor-spaces](https://pypi.org/project/types-aiobotocore-migration-hub-refactor-spaces/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[migration-hub-refactor-spaces]` package installed.

Write your `MigrationHubRefactorSpaces` code as usual,
type checking and code completion should work out of the box.



```python
# MigrationHubRefactorSpacesClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("migration-hub-refactor-spaces") as client:  # (1)
    result = await client.create_application()  # (2)
```

1. client: [MigrationHubRefactorSpacesClient](./client.md)
2. result: [:material-code-braces: CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef) 



```python
# ListApplicationsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("migration-hub-refactor-spaces") as client:  # (1)
    paginator = client.get_paginator("list_applications")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [MigrationHubRefactorSpacesClient](./client.md)
2. paginator: [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
3. item: [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[migration-hub-refactor-spaces]`
or a standalone `types_aiobotocore_migration_hub_refactor_spaces` package, you have to explicitly specify
`client: MigrationHubRefactorSpacesClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# MigrationHubRefactorSpacesClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_migration_hub_refactor_spaces.client import MigrationHubRefactorSpacesClient
from types_aiobotocore_migration_hub_refactor_spaces.type_defs import CreateApplicationResponseTypeDef
from types_aiobotocore_migration_hub_refactor_spaces.type_defs import CreateApplicationRequestTypeDef


session = get_session()

async with session.create_client("migration-hub-refactor-spaces") as client:
    client: MigrationHubRefactorSpacesClient
    kwargs: CreateApplicationRequestTypeDef = {...}
    result: CreateApplicationResponseTypeDef = await client.create_application(**kwargs)
```



```python
# ListApplicationsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_migration_hub_refactor_spaces.client import MigrationHubRefactorSpacesClient
from types_aiobotocore_migration_hub_refactor_spaces.paginator import ListApplicationsPaginator
from types_aiobotocore_migration_hub_refactor_spaces.type_defs import ListApplicationsResponseTypeDef


session = get_session()

async with session.create_client("migration-hub-refactor-spaces") as client:
    client: MigrationHubRefactorSpacesClient
    paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
    async for item in paginator.paginate(...):
        item: ListApplicationsResponseTypeDef
        print(item)
```


