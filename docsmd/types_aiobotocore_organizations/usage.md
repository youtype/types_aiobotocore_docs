# Examples

> [Index](../README.md) > [Organizations](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Organizations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#organizations)
    type annotations stubs module [types-aiobotocore-organizations](https://pypi.org/project/types-aiobotocore-organizations/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[organizations]` package installed.

Write your `Organizations` code as usual,
type checking and code completion should work out of the box.



```python
# OrganizationsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("organizations") as client:  # (1)
    result = await client.accept_handshake()  # (2)
```

1. client: [OrganizationsClient](./client.md)
2. result: [:material-code-braces: AcceptHandshakeResponseTypeDef](./type_defs.md#accepthandshakeresponsetypedef) 



```python
# ListAWSServiceAccessForOrganizationPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("organizations") as client:  # (1)
    paginator = client.get_paginator("list_aws_service_access_for_organization")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [OrganizationsClient](./client.md)
2. paginator: [ListAWSServiceAccessForOrganizationPaginator](./paginators.md#listawsserviceaccessfororganizationpaginator)
3. item: [:material-code-braces: ListAWSServiceAccessForOrganizationResponseTypeDef](./type_defs.md#listawsserviceaccessfororganizationresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[organizations]`
or a standalone `types_aiobotocore_organizations` package, you have to explicitly specify
`client: OrganizationsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# OrganizationsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_organizations.client import OrganizationsClient
from types_aiobotocore_organizations.type_defs import AcceptHandshakeResponseTypeDef
from types_aiobotocore_organizations.type_defs import AcceptHandshakeRequestTypeDef


session = get_session()

async with session.create_client("organizations") as client:
    client: OrganizationsClient
    kwargs: AcceptHandshakeRequestTypeDef = {...}
    result: AcceptHandshakeResponseTypeDef = await client.accept_handshake(**kwargs)
```



```python
# ListAWSServiceAccessForOrganizationPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_organizations.client import OrganizationsClient
from types_aiobotocore_organizations.paginator import ListAWSServiceAccessForOrganizationPaginator
from types_aiobotocore_organizations.type_defs import ListAWSServiceAccessForOrganizationResponseTypeDef


session = get_session()

async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListAWSServiceAccessForOrganizationPaginator = client.get_paginator("list_aws_service_access_for_organization")
    async for item in paginator.paginate(...):
        item: ListAWSServiceAccessForOrganizationResponseTypeDef
        print(item)
```


