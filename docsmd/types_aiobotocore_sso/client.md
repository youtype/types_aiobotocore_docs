# SSOClient

> [Index](../README.md) > [SSO](./README.md) > SSOClient

!!! note ""

    Auto-generated documentation for [SSO](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
    type annotations stubs module [types-aiobotocore-sso](https://pypi.org/project/types-aiobotocore-sso/).

## SSOClient

Type annotations and code completion for `#!python session.create_client("sso")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Client)

```python
# SSOClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_sso.client import SSOClient

session = get_session()
async with session.create_client("sso") as client:
    client: SSOClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("sso").exceptions` structure.

```python
# SSOClient.exceptions usage example

async with session.create_client("sso") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.InvalidRequestException,
        client.ResourceNotFoundException,
        client.TooManyRequestsException,
        client.UnauthorizedException,
    ) as e:
        print(e)
```

```python
# SSOClient usage type checking example

from types_aiobotocore_sso.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("sso").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("sso").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("sso").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Client.generate_presigned_url)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### get\_role\_credentials

Returns the STS short-term credentials for a given role name that is assigned
to the
user.

Type annotations and code completion for `#!python session.create_client("sso").get_role_credentials` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Client.get_role_credentials)

```python
# get_role_credentials method definition

await def get_role_credentials(
    self,
    *,
    roleName: str,
    accountId: str,
    accessToken: str,
) -> GetRoleCredentialsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRoleCredentialsResponseTypeDef](./type_defs.md#getrolecredentialsresponsetypedef) 


```python
# get_role_credentials method usage example with argument unpacking

kwargs: GetRoleCredentialsRequestRequestTypeDef = {  # (1)
    "roleName": ...,
    "accountId": ...,
    "accessToken": ...,
}

parent.get_role_credentials(**kwargs)
```

1. See [:material-code-braces: GetRoleCredentialsRequestRequestTypeDef](./type_defs.md#getrolecredentialsrequestrequesttypedef) 

### list\_account\_roles

Lists all roles that are assigned to the user for a given AWS account.

Type annotations and code completion for `#!python session.create_client("sso").list_account_roles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Client.list_account_roles)

```python
# list_account_roles method definition

await def list_account_roles(
    self,
    *,
    accessToken: str,
    accountId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListAccountRolesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAccountRolesResponseTypeDef](./type_defs.md#listaccountrolesresponsetypedef) 


```python
# list_account_roles method usage example with argument unpacking

kwargs: ListAccountRolesRequestRequestTypeDef = {  # (1)
    "accessToken": ...,
    "accountId": ...,
}

parent.list_account_roles(**kwargs)
```

1. See [:material-code-braces: ListAccountRolesRequestRequestTypeDef](./type_defs.md#listaccountrolesrequestrequesttypedef) 

### list\_accounts

Lists all AWS accounts assigned to the user.

Type annotations and code completion for `#!python session.create_client("sso").list_accounts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Client.list_accounts)

```python
# list_accounts method definition

await def list_accounts(
    self,
    *,
    accessToken: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListAccountsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAccountsResponseTypeDef](./type_defs.md#listaccountsresponsetypedef) 


```python
# list_accounts method usage example with argument unpacking

kwargs: ListAccountsRequestRequestTypeDef = {  # (1)
    "accessToken": ...,
}

parent.list_accounts(**kwargs)
```

1. See [:material-code-braces: ListAccountsRequestRequestTypeDef](./type_defs.md#listaccountsrequestrequesttypedef) 

### logout

Removes the locally stored SSO tokens from the client-side cache and sends an
API call to the IAM Identity Center service to invalidate the corresponding
server-side IAM Identity Center sign in
session.

Type annotations and code completion for `#!python session.create_client("sso").logout` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Client.logout)

```python
# logout method definition

await def logout(
    self,
    *,
    accessToken: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# logout method usage example with argument unpacking

kwargs: LogoutRequestRequestTypeDef = {  # (1)
    "accessToken": ...,
}

parent.logout(**kwargs)
```

1. See [:material-code-braces: LogoutRequestRequestTypeDef](./type_defs.md#logoutrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("sso").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "SSOClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("sso").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Client.__aexit__)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("sso").get_paginator` method with overloads.

- `client.get_paginator("list_account_roles")` -> [ListAccountRolesPaginator](./paginators.md#listaccountrolespaginator)
- `client.get_paginator("list_accounts")` -> [ListAccountsPaginator](./paginators.md#listaccountspaginator)



