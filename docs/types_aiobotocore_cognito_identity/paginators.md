<a id="paginators-for-aiobotocore-cognitoidentity-module"></a>

# Paginators for aiobotocore CognitoIdentity module

> [Index](../README.md) > [CognitoIdentity](./README.md) > Paginators

Auto-generated documentation for
[CognitoIdentity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
type annotations stubs module
[types-aiobotocore-cognito-identity](https://pypi.org/project/types-aiobotocore-cognito-identity/).

- [Paginators for aiobotocore CognitoIdentity module](#paginators-for-aiobotocore-cognitoidentity-module)
  - [ListIdentityPoolsPaginator](#listidentitypoolspaginator)

<a id="listidentitypoolspaginator"></a>

## ListIdentityPoolsPaginator

Type annotations for
`session.create_client("cognito-identity").get_paginator("list_identity_pools")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_cognito_identity.paginator import ListIdentityPoolsPaginator

session = get_session()
async with session.create_client("cognito-identity") as client:
    client: CognitoIdentityClient
    paginator: ListIdentityPoolsPaginator = client.get_paginator("list_identity_pools")
```

Boto3 documentation:
[CognitoIdentity.Paginator.ListIdentityPools](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Paginator.ListIdentityPools)

Arguments for `ListIdentityPoolsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListIdentityPoolsPaginator.paginate` returns
`AsyncIterator`\[[ListIdentityPoolsResponseTypeDef](./type_defs.md#listidentitypoolsresponsetypedef)\].
