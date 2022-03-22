<a id="examples-for-aiobotocore-datapipeline-module"></a>

# Examples for aiobotocore DataPipeline module

> [Index](../README.md) > [DataPipeline](./README.md) > Examples

- [Examples for aiobotocore DataPipeline module](#examples-for-aiobotocore-datapipeline-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[datapipeline]` package installed.

Write your `DataPipeline` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type DataPipelineClient
# and provides type checking and code completion
async with session.create_client("datapipeline") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.activate_pipeline()
    

    
    # paginator has type DescribeObjectsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_objects")
    async for item in paginator.paginate(...):
        # item has type DescribeObjectsOutputTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[datapipeline]` or a standalone
`types_aiobotocore_datapipeline` package, you have to explicitly specify
`client: DataPipelineClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_datapipeline.client import DataPipelineClient
from types_aiobotocore_datapipeline.type_defs import Dict[str, Any]
from types_aiobotocore_datapipeline.paginator import DescribeObjectsPaginator

from types_aiobotocore_datapipeline.literals import PaginatorName



session = get_session()

async with session.create_client("datapipeline") as client:
    client: DataPipelineClient

    
    result: Dict[str, Any] = client.activate_pipeline()
    

    
    paginator_name: PaginatorName = "describe_objects"
    paginator: DescribeObjectsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeObjectsOutputTypeDef
        print(item)
    

    
```
