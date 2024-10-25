# AccessAnalyzer module

> [Index](../README.md) > AccessAnalyzer


!!! note ""

    Auto-generated documentation for [AccessAnalyzer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
    type annotations stubs module [types-aiobotocore-accessanalyzer](https://pypi.org/project/types-aiobotocore-accessanalyzer/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `AccessAnalyzer` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[accessanalyzer]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[accessanalyzer]'


# standalone installation
python -m pip install types-aiobotocore-accessanalyzer
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-accessanalyzer
```

## Usage

Code samples can be found in [Examples](./usage.md).

## AccessAnalyzerClient

Type annotations and code completion for  `#!python session.create_client("accessanalyzer")` as [AccessAnalyzerClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Client)

```python
# AccessAnalyzerClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_accessanalyzer.client import AccessAnalyzerClient


session = get_session()
async with session.create_client("accessanalyzer") as client:
    client: AccessAnalyzerClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("accessanalyzer").get_paginator("...")`.

```python
# GetFindingRecommendationPaginator usage example

from types_aiobotocore_accessanalyzer.paginator import GetFindingRecommendationPaginator

def get_get_finding_recommendation_paginator() -> GetFindingRecommendationPaginator:
    return client.get_paginator("get_finding_recommendation"))
```

- [GetFindingRecommendationPaginator](./paginators.md#getfindingrecommendationpaginator)
- [GetFindingV2Paginator](./paginators.md#getfindingv2paginator)
- [ListAccessPreviewFindingsPaginator](./paginators.md#listaccesspreviewfindingspaginator)
- [ListAccessPreviewsPaginator](./paginators.md#listaccesspreviewspaginator)
- [ListAnalyzedResourcesPaginator](./paginators.md#listanalyzedresourcespaginator)
- [ListAnalyzersPaginator](./paginators.md#listanalyzerspaginator)
- [ListArchiveRulesPaginator](./paginators.md#listarchiverulespaginator)
- [ListFindingsPaginator](./paginators.md#listfindingspaginator)
- [ListFindingsV2Paginator](./paginators.md#listfindingsv2paginator)
- [ListPolicyGenerationsPaginator](./paginators.md#listpolicygenerationspaginator)
- [ValidatePolicyPaginator](./paginators.md#validatepolicypaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AccessCheckPolicyTypeType usage example

from types_aiobotocore_accessanalyzer.literals import AccessCheckPolicyTypeType

def get_value() -> AccessCheckPolicyTypeType:
    return "IDENTITY_POLICY"
```

- [AccessCheckPolicyTypeType](./literals.md#accesscheckpolicytypetype)
- [AccessCheckResourceTypeType](./literals.md#accesscheckresourcetypetype)
- [AccessPreviewStatusReasonCodeType](./literals.md#accesspreviewstatusreasoncodetype)
- [AccessPreviewStatusType](./literals.md#accesspreviewstatustype)
- [AclPermissionType](./literals.md#aclpermissiontype)
- [AnalyzerStatusType](./literals.md#analyzerstatustype)
- [CheckAccessNotGrantedResultType](./literals.md#checkaccessnotgrantedresulttype)
- [CheckNoNewAccessResultType](./literals.md#checknonewaccessresulttype)
- [CheckNoPublicAccessResultType](./literals.md#checknopublicaccessresulttype)
- [FindingChangeTypeType](./literals.md#findingchangetypetype)
- [FindingSourceTypeType](./literals.md#findingsourcetypetype)
- [FindingStatusType](./literals.md#findingstatustype)
- [FindingStatusUpdateType](./literals.md#findingstatusupdatetype)
- [FindingTypeType](./literals.md#findingtypetype)
- [GetFindingRecommendationPaginatorName](./literals.md#getfindingrecommendationpaginatorname)
- [GetFindingV2PaginatorName](./literals.md#getfindingv2paginatorname)
- [JobErrorCodeType](./literals.md#joberrorcodetype)
- [JobStatusType](./literals.md#jobstatustype)
- [KmsGrantOperationType](./literals.md#kmsgrantoperationtype)
- [ListAccessPreviewFindingsPaginatorName](./literals.md#listaccesspreviewfindingspaginatorname)
- [ListAccessPreviewsPaginatorName](./literals.md#listaccesspreviewspaginatorname)
- [ListAnalyzedResourcesPaginatorName](./literals.md#listanalyzedresourcespaginatorname)
- [ListAnalyzersPaginatorName](./literals.md#listanalyzerspaginatorname)
- [ListArchiveRulesPaginatorName](./literals.md#listarchiverulespaginatorname)
- [ListFindingsPaginatorName](./literals.md#listfindingspaginatorname)
- [ListFindingsV2PaginatorName](./literals.md#listfindingsv2paginatorname)
- [ListPolicyGenerationsPaginatorName](./literals.md#listpolicygenerationspaginatorname)
- [LocaleType](./literals.md#localetype)
- [OrderByType](./literals.md#orderbytype)
- [PolicyTypeType](./literals.md#policytypetype)
- [ReasonCodeType](./literals.md#reasoncodetype)
- [RecommendationTypeType](./literals.md#recommendationtypetype)
- [RecommendedRemediationActionType](./literals.md#recommendedremediationactiontype)
- [ResourceTypeType](./literals.md#resourcetypetype)
- [StatusType](./literals.md#statustype)
- [TypeType](./literals.md#typetype)
- [ValidatePolicyFindingTypeType](./literals.md#validatepolicyfindingtypetype)
- [ValidatePolicyPaginatorName](./literals.md#validatepolicypaginatorname)
- [ValidatePolicyResourceTypeType](./literals.md#validatepolicyresourcetypetype)
- [AccessAnalyzerServiceName](./literals.md#accessanalyzerservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccessPreviewStatusReasonTypeDef](./type_defs.md#accesspreviewstatusreasontypedef)
- [AccessTypeDef](./type_defs.md#accesstypedef)
- [AclGranteeTypeDef](./type_defs.md#aclgranteetypedef)
- [AnalyzedResourceSummaryTypeDef](./type_defs.md#analyzedresourcesummarytypedef)
- [AnalyzedResourceTypeDef](./type_defs.md#analyzedresourcetypedef)
- [UnusedAccessConfigurationTypeDef](./type_defs.md#unusedaccessconfigurationtypedef)
- [StatusReasonTypeDef](./type_defs.md#statusreasontypedef)
- [ApplyArchiveRuleRequestRequestTypeDef](./type_defs.md#applyarchiverulerequestrequesttypedef)
- [CriterionOutputTypeDef](./type_defs.md#criterionoutputtypedef)
- [CancelPolicyGenerationRequestRequestTypeDef](./type_defs.md#cancelpolicygenerationrequestrequesttypedef)
- [ReasonSummaryTypeDef](./type_defs.md#reasonsummarytypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CheckNoNewAccessRequestRequestTypeDef](./type_defs.md#checknonewaccessrequestrequesttypedef)
- [CheckNoPublicAccessRequestRequestTypeDef](./type_defs.md#checknopublicaccessrequestrequesttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [TrailTypeDef](./type_defs.md#trailtypedef)
- [TrailPropertiesTypeDef](./type_defs.md#trailpropertiestypedef)
- [DynamodbStreamConfigurationTypeDef](./type_defs.md#dynamodbstreamconfigurationtypedef)
- [DynamodbTableConfigurationTypeDef](./type_defs.md#dynamodbtableconfigurationtypedef)
- [EbsSnapshotConfigurationOutputTypeDef](./type_defs.md#ebssnapshotconfigurationoutputtypedef)
- [EcrRepositoryConfigurationTypeDef](./type_defs.md#ecrrepositoryconfigurationtypedef)
- [EfsFileSystemConfigurationTypeDef](./type_defs.md#efsfilesystemconfigurationtypedef)
- [IamRoleConfigurationTypeDef](./type_defs.md#iamroleconfigurationtypedef)
- [S3ExpressDirectoryBucketConfigurationTypeDef](./type_defs.md#s3expressdirectorybucketconfigurationtypedef)
- [SecretsManagerSecretConfigurationTypeDef](./type_defs.md#secretsmanagersecretconfigurationtypedef)
- [SnsTopicConfigurationTypeDef](./type_defs.md#snstopicconfigurationtypedef)
- [SqsQueueConfigurationTypeDef](./type_defs.md#sqsqueueconfigurationtypedef)
- [CriterionTypeDef](./type_defs.md#criteriontypedef)
- [DeleteAnalyzerRequestRequestTypeDef](./type_defs.md#deleteanalyzerrequestrequesttypedef)
- [DeleteArchiveRuleRequestRequestTypeDef](./type_defs.md#deletearchiverulerequestrequesttypedef)
- [EbsSnapshotConfigurationTypeDef](./type_defs.md#ebssnapshotconfigurationtypedef)
- [UnusedIamRoleDetailsTypeDef](./type_defs.md#unusediamroledetailstypedef)
- [UnusedIamUserAccessKeyDetailsTypeDef](./type_defs.md#unusediamuseraccesskeydetailstypedef)
- [UnusedIamUserPasswordDetailsTypeDef](./type_defs.md#unusediamuserpassworddetailstypedef)
- [FindingSourceDetailTypeDef](./type_defs.md#findingsourcedetailtypedef)
- [FindingSummaryV2TypeDef](./type_defs.md#findingsummaryv2typedef)
- [GenerateFindingRecommendationRequestRequestTypeDef](./type_defs.md#generatefindingrecommendationrequestrequesttypedef)
- [GeneratedPolicyTypeDef](./type_defs.md#generatedpolicytypedef)
- [GetAccessPreviewRequestRequestTypeDef](./type_defs.md#getaccesspreviewrequestrequesttypedef)
- [GetAnalyzedResourceRequestRequestTypeDef](./type_defs.md#getanalyzedresourcerequestrequesttypedef)
- [GetAnalyzerRequestRequestTypeDef](./type_defs.md#getanalyzerrequestrequesttypedef)
- [GetArchiveRuleRequestRequestTypeDef](./type_defs.md#getarchiverulerequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [GetFindingRecommendationRequestRequestTypeDef](./type_defs.md#getfindingrecommendationrequestrequesttypedef)
- [RecommendationErrorTypeDef](./type_defs.md#recommendationerrortypedef)
- [GetFindingRequestRequestTypeDef](./type_defs.md#getfindingrequestrequesttypedef)
- [GetFindingV2RequestRequestTypeDef](./type_defs.md#getfindingv2requestrequesttypedef)
- [GetGeneratedPolicyRequestRequestTypeDef](./type_defs.md#getgeneratedpolicyrequestrequesttypedef)
- [JobErrorTypeDef](./type_defs.md#joberrortypedef)
- [KmsGrantConstraintsOutputTypeDef](./type_defs.md#kmsgrantconstraintsoutputtypedef)
- [KmsGrantConstraintsTypeDef](./type_defs.md#kmsgrantconstraintstypedef)
- [ListAccessPreviewsRequestRequestTypeDef](./type_defs.md#listaccesspreviewsrequestrequesttypedef)
- [ListAnalyzedResourcesRequestRequestTypeDef](./type_defs.md#listanalyzedresourcesrequestrequesttypedef)
- [ListAnalyzersRequestRequestTypeDef](./type_defs.md#listanalyzersrequestrequesttypedef)
- [ListArchiveRulesRequestRequestTypeDef](./type_defs.md#listarchiverulesrequestrequesttypedef)
- [SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef)
- [ListPolicyGenerationsRequestRequestTypeDef](./type_defs.md#listpolicygenerationsrequestrequesttypedef)
- [PolicyGenerationTypeDef](./type_defs.md#policygenerationtypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef)
- [SubstringTypeDef](./type_defs.md#substringtypedef)
- [PolicyGenerationDetailsTypeDef](./type_defs.md#policygenerationdetailstypedef)
- [PositionTypeDef](./type_defs.md#positiontypedef)
- [RdsDbClusterSnapshotAttributeValueOutputTypeDef](./type_defs.md#rdsdbclustersnapshotattributevalueoutputtypedef)
- [RdsDbClusterSnapshotAttributeValueTypeDef](./type_defs.md#rdsdbclustersnapshotattributevaluetypedef)
- [RdsDbSnapshotAttributeValueOutputTypeDef](./type_defs.md#rdsdbsnapshotattributevalueoutputtypedef)
- [RdsDbSnapshotAttributeValueTypeDef](./type_defs.md#rdsdbsnapshotattributevaluetypedef)
- [UnusedPermissionsRecommendedStepTypeDef](./type_defs.md#unusedpermissionsrecommendedsteptypedef)
- [S3PublicAccessBlockConfigurationTypeDef](./type_defs.md#s3publicaccessblockconfigurationtypedef)
- [StartResourceScanRequestRequestTypeDef](./type_defs.md#startresourcescanrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UnusedActionTypeDef](./type_defs.md#unusedactiontypedef)
- [UpdateFindingsRequestRequestTypeDef](./type_defs.md#updatefindingsrequestrequesttypedef)
- [ValidatePolicyRequestRequestTypeDef](./type_defs.md#validatepolicyrequestrequesttypedef)
- [AccessPreviewSummaryTypeDef](./type_defs.md#accesspreviewsummarytypedef)
- [CheckAccessNotGrantedRequestRequestTypeDef](./type_defs.md#checkaccessnotgrantedrequestrequesttypedef)
- [S3BucketAclGrantConfigurationTypeDef](./type_defs.md#s3bucketaclgrantconfigurationtypedef)
- [AnalyzerConfigurationTypeDef](./type_defs.md#analyzerconfigurationtypedef)
- [ArchiveRuleSummaryTypeDef](./type_defs.md#archiverulesummarytypedef)
- [CheckAccessNotGrantedResponseTypeDef](./type_defs.md#checkaccessnotgrantedresponsetypedef)
- [CheckNoNewAccessResponseTypeDef](./type_defs.md#checknonewaccessresponsetypedef)
- [CheckNoPublicAccessResponseTypeDef](./type_defs.md#checknopublicaccessresponsetypedef)
- [CreateAccessPreviewResponseTypeDef](./type_defs.md#createaccesspreviewresponsetypedef)
- [CreateAnalyzerResponseTypeDef](./type_defs.md#createanalyzerresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetAnalyzedResourceResponseTypeDef](./type_defs.md#getanalyzedresourceresponsetypedef)
- [ListAnalyzedResourcesResponseTypeDef](./type_defs.md#listanalyzedresourcesresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [StartPolicyGenerationResponseTypeDef](./type_defs.md#startpolicygenerationresponsetypedef)
- [CloudTrailDetailsTypeDef](./type_defs.md#cloudtraildetailstypedef)
- [CloudTrailPropertiesTypeDef](./type_defs.md#cloudtrailpropertiestypedef)
- [CriterionUnionTypeDef](./type_defs.md#criterionuniontypedef)
- [ListAccessPreviewFindingsRequestRequestTypeDef](./type_defs.md#listaccesspreviewfindingsrequestrequesttypedef)
- [UpdateArchiveRuleRequestRequestTypeDef](./type_defs.md#updatearchiverulerequestrequesttypedef)
- [EbsSnapshotConfigurationUnionTypeDef](./type_defs.md#ebssnapshotconfigurationuniontypedef)
- [FindingSourceTypeDef](./type_defs.md#findingsourcetypedef)
- [ListFindingsV2ResponseTypeDef](./type_defs.md#listfindingsv2responsetypedef)
- [GetFindingRecommendationRequestGetFindingRecommendationPaginateTypeDef](./type_defs.md#getfindingrecommendationrequestgetfindingrecommendationpaginatetypedef)
- [GetFindingV2RequestGetFindingV2PaginateTypeDef](./type_defs.md#getfindingv2requestgetfindingv2paginatetypedef)
- [ListAccessPreviewFindingsRequestListAccessPreviewFindingsPaginateTypeDef](./type_defs.md#listaccesspreviewfindingsrequestlistaccesspreviewfindingspaginatetypedef)
- [ListAccessPreviewsRequestListAccessPreviewsPaginateTypeDef](./type_defs.md#listaccesspreviewsrequestlistaccesspreviewspaginatetypedef)
- [ListAnalyzedResourcesRequestListAnalyzedResourcesPaginateTypeDef](./type_defs.md#listanalyzedresourcesrequestlistanalyzedresourcespaginatetypedef)
- [ListAnalyzersRequestListAnalyzersPaginateTypeDef](./type_defs.md#listanalyzersrequestlistanalyzerspaginatetypedef)
- [ListArchiveRulesRequestListArchiveRulesPaginateTypeDef](./type_defs.md#listarchiverulesrequestlistarchiverulespaginatetypedef)
- [ListPolicyGenerationsRequestListPolicyGenerationsPaginateTypeDef](./type_defs.md#listpolicygenerationsrequestlistpolicygenerationspaginatetypedef)
- [ValidatePolicyRequestValidatePolicyPaginateTypeDef](./type_defs.md#validatepolicyrequestvalidatepolicypaginatetypedef)
- [JobDetailsTypeDef](./type_defs.md#jobdetailstypedef)
- [KmsGrantConfigurationOutputTypeDef](./type_defs.md#kmsgrantconfigurationoutputtypedef)
- [KmsGrantConstraintsUnionTypeDef](./type_defs.md#kmsgrantconstraintsuniontypedef)
- [ListFindingsRequestListFindingsPaginateTypeDef](./type_defs.md#listfindingsrequestlistfindingspaginatetypedef)
- [ListFindingsRequestRequestTypeDef](./type_defs.md#listfindingsrequestrequesttypedef)
- [ListFindingsV2RequestListFindingsV2PaginateTypeDef](./type_defs.md#listfindingsv2requestlistfindingsv2paginatetypedef)
- [ListFindingsV2RequestRequestTypeDef](./type_defs.md#listfindingsv2requestrequesttypedef)
- [ListPolicyGenerationsResponseTypeDef](./type_defs.md#listpolicygenerationsresponsetypedef)
- [NetworkOriginConfigurationOutputTypeDef](./type_defs.md#networkoriginconfigurationoutputtypedef)
- [NetworkOriginConfigurationTypeDef](./type_defs.md#networkoriginconfigurationtypedef)
- [PathElementTypeDef](./type_defs.md#pathelementtypedef)
- [SpanTypeDef](./type_defs.md#spantypedef)
- [RdsDbClusterSnapshotConfigurationOutputTypeDef](./type_defs.md#rdsdbclustersnapshotconfigurationoutputtypedef)
- [RdsDbClusterSnapshotAttributeValueUnionTypeDef](./type_defs.md#rdsdbclustersnapshotattributevalueuniontypedef)
- [RdsDbSnapshotConfigurationOutputTypeDef](./type_defs.md#rdsdbsnapshotconfigurationoutputtypedef)
- [RdsDbSnapshotAttributeValueUnionTypeDef](./type_defs.md#rdsdbsnapshotattributevalueuniontypedef)
- [RecommendedStepTypeDef](./type_defs.md#recommendedsteptypedef)
- [UnusedPermissionDetailsTypeDef](./type_defs.md#unusedpermissiondetailstypedef)
- [ListAccessPreviewsResponseTypeDef](./type_defs.md#listaccesspreviewsresponsetypedef)
- [AnalyzerSummaryTypeDef](./type_defs.md#analyzersummarytypedef)
- [GetArchiveRuleResponseTypeDef](./type_defs.md#getarchiveruleresponsetypedef)
- [ListArchiveRulesResponseTypeDef](./type_defs.md#listarchiverulesresponsetypedef)
- [StartPolicyGenerationRequestRequestTypeDef](./type_defs.md#startpolicygenerationrequestrequesttypedef)
- [GeneratedPolicyPropertiesTypeDef](./type_defs.md#generatedpolicypropertiestypedef)
- [CreateArchiveRuleRequestRequestTypeDef](./type_defs.md#createarchiverulerequestrequesttypedef)
- [InlineArchiveRuleTypeDef](./type_defs.md#inlinearchiveruletypedef)
- [AccessPreviewFindingTypeDef](./type_defs.md#accesspreviewfindingtypedef)
- [ExternalAccessDetailsTypeDef](./type_defs.md#externalaccessdetailstypedef)
- [FindingSummaryTypeDef](./type_defs.md#findingsummarytypedef)
- [FindingTypeDef](./type_defs.md#findingtypedef)
- [KmsKeyConfigurationOutputTypeDef](./type_defs.md#kmskeyconfigurationoutputtypedef)
- [KmsGrantConfigurationTypeDef](./type_defs.md#kmsgrantconfigurationtypedef)
- [S3AccessPointConfigurationOutputTypeDef](./type_defs.md#s3accesspointconfigurationoutputtypedef)
- [NetworkOriginConfigurationUnionTypeDef](./type_defs.md#networkoriginconfigurationuniontypedef)
- [LocationTypeDef](./type_defs.md#locationtypedef)
- [RdsDbClusterSnapshotConfigurationTypeDef](./type_defs.md#rdsdbclustersnapshotconfigurationtypedef)
- [RdsDbSnapshotConfigurationTypeDef](./type_defs.md#rdsdbsnapshotconfigurationtypedef)
- [GetFindingRecommendationResponseTypeDef](./type_defs.md#getfindingrecommendationresponsetypedef)
- [GetAnalyzerResponseTypeDef](./type_defs.md#getanalyzerresponsetypedef)
- [ListAnalyzersResponseTypeDef](./type_defs.md#listanalyzersresponsetypedef)
- [GeneratedPolicyResultTypeDef](./type_defs.md#generatedpolicyresulttypedef)
- [CreateAnalyzerRequestRequestTypeDef](./type_defs.md#createanalyzerrequestrequesttypedef)
- [ListAccessPreviewFindingsResponseTypeDef](./type_defs.md#listaccesspreviewfindingsresponsetypedef)
- [FindingDetailsTypeDef](./type_defs.md#findingdetailstypedef)
- [ListFindingsResponseTypeDef](./type_defs.md#listfindingsresponsetypedef)
- [GetFindingResponseTypeDef](./type_defs.md#getfindingresponsetypedef)
- [KmsGrantConfigurationUnionTypeDef](./type_defs.md#kmsgrantconfigurationuniontypedef)
- [S3BucketConfigurationOutputTypeDef](./type_defs.md#s3bucketconfigurationoutputtypedef)
- [S3AccessPointConfigurationTypeDef](./type_defs.md#s3accesspointconfigurationtypedef)
- [ValidatePolicyFindingTypeDef](./type_defs.md#validatepolicyfindingtypedef)
- [RdsDbClusterSnapshotConfigurationUnionTypeDef](./type_defs.md#rdsdbclustersnapshotconfigurationuniontypedef)
- [RdsDbSnapshotConfigurationUnionTypeDef](./type_defs.md#rdsdbsnapshotconfigurationuniontypedef)
- [GetGeneratedPolicyResponseTypeDef](./type_defs.md#getgeneratedpolicyresponsetypedef)
- [GetFindingV2ResponseTypeDef](./type_defs.md#getfindingv2responsetypedef)
- [KmsKeyConfigurationTypeDef](./type_defs.md#kmskeyconfigurationtypedef)
- [ConfigurationOutputTypeDef](./type_defs.md#configurationoutputtypedef)
- [S3AccessPointConfigurationUnionTypeDef](./type_defs.md#s3accesspointconfigurationuniontypedef)
- [ValidatePolicyResponseTypeDef](./type_defs.md#validatepolicyresponsetypedef)
- [KmsKeyConfigurationUnionTypeDef](./type_defs.md#kmskeyconfigurationuniontypedef)
- [AccessPreviewTypeDef](./type_defs.md#accesspreviewtypedef)
- [S3BucketConfigurationTypeDef](./type_defs.md#s3bucketconfigurationtypedef)
- [GetAccessPreviewResponseTypeDef](./type_defs.md#getaccesspreviewresponsetypedef)
- [S3BucketConfigurationUnionTypeDef](./type_defs.md#s3bucketconfigurationuniontypedef)
- [ConfigurationTypeDef](./type_defs.md#configurationtypedef)
- [ConfigurationUnionTypeDef](./type_defs.md#configurationuniontypedef)
- [CreateAccessPreviewRequestRequestTypeDef](./type_defs.md#createaccesspreviewrequestrequesttypedef)

