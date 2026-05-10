# Paginators

> [Index](../README.md) > [ElementalInference](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ElementalInference](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elementalinference.html#elementalinference)
    type annotations stubs module [types-aiobotocore-elementalinference](https://pypi.org/project/types-aiobotocore-elementalinference/).

## ListFeedsPaginator

Type annotations and code completion for `#!python session.create_client("elementalinference").get_paginator("list_feeds")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elementalinference/paginator/ListFeeds.html#ElementalInference.Paginator.ListFeeds)

```python
# ListFeedsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_elementalinference.paginator import ListFeedsPaginator

session = get_session()
async with session.create_client("elementalinference") as client:  # (1)
    paginator: ListFeedsPaginator = client.get_paginator("list_feeds")  # (2)
    async for item in paginator.paginate(...):
        item: ListFeedsResponseTypeDef
        print(item)  # (3)
```

1. client: [ElementalInferenceClient](./client.md)
2. paginator: [ListFeedsPaginator](./paginators.md#listfeedspaginator)
3. item: `AioPageIterator[ListFeedsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFeedsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListFeedsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListFeedsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFeedsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFeedsRequestPaginateTypeDef](./type_defs.md#listfeedsrequestpaginatetypedef)
