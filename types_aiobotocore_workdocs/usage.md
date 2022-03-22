<a id="examples-for-aiobotocore-workdocs-module"></a>

# Examples for aiobotocore WorkDocs module

> [Index](../README.md) > [WorkDocs](./README.md) > Examples

- [Examples for aiobotocore WorkDocs module](#examples-for-aiobotocore-workdocs-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[workdocs]` package installed.

Write your `WorkDocs` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type WorkDocsClient
# and provides type checking and code completion
async with session.create_client("workdocs") as client:
    
    # result has type None
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.abort_document_version_upload()
    

    
    # paginator has type DescribeActivitiesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_activities")
    async for item in paginator.paginate(...):
        # item has type DescribeActivitiesResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[workdocs]` or a standalone
`types_aiobotocore_workdocs` package, you have to explicitly specify
`client: WorkDocsClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_workdocs.client import WorkDocsClient
from types_aiobotocore_workdocs.type_defs import None
from types_aiobotocore_workdocs.paginator import DescribeActivitiesPaginator

from types_aiobotocore_workdocs.literals import PaginatorName



session = get_session()

async with session.create_client("workdocs") as client:
    client: WorkDocsClient

    
    result: None = client.abort_document_version_upload()
    

    
    paginator_name: PaginatorName = "describe_activities"
    paginator: DescribeActivitiesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeActivitiesResponseTypeDef
        print(item)
    

    
```
