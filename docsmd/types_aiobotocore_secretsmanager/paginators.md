# Paginators

> [Index](../README.md) > [SecretsManager](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [SecretsManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#secretsmanager)
    type annotations stubs module [types-aiobotocore-secretsmanager](https://pypi.org/project/types-aiobotocore-secretsmanager/).

## ListSecretsPaginator

Type annotations and code completion for `#!python session.create_client("secretsmanager").get_paginator("list_secrets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager/paginator/ListSecrets.html#SecretsManager.Paginator.ListSecrets)

```python
# ListSecretsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_secretsmanager.paginator import ListSecretsPaginator

session = get_session()
async with session.create_client("secretsmanager") as client:  # (1)
    paginator: ListSecretsPaginator = client.get_paginator("list_secrets")  # (2)
    async for item in paginator.paginate(...):
        item: ListSecretsResponseTypeDef
        print(item)  # (3)
```

1. client: [SecretsManagerClient](./client.md)
2. paginator: [ListSecretsPaginator](./paginators.md#listsecretspaginator)
3. item: [:material-code-braces: ListSecretsResponseTypeDef](./type_defs.md#listsecretsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSecretsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    IncludePlannedDeletion: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    SortOrder: SortOrderTypeType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListSecretsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListSecretsResponseTypeDef](./type_defs.md#listsecretsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSecretsRequestPaginateTypeDef = {  # (1)
    "IncludePlannedDeletion": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSecretsRequestPaginateTypeDef](./type_defs.md#listsecretsrequestpaginatetypedef) 
