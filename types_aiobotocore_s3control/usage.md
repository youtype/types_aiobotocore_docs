<a id="examples-for-aiobotocore-s3control-module"></a>

# Examples for aiobotocore S3Control module

> [Index](../README.md) > [S3Control](./README.md) > Examples

- [Examples for aiobotocore S3Control module](#examples-for-aiobotocore-s3control-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[s3control]` package installed.

Write your `S3Control` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type S3ControlClient
# and provides type checking and code completion
async with session.create_client("s3control") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListAccessPointsForObjectLambdaPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_access_points_for_object_lambda")
    async for item in paginator.paginate(...):
        # item has type ListAccessPointsForObjectLambdaResultTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[s3control]` or a standalone
`types_aiobotocore_s3control` package, you have to explicitly specify
`client: S3ControlClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_s3control.client import S3ControlClient
from types_aiobotocore_s3control.type_defs import bool
from types_aiobotocore_s3control.paginator import ListAccessPointsForObjectLambdaPaginator

from types_aiobotocore_s3control.literals import PaginatorName



session = get_session()

async with session.create_client("s3control") as client:
    client: S3ControlClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_access_points_for_object_lambda"
    paginator: ListAccessPointsForObjectLambdaPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListAccessPointsForObjectLambdaResultTypeDef
        print(item)
    

    
```
