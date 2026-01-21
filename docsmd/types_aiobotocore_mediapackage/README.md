# MediaPackage module

> [Index](../README.md) > MediaPackage


!!! note ""

    Auto-generated documentation for [MediaPackage](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#mediapackage)
    type annotations stubs module [types-aiobotocore-mediapackage](https://pypi.org/project/types-aiobotocore-mediapackage/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `MediaPackage` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `MediaPackage` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[mediapackage]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[mediapackage]'

# standalone installation
python -m pip install types-aiobotocore-mediapackage
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-mediapackage
```

## Usage

Code samples can be found in [Examples](./usage.md).

## MediaPackageClient

Type annotations and code completion for  `#!python session.create_client("mediapackage")` as [MediaPackageClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#MediaPackage.Client)

```python
# MediaPackageClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_mediapackage.client import MediaPackageClient


session = get_session()
async with session.create_client("mediapackage") as client:
    client: MediaPackageClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("mediapackage").get_paginator("...")`.

```python
# ListChannelsPaginator usage example

from types_aiobotocore_mediapackage.paginator import ListChannelsPaginator

def get_list_channels_paginator() -> ListChannelsPaginator:
    return client.get_paginator("list_channels"))
```

- [ListChannelsPaginator](./paginators.md#listchannelspaginator)
- [ListHarvestJobsPaginator](./paginators.md#listharvestjobspaginator)
- [ListOriginEndpointsPaginator](./paginators.md#listoriginendpointspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AdMarkersType usage example

from types_aiobotocore_mediapackage.literals import AdMarkersType

def get_value() -> AdMarkersType:
    return "DATERANGE"
```

- [AdMarkersType](./literals.md#admarkerstype)
- [AdTriggersElementType](./literals.md#adtriggerselementtype)
- [AdsOnDeliveryRestrictionsType](./literals.md#adsondeliveryrestrictionstype)
- [CmafEncryptionMethodType](./literals.md#cmafencryptionmethodtype)
- [EncryptionMethodType](./literals.md#encryptionmethodtype)
- [ListChannelsPaginatorName](./literals.md#listchannelspaginatorname)
- [ListHarvestJobsPaginatorName](./literals.md#listharvestjobspaginatorname)
- [ListOriginEndpointsPaginatorName](./literals.md#listoriginendpointspaginatorname)
- [ManifestLayoutType](./literals.md#manifestlayouttype)
- [OriginationType](./literals.md#originationtype)
- [PeriodTriggersElementType](./literals.md#periodtriggerselementtype)
- [PlaylistTypeType](./literals.md#playlisttypetype)
- [PresetSpeke20AudioType](./literals.md#presetspeke20audiotype)
- [PresetSpeke20VideoType](./literals.md#presetspeke20videotype)
- [ProfileType](./literals.md#profiletype)
- [SegmentTemplateFormatType](./literals.md#segmenttemplateformattype)
- [StatusType](./literals.md#statustype)
- [StreamOrderType](./literals.md#streamordertype)
- [UtcTimingType](./literals.md#utctimingtype)
- [MediaPackageServiceName](./literals.md#mediapackageservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AuthorizationTypeDef](./type_defs.md#authorizationtypedef)
- [EgressAccessLogsTypeDef](./type_defs.md#egressaccesslogstypedef)
- [IngressAccessLogsTypeDef](./type_defs.md#ingressaccesslogstypedef)
- [HlsManifestCreateOrUpdateParametersTypeDef](./type_defs.md#hlsmanifestcreateorupdateparameterstypedef)
- [StreamSelectionTypeDef](./type_defs.md#streamselectiontypedef)
- [HlsManifestTypeDef](./type_defs.md#hlsmanifesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateChannelRequestTypeDef](./type_defs.md#createchannelrequesttypedef)
- [S3DestinationTypeDef](./type_defs.md#s3destinationtypedef)
- [DeleteChannelRequestTypeDef](./type_defs.md#deletechannelrequesttypedef)
- [DeleteOriginEndpointRequestTypeDef](./type_defs.md#deleteoriginendpointrequesttypedef)
- [DescribeChannelRequestTypeDef](./type_defs.md#describechannelrequesttypedef)
- [DescribeHarvestJobRequestTypeDef](./type_defs.md#describeharvestjobrequesttypedef)
- [DescribeOriginEndpointRequestTypeDef](./type_defs.md#describeoriginendpointrequesttypedef)
- [EncryptionContractConfigurationTypeDef](./type_defs.md#encryptioncontractconfigurationtypedef)
- [IngestEndpointTypeDef](./type_defs.md#ingestendpointtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListChannelsRequestTypeDef](./type_defs.md#listchannelsrequesttypedef)
- [ListHarvestJobsRequestTypeDef](./type_defs.md#listharvestjobsrequesttypedef)
- [ListOriginEndpointsRequestTypeDef](./type_defs.md#listoriginendpointsrequesttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [RotateChannelCredentialsRequestTypeDef](./type_defs.md#rotatechannelcredentialsrequesttypedef)
- [RotateIngestEndpointCredentialsRequestTypeDef](./type_defs.md#rotateingestendpointcredentialsrequesttypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdateChannelRequestTypeDef](./type_defs.md#updatechannelrequesttypedef)
- [ConfigureLogsRequestTypeDef](./type_defs.md#configurelogsrequesttypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [CreateHarvestJobRequestTypeDef](./type_defs.md#createharvestjobrequesttypedef)
- [CreateHarvestJobResponseTypeDef](./type_defs.md#createharvestjobresponsetypedef)
- [DescribeHarvestJobResponseTypeDef](./type_defs.md#describeharvestjobresponsetypedef)
- [HarvestJobTypeDef](./type_defs.md#harvestjobtypedef)
- [SpekeKeyProviderOutputTypeDef](./type_defs.md#spekekeyprovideroutputtypedef)
- [SpekeKeyProviderTypeDef](./type_defs.md#spekekeyprovidertypedef)
- [HlsIngestTypeDef](./type_defs.md#hlsingesttypedef)
- [ListChannelsRequestPaginateTypeDef](./type_defs.md#listchannelsrequestpaginatetypedef)
- [ListHarvestJobsRequestPaginateTypeDef](./type_defs.md#listharvestjobsrequestpaginatetypedef)
- [ListOriginEndpointsRequestPaginateTypeDef](./type_defs.md#listoriginendpointsrequestpaginatetypedef)
- [ListHarvestJobsResponseTypeDef](./type_defs.md#listharvestjobsresponsetypedef)
- [CmafEncryptionOutputTypeDef](./type_defs.md#cmafencryptionoutputtypedef)
- [DashEncryptionOutputTypeDef](./type_defs.md#dashencryptionoutputtypedef)
- [HlsEncryptionOutputTypeDef](./type_defs.md#hlsencryptionoutputtypedef)
- [MssEncryptionOutputTypeDef](./type_defs.md#mssencryptionoutputtypedef)
- [DashEncryptionTypeDef](./type_defs.md#dashencryptiontypedef)
- [HlsEncryptionTypeDef](./type_defs.md#hlsencryptiontypedef)
- [MssEncryptionTypeDef](./type_defs.md#mssencryptiontypedef)
- [SpekeKeyProviderUnionTypeDef](./type_defs.md#spekekeyprovideruniontypedef)
- [ChannelTypeDef](./type_defs.md#channeltypedef)
- [ConfigureLogsResponseTypeDef](./type_defs.md#configurelogsresponsetypedef)
- [CreateChannelResponseTypeDef](./type_defs.md#createchannelresponsetypedef)
- [DescribeChannelResponseTypeDef](./type_defs.md#describechannelresponsetypedef)
- [RotateChannelCredentialsResponseTypeDef](./type_defs.md#rotatechannelcredentialsresponsetypedef)
- [RotateIngestEndpointCredentialsResponseTypeDef](./type_defs.md#rotateingestendpointcredentialsresponsetypedef)
- [UpdateChannelResponseTypeDef](./type_defs.md#updatechannelresponsetypedef)
- [CmafPackageTypeDef](./type_defs.md#cmafpackagetypedef)
- [DashPackageOutputTypeDef](./type_defs.md#dashpackageoutputtypedef)
- [HlsPackageOutputTypeDef](./type_defs.md#hlspackageoutputtypedef)
- [MssPackageOutputTypeDef](./type_defs.md#msspackageoutputtypedef)
- [DashPackageTypeDef](./type_defs.md#dashpackagetypedef)
- [HlsPackageTypeDef](./type_defs.md#hlspackagetypedef)
- [MssPackageTypeDef](./type_defs.md#msspackagetypedef)
- [CmafEncryptionTypeDef](./type_defs.md#cmafencryptiontypedef)
- [ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef)
- [CreateOriginEndpointResponseTypeDef](./type_defs.md#createoriginendpointresponsetypedef)
- [DescribeOriginEndpointResponseTypeDef](./type_defs.md#describeoriginendpointresponsetypedef)
- [OriginEndpointTypeDef](./type_defs.md#originendpointtypedef)
- [UpdateOriginEndpointResponseTypeDef](./type_defs.md#updateoriginendpointresponsetypedef)
- [DashPackageUnionTypeDef](./type_defs.md#dashpackageuniontypedef)
- [HlsPackageUnionTypeDef](./type_defs.md#hlspackageuniontypedef)
- [MssPackageUnionTypeDef](./type_defs.md#msspackageuniontypedef)
- [CmafEncryptionUnionTypeDef](./type_defs.md#cmafencryptionuniontypedef)
- [ListOriginEndpointsResponseTypeDef](./type_defs.md#listoriginendpointsresponsetypedef)
- [CmafPackageCreateOrUpdateParametersTypeDef](./type_defs.md#cmafpackagecreateorupdateparameterstypedef)
- [CreateOriginEndpointRequestTypeDef](./type_defs.md#createoriginendpointrequesttypedef)
- [UpdateOriginEndpointRequestTypeDef](./type_defs.md#updateoriginendpointrequesttypedef)

