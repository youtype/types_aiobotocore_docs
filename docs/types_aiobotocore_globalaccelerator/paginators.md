<a id="paginators-for-aiobotocore-globalaccelerator-module"></a>

# Paginators for aiobotocore GlobalAccelerator module

> [Index](../README.md) > [GlobalAccelerator](./README.md) > Paginators

Auto-generated documentation for
[GlobalAccelerator](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
type annotations stubs module
[types-aiobotocore-globalaccelerator](https://pypi.org/project/types-aiobotocore-globalaccelerator/).

- [Paginators for aiobotocore GlobalAccelerator module](#paginators-for-aiobotocore-globalaccelerator-module)
  - [ListAcceleratorsPaginator](#listacceleratorspaginator)
  - [ListByoipCidrsPaginator](#listbyoipcidrspaginator)
  - [ListCustomRoutingAcceleratorsPaginator](#listcustomroutingacceleratorspaginator)
  - [ListCustomRoutingListenersPaginator](#listcustomroutinglistenerspaginator)
  - [ListCustomRoutingPortMappingsPaginator](#listcustomroutingportmappingspaginator)
  - [ListCustomRoutingPortMappingsByDestinationPaginator](#listcustomroutingportmappingsbydestinationpaginator)
  - [ListEndpointGroupsPaginator](#listendpointgroupspaginator)
  - [ListListenersPaginator](#listlistenerspaginator)

<a id="listacceleratorspaginator"></a>

## ListAcceleratorsPaginator

Type annotations for
`session.create_client("globalaccelerator").get_paginator("list_accelerators")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_globalaccelerator.paginator import ListAcceleratorsPaginator

session = get_session()
async with session.create_client("globalaccelerator") as client:
    client: GlobalAcceleratorClient
    paginator: ListAcceleratorsPaginator = client.get_paginator("list_accelerators")
```

Boto3 documentation:
[GlobalAccelerator.Paginator.ListAccelerators](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListAccelerators)

Arguments for `ListAcceleratorsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAcceleratorsPaginator.paginate` returns
`AsyncIterator`\[[ListAcceleratorsResponseTypeDef](./type_defs.md#listacceleratorsresponsetypedef)\].

<a id="listbyoipcidrspaginator"></a>

## ListByoipCidrsPaginator

Type annotations for
`session.create_client("globalaccelerator").get_paginator("list_byoip_cidrs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_globalaccelerator.paginator import ListByoipCidrsPaginator

session = get_session()
async with session.create_client("globalaccelerator") as client:
    client: GlobalAcceleratorClient
    paginator: ListByoipCidrsPaginator = client.get_paginator("list_byoip_cidrs")
```

Boto3 documentation:
[GlobalAccelerator.Paginator.ListByoipCidrs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListByoipCidrs)

Arguments for `ListByoipCidrsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListByoipCidrsPaginator.paginate` returns
`AsyncIterator`\[[ListByoipCidrsResponseTypeDef](./type_defs.md#listbyoipcidrsresponsetypedef)\].

<a id="listcustomroutingacceleratorspaginator"></a>

## ListCustomRoutingAcceleratorsPaginator

Type annotations for
`session.create_client("globalaccelerator").get_paginator("list_custom_routing_accelerators")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_globalaccelerator.paginator import ListCustomRoutingAcceleratorsPaginator

session = get_session()
async with session.create_client("globalaccelerator") as client:
    client: GlobalAcceleratorClient
    paginator: ListCustomRoutingAcceleratorsPaginator = client.get_paginator("list_custom_routing_accelerators")
```

Boto3 documentation:
[GlobalAccelerator.Paginator.ListCustomRoutingAccelerators](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingAccelerators)

Arguments for `ListCustomRoutingAcceleratorsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListCustomRoutingAcceleratorsPaginator.paginate` returns
`AsyncIterator`\[[ListCustomRoutingAcceleratorsResponseTypeDef](./type_defs.md#listcustomroutingacceleratorsresponsetypedef)\].

<a id="listcustomroutinglistenerspaginator"></a>

## ListCustomRoutingListenersPaginator

Type annotations for
`session.create_client("globalaccelerator").get_paginator("list_custom_routing_listeners")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_globalaccelerator.paginator import ListCustomRoutingListenersPaginator

session = get_session()
async with session.create_client("globalaccelerator") as client:
    client: GlobalAcceleratorClient
    paginator: ListCustomRoutingListenersPaginator = client.get_paginator("list_custom_routing_listeners")
```

Boto3 documentation:
[GlobalAccelerator.Paginator.ListCustomRoutingListeners](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingListeners)

Arguments for `ListCustomRoutingListenersPaginator.paginate` method:

- `AcceleratorArn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListCustomRoutingListenersPaginator.paginate` returns
`AsyncIterator`\[[ListCustomRoutingListenersResponseTypeDef](./type_defs.md#listcustomroutinglistenersresponsetypedef)\].

<a id="listcustomroutingportmappingspaginator"></a>

## ListCustomRoutingPortMappingsPaginator

Type annotations for
`session.create_client("globalaccelerator").get_paginator("list_custom_routing_port_mappings")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_globalaccelerator.paginator import ListCustomRoutingPortMappingsPaginator

session = get_session()
async with session.create_client("globalaccelerator") as client:
    client: GlobalAcceleratorClient
    paginator: ListCustomRoutingPortMappingsPaginator = client.get_paginator("list_custom_routing_port_mappings")
```

Boto3 documentation:
[GlobalAccelerator.Paginator.ListCustomRoutingPortMappings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingPortMappings)

Arguments for `ListCustomRoutingPortMappingsPaginator.paginate` method:

- `AcceleratorArn`: `str` *(required)*
- `EndpointGroupArn`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListCustomRoutingPortMappingsPaginator.paginate` returns
`AsyncIterator`\[[ListCustomRoutingPortMappingsResponseTypeDef](./type_defs.md#listcustomroutingportmappingsresponsetypedef)\].

<a id="listcustomroutingportmappingsbydestinationpaginator"></a>

## ListCustomRoutingPortMappingsByDestinationPaginator

Type annotations for
`session.create_client("globalaccelerator").get_paginator("list_custom_routing_port_mappings_by_destination")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_globalaccelerator.paginator import ListCustomRoutingPortMappingsByDestinationPaginator

session = get_session()
async with session.create_client("globalaccelerator") as client:
    client: GlobalAcceleratorClient
    paginator: ListCustomRoutingPortMappingsByDestinationPaginator = client.get_paginator("list_custom_routing_port_mappings_by_destination")
```

Boto3 documentation:
[GlobalAccelerator.Paginator.ListCustomRoutingPortMappingsByDestination](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingPortMappingsByDestination)

Arguments for `ListCustomRoutingPortMappingsByDestinationPaginator.paginate`
method:

- `EndpointId`: `str` *(required)*
- `DestinationAddress`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListCustomRoutingPortMappingsByDestinationPaginator.paginate` returns
`AsyncIterator`\[[ListCustomRoutingPortMappingsByDestinationResponseTypeDef](./type_defs.md#listcustomroutingportmappingsbydestinationresponsetypedef)\].

<a id="listendpointgroupspaginator"></a>

## ListEndpointGroupsPaginator

Type annotations for
`session.create_client("globalaccelerator").get_paginator("list_endpoint_groups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_globalaccelerator.paginator import ListEndpointGroupsPaginator

session = get_session()
async with session.create_client("globalaccelerator") as client:
    client: GlobalAcceleratorClient
    paginator: ListEndpointGroupsPaginator = client.get_paginator("list_endpoint_groups")
```

Boto3 documentation:
[GlobalAccelerator.Paginator.ListEndpointGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListEndpointGroups)

Arguments for `ListEndpointGroupsPaginator.paginate` method:

- `ListenerArn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListEndpointGroupsPaginator.paginate` returns
`AsyncIterator`\[[ListEndpointGroupsResponseTypeDef](./type_defs.md#listendpointgroupsresponsetypedef)\].

<a id="listlistenerspaginator"></a>

## ListListenersPaginator

Type annotations for
`session.create_client("globalaccelerator").get_paginator("list_listeners")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_globalaccelerator.paginator import ListListenersPaginator

session = get_session()
async with session.create_client("globalaccelerator") as client:
    client: GlobalAcceleratorClient
    paginator: ListListenersPaginator = client.get_paginator("list_listeners")
```

Boto3 documentation:
[GlobalAccelerator.Paginator.ListListeners](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListListeners)

Arguments for `ListListenersPaginator.paginate` method:

- `AcceleratorArn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListListenersPaginator.paginate` returns
`AsyncIterator`\[[ListListenersResponseTypeDef](./type_defs.md#listlistenersresponsetypedef)\].
