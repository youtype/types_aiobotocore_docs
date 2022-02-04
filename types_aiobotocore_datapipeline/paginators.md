<a id="paginators-for-aiobotocore-datapipeline-module"></a>

# Paginators for aiobotocore DataPipeline module

> [Index](..) > [DataPipeline](.) > Paginators

Auto-generated documentation for
[DataPipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
type annotations stubs module
[types-aiobotocore-datapipeline](https://pypi.org/project/types-aiobotocore-datapipeline/).

- [Paginators for aiobotocore DataPipeline module](#paginators-for-aiobotocore-datapipeline-module)
  - [DescribeObjectsPaginator](#describeobjectspaginator)
  - [ListPipelinesPaginator](#listpipelinespaginator)
  - [QueryObjectsPaginator](#queryobjectspaginator)

<a id="describeobjectspaginator"></a>

## DescribeObjectsPaginator

Type annotations for
`aiobotocore.create_client("datapipeline").get_paginator("describe_objects")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_datapipeline.paginator import DescribeObjectsPaginator

def get_describe_objects_paginator() -> DescribeObjectsPaginator:
    return Session().create_client("datapipeline").get_paginator("describe_objects")
```

Boto3 documentation:
[DataPipeline.Paginator.DescribeObjects](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.DescribeObjects)

Arguments for `DescribeObjectsPaginator.paginate` method:

- `pipelineId`: `str` *(required)*
- `objectIds`: `Sequence`\[`str`\] *(required)*
- `evaluateExpressions`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeObjectsPaginator.paginate` returns
`_PageIterator`\[[DescribeObjectsOutputTypeDef](./type_defs.md#describeobjectsoutputtypedef)\].

<a id="listpipelinespaginator"></a>

## ListPipelinesPaginator

Type annotations for
`aiobotocore.create_client("datapipeline").get_paginator("list_pipelines")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_datapipeline.paginator import ListPipelinesPaginator

def get_list_pipelines_paginator() -> ListPipelinesPaginator:
    return Session().create_client("datapipeline").get_paginator("list_pipelines")
```

Boto3 documentation:
[DataPipeline.Paginator.ListPipelines](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.ListPipelines)

Arguments for `ListPipelinesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPipelinesPaginator.paginate` returns
`_PageIterator`\[[ListPipelinesOutputTypeDef](./type_defs.md#listpipelinesoutputtypedef)\].

<a id="queryobjectspaginator"></a>

## QueryObjectsPaginator

Type annotations for
`aiobotocore.create_client("datapipeline").get_paginator("query_objects")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_datapipeline.paginator import QueryObjectsPaginator

def get_query_objects_paginator() -> QueryObjectsPaginator:
    return Session().create_client("datapipeline").get_paginator("query_objects")
```

Boto3 documentation:
[DataPipeline.Paginator.QueryObjects](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.QueryObjects)

Arguments for `QueryObjectsPaginator.paginate` method:

- `pipelineId`: `str` *(required)*
- `sphere`: `str` *(required)*
- `query`: [QueryTypeDef](./type_defs.md#querytypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`QueryObjectsPaginator.paginate` returns
`_PageIterator`\[[QueryObjectsOutputTypeDef](./type_defs.md#queryobjectsoutputtypedef)\].
