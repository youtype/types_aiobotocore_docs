<a id="examples-for-aiobotocore-ssoadmin-module"></a>

# Examples for aiobotocore SSOAdmin module

> [Index](../README.md) > [SSOAdmin](./README.md) > Examples

- [Examples for aiobotocore SSOAdmin module](#examples-for-aiobotocore-ssoadmin-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[sso-admin]` package installed.

Write your `SSOAdmin` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type SSOAdminClient
# and provides type checking and code completion
async with session.create_client("sso-admin") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.attach_managed_policy_to_permission_set()
    

    
    # paginator has type ListAccountAssignmentCreationStatusPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_account_assignment_creation_status")
    async for item in paginator.paginate(...):
        # item has type ListAccountAssignmentCreationStatusResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[sso-admin]` or a standalone
`types_aiobotocore_sso_admin` package, you have to explicitly specify
`client: SSOAdminClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_sso_admin.client import SSOAdminClient
from types_aiobotocore_sso_admin.type_defs import Dict[str, Any]
from types_aiobotocore_sso_admin.paginator import ListAccountAssignmentCreationStatusPaginator

from types_aiobotocore_sso_admin.literals import PaginatorName



session = get_session()

async with session.create_client("sso-admin") as client:
    client: SSOAdminClient

    
    result: Dict[str, Any] = client.attach_managed_policy_to_permission_set()
    

    
    paginator_name: PaginatorName = "list_account_assignment_creation_status"
    paginator: ListAccountAssignmentCreationStatusPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListAccountAssignmentCreationStatusResponseTypeDef
        print(item)
    

    
```
