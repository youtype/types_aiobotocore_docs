# Inspector2 module

> [Index](../README.md) > Inspector2


!!! note ""

    Auto-generated documentation for [Inspector2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#inspector2)
    type annotations stubs module [types-aiobotocore-inspector2](https://pypi.org/project/types-aiobotocore-inspector2/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `Inspector2` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `Inspector2` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[inspector2]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[inspector2]'

# standalone installation
python -m pip install types-aiobotocore-inspector2
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-inspector2
```

## Usage

Code samples can be found in [Examples](./usage.md).

## Inspector2Client

Type annotations and code completion for  `#!python session.create_client("inspector2")` as [Inspector2Client](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client)

```python
# Inspector2Client usage example

from aiobotocore.session import get_session

from types_aiobotocore_inspector2.client import Inspector2Client


session = get_session()
async with session.create_client("inspector2") as client:
    client: Inspector2Client
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("inspector2").get_paginator("...")`.

```python
# GetCisScanResultDetailsPaginator usage example

from types_aiobotocore_inspector2.paginator import GetCisScanResultDetailsPaginator

def get_get_cis_scan_result_details_paginator() -> GetCisScanResultDetailsPaginator:
    return client.get_paginator("get_cis_scan_result_details"))
```

- [GetCisScanResultDetailsPaginator](./paginators.md#getcisscanresultdetailspaginator)
- [ListAccountPermissionsPaginator](./paginators.md#listaccountpermissionspaginator)
- [ListCisScanConfigurationsPaginator](./paginators.md#listcisscanconfigurationspaginator)
- [ListCisScanResultsAggregatedByChecksPaginator](./paginators.md#listcisscanresultsaggregatedbycheckspaginator)
- [ListCisScanResultsAggregatedByTargetResourcePaginator](./paginators.md#listcisscanresultsaggregatedbytargetresourcepaginator)
- [ListCisScansPaginator](./paginators.md#listcisscanspaginator)
- [ListCoveragePaginator](./paginators.md#listcoveragepaginator)
- [ListCoverageStatisticsPaginator](./paginators.md#listcoveragestatisticspaginator)
- [ListDelegatedAdminAccountsPaginator](./paginators.md#listdelegatedadminaccountspaginator)
- [ListFiltersPaginator](./paginators.md#listfilterspaginator)
- [ListFindingAggregationsPaginator](./paginators.md#listfindingaggregationspaginator)
- [ListFindingsPaginator](./paginators.md#listfindingspaginator)
- [ListMembersPaginator](./paginators.md#listmemberspaginator)
- [ListUsageTotalsPaginator](./paginators.md#listusagetotalspaginator)
- [SearchVulnerabilitiesPaginator](./paginators.md#searchvulnerabilitiespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AccountSortByType usage example

from types_aiobotocore_inspector2.literals import AccountSortByType

def get_value() -> AccountSortByType:
    return "ALL"
```

- [AccountSortByType](./literals.md#accountsortbytype)
- [AggregationFindingTypeType](./literals.md#aggregationfindingtypetype)
- [AggregationResourceTypeType](./literals.md#aggregationresourcetypetype)
- [AggregationTypeType](./literals.md#aggregationtypetype)
- [AmiSortByType](./literals.md#amisortbytype)
- [ArchitectureType](./literals.md#architecturetype)
- [AwsEcrContainerSortByType](./literals.md#awsecrcontainersortbytype)
- [CisFindingStatusComparisonType](./literals.md#cisfindingstatuscomparisontype)
- [CisFindingStatusType](./literals.md#cisfindingstatustype)
- [CisReportFormatType](./literals.md#cisreportformattype)
- [CisReportStatusType](./literals.md#cisreportstatustype)
- [CisResultStatusComparisonType](./literals.md#cisresultstatuscomparisontype)
- [CisResultStatusType](./literals.md#cisresultstatustype)
- [CisRuleStatusType](./literals.md#cisrulestatustype)
- [CisScanConfigurationsSortByType](./literals.md#cisscanconfigurationssortbytype)
- [CisScanResultDetailsSortByType](./literals.md#cisscanresultdetailssortbytype)
- [CisScanResultsAggregatedByChecksSortByType](./literals.md#cisscanresultsaggregatedbycheckssortbytype)
- [CisScanResultsAggregatedByTargetResourceSortByType](./literals.md#cisscanresultsaggregatedbytargetresourcesortbytype)
- [CisScanStatusComparisonType](./literals.md#cisscanstatuscomparisontype)
- [CisScanStatusType](./literals.md#cisscanstatustype)
- [CisSecurityLevelComparisonType](./literals.md#cissecuritylevelcomparisontype)
- [CisSecurityLevelType](./literals.md#cissecurityleveltype)
- [CisSortOrderType](./literals.md#cissortordertype)
- [CisStringComparisonType](./literals.md#cisstringcomparisontype)
- [CisTargetStatusComparisonType](./literals.md#cistargetstatuscomparisontype)
- [CisTargetStatusReasonType](./literals.md#cistargetstatusreasontype)
- [CisTargetStatusType](./literals.md#cistargetstatustype)
- [CodeSnippetErrorCodeType](./literals.md#codesnippeterrorcodetype)
- [CoverageMapComparisonType](./literals.md#coveragemapcomparisontype)
- [CoverageResourceTypeType](./literals.md#coverageresourcetypetype)
- [CoverageStringComparisonType](./literals.md#coveragestringcomparisontype)
- [CurrencyType](./literals.md#currencytype)
- [DayType](./literals.md#daytype)
- [DelegatedAdminStatusType](./literals.md#delegatedadminstatustype)
- [Ec2DeepInspectionStatusType](./literals.md#ec2deepinspectionstatustype)
- [Ec2InstanceSortByType](./literals.md#ec2instancesortbytype)
- [Ec2PlatformType](./literals.md#ec2platformtype)
- [Ec2ScanModeStatusType](./literals.md#ec2scanmodestatustype)
- [Ec2ScanModeType](./literals.md#ec2scanmodetype)
- [EcrPullDateRescanDurationType](./literals.md#ecrpulldaterescandurationtype)
- [EcrRescanDurationStatusType](./literals.md#ecrrescandurationstatustype)
- [EcrRescanDurationType](./literals.md#ecrrescandurationtype)
- [EcrScanFrequencyType](./literals.md#ecrscanfrequencytype)
- [ErrorCodeType](./literals.md#errorcodetype)
- [ExploitAvailableType](./literals.md#exploitavailabletype)
- [ExternalReportStatusType](./literals.md#externalreportstatustype)
- [FilterActionType](./literals.md#filteractiontype)
- [FindingDetailsErrorCodeType](./literals.md#findingdetailserrorcodetype)
- [FindingStatusType](./literals.md#findingstatustype)
- [FindingTypeSortByType](./literals.md#findingtypesortbytype)
- [FindingTypeType](./literals.md#findingtypetype)
- [FixAvailableType](./literals.md#fixavailabletype)
- [FreeTrialInfoErrorCodeType](./literals.md#freetrialinfoerrorcodetype)
- [FreeTrialStatusType](./literals.md#freetrialstatustype)
- [FreeTrialTypeType](./literals.md#freetrialtypetype)
- [GetCisScanResultDetailsPaginatorName](./literals.md#getcisscanresultdetailspaginatorname)
- [GroupKeyType](./literals.md#groupkeytype)
- [ImageLayerSortByType](./literals.md#imagelayersortbytype)
- [LambdaFunctionSortByType](./literals.md#lambdafunctionsortbytype)
- [LambdaLayerSortByType](./literals.md#lambdalayersortbytype)
- [ListAccountPermissionsPaginatorName](./literals.md#listaccountpermissionspaginatorname)
- [ListCisScanConfigurationsPaginatorName](./literals.md#listcisscanconfigurationspaginatorname)
- [ListCisScanResultsAggregatedByChecksPaginatorName](./literals.md#listcisscanresultsaggregatedbycheckspaginatorname)
- [ListCisScanResultsAggregatedByTargetResourcePaginatorName](./literals.md#listcisscanresultsaggregatedbytargetresourcepaginatorname)
- [ListCisScansDetailLevelType](./literals.md#listcisscansdetailleveltype)
- [ListCisScansPaginatorName](./literals.md#listcisscanspaginatorname)
- [ListCisScansSortByType](./literals.md#listcisscanssortbytype)
- [ListCoveragePaginatorName](./literals.md#listcoveragepaginatorname)
- [ListCoverageStatisticsPaginatorName](./literals.md#listcoveragestatisticspaginatorname)
- [ListDelegatedAdminAccountsPaginatorName](./literals.md#listdelegatedadminaccountspaginatorname)
- [ListFiltersPaginatorName](./literals.md#listfilterspaginatorname)
- [ListFindingAggregationsPaginatorName](./literals.md#listfindingaggregationspaginatorname)
- [ListFindingsPaginatorName](./literals.md#listfindingspaginatorname)
- [ListMembersPaginatorName](./literals.md#listmemberspaginatorname)
- [ListUsageTotalsPaginatorName](./literals.md#listusagetotalspaginatorname)
- [MapComparisonType](./literals.md#mapcomparisontype)
- [NetworkProtocolType](./literals.md#networkprotocoltype)
- [OperationType](./literals.md#operationtype)
- [PackageManagerType](./literals.md#packagemanagertype)
- [PackageSortByType](./literals.md#packagesortbytype)
- [PackageTypeType](./literals.md#packagetypetype)
- [RelationshipStatusType](./literals.md#relationshipstatustype)
- [ReportFormatType](./literals.md#reportformattype)
- [ReportingErrorCodeType](./literals.md#reportingerrorcodetype)
- [RepositorySortByType](./literals.md#repositorysortbytype)
- [ResourceMapComparisonType](./literals.md#resourcemapcomparisontype)
- [ResourceScanTypeType](./literals.md#resourcescantypetype)
- [ResourceStringComparisonType](./literals.md#resourcestringcomparisontype)
- [ResourceTypeType](./literals.md#resourcetypetype)
- [RuntimeType](./literals.md#runtimetype)
- [SbomReportFormatType](./literals.md#sbomreportformattype)
- [ScanModeType](./literals.md#scanmodetype)
- [ScanStatusCodeType](./literals.md#scanstatuscodetype)
- [ScanStatusReasonType](./literals.md#scanstatusreasontype)
- [ScanTypeType](./literals.md#scantypetype)
- [SearchVulnerabilitiesPaginatorName](./literals.md#searchvulnerabilitiespaginatorname)
- [ServiceType](./literals.md#servicetype)
- [SeverityType](./literals.md#severitytype)
- [SortFieldType](./literals.md#sortfieldtype)
- [SortOrderType](./literals.md#sortordertype)
- [StatusType](./literals.md#statustype)
- [StopCisSessionStatusType](./literals.md#stopcissessionstatustype)
- [StringComparisonType](./literals.md#stringcomparisontype)
- [TagComparisonType](./literals.md#tagcomparisontype)
- [TitleSortByType](./literals.md#titlesortbytype)
- [UsageTypeType](./literals.md#usagetypetype)
- [VulnerabilitySourceType](./literals.md#vulnerabilitysourcetype)
- [Inspector2ServiceName](./literals.md#inspector2servicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [SeverityCountsTypeDef](./type_defs.md#severitycountstypedef)
- [AccountAggregationTypeDef](./type_defs.md#accountaggregationtypedef)
- [StateTypeDef](./type_defs.md#statetypedef)
- [ResourceStatusTypeDef](./type_defs.md#resourcestatustypedef)
- [FindingTypeAggregationTypeDef](./type_defs.md#findingtypeaggregationtypedef)
- [StringFilterTypeDef](./type_defs.md#stringfiltertypedef)
- [AssociateMemberRequestRequestTypeDef](./type_defs.md#associatememberrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [AtigDataTypeDef](./type_defs.md#atigdatatypedef)
- [AutoEnableTypeDef](./type_defs.md#autoenabletypedef)
- [AwsEc2InstanceDetailsTypeDef](./type_defs.md#awsec2instancedetailstypedef)
- [AwsEcrContainerImageDetailsTypeDef](./type_defs.md#awsecrcontainerimagedetailstypedef)
- [LambdaVpcConfigTypeDef](./type_defs.md#lambdavpcconfigtypedef)
- [BatchGetAccountStatusRequestRequestTypeDef](./type_defs.md#batchgetaccountstatusrequestrequesttypedef)
- [BatchGetCodeSnippetRequestRequestTypeDef](./type_defs.md#batchgetcodesnippetrequestrequesttypedef)
- [CodeSnippetErrorTypeDef](./type_defs.md#codesnippeterrortypedef)
- [BatchGetFindingDetailsRequestRequestTypeDef](./type_defs.md#batchgetfindingdetailsrequestrequesttypedef)
- [FindingDetailsErrorTypeDef](./type_defs.md#findingdetailserrortypedef)
- [BatchGetFreeTrialInfoRequestRequestTypeDef](./type_defs.md#batchgetfreetrialinforequestrequesttypedef)
- [FreeTrialInfoErrorTypeDef](./type_defs.md#freetrialinfoerrortypedef)
- [BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef](./type_defs.md#batchgetmemberec2deepinspectionstatusrequestrequesttypedef)
- [FailedMemberAccountEc2DeepInspectionStatusStateTypeDef](./type_defs.md#failedmemberaccountec2deepinspectionstatusstatetypedef)
- [MemberAccountEc2DeepInspectionStatusStateTypeDef](./type_defs.md#memberaccountec2deepinspectionstatusstatetypedef)
- [MemberAccountEc2DeepInspectionStatusTypeDef](./type_defs.md#memberaccountec2deepinspectionstatustypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [CancelFindingsReportRequestRequestTypeDef](./type_defs.md#cancelfindingsreportrequestrequesttypedef)
- [CancelSbomExportRequestRequestTypeDef](./type_defs.md#cancelsbomexportrequestrequesttypedef)
- [StatusCountsTypeDef](./type_defs.md#statuscountstypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [CisFindingStatusFilterTypeDef](./type_defs.md#cisfindingstatusfiltertypedef)
- [CisNumberFilterTypeDef](./type_defs.md#cisnumberfiltertypedef)
- [CisResultStatusFilterTypeDef](./type_defs.md#cisresultstatusfiltertypedef)
- [CisTargetsTypeDef](./type_defs.md#cistargetstypedef)
- [CisSecurityLevelFilterTypeDef](./type_defs.md#cissecuritylevelfiltertypedef)
- [CisStringFilterTypeDef](./type_defs.md#cisstringfiltertypedef)
- [CisScanResultDetailsTypeDef](./type_defs.md#cisscanresultdetailstypedef)
- [CisTargetStatusFilterTypeDef](./type_defs.md#cistargetstatusfiltertypedef)
- [CisTargetStatusReasonFilterTypeDef](./type_defs.md#cistargetstatusreasonfiltertypedef)
- [TagFilterTypeDef](./type_defs.md#tagfiltertypedef)
- [CisScanStatusFilterTypeDef](./type_defs.md#cisscanstatusfiltertypedef)
- [CisaDataTypeDef](./type_defs.md#cisadatatypedef)
- [CodeFilePathTypeDef](./type_defs.md#codefilepathtypedef)
- [CodeLineTypeDef](./type_defs.md#codelinetypedef)
- [SuggestedFixTypeDef](./type_defs.md#suggestedfixtypedef)
- [ComputePlatformTypeDef](./type_defs.md#computeplatformtypedef)
- [CountsTypeDef](./type_defs.md#countstypedef)
- [CoverageMapFilterTypeDef](./type_defs.md#coveragemapfiltertypedef)
- [CoverageStringFilterTypeDef](./type_defs.md#coveragestringfiltertypedef)
- [ScanStatusTypeDef](./type_defs.md#scanstatustypedef)
- [CreateCisTargetsTypeDef](./type_defs.md#createcistargetstypedef)
- [DestinationTypeDef](./type_defs.md#destinationtypedef)
- [Cvss2TypeDef](./type_defs.md#cvss2typedef)
- [Cvss3TypeDef](./type_defs.md#cvss3typedef)
- [CvssScoreAdjustmentTypeDef](./type_defs.md#cvssscoreadjustmenttypedef)
- [CvssScoreTypeDef](./type_defs.md#cvssscoretypedef)
- [TimeTypeDef](./type_defs.md#timetypedef)
- [DateFilterOutputTypeDef](./type_defs.md#datefilteroutputtypedef)
- [DelegatedAdminAccountTypeDef](./type_defs.md#delegatedadminaccounttypedef)
- [DelegatedAdminTypeDef](./type_defs.md#delegatedadmintypedef)
- [DeleteCisScanConfigurationRequestRequestTypeDef](./type_defs.md#deletecisscanconfigurationrequestrequesttypedef)
- [DeleteFilterRequestRequestTypeDef](./type_defs.md#deletefilterrequestrequesttypedef)
- [DisableDelegatedAdminAccountRequestRequestTypeDef](./type_defs.md#disabledelegatedadminaccountrequestrequesttypedef)
- [DisableRequestRequestTypeDef](./type_defs.md#disablerequestrequesttypedef)
- [DisassociateMemberRequestRequestTypeDef](./type_defs.md#disassociatememberrequestrequesttypedef)
- [Ec2ScanModeStateTypeDef](./type_defs.md#ec2scanmodestatetypedef)
- [Ec2ConfigurationTypeDef](./type_defs.md#ec2configurationtypedef)
- [MapFilterTypeDef](./type_defs.md#mapfiltertypedef)
- [Ec2MetadataTypeDef](./type_defs.md#ec2metadatatypedef)
- [EcrRescanDurationStateTypeDef](./type_defs.md#ecrrescandurationstatetypedef)
- [EcrConfigurationTypeDef](./type_defs.md#ecrconfigurationtypedef)
- [EcrContainerImageMetadataTypeDef](./type_defs.md#ecrcontainerimagemetadatatypedef)
- [EcrRepositoryMetadataTypeDef](./type_defs.md#ecrrepositorymetadatatypedef)
- [EnableDelegatedAdminAccountRequestRequestTypeDef](./type_defs.md#enabledelegatedadminaccountrequestrequesttypedef)
- [EnableRequestRequestTypeDef](./type_defs.md#enablerequestrequesttypedef)
- [EpssDetailsTypeDef](./type_defs.md#epssdetailstypedef)
- [EpssTypeDef](./type_defs.md#epsstypedef)
- [EvidenceTypeDef](./type_defs.md#evidencetypedef)
- [ExploitObservedTypeDef](./type_defs.md#exploitobservedtypedef)
- [ExploitabilityDetailsTypeDef](./type_defs.md#exploitabilitydetailstypedef)
- [NumberFilterTypeDef](./type_defs.md#numberfiltertypedef)
- [PortRangeFilterTypeDef](./type_defs.md#portrangefiltertypedef)
- [FreeTrialInfoTypeDef](./type_defs.md#freetrialinfotypedef)
- [GetCisScanReportRequestRequestTypeDef](./type_defs.md#getcisscanreportrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [GetEncryptionKeyRequestRequestTypeDef](./type_defs.md#getencryptionkeyrequestrequesttypedef)
- [GetFindingsReportStatusRequestRequestTypeDef](./type_defs.md#getfindingsreportstatusrequestrequesttypedef)
- [GetMemberRequestRequestTypeDef](./type_defs.md#getmemberrequestrequesttypedef)
- [MemberTypeDef](./type_defs.md#membertypedef)
- [GetSbomExportRequestRequestTypeDef](./type_defs.md#getsbomexportrequestrequesttypedef)
- [LambdaFunctionMetadataTypeDef](./type_defs.md#lambdafunctionmetadatatypedef)
- [ListAccountPermissionsRequestRequestTypeDef](./type_defs.md#listaccountpermissionsrequestrequesttypedef)
- [PermissionTypeDef](./type_defs.md#permissiontypedef)
- [ListDelegatedAdminAccountsRequestRequestTypeDef](./type_defs.md#listdelegatedadminaccountsrequestrequesttypedef)
- [ListFiltersRequestRequestTypeDef](./type_defs.md#listfiltersrequestrequesttypedef)
- [SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef)
- [ListMembersRequestRequestTypeDef](./type_defs.md#listmembersrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListUsageTotalsRequestRequestTypeDef](./type_defs.md#listusagetotalsrequestrequesttypedef)
- [StepTypeDef](./type_defs.md#steptypedef)
- [PortRangeTypeDef](./type_defs.md#portrangetypedef)
- [VulnerablePackageTypeDef](./type_defs.md#vulnerablepackagetypedef)
- [RecommendationTypeDef](./type_defs.md#recommendationtypedef)
- [ResetEncryptionKeyRequestRequestTypeDef](./type_defs.md#resetencryptionkeyrequestrequesttypedef)
- [ResourceMapFilterTypeDef](./type_defs.md#resourcemapfiltertypedef)
- [ResourceStringFilterTypeDef](./type_defs.md#resourcestringfiltertypedef)
- [SearchVulnerabilitiesFilterCriteriaTypeDef](./type_defs.md#searchvulnerabilitiesfiltercriteriatypedef)
- [SendCisSessionHealthRequestRequestTypeDef](./type_defs.md#sendcissessionhealthrequestrequesttypedef)
- [StartCisSessionMessageTypeDef](./type_defs.md#startcissessionmessagetypedef)
- [StopCisMessageProgressTypeDef](./type_defs.md#stopcismessageprogresstypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateCisTargetsTypeDef](./type_defs.md#updatecistargetstypedef)
- [UpdateEc2DeepInspectionConfigurationRequestRequestTypeDef](./type_defs.md#updateec2deepinspectionconfigurationrequestrequesttypedef)
- [UpdateEncryptionKeyRequestRequestTypeDef](./type_defs.md#updateencryptionkeyrequestrequesttypedef)
- [UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef](./type_defs.md#updateorgec2deepinspectionconfigurationrequestrequesttypedef)
- [UsageTypeDef](./type_defs.md#usagetypedef)
- [AccountAggregationResponseTypeDef](./type_defs.md#accountaggregationresponsetypedef)
- [AmiAggregationResponseTypeDef](./type_defs.md#amiaggregationresponsetypedef)
- [AwsEcrContainerAggregationResponseTypeDef](./type_defs.md#awsecrcontaineraggregationresponsetypedef)
- [Ec2InstanceAggregationResponseTypeDef](./type_defs.md#ec2instanceaggregationresponsetypedef)
- [FindingTypeAggregationResponseTypeDef](./type_defs.md#findingtypeaggregationresponsetypedef)
- [ImageLayerAggregationResponseTypeDef](./type_defs.md#imagelayeraggregationresponsetypedef)
- [LambdaFunctionAggregationResponseTypeDef](./type_defs.md#lambdafunctionaggregationresponsetypedef)
- [LambdaLayerAggregationResponseTypeDef](./type_defs.md#lambdalayeraggregationresponsetypedef)
- [PackageAggregationResponseTypeDef](./type_defs.md#packageaggregationresponsetypedef)
- [RepositoryAggregationResponseTypeDef](./type_defs.md#repositoryaggregationresponsetypedef)
- [TitleAggregationResponseTypeDef](./type_defs.md#titleaggregationresponsetypedef)
- [ResourceStateTypeDef](./type_defs.md#resourcestatetypedef)
- [AccountTypeDef](./type_defs.md#accounttypedef)
- [FailedAccountTypeDef](./type_defs.md#failedaccounttypedef)
- [AmiAggregationTypeDef](./type_defs.md#amiaggregationtypedef)
- [AwsEcrContainerAggregationTypeDef](./type_defs.md#awsecrcontaineraggregationtypedef)
- [ImageLayerAggregationTypeDef](./type_defs.md#imagelayeraggregationtypedef)
- [LambdaLayerAggregationTypeDef](./type_defs.md#lambdalayeraggregationtypedef)
- [PackageAggregationTypeDef](./type_defs.md#packageaggregationtypedef)
- [RepositoryAggregationTypeDef](./type_defs.md#repositoryaggregationtypedef)
- [TitleAggregationTypeDef](./type_defs.md#titleaggregationtypedef)
- [AssociateMemberResponseTypeDef](./type_defs.md#associatememberresponsetypedef)
- [CancelFindingsReportResponseTypeDef](./type_defs.md#cancelfindingsreportresponsetypedef)
- [CancelSbomExportResponseTypeDef](./type_defs.md#cancelsbomexportresponsetypedef)
- [CreateCisScanConfigurationResponseTypeDef](./type_defs.md#createcisscanconfigurationresponsetypedef)
- [CreateFilterResponseTypeDef](./type_defs.md#createfilterresponsetypedef)
- [CreateFindingsReportResponseTypeDef](./type_defs.md#createfindingsreportresponsetypedef)
- [CreateSbomExportResponseTypeDef](./type_defs.md#createsbomexportresponsetypedef)
- [DeleteCisScanConfigurationResponseTypeDef](./type_defs.md#deletecisscanconfigurationresponsetypedef)
- [DeleteFilterResponseTypeDef](./type_defs.md#deletefilterresponsetypedef)
- [DisableDelegatedAdminAccountResponseTypeDef](./type_defs.md#disabledelegatedadminaccountresponsetypedef)
- [DisassociateMemberResponseTypeDef](./type_defs.md#disassociatememberresponsetypedef)
- [EnableDelegatedAdminAccountResponseTypeDef](./type_defs.md#enabledelegatedadminaccountresponsetypedef)
- [GetCisScanReportResponseTypeDef](./type_defs.md#getcisscanreportresponsetypedef)
- [GetEc2DeepInspectionConfigurationResponseTypeDef](./type_defs.md#getec2deepinspectionconfigurationresponsetypedef)
- [GetEncryptionKeyResponseTypeDef](./type_defs.md#getencryptionkeyresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [UpdateCisScanConfigurationResponseTypeDef](./type_defs.md#updatecisscanconfigurationresponsetypedef)
- [UpdateEc2DeepInspectionConfigurationResponseTypeDef](./type_defs.md#updateec2deepinspectionconfigurationresponsetypedef)
- [UpdateFilterResponseTypeDef](./type_defs.md#updatefilterresponsetypedef)
- [DescribeOrganizationConfigurationResponseTypeDef](./type_defs.md#describeorganizationconfigurationresponsetypedef)
- [UpdateOrganizationConfigurationRequestRequestTypeDef](./type_defs.md#updateorganizationconfigurationrequestrequesttypedef)
- [UpdateOrganizationConfigurationResponseTypeDef](./type_defs.md#updateorganizationconfigurationresponsetypedef)
- [AwsLambdaFunctionDetailsTypeDef](./type_defs.md#awslambdafunctiondetailstypedef)
- [BatchGetMemberEc2DeepInspectionStatusResponseTypeDef](./type_defs.md#batchgetmemberec2deepinspectionstatusresponsetypedef)
- [BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef](./type_defs.md#batchupdatememberec2deepinspectionstatusresponsetypedef)
- [BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef](./type_defs.md#batchupdatememberec2deepinspectionstatusrequestrequesttypedef)
- [CisSessionMessageTypeDef](./type_defs.md#cissessionmessagetypedef)
- [CisCheckAggregationTypeDef](./type_defs.md#cischeckaggregationtypedef)
- [CisTargetResourceAggregationTypeDef](./type_defs.md#cistargetresourceaggregationtypedef)
- [CisDateFilterTypeDef](./type_defs.md#cisdatefiltertypedef)
- [CoverageDateFilterTypeDef](./type_defs.md#coveragedatefiltertypedef)
- [DateFilterTypeDef](./type_defs.md#datefiltertypedef)
- [CisScanTypeDef](./type_defs.md#cisscantypedef)
- [CisScanResultDetailsFilterCriteriaTypeDef](./type_defs.md#cisscanresultdetailsfiltercriteriatypedef)
- [CisScanResultsAggregatedByChecksFilterCriteriaTypeDef](./type_defs.md#cisscanresultsaggregatedbychecksfiltercriteriatypedef)
- [GetCisScanResultDetailsResponseTypeDef](./type_defs.md#getcisscanresultdetailsresponsetypedef)
- [CisScanResultsAggregatedByTargetResourceFilterCriteriaTypeDef](./type_defs.md#cisscanresultsaggregatedbytargetresourcefiltercriteriatypedef)
- [ListCisScanConfigurationsFilterCriteriaTypeDef](./type_defs.md#listcisscanconfigurationsfiltercriteriatypedef)
- [CodeVulnerabilityDetailsTypeDef](./type_defs.md#codevulnerabilitydetailstypedef)
- [CodeSnippetResultTypeDef](./type_defs.md#codesnippetresulttypedef)
- [ListCoverageStatisticsResponseTypeDef](./type_defs.md#listcoveragestatisticsresponsetypedef)
- [CvssScoreDetailsTypeDef](./type_defs.md#cvssscoredetailstypedef)
- [DailyScheduleTypeDef](./type_defs.md#dailyscheduletypedef)
- [MonthlyScheduleTypeDef](./type_defs.md#monthlyscheduletypedef)
- [WeeklyScheduleOutputTypeDef](./type_defs.md#weeklyscheduleoutputtypedef)
- [WeeklyScheduleTypeDef](./type_defs.md#weeklyscheduletypedef)
- [ListDelegatedAdminAccountsResponseTypeDef](./type_defs.md#listdelegatedadminaccountsresponsetypedef)
- [GetDelegatedAdminAccountResponseTypeDef](./type_defs.md#getdelegatedadminaccountresponsetypedef)
- [Ec2ConfigurationStateTypeDef](./type_defs.md#ec2configurationstatetypedef)
- [Ec2InstanceAggregationTypeDef](./type_defs.md#ec2instanceaggregationtypedef)
- [LambdaFunctionAggregationTypeDef](./type_defs.md#lambdafunctionaggregationtypedef)
- [EcrConfigurationStateTypeDef](./type_defs.md#ecrconfigurationstatetypedef)
- [UpdateConfigurationRequestRequestTypeDef](./type_defs.md#updateconfigurationrequestrequesttypedef)
- [FindingDetailTypeDef](./type_defs.md#findingdetailtypedef)
- [VulnerabilityTypeDef](./type_defs.md#vulnerabilitytypedef)
- [PackageFilterTypeDef](./type_defs.md#packagefiltertypedef)
- [FreeTrialAccountInfoTypeDef](./type_defs.md#freetrialaccountinfotypedef)
- [ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef](./type_defs.md#listaccountpermissionsrequestlistaccountpermissionspaginatetypedef)
- [ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef](./type_defs.md#listdelegatedadminaccountsrequestlistdelegatedadminaccountspaginatetypedef)
- [ListFiltersRequestListFiltersPaginateTypeDef](./type_defs.md#listfiltersrequestlistfilterspaginatetypedef)
- [ListMembersRequestListMembersPaginateTypeDef](./type_defs.md#listmembersrequestlistmemberspaginatetypedef)
- [ListUsageTotalsRequestListUsageTotalsPaginateTypeDef](./type_defs.md#listusagetotalsrequestlistusagetotalspaginatetypedef)
- [GetMemberResponseTypeDef](./type_defs.md#getmemberresponsetypedef)
- [ListMembersResponseTypeDef](./type_defs.md#listmembersresponsetypedef)
- [ResourceScanMetadataTypeDef](./type_defs.md#resourcescanmetadatatypedef)
- [ListAccountPermissionsResponseTypeDef](./type_defs.md#listaccountpermissionsresponsetypedef)
- [NetworkPathTypeDef](./type_defs.md#networkpathtypedef)
- [PackageVulnerabilityDetailsTypeDef](./type_defs.md#packagevulnerabilitydetailstypedef)
- [RemediationTypeDef](./type_defs.md#remediationtypedef)
- [ResourceFilterCriteriaOutputTypeDef](./type_defs.md#resourcefiltercriteriaoutputtypedef)
- [ResourceFilterCriteriaTypeDef](./type_defs.md#resourcefiltercriteriatypedef)
- [SearchVulnerabilitiesRequestRequestTypeDef](./type_defs.md#searchvulnerabilitiesrequestrequesttypedef)
- [SearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef](./type_defs.md#searchvulnerabilitiesrequestsearchvulnerabilitiespaginatetypedef)
- [StartCisSessionRequestRequestTypeDef](./type_defs.md#startcissessionrequestrequesttypedef)
- [StopCisSessionMessageTypeDef](./type_defs.md#stopcissessionmessagetypedef)
- [UsageTotalTypeDef](./type_defs.md#usagetotaltypedef)
- [AggregationResponseTypeDef](./type_defs.md#aggregationresponsetypedef)
- [AccountStateTypeDef](./type_defs.md#accountstatetypedef)
- [DisableResponseTypeDef](./type_defs.md#disableresponsetypedef)
- [EnableResponseTypeDef](./type_defs.md#enableresponsetypedef)
- [ResourceDetailsTypeDef](./type_defs.md#resourcedetailstypedef)
- [SendCisSessionTelemetryRequestRequestTypeDef](./type_defs.md#sendcissessiontelemetryrequestrequesttypedef)
- [ListCisScanResultsAggregatedByChecksResponseTypeDef](./type_defs.md#listcisscanresultsaggregatedbychecksresponsetypedef)
- [ListCisScanResultsAggregatedByTargetResourceResponseTypeDef](./type_defs.md#listcisscanresultsaggregatedbytargetresourceresponsetypedef)
- [ListCisScansFilterCriteriaTypeDef](./type_defs.md#listcisscansfiltercriteriatypedef)
- [CoverageFilterCriteriaTypeDef](./type_defs.md#coveragefiltercriteriatypedef)
- [DateFilterUnionTypeDef](./type_defs.md#datefilteruniontypedef)
- [ListCisScansResponseTypeDef](./type_defs.md#listcisscansresponsetypedef)
- [GetCisScanResultDetailsRequestGetCisScanResultDetailsPaginateTypeDef](./type_defs.md#getcisscanresultdetailsrequestgetcisscanresultdetailspaginatetypedef)
- [GetCisScanResultDetailsRequestRequestTypeDef](./type_defs.md#getcisscanresultdetailsrequestrequesttypedef)
- [ListCisScanResultsAggregatedByChecksRequestListCisScanResultsAggregatedByChecksPaginateTypeDef](./type_defs.md#listcisscanresultsaggregatedbychecksrequestlistcisscanresultsaggregatedbycheckspaginatetypedef)
- [ListCisScanResultsAggregatedByChecksRequestRequestTypeDef](./type_defs.md#listcisscanresultsaggregatedbychecksrequestrequesttypedef)
- [ListCisScanResultsAggregatedByTargetResourceRequestListCisScanResultsAggregatedByTargetResourcePaginateTypeDef](./type_defs.md#listcisscanresultsaggregatedbytargetresourcerequestlistcisscanresultsaggregatedbytargetresourcepaginatetypedef)
- [ListCisScanResultsAggregatedByTargetResourceRequestRequestTypeDef](./type_defs.md#listcisscanresultsaggregatedbytargetresourcerequestrequesttypedef)
- [ListCisScanConfigurationsRequestListCisScanConfigurationsPaginateTypeDef](./type_defs.md#listcisscanconfigurationsrequestlistcisscanconfigurationspaginatetypedef)
- [ListCisScanConfigurationsRequestRequestTypeDef](./type_defs.md#listcisscanconfigurationsrequestrequesttypedef)
- [BatchGetCodeSnippetResponseTypeDef](./type_defs.md#batchgetcodesnippetresponsetypedef)
- [InspectorScoreDetailsTypeDef](./type_defs.md#inspectorscoredetailstypedef)
- [ScheduleOutputTypeDef](./type_defs.md#scheduleoutputtypedef)
- [WeeklyScheduleUnionTypeDef](./type_defs.md#weeklyscheduleuniontypedef)
- [AggregationRequestTypeDef](./type_defs.md#aggregationrequesttypedef)
- [GetConfigurationResponseTypeDef](./type_defs.md#getconfigurationresponsetypedef)
- [BatchGetFindingDetailsResponseTypeDef](./type_defs.md#batchgetfindingdetailsresponsetypedef)
- [SearchVulnerabilitiesResponseTypeDef](./type_defs.md#searchvulnerabilitiesresponsetypedef)
- [FilterCriteriaOutputTypeDef](./type_defs.md#filtercriteriaoutputtypedef)
- [BatchGetFreeTrialInfoResponseTypeDef](./type_defs.md#batchgetfreetrialinforesponsetypedef)
- [CoveredResourceTypeDef](./type_defs.md#coveredresourcetypedef)
- [NetworkReachabilityDetailsTypeDef](./type_defs.md#networkreachabilitydetailstypedef)
- [GetSbomExportResponseTypeDef](./type_defs.md#getsbomexportresponsetypedef)
- [CreateSbomExportRequestRequestTypeDef](./type_defs.md#createsbomexportrequestrequesttypedef)
- [StopCisSessionRequestRequestTypeDef](./type_defs.md#stopcissessionrequestrequesttypedef)
- [ListUsageTotalsResponseTypeDef](./type_defs.md#listusagetotalsresponsetypedef)
- [ListFindingAggregationsResponseTypeDef](./type_defs.md#listfindingaggregationsresponsetypedef)
- [BatchGetAccountStatusResponseTypeDef](./type_defs.md#batchgetaccountstatusresponsetypedef)
- [ResourceTypeDef](./type_defs.md#resourcetypedef)
- [ListCisScansRequestListCisScansPaginateTypeDef](./type_defs.md#listcisscansrequestlistcisscanspaginatetypedef)
- [ListCisScansRequestRequestTypeDef](./type_defs.md#listcisscansrequestrequesttypedef)
- [ListCoverageRequestListCoveragePaginateTypeDef](./type_defs.md#listcoveragerequestlistcoveragepaginatetypedef)
- [ListCoverageRequestRequestTypeDef](./type_defs.md#listcoveragerequestrequesttypedef)
- [ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef](./type_defs.md#listcoveragestatisticsrequestlistcoveragestatisticspaginatetypedef)
- [ListCoverageStatisticsRequestRequestTypeDef](./type_defs.md#listcoveragestatisticsrequestrequesttypedef)
- [FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef)
- [CisScanConfigurationTypeDef](./type_defs.md#cisscanconfigurationtypedef)
- [ScheduleTypeDef](./type_defs.md#scheduletypedef)
- [ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef](./type_defs.md#listfindingaggregationsrequestlistfindingaggregationspaginatetypedef)
- [ListFindingAggregationsRequestRequestTypeDef](./type_defs.md#listfindingaggregationsrequestrequesttypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [GetFindingsReportStatusResponseTypeDef](./type_defs.md#getfindingsreportstatusresponsetypedef)
- [ListCoverageResponseTypeDef](./type_defs.md#listcoverageresponsetypedef)
- [FindingTypeDef](./type_defs.md#findingtypedef)
- [CreateFilterRequestRequestTypeDef](./type_defs.md#createfilterrequestrequesttypedef)
- [CreateFindingsReportRequestRequestTypeDef](./type_defs.md#createfindingsreportrequestrequesttypedef)
- [ListFindingsRequestListFindingsPaginateTypeDef](./type_defs.md#listfindingsrequestlistfindingspaginatetypedef)
- [ListFindingsRequestRequestTypeDef](./type_defs.md#listfindingsrequestrequesttypedef)
- [UpdateFilterRequestRequestTypeDef](./type_defs.md#updatefilterrequestrequesttypedef)
- [ListCisScanConfigurationsResponseTypeDef](./type_defs.md#listcisscanconfigurationsresponsetypedef)
- [CreateCisScanConfigurationRequestRequestTypeDef](./type_defs.md#createcisscanconfigurationrequestrequesttypedef)
- [UpdateCisScanConfigurationRequestRequestTypeDef](./type_defs.md#updatecisscanconfigurationrequestrequesttypedef)
- [ListFiltersResponseTypeDef](./type_defs.md#listfiltersresponsetypedef)
- [ListFindingsResponseTypeDef](./type_defs.md#listfindingsresponsetypedef)

