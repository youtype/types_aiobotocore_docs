# Examples

> [Index](../README.md) > [DataPipeline](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DataPipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#datapipeline)
    type annotations stubs module [types-aiobotocore-datapipeline](https://pypi.org/project/types-aiobotocore-datapipeline/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[datapipeline]` package installed.

Write your `DataPipeline` code as usual,
type checking and code completion should work out of the box.



```python
# DataPipelineClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("datapipeline") as client:  # (1)
    result = await client.create_pipeline()  # (2)
```

1. client: [DataPipelineClient](./client.md)
2. result: [:material-code-braces: CreatePipelineOutputTypeDef](./type_defs.md#createpipelineoutputtypedef) 



```python
# DescribeObjectsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("datapipeline") as client:  # (1)
    paginator = client.get_paginator("describe_objects")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [DataPipelineClient](./client.md)
2. paginator: [DescribeObjectsPaginator](./paginators.md#describeobjectspaginator)
3. item: [:material-code-braces: DescribeObjectsOutputTypeDef](./type_defs.md#describeobjectsoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[datapipeline]`
or a standalone `types_aiobotocore_datapipeline` package, you have to explicitly specify
`client: DataPipelineClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# DataPipelineClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_datapipeline.client import DataPipelineClient
from types_aiobotocore_datapipeline.type_defs import CreatePipelineOutputTypeDef
from types_aiobotocore_datapipeline.type_defs import CreatePipelineInputTypeDef


session = get_session()

async with session.create_client("datapipeline") as client:
    client: DataPipelineClient
    kwargs: CreatePipelineInputTypeDef = {...}
    result: CreatePipelineOutputTypeDef = await client.create_pipeline(**kwargs)
```



```python
# DescribeObjectsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_datapipeline.client import DataPipelineClient
from types_aiobotocore_datapipeline.paginator import DescribeObjectsPaginator
from types_aiobotocore_datapipeline.type_defs import DescribeObjectsOutputTypeDef


session = get_session()

async with session.create_client("datapipeline") as client:
    client: DataPipelineClient
    paginator: DescribeObjectsPaginator = client.get_paginator("describe_objects")
    async for item in paginator.paginate(...):
        item: DescribeObjectsOutputTypeDef
        print(item)
```


