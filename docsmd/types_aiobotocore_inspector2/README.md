# Inspector2 module

> [Index](../README.md) > Inspector2


!!! note ""

    Auto-generated documentation for [Inspector2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
    type annotations stubs module [types-aiobotocore-inspector2](https://pypi.org/project/types-aiobotocore-inspector2/).

## How to install



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
# ListAccountPermissionsPaginator usage example

from types_aiobotocore_inspector2.paginator import ListAccountPermissionsPaginator

def get_list_account_permissions_paginator() -> ListAccountPermissionsPaginator:
    return client.get_paginator("list_account_permissions"))
```

- [ListAccountPermissionsPaginator](./paginators.md#listaccountpermissionspaginator)
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
- [CodeSnippetErrorCodeType](./literals.md#codesnippeterrorcodetype)
- [CoverageMapComparisonType](./literals.md#coveragemapcomparisontype)
- [CoverageResourceTypeType](./literals.md#coverageresourcetypetype)
- [CoverageStringComparisonType](./literals.md#coveragestringcomparisontype)
- [CurrencyType](./literals.md#currencytype)
- [DelegatedAdminStatusType](./literals.md#delegatedadminstatustype)
- [Ec2DeepInspectionStatusType](./literals.md#ec2deepinspectionstatustype)
- [Ec2InstanceSortByType](./literals.md#ec2instancesortbytype)
- [Ec2PlatformType](./literals.md#ec2platformtype)
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
- [GroupKeyType](./literals.md#groupkeytype)
- [ImageLayerSortByType](./literals.md#imagelayersortbytype)
- [LambdaFunctionSortByType](./literals.md#lambdafunctionsortbytype)
- [LambdaLayerSortByType](./literals.md#lambdalayersortbytype)
- [ListAccountPermissionsPaginatorName](./literals.md#listaccountpermissionspaginatorname)
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
- [ScanStatusCodeType](./literals.md#scanstatuscodetype)
- [ScanStatusReasonType](./literals.md#scanstatusreasontype)
- [ScanTypeType](./literals.md#scantypetype)
- [SearchVulnerabilitiesPaginatorName](./literals.md#searchvulnerabilitiespaginatorname)
- [ServiceType](./literals.md#servicetype)
- [SeverityType](./literals.md#severitytype)
- [SortFieldType](./literals.md#sortfieldtype)
- [SortOrderType](./literals.md#sortordertype)
- [StatusType](./literals.md#statustype)
- [StringComparisonType](./literals.md#stringcomparisontype)
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
- [CancelFindingsReportRequestRequestTypeDef](./type_defs.md#cancelfindingsreportrequestrequesttypedef)
- [CancelSbomExportRequestRequestTypeDef](./type_defs.md#cancelsbomexportrequestrequesttypedef)
- [CisaDataTypeDef](./type_defs.md#cisadatatypedef)
- [CodeFilePathTypeDef](./type_defs.md#codefilepathtypedef)
- [CodeLineTypeDef](./type_defs.md#codelinetypedef)
- [SuggestedFixTypeDef](./type_defs.md#suggestedfixtypedef)
- [CountsTypeDef](./type_defs.md#countstypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [CoverageMapFilterTypeDef](./type_defs.md#coveragemapfiltertypedef)
- [CoverageStringFilterTypeDef](./type_defs.md#coveragestringfiltertypedef)
- [ScanStatusTypeDef](./type_defs.md#scanstatustypedef)
- [DestinationTypeDef](./type_defs.md#destinationtypedef)
- [Cvss2TypeDef](./type_defs.md#cvss2typedef)
- [Cvss3TypeDef](./type_defs.md#cvss3typedef)
- [CvssScoreAdjustmentTypeDef](./type_defs.md#cvssscoreadjustmenttypedef)
- [CvssScoreTypeDef](./type_defs.md#cvssscoretypedef)
- [DelegatedAdminAccountTypeDef](./type_defs.md#delegatedadminaccounttypedef)
- [DelegatedAdminTypeDef](./type_defs.md#delegatedadmintypedef)
- [DeleteFilterRequestRequestTypeDef](./type_defs.md#deletefilterrequestrequesttypedef)
- [DisableDelegatedAdminAccountRequestRequestTypeDef](./type_defs.md#disabledelegatedadminaccountrequestrequesttypedef)
- [DisableRequestRequestTypeDef](./type_defs.md#disablerequestrequesttypedef)
- [DisassociateMemberRequestRequestTypeDef](./type_defs.md#disassociatememberrequestrequesttypedef)
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
- [GetEncryptionKeyRequestRequestTypeDef](./type_defs.md#getencryptionkeyrequestrequesttypedef)
- [GetFindingsReportStatusRequestRequestTypeDef](./type_defs.md#getfindingsreportstatusrequestrequesttypedef)
- [GetMemberRequestRequestTypeDef](./type_defs.md#getmemberrequestrequesttypedef)
- [MemberTypeDef](./type_defs.md#membertypedef)
- [GetSbomExportRequestRequestTypeDef](./type_defs.md#getsbomexportrequestrequesttypedef)
- [LambdaFunctionMetadataTypeDef](./type_defs.md#lambdafunctionmetadatatypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
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
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
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
- [CreateFilterResponseTypeDef](./type_defs.md#createfilterresponsetypedef)
- [CreateFindingsReportResponseTypeDef](./type_defs.md#createfindingsreportresponsetypedef)
- [CreateSbomExportResponseTypeDef](./type_defs.md#createsbomexportresponsetypedef)
- [DeleteFilterResponseTypeDef](./type_defs.md#deletefilterresponsetypedef)
- [DisableDelegatedAdminAccountResponseTypeDef](./type_defs.md#disabledelegatedadminaccountresponsetypedef)
- [DisassociateMemberResponseTypeDef](./type_defs.md#disassociatememberresponsetypedef)
- [EnableDelegatedAdminAccountResponseTypeDef](./type_defs.md#enabledelegatedadminaccountresponsetypedef)
- [GetEc2DeepInspectionConfigurationResponseTypeDef](./type_defs.md#getec2deepinspectionconfigurationresponsetypedef)
- [GetEncryptionKeyResponseTypeDef](./type_defs.md#getencryptionkeyresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [UpdateEc2DeepInspectionConfigurationResponseTypeDef](./type_defs.md#updateec2deepinspectionconfigurationresponsetypedef)
- [UpdateFilterResponseTypeDef](./type_defs.md#updatefilterresponsetypedef)
- [DescribeOrganizationConfigurationResponseTypeDef](./type_defs.md#describeorganizationconfigurationresponsetypedef)
- [UpdateOrganizationConfigurationRequestRequestTypeDef](./type_defs.md#updateorganizationconfigurationrequestrequesttypedef)
- [UpdateOrganizationConfigurationResponseTypeDef](./type_defs.md#updateorganizationconfigurationresponsetypedef)
- [AwsLambdaFunctionDetailsTypeDef](./type_defs.md#awslambdafunctiondetailstypedef)
- [BatchGetMemberEc2DeepInspectionStatusResponseTypeDef](./type_defs.md#batchgetmemberec2deepinspectionstatusresponsetypedef)
- [BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef](./type_defs.md#batchupdatememberec2deepinspectionstatusresponsetypedef)
- [BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef](./type_defs.md#batchupdatememberec2deepinspectionstatusrequestrequesttypedef)
- [CodeVulnerabilityDetailsTypeDef](./type_defs.md#codevulnerabilitydetailstypedef)
- [CodeSnippetResultTypeDef](./type_defs.md#codesnippetresulttypedef)
- [ListCoverageStatisticsResponseTypeDef](./type_defs.md#listcoveragestatisticsresponsetypedef)
- [CoverageDateFilterTypeDef](./type_defs.md#coveragedatefiltertypedef)
- [DateFilterTypeDef](./type_defs.md#datefiltertypedef)
- [CvssScoreDetailsTypeDef](./type_defs.md#cvssscoredetailstypedef)
- [ListDelegatedAdminAccountsResponseTypeDef](./type_defs.md#listdelegatedadminaccountsresponsetypedef)
- [GetDelegatedAdminAccountResponseTypeDef](./type_defs.md#getdelegatedadminaccountresponsetypedef)
- [Ec2InstanceAggregationTypeDef](./type_defs.md#ec2instanceaggregationtypedef)
- [LambdaFunctionAggregationTypeDef](./type_defs.md#lambdafunctionaggregationtypedef)
- [EcrConfigurationStateTypeDef](./type_defs.md#ecrconfigurationstatetypedef)
- [UpdateConfigurationRequestRequestTypeDef](./type_defs.md#updateconfigurationrequestrequesttypedef)
- [FindingDetailTypeDef](./type_defs.md#findingdetailtypedef)
- [VulnerabilityTypeDef](./type_defs.md#vulnerabilitytypedef)
- [PackageFilterTypeDef](./type_defs.md#packagefiltertypedef)
- [FreeTrialAccountInfoTypeDef](./type_defs.md#freetrialaccountinfotypedef)
- [GetMemberResponseTypeDef](./type_defs.md#getmemberresponsetypedef)
- [ListMembersResponseTypeDef](./type_defs.md#listmembersresponsetypedef)
- [ResourceScanMetadataTypeDef](./type_defs.md#resourcescanmetadatatypedef)
- [ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef](./type_defs.md#listaccountpermissionsrequestlistaccountpermissionspaginatetypedef)
- [ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef](./type_defs.md#listdelegatedadminaccountsrequestlistdelegatedadminaccountspaginatetypedef)
- [ListFiltersRequestListFiltersPaginateTypeDef](./type_defs.md#listfiltersrequestlistfilterspaginatetypedef)
- [ListMembersRequestListMembersPaginateTypeDef](./type_defs.md#listmembersrequestlistmemberspaginatetypedef)
- [ListUsageTotalsRequestListUsageTotalsPaginateTypeDef](./type_defs.md#listusagetotalsrequestlistusagetotalspaginatetypedef)
- [ListAccountPermissionsResponseTypeDef](./type_defs.md#listaccountpermissionsresponsetypedef)
- [NetworkPathTypeDef](./type_defs.md#networkpathtypedef)
- [PackageVulnerabilityDetailsTypeDef](./type_defs.md#packagevulnerabilitydetailstypedef)
- [RemediationTypeDef](./type_defs.md#remediationtypedef)
- [ResourceFilterCriteriaTypeDef](./type_defs.md#resourcefiltercriteriatypedef)
- [SearchVulnerabilitiesRequestRequestTypeDef](./type_defs.md#searchvulnerabilitiesrequestrequesttypedef)
- [SearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef](./type_defs.md#searchvulnerabilitiesrequestsearchvulnerabilitiespaginatetypedef)
- [UsageTotalTypeDef](./type_defs.md#usagetotaltypedef)
- [AggregationResponseTypeDef](./type_defs.md#aggregationresponsetypedef)
- [AccountStateTypeDef](./type_defs.md#accountstatetypedef)
- [DisableResponseTypeDef](./type_defs.md#disableresponsetypedef)
- [EnableResponseTypeDef](./type_defs.md#enableresponsetypedef)
- [ResourceDetailsTypeDef](./type_defs.md#resourcedetailstypedef)
- [BatchGetCodeSnippetResponseTypeDef](./type_defs.md#batchgetcodesnippetresponsetypedef)
- [CoverageFilterCriteriaTypeDef](./type_defs.md#coveragefiltercriteriatypedef)
- [InspectorScoreDetailsTypeDef](./type_defs.md#inspectorscoredetailstypedef)
- [AggregationRequestTypeDef](./type_defs.md#aggregationrequesttypedef)
- [GetConfigurationResponseTypeDef](./type_defs.md#getconfigurationresponsetypedef)
- [BatchGetFindingDetailsResponseTypeDef](./type_defs.md#batchgetfindingdetailsresponsetypedef)
- [SearchVulnerabilitiesResponseTypeDef](./type_defs.md#searchvulnerabilitiesresponsetypedef)
- [FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef)
- [BatchGetFreeTrialInfoResponseTypeDef](./type_defs.md#batchgetfreetrialinforesponsetypedef)
- [CoveredResourceTypeDef](./type_defs.md#coveredresourcetypedef)
- [NetworkReachabilityDetailsTypeDef](./type_defs.md#networkreachabilitydetailstypedef)
- [CreateSbomExportRequestRequestTypeDef](./type_defs.md#createsbomexportrequestrequesttypedef)
- [GetSbomExportResponseTypeDef](./type_defs.md#getsbomexportresponsetypedef)
- [ListUsageTotalsResponseTypeDef](./type_defs.md#listusagetotalsresponsetypedef)
- [ListFindingAggregationsResponseTypeDef](./type_defs.md#listfindingaggregationsresponsetypedef)
- [BatchGetAccountStatusResponseTypeDef](./type_defs.md#batchgetaccountstatusresponsetypedef)
- [ResourceTypeDef](./type_defs.md#resourcetypedef)
- [ListCoverageRequestListCoveragePaginateTypeDef](./type_defs.md#listcoveragerequestlistcoveragepaginatetypedef)
- [ListCoverageRequestRequestTypeDef](./type_defs.md#listcoveragerequestrequesttypedef)
- [ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef](./type_defs.md#listcoveragestatisticsrequestlistcoveragestatisticspaginatetypedef)
- [ListCoverageStatisticsRequestRequestTypeDef](./type_defs.md#listcoveragestatisticsrequestrequesttypedef)
- [ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef](./type_defs.md#listfindingaggregationsrequestlistfindingaggregationspaginatetypedef)
- [ListFindingAggregationsRequestRequestTypeDef](./type_defs.md#listfindingaggregationsrequestrequesttypedef)
- [CreateFilterRequestRequestTypeDef](./type_defs.md#createfilterrequestrequesttypedef)
- [CreateFindingsReportRequestRequestTypeDef](./type_defs.md#createfindingsreportrequestrequesttypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [GetFindingsReportStatusResponseTypeDef](./type_defs.md#getfindingsreportstatusresponsetypedef)
- [ListFindingsRequestListFindingsPaginateTypeDef](./type_defs.md#listfindingsrequestlistfindingspaginatetypedef)
- [ListFindingsRequestRequestTypeDef](./type_defs.md#listfindingsrequestrequesttypedef)
- [UpdateFilterRequestRequestTypeDef](./type_defs.md#updatefilterrequestrequesttypedef)
- [ListCoverageResponseTypeDef](./type_defs.md#listcoverageresponsetypedef)
- [FindingTypeDef](./type_defs.md#findingtypedef)
- [ListFiltersResponseTypeDef](./type_defs.md#listfiltersresponsetypedef)
- [ListFindingsResponseTypeDef](./type_defs.md#listfindingsresponsetypedef)

