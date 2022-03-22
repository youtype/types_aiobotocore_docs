<a id="examples-for-aiobotocore-s3outposts-module"></a>

# Examples for aiobotocore S3Outposts module

> [Index](../README.md) > [S3Outposts](./README.md) > Examples

- [Examples for aiobotocore S3Outposts module](#examples-for-aiobotocore-s3outposts-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[s3outposts]` package installed.

Write your `S3Outposts` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type S3OutpostsClient
# and provides type checking and code completion
async with session.create_client("s3outposts") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListEndpointsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_endpoints")
    async for item in paginator.paginate(...):
        # item has type ListEndpointsResultTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[s3outposts]` or a standalone
`types_aiobotocore_s3outposts` package, you have to explicitly specify
`client: S3OutpostsClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_s3outposts.client import S3OutpostsClient
from types_aiobotocore_s3outposts.type_defs import bool
from types_aiobotocore_s3outposts.paginator import ListEndpointsPaginator

from types_aiobotocore_s3outposts.literals import PaginatorName



session = get_session()

async with session.create_client("s3outposts") as client:
    client: S3OutpostsClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_endpoints"
    paginator: ListEndpointsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListEndpointsResultTypeDef
        print(item)
    

    
```
