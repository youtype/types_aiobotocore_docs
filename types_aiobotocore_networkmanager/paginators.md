<a id="paginators-for-aiobotocore-networkmanager-module"></a>

# Paginators for aiobotocore NetworkManager module

> [Index](..) > [NetworkManager](.) > Paginators

Auto-generated documentation for
[NetworkManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager)
type annotations stubs module
[types-aiobotocore-networkmanager](https://pypi.org/project/types-aiobotocore-networkmanager/).

- [Paginators for aiobotocore NetworkManager module](#paginators-for-aiobotocore-networkmanager-module)
  - [DescribeGlobalNetworksPaginator](#describeglobalnetworkspaginator)
  - [GetConnectPeerAssociationsPaginator](#getconnectpeerassociationspaginator)
  - [GetConnectionsPaginator](#getconnectionspaginator)
  - [GetCoreNetworkChangeSetPaginator](#getcorenetworkchangesetpaginator)
  - [GetCustomerGatewayAssociationsPaginator](#getcustomergatewayassociationspaginator)
  - [GetDevicesPaginator](#getdevicespaginator)
  - [GetLinkAssociationsPaginator](#getlinkassociationspaginator)
  - [GetLinksPaginator](#getlinkspaginator)
  - [GetNetworkResourceCountsPaginator](#getnetworkresourcecountspaginator)
  - [GetNetworkResourceRelationshipsPaginator](#getnetworkresourcerelationshipspaginator)
  - [GetNetworkResourcesPaginator](#getnetworkresourcespaginator)
  - [GetNetworkTelemetryPaginator](#getnetworktelemetrypaginator)
  - [GetSitesPaginator](#getsitespaginator)
  - [GetTransitGatewayConnectPeerAssociationsPaginator](#gettransitgatewayconnectpeerassociationspaginator)
  - [GetTransitGatewayRegistrationsPaginator](#gettransitgatewayregistrationspaginator)
  - [ListAttachmentsPaginator](#listattachmentspaginator)
  - [ListConnectPeersPaginator](#listconnectpeerspaginator)
  - [ListCoreNetworkPolicyVersionsPaginator](#listcorenetworkpolicyversionspaginator)
  - [ListCoreNetworksPaginator](#listcorenetworkspaginator)

<a id="describeglobalnetworkspaginator"></a>

## DescribeGlobalNetworksPaginator

Type annotations for
`session.create_client("networkmanager").get_paginator("describe_global_networks")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import DescribeGlobalNetworksPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: DescribeGlobalNetworksPaginator = client.get_paginator("describe_global_networks")
```

Boto3 documentation:
[NetworkManager.Paginator.DescribeGlobalNetworks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.DescribeGlobalNetworks)

Arguments for `DescribeGlobalNetworksPaginator.paginate` method:

- `GlobalNetworkIds`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeGlobalNetworksPaginator.paginate` returns
`AsyncIterable`\[[DescribeGlobalNetworksResponseTypeDef](./type_defs.md#describeglobalnetworksresponsetypedef)\].

<a id="getconnectpeerassociationspaginator"></a>

## GetConnectPeerAssociationsPaginator

Type annotations for
`session.create_client("networkmanager").get_paginator("get_connect_peer_associations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import GetConnectPeerAssociationsPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: GetConnectPeerAssociationsPaginator = client.get_paginator("get_connect_peer_associations")
```

Boto3 documentation:
[NetworkManager.Paginator.GetConnectPeerAssociations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetConnectPeerAssociations)

Arguments for `GetConnectPeerAssociationsPaginator.paginate` method:

- `GlobalNetworkId`: `str` *(required)*
- `ConnectPeerIds`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetConnectPeerAssociationsPaginator.paginate` returns
`AsyncIterable`\[[GetConnectPeerAssociationsResponseTypeDef](./type_defs.md#getconnectpeerassociationsresponsetypedef)\].

<a id="getconnectionspaginator"></a>

## GetConnectionsPaginator

Type annotations for
`session.create_client("networkmanager").get_paginator("get_connections")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import GetConnectionsPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: GetConnectionsPaginator = client.get_paginator("get_connections")
```

Boto3 documentation:
[NetworkManager.Paginator.GetConnections](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetConnections)

Arguments for `GetConnectionsPaginator.paginate` method:

- `GlobalNetworkId`: `str` *(required)*
- `ConnectionIds`: `Sequence`\[`str`\]
- `DeviceId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetConnectionsPaginator.paginate` returns
`AsyncIterable`\[[GetConnectionsResponseTypeDef](./type_defs.md#getconnectionsresponsetypedef)\].

<a id="getcorenetworkchangesetpaginator"></a>

## GetCoreNetworkChangeSetPaginator

Type annotations for
`session.create_client("networkmanager").get_paginator("get_core_network_change_set")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import GetCoreNetworkChangeSetPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: GetCoreNetworkChangeSetPaginator = client.get_paginator("get_core_network_change_set")
```

Boto3 documentation:
[NetworkManager.Paginator.GetCoreNetworkChangeSet](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetCoreNetworkChangeSet)

Arguments for `GetCoreNetworkChangeSetPaginator.paginate` method:

- `CoreNetworkId`: `str` *(required)*
- `PolicyVersionId`: `int` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetCoreNetworkChangeSetPaginator.paginate` returns
`AsyncIterable`\[[GetCoreNetworkChangeSetResponseTypeDef](./type_defs.md#getcorenetworkchangesetresponsetypedef)\].

<a id="getcustomergatewayassociationspaginator"></a>

## GetCustomerGatewayAssociationsPaginator

Type annotations for
`session.create_client("networkmanager").get_paginator("get_customer_gateway_associations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import GetCustomerGatewayAssociationsPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: GetCustomerGatewayAssociationsPaginator = client.get_paginator("get_customer_gateway_associations")
```

Boto3 documentation:
[NetworkManager.Paginator.GetCustomerGatewayAssociations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetCustomerGatewayAssociations)

Arguments for `GetCustomerGatewayAssociationsPaginator.paginate` method:

- `GlobalNetworkId`: `str` *(required)*
- `CustomerGatewayArns`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetCustomerGatewayAssociationsPaginator.paginate` returns
`AsyncIterable`\[[GetCustomerGatewayAssociationsResponseTypeDef](./type_defs.md#getcustomergatewayassociationsresponsetypedef)\].

<a id="getdevicespaginator"></a>

## GetDevicesPaginator

Type annotations for
`session.create_client("networkmanager").get_paginator("get_devices")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import GetDevicesPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: GetDevicesPaginator = client.get_paginator("get_devices")
```

Boto3 documentation:
[NetworkManager.Paginator.GetDevices](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetDevices)

Arguments for `GetDevicesPaginator.paginate` method:

- `GlobalNetworkId`: `str` *(required)*
- `DeviceIds`: `Sequence`\[`str`\]
- `SiteId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetDevicesPaginator.paginate` returns
`AsyncIterable`\[[GetDevicesResponseTypeDef](./type_defs.md#getdevicesresponsetypedef)\].

<a id="getlinkassociationspaginator"></a>

## GetLinkAssociationsPaginator

Type annotations for
`session.create_client("networkmanager").get_paginator("get_link_associations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import GetLinkAssociationsPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: GetLinkAssociationsPaginator = client.get_paginator("get_link_associations")
```

Boto3 documentation:
[NetworkManager.Paginator.GetLinkAssociations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetLinkAssociations)

Arguments for `GetLinkAssociationsPaginator.paginate` method:

- `GlobalNetworkId`: `str` *(required)*
- `DeviceId`: `str`
- `LinkId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetLinkAssociationsPaginator.paginate` returns
`AsyncIterable`\[[GetLinkAssociationsResponseTypeDef](./type_defs.md#getlinkassociationsresponsetypedef)\].

<a id="getlinkspaginator"></a>

## GetLinksPaginator

Type annotations for
`session.create_client("networkmanager").get_paginator("get_links")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import GetLinksPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: GetLinksPaginator = client.get_paginator("get_links")
```

Boto3 documentation:
[NetworkManager.Paginator.GetLinks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetLinks)

Arguments for `GetLinksPaginator.paginate` method:

- `GlobalNetworkId`: `str` *(required)*
- `LinkIds`: `Sequence`\[`str`\]
- `SiteId`: `str`
- `Type`: `str`
- `Provider`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetLinksPaginator.paginate` returns
`AsyncIterable`\[[GetLinksResponseTypeDef](./type_defs.md#getlinksresponsetypedef)\].

<a id="getnetworkresourcecountspaginator"></a>

## GetNetworkResourceCountsPaginator

Type annotations for
`session.create_client("networkmanager").get_paginator("get_network_resource_counts")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import GetNetworkResourceCountsPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: GetNetworkResourceCountsPaginator = client.get_paginator("get_network_resource_counts")
```

Boto3 documentation:
[NetworkManager.Paginator.GetNetworkResourceCounts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetNetworkResourceCounts)

Arguments for `GetNetworkResourceCountsPaginator.paginate` method:

- `GlobalNetworkId`: `str` *(required)*
- `ResourceType`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetNetworkResourceCountsPaginator.paginate` returns
`AsyncIterable`\[[GetNetworkResourceCountsResponseTypeDef](./type_defs.md#getnetworkresourcecountsresponsetypedef)\].

<a id="getnetworkresourcerelationshipspaginator"></a>

## GetNetworkResourceRelationshipsPaginator

Type annotations for
`session.create_client("networkmanager").get_paginator("get_network_resource_relationships")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import GetNetworkResourceRelationshipsPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: GetNetworkResourceRelationshipsPaginator = client.get_paginator("get_network_resource_relationships")
```

Boto3 documentation:
[NetworkManager.Paginator.GetNetworkResourceRelationships](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetNetworkResourceRelationships)

Arguments for `GetNetworkResourceRelationshipsPaginator.paginate` method:

- `GlobalNetworkId`: `str` *(required)*
- `CoreNetworkId`: `str`
- `RegisteredGatewayArn`: `str`
- `AwsRegion`: `str`
- `AccountId`: `str`
- `ResourceType`: `str`
- `ResourceArn`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetNetworkResourceRelationshipsPaginator.paginate` returns
`AsyncIterable`\[[GetNetworkResourceRelationshipsResponseTypeDef](./type_defs.md#getnetworkresourcerelationshipsresponsetypedef)\].

<a id="getnetworkresourcespaginator"></a>

## GetNetworkResourcesPaginator

Type annotations for
`session.create_client("networkmanager").get_paginator("get_network_resources")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import GetNetworkResourcesPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: GetNetworkResourcesPaginator = client.get_paginator("get_network_resources")
```

Boto3 documentation:
[NetworkManager.Paginator.GetNetworkResources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetNetworkResources)

Arguments for `GetNetworkResourcesPaginator.paginate` method:

- `GlobalNetworkId`: `str` *(required)*
- `CoreNetworkId`: `str`
- `RegisteredGatewayArn`: `str`
- `AwsRegion`: `str`
- `AccountId`: `str`
- `ResourceType`: `str`
- `ResourceArn`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetNetworkResourcesPaginator.paginate` returns
`AsyncIterable`\[[GetNetworkResourcesResponseTypeDef](./type_defs.md#getnetworkresourcesresponsetypedef)\].

<a id="getnetworktelemetrypaginator"></a>

## GetNetworkTelemetryPaginator

Type annotations for
`session.create_client("networkmanager").get_paginator("get_network_telemetry")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import GetNetworkTelemetryPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: GetNetworkTelemetryPaginator = client.get_paginator("get_network_telemetry")
```

Boto3 documentation:
[NetworkManager.Paginator.GetNetworkTelemetry](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetNetworkTelemetry)

Arguments for `GetNetworkTelemetryPaginator.paginate` method:

- `GlobalNetworkId`: `str` *(required)*
- `CoreNetworkId`: `str`
- `RegisteredGatewayArn`: `str`
- `AwsRegion`: `str`
- `AccountId`: `str`
- `ResourceType`: `str`
- `ResourceArn`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetNetworkTelemetryPaginator.paginate` returns
`AsyncIterable`\[[GetNetworkTelemetryResponseTypeDef](./type_defs.md#getnetworktelemetryresponsetypedef)\].

<a id="getsitespaginator"></a>

## GetSitesPaginator

Type annotations for
`session.create_client("networkmanager").get_paginator("get_sites")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import GetSitesPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: GetSitesPaginator = client.get_paginator("get_sites")
```

Boto3 documentation:
[NetworkManager.Paginator.GetSites](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetSites)

Arguments for `GetSitesPaginator.paginate` method:

- `GlobalNetworkId`: `str` *(required)*
- `SiteIds`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetSitesPaginator.paginate` returns
`AsyncIterable`\[[GetSitesResponseTypeDef](./type_defs.md#getsitesresponsetypedef)\].

<a id="gettransitgatewayconnectpeerassociationspaginator"></a>

## GetTransitGatewayConnectPeerAssociationsPaginator

Type annotations for
`session.create_client("networkmanager").get_paginator("get_transit_gateway_connect_peer_associations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import GetTransitGatewayConnectPeerAssociationsPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: GetTransitGatewayConnectPeerAssociationsPaginator = client.get_paginator("get_transit_gateway_connect_peer_associations")
```

Boto3 documentation:
[NetworkManager.Paginator.GetTransitGatewayConnectPeerAssociations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetTransitGatewayConnectPeerAssociations)

Arguments for `GetTransitGatewayConnectPeerAssociationsPaginator.paginate`
method:

- `GlobalNetworkId`: `str` *(required)*
- `TransitGatewayConnectPeerArns`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetTransitGatewayConnectPeerAssociationsPaginator.paginate` returns
`AsyncIterable`\[[GetTransitGatewayConnectPeerAssociationsResponseTypeDef](./type_defs.md#gettransitgatewayconnectpeerassociationsresponsetypedef)\].

<a id="gettransitgatewayregistrationspaginator"></a>

## GetTransitGatewayRegistrationsPaginator

Type annotations for
`session.create_client("networkmanager").get_paginator("get_transit_gateway_registrations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import GetTransitGatewayRegistrationsPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: GetTransitGatewayRegistrationsPaginator = client.get_paginator("get_transit_gateway_registrations")
```

Boto3 documentation:
[NetworkManager.Paginator.GetTransitGatewayRegistrations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetTransitGatewayRegistrations)

Arguments for `GetTransitGatewayRegistrationsPaginator.paginate` method:

- `GlobalNetworkId`: `str` *(required)*
- `TransitGatewayArns`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetTransitGatewayRegistrationsPaginator.paginate` returns
`AsyncIterable`\[[GetTransitGatewayRegistrationsResponseTypeDef](./type_defs.md#gettransitgatewayregistrationsresponsetypedef)\].

<a id="listattachmentspaginator"></a>

## ListAttachmentsPaginator

Type annotations for
`session.create_client("networkmanager").get_paginator("list_attachments")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import ListAttachmentsPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: ListAttachmentsPaginator = client.get_paginator("list_attachments")
```

Boto3 documentation:
[NetworkManager.Paginator.ListAttachments](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.ListAttachments)

Arguments for `ListAttachmentsPaginator.paginate` method:

- `CoreNetworkId`: `str`
- `AttachmentType`: [AttachmentTypeType](./literals.md#attachmenttypetype)
- `EdgeLocation`: `str`
- `State`: [AttachmentStateType](./literals.md#attachmentstatetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAttachmentsPaginator.paginate` returns
`AsyncIterable`\[[ListAttachmentsResponseTypeDef](./type_defs.md#listattachmentsresponsetypedef)\].

<a id="listconnectpeerspaginator"></a>

## ListConnectPeersPaginator

Type annotations for
`session.create_client("networkmanager").get_paginator("list_connect_peers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import ListConnectPeersPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: ListConnectPeersPaginator = client.get_paginator("list_connect_peers")
```

Boto3 documentation:
[NetworkManager.Paginator.ListConnectPeers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.ListConnectPeers)

Arguments for `ListConnectPeersPaginator.paginate` method:

- `CoreNetworkId`: `str`
- `ConnectAttachmentId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListConnectPeersPaginator.paginate` returns
`AsyncIterable`\[[ListConnectPeersResponseTypeDef](./type_defs.md#listconnectpeersresponsetypedef)\].

<a id="listcorenetworkpolicyversionspaginator"></a>

## ListCoreNetworkPolicyVersionsPaginator

Type annotations for
`session.create_client("networkmanager").get_paginator("list_core_network_policy_versions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import ListCoreNetworkPolicyVersionsPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: ListCoreNetworkPolicyVersionsPaginator = client.get_paginator("list_core_network_policy_versions")
```

Boto3 documentation:
[NetworkManager.Paginator.ListCoreNetworkPolicyVersions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.ListCoreNetworkPolicyVersions)

Arguments for `ListCoreNetworkPolicyVersionsPaginator.paginate` method:

- `CoreNetworkId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListCoreNetworkPolicyVersionsPaginator.paginate` returns
`AsyncIterable`\[[ListCoreNetworkPolicyVersionsResponseTypeDef](./type_defs.md#listcorenetworkpolicyversionsresponsetypedef)\].

<a id="listcorenetworkspaginator"></a>

## ListCoreNetworksPaginator

Type annotations for
`session.create_client("networkmanager").get_paginator("list_core_networks")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_networkmanager.paginator import ListCoreNetworksPaginator

session = get_session()
async with session.create_client("networkmanager") as client:
    client: NetworkManagerClient
    paginator: ListCoreNetworksPaginator = client.get_paginator("list_core_networks")
```

Boto3 documentation:
[NetworkManager.Paginator.ListCoreNetworks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.ListCoreNetworks)

Arguments for `ListCoreNetworksPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListCoreNetworksPaginator.paginate` returns
`AsyncIterable`\[[ListCoreNetworksResponseTypeDef](./type_defs.md#listcorenetworksresponsetypedef)\].
