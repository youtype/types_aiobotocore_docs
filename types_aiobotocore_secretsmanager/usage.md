<a id="examples-for-aiobotocore-secretsmanager-module"></a>

# Examples for aiobotocore SecretsManager module

> [Index](../README.md) > [SecretsManager](./README.md) > Examples

- [Examples for aiobotocore SecretsManager module](#examples-for-aiobotocore-secretsmanager-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[secretsmanager]` package installed.

Write your `SecretsManager` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type SecretsManagerClient
# and provides type checking and code completion
async with session.create_client("secretsmanager") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListSecretsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_secrets")
    async for item in paginator.paginate(...):
        # item has type ListSecretsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[secretsmanager]` or a standalone
`types_aiobotocore_secretsmanager` package, you have to explicitly specify
`client: SecretsManagerClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_secretsmanager.client import SecretsManagerClient
from types_aiobotocore_secretsmanager.type_defs import bool
from types_aiobotocore_secretsmanager.paginator import ListSecretsPaginator

from types_aiobotocore_secretsmanager.literals import PaginatorName



session = get_session()

async with session.create_client("secretsmanager") as client:
    client: SecretsManagerClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_secrets"
    paginator: ListSecretsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListSecretsResponseTypeDef
        print(item)
    

    
```
