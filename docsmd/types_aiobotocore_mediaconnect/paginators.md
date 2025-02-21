# Paginators

> [Index](../README.md) > [MediaConnect](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MediaConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#mediaconnect)
    type annotations stubs module [types-aiobotocore-mediaconnect](https://pypi.org/project/types-aiobotocore-mediaconnect/).

## ListBridgesPaginator

Type annotations and code completion for `#!python session.create_client("mediaconnect").get_paginator("list_bridges")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect/paginator/ListBridges.html#MediaConnect.Paginator.ListBridges)

```python
# ListBridgesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mediaconnect.paginator import ListBridgesPaginator

session = get_session()
async with session.create_client("mediaconnect") as client:  # (1)
    paginator: ListBridgesPaginator = client.get_paginator("list_bridges")  # (2)
    async for item in paginator.paginate(...):
        item: ListBridgesResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaConnectClient](./client.md)
2. paginator: [ListBridgesPaginator](./paginators.md#listbridgespaginator)
3. item: [:material-code-braces: ListBridgesResponseTypeDef](./type_defs.md#listbridgesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListBridgesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FilterArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListBridgesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListBridgesResponseTypeDef](./type_defs.md#listbridgesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListBridgesRequestPaginateTypeDef = {  # (1)
    "FilterArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBridgesRequestPaginateTypeDef](./type_defs.md#listbridgesrequestpaginatetypedef) 
## ListEntitlementsPaginator

Type annotations and code completion for `#!python session.create_client("mediaconnect").get_paginator("list_entitlements")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect/paginator/ListEntitlements.html#MediaConnect.Paginator.ListEntitlements)

```python
# ListEntitlementsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListEntitlementsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEntitlementsResponseTypeDef](./type_defs.md#listentitlementsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEntitlementsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEntitlementsRequestPaginateTypeDef](./type_defs.md#listentitlementsrequestpaginatetypedef) 
## ListFlowsPaginator

Type annotations and code completion for `#!python session.create_client("mediaconnect").get_paginator("list_flows")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect/paginator/ListFlows.html#MediaConnect.Paginator.ListFlows)

```python
# ListFlowsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListFlowsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFlowsResponseTypeDef](./type_defs.md#listflowsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFlowsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFlowsRequestPaginateTypeDef](./type_defs.md#listflowsrequestpaginatetypedef) 
## ListGatewayInstancesPaginator

Type annotations and code completion for `#!python session.create_client("mediaconnect").get_paginator("list_gateway_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect/paginator/ListGatewayInstances.html#MediaConnect.Paginator.ListGatewayInstances)

```python
# ListGatewayInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mediaconnect.paginator import ListGatewayInstancesPaginator

session = get_session()
async with session.create_client("mediaconnect") as client:  # (1)
    paginator: ListGatewayInstancesPaginator = client.get_paginator("list_gateway_instances")  # (2)
    async for item in paginator.paginate(...):
        item: ListGatewayInstancesResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaConnectClient](./client.md)
2. paginator: [ListGatewayInstancesPaginator](./paginators.md#listgatewayinstancespaginator)
3. item: [:material-code-braces: ListGatewayInstancesResponseTypeDef](./type_defs.md#listgatewayinstancesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListGatewayInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FilterArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListGatewayInstancesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGatewayInstancesResponseTypeDef](./type_defs.md#listgatewayinstancesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListGatewayInstancesRequestPaginateTypeDef = {  # (1)
    "FilterArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGatewayInstancesRequestPaginateTypeDef](./type_defs.md#listgatewayinstancesrequestpaginatetypedef) 
## ListGatewaysPaginator

Type annotations and code completion for `#!python session.create_client("mediaconnect").get_paginator("list_gateways")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect/paginator/ListGateways.html#MediaConnect.Paginator.ListGateways)

```python
# ListGatewaysPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mediaconnect.paginator import ListGatewaysPaginator

session = get_session()
async with session.create_client("mediaconnect") as client:  # (1)
    paginator: ListGatewaysPaginator = client.get_paginator("list_gateways")  # (2)
    async for item in paginator.paginate(...):
        item: ListGatewaysResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaConnectClient](./client.md)
2. paginator: [ListGatewaysPaginator](./paginators.md#listgatewayspaginator)
3. item: [:material-code-braces: ListGatewaysResponseTypeDef](./type_defs.md#listgatewaysresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListGatewaysPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListGatewaysResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGatewaysResponseTypeDef](./type_defs.md#listgatewaysresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListGatewaysRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGatewaysRequestPaginateTypeDef](./type_defs.md#listgatewaysrequestpaginatetypedef) 
## ListOfferingsPaginator

Type annotations and code completion for `#!python session.create_client("mediaconnect").get_paginator("list_offerings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect/paginator/ListOfferings.html#MediaConnect.Paginator.ListOfferings)

```python
# ListOfferingsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListOfferingsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListOfferingsResponseTypeDef](./type_defs.md#listofferingsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListOfferingsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOfferingsRequestPaginateTypeDef](./type_defs.md#listofferingsrequestpaginatetypedef) 
## ListReservationsPaginator

Type annotations and code completion for `#!python session.create_client("mediaconnect").get_paginator("list_reservations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect/paginator/ListReservations.html#MediaConnect.Paginator.ListReservations)

```python
# ListReservationsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListReservationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListReservationsResponseTypeDef](./type_defs.md#listreservationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListReservationsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListReservationsRequestPaginateTypeDef](./type_defs.md#listreservationsrequestpaginatetypedef) 
