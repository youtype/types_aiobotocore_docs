# Paginators

> [Index](../README.md) > [DataPipeline](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [DataPipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
    type annotations stubs module [types-aiobotocore-datapipeline](https://pypi.org/project/types-aiobotocore-datapipeline/).

## DescribeObjectsPaginator

Type annotations and code completion for `#!python session.create_client("datapipeline").get_paginator("describe_objects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.DescribeObjects)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_datapipeline.paginator import DescribeObjectsPaginator

session = get_session()
async with session.create_client("datapipeline") as client:  # (1)
    paginator: DescribeObjectsPaginator = client.get_paginator("describe_objects")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeObjectsOutputTypeDef
        print(item)  # (3)
```

1. client: [DataPipelineClient](./client.md)
2. paginator: [DescribeObjectsPaginator](./paginators.md#describeobjectspaginator)
3. item: [:material-code-braces: DescribeObjectsOutputTypeDef](./type_defs.md#describeobjectsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python DescribeObjectsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    pipelineId: str,
    objectIds: Sequence[str],
    evaluateExpressions: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeObjectsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeObjectsOutputTypeDef](./type_defs.md#describeobjectsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeObjectsInputDescribeObjectsPaginateTypeDef = {  # (1)
    "pipelineId": ...,
    "objectIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeObjectsInputDescribeObjectsPaginateTypeDef](./type_defs.md#describeobjectsinputdescribeobjectspaginatetypedef) 
## ListPipelinesPaginator

Type annotations and code completion for `#!python session.create_client("datapipeline").get_paginator("list_pipelines")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.ListPipelines)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_datapipeline.paginator import ListPipelinesPaginator

session = get_session()
async with session.create_client("datapipeline") as client:  # (1)
    paginator: ListPipelinesPaginator = client.get_paginator("list_pipelines")  # (2)
    async for item in paginator.paginate(...):
        item: ListPipelinesOutputTypeDef
        print(item)  # (3)
```

1. client: [DataPipelineClient](./client.md)
2. paginator: [ListPipelinesPaginator](./paginators.md#listpipelinespaginator)
3. item: [:material-code-braces: ListPipelinesOutputTypeDef](./type_defs.md#listpipelinesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListPipelinesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPipelinesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPipelinesOutputTypeDef](./type_defs.md#listpipelinesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListPipelinesInputListPipelinesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPipelinesInputListPipelinesPaginateTypeDef](./type_defs.md#listpipelinesinputlistpipelinespaginatetypedef) 
## QueryObjectsPaginator

Type annotations and code completion for `#!python session.create_client("datapipeline").get_paginator("query_objects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.QueryObjects)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_datapipeline.paginator import QueryObjectsPaginator

session = get_session()
async with session.create_client("datapipeline") as client:  # (1)
    paginator: QueryObjectsPaginator = client.get_paginator("query_objects")  # (2)
    async for item in paginator.paginate(...):
        item: QueryObjectsOutputTypeDef
        print(item)  # (3)
```

1. client: [DataPipelineClient](./client.md)
2. paginator: [QueryObjectsPaginator](./paginators.md#queryobjectspaginator)
3. item: [:material-code-braces: QueryObjectsOutputTypeDef](./type_defs.md#queryobjectsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python QueryObjectsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    pipelineId: str,
    sphere: str,
    query: QueryTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[QueryObjectsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: QueryTypeDef](./type_defs.md#querytypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: QueryObjectsOutputTypeDef](./type_defs.md#queryobjectsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: QueryObjectsInputQueryObjectsPaginateTypeDef = {  # (1)
    "pipelineId": ...,
    "sphere": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: QueryObjectsInputQueryObjectsPaginateTypeDef](./type_defs.md#queryobjectsinputqueryobjectspaginatetypedef) 
