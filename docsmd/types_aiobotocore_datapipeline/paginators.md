# Paginators

> [Index](../README.md) > [DataPipeline](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [DataPipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#datapipeline)
    type annotations stubs module [types-aiobotocore-datapipeline](https://pypi.org/project/types-aiobotocore-datapipeline/).

## DescribeObjectsPaginator

Type annotations and code completion for `#!python session.create_client("datapipeline").get_paginator("describe_objects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline/paginator/DescribeObjects.html#DataPipeline.Paginator.DescribeObjects)

```python
# DescribeObjectsPaginator usage example

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
3. item: `AioPageIterator[DescribeObjectsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeObjectsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    pipelineId: str,
    objectIds: Sequence[str],
    evaluateExpressions: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeObjectsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeObjectsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeObjectsInputPaginateTypeDef = {  # (1)
    "pipelineId": ...,
    "objectIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeObjectsInputPaginateTypeDef](./type_defs.md#describeobjectsinputpaginatetypedef)
## ListPipelinesPaginator

Type annotations and code completion for `#!python session.create_client("datapipeline").get_paginator("list_pipelines")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline/paginator/ListPipelines.html#DataPipeline.Paginator.ListPipelines)

```python
# ListPipelinesPaginator usage example

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
3. item: `AioPageIterator[ListPipelinesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPipelinesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListPipelinesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListPipelinesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPipelinesInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPipelinesInputPaginateTypeDef](./type_defs.md#listpipelinesinputpaginatetypedef)
## QueryObjectsPaginator

Type annotations and code completion for `#!python session.create_client("datapipeline").get_paginator("query_objects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline/paginator/QueryObjects.html#DataPipeline.Paginator.QueryObjects)

```python
# QueryObjectsPaginator usage example

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
3. item: `AioPageIterator[QueryObjectsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python QueryObjectsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    pipelineId: str,
    sphere: str,
    query: QueryTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[QueryObjectsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: QueryTypeDef](./type_defs.md#querytypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[QueryObjectsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: QueryObjectsInputPaginateTypeDef = {  # (1)
    "pipelineId": ...,
    "sphere": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: QueryObjectsInputPaginateTypeDef](./type_defs.md#queryobjectsinputpaginatetypedef)
