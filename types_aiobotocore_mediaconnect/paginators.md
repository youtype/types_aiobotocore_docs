<a id="paginators-for-aiobotocore-mediaconnect-module"></a>

# Paginators for aiobotocore MediaConnect module

> [Index](..) > [MediaConnect](.) > Paginators

Auto-generated documentation for
[MediaConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
type annotations stubs module
[types-aiobotocore-mediaconnect](https://pypi.org/project/types-aiobotocore-mediaconnect/).

- [Paginators for aiobotocore MediaConnect module](#paginators-for-aiobotocore-mediaconnect-module)
  - [ListEntitlementsPaginator](#listentitlementspaginator)
  - [ListFlowsPaginator](#listflowspaginator)
  - [ListOfferingsPaginator](#listofferingspaginator)
  - [ListReservationsPaginator](#listreservationspaginator)

<a id="listentitlementspaginator"></a>

## ListEntitlementsPaginator

Type annotations for
`session.create_client("mediaconnect").get_paginator("list_entitlements")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mediaconnect.paginator import ListEntitlementsPaginator

session = get_session()
async with session.create_client("mediaconnect") as client:
    client: MediaConnectClient
    paginator: ListEntitlementsPaginator = client.get_paginator("list_entitlements")
```

Boto3 documentation:
[MediaConnect.Paginator.ListEntitlements](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListEntitlements)

Arguments for `ListEntitlementsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListEntitlementsPaginator.paginate` returns
`_PageIterator`\[[ListEntitlementsResponseTypeDef](./type_defs.md#listentitlementsresponsetypedef)\].

<a id="listflowspaginator"></a>

## ListFlowsPaginator

Type annotations for
`session.create_client("mediaconnect").get_paginator("list_flows")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mediaconnect.paginator import ListFlowsPaginator

session = get_session()
async with session.create_client("mediaconnect") as client:
    client: MediaConnectClient
    paginator: ListFlowsPaginator = client.get_paginator("list_flows")
```

Boto3 documentation:
[MediaConnect.Paginator.ListFlows](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListFlows)

Arguments for `ListFlowsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListFlowsPaginator.paginate` returns
`_PageIterator`\[[ListFlowsResponseTypeDef](./type_defs.md#listflowsresponsetypedef)\].

<a id="listofferingspaginator"></a>

## ListOfferingsPaginator

Type annotations for
`session.create_client("mediaconnect").get_paginator("list_offerings")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mediaconnect.paginator import ListOfferingsPaginator

session = get_session()
async with session.create_client("mediaconnect") as client:
    client: MediaConnectClient
    paginator: ListOfferingsPaginator = client.get_paginator("list_offerings")
```

Boto3 documentation:
[MediaConnect.Paginator.ListOfferings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListOfferings)

Arguments for `ListOfferingsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListOfferingsPaginator.paginate` returns
`_PageIterator`\[[ListOfferingsResponseTypeDef](./type_defs.md#listofferingsresponsetypedef)\].

<a id="listreservationspaginator"></a>

## ListReservationsPaginator

Type annotations for
`session.create_client("mediaconnect").get_paginator("list_reservations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mediaconnect.paginator import ListReservationsPaginator

session = get_session()
async with session.create_client("mediaconnect") as client:
    client: MediaConnectClient
    paginator: ListReservationsPaginator = client.get_paginator("list_reservations")
```

Boto3 documentation:
[MediaConnect.Paginator.ListReservations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Paginator.ListReservations)

Arguments for `ListReservationsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListReservationsPaginator.paginate` returns
`_PageIterator`\[[ListReservationsResponseTypeDef](./type_defs.md#listreservationsresponsetypedef)\].
