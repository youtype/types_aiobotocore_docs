# MediaPackageVod module

> [Index](../README.md) > MediaPackageVod


!!! note ""

    Auto-generated documentation for [MediaPackageVod](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#mediapackagevod)
    type annotations stubs module [types-aiobotocore-mediapackage-vod](https://pypi.org/project/types-aiobotocore-mediapackage-vod/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `MediaPackageVod` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `MediaPackageVod` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[mediapackage-vod]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[mediapackage-vod]'

# standalone installation
python -m pip install types-aiobotocore-mediapackage-vod
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-mediapackage-vod
```

## Usage

Code samples can be found in [Examples](./usage.md).

## MediaPackageVodClient

Type annotations and code completion for  `#!python session.create_client("mediapackage-vod")` as [MediaPackageVodClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#MediaPackageVod.Client)

```python
# MediaPackageVodClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_mediapackage_vod.client import MediaPackageVodClient


session = get_session()
async with session.create_client("mediapackage-vod") as client:
    client: MediaPackageVodClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("mediapackage-vod").get_paginator("...")`.

```python
# ListAssetsPaginator usage example

from types_aiobotocore_mediapackage_vod.paginator import ListAssetsPaginator

def get_list_assets_paginator() -> ListAssetsPaginator:
    return client.get_paginator("list_assets"))
```

- [ListAssetsPaginator](./paginators.md#listassetspaginator)
- [ListPackagingConfigurationsPaginator](./paginators.md#listpackagingconfigurationspaginator)
- [ListPackagingGroupsPaginator](./paginators.md#listpackaginggroupspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AdMarkersType usage example

from types_aiobotocore_mediapackage_vod.literals import AdMarkersType

def get_value() -> AdMarkersType:
    return "NONE"
```

- [AdMarkersType](./literals.md#admarkerstype)
- [EncryptionMethodType](./literals.md#encryptionmethodtype)
- [ListAssetsPaginatorName](./literals.md#listassetspaginatorname)
- [ListPackagingConfigurationsPaginatorName](./literals.md#listpackagingconfigurationspaginatorname)
- [ListPackagingGroupsPaginatorName](./literals.md#listpackaginggroupspaginatorname)
- [ManifestLayoutType](./literals.md#manifestlayouttype)
- [PeriodTriggersElementType](./literals.md#periodtriggerselementtype)
- [PresetSpeke20AudioType](./literals.md#presetspeke20audiotype)
- [PresetSpeke20VideoType](./literals.md#presetspeke20videotype)
- [ProfileType](./literals.md#profiletype)
- [ScteMarkersSourceType](./literals.md#sctemarkerssourcetype)
- [SegmentTemplateFormatType](./literals.md#segmenttemplateformattype)
- [StreamOrderType](./literals.md#streamordertype)
- [MediaPackageVodServiceName](./literals.md#mediapackagevodservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AssetShallowTypeDef](./type_defs.md#assetshallowtypedef)
- [AuthorizationTypeDef](./type_defs.md#authorizationtypedef)
- [EgressAccessLogsTypeDef](./type_defs.md#egressaccesslogstypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateAssetRequestTypeDef](./type_defs.md#createassetrequesttypedef)
- [EgressEndpointTypeDef](./type_defs.md#egressendpointtypedef)
- [StreamSelectionTypeDef](./type_defs.md#streamselectiontypedef)
- [DeleteAssetRequestTypeDef](./type_defs.md#deleteassetrequesttypedef)
- [DeletePackagingConfigurationRequestTypeDef](./type_defs.md#deletepackagingconfigurationrequesttypedef)
- [DeletePackagingGroupRequestTypeDef](./type_defs.md#deletepackaginggrouprequesttypedef)
- [DescribeAssetRequestTypeDef](./type_defs.md#describeassetrequesttypedef)
- [DescribePackagingConfigurationRequestTypeDef](./type_defs.md#describepackagingconfigurationrequesttypedef)
- [DescribePackagingGroupRequestTypeDef](./type_defs.md#describepackaginggrouprequesttypedef)
- [EncryptionContractConfigurationTypeDef](./type_defs.md#encryptioncontractconfigurationtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAssetsRequestTypeDef](./type_defs.md#listassetsrequesttypedef)
- [ListPackagingConfigurationsRequestTypeDef](./type_defs.md#listpackagingconfigurationsrequesttypedef)
- [ListPackagingGroupsRequestTypeDef](./type_defs.md#listpackaginggroupsrequesttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdatePackagingGroupRequestTypeDef](./type_defs.md#updatepackaginggrouprequesttypedef)
- [ConfigureLogsRequestTypeDef](./type_defs.md#configurelogsrequesttypedef)
- [CreatePackagingGroupRequestTypeDef](./type_defs.md#createpackaginggrouprequesttypedef)
- [PackagingGroupTypeDef](./type_defs.md#packaginggrouptypedef)
- [ConfigureLogsResponseTypeDef](./type_defs.md#configurelogsresponsetypedef)
- [CreatePackagingGroupResponseTypeDef](./type_defs.md#createpackaginggroupresponsetypedef)
- [DescribePackagingGroupResponseTypeDef](./type_defs.md#describepackaginggroupresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ListAssetsResponseTypeDef](./type_defs.md#listassetsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [UpdatePackagingGroupResponseTypeDef](./type_defs.md#updatepackaginggroupresponsetypedef)
- [CreateAssetResponseTypeDef](./type_defs.md#createassetresponsetypedef)
- [DescribeAssetResponseTypeDef](./type_defs.md#describeassetresponsetypedef)
- [DashManifestTypeDef](./type_defs.md#dashmanifesttypedef)
- [HlsManifestTypeDef](./type_defs.md#hlsmanifesttypedef)
- [MssManifestTypeDef](./type_defs.md#mssmanifesttypedef)
- [SpekeKeyProviderOutputTypeDef](./type_defs.md#spekekeyprovideroutputtypedef)
- [SpekeKeyProviderTypeDef](./type_defs.md#spekekeyprovidertypedef)
- [ListAssetsRequestPaginateTypeDef](./type_defs.md#listassetsrequestpaginatetypedef)
- [ListPackagingConfigurationsRequestPaginateTypeDef](./type_defs.md#listpackagingconfigurationsrequestpaginatetypedef)
- [ListPackagingGroupsRequestPaginateTypeDef](./type_defs.md#listpackaginggroupsrequestpaginatetypedef)
- [ListPackagingGroupsResponseTypeDef](./type_defs.md#listpackaginggroupsresponsetypedef)
- [CmafEncryptionOutputTypeDef](./type_defs.md#cmafencryptionoutputtypedef)
- [DashEncryptionOutputTypeDef](./type_defs.md#dashencryptionoutputtypedef)
- [HlsEncryptionOutputTypeDef](./type_defs.md#hlsencryptionoutputtypedef)
- [MssEncryptionOutputTypeDef](./type_defs.md#mssencryptionoutputtypedef)
- [CmafEncryptionTypeDef](./type_defs.md#cmafencryptiontypedef)
- [DashEncryptionTypeDef](./type_defs.md#dashencryptiontypedef)
- [HlsEncryptionTypeDef](./type_defs.md#hlsencryptiontypedef)
- [MssEncryptionTypeDef](./type_defs.md#mssencryptiontypedef)
- [CmafPackageOutputTypeDef](./type_defs.md#cmafpackageoutputtypedef)
- [DashPackageOutputTypeDef](./type_defs.md#dashpackageoutputtypedef)
- [HlsPackageOutputTypeDef](./type_defs.md#hlspackageoutputtypedef)
- [MssPackageOutputTypeDef](./type_defs.md#msspackageoutputtypedef)
- [CmafPackageTypeDef](./type_defs.md#cmafpackagetypedef)
- [DashPackageTypeDef](./type_defs.md#dashpackagetypedef)
- [HlsPackageTypeDef](./type_defs.md#hlspackagetypedef)
- [MssPackageTypeDef](./type_defs.md#msspackagetypedef)
- [CreatePackagingConfigurationResponseTypeDef](./type_defs.md#createpackagingconfigurationresponsetypedef)
- [DescribePackagingConfigurationResponseTypeDef](./type_defs.md#describepackagingconfigurationresponsetypedef)
- [PackagingConfigurationTypeDef](./type_defs.md#packagingconfigurationtypedef)
- [CmafPackageUnionTypeDef](./type_defs.md#cmafpackageuniontypedef)
- [DashPackageUnionTypeDef](./type_defs.md#dashpackageuniontypedef)
- [HlsPackageUnionTypeDef](./type_defs.md#hlspackageuniontypedef)
- [MssPackageUnionTypeDef](./type_defs.md#msspackageuniontypedef)
- [ListPackagingConfigurationsResponseTypeDef](./type_defs.md#listpackagingconfigurationsresponsetypedef)
- [CreatePackagingConfigurationRequestTypeDef](./type_defs.md#createpackagingconfigurationrequesttypedef)

