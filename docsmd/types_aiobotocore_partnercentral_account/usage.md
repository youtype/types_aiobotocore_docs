# Examples

> [Index](../README.md) > [PartnerCentralAccountAPI](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [PartnerCentralAccountAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-account.html#partnercentralaccountapi)
    type annotations stubs module [types-aiobotocore-partnercentral-account](https://pypi.org/project/types-aiobotocore-partnercentral-account/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[partnercentral-account]` package installed.

Write your `PartnerCentralAccountAPI` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# PartnerCentralAccountAPIClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("partnercentral-account") as client:  # (1)
    result = await client.accept_connection_invitation()  # (2)
```

1. client: [PartnerCentralAccountAPIClient](./client.md)
2. result: [:material-code-braces: AcceptConnectionInvitationResponseTypeDef](./type_defs.md#acceptconnectioninvitationresponsetypedef)



#### Paginator usage example

```python
# ListConnectionInvitationsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("partnercentral-account") as client:  # (1)
    paginator = client.get_paginator("list_connection_invitations")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [PartnerCentralAccountAPIClient](./client.md)
2. paginator: [ListConnectionInvitationsPaginator](./paginators.md#listconnectioninvitationspaginator)
3. item: [:material-code-braces: ListConnectionInvitationsResponseTypeDef](./type_defs.md#listconnectioninvitationsresponsetypedef)




### Explicit type annotations

With `types-aiobotocore-lite[partnercentral-account]`
or a standalone `types_aiobotocore_partnercentral_account` package, you have to explicitly specify
`client: PartnerCentralAccountAPIClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# PartnerCentralAccountAPIClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_partnercentral_account.client import PartnerCentralAccountAPIClient
from types_aiobotocore_partnercentral_account.type_defs import AcceptConnectionInvitationResponseTypeDef
from types_aiobotocore_partnercentral_account.type_defs import AcceptConnectionInvitationRequestTypeDef


session = get_session()

async with session.create_client("partnercentral-account") as client:
    client: PartnerCentralAccountAPIClient
    kwargs: AcceptConnectionInvitationRequestTypeDef = {...}
    result: AcceptConnectionInvitationResponseTypeDef = await client.accept_connection_invitation(**kwargs)
```



#### Paginator usage example

```python
# ListConnectionInvitationsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_partnercentral_account.client import PartnerCentralAccountAPIClient
from types_aiobotocore_partnercentral_account.paginator import ListConnectionInvitationsPaginator
from types_aiobotocore_partnercentral_account.type_defs import ListConnectionInvitationsResponseTypeDef


session = get_session()

async with session.create_client("partnercentral-account") as client:
    client: PartnerCentralAccountAPIClient
    paginator: ListConnectionInvitationsPaginator = client.get_paginator("list_connection_invitations")
    async for item in paginator.paginate(...):
        item: ListConnectionInvitationsResponseTypeDef
        print(item)
```


