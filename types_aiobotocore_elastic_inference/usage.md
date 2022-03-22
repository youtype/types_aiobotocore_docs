<a id="examples-for-aiobotocore-elasticinference-module"></a>

# Examples for aiobotocore ElasticInference module

> [Index](../README.md) > [ElasticInference](./README.md) > Examples

- [Examples for aiobotocore ElasticInference module](#examples-for-aiobotocore-elasticinference-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[elastic-inference]` package installed.

Write your `ElasticInference` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ElasticInferenceClient
# and provides type checking and code completion
async with session.create_client("elastic-inference") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type DescribeAcceleratorsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_accelerators")
    async for item in paginator.paginate(...):
        # item has type DescribeAcceleratorsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[elastic-inference]` or a standalone
`types_aiobotocore_elastic_inference` package, you have to explicitly specify
`client: ElasticInferenceClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_elastic_inference.client import ElasticInferenceClient
from types_aiobotocore_elastic_inference.type_defs import bool
from types_aiobotocore_elastic_inference.paginator import DescribeAcceleratorsPaginator

from types_aiobotocore_elastic_inference.literals import PaginatorName



session = get_session()

async with session.create_client("elastic-inference") as client:
    client: ElasticInferenceClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "describe_accelerators"
    paginator: DescribeAcceleratorsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeAcceleratorsResponseTypeDef
        print(item)
    

    
```
