# Paginators

> [Index](../README.md) > [Textract](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Textract](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
    type annotations stubs module [types-aiobotocore-textract](https://pypi.org/project/types-aiobotocore-textract/).

## ListAdapterVersionsPaginator

Type annotations and code completion for `#!python session.create_client("textract").get_paginator("list_adapter_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Paginator.ListAdapterVersions)

```python
# ListAdapterVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_textract.paginator import ListAdapterVersionsPaginator

session = get_session()
async with session.create_client("textract") as client:  # (1)
    paginator: ListAdapterVersionsPaginator = client.get_paginator("list_adapter_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListAdapterVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [TextractClient](./client.md)
2. paginator: [ListAdapterVersionsPaginator](./paginators.md#listadapterversionspaginator)
3. item: [:material-code-braces: ListAdapterVersionsResponseTypeDef](./type_defs.md#listadapterversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAdapterVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AdapterId: str = ...,
    AfterCreationTime: TimestampTypeDef = ...,
    BeforeCreationTime: TimestampTypeDef = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAdapterVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAdapterVersionsResponseTypeDef](./type_defs.md#listadapterversionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAdapterVersionsRequestListAdapterVersionsPaginateTypeDef = {  # (1)
    "AdapterId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAdapterVersionsRequestListAdapterVersionsPaginateTypeDef](./type_defs.md#listadapterversionsrequestlistadapterversionspaginatetypedef) 
## ListAdaptersPaginator

Type annotations and code completion for `#!python session.create_client("textract").get_paginator("list_adapters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Paginator.ListAdapters)

```python
# ListAdaptersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_textract.paginator import ListAdaptersPaginator

session = get_session()
async with session.create_client("textract") as client:  # (1)
    paginator: ListAdaptersPaginator = client.get_paginator("list_adapters")  # (2)
    async for item in paginator.paginate(...):
        item: ListAdaptersResponseTypeDef
        print(item)  # (3)
```

1. client: [TextractClient](./client.md)
2. paginator: [ListAdaptersPaginator](./paginators.md#listadapterspaginator)
3. item: [:material-code-braces: ListAdaptersResponseTypeDef](./type_defs.md#listadaptersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAdaptersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AfterCreationTime: TimestampTypeDef = ...,
    BeforeCreationTime: TimestampTypeDef = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAdaptersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAdaptersResponseTypeDef](./type_defs.md#listadaptersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAdaptersRequestListAdaptersPaginateTypeDef = {  # (1)
    "AfterCreationTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAdaptersRequestListAdaptersPaginateTypeDef](./type_defs.md#listadaptersrequestlistadapterspaginatetypedef) 
