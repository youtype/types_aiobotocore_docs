# Private5G module

> [Index](../README.md) > Private5G


!!! note ""

    Auto-generated documentation for [Private5G](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
    type annotations stubs module [types-aiobotocore-privatenetworks](https://pypi.org/project/types-aiobotocore-privatenetworks/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `Private5G` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[privatenetworks]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[privatenetworks]'


# standalone installation
python -m pip install types-aiobotocore-privatenetworks
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-privatenetworks
```

## Usage

Code samples can be found in [Examples](./usage.md).

## Private5GClient

Type annotations and code completion for  `#!python session.create_client("privatenetworks")` as [Private5GClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_privatenetworks.client import Private5GClient


session = get_session()
async with session.create_client("privatenetworks") as client:
    client: Private5GClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("privatenetworks").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_privatenetworks.paginator import ListDeviceIdentifiersPaginator

def get_list_device_identifiers_paginator() -> ListDeviceIdentifiersPaginator:
    return client.get_paginator("list_device_identifiers"))
```

- [ListDeviceIdentifiersPaginator](./paginators.md#listdeviceidentifierspaginator)
- [ListNetworkResourcesPaginator](./paginators.md#listnetworkresourcespaginator)
- [ListNetworkSitesPaginator](./paginators.md#listnetworksitespaginator)
- [ListNetworksPaginator](./paginators.md#listnetworkspaginator)
- [ListOrdersPaginator](./paginators.md#listorderspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_privatenetworks.literals import AcknowledgmentStatusType

def get_value() -> AcknowledgmentStatusType:
    return "ACKNOWLEDGED"
```

- [AcknowledgmentStatusType](./literals.md#acknowledgmentstatustype)
- [DeviceIdentifierFilterKeysType](./literals.md#deviceidentifierfilterkeystype)
- [DeviceIdentifierStatusType](./literals.md#deviceidentifierstatustype)
- [ElevationReferenceType](./literals.md#elevationreferencetype)
- [ElevationUnitType](./literals.md#elevationunittype)
- [HealthStatusType](./literals.md#healthstatustype)
- [ListDeviceIdentifiersPaginatorName](./literals.md#listdeviceidentifierspaginatorname)
- [ListNetworkResourcesPaginatorName](./literals.md#listnetworkresourcespaginatorname)
- [ListNetworkSitesPaginatorName](./literals.md#listnetworksitespaginatorname)
- [ListNetworksPaginatorName](./literals.md#listnetworkspaginatorname)
- [ListOrdersPaginatorName](./literals.md#listorderspaginatorname)
- [NetworkFilterKeysType](./literals.md#networkfilterkeystype)
- [NetworkResourceDefinitionTypeType](./literals.md#networkresourcedefinitiontypetype)
- [NetworkResourceFilterKeysType](./literals.md#networkresourcefilterkeystype)
- [NetworkResourceStatusType](./literals.md#networkresourcestatustype)
- [NetworkResourceTypeType](./literals.md#networkresourcetypetype)
- [NetworkSiteFilterKeysType](./literals.md#networksitefilterkeystype)
- [NetworkSiteStatusType](./literals.md#networksitestatustype)
- [NetworkStatusType](./literals.md#networkstatustype)
- [OrderFilterKeysType](./literals.md#orderfilterkeystype)
- [Private5GServiceName](./literals.md#private5gservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_privatenetworks.type_defs import AcknowledgeOrderReceiptRequestRequestTypeDef

def get_value() -> AcknowledgeOrderReceiptRequestRequestTypeDef:
    return {
        "orderArn": ...,
    }
```

- [AcknowledgeOrderReceiptRequestRequestTypeDef](./type_defs.md#acknowledgeorderreceiptrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ActivateDeviceIdentifierRequestRequestTypeDef](./type_defs.md#activatedeviceidentifierrequestrequesttypedef)
- [DeviceIdentifierTypeDef](./type_defs.md#deviceidentifiertypedef)
- [AddressTypeDef](./type_defs.md#addresstypedef)
- [PositionTypeDef](./type_defs.md#positiontypedef)
- [CreateNetworkRequestRequestTypeDef](./type_defs.md#createnetworkrequestrequesttypedef)
- [NetworkTypeDef](./type_defs.md#networktypedef)
- [DeactivateDeviceIdentifierRequestRequestTypeDef](./type_defs.md#deactivatedeviceidentifierrequestrequesttypedef)
- [DeleteNetworkRequestRequestTypeDef](./type_defs.md#deletenetworkrequestrequesttypedef)
- [DeleteNetworkSiteRequestRequestTypeDef](./type_defs.md#deletenetworksiterequestrequesttypedef)
- [GetDeviceIdentifierRequestRequestTypeDef](./type_defs.md#getdeviceidentifierrequestrequesttypedef)
- [GetNetworkRequestRequestTypeDef](./type_defs.md#getnetworkrequestrequesttypedef)
- [GetNetworkResourceRequestRequestTypeDef](./type_defs.md#getnetworkresourcerequestrequesttypedef)
- [GetNetworkSiteRequestRequestTypeDef](./type_defs.md#getnetworksiterequestrequesttypedef)
- [GetOrderRequestRequestTypeDef](./type_defs.md#getorderrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListDeviceIdentifiersRequestRequestTypeDef](./type_defs.md#listdeviceidentifiersrequestrequesttypedef)
- [ListNetworkResourcesRequestRequestTypeDef](./type_defs.md#listnetworkresourcesrequestrequesttypedef)
- [ListNetworkSitesRequestRequestTypeDef](./type_defs.md#listnetworksitesrequestrequesttypedef)
- [ListNetworksRequestRequestTypeDef](./type_defs.md#listnetworksrequestrequesttypedef)
- [ListOrdersRequestRequestTypeDef](./type_defs.md#listordersrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [NameValuePairTypeDef](./type_defs.md#namevaluepairtypedef)
- [TrackingInformationTypeDef](./type_defs.md#trackinginformationtypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateNetworkSiteRequestRequestTypeDef](./type_defs.md#updatenetworksiterequestrequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [PingResponseTypeDef](./type_defs.md#pingresponsetypedef)
- [ActivateDeviceIdentifierResponseTypeDef](./type_defs.md#activatedeviceidentifierresponsetypedef)
- [DeactivateDeviceIdentifierResponseTypeDef](./type_defs.md#deactivatedeviceidentifierresponsetypedef)
- [GetDeviceIdentifierResponseTypeDef](./type_defs.md#getdeviceidentifierresponsetypedef)
- [ListDeviceIdentifiersResponseTypeDef](./type_defs.md#listdeviceidentifiersresponsetypedef)
- [ActivateNetworkSiteRequestRequestTypeDef](./type_defs.md#activatenetworksiterequestrequesttypedef)
- [ConfigureAccessPointRequestRequestTypeDef](./type_defs.md#configureaccesspointrequestrequesttypedef)
- [CreateNetworkResponseTypeDef](./type_defs.md#createnetworkresponsetypedef)
- [DeleteNetworkResponseTypeDef](./type_defs.md#deletenetworkresponsetypedef)
- [GetNetworkResponseTypeDef](./type_defs.md#getnetworkresponsetypedef)
- [ListNetworksResponseTypeDef](./type_defs.md#listnetworksresponsetypedef)
- [ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef](./type_defs.md#listdeviceidentifiersrequestlistdeviceidentifierspaginatetypedef)
- [ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef](./type_defs.md#listnetworkresourcesrequestlistnetworkresourcespaginatetypedef)
- [ListNetworkSitesRequestListNetworkSitesPaginateTypeDef](./type_defs.md#listnetworksitesrequestlistnetworksitespaginatetypedef)
- [ListNetworksRequestListNetworksPaginateTypeDef](./type_defs.md#listnetworksrequestlistnetworkspaginatetypedef)
- [ListOrdersRequestListOrdersPaginateTypeDef](./type_defs.md#listordersrequestlistorderspaginatetypedef)
- [NetworkResourceDefinitionTypeDef](./type_defs.md#networkresourcedefinitiontypedef)
- [NetworkResourceTypeDef](./type_defs.md#networkresourcetypedef)
- [OrderTypeDef](./type_defs.md#ordertypedef)
- [SitePlanTypeDef](./type_defs.md#siteplantypedef)
- [ConfigureAccessPointResponseTypeDef](./type_defs.md#configureaccesspointresponsetypedef)
- [GetNetworkResourceResponseTypeDef](./type_defs.md#getnetworkresourceresponsetypedef)
- [ListNetworkResourcesResponseTypeDef](./type_defs.md#listnetworkresourcesresponsetypedef)
- [AcknowledgeOrderReceiptResponseTypeDef](./type_defs.md#acknowledgeorderreceiptresponsetypedef)
- [GetOrderResponseTypeDef](./type_defs.md#getorderresponsetypedef)
- [ListOrdersResponseTypeDef](./type_defs.md#listordersresponsetypedef)
- [CreateNetworkSiteRequestRequestTypeDef](./type_defs.md#createnetworksiterequestrequesttypedef)
- [NetworkSiteTypeDef](./type_defs.md#networksitetypedef)
- [UpdateNetworkSitePlanRequestRequestTypeDef](./type_defs.md#updatenetworksiteplanrequestrequesttypedef)
- [ActivateNetworkSiteResponseTypeDef](./type_defs.md#activatenetworksiteresponsetypedef)
- [CreateNetworkSiteResponseTypeDef](./type_defs.md#createnetworksiteresponsetypedef)
- [DeleteNetworkSiteResponseTypeDef](./type_defs.md#deletenetworksiteresponsetypedef)
- [GetNetworkSiteResponseTypeDef](./type_defs.md#getnetworksiteresponsetypedef)
- [ListNetworkSitesResponseTypeDef](./type_defs.md#listnetworksitesresponsetypedef)
- [UpdateNetworkSiteResponseTypeDef](./type_defs.md#updatenetworksiteresponsetypedef)

