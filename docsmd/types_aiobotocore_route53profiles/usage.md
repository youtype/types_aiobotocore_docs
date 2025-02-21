# Examples

> [Index](../README.md) > [Route53Profiles](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Route53Profiles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53profiles.html#route53profiles)
    type annotations stubs module [types-aiobotocore-route53profiles](https://pypi.org/project/types-aiobotocore-route53profiles/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[route53profiles]` package installed.

Write your `Route53Profiles` code as usual,
type checking and code completion should work out of the box.



```python
# Route53ProfilesClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("route53profiles") as client:  # (1)
    result = await client.associate_profile()  # (2)
```

1. client: [Route53ProfilesClient](./client.md)
2. result: [:material-code-braces: AssociateProfileResponseTypeDef](./type_defs.md#associateprofileresponsetypedef) 



```python
# ListProfileAssociationsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("route53profiles") as client:  # (1)
    paginator = client.get_paginator("list_profile_associations")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [Route53ProfilesClient](./client.md)
2. paginator: [ListProfileAssociationsPaginator](./paginators.md#listprofileassociationspaginator)
3. item: [:material-code-braces: ListProfileAssociationsResponseTypeDef](./type_defs.md#listprofileassociationsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[route53profiles]`
or a standalone `types_aiobotocore_route53profiles` package, you have to explicitly specify
`client: Route53ProfilesClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# Route53ProfilesClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_route53profiles.client import Route53ProfilesClient
from types_aiobotocore_route53profiles.type_defs import AssociateProfileResponseTypeDef
from types_aiobotocore_route53profiles.type_defs import AssociateProfileRequestTypeDef


session = get_session()

async with session.create_client("route53profiles") as client:
    client: Route53ProfilesClient
    kwargs: AssociateProfileRequestTypeDef = {...}
    result: AssociateProfileResponseTypeDef = await client.associate_profile(**kwargs)
```



```python
# ListProfileAssociationsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_route53profiles.client import Route53ProfilesClient
from types_aiobotocore_route53profiles.paginator import ListProfileAssociationsPaginator
from types_aiobotocore_route53profiles.type_defs import ListProfileAssociationsResponseTypeDef


session = get_session()

async with session.create_client("route53profiles") as client:
    client: Route53ProfilesClient
    paginator: ListProfileAssociationsPaginator = client.get_paginator("list_profile_associations")
    async for item in paginator.paginate(...):
        item: ListProfileAssociationsResponseTypeDef
        print(item)
```


