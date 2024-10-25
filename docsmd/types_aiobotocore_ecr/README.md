# ECR module

> [Index](../README.md) > ECR


!!! note ""

    Auto-generated documentation for [ECR](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
    type annotations stubs module [types-aiobotocore-ecr](https://pypi.org/project/types-aiobotocore-ecr/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `ECR` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[ecr]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[ecr]'


# standalone installation
python -m pip install types-aiobotocore-ecr
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-ecr
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ECRClient

Type annotations and code completion for  `#!python session.create_client("ecr")` as [ECRClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client)

```python
# ECRClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_ecr.client import ECRClient


session = get_session()
async with session.create_client("ecr") as client:
    client: ECRClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("ecr").get_paginator("...")`.

```python
# DescribeImageScanFindingsPaginator usage example

from types_aiobotocore_ecr.paginator import DescribeImageScanFindingsPaginator

def get_describe_image_scan_findings_paginator() -> DescribeImageScanFindingsPaginator:
    return client.get_paginator("describe_image_scan_findings"))
```

- [DescribeImageScanFindingsPaginator](./paginators.md#describeimagescanfindingspaginator)
- [DescribeImagesPaginator](./paginators.md#describeimagespaginator)
- [DescribePullThroughCacheRulesPaginator](./paginators.md#describepullthroughcacherulespaginator)
- [DescribeRepositoriesPaginator](./paginators.md#describerepositoriespaginator)
- [DescribeRepositoryCreationTemplatesPaginator](./paginators.md#describerepositorycreationtemplatespaginator)
- [GetLifecyclePolicyPreviewPaginator](./paginators.md#getlifecyclepolicypreviewpaginator)
- [ListImagesPaginator](./paginators.md#listimagespaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("ecr").get_waiter("...")`.

```python
# ImageScanCompleteWaiter usage example

from types_aiobotocore_ecr.waiter import ImageScanCompleteWaiter

def get_image_scan_complete_waiter() -> ImageScanCompleteWaiter:
    return Session().client("ecr").get_waiter("image_scan_complete")
```

- [ImageScanCompleteWaiter](./waiters.md#imagescancompletewaiter)
- [LifecyclePolicyPreviewCompleteWaiter](./waiters.md#lifecyclepolicypreviewcompletewaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# DescribeImageScanFindingsPaginatorName usage example

from types_aiobotocore_ecr.literals import DescribeImageScanFindingsPaginatorName

def get_value() -> DescribeImageScanFindingsPaginatorName:
    return "describe_image_scan_findings"
```

- [DescribeImageScanFindingsPaginatorName](./literals.md#describeimagescanfindingspaginatorname)
- [DescribeImagesPaginatorName](./literals.md#describeimagespaginatorname)
- [DescribePullThroughCacheRulesPaginatorName](./literals.md#describepullthroughcacherulespaginatorname)
- [DescribeRepositoriesPaginatorName](./literals.md#describerepositoriespaginatorname)
- [DescribeRepositoryCreationTemplatesPaginatorName](./literals.md#describerepositorycreationtemplatespaginatorname)
- [EncryptionTypeType](./literals.md#encryptiontypetype)
- [FindingSeverityType](./literals.md#findingseveritytype)
- [GetLifecyclePolicyPreviewPaginatorName](./literals.md#getlifecyclepolicypreviewpaginatorname)
- [ImageActionTypeType](./literals.md#imageactiontypetype)
- [ImageFailureCodeType](./literals.md#imagefailurecodetype)
- [ImageScanCompleteWaiterName](./literals.md#imagescancompletewaitername)
- [ImageTagMutabilityType](./literals.md#imagetagmutabilitytype)
- [LayerAvailabilityType](./literals.md#layeravailabilitytype)
- [LayerFailureCodeType](./literals.md#layerfailurecodetype)
- [LifecyclePolicyPreviewCompleteWaiterName](./literals.md#lifecyclepolicypreviewcompletewaitername)
- [LifecyclePolicyPreviewStatusType](./literals.md#lifecyclepolicypreviewstatustype)
- [ListImagesPaginatorName](./literals.md#listimagespaginatorname)
- [RCTAppliedForType](./literals.md#rctappliedfortype)
- [ReplicationStatusType](./literals.md#replicationstatustype)
- [RepositoryFilterTypeType](./literals.md#repositoryfiltertypetype)
- [ScanFrequencyType](./literals.md#scanfrequencytype)
- [ScanStatusType](./literals.md#scanstatustype)
- [ScanTypeType](./literals.md#scantypetype)
- [ScanningConfigurationFailureCodeType](./literals.md#scanningconfigurationfailurecodetype)
- [ScanningRepositoryFilterTypeType](./literals.md#scanningrepositoryfiltertypetype)
- [TagStatusType](./literals.md#tagstatustype)
- [UpstreamRegistryType](./literals.md#upstreamregistrytype)
- [ECRServiceName](./literals.md#ecrservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AttributeTypeDef](./type_defs.md#attributetypedef)
- [AuthorizationDataTypeDef](./type_defs.md#authorizationdatatypedef)
- [AwsEcrContainerImageDetailsTypeDef](./type_defs.md#awsecrcontainerimagedetailstypedef)
- [BatchCheckLayerAvailabilityRequestRequestTypeDef](./type_defs.md#batchchecklayeravailabilityrequestrequesttypedef)
- [LayerFailureTypeDef](./type_defs.md#layerfailuretypedef)
- [LayerTypeDef](./type_defs.md#layertypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ImageIdentifierTypeDef](./type_defs.md#imageidentifiertypedef)
- [BatchGetRepositoryScanningConfigurationRequestRequestTypeDef](./type_defs.md#batchgetrepositoryscanningconfigurationrequestrequesttypedef)
- [RepositoryScanningConfigurationFailureTypeDef](./type_defs.md#repositoryscanningconfigurationfailuretypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [CompleteLayerUploadRequestRequestTypeDef](./type_defs.md#completelayeruploadrequestrequesttypedef)
- [CreatePullThroughCacheRuleRequestRequestTypeDef](./type_defs.md#createpullthroughcacherulerequestrequesttypedef)
- [EncryptionConfigurationForRepositoryCreationTemplateTypeDef](./type_defs.md#encryptionconfigurationforrepositorycreationtemplatetypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef)
- [ImageScanningConfigurationTypeDef](./type_defs.md#imagescanningconfigurationtypedef)
- [CvssScoreAdjustmentTypeDef](./type_defs.md#cvssscoreadjustmenttypedef)
- [CvssScoreTypeDef](./type_defs.md#cvssscoretypedef)
- [DeleteLifecyclePolicyRequestRequestTypeDef](./type_defs.md#deletelifecyclepolicyrequestrequesttypedef)
- [DeletePullThroughCacheRuleRequestRequestTypeDef](./type_defs.md#deletepullthroughcacherulerequestrequesttypedef)
- [DeleteRepositoryCreationTemplateRequestRequestTypeDef](./type_defs.md#deleterepositorycreationtemplaterequestrequesttypedef)
- [DeleteRepositoryPolicyRequestRequestTypeDef](./type_defs.md#deleterepositorypolicyrequestrequesttypedef)
- [DeleteRepositoryRequestRequestTypeDef](./type_defs.md#deleterepositoryrequestrequesttypedef)
- [ImageReplicationStatusTypeDef](./type_defs.md#imagereplicationstatustypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [ImageScanStatusTypeDef](./type_defs.md#imagescanstatustypedef)
- [DescribeImagesFilterTypeDef](./type_defs.md#describeimagesfiltertypedef)
- [DescribePullThroughCacheRulesRequestRequestTypeDef](./type_defs.md#describepullthroughcacherulesrequestrequesttypedef)
- [PullThroughCacheRuleTypeDef](./type_defs.md#pullthroughcacheruletypedef)
- [DescribeRepositoriesRequestRequestTypeDef](./type_defs.md#describerepositoriesrequestrequesttypedef)
- [DescribeRepositoryCreationTemplatesRequestRequestTypeDef](./type_defs.md#describerepositorycreationtemplatesrequestrequesttypedef)
- [GetAccountSettingRequestRequestTypeDef](./type_defs.md#getaccountsettingrequestrequesttypedef)
- [GetAuthorizationTokenRequestRequestTypeDef](./type_defs.md#getauthorizationtokenrequestrequesttypedef)
- [GetDownloadUrlForLayerRequestRequestTypeDef](./type_defs.md#getdownloadurlforlayerrequestrequesttypedef)
- [LifecyclePolicyPreviewFilterTypeDef](./type_defs.md#lifecyclepolicypreviewfiltertypedef)
- [LifecyclePolicyPreviewSummaryTypeDef](./type_defs.md#lifecyclepolicypreviewsummarytypedef)
- [GetLifecyclePolicyRequestRequestTypeDef](./type_defs.md#getlifecyclepolicyrequestrequesttypedef)
- [GetRepositoryPolicyRequestRequestTypeDef](./type_defs.md#getrepositorypolicyrequestrequesttypedef)
- [ImageScanFindingsSummaryTypeDef](./type_defs.md#imagescanfindingssummarytypedef)
- [InitiateLayerUploadRequestRequestTypeDef](./type_defs.md#initiatelayeruploadrequestrequesttypedef)
- [LifecyclePolicyRuleActionTypeDef](./type_defs.md#lifecyclepolicyruleactiontypedef)
- [ListImagesFilterTypeDef](./type_defs.md#listimagesfiltertypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [VulnerablePackageTypeDef](./type_defs.md#vulnerablepackagetypedef)
- [PutAccountSettingRequestRequestTypeDef](./type_defs.md#putaccountsettingrequestrequesttypedef)
- [PutImageRequestRequestTypeDef](./type_defs.md#putimagerequestrequesttypedef)
- [PutImageTagMutabilityRequestRequestTypeDef](./type_defs.md#putimagetagmutabilityrequestrequesttypedef)
- [PutLifecyclePolicyRequestRequestTypeDef](./type_defs.md#putlifecyclepolicyrequestrequesttypedef)
- [PutRegistryPolicyRequestRequestTypeDef](./type_defs.md#putregistrypolicyrequestrequesttypedef)
- [RecommendationTypeDef](./type_defs.md#recommendationtypedef)
- [ScanningRepositoryFilterTypeDef](./type_defs.md#scanningrepositoryfiltertypedef)
- [ReplicationDestinationTypeDef](./type_defs.md#replicationdestinationtypedef)
- [RepositoryFilterTypeDef](./type_defs.md#repositoryfiltertypedef)
- [SetRepositoryPolicyRequestRequestTypeDef](./type_defs.md#setrepositorypolicyrequestrequesttypedef)
- [StartLifecyclePolicyPreviewRequestRequestTypeDef](./type_defs.md#startlifecyclepolicypreviewrequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdatePullThroughCacheRuleRequestRequestTypeDef](./type_defs.md#updatepullthroughcacherulerequestrequesttypedef)
- [ValidatePullThroughCacheRuleRequestRequestTypeDef](./type_defs.md#validatepullthroughcacherulerequestrequesttypedef)
- [ImageScanFindingTypeDef](./type_defs.md#imagescanfindingtypedef)
- [ResourceDetailsTypeDef](./type_defs.md#resourcedetailstypedef)
- [BatchCheckLayerAvailabilityResponseTypeDef](./type_defs.md#batchchecklayeravailabilityresponsetypedef)
- [CompleteLayerUploadResponseTypeDef](./type_defs.md#completelayeruploadresponsetypedef)
- [CreatePullThroughCacheRuleResponseTypeDef](./type_defs.md#createpullthroughcacheruleresponsetypedef)
- [DeleteLifecyclePolicyResponseTypeDef](./type_defs.md#deletelifecyclepolicyresponsetypedef)
- [DeletePullThroughCacheRuleResponseTypeDef](./type_defs.md#deletepullthroughcacheruleresponsetypedef)
- [DeleteRegistryPolicyResponseTypeDef](./type_defs.md#deleteregistrypolicyresponsetypedef)
- [DeleteRepositoryPolicyResponseTypeDef](./type_defs.md#deleterepositorypolicyresponsetypedef)
- [GetAccountSettingResponseTypeDef](./type_defs.md#getaccountsettingresponsetypedef)
- [GetAuthorizationTokenResponseTypeDef](./type_defs.md#getauthorizationtokenresponsetypedef)
- [GetDownloadUrlForLayerResponseTypeDef](./type_defs.md#getdownloadurlforlayerresponsetypedef)
- [GetLifecyclePolicyResponseTypeDef](./type_defs.md#getlifecyclepolicyresponsetypedef)
- [GetRegistryPolicyResponseTypeDef](./type_defs.md#getregistrypolicyresponsetypedef)
- [GetRepositoryPolicyResponseTypeDef](./type_defs.md#getrepositorypolicyresponsetypedef)
- [InitiateLayerUploadResponseTypeDef](./type_defs.md#initiatelayeruploadresponsetypedef)
- [PutAccountSettingResponseTypeDef](./type_defs.md#putaccountsettingresponsetypedef)
- [PutImageTagMutabilityResponseTypeDef](./type_defs.md#putimagetagmutabilityresponsetypedef)
- [PutLifecyclePolicyResponseTypeDef](./type_defs.md#putlifecyclepolicyresponsetypedef)
- [PutRegistryPolicyResponseTypeDef](./type_defs.md#putregistrypolicyresponsetypedef)
- [SetRepositoryPolicyResponseTypeDef](./type_defs.md#setrepositorypolicyresponsetypedef)
- [StartLifecyclePolicyPreviewResponseTypeDef](./type_defs.md#startlifecyclepolicypreviewresponsetypedef)
- [UpdatePullThroughCacheRuleResponseTypeDef](./type_defs.md#updatepullthroughcacheruleresponsetypedef)
- [UploadLayerPartResponseTypeDef](./type_defs.md#uploadlayerpartresponsetypedef)
- [ValidatePullThroughCacheRuleResponseTypeDef](./type_defs.md#validatepullthroughcacheruleresponsetypedef)
- [BatchDeleteImageRequestRequestTypeDef](./type_defs.md#batchdeleteimagerequestrequesttypedef)
- [BatchGetImageRequestRequestTypeDef](./type_defs.md#batchgetimagerequestrequesttypedef)
- [DescribeImageReplicationStatusRequestRequestTypeDef](./type_defs.md#describeimagereplicationstatusrequestrequesttypedef)
- [DescribeImageScanFindingsRequestRequestTypeDef](./type_defs.md#describeimagescanfindingsrequestrequesttypedef)
- [ImageFailureTypeDef](./type_defs.md#imagefailuretypedef)
- [ImageTypeDef](./type_defs.md#imagetypedef)
- [ListImagesResponseTypeDef](./type_defs.md#listimagesresponsetypedef)
- [StartImageScanRequestRequestTypeDef](./type_defs.md#startimagescanrequestrequesttypedef)
- [UploadLayerPartRequestRequestTypeDef](./type_defs.md#uploadlayerpartrequestrequesttypedef)
- [CreateRepositoryCreationTemplateRequestRequestTypeDef](./type_defs.md#createrepositorycreationtemplaterequestrequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [RepositoryCreationTemplateTypeDef](./type_defs.md#repositorycreationtemplatetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UpdateRepositoryCreationTemplateRequestRequestTypeDef](./type_defs.md#updaterepositorycreationtemplaterequestrequesttypedef)
- [CreateRepositoryRequestRequestTypeDef](./type_defs.md#createrepositoryrequestrequesttypedef)
- [PutImageScanningConfigurationRequestRequestTypeDef](./type_defs.md#putimagescanningconfigurationrequestrequesttypedef)
- [PutImageScanningConfigurationResponseTypeDef](./type_defs.md#putimagescanningconfigurationresponsetypedef)
- [RepositoryTypeDef](./type_defs.md#repositorytypedef)
- [CvssScoreDetailsTypeDef](./type_defs.md#cvssscoredetailstypedef)
- [DescribeImageReplicationStatusResponseTypeDef](./type_defs.md#describeimagereplicationstatusresponsetypedef)
- [DescribeImageScanFindingsRequestDescribeImageScanFindingsPaginateTypeDef](./type_defs.md#describeimagescanfindingsrequestdescribeimagescanfindingspaginatetypedef)
- [DescribePullThroughCacheRulesRequestDescribePullThroughCacheRulesPaginateTypeDef](./type_defs.md#describepullthroughcacherulesrequestdescribepullthroughcacherulespaginatetypedef)
- [DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef](./type_defs.md#describerepositoriesrequestdescriberepositoriespaginatetypedef)
- [DescribeRepositoryCreationTemplatesRequestDescribeRepositoryCreationTemplatesPaginateTypeDef](./type_defs.md#describerepositorycreationtemplatesrequestdescriberepositorycreationtemplatespaginatetypedef)
- [DescribeImageScanFindingsRequestImageScanCompleteWaitTypeDef](./type_defs.md#describeimagescanfindingsrequestimagescancompletewaittypedef)
- [StartImageScanResponseTypeDef](./type_defs.md#startimagescanresponsetypedef)
- [DescribeImagesRequestDescribeImagesPaginateTypeDef](./type_defs.md#describeimagesrequestdescribeimagespaginatetypedef)
- [DescribeImagesRequestRequestTypeDef](./type_defs.md#describeimagesrequestrequesttypedef)
- [DescribePullThroughCacheRulesResponseTypeDef](./type_defs.md#describepullthroughcacherulesresponsetypedef)
- [GetLifecyclePolicyPreviewRequestGetLifecyclePolicyPreviewPaginateTypeDef](./type_defs.md#getlifecyclepolicypreviewrequestgetlifecyclepolicypreviewpaginatetypedef)
- [GetLifecyclePolicyPreviewRequestLifecyclePolicyPreviewCompleteWaitTypeDef](./type_defs.md#getlifecyclepolicypreviewrequestlifecyclepolicypreviewcompletewaittypedef)
- [GetLifecyclePolicyPreviewRequestRequestTypeDef](./type_defs.md#getlifecyclepolicypreviewrequestrequesttypedef)
- [ImageDetailTypeDef](./type_defs.md#imagedetailtypedef)
- [LifecyclePolicyPreviewResultTypeDef](./type_defs.md#lifecyclepolicypreviewresulttypedef)
- [ListImagesRequestListImagesPaginateTypeDef](./type_defs.md#listimagesrequestlistimagespaginatetypedef)
- [ListImagesRequestRequestTypeDef](./type_defs.md#listimagesrequestrequesttypedef)
- [PackageVulnerabilityDetailsTypeDef](./type_defs.md#packagevulnerabilitydetailstypedef)
- [RemediationTypeDef](./type_defs.md#remediationtypedef)
- [RegistryScanningRuleOutputTypeDef](./type_defs.md#registryscanningruleoutputtypedef)
- [RegistryScanningRuleTypeDef](./type_defs.md#registryscanningruletypedef)
- [RepositoryScanningConfigurationTypeDef](./type_defs.md#repositoryscanningconfigurationtypedef)
- [ReplicationRuleOutputTypeDef](./type_defs.md#replicationruleoutputtypedef)
- [ReplicationRuleTypeDef](./type_defs.md#replicationruletypedef)
- [ResourceTypeDef](./type_defs.md#resourcetypedef)
- [BatchDeleteImageResponseTypeDef](./type_defs.md#batchdeleteimageresponsetypedef)
- [BatchGetImageResponseTypeDef](./type_defs.md#batchgetimageresponsetypedef)
- [PutImageResponseTypeDef](./type_defs.md#putimageresponsetypedef)
- [CreateRepositoryCreationTemplateResponseTypeDef](./type_defs.md#createrepositorycreationtemplateresponsetypedef)
- [DeleteRepositoryCreationTemplateResponseTypeDef](./type_defs.md#deleterepositorycreationtemplateresponsetypedef)
- [DescribeRepositoryCreationTemplatesResponseTypeDef](./type_defs.md#describerepositorycreationtemplatesresponsetypedef)
- [UpdateRepositoryCreationTemplateResponseTypeDef](./type_defs.md#updaterepositorycreationtemplateresponsetypedef)
- [CreateRepositoryResponseTypeDef](./type_defs.md#createrepositoryresponsetypedef)
- [DeleteRepositoryResponseTypeDef](./type_defs.md#deleterepositoryresponsetypedef)
- [DescribeRepositoriesResponseTypeDef](./type_defs.md#describerepositoriesresponsetypedef)
- [ScoreDetailsTypeDef](./type_defs.md#scoredetailstypedef)
- [DescribeImagesResponseTypeDef](./type_defs.md#describeimagesresponsetypedef)
- [GetLifecyclePolicyPreviewResponseTypeDef](./type_defs.md#getlifecyclepolicypreviewresponsetypedef)
- [RegistryScanningConfigurationTypeDef](./type_defs.md#registryscanningconfigurationtypedef)
- [RegistryScanningRuleUnionTypeDef](./type_defs.md#registryscanningruleuniontypedef)
- [BatchGetRepositoryScanningConfigurationResponseTypeDef](./type_defs.md#batchgetrepositoryscanningconfigurationresponsetypedef)
- [ReplicationConfigurationOutputTypeDef](./type_defs.md#replicationconfigurationoutputtypedef)
- [ReplicationRuleUnionTypeDef](./type_defs.md#replicationruleuniontypedef)
- [EnhancedImageScanFindingTypeDef](./type_defs.md#enhancedimagescanfindingtypedef)
- [GetRegistryScanningConfigurationResponseTypeDef](./type_defs.md#getregistryscanningconfigurationresponsetypedef)
- [PutRegistryScanningConfigurationResponseTypeDef](./type_defs.md#putregistryscanningconfigurationresponsetypedef)
- [PutRegistryScanningConfigurationRequestRequestTypeDef](./type_defs.md#putregistryscanningconfigurationrequestrequesttypedef)
- [DescribeRegistryResponseTypeDef](./type_defs.md#describeregistryresponsetypedef)
- [PutReplicationConfigurationResponseTypeDef](./type_defs.md#putreplicationconfigurationresponsetypedef)
- [ReplicationConfigurationTypeDef](./type_defs.md#replicationconfigurationtypedef)
- [ImageScanFindingsTypeDef](./type_defs.md#imagescanfindingstypedef)
- [PutReplicationConfigurationRequestRequestTypeDef](./type_defs.md#putreplicationconfigurationrequestrequesttypedef)
- [DescribeImageScanFindingsResponseTypeDef](./type_defs.md#describeimagescanfindingsresponsetypedef)

