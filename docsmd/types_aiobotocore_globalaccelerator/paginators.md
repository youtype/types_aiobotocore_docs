# Paginators

> [Index](../README.md) > [GlobalAccelerator](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [GlobalAccelerator](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#globalaccelerator)
    type annotations stubs module [types-aiobotocore-globalaccelerator](https://pypi.org/project/types-aiobotocore-globalaccelerator/).

## ListAcceleratorsPaginator

Type annotations and code completion for `#!python session.create_client("globalaccelerator").get_paginator("list_accelerators")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator/paginator/ListAccelerators.html#GlobalAccelerator.Paginator.ListAccelerators)

```python
# ListAcceleratorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_globalaccelerator.paginator import ListAcceleratorsPaginator

session = get_session()
async with session.create_client("globalaccelerator") as client:  # (1)
    paginator: ListAcceleratorsPaginator = client.get_paginator("list_accelerators")  # (2)
    async for item in paginator.paginate(...):
        item: ListAcceleratorsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlobalAcceleratorClient](./client.md)
2. paginator: [ListAcceleratorsPaginator](./paginators.md#listacceleratorspaginator)
3. item: [:material-code-braces: ListAcceleratorsResponseTypeDef](./type_defs.md#listacceleratorsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAcceleratorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAcceleratorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAcceleratorsResponseTypeDef](./type_defs.md#listacceleratorsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAcceleratorsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAcceleratorsRequestPaginateTypeDef](./type_defs.md#listacceleratorsrequestpaginatetypedef) 
## ListByoipCidrsPaginator

Type annotations and code completion for `#!python session.create_client("globalaccelerator").get_paginator("list_byoip_cidrs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator/paginator/ListByoipCidrs.html#GlobalAccelerator.Paginator.ListByoipCidrs)

```python
# ListByoipCidrsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_globalaccelerator.paginator import ListByoipCidrsPaginator

session = get_session()
async with session.create_client("globalaccelerator") as client:  # (1)
    paginator: ListByoipCidrsPaginator = client.get_paginator("list_byoip_cidrs")  # (2)
    async for item in paginator.paginate(...):
        item: ListByoipCidrsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlobalAcceleratorClient](./client.md)
2. paginator: [ListByoipCidrsPaginator](./paginators.md#listbyoipcidrspaginator)
3. item: [:material-code-braces: ListByoipCidrsResponseTypeDef](./type_defs.md#listbyoipcidrsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListByoipCidrsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListByoipCidrsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListByoipCidrsResponseTypeDef](./type_defs.md#listbyoipcidrsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListByoipCidrsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListByoipCidrsRequestPaginateTypeDef](./type_defs.md#listbyoipcidrsrequestpaginatetypedef) 
## ListCrossAccountAttachmentsPaginator

Type annotations and code completion for `#!python session.create_client("globalaccelerator").get_paginator("list_cross_account_attachments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator/paginator/ListCrossAccountAttachments.html#GlobalAccelerator.Paginator.ListCrossAccountAttachments)

```python
# ListCrossAccountAttachmentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_globalaccelerator.paginator import ListCrossAccountAttachmentsPaginator

session = get_session()
async with session.create_client("globalaccelerator") as client:  # (1)
    paginator: ListCrossAccountAttachmentsPaginator = client.get_paginator("list_cross_account_attachments")  # (2)
    async for item in paginator.paginate(...):
        item: ListCrossAccountAttachmentsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlobalAcceleratorClient](./client.md)
2. paginator: [ListCrossAccountAttachmentsPaginator](./paginators.md#listcrossaccountattachmentspaginator)
3. item: [:material-code-braces: ListCrossAccountAttachmentsResponseTypeDef](./type_defs.md#listcrossaccountattachmentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCrossAccountAttachmentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListCrossAccountAttachmentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCrossAccountAttachmentsResponseTypeDef](./type_defs.md#listcrossaccountattachmentsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCrossAccountAttachmentsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCrossAccountAttachmentsRequestPaginateTypeDef](./type_defs.md#listcrossaccountattachmentsrequestpaginatetypedef) 
## ListCrossAccountResourcesPaginator

Type annotations and code completion for `#!python session.create_client("globalaccelerator").get_paginator("list_cross_account_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator/paginator/ListCrossAccountResources.html#GlobalAccelerator.Paginator.ListCrossAccountResources)

```python
# ListCrossAccountResourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_globalaccelerator.paginator import ListCrossAccountResourcesPaginator

session = get_session()
async with session.create_client("globalaccelerator") as client:  # (1)
    paginator: ListCrossAccountResourcesPaginator = client.get_paginator("list_cross_account_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListCrossAccountResourcesResponseTypeDef
        print(item)  # (3)
```

1. client: [GlobalAcceleratorClient](./client.md)
2. paginator: [ListCrossAccountResourcesPaginator](./paginators.md#listcrossaccountresourcespaginator)
3. item: [:material-code-braces: ListCrossAccountResourcesResponseTypeDef](./type_defs.md#listcrossaccountresourcesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCrossAccountResourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceOwnerAwsAccountId: str,
    AcceleratorArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListCrossAccountResourcesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCrossAccountResourcesResponseTypeDef](./type_defs.md#listcrossaccountresourcesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCrossAccountResourcesRequestPaginateTypeDef = {  # (1)
    "ResourceOwnerAwsAccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCrossAccountResourcesRequestPaginateTypeDef](./type_defs.md#listcrossaccountresourcesrequestpaginatetypedef) 
## ListCustomRoutingAcceleratorsPaginator

Type annotations and code completion for `#!python session.create_client("globalaccelerator").get_paginator("list_custom_routing_accelerators")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator/paginator/ListCustomRoutingAccelerators.html#GlobalAccelerator.Paginator.ListCustomRoutingAccelerators)

```python
# ListCustomRoutingAcceleratorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_globalaccelerator.paginator import ListCustomRoutingAcceleratorsPaginator

session = get_session()
async with session.create_client("globalaccelerator") as client:  # (1)
    paginator: ListCustomRoutingAcceleratorsPaginator = client.get_paginator("list_custom_routing_accelerators")  # (2)
    async for item in paginator.paginate(...):
        item: ListCustomRoutingAcceleratorsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlobalAcceleratorClient](./client.md)
2. paginator: [ListCustomRoutingAcceleratorsPaginator](./paginators.md#listcustomroutingacceleratorspaginator)
3. item: [:material-code-braces: ListCustomRoutingAcceleratorsResponseTypeDef](./type_defs.md#listcustomroutingacceleratorsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCustomRoutingAcceleratorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListCustomRoutingAcceleratorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCustomRoutingAcceleratorsResponseTypeDef](./type_defs.md#listcustomroutingacceleratorsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCustomRoutingAcceleratorsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCustomRoutingAcceleratorsRequestPaginateTypeDef](./type_defs.md#listcustomroutingacceleratorsrequestpaginatetypedef) 
## ListCustomRoutingEndpointGroupsPaginator

Type annotations and code completion for `#!python session.create_client("globalaccelerator").get_paginator("list_custom_routing_endpoint_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator/paginator/ListCustomRoutingEndpointGroups.html#GlobalAccelerator.Paginator.ListCustomRoutingEndpointGroups)

```python
# ListCustomRoutingEndpointGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_globalaccelerator.paginator import ListCustomRoutingEndpointGroupsPaginator

session = get_session()
async with session.create_client("globalaccelerator") as client:  # (1)
    paginator: ListCustomRoutingEndpointGroupsPaginator = client.get_paginator("list_custom_routing_endpoint_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListCustomRoutingEndpointGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlobalAcceleratorClient](./client.md)
2. paginator: [ListCustomRoutingEndpointGroupsPaginator](./paginators.md#listcustomroutingendpointgroupspaginator)
3. item: [:material-code-braces: ListCustomRoutingEndpointGroupsResponseTypeDef](./type_defs.md#listcustomroutingendpointgroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCustomRoutingEndpointGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ListenerArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListCustomRoutingEndpointGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCustomRoutingEndpointGroupsResponseTypeDef](./type_defs.md#listcustomroutingendpointgroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCustomRoutingEndpointGroupsRequestPaginateTypeDef = {  # (1)
    "ListenerArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCustomRoutingEndpointGroupsRequestPaginateTypeDef](./type_defs.md#listcustomroutingendpointgroupsrequestpaginatetypedef) 
## ListCustomRoutingListenersPaginator

Type annotations and code completion for `#!python session.create_client("globalaccelerator").get_paginator("list_custom_routing_listeners")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator/paginator/ListCustomRoutingListeners.html#GlobalAccelerator.Paginator.ListCustomRoutingListeners)

```python
# ListCustomRoutingListenersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_globalaccelerator.paginator import ListCustomRoutingListenersPaginator

session = get_session()
async with session.create_client("globalaccelerator") as client:  # (1)
    paginator: ListCustomRoutingListenersPaginator = client.get_paginator("list_custom_routing_listeners")  # (2)
    async for item in paginator.paginate(...):
        item: ListCustomRoutingListenersResponseTypeDef
        print(item)  # (3)
```

1. client: [GlobalAcceleratorClient](./client.md)
2. paginator: [ListCustomRoutingListenersPaginator](./paginators.md#listcustomroutinglistenerspaginator)
3. item: [:material-code-braces: ListCustomRoutingListenersResponseTypeDef](./type_defs.md#listcustomroutinglistenersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCustomRoutingListenersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AcceleratorArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListCustomRoutingListenersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCustomRoutingListenersResponseTypeDef](./type_defs.md#listcustomroutinglistenersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCustomRoutingListenersRequestPaginateTypeDef = {  # (1)
    "AcceleratorArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCustomRoutingListenersRequestPaginateTypeDef](./type_defs.md#listcustomroutinglistenersrequestpaginatetypedef) 
## ListCustomRoutingPortMappingsByDestinationPaginator

Type annotations and code completion for `#!python session.create_client("globalaccelerator").get_paginator("list_custom_routing_port_mappings_by_destination")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator/paginator/ListCustomRoutingPortMappingsByDestination.html#GlobalAccelerator.Paginator.ListCustomRoutingPortMappingsByDestination)

```python
# ListCustomRoutingPortMappingsByDestinationPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_globalaccelerator.paginator import ListCustomRoutingPortMappingsByDestinationPaginator

session = get_session()
async with session.create_client("globalaccelerator") as client:  # (1)
    paginator: ListCustomRoutingPortMappingsByDestinationPaginator = client.get_paginator("list_custom_routing_port_mappings_by_destination")  # (2)
    async for item in paginator.paginate(...):
        item: ListCustomRoutingPortMappingsByDestinationResponseTypeDef
        print(item)  # (3)
```

1. client: [GlobalAcceleratorClient](./client.md)
2. paginator: [ListCustomRoutingPortMappingsByDestinationPaginator](./paginators.md#listcustomroutingportmappingsbydestinationpaginator)
3. item: [:material-code-braces: ListCustomRoutingPortMappingsByDestinationResponseTypeDef](./type_defs.md#listcustomroutingportmappingsbydestinationresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCustomRoutingPortMappingsByDestinationPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    EndpointId: str,
    DestinationAddress: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListCustomRoutingPortMappingsByDestinationResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCustomRoutingPortMappingsByDestinationResponseTypeDef](./type_defs.md#listcustomroutingportmappingsbydestinationresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCustomRoutingPortMappingsByDestinationRequestPaginateTypeDef = {  # (1)
    "EndpointId": ...,
    "DestinationAddress": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCustomRoutingPortMappingsByDestinationRequestPaginateTypeDef](./type_defs.md#listcustomroutingportmappingsbydestinationrequestpaginatetypedef) 
## ListCustomRoutingPortMappingsPaginator

Type annotations and code completion for `#!python session.create_client("globalaccelerator").get_paginator("list_custom_routing_port_mappings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator/paginator/ListCustomRoutingPortMappings.html#GlobalAccelerator.Paginator.ListCustomRoutingPortMappings)

```python
# ListCustomRoutingPortMappingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_globalaccelerator.paginator import ListCustomRoutingPortMappingsPaginator

session = get_session()
async with session.create_client("globalaccelerator") as client:  # (1)
    paginator: ListCustomRoutingPortMappingsPaginator = client.get_paginator("list_custom_routing_port_mappings")  # (2)
    async for item in paginator.paginate(...):
        item: ListCustomRoutingPortMappingsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlobalAcceleratorClient](./client.md)
2. paginator: [ListCustomRoutingPortMappingsPaginator](./paginators.md#listcustomroutingportmappingspaginator)
3. item: [:material-code-braces: ListCustomRoutingPortMappingsResponseTypeDef](./type_defs.md#listcustomroutingportmappingsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCustomRoutingPortMappingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AcceleratorArn: str,
    EndpointGroupArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListCustomRoutingPortMappingsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCustomRoutingPortMappingsResponseTypeDef](./type_defs.md#listcustomroutingportmappingsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCustomRoutingPortMappingsRequestPaginateTypeDef = {  # (1)
    "AcceleratorArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCustomRoutingPortMappingsRequestPaginateTypeDef](./type_defs.md#listcustomroutingportmappingsrequestpaginatetypedef) 
## ListEndpointGroupsPaginator

Type annotations and code completion for `#!python session.create_client("globalaccelerator").get_paginator("list_endpoint_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator/paginator/ListEndpointGroups.html#GlobalAccelerator.Paginator.ListEndpointGroups)

```python
# ListEndpointGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_globalaccelerator.paginator import ListEndpointGroupsPaginator

session = get_session()
async with session.create_client("globalaccelerator") as client:  # (1)
    paginator: ListEndpointGroupsPaginator = client.get_paginator("list_endpoint_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListEndpointGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [GlobalAcceleratorClient](./client.md)
2. paginator: [ListEndpointGroupsPaginator](./paginators.md#listendpointgroupspaginator)
3. item: [:material-code-braces: ListEndpointGroupsResponseTypeDef](./type_defs.md#listendpointgroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEndpointGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ListenerArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListEndpointGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEndpointGroupsResponseTypeDef](./type_defs.md#listendpointgroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEndpointGroupsRequestPaginateTypeDef = {  # (1)
    "ListenerArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEndpointGroupsRequestPaginateTypeDef](./type_defs.md#listendpointgroupsrequestpaginatetypedef) 
## ListListenersPaginator

Type annotations and code completion for `#!python session.create_client("globalaccelerator").get_paginator("list_listeners")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator/paginator/ListListeners.html#GlobalAccelerator.Paginator.ListListeners)

```python
# ListListenersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_globalaccelerator.paginator import ListListenersPaginator

session = get_session()
async with session.create_client("globalaccelerator") as client:  # (1)
    paginator: ListListenersPaginator = client.get_paginator("list_listeners")  # (2)
    async for item in paginator.paginate(...):
        item: ListListenersResponseTypeDef
        print(item)  # (3)
```

1. client: [GlobalAcceleratorClient](./client.md)
2. paginator: [ListListenersPaginator](./paginators.md#listlistenerspaginator)
3. item: [:material-code-braces: ListListenersResponseTypeDef](./type_defs.md#listlistenersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListListenersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AcceleratorArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListListenersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListListenersResponseTypeDef](./type_defs.md#listlistenersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListListenersRequestPaginateTypeDef = {  # (1)
    "AcceleratorArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListListenersRequestPaginateTypeDef](./type_defs.md#listlistenersrequestpaginatetypedef) 
