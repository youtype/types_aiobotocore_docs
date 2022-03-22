<a id="examples-for-aiobotocore-sso-module"></a>

# Examples for aiobotocore SSO module

> [Index](../README.md) > [SSO](./README.md) > Examples

- [Examples for aiobotocore SSO module](#examples-for-aiobotocore-sso-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[sso]` package installed.

Write your `SSO` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type SSOClient
# and provides type checking and code completion
async with session.create_client("sso") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListAccountRolesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_account_roles")
    async for item in paginator.paginate(...):
        # item has type ListAccountRolesResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[sso]` or a standalone `types_aiobotocore_sso`
package, you have to explicitly specify `client: SSOClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_sso.client import SSOClient
from types_aiobotocore_sso.type_defs import bool
from types_aiobotocore_sso.paginator import ListAccountRolesPaginator

from types_aiobotocore_sso.literals import PaginatorName



session = get_session()

async with session.create_client("sso") as client:
    client: SSOClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_account_roles"
    paginator: ListAccountRolesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListAccountRolesResponseTypeDef
        print(item)
    

    
```
