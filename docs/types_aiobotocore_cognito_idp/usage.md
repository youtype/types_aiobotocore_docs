<a id="examples-for-aiobotocore-cognitoidentityprovider-module"></a>

# Examples for aiobotocore CognitoIdentityProvider module

> [Index](../README.md) > [CognitoIdentityProvider](./README.md) > Examples

- [Examples for aiobotocore CognitoIdentityProvider module](#examples-for-aiobotocore-cognitoidentityprovider-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[cognito-idp]` package installed.

Write your `CognitoIdentityProvider` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type CognitoIdentityProviderClient
# and provides type checking and code completion
async with session.create_client("cognito-idp") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_custom_attributes()
    

    
    # paginator has type AdminListGroupsForUserPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("admin_list_groups_for_user")
    async for item in paginator.paginate(...):
        # item has type AdminListGroupsForUserResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[cognito-idp]` or a standalone
`types_aiobotocore_cognito_idp` package, you have to explicitly specify
`client: CognitoIdentityProviderClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_cognito_idp.client import CognitoIdentityProviderClient
from types_aiobotocore_cognito_idp.type_defs import Dict[str, Any]
from types_aiobotocore_cognito_idp.paginator import AdminListGroupsForUserPaginator

from types_aiobotocore_cognito_idp.literals import PaginatorName



session = get_session()

async with session.create_client("cognito-idp") as client:
    client: CognitoIdentityProviderClient

    
    result: Dict[str, Any] = client.add_custom_attributes()
    

    
    paginator_name: PaginatorName = "admin_list_groups_for_user"
    paginator: AdminListGroupsForUserPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: AdminListGroupsForUserResponseTypeDef
        print(item)
    

    
```
