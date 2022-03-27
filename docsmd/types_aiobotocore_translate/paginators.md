# Paginators

> [Index](../README.md) > [Translate](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Translate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
    type annotations stubs module [types-aiobotocore-translate](https://pypi.org/project/types-aiobotocore-translate/).

## ListTerminologiesPaginator

Type annotations and code completion for `#!python session.create_client("translate").get_paginator("list_terminologies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Paginator.ListTerminologies)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_translate.paginator import ListTerminologiesPaginator

session = get_session()
async with session.create_client("translate") as client:
    client: TranslateClient
    paginator: ListTerminologiesPaginator = client.get_paginator("list_terminologies")
```


### paginate

Type annotations and code completion for `#!python ListTerminologiesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTerminologiesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTerminologiesResponseTypeDef](./type_defs.md#listterminologiesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTerminologiesRequestListTerminologiesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTerminologiesRequestListTerminologiesPaginateTypeDef](./type_defs.md#listterminologiesrequestlistterminologiespaginatetypedef) 
