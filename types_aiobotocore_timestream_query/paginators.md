<a id="paginators-for-aiobotocore-timestreamquery-module"></a>

# Paginators for aiobotocore TimestreamQuery module

> [Index](..) > [TimestreamQuery](.) > Paginators

Auto-generated documentation for
[TimestreamQuery](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
type annotations stubs module
[types-aiobotocore-timestream-query](https://pypi.org/project/types-aiobotocore-timestream-query/).

- [Paginators for aiobotocore TimestreamQuery module](#paginators-for-aiobotocore-timestreamquery-module)
  - [ListScheduledQueriesPaginator](#listscheduledqueriespaginator)
  - [ListTagsForResourcePaginator](#listtagsforresourcepaginator)
  - [QueryPaginator](#querypaginator)

<a id="listscheduledqueriespaginator"></a>

## ListScheduledQueriesPaginator

Type annotations for
`session.create_client("timestream-query").get_paginator("list_scheduled_queries")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_timestream_query.paginator import ListScheduledQueriesPaginator

session = get_session()
async with session.create_client("timestream-query") as client:
    client: TimestreamQueryClient
    paginator: ListScheduledQueriesPaginator = client.get_paginator("list_scheduled_queries")
```

Boto3 documentation:
[TimestreamQuery.Paginator.ListScheduledQueries](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.ListScheduledQueries)

Arguments for `ListScheduledQueriesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListScheduledQueriesPaginator.paginate` returns
`AsyncIterable`\[[ListScheduledQueriesResponseTypeDef](./type_defs.md#listscheduledqueriesresponsetypedef)\].

<a id="listtagsforresourcepaginator"></a>

## ListTagsForResourcePaginator

Type annotations for
`session.create_client("timestream-query").get_paginator("list_tags_for_resource")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_timestream_query.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("timestream-query") as client:
    client: TimestreamQueryClient
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
```

Boto3 documentation:
[TimestreamQuery.Paginator.ListTagsForResource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.ListTagsForResource)

Arguments for `ListTagsForResourcePaginator.paginate` method:

- `ResourceARN`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTagsForResourcePaginator.paginate` returns
`AsyncIterable`\[[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)\].

<a id="querypaginator"></a>

## QueryPaginator

Type annotations for
`session.create_client("timestream-query").get_paginator("query")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_timestream_query.paginator import QueryPaginator

session = get_session()
async with session.create_client("timestream-query") as client:
    client: TimestreamQueryClient
    paginator: QueryPaginator = client.get_paginator("query")
```

Boto3 documentation:
[TimestreamQuery.Paginator.Query](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.Query)

Arguments for `QueryPaginator.paginate` method:

- `QueryString`: `str` *(required)*
- `ClientToken`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`QueryPaginator.paginate` returns
`AsyncIterable`\[[QueryResponseTypeDef](./type_defs.md#queryresponsetypedef)\].
