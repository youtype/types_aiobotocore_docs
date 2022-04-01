# Paginators

> [Index](../README.md) > [GlobalAccelerator](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [GlobalAccelerator](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
    type annotations stubs module [types-aiobotocore-globalaccelerator](https://pypi.org/project/types-aiobotocore-globalaccelerator/).

## ListAcceleratorsPaginator

Type annotations and code completion for `#!python session.create_client("globalaccelerator").get_paginator("list_accelerators")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListAccelerators)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_globalaccelerator.paginator import ListAcceleratorsPaginator

session = get_session()
async with session.create_client("globalaccelerator") as client:
    client: GlobalAcceleratorClient
    paginator: ListAcceleratorsPaginator = client.get_paginator("list_accelerators")
```


### paginate

Type annotations and code completion for `#!python ListAcceleratorsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAcceleratorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAcceleratorsResponseTypeDef](./type_defs.md#listacceleratorsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAcceleratorsRequestListAcceleratorsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAcceleratorsRequestListAcceleratorsPaginateTypeDef](./type_defs.md#listacceleratorsrequestlistacceleratorspaginatetypedef) 
## ListByoipCidrsPaginator

Type annotations and code completion for `#!python session.create_client("globalaccelerator").get_paginator("list_byoip_cidrs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListByoipCidrs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_globalaccelerator.paginator import ListByoipCidrsPaginator

session = get_session()
async with session.create_client("globalaccelerator") as client:
    client: GlobalAcceleratorClient
    paginator: ListByoipCidrsPaginator = client.get_paginator("list_byoip_cidrs")
```


### paginate

Type annotations and code completion for `#!python ListByoipCidrsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListByoipCidrsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListByoipCidrsResponseTypeDef](./type_defs.md#listbyoipcidrsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListByoipCidrsRequestListByoipCidrsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListByoipCidrsRequestListByoipCidrsPaginateTypeDef](./type_defs.md#listbyoipcidrsrequestlistbyoipcidrspaginatetypedef) 
## ListCustomRoutingAcceleratorsPaginator

Type annotations and code completion for `#!python session.create_client("globalaccelerator").get_paginator("list_custom_routing_accelerators")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingAccelerators)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_globalaccelerator.paginator import ListCustomRoutingAcceleratorsPaginator

session = get_session()
async with session.create_client("globalaccelerator") as client:
    client: GlobalAcceleratorClient
    paginator: ListCustomRoutingAcceleratorsPaginator = client.get_paginator("list_custom_routing_accelerators")
```


### paginate

Type annotations and code completion for `#!python ListCustomRoutingAcceleratorsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListCustomRoutingAcceleratorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCustomRoutingAcceleratorsResponseTypeDef](./type_defs.md#listcustomroutingacceleratorsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef](./type_defs.md#listcustomroutingacceleratorsrequestlistcustomroutingacceleratorspaginatetypedef) 
## ListCustomRoutingListenersPaginator

Type annotations and code completion for `#!python session.create_client("globalaccelerator").get_paginator("list_custom_routing_listeners")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingListeners)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_globalaccelerator.paginator import ListCustomRoutingListenersPaginator

session = get_session()
async with session.create_client("globalaccelerator") as client:
    client: GlobalAcceleratorClient
    paginator: ListCustomRoutingListenersPaginator = client.get_paginator("list_custom_routing_listeners")
```


### paginate

Type annotations and code completion for `#!python ListCustomRoutingListenersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    AcceleratorArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListCustomRoutingListenersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCustomRoutingListenersResponseTypeDef](./type_defs.md#listcustomroutinglistenersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef = {  # (1)
    "AcceleratorArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef](./type_defs.md#listcustomroutinglistenersrequestlistcustomroutinglistenerspaginatetypedef) 
## ListCustomRoutingPortMappingsPaginator

Type annotations and code completion for `#!python session.create_client("globalaccelerator").get_paginator("list_custom_routing_port_mappings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingPortMappings)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_globalaccelerator.paginator import ListCustomRoutingPortMappingsPaginator

session = get_session()
async with session.create_client("globalaccelerator") as client:
    client: GlobalAcceleratorClient
    paginator: ListCustomRoutingPortMappingsPaginator = client.get_paginator("list_custom_routing_port_mappings")
```


### paginate

Type annotations and code completion for `#!python ListCustomRoutingPortMappingsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    AcceleratorArn: str,
    EndpointGroupArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListCustomRoutingPortMappingsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCustomRoutingPortMappingsResponseTypeDef](./type_defs.md#listcustomroutingportmappingsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef = {  # (1)
    "AcceleratorArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef](./type_defs.md#listcustomroutingportmappingsrequestlistcustomroutingportmappingspaginatetypedef) 
## ListCustomRoutingPortMappingsByDestinationPaginator

Type annotations and code completion for `#!python session.create_client("globalaccelerator").get_paginator("list_custom_routing_port_mappings_by_destination")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingPortMappingsByDestination)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_globalaccelerator.paginator import ListCustomRoutingPortMappingsByDestinationPaginator

session = get_session()
async with session.create_client("globalaccelerator") as client:
    client: GlobalAcceleratorClient
    paginator: ListCustomRoutingPortMappingsByDestinationPaginator = client.get_paginator("list_custom_routing_port_mappings_by_destination")
```


### paginate

Type annotations and code completion for `#!python ListCustomRoutingPortMappingsByDestinationPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    EndpointId: str,
    DestinationAddress: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListCustomRoutingPortMappingsByDestinationResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCustomRoutingPortMappingsByDestinationResponseTypeDef](./type_defs.md#listcustomroutingportmappingsbydestinationresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef = {  # (1)
    "EndpointId": ...,
    "DestinationAddress": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef](./type_defs.md#listcustomroutingportmappingsbydestinationrequestlistcustomroutingportmappingsbydestinationpaginatetypedef) 
## ListEndpointGroupsPaginator

Type annotations and code completion for `#!python session.create_client("globalaccelerator").get_paginator("list_endpoint_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListEndpointGroups)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_globalaccelerator.paginator import ListEndpointGroupsPaginator

session = get_session()
async with session.create_client("globalaccelerator") as client:
    client: GlobalAcceleratorClient
    paginator: ListEndpointGroupsPaginator = client.get_paginator("list_endpoint_groups")
```


### paginate

Type annotations and code completion for `#!python ListEndpointGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ListenerArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListEndpointGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEndpointGroupsResponseTypeDef](./type_defs.md#listendpointgroupsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef = {  # (1)
    "ListenerArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef](./type_defs.md#listendpointgroupsrequestlistendpointgroupspaginatetypedef) 
## ListListenersPaginator

Type annotations and code completion for `#!python session.create_client("globalaccelerator").get_paginator("list_listeners")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListListeners)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_globalaccelerator.paginator import ListListenersPaginator

session = get_session()
async with session.create_client("globalaccelerator") as client:
    client: GlobalAcceleratorClient
    paginator: ListListenersPaginator = client.get_paginator("list_listeners")
```


### paginate

Type annotations and code completion for `#!python ListListenersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    AcceleratorArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListListenersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListListenersResponseTypeDef](./type_defs.md#listlistenersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListListenersRequestListListenersPaginateTypeDef = {  # (1)
    "AcceleratorArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListListenersRequestListListenersPaginateTypeDef](./type_defs.md#listlistenersrequestlistlistenerspaginatetypedef) 
