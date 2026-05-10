# Paginators

> [Index](../README.md) > [PartnerCentralChannelAPI](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [PartnerCentralChannelAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-channel.html#partnercentralchannelapi)
    type annotations stubs module [types-aiobotocore-partnercentral-channel](https://pypi.org/project/types-aiobotocore-partnercentral-channel/).

## ListChannelHandshakesPaginator

Type annotations and code completion for `#!python session.create_client("partnercentral-channel").get_paginator("list_channel_handshakes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-channel/paginator/ListChannelHandshakes.html#PartnerCentralChannelAPI.Paginator.ListChannelHandshakes)

```python
# ListChannelHandshakesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_partnercentral_channel.paginator import ListChannelHandshakesPaginator

session = get_session()
async with session.create_client("partnercentral-channel") as client:  # (1)
    paginator: ListChannelHandshakesPaginator = client.get_paginator("list_channel_handshakes")  # (2)
    async for item in paginator.paginate(...):
        item: ListChannelHandshakesResponseTypeDef
        print(item)  # (3)
```

1. client: [PartnerCentralChannelAPIClient](./client.md)
2. paginator: [ListChannelHandshakesPaginator](./paginators.md#listchannelhandshakespaginator)
3. item: `AioPageIterator[ListChannelHandshakesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListChannelHandshakesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    handshakeType: HandshakeTypeType,  # (1)
    catalog: str,
    participantType: ParticipantTypeType,  # (2)
    statuses: Sequence[HandshakeStatusType] = ...,  # (3)
    associatedResourceIdentifiers: Sequence[str] = ...,
    handshakeTypeFilters: ListChannelHandshakesTypeFiltersTypeDef = ...,  # (4)
    handshakeTypeSort: ListChannelHandshakesTypeSortTypeDef = ...,  # (5)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (6)
) -> aiobotocore.paginate.AioPageIterator[ListChannelHandshakesResponseTypeDef]:  # (7)
    ...
```

1. See [:material-code-brackets: HandshakeTypeType](./literals.md#handshaketypetype)
2. See [:material-code-brackets: ParticipantTypeType](./literals.md#participanttypetype)
3. See `Sequence[HandshakeStatusType]`
4. See [:material-code-braces: ListChannelHandshakesTypeFiltersTypeDef](./type_defs.md#listchannelhandshakestypefilterstypedef)
5. See [:material-code-braces: ListChannelHandshakesTypeSortTypeDef](./type_defs.md#listchannelhandshakestypesorttypedef)
6. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
7. See `AioPageIterator[ListChannelHandshakesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListChannelHandshakesRequestPaginateTypeDef = {  # (1)
    "handshakeType": ...,
    "catalog": ...,
    "participantType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListChannelHandshakesRequestPaginateTypeDef](./type_defs.md#listchannelhandshakesrequestpaginatetypedef)
## ListProgramManagementAccountsPaginator

Type annotations and code completion for `#!python session.create_client("partnercentral-channel").get_paginator("list_program_management_accounts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-channel/paginator/ListProgramManagementAccounts.html#PartnerCentralChannelAPI.Paginator.ListProgramManagementAccounts)

```python
# ListProgramManagementAccountsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_partnercentral_channel.paginator import ListProgramManagementAccountsPaginator

session = get_session()
async with session.create_client("partnercentral-channel") as client:  # (1)
    paginator: ListProgramManagementAccountsPaginator = client.get_paginator("list_program_management_accounts")  # (2)
    async for item in paginator.paginate(...):
        item: ListProgramManagementAccountsResponseTypeDef
        print(item)  # (3)
```

1. client: [PartnerCentralChannelAPIClient](./client.md)
2. paginator: [ListProgramManagementAccountsPaginator](./paginators.md#listprogrammanagementaccountspaginator)
3. item: `AioPageIterator[ListProgramManagementAccountsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListProgramManagementAccountsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    catalog: str,
    displayNames: Sequence[str] = ...,
    programs: Sequence[ProgramType] = ...,  # (1)
    accountIds: Sequence[str] = ...,
    statuses: Sequence[ProgramManagementAccountStatusType] = ...,  # (2)
    sort: ListProgramManagementAccountsSortBaseTypeDef = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[ListProgramManagementAccountsResponseTypeDef]:  # (5)
    ...
```

1. See `Sequence[ProgramType]`
2. See `Sequence[ProgramManagementAccountStatusType]`
3. See [:material-code-braces: ListProgramManagementAccountsSortBaseTypeDef](./type_defs.md#listprogrammanagementaccountssortbasetypedef)
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[ListProgramManagementAccountsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListProgramManagementAccountsRequestPaginateTypeDef = {  # (1)
    "catalog": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProgramManagementAccountsRequestPaginateTypeDef](./type_defs.md#listprogrammanagementaccountsrequestpaginatetypedef)
## ListRelationshipsPaginator

Type annotations and code completion for `#!python session.create_client("partnercentral-channel").get_paginator("list_relationships")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-channel/paginator/ListRelationships.html#PartnerCentralChannelAPI.Paginator.ListRelationships)

```python
# ListRelationshipsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_partnercentral_channel.paginator import ListRelationshipsPaginator

session = get_session()
async with session.create_client("partnercentral-channel") as client:  # (1)
    paginator: ListRelationshipsPaginator = client.get_paginator("list_relationships")  # (2)
    async for item in paginator.paginate(...):
        item: ListRelationshipsResponseTypeDef
        print(item)  # (3)
```

1. client: [PartnerCentralChannelAPIClient](./client.md)
2. paginator: [ListRelationshipsPaginator](./paginators.md#listrelationshipspaginator)
3. item: `AioPageIterator[ListRelationshipsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRelationshipsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    catalog: str,
    associatedAccountIds: Sequence[str] = ...,
    associationTypes: Sequence[AssociationTypeType] = ...,  # (1)
    displayNames: Sequence[str] = ...,
    programManagementAccountIdentifiers: Sequence[str] = ...,
    sort: ListRelationshipsSortBaseTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListRelationshipsResponseTypeDef]:  # (4)
    ...
```

1. See `Sequence[AssociationTypeType]`
2. See [:material-code-braces: ListRelationshipsSortBaseTypeDef](./type_defs.md#listrelationshipssortbasetypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListRelationshipsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRelationshipsRequestPaginateTypeDef = {  # (1)
    "catalog": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRelationshipsRequestPaginateTypeDef](./type_defs.md#listrelationshipsrequestpaginatetypedef)
