# Paginators

> [Index](../README.md) > [PartnerCentralAccountAPI](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [PartnerCentralAccountAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-account.html#partnercentralaccountapi)
    type annotations stubs module [types-aiobotocore-partnercentral-account](https://pypi.org/project/types-aiobotocore-partnercentral-account/).

## ListConnectionInvitationsPaginator

Type annotations and code completion for `#!python session.create_client("partnercentral-account").get_paginator("list_connection_invitations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-account/paginator/ListConnectionInvitations.html#PartnerCentralAccountAPI.Paginator.ListConnectionInvitations)

```python
# ListConnectionInvitationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_partnercentral_account.paginator import ListConnectionInvitationsPaginator

session = get_session()
async with session.create_client("partnercentral-account") as client:  # (1)
    paginator: ListConnectionInvitationsPaginator = client.get_paginator("list_connection_invitations")  # (2)
    async for item in paginator.paginate(...):
        item: ListConnectionInvitationsResponseTypeDef
        print(item)  # (3)
```

1. client: [PartnerCentralAccountAPIClient](./client.md)
2. paginator: [ListConnectionInvitationsPaginator](./paginators.md#listconnectioninvitationspaginator)
3. item: `AioPageIterator[ListConnectionInvitationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListConnectionInvitationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Catalog: str,
    ConnectionType: ConnectionTypeType = ...,  # (1)
    OtherParticipantIdentifiers: Sequence[str] = ...,
    ParticipantType: ParticipantTypeType = ...,  # (2)
    Status: InvitationStatusType = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[ListConnectionInvitationsResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype)
2. See [:material-code-brackets: ParticipantTypeType](./literals.md#participanttypetype)
3. See [:material-code-brackets: InvitationStatusType](./literals.md#invitationstatustype)
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[ListConnectionInvitationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListConnectionInvitationsRequestPaginateTypeDef = {  # (1)
    "Catalog": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConnectionInvitationsRequestPaginateTypeDef](./type_defs.md#listconnectioninvitationsrequestpaginatetypedef)
## ListConnectionsPaginator

Type annotations and code completion for `#!python session.create_client("partnercentral-account").get_paginator("list_connections")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-account/paginator/ListConnections.html#PartnerCentralAccountAPI.Paginator.ListConnections)

```python
# ListConnectionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_partnercentral_account.paginator import ListConnectionsPaginator

session = get_session()
async with session.create_client("partnercentral-account") as client:  # (1)
    paginator: ListConnectionsPaginator = client.get_paginator("list_connections")  # (2)
    async for item in paginator.paginate(...):
        item: ListConnectionsResponseTypeDef
        print(item)  # (3)
```

1. client: [PartnerCentralAccountAPIClient](./client.md)
2. paginator: [ListConnectionsPaginator](./paginators.md#listconnectionspaginator)
3. item: `AioPageIterator[ListConnectionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListConnectionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Catalog: str,
    ConnectionType: str = ...,
    OtherParticipantIdentifiers: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListConnectionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListConnectionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListConnectionsRequestPaginateTypeDef = {  # (1)
    "Catalog": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConnectionsRequestPaginateTypeDef](./type_defs.md#listconnectionsrequestpaginatetypedef)
## ListPartnersPaginator

Type annotations and code completion for `#!python session.create_client("partnercentral-account").get_paginator("list_partners")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-account/paginator/ListPartners.html#PartnerCentralAccountAPI.Paginator.ListPartners)

```python
# ListPartnersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_partnercentral_account.paginator import ListPartnersPaginator

session = get_session()
async with session.create_client("partnercentral-account") as client:  # (1)
    paginator: ListPartnersPaginator = client.get_paginator("list_partners")  # (2)
    async for item in paginator.paginate(...):
        item: ListPartnersResponseTypeDef
        print(item)  # (3)
```

1. client: [PartnerCentralAccountAPIClient](./client.md)
2. paginator: [ListPartnersPaginator](./paginators.md#listpartnerspaginator)
3. item: `AioPageIterator[ListPartnersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPartnersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Catalog: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListPartnersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListPartnersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPartnersRequestPaginateTypeDef = {  # (1)
    "Catalog": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPartnersRequestPaginateTypeDef](./type_defs.md#listpartnersrequestpaginatetypedef)
