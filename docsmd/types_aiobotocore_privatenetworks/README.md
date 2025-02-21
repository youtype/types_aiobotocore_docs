# Private5G module

> [Index](../README.md) > Private5G


!!! note ""

    Auto-generated documentation for [Private5G](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#private5g)
    type annotations stubs module [types-aiobotocore-privatenetworks](https://pypi.org/project/types-aiobotocore-privatenetworks/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.20.0' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `Private5G` service.
1. Use provided commands to install generated packages.



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

```python
# Private5GClient usage example

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

```python
# ListDeviceIdentifiersPaginator usage example

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

```python
# AcknowledgmentStatusType usage example

from types_aiobotocore_privatenetworks.literals import AcknowledgmentStatusType

def get_value() -> AcknowledgmentStatusType:
    return "ACKNOWLEDGED"
```

- [AcknowledgmentStatusType](./literals.md#acknowledgmentstatustype)
- [CommitmentLengthType](./literals.md#commitmentlengthtype)
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
- [UpdateTypeType](./literals.md#updatetypetype)
- [Private5GServiceName](./literals.md#private5gservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AcknowledgeOrderReceiptRequestTypeDef](./type_defs.md#acknowledgeorderreceiptrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ActivateDeviceIdentifierRequestTypeDef](./type_defs.md#activatedeviceidentifierrequesttypedef)
- [DeviceIdentifierTypeDef](./type_defs.md#deviceidentifiertypedef)
- [AddressTypeDef](./type_defs.md#addresstypedef)
- [CommitmentConfigurationTypeDef](./type_defs.md#commitmentconfigurationtypedef)
- [PositionTypeDef](./type_defs.md#positiontypedef)
- [CreateNetworkRequestTypeDef](./type_defs.md#createnetworkrequesttypedef)
- [NetworkTypeDef](./type_defs.md#networktypedef)
- [DeactivateDeviceIdentifierRequestTypeDef](./type_defs.md#deactivatedeviceidentifierrequesttypedef)
- [DeleteNetworkRequestTypeDef](./type_defs.md#deletenetworkrequesttypedef)
- [DeleteNetworkSiteRequestTypeDef](./type_defs.md#deletenetworksiterequesttypedef)
- [GetDeviceIdentifierRequestTypeDef](./type_defs.md#getdeviceidentifierrequesttypedef)
- [GetNetworkRequestTypeDef](./type_defs.md#getnetworkrequesttypedef)
- [GetNetworkResourceRequestTypeDef](./type_defs.md#getnetworkresourcerequesttypedef)
- [GetNetworkSiteRequestTypeDef](./type_defs.md#getnetworksiterequesttypedef)
- [GetOrderRequestTypeDef](./type_defs.md#getorderrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListDeviceIdentifiersRequestTypeDef](./type_defs.md#listdeviceidentifiersrequesttypedef)
- [ListNetworkResourcesRequestTypeDef](./type_defs.md#listnetworkresourcesrequesttypedef)
- [ListNetworkSitesRequestTypeDef](./type_defs.md#listnetworksitesrequesttypedef)
- [ListNetworksRequestTypeDef](./type_defs.md#listnetworksrequesttypedef)
- [ListOrdersRequestTypeDef](./type_defs.md#listordersrequesttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [NameValuePairTypeDef](./type_defs.md#namevaluepairtypedef)
- [TrackingInformationTypeDef](./type_defs.md#trackinginformationtypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdateNetworkSiteRequestTypeDef](./type_defs.md#updatenetworksiterequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [PingResponseTypeDef](./type_defs.md#pingresponsetypedef)
- [ActivateDeviceIdentifierResponseTypeDef](./type_defs.md#activatedeviceidentifierresponsetypedef)
- [DeactivateDeviceIdentifierResponseTypeDef](./type_defs.md#deactivatedeviceidentifierresponsetypedef)
- [GetDeviceIdentifierResponseTypeDef](./type_defs.md#getdeviceidentifierresponsetypedef)
- [ListDeviceIdentifiersResponseTypeDef](./type_defs.md#listdeviceidentifiersresponsetypedef)
- [ReturnInformationTypeDef](./type_defs.md#returninformationtypedef)
- [ActivateNetworkSiteRequestTypeDef](./type_defs.md#activatenetworksiterequesttypedef)
- [CommitmentInformationTypeDef](./type_defs.md#commitmentinformationtypedef)
- [OrderedResourceDefinitionTypeDef](./type_defs.md#orderedresourcedefinitiontypedef)
- [StartNetworkResourceUpdateRequestTypeDef](./type_defs.md#startnetworkresourceupdaterequesttypedef)
- [ConfigureAccessPointRequestTypeDef](./type_defs.md#configureaccesspointrequesttypedef)
- [CreateNetworkResponseTypeDef](./type_defs.md#createnetworkresponsetypedef)
- [DeleteNetworkResponseTypeDef](./type_defs.md#deletenetworkresponsetypedef)
- [GetNetworkResponseTypeDef](./type_defs.md#getnetworkresponsetypedef)
- [ListNetworksResponseTypeDef](./type_defs.md#listnetworksresponsetypedef)
- [ListDeviceIdentifiersRequestPaginateTypeDef](./type_defs.md#listdeviceidentifiersrequestpaginatetypedef)
- [ListNetworkResourcesRequestPaginateTypeDef](./type_defs.md#listnetworkresourcesrequestpaginatetypedef)
- [ListNetworkSitesRequestPaginateTypeDef](./type_defs.md#listnetworksitesrequestpaginatetypedef)
- [ListNetworksRequestPaginateTypeDef](./type_defs.md#listnetworksrequestpaginatetypedef)
- [ListOrdersRequestPaginateTypeDef](./type_defs.md#listordersrequestpaginatetypedef)
- [NetworkResourceDefinitionOutputTypeDef](./type_defs.md#networkresourcedefinitionoutputtypedef)
- [NetworkResourceDefinitionTypeDef](./type_defs.md#networkresourcedefinitiontypedef)
- [NetworkResourceTypeDef](./type_defs.md#networkresourcetypedef)
- [OrderTypeDef](./type_defs.md#ordertypedef)
- [SitePlanOutputTypeDef](./type_defs.md#siteplanoutputtypedef)
- [SitePlanTypeDef](./type_defs.md#siteplantypedef)
- [ConfigureAccessPointResponseTypeDef](./type_defs.md#configureaccesspointresponsetypedef)
- [GetNetworkResourceResponseTypeDef](./type_defs.md#getnetworkresourceresponsetypedef)
- [ListNetworkResourcesResponseTypeDef](./type_defs.md#listnetworkresourcesresponsetypedef)
- [StartNetworkResourceUpdateResponseTypeDef](./type_defs.md#startnetworkresourceupdateresponsetypedef)
- [AcknowledgeOrderReceiptResponseTypeDef](./type_defs.md#acknowledgeorderreceiptresponsetypedef)
- [GetOrderResponseTypeDef](./type_defs.md#getorderresponsetypedef)
- [ListOrdersResponseTypeDef](./type_defs.md#listordersresponsetypedef)
- [NetworkSiteTypeDef](./type_defs.md#networksitetypedef)
- [SitePlanUnionTypeDef](./type_defs.md#siteplanuniontypedef)
- [ActivateNetworkSiteResponseTypeDef](./type_defs.md#activatenetworksiteresponsetypedef)
- [CreateNetworkSiteResponseTypeDef](./type_defs.md#createnetworksiteresponsetypedef)
- [DeleteNetworkSiteResponseTypeDef](./type_defs.md#deletenetworksiteresponsetypedef)
- [GetNetworkSiteResponseTypeDef](./type_defs.md#getnetworksiteresponsetypedef)
- [ListNetworkSitesResponseTypeDef](./type_defs.md#listnetworksitesresponsetypedef)
- [UpdateNetworkSiteResponseTypeDef](./type_defs.md#updatenetworksiteresponsetypedef)
- [CreateNetworkSiteRequestTypeDef](./type_defs.md#createnetworksiterequesttypedef)
- [UpdateNetworkSitePlanRequestTypeDef](./type_defs.md#updatenetworksiteplanrequesttypedef)

