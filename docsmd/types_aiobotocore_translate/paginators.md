# Paginators

> [Index](../README.md) > [Translate](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Translate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#translate)
    type annotations stubs module [types-aiobotocore-translate](https://pypi.org/project/types-aiobotocore-translate/).

## ListTerminologiesPaginator

Type annotations and code completion for `#!python session.create_client("translate").get_paginator("list_terminologies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate/paginator/ListTerminologies.html#Translate.Paginator.ListTerminologies)

```python
# ListTerminologiesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_translate.paginator import ListTerminologiesPaginator

session = get_session()
async with session.create_client("translate") as client:  # (1)
    paginator: ListTerminologiesPaginator = client.get_paginator("list_terminologies")  # (2)
    async for item in paginator.paginate(...):
        item: ListTerminologiesResponseTypeDef
        print(item)  # (3)
```

1. client: [TranslateClient](./client.md)
2. paginator: [ListTerminologiesPaginator](./paginators.md#listterminologiespaginator)
3. item: [:material-code-braces: ListTerminologiesResponseTypeDef](./type_defs.md#listterminologiesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTerminologiesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTerminologiesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTerminologiesResponseTypeDef](./type_defs.md#listterminologiesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTerminologiesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTerminologiesRequestPaginateTypeDef](./type_defs.md#listterminologiesrequestpaginatetypedef) 
