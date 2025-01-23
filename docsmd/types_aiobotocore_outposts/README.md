# Outposts module

> [Index](../README.md) > Outposts


!!! note ""

    Auto-generated documentation for [Outposts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#outposts)
    type annotations stubs module [types-aiobotocore-outposts](https://pypi.org/project/types-aiobotocore-outposts/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `Outposts` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `Outposts` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[outposts]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[outposts]'

# standalone installation
python -m pip install types-aiobotocore-outposts
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-outposts
```

## Usage

Code samples can be found in [Examples](./usage.md).

## OutpostsClient

Type annotations and code completion for  `#!python session.create_client("outposts")` as [OutpostsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client)

```python
# OutpostsClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_outposts.client import OutpostsClient


session = get_session()
async with session.create_client("outposts") as client:
    client: OutpostsClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("outposts").get_paginator("...")`.

```python
# GetOutpostInstanceTypesPaginator usage example

from types_aiobotocore_outposts.paginator import GetOutpostInstanceTypesPaginator

def get_get_outpost_instance_types_paginator() -> GetOutpostInstanceTypesPaginator:
    return client.get_paginator("get_outpost_instance_types"))
```

- [GetOutpostInstanceTypesPaginator](./paginators.md#getoutpostinstancetypespaginator)
- [GetOutpostSupportedInstanceTypesPaginator](./paginators.md#getoutpostsupportedinstancetypespaginator)
- [ListAssetInstancesPaginator](./paginators.md#listassetinstancespaginator)
- [ListAssetsPaginator](./paginators.md#listassetspaginator)
- [ListBlockingInstancesForCapacityTaskPaginator](./paginators.md#listblockinginstancesforcapacitytaskpaginator)
- [ListCapacityTasksPaginator](./paginators.md#listcapacitytaskspaginator)
- [ListCatalogItemsPaginator](./paginators.md#listcatalogitemspaginator)
- [ListOrdersPaginator](./paginators.md#listorderspaginator)
- [ListOutpostsPaginator](./paginators.md#listoutpostspaginator)
- [ListSitesPaginator](./paginators.md#listsitespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AWSServiceNameType usage example

from types_aiobotocore_outposts.literals import AWSServiceNameType

def get_value() -> AWSServiceNameType:
    return "AWS"
```

- [AWSServiceNameType](./literals.md#awsservicenametype)
- [AddressTypeType](./literals.md#addresstypetype)
- [AssetStateType](./literals.md#assetstatetype)
- [AssetTypeType](./literals.md#assettypetype)
- [CapacityTaskFailureTypeType](./literals.md#capacitytaskfailuretypetype)
- [CapacityTaskStatusType](./literals.md#capacitytaskstatustype)
- [CatalogItemClassType](./literals.md#catalogitemclasstype)
- [CatalogItemStatusType](./literals.md#catalogitemstatustype)
- [ComputeAssetStateType](./literals.md#computeassetstatetype)
- [FiberOpticCableTypeType](./literals.md#fiberopticcabletypetype)
- [GetOutpostInstanceTypesPaginatorName](./literals.md#getoutpostinstancetypespaginatorname)
- [GetOutpostSupportedInstanceTypesPaginatorName](./literals.md#getoutpostsupportedinstancetypespaginatorname)
- [LineItemStatusType](./literals.md#lineitemstatustype)
- [ListAssetInstancesPaginatorName](./literals.md#listassetinstancespaginatorname)
- [ListAssetsPaginatorName](./literals.md#listassetspaginatorname)
- [ListBlockingInstancesForCapacityTaskPaginatorName](./literals.md#listblockinginstancesforcapacitytaskpaginatorname)
- [ListCapacityTasksPaginatorName](./literals.md#listcapacitytaskspaginatorname)
- [ListCatalogItemsPaginatorName](./literals.md#listcatalogitemspaginatorname)
- [ListOrdersPaginatorName](./literals.md#listorderspaginatorname)
- [ListOutpostsPaginatorName](./literals.md#listoutpostspaginatorname)
- [ListSitesPaginatorName](./literals.md#listsitespaginatorname)
- [MaximumSupportedWeightLbsType](./literals.md#maximumsupportedweightlbstype)
- [OpticalStandardType](./literals.md#opticalstandardtype)
- [OrderStatusType](./literals.md#orderstatustype)
- [OrderTypeType](./literals.md#ordertypetype)
- [PaymentOptionType](./literals.md#paymentoptiontype)
- [PaymentTermType](./literals.md#paymenttermtype)
- [PowerConnectorType](./literals.md#powerconnectortype)
- [PowerDrawKvaType](./literals.md#powerdrawkvatype)
- [PowerFeedDropType](./literals.md#powerfeeddroptype)
- [PowerPhaseType](./literals.md#powerphasetype)
- [ShipmentCarrierType](./literals.md#shipmentcarriertype)
- [SupportedHardwareTypeType](./literals.md#supportedhardwaretypetype)
- [SupportedStorageEnumType](./literals.md#supportedstorageenumtype)
- [TaskActionOnBlockingInstancesType](./literals.md#taskactiononblockinginstancestype)
- [UplinkCountType](./literals.md#uplinkcounttype)
- [UplinkGbpsType](./literals.md#uplinkgbpstype)
- [OutpostsServiceName](./literals.md#outpostsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AddressTypeDef](./type_defs.md#addresstypedef)
- [AssetLocationTypeDef](./type_defs.md#assetlocationtypedef)
- [AssetInstanceTypeCapacityTypeDef](./type_defs.md#assetinstancetypecapacitytypedef)
- [AssetInstanceTypeDef](./type_defs.md#assetinstancetypedef)
- [BlockingInstanceTypeDef](./type_defs.md#blockinginstancetypedef)
- [CancelCapacityTaskInputRequestTypeDef](./type_defs.md#cancelcapacitytaskinputrequesttypedef)
- [CancelOrderInputRequestTypeDef](./type_defs.md#cancelorderinputrequesttypedef)
- [CapacityTaskFailureTypeDef](./type_defs.md#capacitytaskfailuretypedef)
- [CapacityTaskSummaryTypeDef](./type_defs.md#capacitytasksummarytypedef)
- [EC2CapacityTypeDef](./type_defs.md#ec2capacitytypedef)
- [ConnectionDetailsTypeDef](./type_defs.md#connectiondetailstypedef)
- [LineItemRequestTypeDef](./type_defs.md#lineitemrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateOutpostInputRequestTypeDef](./type_defs.md#createoutpostinputrequesttypedef)
- [OutpostTypeDef](./type_defs.md#outposttypedef)
- [RackPhysicalPropertiesTypeDef](./type_defs.md#rackphysicalpropertiestypedef)
- [DeleteOutpostInputRequestTypeDef](./type_defs.md#deleteoutpostinputrequesttypedef)
- [DeleteSiteInputRequestTypeDef](./type_defs.md#deletesiteinputrequesttypedef)
- [GetCapacityTaskInputRequestTypeDef](./type_defs.md#getcapacitytaskinputrequesttypedef)
- [InstanceTypeCapacityTypeDef](./type_defs.md#instancetypecapacitytypedef)
- [InstancesToExcludeOutputTypeDef](./type_defs.md#instancestoexcludeoutputtypedef)
- [GetCatalogItemInputRequestTypeDef](./type_defs.md#getcatalogiteminputrequesttypedef)
- [GetConnectionRequestRequestTypeDef](./type_defs.md#getconnectionrequestrequesttypedef)
- [GetOrderInputRequestTypeDef](./type_defs.md#getorderinputrequesttypedef)
- [GetOutpostInputRequestTypeDef](./type_defs.md#getoutpostinputrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [GetOutpostInstanceTypesInputRequestTypeDef](./type_defs.md#getoutpostinstancetypesinputrequesttypedef)
- [InstanceTypeItemTypeDef](./type_defs.md#instancetypeitemtypedef)
- [GetOutpostSupportedInstanceTypesInputRequestTypeDef](./type_defs.md#getoutpostsupportedinstancetypesinputrequesttypedef)
- [GetSiteAddressInputRequestTypeDef](./type_defs.md#getsiteaddressinputrequesttypedef)
- [GetSiteInputRequestTypeDef](./type_defs.md#getsiteinputrequesttypedef)
- [InstancesToExcludeTypeDef](./type_defs.md#instancestoexcludetypedef)
- [LineItemAssetInformationTypeDef](./type_defs.md#lineitemassetinformationtypedef)
- [ShipmentInformationTypeDef](./type_defs.md#shipmentinformationtypedef)
- [ListAssetInstancesInputRequestTypeDef](./type_defs.md#listassetinstancesinputrequesttypedef)
- [ListAssetsInputRequestTypeDef](./type_defs.md#listassetsinputrequesttypedef)
- [ListBlockingInstancesForCapacityTaskInputRequestTypeDef](./type_defs.md#listblockinginstancesforcapacitytaskinputrequesttypedef)
- [ListCapacityTasksInputRequestTypeDef](./type_defs.md#listcapacitytasksinputrequesttypedef)
- [ListCatalogItemsInputRequestTypeDef](./type_defs.md#listcatalogitemsinputrequesttypedef)
- [ListOrdersInputRequestTypeDef](./type_defs.md#listordersinputrequesttypedef)
- [OrderSummaryTypeDef](./type_defs.md#ordersummarytypedef)
- [ListOutpostsInputRequestTypeDef](./type_defs.md#listoutpostsinputrequesttypedef)
- [ListSitesInputRequestTypeDef](./type_defs.md#listsitesinputrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [StartConnectionRequestRequestTypeDef](./type_defs.md#startconnectionrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateOutpostInputRequestTypeDef](./type_defs.md#updateoutpostinputrequesttypedef)
- [UpdateSiteInputRequestTypeDef](./type_defs.md#updatesiteinputrequesttypedef)
- [UpdateSiteRackPhysicalPropertiesInputRequestTypeDef](./type_defs.md#updatesiterackphysicalpropertiesinputrequesttypedef)
- [UpdateSiteAddressInputRequestTypeDef](./type_defs.md#updatesiteaddressinputrequesttypedef)
- [ComputeAttributesTypeDef](./type_defs.md#computeattributestypedef)
- [CatalogItemTypeDef](./type_defs.md#catalogitemtypedef)
- [CreateOrderInputRequestTypeDef](./type_defs.md#createorderinputrequesttypedef)
- [GetConnectionResponseTypeDef](./type_defs.md#getconnectionresponsetypedef)
- [GetSiteAddressOutputTypeDef](./type_defs.md#getsiteaddressoutputtypedef)
- [ListAssetInstancesOutputTypeDef](./type_defs.md#listassetinstancesoutputtypedef)
- [ListBlockingInstancesForCapacityTaskOutputTypeDef](./type_defs.md#listblockinginstancesforcapacitytaskoutputtypedef)
- [ListCapacityTasksOutputTypeDef](./type_defs.md#listcapacitytasksoutputtypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [StartConnectionResponseTypeDef](./type_defs.md#startconnectionresponsetypedef)
- [UpdateSiteAddressOutputTypeDef](./type_defs.md#updatesiteaddressoutputtypedef)
- [CreateOutpostOutputTypeDef](./type_defs.md#createoutpostoutputtypedef)
- [GetOutpostOutputTypeDef](./type_defs.md#getoutpostoutputtypedef)
- [ListOutpostsOutputTypeDef](./type_defs.md#listoutpostsoutputtypedef)
- [UpdateOutpostOutputTypeDef](./type_defs.md#updateoutpostoutputtypedef)
- [CreateSiteInputRequestTypeDef](./type_defs.md#createsiteinputrequesttypedef)
- [SiteTypeDef](./type_defs.md#sitetypedef)
- [GetCapacityTaskOutputTypeDef](./type_defs.md#getcapacitytaskoutputtypedef)
- [StartCapacityTaskOutputTypeDef](./type_defs.md#startcapacitytaskoutputtypedef)
- [GetOutpostInstanceTypesInputPaginateTypeDef](./type_defs.md#getoutpostinstancetypesinputpaginatetypedef)
- [GetOutpostSupportedInstanceTypesInputPaginateTypeDef](./type_defs.md#getoutpostsupportedinstancetypesinputpaginatetypedef)
- [ListAssetInstancesInputPaginateTypeDef](./type_defs.md#listassetinstancesinputpaginatetypedef)
- [ListAssetsInputPaginateTypeDef](./type_defs.md#listassetsinputpaginatetypedef)
- [ListBlockingInstancesForCapacityTaskInputPaginateTypeDef](./type_defs.md#listblockinginstancesforcapacitytaskinputpaginatetypedef)
- [ListCapacityTasksInputPaginateTypeDef](./type_defs.md#listcapacitytasksinputpaginatetypedef)
- [ListCatalogItemsInputPaginateTypeDef](./type_defs.md#listcatalogitemsinputpaginatetypedef)
- [ListOrdersInputPaginateTypeDef](./type_defs.md#listordersinputpaginatetypedef)
- [ListOutpostsInputPaginateTypeDef](./type_defs.md#listoutpostsinputpaginatetypedef)
- [ListSitesInputPaginateTypeDef](./type_defs.md#listsitesinputpaginatetypedef)
- [GetOutpostInstanceTypesOutputTypeDef](./type_defs.md#getoutpostinstancetypesoutputtypedef)
- [GetOutpostSupportedInstanceTypesOutputTypeDef](./type_defs.md#getoutpostsupportedinstancetypesoutputtypedef)
- [StartCapacityTaskInputRequestTypeDef](./type_defs.md#startcapacitytaskinputrequesttypedef)
- [LineItemTypeDef](./type_defs.md#lineitemtypedef)
- [ListOrdersOutputTypeDef](./type_defs.md#listordersoutputtypedef)
- [AssetInfoTypeDef](./type_defs.md#assetinfotypedef)
- [GetCatalogItemOutputTypeDef](./type_defs.md#getcatalogitemoutputtypedef)
- [ListCatalogItemsOutputTypeDef](./type_defs.md#listcatalogitemsoutputtypedef)
- [CreateSiteOutputTypeDef](./type_defs.md#createsiteoutputtypedef)
- [GetSiteOutputTypeDef](./type_defs.md#getsiteoutputtypedef)
- [ListSitesOutputTypeDef](./type_defs.md#listsitesoutputtypedef)
- [UpdateSiteOutputTypeDef](./type_defs.md#updatesiteoutputtypedef)
- [UpdateSiteRackPhysicalPropertiesOutputTypeDef](./type_defs.md#updatesiterackphysicalpropertiesoutputtypedef)
- [OrderTypeDef](./type_defs.md#ordertypedef)
- [ListAssetsOutputTypeDef](./type_defs.md#listassetsoutputtypedef)
- [CreateOrderOutputTypeDef](./type_defs.md#createorderoutputtypedef)
- [GetOrderOutputTypeDef](./type_defs.md#getorderoutputtypedef)

