# Paginators

> [Index](../README.md) > [CognitoIdentity](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CognitoIdentity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#cognitoidentity)
    type annotations stubs module [types-aiobotocore-cognito-identity](https://pypi.org/project/types-aiobotocore-cognito-identity/).

## ListIdentityPoolsPaginator

Type annotations and code completion for `#!python session.create_client("cognito-identity").get_paginator("list_identity_pools")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity/paginator/ListIdentityPools.html#CognitoIdentity.Paginator.ListIdentityPools)

```python
# ListIdentityPoolsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_cognito_identity.paginator import ListIdentityPoolsPaginator

session = get_session()
async with session.create_client("cognito-identity") as client:  # (1)
    paginator: ListIdentityPoolsPaginator = client.get_paginator("list_identity_pools")  # (2)
    async for item in paginator.paginate(...):
        item: ListIdentityPoolsResponseTypeDef
        print(item)  # (3)
```

1. client: [CognitoIdentityClient](./client.md)
2. paginator: [ListIdentityPoolsPaginator](./paginators.md#listidentitypoolspaginator)
3. item: [:material-code-braces: ListIdentityPoolsResponseTypeDef](./type_defs.md#listidentitypoolsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListIdentityPoolsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListIdentityPoolsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListIdentityPoolsResponseTypeDef](./type_defs.md#listidentitypoolsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListIdentityPoolsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIdentityPoolsInputPaginateTypeDef](./type_defs.md#listidentitypoolsinputpaginatetypedef) 
