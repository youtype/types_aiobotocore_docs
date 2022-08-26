# Paginators

> [Index](../README.md) > [MediaConnect](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MediaConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
    type annotations stubs module [types-aiobotocore-mediaconnect](https://pypi.org/project/types-aiobotocore-mediaconnect/).

## ListEntitlementsPaginator

Type annotations and code completion for `#!python session.create_client("mediaconnect").get_paginator("list_entitlements")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListEntitlements)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_mediaconnect.paginator import ListEntitlementsPaginator

session = get_session()
async with session.create_client("mediaconnect") as client:  # (1)
    paginator: ListEntitlementsPaginator = client.get_paginator("list_entitlements")  # (2)
    async for item in paginator.paginate(...):
        item: ListEntitlementsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaConnectClient](./client.md)
2. paginator: [ListEntitlementsPaginator](./paginators.md#listentitlementspaginator)
3. item: [:material-code-braces: ListEntitlementsResponseTypeDef](./type_defs.md#listentitlementsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEntitlementsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListEntitlementsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEntitlementsResponseTypeDef](./type_defs.md#listentitlementsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListEntitlementsRequestListEntitlementsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEntitlementsRequestListEntitlementsPaginateTypeDef](./type_defs.md#listentitlementsrequestlistentitlementspaginatetypedef) 
## ListFlowsPaginator

Type annotations and code completion for `#!python session.create_client("mediaconnect").get_paginator("list_flows")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListFlows)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_mediaconnect.paginator import ListFlowsPaginator

session = get_session()
async with session.create_client("mediaconnect") as client:  # (1)
    paginator: ListFlowsPaginator = client.get_paginator("list_flows")  # (2)
    async for item in paginator.paginate(...):
        item: ListFlowsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaConnectClient](./client.md)
2. paginator: [ListFlowsPaginator](./paginators.md#listflowspaginator)
3. item: [:material-code-braces: ListFlowsResponseTypeDef](./type_defs.md#listflowsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFlowsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListFlowsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFlowsResponseTypeDef](./type_defs.md#listflowsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListFlowsRequestListFlowsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFlowsRequestListFlowsPaginateTypeDef](./type_defs.md#listflowsrequestlistflowspaginatetypedef) 
## ListOfferingsPaginator

Type annotations and code completion for `#!python session.create_client("mediaconnect").get_paginator("list_offerings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListOfferings)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_mediaconnect.paginator import ListOfferingsPaginator

session = get_session()
async with session.create_client("mediaconnect") as client:  # (1)
    paginator: ListOfferingsPaginator = client.get_paginator("list_offerings")  # (2)
    async for item in paginator.paginate(...):
        item: ListOfferingsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaConnectClient](./client.md)
2. paginator: [ListOfferingsPaginator](./paginators.md#listofferingspaginator)
3. item: [:material-code-braces: ListOfferingsResponseTypeDef](./type_defs.md#listofferingsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListOfferingsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListOfferingsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListOfferingsResponseTypeDef](./type_defs.md#listofferingsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListOfferingsRequestListOfferingsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOfferingsRequestListOfferingsPaginateTypeDef](./type_defs.md#listofferingsrequestlistofferingspaginatetypedef) 
## ListReservationsPaginator

Type annotations and code completion for `#!python session.create_client("mediaconnect").get_paginator("list_reservations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListReservations)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_mediaconnect.paginator import ListReservationsPaginator

session = get_session()
async with session.create_client("mediaconnect") as client:  # (1)
    paginator: ListReservationsPaginator = client.get_paginator("list_reservations")  # (2)
    async for item in paginator.paginate(...):
        item: ListReservationsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaConnectClient](./client.md)
2. paginator: [ListReservationsPaginator](./paginators.md#listreservationspaginator)
3. item: [:material-code-braces: ListReservationsResponseTypeDef](./type_defs.md#listreservationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListReservationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListReservationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListReservationsResponseTypeDef](./type_defs.md#listreservationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListReservationsRequestListReservationsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListReservationsRequestListReservationsPaginateTypeDef](./type_defs.md#listreservationsrequestlistreservationspaginatetypedef) 
