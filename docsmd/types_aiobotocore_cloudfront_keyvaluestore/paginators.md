# Paginators

> [Index](../README.md) > [CloudFrontKeyValueStore](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CloudFrontKeyValueStore](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront-keyvaluestore.html#cloudfrontkeyvaluestore)
    type annotations stubs module [types-aiobotocore-cloudfront-keyvaluestore](https://pypi.org/project/types-aiobotocore-cloudfront-keyvaluestore/).

## ListKeysPaginator

Type annotations and code completion for `#!python session.create_client("cloudfront-keyvaluestore").get_paginator("list_keys")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront-keyvaluestore/paginator/ListKeys.html#CloudFrontKeyValueStore.Paginator.ListKeys)

```python
# ListKeysPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cloudfront_keyvaluestore.paginator import ListKeysPaginator

session = get_session()
async with session.create_client("cloudfront-keyvaluestore") as client:  # (1)
    paginator: ListKeysPaginator = client.get_paginator("list_keys")  # (2)
    async for item in paginator.paginate(...):
        item: ListKeysResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudFrontKeyValueStoreClient](./client.md)
2. paginator: [ListKeysPaginator](./paginators.md#listkeyspaginator)
3. item: [:material-code-braces: ListKeysResponseTypeDef](./type_defs.md#listkeysresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListKeysPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    KvsARN: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListKeysResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListKeysResponseTypeDef](./type_defs.md#listkeysresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListKeysRequestPaginateTypeDef = {  # (1)
    "KvsARN": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListKeysRequestPaginateTypeDef](./type_defs.md#listkeysrequestpaginatetypedef) 
