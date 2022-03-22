<a id="examples-for-aiobotocore-codegurureviewer-module"></a>

# Examples for aiobotocore CodeGuruReviewer module

> [Index](../README.md) > [CodeGuruReviewer](./README.md) > Examples

- [Examples for aiobotocore CodeGuruReviewer module](#examples-for-aiobotocore-codegurureviewer-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[codeguru-reviewer]` package installed.

Write your `CodeGuruReviewer` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type CodeGuruReviewerClient
# and provides type checking and code completion
async with session.create_client("codeguru-reviewer") as client:
    
    # result has type AssociateRepositoryResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_repository()
    

    
    # paginator has type ListRepositoryAssociationsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_repository_associations")
    async for item in paginator.paginate(...):
        # item has type ListRepositoryAssociationsResponseTypeDef
        print(item)
    

    
    # waiter has type CodeReviewCompletedWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("code_review_completed")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[codeguru-reviewer]` or a standalone
`types_aiobotocore_codeguru_reviewer` package, you have to explicitly specify
`client: CodeGuruReviewerClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_codeguru_reviewer.client import CodeGuruReviewerClient
from types_aiobotocore_codeguru_reviewer.type_defs import AssociateRepositoryResponseTypeDef
from types_aiobotocore_codeguru_reviewer.paginator import ListRepositoryAssociationsPaginator
from types_aiobotocore_codeguru_reviewer.waiter import CodeReviewCompletedWaiter
from types_aiobotocore_codeguru_reviewer.literals import PaginatorName
from types_aiobotocore_codeguru_reviewer.literals import WaiterName


session = get_session()

async with session.create_client("codeguru-reviewer") as client:
    client: CodeGuruReviewerClient

    
    result: AssociateRepositoryResponseTypeDef = client.associate_repository()
    

    
    paginator_name: PaginatorName = "list_repository_associations"
    paginator: ListRepositoryAssociationsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListRepositoryAssociationsResponseTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "code_review_completed"
    waiter: CodeReviewCompletedWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
