<a id="examples-for-aiobotocore-mediaconvert-module"></a>

# Examples for aiobotocore MediaConvert module

> [Index](../README.md) > [MediaConvert](./README.md) > Examples

- [Examples for aiobotocore MediaConvert module](#examples-for-aiobotocore-mediaconvert-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[mediaconvert]` package installed.

Write your `MediaConvert` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type MediaConvertClient
# and provides type checking and code completion
async with session.create_client("mediaconvert") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_certificate()
    

    
    # paginator has type DescribeEndpointsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_endpoints")
    async for item in paginator.paginate(...):
        # item has type DescribeEndpointsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[mediaconvert]` or a standalone
`types_aiobotocore_mediaconvert` package, you have to explicitly specify
`client: MediaConvertClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_mediaconvert.client import MediaConvertClient
from types_aiobotocore_mediaconvert.type_defs import Dict[str, Any]
from types_aiobotocore_mediaconvert.paginator import DescribeEndpointsPaginator

from types_aiobotocore_mediaconvert.literals import PaginatorName



session = get_session()

async with session.create_client("mediaconvert") as client:
    client: MediaConvertClient

    
    result: Dict[str, Any] = client.associate_certificate()
    

    
    paginator_name: PaginatorName = "describe_endpoints"
    paginator: DescribeEndpointsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeEndpointsResponseTypeDef
        print(item)
    

    
```
