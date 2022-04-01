# Paginators

> [Index](../README.md) > [NetworkManager](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [NetworkManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager)
    type annotations stubs module [types-aiobotocore-networkmanager](https://pypi.org/project/types-aiobotocore-networkmanager/).

## DescribeGlobalNetworksPaginator

Type annotations and code completion for `#!python session.create_client("networkmanager").get_paginator("describe_global_networks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.DescribeGlobalNetworks)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import DescribeGlobalNetworksPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: DescribeGlobalNetworksPaginator = client.get_paginator("describe_global_networks")
```


### paginate

Type annotations and code completion for `#!python DescribeGlobalNetworksPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    GlobalNetworkIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeGlobalNetworksResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeGlobalNetworksResponseTypeDef](./type_defs.md#describeglobalnetworksresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeGlobalNetworksRequestDescribeGlobalNetworksPaginateTypeDef = {  # (1)
    "GlobalNetworkIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeGlobalNetworksRequestDescribeGlobalNetworksPaginateTypeDef](./type_defs.md#describeglobalnetworksrequestdescribeglobalnetworkspaginatetypedef) 
## GetConnectPeerAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("networkmanager").get_paginator("get_connect_peer_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetConnectPeerAssociations)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import GetConnectPeerAssociationsPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: GetConnectPeerAssociationsPaginator = client.get_paginator("get_connect_peer_associations")
```


### paginate

Type annotations and code completion for `#!python GetConnectPeerAssociationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    GlobalNetworkId: str,
    ConnectPeerIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetConnectPeerAssociationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetConnectPeerAssociationsResponseTypeDef](./type_defs.md#getconnectpeerassociationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef = {  # (1)
    "GlobalNetworkId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef](./type_defs.md#getconnectpeerassociationsrequestgetconnectpeerassociationspaginatetypedef) 
## GetConnectionsPaginator

Type annotations and code completion for `#!python session.create_client("networkmanager").get_paginator("get_connections")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetConnections)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import GetConnectionsPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: GetConnectionsPaginator = client.get_paginator("get_connections")
```


### paginate

Type annotations and code completion for `#!python GetConnectionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    GlobalNetworkId: str,
    ConnectionIds: Sequence[str] = ...,
    DeviceId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetConnectionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetConnectionsResponseTypeDef](./type_defs.md#getconnectionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetConnectionsRequestGetConnectionsPaginateTypeDef = {  # (1)
    "GlobalNetworkId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetConnectionsRequestGetConnectionsPaginateTypeDef](./type_defs.md#getconnectionsrequestgetconnectionspaginatetypedef) 
## GetCoreNetworkChangeSetPaginator

Type annotations and code completion for `#!python session.create_client("networkmanager").get_paginator("get_core_network_change_set")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetCoreNetworkChangeSet)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import GetCoreNetworkChangeSetPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: GetCoreNetworkChangeSetPaginator = client.get_paginator("get_core_network_change_set")
```


### paginate

Type annotations and code completion for `#!python GetCoreNetworkChangeSetPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    CoreNetworkId: str,
    PolicyVersionId: int,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetCoreNetworkChangeSetResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetCoreNetworkChangeSetResponseTypeDef](./type_defs.md#getcorenetworkchangesetresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef = {  # (1)
    "CoreNetworkId": ...,
    "PolicyVersionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef](./type_defs.md#getcorenetworkchangesetrequestgetcorenetworkchangesetpaginatetypedef) 
## GetCustomerGatewayAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("networkmanager").get_paginator("get_customer_gateway_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetCustomerGatewayAssociations)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import GetCustomerGatewayAssociationsPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: GetCustomerGatewayAssociationsPaginator = client.get_paginator("get_customer_gateway_associations")
```


### paginate

Type annotations and code completion for `#!python GetCustomerGatewayAssociationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    GlobalNetworkId: str,
    CustomerGatewayArns: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetCustomerGatewayAssociationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetCustomerGatewayAssociationsResponseTypeDef](./type_defs.md#getcustomergatewayassociationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef = {  # (1)
    "GlobalNetworkId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef](./type_defs.md#getcustomergatewayassociationsrequestgetcustomergatewayassociationspaginatetypedef) 
## GetDevicesPaginator

Type annotations and code completion for `#!python session.create_client("networkmanager").get_paginator("get_devices")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetDevices)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import GetDevicesPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: GetDevicesPaginator = client.get_paginator("get_devices")
```


### paginate

Type annotations and code completion for `#!python GetDevicesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    GlobalNetworkId: str,
    DeviceIds: Sequence[str] = ...,
    SiteId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetDevicesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetDevicesResponseTypeDef](./type_defs.md#getdevicesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetDevicesRequestGetDevicesPaginateTypeDef = {  # (1)
    "GlobalNetworkId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetDevicesRequestGetDevicesPaginateTypeDef](./type_defs.md#getdevicesrequestgetdevicespaginatetypedef) 
## GetLinkAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("networkmanager").get_paginator("get_link_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetLinkAssociations)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import GetLinkAssociationsPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: GetLinkAssociationsPaginator = client.get_paginator("get_link_associations")
```


### paginate

Type annotations and code completion for `#!python GetLinkAssociationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    GlobalNetworkId: str,
    DeviceId: str = ...,
    LinkId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetLinkAssociationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetLinkAssociationsResponseTypeDef](./type_defs.md#getlinkassociationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef = {  # (1)
    "GlobalNetworkId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef](./type_defs.md#getlinkassociationsrequestgetlinkassociationspaginatetypedef) 
## GetLinksPaginator

Type annotations and code completion for `#!python session.create_client("networkmanager").get_paginator("get_links")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetLinks)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import GetLinksPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: GetLinksPaginator = client.get_paginator("get_links")
```


### paginate

Type annotations and code completion for `#!python GetLinksPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    GlobalNetworkId: str,
    LinkIds: Sequence[str] = ...,
    SiteId: str = ...,
    Type: str = ...,
    Provider: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetLinksResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetLinksResponseTypeDef](./type_defs.md#getlinksresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetLinksRequestGetLinksPaginateTypeDef = {  # (1)
    "GlobalNetworkId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetLinksRequestGetLinksPaginateTypeDef](./type_defs.md#getlinksrequestgetlinkspaginatetypedef) 
## GetNetworkResourceCountsPaginator

Type annotations and code completion for `#!python session.create_client("networkmanager").get_paginator("get_network_resource_counts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetNetworkResourceCounts)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import GetNetworkResourceCountsPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: GetNetworkResourceCountsPaginator = client.get_paginator("get_network_resource_counts")
```


### paginate

Type annotations and code completion for `#!python GetNetworkResourceCountsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    GlobalNetworkId: str,
    ResourceType: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetNetworkResourceCountsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetNetworkResourceCountsResponseTypeDef](./type_defs.md#getnetworkresourcecountsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef = {  # (1)
    "GlobalNetworkId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef](./type_defs.md#getnetworkresourcecountsrequestgetnetworkresourcecountspaginatetypedef) 
## GetNetworkResourceRelationshipsPaginator

Type annotations and code completion for `#!python session.create_client("networkmanager").get_paginator("get_network_resource_relationships")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetNetworkResourceRelationships)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import GetNetworkResourceRelationshipsPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: GetNetworkResourceRelationshipsPaginator = client.get_paginator("get_network_resource_relationships")
```


### paginate

Type annotations and code completion for `#!python GetNetworkResourceRelationshipsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    GlobalNetworkId: str,
    CoreNetworkId: str = ...,
    RegisteredGatewayArn: str = ...,
    AwsRegion: str = ...,
    AccountId: str = ...,
    ResourceType: str = ...,
    ResourceArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetNetworkResourceRelationshipsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetNetworkResourceRelationshipsResponseTypeDef](./type_defs.md#getnetworkresourcerelationshipsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef = {  # (1)
    "GlobalNetworkId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef](./type_defs.md#getnetworkresourcerelationshipsrequestgetnetworkresourcerelationshipspaginatetypedef) 
## GetNetworkResourcesPaginator

Type annotations and code completion for `#!python session.create_client("networkmanager").get_paginator("get_network_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetNetworkResources)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import GetNetworkResourcesPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: GetNetworkResourcesPaginator = client.get_paginator("get_network_resources")
```


### paginate

Type annotations and code completion for `#!python GetNetworkResourcesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    GlobalNetworkId: str,
    CoreNetworkId: str = ...,
    RegisteredGatewayArn: str = ...,
    AwsRegion: str = ...,
    AccountId: str = ...,
    ResourceType: str = ...,
    ResourceArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetNetworkResourcesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetNetworkResourcesResponseTypeDef](./type_defs.md#getnetworkresourcesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef = {  # (1)
    "GlobalNetworkId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef](./type_defs.md#getnetworkresourcesrequestgetnetworkresourcespaginatetypedef) 
## GetNetworkTelemetryPaginator

Type annotations and code completion for `#!python session.create_client("networkmanager").get_paginator("get_network_telemetry")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetNetworkTelemetry)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import GetNetworkTelemetryPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: GetNetworkTelemetryPaginator = client.get_paginator("get_network_telemetry")
```


### paginate

Type annotations and code completion for `#!python GetNetworkTelemetryPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    GlobalNetworkId: str,
    CoreNetworkId: str = ...,
    RegisteredGatewayArn: str = ...,
    AwsRegion: str = ...,
    AccountId: str = ...,
    ResourceType: str = ...,
    ResourceArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetNetworkTelemetryResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetNetworkTelemetryResponseTypeDef](./type_defs.md#getnetworktelemetryresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef = {  # (1)
    "GlobalNetworkId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef](./type_defs.md#getnetworktelemetryrequestgetnetworktelemetrypaginatetypedef) 
## GetSitesPaginator

Type annotations and code completion for `#!python session.create_client("networkmanager").get_paginator("get_sites")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetSites)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import GetSitesPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: GetSitesPaginator = client.get_paginator("get_sites")
```


### paginate

Type annotations and code completion for `#!python GetSitesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    GlobalNetworkId: str,
    SiteIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetSitesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetSitesResponseTypeDef](./type_defs.md#getsitesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetSitesRequestGetSitesPaginateTypeDef = {  # (1)
    "GlobalNetworkId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetSitesRequestGetSitesPaginateTypeDef](./type_defs.md#getsitesrequestgetsitespaginatetypedef) 
## GetTransitGatewayConnectPeerAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("networkmanager").get_paginator("get_transit_gateway_connect_peer_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetTransitGatewayConnectPeerAssociations)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import GetTransitGatewayConnectPeerAssociationsPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: GetTransitGatewayConnectPeerAssociationsPaginator = client.get_paginator("get_transit_gateway_connect_peer_associations")
```


### paginate

Type annotations and code completion for `#!python GetTransitGatewayConnectPeerAssociationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    GlobalNetworkId: str,
    TransitGatewayConnectPeerArns: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetTransitGatewayConnectPeerAssociationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetTransitGatewayConnectPeerAssociationsResponseTypeDef](./type_defs.md#gettransitgatewayconnectpeerassociationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef = {  # (1)
    "GlobalNetworkId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef](./type_defs.md#gettransitgatewayconnectpeerassociationsrequestgettransitgatewayconnectpeerassociationspaginatetypedef) 
## GetTransitGatewayRegistrationsPaginator

Type annotations and code completion for `#!python session.create_client("networkmanager").get_paginator("get_transit_gateway_registrations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetTransitGatewayRegistrations)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import GetTransitGatewayRegistrationsPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: GetTransitGatewayRegistrationsPaginator = client.get_paginator("get_transit_gateway_registrations")
```


### paginate

Type annotations and code completion for `#!python GetTransitGatewayRegistrationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    GlobalNetworkId: str,
    TransitGatewayArns: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetTransitGatewayRegistrationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetTransitGatewayRegistrationsResponseTypeDef](./type_defs.md#gettransitgatewayregistrationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef = {  # (1)
    "GlobalNetworkId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef](./type_defs.md#gettransitgatewayregistrationsrequestgettransitgatewayregistrationspaginatetypedef) 
## ListAttachmentsPaginator

Type annotations and code completion for `#!python session.create_client("networkmanager").get_paginator("list_attachments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.ListAttachments)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import ListAttachmentsPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: ListAttachmentsPaginator = client.get_paginator("list_attachments")
```


### paginate

Type annotations and code completion for `#!python ListAttachmentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    CoreNetworkId: str = ...,
    AttachmentType: AttachmentTypeType = ...,  # (1)
    EdgeLocation: str = ...,
    State: AttachmentStateType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListAttachmentsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: AttachmentTypeType](./literals.md#attachmenttypetype) 
2. See [:material-code-brackets: AttachmentStateType](./literals.md#attachmentstatetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListAttachmentsResponseTypeDef](./type_defs.md#listattachmentsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAttachmentsRequestListAttachmentsPaginateTypeDef = {  # (1)
    "CoreNetworkId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAttachmentsRequestListAttachmentsPaginateTypeDef](./type_defs.md#listattachmentsrequestlistattachmentspaginatetypedef) 
## ListConnectPeersPaginator

Type annotations and code completion for `#!python session.create_client("networkmanager").get_paginator("list_connect_peers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.ListConnectPeers)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import ListConnectPeersPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: ListConnectPeersPaginator = client.get_paginator("list_connect_peers")
```


### paginate

Type annotations and code completion for `#!python ListConnectPeersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    CoreNetworkId: str = ...,
    ConnectAttachmentId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListConnectPeersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListConnectPeersResponseTypeDef](./type_defs.md#listconnectpeersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListConnectPeersRequestListConnectPeersPaginateTypeDef = {  # (1)
    "CoreNetworkId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConnectPeersRequestListConnectPeersPaginateTypeDef](./type_defs.md#listconnectpeersrequestlistconnectpeerspaginatetypedef) 
## ListCoreNetworkPolicyVersionsPaginator

Type annotations and code completion for `#!python session.create_client("networkmanager").get_paginator("list_core_network_policy_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.ListCoreNetworkPolicyVersions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import ListCoreNetworkPolicyVersionsPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: ListCoreNetworkPolicyVersionsPaginator = client.get_paginator("list_core_network_policy_versions")
```


### paginate

Type annotations and code completion for `#!python ListCoreNetworkPolicyVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    CoreNetworkId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListCoreNetworkPolicyVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCoreNetworkPolicyVersionsResponseTypeDef](./type_defs.md#listcorenetworkpolicyversionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef = {  # (1)
    "CoreNetworkId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef](./type_defs.md#listcorenetworkpolicyversionsrequestlistcorenetworkpolicyversionspaginatetypedef) 
## ListCoreNetworksPaginator

Type annotations and code completion for `#!python session.create_client("networkmanager").get_paginator("list_core_networks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.ListCoreNetworks)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import ListCoreNetworksPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: ListCoreNetworksPaginator = client.get_paginator("list_core_networks")
```


### paginate

Type annotations and code completion for `#!python ListCoreNetworksPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListCoreNetworksResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCoreNetworksResponseTypeDef](./type_defs.md#listcorenetworksresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListCoreNetworksRequestListCoreNetworksPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCoreNetworksRequestListCoreNetworksPaginateTypeDef](./type_defs.md#listcorenetworksrequestlistcorenetworkspaginatetypedef) 
