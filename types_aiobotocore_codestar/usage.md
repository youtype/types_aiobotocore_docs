<a id="examples-for-aiobotocore-codestar-module"></a>

# Examples for aiobotocore CodeStar module

> [Index](../README.md) > [CodeStar](./README.md) > Examples

- [Examples for aiobotocore CodeStar module](#examples-for-aiobotocore-codestar-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[codestar]` package installed.

Write your `CodeStar` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type CodeStarClient
# and provides type checking and code completion
async with session.create_client("codestar") as client:
    
    # result has type AssociateTeamMemberResultTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_team_member()
    

    
    # paginator has type ListProjectsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_projects")
    async for item in paginator.paginate(...):
        # item has type ListProjectsResultTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[codestar]` or a standalone
`types_aiobotocore_codestar` package, you have to explicitly specify
`client: CodeStarClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_codestar.client import CodeStarClient
from types_aiobotocore_codestar.type_defs import AssociateTeamMemberResultTypeDef
from types_aiobotocore_codestar.paginator import ListProjectsPaginator

from types_aiobotocore_codestar.literals import PaginatorName



session = get_session()

async with session.create_client("codestar") as client:
    client: CodeStarClient

    
    result: AssociateTeamMemberResultTypeDef = client.associate_team_member()
    

    
    paginator_name: PaginatorName = "list_projects"
    paginator: ListProjectsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListProjectsResultTypeDef
        print(item)
    

    
```
