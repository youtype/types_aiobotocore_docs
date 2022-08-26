# Snowball module

> [Index](../README.md) > Snowball


!!! note ""

    Auto-generated documentation for [Snowball](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
    type annotations stubs module [types-aiobotocore-snowball](https://pypi.org/project/types-aiobotocore-snowball/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `Snowball` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[snowball]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[snowball]'


# standalone installation
python -m pip install types-aiobotocore-snowball
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-snowball
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SnowballClient

Type annotations and code completion for  `#!python session.create_client("snowball")` as [SnowballClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_snowball.client import SnowballClient


session = get_session()
async with session.create_client("snowball") as client:
    client: SnowballClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("snowball").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_snowball.paginator import DescribeAddressesPaginator

def get_describe_addresses_paginator() -> DescribeAddressesPaginator:
    return client.get_paginator("describe_addresses"))
```

- [DescribeAddressesPaginator](./paginators.md#describeaddressespaginator)
- [ListClusterJobsPaginator](./paginators.md#listclusterjobspaginator)
- [ListClustersPaginator](./paginators.md#listclusterspaginator)
- [ListCompatibleImagesPaginator](./paginators.md#listcompatibleimagespaginator)
- [ListJobsPaginator](./paginators.md#listjobspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_snowball.literals import ClusterStateType

def get_value() -> ClusterStateType:
    return "AwaitingQuorum"
```

- [ClusterStateType](./literals.md#clusterstatetype)
- [DescribeAddressesPaginatorName](./literals.md#describeaddressespaginatorname)
- [DeviceServiceNameType](./literals.md#deviceservicenametype)
- [JobStateType](./literals.md#jobstatetype)
- [JobTypeType](./literals.md#jobtypetype)
- [ListClusterJobsPaginatorName](./literals.md#listclusterjobspaginatorname)
- [ListClustersPaginatorName](./literals.md#listclusterspaginatorname)
- [ListCompatibleImagesPaginatorName](./literals.md#listcompatibleimagespaginatorname)
- [ListJobsPaginatorName](./literals.md#listjobspaginatorname)
- [LongTermPricingTypeType](./literals.md#longtermpricingtypetype)
- [RemoteManagementType](./literals.md#remotemanagementtype)
- [ShipmentStateType](./literals.md#shipmentstatetype)
- [ShippingLabelStatusType](./literals.md#shippinglabelstatustype)
- [ShippingOptionType](./literals.md#shippingoptiontype)
- [SnowballCapacityType](./literals.md#snowballcapacitytype)
- [SnowballTypeType](./literals.md#snowballtypetype)
- [StorageUnitType](./literals.md#storageunittype)
- [TransferOptionType](./literals.md#transferoptiontype)
- [SnowballServiceName](./literals.md#snowballservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_snowball.type_defs import AddressTypeDef

def get_value() -> AddressTypeDef:
    return {
        "AddressId": ...,
    }
```

- [AddressTypeDef](./type_defs.md#addresstypedef)
- [CancelClusterRequestRequestTypeDef](./type_defs.md#cancelclusterrequestrequesttypedef)
- [CancelJobRequestRequestTypeDef](./type_defs.md#canceljobrequestrequesttypedef)
- [ClusterListEntryTypeDef](./type_defs.md#clusterlistentrytypedef)
- [NotificationTypeDef](./type_defs.md#notificationtypedef)
- [CompatibleImageTypeDef](./type_defs.md#compatibleimagetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateLongTermPricingRequestRequestTypeDef](./type_defs.md#createlongtermpricingrequestrequesttypedef)
- [CreateReturnShippingLabelRequestRequestTypeDef](./type_defs.md#createreturnshippinglabelrequestrequesttypedef)
- [DataTransferTypeDef](./type_defs.md#datatransfertypedef)
- [DescribeAddressRequestRequestTypeDef](./type_defs.md#describeaddressrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeAddressesRequestRequestTypeDef](./type_defs.md#describeaddressesrequestrequesttypedef)
- [DescribeClusterRequestRequestTypeDef](./type_defs.md#describeclusterrequestrequesttypedef)
- [DescribeJobRequestRequestTypeDef](./type_defs.md#describejobrequestrequesttypedef)
- [DescribeReturnShippingLabelRequestRequestTypeDef](./type_defs.md#describereturnshippinglabelrequestrequesttypedef)
- [Ec2AmiResourceTypeDef](./type_defs.md#ec2amiresourcetypedef)
- [EventTriggerDefinitionTypeDef](./type_defs.md#eventtriggerdefinitiontypedef)
- [GetJobManifestRequestRequestTypeDef](./type_defs.md#getjobmanifestrequestrequesttypedef)
- [GetJobUnlockCodeRequestRequestTypeDef](./type_defs.md#getjobunlockcoderequestrequesttypedef)
- [GetSoftwareUpdatesRequestRequestTypeDef](./type_defs.md#getsoftwareupdatesrequestrequesttypedef)
- [INDTaxDocumentsTypeDef](./type_defs.md#indtaxdocumentstypedef)
- [JobListEntryTypeDef](./type_defs.md#joblistentrytypedef)
- [JobLogsTypeDef](./type_defs.md#joblogstypedef)
- [KeyRangeTypeDef](./type_defs.md#keyrangetypedef)
- [ListClusterJobsRequestRequestTypeDef](./type_defs.md#listclusterjobsrequestrequesttypedef)
- [ListClustersRequestRequestTypeDef](./type_defs.md#listclustersrequestrequesttypedef)
- [ListCompatibleImagesRequestRequestTypeDef](./type_defs.md#listcompatibleimagesrequestrequesttypedef)
- [ListJobsRequestRequestTypeDef](./type_defs.md#listjobsrequestrequesttypedef)
- [ListLongTermPricingRequestRequestTypeDef](./type_defs.md#listlongtermpricingrequestrequesttypedef)
- [LongTermPricingListEntryTypeDef](./type_defs.md#longtermpricinglistentrytypedef)
- [NFSOnDeviceServiceConfigurationTypeDef](./type_defs.md#nfsondeviceserviceconfigurationtypedef)
- [TGWOnDeviceServiceConfigurationTypeDef](./type_defs.md#tgwondeviceserviceconfigurationtypedef)
- [TargetOnDeviceServiceTypeDef](./type_defs.md#targetondeviceservicetypedef)
- [ShipmentTypeDef](./type_defs.md#shipmenttypedef)
- [WirelessConnectionTypeDef](./type_defs.md#wirelessconnectiontypedef)
- [UpdateJobShipmentStateRequestRequestTypeDef](./type_defs.md#updatejobshipmentstaterequestrequesttypedef)
- [UpdateLongTermPricingRequestRequestTypeDef](./type_defs.md#updatelongtermpricingrequestrequesttypedef)
- [CreateAddressRequestRequestTypeDef](./type_defs.md#createaddressrequestrequesttypedef)
- [CreateAddressResultTypeDef](./type_defs.md#createaddressresulttypedef)
- [CreateClusterResultTypeDef](./type_defs.md#createclusterresulttypedef)
- [CreateJobResultTypeDef](./type_defs.md#createjobresulttypedef)
- [CreateLongTermPricingResultTypeDef](./type_defs.md#createlongtermpricingresulttypedef)
- [CreateReturnShippingLabelResultTypeDef](./type_defs.md#createreturnshippinglabelresulttypedef)
- [DescribeAddressResultTypeDef](./type_defs.md#describeaddressresulttypedef)
- [DescribeAddressesResultTypeDef](./type_defs.md#describeaddressesresulttypedef)
- [DescribeReturnShippingLabelResultTypeDef](./type_defs.md#describereturnshippinglabelresulttypedef)
- [GetJobManifestResultTypeDef](./type_defs.md#getjobmanifestresulttypedef)
- [GetJobUnlockCodeResultTypeDef](./type_defs.md#getjobunlockcoderesulttypedef)
- [GetSnowballUsageResultTypeDef](./type_defs.md#getsnowballusageresulttypedef)
- [GetSoftwareUpdatesResultTypeDef](./type_defs.md#getsoftwareupdatesresulttypedef)
- [ListClustersResultTypeDef](./type_defs.md#listclustersresulttypedef)
- [ListCompatibleImagesResultTypeDef](./type_defs.md#listcompatibleimagesresulttypedef)
- [DescribeAddressesRequestDescribeAddressesPaginateTypeDef](./type_defs.md#describeaddressesrequestdescribeaddressespaginatetypedef)
- [ListClusterJobsRequestListClusterJobsPaginateTypeDef](./type_defs.md#listclusterjobsrequestlistclusterjobspaginatetypedef)
- [ListClustersRequestListClustersPaginateTypeDef](./type_defs.md#listclustersrequestlistclusterspaginatetypedef)
- [ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef](./type_defs.md#listcompatibleimagesrequestlistcompatibleimagespaginatetypedef)
- [ListJobsRequestListJobsPaginateTypeDef](./type_defs.md#listjobsrequestlistjobspaginatetypedef)
- [LambdaResourceTypeDef](./type_defs.md#lambdaresourcetypedef)
- [TaxDocumentsTypeDef](./type_defs.md#taxdocumentstypedef)
- [ListClusterJobsResultTypeDef](./type_defs.md#listclusterjobsresulttypedef)
- [ListJobsResultTypeDef](./type_defs.md#listjobsresulttypedef)
- [ListLongTermPricingResultTypeDef](./type_defs.md#listlongtermpricingresulttypedef)
- [OnDeviceServiceConfigurationTypeDef](./type_defs.md#ondeviceserviceconfigurationtypedef)
- [S3ResourceTypeDef](./type_defs.md#s3resourcetypedef)
- [ShippingDetailsTypeDef](./type_defs.md#shippingdetailstypedef)
- [SnowconeDeviceConfigurationTypeDef](./type_defs.md#snowconedeviceconfigurationtypedef)
- [JobResourceTypeDef](./type_defs.md#jobresourcetypedef)
- [DeviceConfigurationTypeDef](./type_defs.md#deviceconfigurationtypedef)
- [ClusterMetadataTypeDef](./type_defs.md#clustermetadatatypedef)
- [CreateClusterRequestRequestTypeDef](./type_defs.md#createclusterrequestrequesttypedef)
- [UpdateClusterRequestRequestTypeDef](./type_defs.md#updateclusterrequestrequesttypedef)
- [UpdateJobRequestRequestTypeDef](./type_defs.md#updatejobrequestrequesttypedef)
- [CreateJobRequestRequestTypeDef](./type_defs.md#createjobrequestrequesttypedef)
- [JobMetadataTypeDef](./type_defs.md#jobmetadatatypedef)
- [DescribeClusterResultTypeDef](./type_defs.md#describeclusterresulttypedef)
- [DescribeJobResultTypeDef](./type_defs.md#describejobresulttypedef)

