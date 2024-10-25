# Macie2 module

> [Index](../README.md) > Macie2


!!! note ""

    Auto-generated documentation for [Macie2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
    type annotations stubs module [types-aiobotocore-macie2](https://pypi.org/project/types-aiobotocore-macie2/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `Macie2` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[macie2]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[macie2]'


# standalone installation
python -m pip install types-aiobotocore-macie2
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-macie2
```

## Usage

Code samples can be found in [Examples](./usage.md).

## Macie2Client

Type annotations and code completion for  `#!python session.create_client("macie2")` as [Macie2Client](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client)

```python
# Macie2Client usage example

from aiobotocore.session import get_session

from types_aiobotocore_macie2.client import Macie2Client


session = get_session()
async with session.create_client("macie2") as client:
    client: Macie2Client
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("macie2").get_paginator("...")`.

```python
# DescribeBucketsPaginator usage example

from types_aiobotocore_macie2.paginator import DescribeBucketsPaginator

def get_describe_buckets_paginator() -> DescribeBucketsPaginator:
    return client.get_paginator("describe_buckets"))
```

- [DescribeBucketsPaginator](./paginators.md#describebucketspaginator)
- [GetUsageStatisticsPaginator](./paginators.md#getusagestatisticspaginator)
- [ListAllowListsPaginator](./paginators.md#listallowlistspaginator)
- [ListAutomatedDiscoveryAccountsPaginator](./paginators.md#listautomateddiscoveryaccountspaginator)
- [ListClassificationJobsPaginator](./paginators.md#listclassificationjobspaginator)
- [ListClassificationScopesPaginator](./paginators.md#listclassificationscopespaginator)
- [ListCustomDataIdentifiersPaginator](./paginators.md#listcustomdataidentifierspaginator)
- [ListFindingsPaginator](./paginators.md#listfindingspaginator)
- [ListFindingsFiltersPaginator](./paginators.md#listfindingsfilterspaginator)
- [ListInvitationsPaginator](./paginators.md#listinvitationspaginator)
- [ListManagedDataIdentifiersPaginator](./paginators.md#listmanageddataidentifierspaginator)
- [ListMembersPaginator](./paginators.md#listmemberspaginator)
- [ListOrganizationAdminAccountsPaginator](./paginators.md#listorganizationadminaccountspaginator)
- [ListResourceProfileArtifactsPaginator](./paginators.md#listresourceprofileartifactspaginator)
- [ListResourceProfileDetectionsPaginator](./paginators.md#listresourceprofiledetectionspaginator)
- [ListSensitivityInspectionTemplatesPaginator](./paginators.md#listsensitivityinspectiontemplatespaginator)
- [SearchResourcesPaginator](./paginators.md#searchresourcespaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("macie2").get_waiter("...")`.

```python
# FindingRevealedWaiter usage example

from types_aiobotocore_macie2.waiter import FindingRevealedWaiter

def get_finding_revealed_waiter() -> FindingRevealedWaiter:
    return Session().client("macie2").get_waiter("finding_revealed")
```

- [FindingRevealedWaiter](./waiters.md#findingrevealedwaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AdminStatusType usage example

from types_aiobotocore_macie2.literals import AdminStatusType

def get_value() -> AdminStatusType:
    return "DISABLING_IN_PROGRESS"
```

- [AdminStatusType](./literals.md#adminstatustype)
- [AllowListStatusCodeType](./literals.md#allowliststatuscodetype)
- [AllowsUnencryptedObjectUploadsType](./literals.md#allowsunencryptedobjectuploadstype)
- [AutoEnableModeType](./literals.md#autoenablemodetype)
- [AutomatedDiscoveryAccountStatusType](./literals.md#automateddiscoveryaccountstatustype)
- [AutomatedDiscoveryAccountUpdateErrorCodeType](./literals.md#automateddiscoveryaccountupdateerrorcodetype)
- [AutomatedDiscoveryMonitoringStatusType](./literals.md#automateddiscoverymonitoringstatustype)
- [AutomatedDiscoveryStatusType](./literals.md#automateddiscoverystatustype)
- [AvailabilityCodeType](./literals.md#availabilitycodetype)
- [BucketMetadataErrorCodeType](./literals.md#bucketmetadataerrorcodetype)
- [ClassificationScopeUpdateOperationType](./literals.md#classificationscopeupdateoperationtype)
- [CurrencyType](./literals.md#currencytype)
- [DataIdentifierSeverityType](./literals.md#dataidentifierseveritytype)
- [DataIdentifierTypeType](./literals.md#dataidentifiertypetype)
- [DayOfWeekType](./literals.md#dayofweektype)
- [DescribeBucketsPaginatorName](./literals.md#describebucketspaginatorname)
- [EffectivePermissionType](./literals.md#effectivepermissiontype)
- [EncryptionTypeType](./literals.md#encryptiontypetype)
- [ErrorCodeType](./literals.md#errorcodetype)
- [FindingActionTypeType](./literals.md#findingactiontypetype)
- [FindingCategoryType](./literals.md#findingcategorytype)
- [FindingPublishingFrequencyType](./literals.md#findingpublishingfrequencytype)
- [FindingRevealedWaiterName](./literals.md#findingrevealedwaitername)
- [FindingStatisticsSortAttributeNameType](./literals.md#findingstatisticssortattributenametype)
- [FindingTypeType](./literals.md#findingtypetype)
- [FindingsFilterActionType](./literals.md#findingsfilteractiontype)
- [GetUsageStatisticsPaginatorName](./literals.md#getusagestatisticspaginatorname)
- [GroupByType](./literals.md#groupbytype)
- [IsDefinedInJobType](./literals.md#isdefinedinjobtype)
- [IsMonitoredByJobType](./literals.md#ismonitoredbyjobtype)
- [JobComparatorType](./literals.md#jobcomparatortype)
- [JobStatusType](./literals.md#jobstatustype)
- [JobTypeType](./literals.md#jobtypetype)
- [LastRunErrorStatusCodeType](./literals.md#lastrunerrorstatuscodetype)
- [ListAllowListsPaginatorName](./literals.md#listallowlistspaginatorname)
- [ListAutomatedDiscoveryAccountsPaginatorName](./literals.md#listautomateddiscoveryaccountspaginatorname)
- [ListClassificationJobsPaginatorName](./literals.md#listclassificationjobspaginatorname)
- [ListClassificationScopesPaginatorName](./literals.md#listclassificationscopespaginatorname)
- [ListCustomDataIdentifiersPaginatorName](./literals.md#listcustomdataidentifierspaginatorname)
- [ListFindingsFiltersPaginatorName](./literals.md#listfindingsfilterspaginatorname)
- [ListFindingsPaginatorName](./literals.md#listfindingspaginatorname)
- [ListInvitationsPaginatorName](./literals.md#listinvitationspaginatorname)
- [ListJobsFilterKeyType](./literals.md#listjobsfilterkeytype)
- [ListJobsSortAttributeNameType](./literals.md#listjobssortattributenametype)
- [ListManagedDataIdentifiersPaginatorName](./literals.md#listmanageddataidentifierspaginatorname)
- [ListMembersPaginatorName](./literals.md#listmemberspaginatorname)
- [ListOrganizationAdminAccountsPaginatorName](./literals.md#listorganizationadminaccountspaginatorname)
- [ListResourceProfileArtifactsPaginatorName](./literals.md#listresourceprofileartifactspaginatorname)
- [ListResourceProfileDetectionsPaginatorName](./literals.md#listresourceprofiledetectionspaginatorname)
- [ListSensitivityInspectionTemplatesPaginatorName](./literals.md#listsensitivityinspectiontemplatespaginatorname)
- [MacieStatusType](./literals.md#maciestatustype)
- [ManagedDataIdentifierSelectorType](./literals.md#manageddataidentifierselectortype)
- [OrderByType](./literals.md#orderbytype)
- [OriginTypeType](./literals.md#origintypetype)
- [RelationshipStatusType](./literals.md#relationshipstatustype)
- [RetrievalModeType](./literals.md#retrievalmodetype)
- [RevealRequestStatusType](./literals.md#revealrequeststatustype)
- [RevealStatusType](./literals.md#revealstatustype)
- [ScopeFilterKeyType](./literals.md#scopefilterkeytype)
- [SearchResourcesComparatorType](./literals.md#searchresourcescomparatortype)
- [SearchResourcesPaginatorName](./literals.md#searchresourcespaginatorname)
- [SearchResourcesSimpleCriterionKeyType](./literals.md#searchresourcessimplecriterionkeytype)
- [SearchResourcesSortAttributeNameType](./literals.md#searchresourcessortattributenametype)
- [SensitiveDataItemCategoryType](./literals.md#sensitivedataitemcategorytype)
- [SeverityDescriptionType](./literals.md#severitydescriptiontype)
- [SharedAccessType](./literals.md#sharedaccesstype)
- [SimpleCriterionKeyForJobType](./literals.md#simplecriterionkeyforjobtype)
- [StorageClassType](./literals.md#storageclasstype)
- [TagTargetType](./literals.md#tagtargettype)
- [TimeRangeType](./literals.md#timerangetype)
- [TypeType](./literals.md#typetype)
- [UnavailabilityReasonCodeType](./literals.md#unavailabilityreasoncodetype)
- [UnitType](./literals.md#unittype)
- [UsageStatisticsFilterComparatorType](./literals.md#usagestatisticsfiltercomparatortype)
- [UsageStatisticsFilterKeyType](./literals.md#usagestatisticsfilterkeytype)
- [UsageStatisticsSortKeyType](./literals.md#usagestatisticssortkeytype)
- [UsageTypeType](./literals.md#usagetypetype)
- [UserIdentityTypeType](./literals.md#useridentitytypetype)
- [Macie2ServiceName](./literals.md#macie2servicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AcceptInvitationRequestRequestTypeDef](./type_defs.md#acceptinvitationrequestrequesttypedef)
- [AccessControlListTypeDef](./type_defs.md#accesscontrollisttypedef)
- [AccountDetailTypeDef](./type_defs.md#accountdetailtypedef)
- [BlockPublicAccessTypeDef](./type_defs.md#blockpublicaccesstypedef)
- [AdminAccountTypeDef](./type_defs.md#adminaccounttypedef)
- [S3WordsListTypeDef](./type_defs.md#s3wordslisttypedef)
- [AllowListStatusTypeDef](./type_defs.md#allowliststatustypedef)
- [AllowListSummaryTypeDef](./type_defs.md#allowlistsummarytypedef)
- [ApiCallDetailsTypeDef](./type_defs.md#apicalldetailstypedef)
- [AutomatedDiscoveryAccountTypeDef](./type_defs.md#automateddiscoveryaccounttypedef)
- [AutomatedDiscoveryAccountUpdateErrorTypeDef](./type_defs.md#automateddiscoveryaccountupdateerrortypedef)
- [AutomatedDiscoveryAccountUpdateTypeDef](./type_defs.md#automateddiscoveryaccountupdatetypedef)
- [AwsAccountTypeDef](./type_defs.md#awsaccounttypedef)
- [AwsServiceTypeDef](./type_defs.md#awsservicetypedef)
- [BatchGetCustomDataIdentifierSummaryTypeDef](./type_defs.md#batchgetcustomdataidentifiersummarytypedef)
- [BatchGetCustomDataIdentifiersRequestRequestTypeDef](./type_defs.md#batchgetcustomdataidentifiersrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BucketCountByEffectivePermissionTypeDef](./type_defs.md#bucketcountbyeffectivepermissiontypedef)
- [BucketCountByEncryptionTypeTypeDef](./type_defs.md#bucketcountbyencryptiontypetypedef)
- [BucketCountBySharedAccessTypeTypeDef](./type_defs.md#bucketcountbysharedaccesstypetypedef)
- [BucketCountPolicyAllowsUnencryptedObjectUploadsTypeDef](./type_defs.md#bucketcountpolicyallowsunencryptedobjectuploadstypedef)
- [BucketCriteriaAdditionalPropertiesTypeDef](./type_defs.md#bucketcriteriaadditionalpropertiestypedef)
- [BucketPolicyTypeDef](./type_defs.md#bucketpolicytypedef)
- [BucketServerSideEncryptionTypeDef](./type_defs.md#bucketserversideencryptiontypedef)
- [JobDetailsTypeDef](./type_defs.md#jobdetailstypedef)
- [KeyValuePairTypeDef](./type_defs.md#keyvaluepairtypedef)
- [ObjectCountByEncryptionTypeTypeDef](./type_defs.md#objectcountbyencryptiontypetypedef)
- [ObjectLevelStatisticsTypeDef](./type_defs.md#objectlevelstatisticstypedef)
- [ReplicationDetailsTypeDef](./type_defs.md#replicationdetailstypedef)
- [BucketSortCriteriaTypeDef](./type_defs.md#bucketsortcriteriatypedef)
- [SensitivityAggregationsTypeDef](./type_defs.md#sensitivityaggregationstypedef)
- [CellTypeDef](./type_defs.md#celltypedef)
- [S3DestinationTypeDef](./type_defs.md#s3destinationtypedef)
- [ClassificationResultStatusTypeDef](./type_defs.md#classificationresultstatustypedef)
- [ClassificationScopeSummaryTypeDef](./type_defs.md#classificationscopesummarytypedef)
- [SeverityLevelTypeDef](./type_defs.md#severityleveltypedef)
- [CreateInvitationsRequestRequestTypeDef](./type_defs.md#createinvitationsrequestrequesttypedef)
- [UnprocessedAccountTypeDef](./type_defs.md#unprocessedaccounttypedef)
- [CreateSampleFindingsRequestRequestTypeDef](./type_defs.md#createsamplefindingsrequestrequesttypedef)
- [SimpleCriterionForJobOutputTypeDef](./type_defs.md#simplecriterionforjoboutputtypedef)
- [CriterionAdditionalPropertiesOutputTypeDef](./type_defs.md#criterionadditionalpropertiesoutputtypedef)
- [CriterionAdditionalPropertiesTypeDef](./type_defs.md#criterionadditionalpropertiestypedef)
- [CustomDataIdentifierSummaryTypeDef](./type_defs.md#customdataidentifiersummarytypedef)
- [DeclineInvitationsRequestRequestTypeDef](./type_defs.md#declineinvitationsrequestrequesttypedef)
- [DeleteAllowListRequestRequestTypeDef](./type_defs.md#deleteallowlistrequestrequesttypedef)
- [DeleteCustomDataIdentifierRequestRequestTypeDef](./type_defs.md#deletecustomdataidentifierrequestrequesttypedef)
- [DeleteFindingsFilterRequestRequestTypeDef](./type_defs.md#deletefindingsfilterrequestrequesttypedef)
- [DeleteInvitationsRequestRequestTypeDef](./type_defs.md#deleteinvitationsrequestrequesttypedef)
- [DeleteMemberRequestRequestTypeDef](./type_defs.md#deletememberrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeClassificationJobRequestRequestTypeDef](./type_defs.md#describeclassificationjobrequestrequesttypedef)
- [LastRunErrorStatusTypeDef](./type_defs.md#lastrunerrorstatustypedef)
- [StatisticsTypeDef](./type_defs.md#statisticstypedef)
- [UserPausedDetailsTypeDef](./type_defs.md#userpauseddetailstypedef)
- [DetectedDataDetailsTypeDef](./type_defs.md#detecteddatadetailstypedef)
- [DetectionTypeDef](./type_defs.md#detectiontypedef)
- [DisableOrganizationAdminAccountRequestRequestTypeDef](./type_defs.md#disableorganizationadminaccountrequestrequesttypedef)
- [DisassociateMemberRequestRequestTypeDef](./type_defs.md#disassociatememberrequestrequesttypedef)
- [DomainDetailsTypeDef](./type_defs.md#domaindetailstypedef)
- [EnableMacieRequestRequestTypeDef](./type_defs.md#enablemacierequestrequesttypedef)
- [EnableOrganizationAdminAccountRequestRequestTypeDef](./type_defs.md#enableorganizationadminaccountrequestrequesttypedef)
- [FindingStatisticsSortCriteriaTypeDef](./type_defs.md#findingstatisticssortcriteriatypedef)
- [SeverityTypeDef](./type_defs.md#severitytypedef)
- [FindingsFilterListItemTypeDef](./type_defs.md#findingsfilterlistitemtypedef)
- [InvitationTypeDef](./type_defs.md#invitationtypedef)
- [GetAllowListRequestRequestTypeDef](./type_defs.md#getallowlistrequestrequesttypedef)
- [GetBucketStatisticsRequestRequestTypeDef](./type_defs.md#getbucketstatisticsrequestrequesttypedef)
- [GetClassificationScopeRequestRequestTypeDef](./type_defs.md#getclassificationscoperequestrequesttypedef)
- [GetCustomDataIdentifierRequestRequestTypeDef](./type_defs.md#getcustomdataidentifierrequestrequesttypedef)
- [GroupCountTypeDef](./type_defs.md#groupcounttypedef)
- [GetFindingsFilterRequestRequestTypeDef](./type_defs.md#getfindingsfilterrequestrequesttypedef)
- [SecurityHubConfigurationTypeDef](./type_defs.md#securityhubconfigurationtypedef)
- [SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef)
- [GetMemberRequestRequestTypeDef](./type_defs.md#getmemberrequestrequesttypedef)
- [GetResourceProfileRequestRequestTypeDef](./type_defs.md#getresourceprofilerequestrequesttypedef)
- [ResourceStatisticsTypeDef](./type_defs.md#resourcestatisticstypedef)
- [RetrievalConfigurationTypeDef](./type_defs.md#retrievalconfigurationtypedef)
- [RevealConfigurationTypeDef](./type_defs.md#revealconfigurationtypedef)
- [GetSensitiveDataOccurrencesAvailabilityRequestRequestTypeDef](./type_defs.md#getsensitivedataoccurrencesavailabilityrequestrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [GetSensitiveDataOccurrencesRequestRequestTypeDef](./type_defs.md#getsensitivedataoccurrencesrequestrequesttypedef)
- [GetSensitivityInspectionTemplateRequestRequestTypeDef](./type_defs.md#getsensitivityinspectiontemplaterequestrequesttypedef)
- [SensitivityInspectionTemplateExcludesOutputTypeDef](./type_defs.md#sensitivityinspectiontemplateexcludesoutputtypedef)
- [SensitivityInspectionTemplateIncludesOutputTypeDef](./type_defs.md#sensitivityinspectiontemplateincludesoutputtypedef)
- [UsageStatisticsFilterTypeDef](./type_defs.md#usagestatisticsfiltertypedef)
- [UsageStatisticsSortByTypeDef](./type_defs.md#usagestatisticssortbytypedef)
- [GetUsageTotalsRequestRequestTypeDef](./type_defs.md#getusagetotalsrequestrequesttypedef)
- [UsageTotalTypeDef](./type_defs.md#usagetotaltypedef)
- [IamUserTypeDef](./type_defs.md#iamusertypedef)
- [IpCityTypeDef](./type_defs.md#ipcitytypedef)
- [IpCountryTypeDef](./type_defs.md#ipcountrytypedef)
- [IpGeoLocationTypeDef](./type_defs.md#ipgeolocationtypedef)
- [IpOwnerTypeDef](./type_defs.md#ipownertypedef)
- [MonthlyScheduleTypeDef](./type_defs.md#monthlyscheduletypedef)
- [WeeklyScheduleTypeDef](./type_defs.md#weeklyscheduletypedef)
- [SimpleScopeTermOutputTypeDef](./type_defs.md#simplescopetermoutputtypedef)
- [S3BucketDefinitionForJobOutputTypeDef](./type_defs.md#s3bucketdefinitionforjoboutputtypedef)
- [ListAllowListsRequestRequestTypeDef](./type_defs.md#listallowlistsrequestrequesttypedef)
- [ListAutomatedDiscoveryAccountsRequestRequestTypeDef](./type_defs.md#listautomateddiscoveryaccountsrequestrequesttypedef)
- [ListJobsSortCriteriaTypeDef](./type_defs.md#listjobssortcriteriatypedef)
- [ListClassificationScopesRequestRequestTypeDef](./type_defs.md#listclassificationscopesrequestrequesttypedef)
- [ListCustomDataIdentifiersRequestRequestTypeDef](./type_defs.md#listcustomdataidentifiersrequestrequesttypedef)
- [ListFindingsFiltersRequestRequestTypeDef](./type_defs.md#listfindingsfiltersrequestrequesttypedef)
- [ListInvitationsRequestRequestTypeDef](./type_defs.md#listinvitationsrequestrequesttypedef)
- [ListJobsFilterTermTypeDef](./type_defs.md#listjobsfiltertermtypedef)
- [ListManagedDataIdentifiersRequestRequestTypeDef](./type_defs.md#listmanageddataidentifiersrequestrequesttypedef)
- [ManagedDataIdentifierSummaryTypeDef](./type_defs.md#manageddataidentifiersummarytypedef)
- [ListMembersRequestRequestTypeDef](./type_defs.md#listmembersrequestrequesttypedef)
- [MemberTypeDef](./type_defs.md#membertypedef)
- [ListOrganizationAdminAccountsRequestRequestTypeDef](./type_defs.md#listorganizationadminaccountsrequestrequesttypedef)
- [ListResourceProfileArtifactsRequestRequestTypeDef](./type_defs.md#listresourceprofileartifactsrequestrequesttypedef)
- [ResourceProfileArtifactTypeDef](./type_defs.md#resourceprofileartifacttypedef)
- [ListResourceProfileDetectionsRequestRequestTypeDef](./type_defs.md#listresourceprofiledetectionsrequestrequesttypedef)
- [ListSensitivityInspectionTemplatesRequestRequestTypeDef](./type_defs.md#listsensitivityinspectiontemplatesrequestrequesttypedef)
- [SensitivityInspectionTemplatesEntryTypeDef](./type_defs.md#sensitivityinspectiontemplatesentrytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [RangeTypeDef](./type_defs.md#rangetypedef)
- [RecordTypeDef](./type_defs.md#recordtypedef)
- [S3BucketDefinitionForJobTypeDef](./type_defs.md#s3bucketdefinitionforjobtypedef)
- [S3BucketOwnerTypeDef](./type_defs.md#s3bucketownertypedef)
- [ServerSideEncryptionTypeDef](./type_defs.md#serversideencryptiontypedef)
- [S3ClassificationScopeExclusionTypeDef](./type_defs.md#s3classificationscopeexclusiontypedef)
- [S3ClassificationScopeExclusionUpdateTypeDef](./type_defs.md#s3classificationscopeexclusionupdatetypedef)
- [SearchResourcesSimpleCriterionTypeDef](./type_defs.md#searchresourcessimplecriteriontypedef)
- [SearchResourcesSortCriteriaTypeDef](./type_defs.md#searchresourcessortcriteriatypedef)
- [SearchResourcesTagCriterionPairTypeDef](./type_defs.md#searchresourcestagcriterionpairtypedef)
- [SensitivityInspectionTemplateExcludesTypeDef](./type_defs.md#sensitivityinspectiontemplateexcludestypedef)
- [SensitivityInspectionTemplateIncludesTypeDef](./type_defs.md#sensitivityinspectiontemplateincludestypedef)
- [ServiceLimitTypeDef](./type_defs.md#servicelimittypedef)
- [SessionContextAttributesTypeDef](./type_defs.md#sessioncontextattributestypedef)
- [SessionIssuerTypeDef](./type_defs.md#sessionissuertypedef)
- [SimpleCriterionForJobTypeDef](./type_defs.md#simplecriterionforjobtypedef)
- [SimpleScopeTermTypeDef](./type_defs.md#simplescopetermtypedef)
- [SuppressDataIdentifierTypeDef](./type_defs.md#suppressdataidentifiertypedef)
- [TagCriterionPairForJobTypeDef](./type_defs.md#tagcriterionpairforjobtypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [TagValuePairTypeDef](./type_defs.md#tagvaluepairtypedef)
- [TestCustomDataIdentifierRequestRequestTypeDef](./type_defs.md#testcustomdataidentifierrequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateAutomatedDiscoveryConfigurationRequestRequestTypeDef](./type_defs.md#updateautomateddiscoveryconfigurationrequestrequesttypedef)
- [UpdateClassificationJobRequestRequestTypeDef](./type_defs.md#updateclassificationjobrequestrequesttypedef)
- [UpdateMacieSessionRequestRequestTypeDef](./type_defs.md#updatemaciesessionrequestrequesttypedef)
- [UpdateMemberSessionRequestRequestTypeDef](./type_defs.md#updatemembersessionrequestrequesttypedef)
- [UpdateOrganizationConfigurationRequestRequestTypeDef](./type_defs.md#updateorganizationconfigurationrequestrequesttypedef)
- [UpdateResourceProfileRequestRequestTypeDef](./type_defs.md#updateresourceprofilerequestrequesttypedef)
- [UpdateRetrievalConfigurationTypeDef](./type_defs.md#updateretrievalconfigurationtypedef)
- [UserIdentityRootTypeDef](./type_defs.md#useridentityroottypedef)
- [CreateMemberRequestRequestTypeDef](./type_defs.md#creatememberrequestrequesttypedef)
- [AccountLevelPermissionsTypeDef](./type_defs.md#accountlevelpermissionstypedef)
- [AllowListCriteriaTypeDef](./type_defs.md#allowlistcriteriatypedef)
- [FindingActionTypeDef](./type_defs.md#findingactiontypedef)
- [BatchUpdateAutomatedDiscoveryAccountsRequestRequestTypeDef](./type_defs.md#batchupdateautomateddiscoveryaccountsrequestrequesttypedef)
- [BatchGetCustomDataIdentifiersResponseTypeDef](./type_defs.md#batchgetcustomdataidentifiersresponsetypedef)
- [BatchUpdateAutomatedDiscoveryAccountsResponseTypeDef](./type_defs.md#batchupdateautomateddiscoveryaccountsresponsetypedef)
- [CreateAllowListResponseTypeDef](./type_defs.md#createallowlistresponsetypedef)
- [CreateClassificationJobResponseTypeDef](./type_defs.md#createclassificationjobresponsetypedef)
- [CreateCustomDataIdentifierResponseTypeDef](./type_defs.md#createcustomdataidentifierresponsetypedef)
- [CreateFindingsFilterResponseTypeDef](./type_defs.md#createfindingsfilterresponsetypedef)
- [CreateMemberResponseTypeDef](./type_defs.md#creatememberresponsetypedef)
- [DescribeOrganizationConfigurationResponseTypeDef](./type_defs.md#describeorganizationconfigurationresponsetypedef)
- [GetAutomatedDiscoveryConfigurationResponseTypeDef](./type_defs.md#getautomateddiscoveryconfigurationresponsetypedef)
- [GetInvitationsCountResponseTypeDef](./type_defs.md#getinvitationscountresponsetypedef)
- [GetMacieSessionResponseTypeDef](./type_defs.md#getmaciesessionresponsetypedef)
- [GetMemberResponseTypeDef](./type_defs.md#getmemberresponsetypedef)
- [GetSensitiveDataOccurrencesAvailabilityResponseTypeDef](./type_defs.md#getsensitivedataoccurrencesavailabilityresponsetypedef)
- [ListAllowListsResponseTypeDef](./type_defs.md#listallowlistsresponsetypedef)
- [ListAutomatedDiscoveryAccountsResponseTypeDef](./type_defs.md#listautomateddiscoveryaccountsresponsetypedef)
- [ListFindingsResponseTypeDef](./type_defs.md#listfindingsresponsetypedef)
- [ListOrganizationAdminAccountsResponseTypeDef](./type_defs.md#listorganizationadminaccountsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TestCustomDataIdentifierResponseTypeDef](./type_defs.md#testcustomdataidentifierresponsetypedef)
- [UpdateAllowListResponseTypeDef](./type_defs.md#updateallowlistresponsetypedef)
- [UpdateFindingsFilterResponseTypeDef](./type_defs.md#updatefindingsfilterresponsetypedef)
- [BucketLevelPermissionsTypeDef](./type_defs.md#bucketlevelpermissionstypedef)
- [MatchingBucketTypeDef](./type_defs.md#matchingbuckettypedef)
- [DescribeBucketsRequestRequestTypeDef](./type_defs.md#describebucketsrequestrequesttypedef)
- [BucketStatisticsBySensitivityTypeDef](./type_defs.md#bucketstatisticsbysensitivitytypedef)
- [ClassificationExportConfigurationTypeDef](./type_defs.md#classificationexportconfigurationtypedef)
- [ListClassificationScopesResponseTypeDef](./type_defs.md#listclassificationscopesresponsetypedef)
- [CreateCustomDataIdentifierRequestRequestTypeDef](./type_defs.md#createcustomdataidentifierrequestrequesttypedef)
- [GetCustomDataIdentifierResponseTypeDef](./type_defs.md#getcustomdataidentifierresponsetypedef)
- [CreateInvitationsResponseTypeDef](./type_defs.md#createinvitationsresponsetypedef)
- [DeclineInvitationsResponseTypeDef](./type_defs.md#declineinvitationsresponsetypedef)
- [DeleteInvitationsResponseTypeDef](./type_defs.md#deleteinvitationsresponsetypedef)
- [FindingCriteriaOutputTypeDef](./type_defs.md#findingcriteriaoutputtypedef)
- [CriterionAdditionalPropertiesUnionTypeDef](./type_defs.md#criterionadditionalpropertiesuniontypedef)
- [ListCustomDataIdentifiersResponseTypeDef](./type_defs.md#listcustomdataidentifiersresponsetypedef)
- [DescribeBucketsRequestDescribeBucketsPaginateTypeDef](./type_defs.md#describebucketsrequestdescribebucketspaginatetypedef)
- [ListAllowListsRequestListAllowListsPaginateTypeDef](./type_defs.md#listallowlistsrequestlistallowlistspaginatetypedef)
- [ListAutomatedDiscoveryAccountsRequestListAutomatedDiscoveryAccountsPaginateTypeDef](./type_defs.md#listautomateddiscoveryaccountsrequestlistautomateddiscoveryaccountspaginatetypedef)
- [ListClassificationScopesRequestListClassificationScopesPaginateTypeDef](./type_defs.md#listclassificationscopesrequestlistclassificationscopespaginatetypedef)
- [ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef](./type_defs.md#listcustomdataidentifiersrequestlistcustomdataidentifierspaginatetypedef)
- [ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef](./type_defs.md#listfindingsfiltersrequestlistfindingsfilterspaginatetypedef)
- [ListInvitationsRequestListInvitationsPaginateTypeDef](./type_defs.md#listinvitationsrequestlistinvitationspaginatetypedef)
- [ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef](./type_defs.md#listmanageddataidentifiersrequestlistmanageddataidentifierspaginatetypedef)
- [ListMembersRequestListMembersPaginateTypeDef](./type_defs.md#listmembersrequestlistmemberspaginatetypedef)
- [ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef](./type_defs.md#listorganizationadminaccountsrequestlistorganizationadminaccountspaginatetypedef)
- [ListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef](./type_defs.md#listresourceprofileartifactsrequestlistresourceprofileartifactspaginatetypedef)
- [ListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef](./type_defs.md#listresourceprofiledetectionsrequestlistresourceprofiledetectionspaginatetypedef)
- [ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef](./type_defs.md#listsensitivityinspectiontemplatesrequestlistsensitivityinspectiontemplatespaginatetypedef)
- [GetSensitiveDataOccurrencesResponseTypeDef](./type_defs.md#getsensitivedataoccurrencesresponsetypedef)
- [ListResourceProfileDetectionsResponseTypeDef](./type_defs.md#listresourceprofiledetectionsresponsetypedef)
- [ListFindingsFiltersResponseTypeDef](./type_defs.md#listfindingsfiltersresponsetypedef)
- [GetAdministratorAccountResponseTypeDef](./type_defs.md#getadministratoraccountresponsetypedef)
- [GetMasterAccountResponseTypeDef](./type_defs.md#getmasteraccountresponsetypedef)
- [ListInvitationsResponseTypeDef](./type_defs.md#listinvitationsresponsetypedef)
- [GetFindingStatisticsResponseTypeDef](./type_defs.md#getfindingstatisticsresponsetypedef)
- [GetFindingsPublicationConfigurationResponseTypeDef](./type_defs.md#getfindingspublicationconfigurationresponsetypedef)
- [PutFindingsPublicationConfigurationRequestRequestTypeDef](./type_defs.md#putfindingspublicationconfigurationrequestrequesttypedef)
- [GetFindingsRequestRequestTypeDef](./type_defs.md#getfindingsrequestrequesttypedef)
- [GetResourceProfileResponseTypeDef](./type_defs.md#getresourceprofileresponsetypedef)
- [GetRevealConfigurationResponseTypeDef](./type_defs.md#getrevealconfigurationresponsetypedef)
- [UpdateRevealConfigurationResponseTypeDef](./type_defs.md#updaterevealconfigurationresponsetypedef)
- [GetSensitiveDataOccurrencesRequestFindingRevealedWaitTypeDef](./type_defs.md#getsensitivedataoccurrencesrequestfindingrevealedwaittypedef)
- [GetSensitivityInspectionTemplateResponseTypeDef](./type_defs.md#getsensitivityinspectiontemplateresponsetypedef)
- [GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef](./type_defs.md#getusagestatisticsrequestgetusagestatisticspaginatetypedef)
- [GetUsageStatisticsRequestRequestTypeDef](./type_defs.md#getusagestatisticsrequestrequesttypedef)
- [GetUsageTotalsResponseTypeDef](./type_defs.md#getusagetotalsresponsetypedef)
- [IpAddressDetailsTypeDef](./type_defs.md#ipaddressdetailstypedef)
- [JobScheduleFrequencyOutputTypeDef](./type_defs.md#jobschedulefrequencyoutputtypedef)
- [JobScheduleFrequencyTypeDef](./type_defs.md#jobschedulefrequencytypedef)
- [ListJobsFilterCriteriaTypeDef](./type_defs.md#listjobsfiltercriteriatypedef)
- [ListManagedDataIdentifiersResponseTypeDef](./type_defs.md#listmanageddataidentifiersresponsetypedef)
- [ListMembersResponseTypeDef](./type_defs.md#listmembersresponsetypedef)
- [ListResourceProfileArtifactsResponseTypeDef](./type_defs.md#listresourceprofileartifactsresponsetypedef)
- [ListSensitivityInspectionTemplatesResponseTypeDef](./type_defs.md#listsensitivityinspectiontemplatesresponsetypedef)
- [PageTypeDef](./type_defs.md#pagetypedef)
- [S3BucketDefinitionForJobUnionTypeDef](./type_defs.md#s3bucketdefinitionforjobuniontypedef)
- [S3ObjectTypeDef](./type_defs.md#s3objecttypedef)
- [S3ClassificationScopeTypeDef](./type_defs.md#s3classificationscopetypedef)
- [S3ClassificationScopeUpdateTypeDef](./type_defs.md#s3classificationscopeupdatetypedef)
- [SearchResourcesTagCriterionTypeDef](./type_defs.md#searchresourcestagcriteriontypedef)
- [UpdateSensitivityInspectionTemplateRequestRequestTypeDef](./type_defs.md#updatesensitivityinspectiontemplaterequestrequesttypedef)
- [UsageByAccountTypeDef](./type_defs.md#usagebyaccounttypedef)
- [SessionContextTypeDef](./type_defs.md#sessioncontexttypedef)
- [SimpleCriterionForJobUnionTypeDef](./type_defs.md#simplecriterionforjobuniontypedef)
- [SimpleScopeTermUnionTypeDef](./type_defs.md#simplescopetermuniontypedef)
- [UpdateResourceProfileDetectionsRequestRequestTypeDef](./type_defs.md#updateresourceprofiledetectionsrequestrequesttypedef)
- [TagCriterionForJobOutputTypeDef](./type_defs.md#tagcriterionforjoboutputtypedef)
- [TagCriterionForJobTypeDef](./type_defs.md#tagcriterionforjobtypedef)
- [TagScopeTermOutputTypeDef](./type_defs.md#tagscopetermoutputtypedef)
- [TagScopeTermTypeDef](./type_defs.md#tagscopetermtypedef)
- [UpdateRevealConfigurationRequestRequestTypeDef](./type_defs.md#updaterevealconfigurationrequestrequesttypedef)
- [CreateAllowListRequestRequestTypeDef](./type_defs.md#createallowlistrequestrequesttypedef)
- [GetAllowListResponseTypeDef](./type_defs.md#getallowlistresponsetypedef)
- [UpdateAllowListRequestRequestTypeDef](./type_defs.md#updateallowlistrequestrequesttypedef)
- [BucketPermissionConfigurationTypeDef](./type_defs.md#bucketpermissionconfigurationtypedef)
- [MatchingResourceTypeDef](./type_defs.md#matchingresourcetypedef)
- [GetBucketStatisticsResponseTypeDef](./type_defs.md#getbucketstatisticsresponsetypedef)
- [GetClassificationExportConfigurationResponseTypeDef](./type_defs.md#getclassificationexportconfigurationresponsetypedef)
- [PutClassificationExportConfigurationRequestRequestTypeDef](./type_defs.md#putclassificationexportconfigurationrequestrequesttypedef)
- [PutClassificationExportConfigurationResponseTypeDef](./type_defs.md#putclassificationexportconfigurationresponsetypedef)
- [GetFindingsFilterResponseTypeDef](./type_defs.md#getfindingsfilterresponsetypedef)
- [FindingCriteriaTypeDef](./type_defs.md#findingcriteriatypedef)
- [ListClassificationJobsRequestListClassificationJobsPaginateTypeDef](./type_defs.md#listclassificationjobsrequestlistclassificationjobspaginatetypedef)
- [ListClassificationJobsRequestRequestTypeDef](./type_defs.md#listclassificationjobsrequestrequesttypedef)
- [OccurrencesTypeDef](./type_defs.md#occurrencestypedef)
- [GetClassificationScopeResponseTypeDef](./type_defs.md#getclassificationscoperesponsetypedef)
- [UpdateClassificationScopeRequestRequestTypeDef](./type_defs.md#updateclassificationscoperequestrequesttypedef)
- [SearchResourcesCriteriaTypeDef](./type_defs.md#searchresourcescriteriatypedef)
- [UsageRecordTypeDef](./type_defs.md#usagerecordtypedef)
- [AssumedRoleTypeDef](./type_defs.md#assumedroletypedef)
- [FederatedUserTypeDef](./type_defs.md#federatedusertypedef)
- [CriteriaForJobOutputTypeDef](./type_defs.md#criteriaforjoboutputtypedef)
- [TagCriterionForJobUnionTypeDef](./type_defs.md#tagcriterionforjobuniontypedef)
- [JobScopeTermOutputTypeDef](./type_defs.md#jobscopetermoutputtypedef)
- [TagScopeTermUnionTypeDef](./type_defs.md#tagscopetermuniontypedef)
- [BucketPublicAccessTypeDef](./type_defs.md#bucketpublicaccesstypedef)
- [SearchResourcesResponseTypeDef](./type_defs.md#searchresourcesresponsetypedef)
- [CreateFindingsFilterRequestRequestTypeDef](./type_defs.md#createfindingsfilterrequestrequesttypedef)
- [GetFindingStatisticsRequestRequestTypeDef](./type_defs.md#getfindingstatisticsrequestrequesttypedef)
- [ListFindingsRequestListFindingsPaginateTypeDef](./type_defs.md#listfindingsrequestlistfindingspaginatetypedef)
- [ListFindingsRequestRequestTypeDef](./type_defs.md#listfindingsrequestrequesttypedef)
- [UpdateFindingsFilterRequestRequestTypeDef](./type_defs.md#updatefindingsfilterrequestrequesttypedef)
- [CustomDetectionTypeDef](./type_defs.md#customdetectiontypedef)
- [DefaultDetectionTypeDef](./type_defs.md#defaultdetectiontypedef)
- [SearchResourcesCriteriaBlockTypeDef](./type_defs.md#searchresourcescriteriablocktypedef)
- [GetUsageStatisticsResponseTypeDef](./type_defs.md#getusagestatisticsresponsetypedef)
- [UserIdentityTypeDef](./type_defs.md#useridentitytypedef)
- [CriteriaBlockForJobOutputTypeDef](./type_defs.md#criteriablockforjoboutputtypedef)
- [CriteriaForJobTypeDef](./type_defs.md#criteriaforjobtypedef)
- [JobScopingBlockOutputTypeDef](./type_defs.md#jobscopingblockoutputtypedef)
- [JobScopeTermTypeDef](./type_defs.md#jobscopetermtypedef)
- [BucketMetadataTypeDef](./type_defs.md#bucketmetadatatypedef)
- [S3BucketTypeDef](./type_defs.md#s3buckettypedef)
- [CustomDataIdentifiersTypeDef](./type_defs.md#customdataidentifierstypedef)
- [SensitiveDataItemTypeDef](./type_defs.md#sensitivedataitemtypedef)
- [SearchResourcesBucketCriteriaTypeDef](./type_defs.md#searchresourcesbucketcriteriatypedef)
- [FindingActorTypeDef](./type_defs.md#findingactortypedef)
- [S3BucketCriteriaForJobOutputTypeDef](./type_defs.md#s3bucketcriteriaforjoboutputtypedef)
- [CriteriaForJobUnionTypeDef](./type_defs.md#criteriaforjobuniontypedef)
- [ScopingOutputTypeDef](./type_defs.md#scopingoutputtypedef)
- [JobScopeTermUnionTypeDef](./type_defs.md#jobscopetermuniontypedef)
- [DescribeBucketsResponseTypeDef](./type_defs.md#describebucketsresponsetypedef)
- [ResourcesAffectedTypeDef](./type_defs.md#resourcesaffectedtypedef)
- [ClassificationResultTypeDef](./type_defs.md#classificationresulttypedef)
- [SearchResourcesRequestRequestTypeDef](./type_defs.md#searchresourcesrequestrequesttypedef)
- [SearchResourcesRequestSearchResourcesPaginateTypeDef](./type_defs.md#searchresourcesrequestsearchresourcespaginatetypedef)
- [PolicyDetailsTypeDef](./type_defs.md#policydetailstypedef)
- [JobSummaryTypeDef](./type_defs.md#jobsummarytypedef)
- [CriteriaBlockForJobTypeDef](./type_defs.md#criteriablockforjobtypedef)
- [S3JobDefinitionOutputTypeDef](./type_defs.md#s3jobdefinitionoutputtypedef)
- [JobScopingBlockTypeDef](./type_defs.md#jobscopingblocktypedef)
- [ClassificationDetailsTypeDef](./type_defs.md#classificationdetailstypedef)
- [ListClassificationJobsResponseTypeDef](./type_defs.md#listclassificationjobsresponsetypedef)
- [CriteriaBlockForJobUnionTypeDef](./type_defs.md#criteriablockforjobuniontypedef)
- [DescribeClassificationJobResponseTypeDef](./type_defs.md#describeclassificationjobresponsetypedef)
- [JobScopingBlockUnionTypeDef](./type_defs.md#jobscopingblockuniontypedef)
- [FindingTypeDef](./type_defs.md#findingtypedef)
- [S3BucketCriteriaForJobTypeDef](./type_defs.md#s3bucketcriteriaforjobtypedef)
- [ScopingTypeDef](./type_defs.md#scopingtypedef)
- [GetFindingsResponseTypeDef](./type_defs.md#getfindingsresponsetypedef)
- [S3BucketCriteriaForJobUnionTypeDef](./type_defs.md#s3bucketcriteriaforjobuniontypedef)
- [ScopingUnionTypeDef](./type_defs.md#scopinguniontypedef)
- [S3JobDefinitionTypeDef](./type_defs.md#s3jobdefinitiontypedef)
- [CreateClassificationJobRequestRequestTypeDef](./type_defs.md#createclassificationjobrequestrequesttypedef)

