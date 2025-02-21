# Examples

> [Index](../README.md) > [CodeGuruReviewer](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CodeGuruReviewer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#codegurureviewer)
    type annotations stubs module [types-aiobotocore-codeguru-reviewer](https://pypi.org/project/types-aiobotocore-codeguru-reviewer/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[codeguru-reviewer]` package installed.

Write your `CodeGuruReviewer` code as usual,
type checking and code completion should work out of the box.



```python
# CodeGuruReviewerClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("codeguru-reviewer") as client:  # (1)
    result = await client.associate_repository()  # (2)
```

1. client: [CodeGuruReviewerClient](./client.md)
2. result: [:material-code-braces: AssociateRepositoryResponseTypeDef](./type_defs.md#associaterepositoryresponsetypedef) 



```python
# ListRepositoryAssociationsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("codeguru-reviewer") as client:  # (1)
    paginator = client.get_paginator("list_repository_associations")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CodeGuruReviewerClient](./client.md)
2. paginator: [ListRepositoryAssociationsPaginator](./paginators.md#listrepositoryassociationspaginator)
3. item: [:material-code-braces: ListRepositoryAssociationsResponseTypeDef](./type_defs.md#listrepositoryassociationsresponsetypedef) 



```python
# CodeReviewCompletedWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("codeguru-reviewer") as client:  # (1)
    waiter = client.get_waiter("code_review_completed")  # (2)
    await waiter.wait()
```

1. client: [CodeGuruReviewerClient](./client.md)
2. waiter: [CodeReviewCompletedWaiter](./waiters.md#codereviewcompletedwaiter)


### Explicit type annotations

With `types-aiobotocore-lite[codeguru-reviewer]`
or a standalone `types_aiobotocore_codeguru_reviewer` package, you have to explicitly specify
`client: CodeGuruReviewerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# CodeGuruReviewerClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_codeguru_reviewer.client import CodeGuruReviewerClient
from types_aiobotocore_codeguru_reviewer.type_defs import AssociateRepositoryResponseTypeDef
from types_aiobotocore_codeguru_reviewer.type_defs import AssociateRepositoryRequestTypeDef


session = get_session()

async with session.create_client("codeguru-reviewer") as client:
    client: CodeGuruReviewerClient
    kwargs: AssociateRepositoryRequestTypeDef = {...}
    result: AssociateRepositoryResponseTypeDef = await client.associate_repository(**kwargs)
```



```python
# ListRepositoryAssociationsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_codeguru_reviewer.client import CodeGuruReviewerClient
from types_aiobotocore_codeguru_reviewer.paginator import ListRepositoryAssociationsPaginator
from types_aiobotocore_codeguru_reviewer.type_defs import ListRepositoryAssociationsResponseTypeDef


session = get_session()

async with session.create_client("codeguru-reviewer") as client:
    client: CodeGuruReviewerClient
    paginator: ListRepositoryAssociationsPaginator = client.get_paginator("list_repository_associations")
    async for item in paginator.paginate(...):
        item: ListRepositoryAssociationsResponseTypeDef
        print(item)
```



```python
# CodeReviewCompletedWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_codeguru_reviewer.client import CodeGuruReviewerClient
from types_aiobotocore_codeguru_reviewer.waiter import CodeReviewCompletedWaiter


session = get_session()

async with session.create_client("codeguru-reviewer") as client:
    client: CodeGuruReviewerClient
    waiter: CodeReviewCompletedWaiter = client.get_waiter("code_review_completed")
    await waiter.wait()
```
