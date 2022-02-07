<a id="paginators-for-aiobotocore-secretsmanager-module"></a>

# Paginators for aiobotocore SecretsManager module

> [Index](..) > [SecretsManager](.) > Paginators

Auto-generated documentation for
[SecretsManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
type annotations stubs module
[types-aiobotocore-secretsmanager](https://pypi.org/project/types-aiobotocore-secretsmanager/).

- [Paginators for aiobotocore SecretsManager module](#paginators-for-aiobotocore-secretsmanager-module)
  - [ListSecretsPaginator](#listsecretspaginator)

<a id="listsecretspaginator"></a>

## ListSecretsPaginator

Type annotations for
`session.create_client("secretsmanager").get_paginator("list_secrets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_secretsmanager.paginator import ListSecretsPaginator

session = get_session()
async with session.create_client("secretsmanager") as client:
    client: SecretsManagerClient
    paginator: ListSecretsPaginator = client.get_paginator("list_secrets")
```

Boto3 documentation:
[SecretsManager.Paginator.ListSecrets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Paginator.ListSecrets)

Arguments for `ListSecretsPaginator.paginate` method:

- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `SortOrder`: [SortOrderTypeType](./literals.md#sortordertypetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSecretsPaginator.paginate` returns
`_PageIterator`\[[ListSecretsResponseTypeDef](./type_defs.md#listsecretsresponsetypedef)\].
