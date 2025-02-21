# Examples

> [Index](../README.md) > [SecretsManager](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SecretsManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#secretsmanager)
    type annotations stubs module [types-aiobotocore-secretsmanager](https://pypi.org/project/types-aiobotocore-secretsmanager/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[secretsmanager]` package installed.

Write your `SecretsManager` code as usual,
type checking and code completion should work out of the box.



```python
# SecretsManagerClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("secretsmanager") as client:  # (1)
    result = await client.batch_get_secret_value()  # (2)
```

1. client: [SecretsManagerClient](./client.md)
2. result: [:material-code-braces: BatchGetSecretValueResponseTypeDef](./type_defs.md#batchgetsecretvalueresponsetypedef) 



```python
# ListSecretsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("secretsmanager") as client:  # (1)
    paginator = client.get_paginator("list_secrets")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SecretsManagerClient](./client.md)
2. paginator: [ListSecretsPaginator](./paginators.md#listsecretspaginator)
3. item: [:material-code-braces: ListSecretsResponseTypeDef](./type_defs.md#listsecretsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[secretsmanager]`
or a standalone `types_aiobotocore_secretsmanager` package, you have to explicitly specify
`client: SecretsManagerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# SecretsManagerClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_secretsmanager.client import SecretsManagerClient
from types_aiobotocore_secretsmanager.type_defs import BatchGetSecretValueResponseTypeDef
from types_aiobotocore_secretsmanager.type_defs import BatchGetSecretValueRequestTypeDef


session = get_session()

async with session.create_client("secretsmanager") as client:
    client: SecretsManagerClient
    kwargs: BatchGetSecretValueRequestTypeDef = {...}
    result: BatchGetSecretValueResponseTypeDef = await client.batch_get_secret_value(**kwargs)
```



```python
# ListSecretsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_secretsmanager.client import SecretsManagerClient
from types_aiobotocore_secretsmanager.paginator import ListSecretsPaginator
from types_aiobotocore_secretsmanager.type_defs import ListSecretsResponseTypeDef


session = get_session()

async with session.create_client("secretsmanager") as client:
    client: SecretsManagerClient
    paginator: ListSecretsPaginator = client.get_paginator("list_secrets")
    async for item in paginator.paginate(...):
        item: ListSecretsResponseTypeDef
        print(item)
```


