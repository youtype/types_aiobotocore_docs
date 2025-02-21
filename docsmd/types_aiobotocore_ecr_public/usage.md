# Examples

> [Index](../README.md) > [ECRPublic](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ECRPublic](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ecrpublic)
    type annotations stubs module [types-aiobotocore-ecr-public](https://pypi.org/project/types-aiobotocore-ecr-public/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[ecr-public]` package installed.

Write your `ECRPublic` code as usual,
type checking and code completion should work out of the box.



```python
# ECRPublicClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ecr-public") as client:  # (1)
    result = await client.batch_check_layer_availability()  # (2)
```

1. client: [ECRPublicClient](./client.md)
2. result: [:material-code-braces: BatchCheckLayerAvailabilityResponseTypeDef](./type_defs.md#batchchecklayeravailabilityresponsetypedef) 



```python
# DescribeImageTagsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ecr-public") as client:  # (1)
    paginator = client.get_paginator("describe_image_tags")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ECRPublicClient](./client.md)
2. paginator: [DescribeImageTagsPaginator](./paginators.md#describeimagetagspaginator)
3. item: [:material-code-braces: DescribeImageTagsResponseTypeDef](./type_defs.md#describeimagetagsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[ecr-public]`
or a standalone `types_aiobotocore_ecr_public` package, you have to explicitly specify
`client: ECRPublicClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ECRPublicClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ecr_public.client import ECRPublicClient
from types_aiobotocore_ecr_public.type_defs import BatchCheckLayerAvailabilityResponseTypeDef
from types_aiobotocore_ecr_public.type_defs import BatchCheckLayerAvailabilityRequestTypeDef


session = get_session()

async with session.create_client("ecr-public") as client:
    client: ECRPublicClient
    kwargs: BatchCheckLayerAvailabilityRequestTypeDef = {...}
    result: BatchCheckLayerAvailabilityResponseTypeDef = await client.batch_check_layer_availability(**kwargs)
```



```python
# DescribeImageTagsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ecr_public.client import ECRPublicClient
from types_aiobotocore_ecr_public.paginator import DescribeImageTagsPaginator
from types_aiobotocore_ecr_public.type_defs import DescribeImageTagsResponseTypeDef


session = get_session()

async with session.create_client("ecr-public") as client:
    client: ECRPublicClient
    paginator: DescribeImageTagsPaginator = client.get_paginator("describe_image_tags")
    async for item in paginator.paginate(...):
        item: DescribeImageTagsResponseTypeDef
        print(item)
```


