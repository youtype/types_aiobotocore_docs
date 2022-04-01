# Paginators

> [Index](../README.md) > [CognitoIdentity](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CognitoIdentity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity)
    type annotations stubs module [types-aiobotocore-cognito-identity](https://pypi.org/project/types-aiobotocore-cognito-identity/).

## ListIdentityPoolsPaginator

Type annotations and code completion for `#!python session.create_client("cognito-identity").get_paginator("list_identity_pools")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Paginator.ListIdentityPools)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_cognito_identity.paginator import ListIdentityPoolsPaginator

session = get_session()
async with session.create_client("cognito-identity") as client:
    client: CognitoIdentityClient
    paginator: ListIdentityPoolsPaginator = client.get_paginator("list_identity_pools")
```


### paginate

Type annotations and code completion for `#!python ListIdentityPoolsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListIdentityPoolsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListIdentityPoolsResponseTypeDef](./type_defs.md#listidentitypoolsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef](./type_defs.md#listidentitypoolsinputlistidentitypoolspaginatetypedef) 
