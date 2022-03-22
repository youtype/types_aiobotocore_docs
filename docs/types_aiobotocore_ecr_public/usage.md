<a id="examples-for-aiobotocore-ecrpublic-module"></a>

# Examples for aiobotocore ECRPublic module

> [Index](../README.md) > [ECRPublic](./README.md) > Examples

- [Examples for aiobotocore ECRPublic module](#examples-for-aiobotocore-ecrpublic-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[ecr-public]` package installed.

Write your `ECRPublic` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ECRPublicClient
# and provides type checking and code completion
async with session.create_client("ecr-public") as client:
    
    # result has type BatchCheckLayerAvailabilityResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.batch_check_layer_availability()
    

    
    # paginator has type DescribeImageTagsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_image_tags")
    async for item in paginator.paginate(...):
        # item has type DescribeImageTagsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[ecr-public]` or a standalone
`types_aiobotocore_ecr_public` package, you have to explicitly specify
`client: ECRPublicClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_ecr_public.client import ECRPublicClient
from types_aiobotocore_ecr_public.type_defs import BatchCheckLayerAvailabilityResponseTypeDef
from types_aiobotocore_ecr_public.paginator import DescribeImageTagsPaginator

from types_aiobotocore_ecr_public.literals import PaginatorName



session = get_session()

async with session.create_client("ecr-public") as client:
    client: ECRPublicClient

    
    result: BatchCheckLayerAvailabilityResponseTypeDef = client.batch_check_layer_availability()
    

    
    paginator_name: PaginatorName = "describe_image_tags"
    paginator: DescribeImageTagsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeImageTagsResponseTypeDef
        print(item)
    

    
```
