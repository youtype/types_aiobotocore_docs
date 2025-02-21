# Examples

> [Index](../README.md) > [CognitoIdentityProvider](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CognitoIdentityProvider](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#cognitoidentityprovider)
    type annotations stubs module [types-aiobotocore-cognito-idp](https://pypi.org/project/types-aiobotocore-cognito-idp/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[cognito-idp]` package installed.

Write your `CognitoIdentityProvider` code as usual,
type checking and code completion should work out of the box.



```python
# CognitoIdentityProviderClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("cognito-idp") as client:  # (1)
    result = await client.admin_add_user_to_group()  # (2)
```

1. client: [CognitoIdentityProviderClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



```python
# AdminListGroupsForUserPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("cognito-idp") as client:  # (1)
    paginator = client.get_paginator("admin_list_groups_for_user")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CognitoIdentityProviderClient](./client.md)
2. paginator: [AdminListGroupsForUserPaginator](./paginators.md#adminlistgroupsforuserpaginator)
3. item: [:material-code-braces: AdminListGroupsForUserResponseTypeDef](./type_defs.md#adminlistgroupsforuserresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[cognito-idp]`
or a standalone `types_aiobotocore_cognito_idp` package, you have to explicitly specify
`client: CognitoIdentityProviderClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# CognitoIdentityProviderClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_cognito_idp.client import CognitoIdentityProviderClient
from types_aiobotocore_cognito_idp.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_cognito_idp.type_defs import AdminAddUserToGroupRequestTypeDef


session = get_session()

async with session.create_client("cognito-idp") as client:
    client: CognitoIdentityProviderClient
    kwargs: AdminAddUserToGroupRequestTypeDef = {...}
    result: EmptyResponseMetadataTypeDef = await client.admin_add_user_to_group(**kwargs)
```



```python
# AdminListGroupsForUserPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_cognito_idp.client import CognitoIdentityProviderClient
from types_aiobotocore_cognito_idp.paginator import AdminListGroupsForUserPaginator
from types_aiobotocore_cognito_idp.type_defs import AdminListGroupsForUserResponseTypeDef


session = get_session()

async with session.create_client("cognito-idp") as client:
    client: CognitoIdentityProviderClient
    paginator: AdminListGroupsForUserPaginator = client.get_paginator("admin_list_groups_for_user")
    async for item in paginator.paginate(...):
        item: AdminListGroupsForUserResponseTypeDef
        print(item)
```


