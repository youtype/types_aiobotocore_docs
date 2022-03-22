<a id="examples-for-aiobotocore-workspaces-module"></a>

# Examples for aiobotocore WorkSpaces module

> [Index](../README.md) > [WorkSpaces](./README.md) > Examples

- [Examples for aiobotocore WorkSpaces module](#examples-for-aiobotocore-workspaces-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[workspaces]` package installed.

Write your `WorkSpaces` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type WorkSpacesClient
# and provides type checking and code completion
async with session.create_client("workspaces") as client:
    
    # result has type AssociateConnectionAliasResultTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_connection_alias()
    

    
    # paginator has type DescribeAccountModificationsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_account_modifications")
    async for item in paginator.paginate(...):
        # item has type DescribeAccountModificationsResultTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[workspaces]` or a standalone
`types_aiobotocore_workspaces` package, you have to explicitly specify
`client: WorkSpacesClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_workspaces.client import WorkSpacesClient
from types_aiobotocore_workspaces.type_defs import AssociateConnectionAliasResultTypeDef
from types_aiobotocore_workspaces.paginator import DescribeAccountModificationsPaginator

from types_aiobotocore_workspaces.literals import PaginatorName



session = get_session()

async with session.create_client("workspaces") as client:
    client: WorkSpacesClient

    
    result: AssociateConnectionAliasResultTypeDef = client.associate_connection_alias()
    

    
    paginator_name: PaginatorName = "describe_account_modifications"
    paginator: DescribeAccountModificationsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeAccountModificationsResultTypeDef
        print(item)
    

    
```
