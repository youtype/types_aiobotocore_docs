# Paginators

> [Index](../README.md) > [SecretsManager](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [SecretsManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
    type annotations stubs module [types-aiobotocore-secretsmanager](https://pypi.org/project/types-aiobotocore-secretsmanager/).

## ListSecretsPaginator

Type annotations and code completion for `#!python session.create_client("secretsmanager").get_paginator("list_secrets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Paginator.ListSecrets)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_secretsmanager.paginator import ListSecretsPaginator

session = get_session()
async with session.create_client("secretsmanager") as client:
    client: SecretsManagerClient
    paginator: ListSecretsPaginator = client.get_paginator("list_secrets")
```


### paginate

Type annotations and code completion for `#!python ListSecretsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    SortOrder: SortOrderTypeType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListSecretsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListSecretsResponseTypeDef](./type_defs.md#listsecretsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSecretsRequestListSecretsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSecretsRequestListSecretsPaginateTypeDef](./type_defs.md#listsecretsrequestlistsecretspaginatetypedef) 
