<a id="examples-for-aiobotocore-organizations-module"></a>

# Examples for aiobotocore Organizations module

> [Index](../README.md) > [Organizations](./README.md) > Examples

- [Examples for aiobotocore Organizations module](#examples-for-aiobotocore-organizations-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[organizations]` package installed.

Write your `Organizations` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type OrganizationsClient
# and provides type checking and code completion
async with session.create_client("organizations") as client:
    
    # result has type AcceptHandshakeResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.accept_handshake()
    

    
    # paginator has type ListAWSServiceAccessForOrganizationPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_aws_service_access_for_organization")
    async for item in paginator.paginate(...):
        # item has type ListAWSServiceAccessForOrganizationResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[organizations]` or a standalone
`types_aiobotocore_organizations` package, you have to explicitly specify
`client: OrganizationsClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_organizations.client import OrganizationsClient
from types_aiobotocore_organizations.type_defs import AcceptHandshakeResponseTypeDef
from types_aiobotocore_organizations.paginator import ListAWSServiceAccessForOrganizationPaginator

from types_aiobotocore_organizations.literals import PaginatorName



session = get_session()

async with session.create_client("organizations") as client:
    client: OrganizationsClient

    
    result: AcceptHandshakeResponseTypeDef = client.accept_handshake()
    

    
    paginator_name: PaginatorName = "list_aws_service_access_for_organization"
    paginator: ListAWSServiceAccessForOrganizationPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListAWSServiceAccessForOrganizationResponseTypeDef
        print(item)
    

    
```
