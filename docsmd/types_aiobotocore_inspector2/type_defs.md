# Type definitions

> [Index](../README.md) > [Inspector2](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Inspector2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
    type annotations stubs module [types-aiobotocore-inspector2](https://pypi.org/project/types-aiobotocore-inspector2/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## SeverityCountsTypeDef

```python
# SeverityCountsTypeDef definition

class SeverityCountsTypeDef(TypedDict):
    all: NotRequired[int],
    critical: NotRequired[int],
    high: NotRequired[int],
    medium: NotRequired[int],
```

## AccountAggregationTypeDef

```python
# AccountAggregationTypeDef definition

class AccountAggregationTypeDef(TypedDict):
    findingType: NotRequired[AggregationFindingTypeType],  # (1)
    resourceType: NotRequired[AggregationResourceTypeType],  # (2)
    sortBy: NotRequired[AccountSortByType],  # (3)
    sortOrder: NotRequired[SortOrderType],  # (4)
```

1. See [:material-code-brackets: AggregationFindingTypeType](./literals.md#aggregationfindingtypetype) 
2. See [:material-code-brackets: AggregationResourceTypeType](./literals.md#aggregationresourcetypetype) 
3. See [:material-code-brackets: AccountSortByType](./literals.md#accountsortbytype) 
4. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## StateTypeDef

```python
# StateTypeDef definition

class StateTypeDef(TypedDict):
    errorCode: ErrorCodeType,  # (1)
    errorMessage: str,
    status: StatusType,  # (2)
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## ResourceStatusTypeDef

```python
# ResourceStatusTypeDef definition

class ResourceStatusTypeDef(TypedDict):
    ec2: StatusType,  # (1)
    ecr: StatusType,  # (1)
    lambda: NotRequired[StatusType],  # (1)
    lambdaCode: NotRequired[StatusType],  # (1)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
3. See [:material-code-brackets: StatusType](./literals.md#statustype) 
4. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## FindingTypeAggregationTypeDef

```python
# FindingTypeAggregationTypeDef definition

class FindingTypeAggregationTypeDef(TypedDict):
    findingType: NotRequired[AggregationFindingTypeType],  # (1)
    resourceType: NotRequired[AggregationResourceTypeType],  # (2)
    sortBy: NotRequired[FindingTypeSortByType],  # (3)
    sortOrder: NotRequired[SortOrderType],  # (4)
```

1. See [:material-code-brackets: AggregationFindingTypeType](./literals.md#aggregationfindingtypetype) 
2. See [:material-code-brackets: AggregationResourceTypeType](./literals.md#aggregationresourcetypetype) 
3. See [:material-code-brackets: FindingTypeSortByType](./literals.md#findingtypesortbytype) 
4. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## StringFilterTypeDef

```python
# StringFilterTypeDef definition

class StringFilterTypeDef(TypedDict):
    comparison: StringComparisonType,  # (1)
    value: str,
```

1. See [:material-code-brackets: StringComparisonType](./literals.md#stringcomparisontype) 
## AssociateMemberRequestRequestTypeDef

```python
# AssociateMemberRequestRequestTypeDef definition

class AssociateMemberRequestRequestTypeDef(TypedDict):
    accountId: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## AtigDataTypeDef

```python
# AtigDataTypeDef definition

class AtigDataTypeDef(TypedDict):
    firstSeen: NotRequired[datetime],
    lastSeen: NotRequired[datetime],
    targets: NotRequired[List[str]],
    ttps: NotRequired[List[str]],
```

## AutoEnableTypeDef

```python
# AutoEnableTypeDef definition

class AutoEnableTypeDef(TypedDict):
    ec2: bool,
    ecr: bool,
    lambda: NotRequired[bool],
    lambdaCode: NotRequired[bool],
```

## AwsEc2InstanceDetailsTypeDef

```python
# AwsEc2InstanceDetailsTypeDef definition

class AwsEc2InstanceDetailsTypeDef(TypedDict):
    iamInstanceProfileArn: NotRequired[str],
    imageId: NotRequired[str],
    ipV4Addresses: NotRequired[List[str]],
    ipV6Addresses: NotRequired[List[str]],
    keyName: NotRequired[str],
    launchedAt: NotRequired[datetime],
    platform: NotRequired[str],
    subnetId: NotRequired[str],
    type: NotRequired[str],
    vpcId: NotRequired[str],
```

## AwsEcrContainerImageDetailsTypeDef

```python
# AwsEcrContainerImageDetailsTypeDef definition

class AwsEcrContainerImageDetailsTypeDef(TypedDict):
    imageHash: str,
    registry: str,
    repositoryName: str,
    architecture: NotRequired[str],
    author: NotRequired[str],
    imageTags: NotRequired[List[str]],
    platform: NotRequired[str],
    pushedAt: NotRequired[datetime],
```

## LambdaVpcConfigTypeDef

```python
# LambdaVpcConfigTypeDef definition

class LambdaVpcConfigTypeDef(TypedDict):
    securityGroupIds: NotRequired[List[str]],
    subnetIds: NotRequired[List[str]],
    vpcId: NotRequired[str],
```

## BatchGetAccountStatusRequestRequestTypeDef

```python
# BatchGetAccountStatusRequestRequestTypeDef definition

class BatchGetAccountStatusRequestRequestTypeDef(TypedDict):
    accountIds: NotRequired[Sequence[str]],
```

## BatchGetCodeSnippetRequestRequestTypeDef

```python
# BatchGetCodeSnippetRequestRequestTypeDef definition

class BatchGetCodeSnippetRequestRequestTypeDef(TypedDict):
    findingArns: Sequence[str],
```

## CodeSnippetErrorTypeDef

```python
# CodeSnippetErrorTypeDef definition

class CodeSnippetErrorTypeDef(TypedDict):
    errorCode: CodeSnippetErrorCodeType,  # (1)
    errorMessage: str,
    findingArn: str,
```

1. See [:material-code-brackets: CodeSnippetErrorCodeType](./literals.md#codesnippeterrorcodetype) 
## BatchGetFindingDetailsRequestRequestTypeDef

```python
# BatchGetFindingDetailsRequestRequestTypeDef definition

class BatchGetFindingDetailsRequestRequestTypeDef(TypedDict):
    findingArns: Sequence[str],
```

## FindingDetailsErrorTypeDef

```python
# FindingDetailsErrorTypeDef definition

class FindingDetailsErrorTypeDef(TypedDict):
    errorCode: FindingDetailsErrorCodeType,  # (1)
    errorMessage: str,
    findingArn: str,
```

1. See [:material-code-brackets: FindingDetailsErrorCodeType](./literals.md#findingdetailserrorcodetype) 
## BatchGetFreeTrialInfoRequestRequestTypeDef

```python
# BatchGetFreeTrialInfoRequestRequestTypeDef definition

class BatchGetFreeTrialInfoRequestRequestTypeDef(TypedDict):
    accountIds: Sequence[str],
```

## FreeTrialInfoErrorTypeDef

```python
# FreeTrialInfoErrorTypeDef definition

class FreeTrialInfoErrorTypeDef(TypedDict):
    accountId: str,
    code: FreeTrialInfoErrorCodeType,  # (1)
    message: str,
```

1. See [:material-code-brackets: FreeTrialInfoErrorCodeType](./literals.md#freetrialinfoerrorcodetype) 
## BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef

```python
# BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef definition

class BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef(TypedDict):
    accountIds: NotRequired[Sequence[str]],
```

## FailedMemberAccountEc2DeepInspectionStatusStateTypeDef

```python
# FailedMemberAccountEc2DeepInspectionStatusStateTypeDef definition

class FailedMemberAccountEc2DeepInspectionStatusStateTypeDef(TypedDict):
    accountId: str,
    ec2ScanStatus: NotRequired[StatusType],  # (1)
    errorMessage: NotRequired[str],
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## MemberAccountEc2DeepInspectionStatusStateTypeDef

```python
# MemberAccountEc2DeepInspectionStatusStateTypeDef definition

class MemberAccountEc2DeepInspectionStatusStateTypeDef(TypedDict):
    accountId: str,
    errorMessage: NotRequired[str],
    status: NotRequired[Ec2DeepInspectionStatusType],  # (1)
```

1. See [:material-code-brackets: Ec2DeepInspectionStatusType](./literals.md#ec2deepinspectionstatustype) 
## MemberAccountEc2DeepInspectionStatusTypeDef

```python
# MemberAccountEc2DeepInspectionStatusTypeDef definition

class MemberAccountEc2DeepInspectionStatusTypeDef(TypedDict):
    accountId: str,
    activateDeepInspection: bool,
```

## CancelFindingsReportRequestRequestTypeDef

```python
# CancelFindingsReportRequestRequestTypeDef definition

class CancelFindingsReportRequestRequestTypeDef(TypedDict):
    reportId: str,
```

## CancelSbomExportRequestRequestTypeDef

```python
# CancelSbomExportRequestRequestTypeDef definition

class CancelSbomExportRequestRequestTypeDef(TypedDict):
    reportId: str,
```

## CisaDataTypeDef

```python
# CisaDataTypeDef definition

class CisaDataTypeDef(TypedDict):
    action: NotRequired[str],
    dateAdded: NotRequired[datetime],
    dateDue: NotRequired[datetime],
```

## CodeFilePathTypeDef

```python
# CodeFilePathTypeDef definition

class CodeFilePathTypeDef(TypedDict):
    endLine: int,
    fileName: str,
    filePath: str,
    startLine: int,
```

## CodeLineTypeDef

```python
# CodeLineTypeDef definition

class CodeLineTypeDef(TypedDict):
    content: str,
    lineNumber: int,
```

## SuggestedFixTypeDef

```python
# SuggestedFixTypeDef definition

class SuggestedFixTypeDef(TypedDict):
    code: NotRequired[str],
    description: NotRequired[str],
```

## CountsTypeDef

```python
# CountsTypeDef definition

class CountsTypeDef(TypedDict):
    count: NotRequired[int],
    groupKey: NotRequired[GroupKeyType],  # (1)
```

1. See [:material-code-brackets: GroupKeyType](./literals.md#groupkeytype) 
## CoverageMapFilterTypeDef

```python
# CoverageMapFilterTypeDef definition

class CoverageMapFilterTypeDef(TypedDict):
    comparison: CoverageMapComparisonType,  # (1)
    key: str,
    value: NotRequired[str],
```

1. See [:material-code-brackets: CoverageMapComparisonType](./literals.md#coveragemapcomparisontype) 
## CoverageStringFilterTypeDef

```python
# CoverageStringFilterTypeDef definition

class CoverageStringFilterTypeDef(TypedDict):
    comparison: CoverageStringComparisonType,  # (1)
    value: str,
```

1. See [:material-code-brackets: CoverageStringComparisonType](./literals.md#coveragestringcomparisontype) 
## ScanStatusTypeDef

```python
# ScanStatusTypeDef definition

class ScanStatusTypeDef(TypedDict):
    reason: ScanStatusReasonType,  # (1)
    statusCode: ScanStatusCodeType,  # (2)
```

1. See [:material-code-brackets: ScanStatusReasonType](./literals.md#scanstatusreasontype) 
2. See [:material-code-brackets: ScanStatusCodeType](./literals.md#scanstatuscodetype) 
## DestinationTypeDef

```python
# DestinationTypeDef definition

class DestinationTypeDef(TypedDict):
    bucketName: str,
    kmsKeyArn: str,
    keyPrefix: NotRequired[str],
```

## Cvss2TypeDef

```python
# Cvss2TypeDef definition

class Cvss2TypeDef(TypedDict):
    baseScore: NotRequired[float],
    scoringVector: NotRequired[str],
```

## Cvss3TypeDef

```python
# Cvss3TypeDef definition

class Cvss3TypeDef(TypedDict):
    baseScore: NotRequired[float],
    scoringVector: NotRequired[str],
```

## CvssScoreAdjustmentTypeDef

```python
# CvssScoreAdjustmentTypeDef definition

class CvssScoreAdjustmentTypeDef(TypedDict):
    metric: str,
    reason: str,
```

## CvssScoreTypeDef

```python
# CvssScoreTypeDef definition

class CvssScoreTypeDef(TypedDict):
    baseScore: float,
    scoringVector: str,
    source: str,
    version: str,
```

## DelegatedAdminAccountTypeDef

```python
# DelegatedAdminAccountTypeDef definition

class DelegatedAdminAccountTypeDef(TypedDict):
    accountId: NotRequired[str],
    status: NotRequired[DelegatedAdminStatusType],  # (1)
```

1. See [:material-code-brackets: DelegatedAdminStatusType](./literals.md#delegatedadminstatustype) 
## DelegatedAdminTypeDef

```python
# DelegatedAdminTypeDef definition

class DelegatedAdminTypeDef(TypedDict):
    accountId: NotRequired[str],
    relationshipStatus: NotRequired[RelationshipStatusType],  # (1)
```

1. See [:material-code-brackets: RelationshipStatusType](./literals.md#relationshipstatustype) 
## DeleteFilterRequestRequestTypeDef

```python
# DeleteFilterRequestRequestTypeDef definition

class DeleteFilterRequestRequestTypeDef(TypedDict):
    arn: str,
```

## DisableDelegatedAdminAccountRequestRequestTypeDef

```python
# DisableDelegatedAdminAccountRequestRequestTypeDef definition

class DisableDelegatedAdminAccountRequestRequestTypeDef(TypedDict):
    delegatedAdminAccountId: str,
```

## DisableRequestRequestTypeDef

```python
# DisableRequestRequestTypeDef definition

class DisableRequestRequestTypeDef(TypedDict):
    accountIds: NotRequired[Sequence[str]],
    resourceTypes: NotRequired[Sequence[ResourceScanTypeType]],  # (1)
```

1. See [:material-code-brackets: ResourceScanTypeType](./literals.md#resourcescantypetype) 
## DisassociateMemberRequestRequestTypeDef

```python
# DisassociateMemberRequestRequestTypeDef definition

class DisassociateMemberRequestRequestTypeDef(TypedDict):
    accountId: str,
```

## MapFilterTypeDef

```python
# MapFilterTypeDef definition

class MapFilterTypeDef(TypedDict):
    comparison: MapComparisonType,  # (1)
    key: str,
    value: NotRequired[str],
```

1. See [:material-code-brackets: MapComparisonType](./literals.md#mapcomparisontype) 
## Ec2MetadataTypeDef

```python
# Ec2MetadataTypeDef definition

class Ec2MetadataTypeDef(TypedDict):
    amiId: NotRequired[str],
    platform: NotRequired[Ec2PlatformType],  # (1)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: Ec2PlatformType](./literals.md#ec2platformtype) 
## EcrRescanDurationStateTypeDef

```python
# EcrRescanDurationStateTypeDef definition

class EcrRescanDurationStateTypeDef(TypedDict):
    rescanDuration: NotRequired[EcrRescanDurationType],  # (1)
    status: NotRequired[EcrRescanDurationStatusType],  # (2)
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: EcrRescanDurationType](./literals.md#ecrrescandurationtype) 
2. See [:material-code-brackets: EcrRescanDurationStatusType](./literals.md#ecrrescandurationstatustype) 
## EcrConfigurationTypeDef

```python
# EcrConfigurationTypeDef definition

class EcrConfigurationTypeDef(TypedDict):
    rescanDuration: EcrRescanDurationType,  # (1)
```

1. See [:material-code-brackets: EcrRescanDurationType](./literals.md#ecrrescandurationtype) 
## EcrContainerImageMetadataTypeDef

```python
# EcrContainerImageMetadataTypeDef definition

class EcrContainerImageMetadataTypeDef(TypedDict):
    tags: NotRequired[List[str]],
```

## EcrRepositoryMetadataTypeDef

```python
# EcrRepositoryMetadataTypeDef definition

class EcrRepositoryMetadataTypeDef(TypedDict):
    name: NotRequired[str],
    scanFrequency: NotRequired[EcrScanFrequencyType],  # (1)
```

1. See [:material-code-brackets: EcrScanFrequencyType](./literals.md#ecrscanfrequencytype) 
## EnableDelegatedAdminAccountRequestRequestTypeDef

```python
# EnableDelegatedAdminAccountRequestRequestTypeDef definition

class EnableDelegatedAdminAccountRequestRequestTypeDef(TypedDict):
    delegatedAdminAccountId: str,
    clientToken: NotRequired[str],
```

## EnableRequestRequestTypeDef

```python
# EnableRequestRequestTypeDef definition

class EnableRequestRequestTypeDef(TypedDict):
    resourceTypes: Sequence[ResourceScanTypeType],  # (1)
    accountIds: NotRequired[Sequence[str]],
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: ResourceScanTypeType](./literals.md#resourcescantypetype) 
## EpssDetailsTypeDef

```python
# EpssDetailsTypeDef definition

class EpssDetailsTypeDef(TypedDict):
    score: NotRequired[float],
```

## EpssTypeDef

```python
# EpssTypeDef definition

class EpssTypeDef(TypedDict):
    score: NotRequired[float],
```

## EvidenceTypeDef

```python
# EvidenceTypeDef definition

class EvidenceTypeDef(TypedDict):
    evidenceDetail: NotRequired[str],
    evidenceRule: NotRequired[str],
    severity: NotRequired[str],
```

## ExploitObservedTypeDef

```python
# ExploitObservedTypeDef definition

class ExploitObservedTypeDef(TypedDict):
    firstSeen: NotRequired[datetime],
    lastSeen: NotRequired[datetime],
```

## ExploitabilityDetailsTypeDef

```python
# ExploitabilityDetailsTypeDef definition

class ExploitabilityDetailsTypeDef(TypedDict):
    lastKnownExploitAt: NotRequired[datetime],
```

## NumberFilterTypeDef

```python
# NumberFilterTypeDef definition

class NumberFilterTypeDef(TypedDict):
    lowerInclusive: NotRequired[float],
    upperInclusive: NotRequired[float],
```

## PortRangeFilterTypeDef

```python
# PortRangeFilterTypeDef definition

class PortRangeFilterTypeDef(TypedDict):
    beginInclusive: NotRequired[int],
    endInclusive: NotRequired[int],
```

## FreeTrialInfoTypeDef

```python
# FreeTrialInfoTypeDef definition

class FreeTrialInfoTypeDef(TypedDict):
    end: datetime,
    start: datetime,
    status: FreeTrialStatusType,  # (1)
    type: FreeTrialTypeType,  # (2)
```

1. See [:material-code-brackets: FreeTrialStatusType](./literals.md#freetrialstatustype) 
2. See [:material-code-brackets: FreeTrialTypeType](./literals.md#freetrialtypetype) 
## GetEncryptionKeyRequestRequestTypeDef

```python
# GetEncryptionKeyRequestRequestTypeDef definition

class GetEncryptionKeyRequestRequestTypeDef(TypedDict):
    resourceType: ResourceTypeType,  # (1)
    scanType: ScanTypeType,  # (2)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: ScanTypeType](./literals.md#scantypetype) 
## GetFindingsReportStatusRequestRequestTypeDef

```python
# GetFindingsReportStatusRequestRequestTypeDef definition

class GetFindingsReportStatusRequestRequestTypeDef(TypedDict):
    reportId: NotRequired[str],
```

## GetMemberRequestRequestTypeDef

```python
# GetMemberRequestRequestTypeDef definition

class GetMemberRequestRequestTypeDef(TypedDict):
    accountId: str,
```

## MemberTypeDef

```python
# MemberTypeDef definition

class MemberTypeDef(TypedDict):
    accountId: NotRequired[str],
    delegatedAdminAccountId: NotRequired[str],
    relationshipStatus: NotRequired[RelationshipStatusType],  # (1)
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: RelationshipStatusType](./literals.md#relationshipstatustype) 
## GetSbomExportRequestRequestTypeDef

```python
# GetSbomExportRequestRequestTypeDef definition

class GetSbomExportRequestRequestTypeDef(TypedDict):
    reportId: str,
```

## LambdaFunctionMetadataTypeDef

```python
# LambdaFunctionMetadataTypeDef definition

class LambdaFunctionMetadataTypeDef(TypedDict):
    functionName: NotRequired[str],
    functionTags: NotRequired[Dict[str, str]],
    layers: NotRequired[List[str]],
    runtime: NotRequired[RuntimeType],  # (1)
```

1. See [:material-code-brackets: RuntimeType](./literals.md#runtimetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAccountPermissionsRequestRequestTypeDef

```python
# ListAccountPermissionsRequestRequestTypeDef definition

class ListAccountPermissionsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    service: NotRequired[ServiceType],  # (1)
```

1. See [:material-code-brackets: ServiceType](./literals.md#servicetype) 
## PermissionTypeDef

```python
# PermissionTypeDef definition

class PermissionTypeDef(TypedDict):
    operation: OperationType,  # (1)
    service: ServiceType,  # (2)
```

1. See [:material-code-brackets: OperationType](./literals.md#operationtype) 
2. See [:material-code-brackets: ServiceType](./literals.md#servicetype) 
## ListDelegatedAdminAccountsRequestRequestTypeDef

```python
# ListDelegatedAdminAccountsRequestRequestTypeDef definition

class ListDelegatedAdminAccountsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListFiltersRequestRequestTypeDef

```python
# ListFiltersRequestRequestTypeDef definition

class ListFiltersRequestRequestTypeDef(TypedDict):
    action: NotRequired[FilterActionType],  # (1)
    arns: NotRequired[Sequence[str]],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: FilterActionType](./literals.md#filteractiontype) 
## SortCriteriaTypeDef

```python
# SortCriteriaTypeDef definition

class SortCriteriaTypeDef(TypedDict):
    field: SortFieldType,  # (1)
    sortOrder: SortOrderType,  # (2)
```

1. See [:material-code-brackets: SortFieldType](./literals.md#sortfieldtype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListMembersRequestRequestTypeDef

```python
# ListMembersRequestRequestTypeDef definition

class ListMembersRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    onlyAssociated: NotRequired[bool],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListUsageTotalsRequestRequestTypeDef

```python
# ListUsageTotalsRequestRequestTypeDef definition

class ListUsageTotalsRequestRequestTypeDef(TypedDict):
    accountIds: NotRequired[Sequence[str]],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## StepTypeDef

```python
# StepTypeDef definition

class StepTypeDef(TypedDict):
    componentId: str,
    componentType: str,
```

## PortRangeTypeDef

```python
# PortRangeTypeDef definition

class PortRangeTypeDef(TypedDict):
    begin: int,
    end: int,
```

## VulnerablePackageTypeDef

```python
# VulnerablePackageTypeDef definition

class VulnerablePackageTypeDef(TypedDict):
    name: str,
    version: str,
    arch: NotRequired[str],
    epoch: NotRequired[int],
    filePath: NotRequired[str],
    fixedInVersion: NotRequired[str],
    packageManager: NotRequired[PackageManagerType],  # (1)
    release: NotRequired[str],
    remediation: NotRequired[str],
    sourceLambdaLayerArn: NotRequired[str],
    sourceLayerHash: NotRequired[str],
```

1. See [:material-code-brackets: PackageManagerType](./literals.md#packagemanagertype) 
## RecommendationTypeDef

```python
# RecommendationTypeDef definition

class RecommendationTypeDef(TypedDict):
    Url: NotRequired[str],
    text: NotRequired[str],
```

## ResetEncryptionKeyRequestRequestTypeDef

```python
# ResetEncryptionKeyRequestRequestTypeDef definition

class ResetEncryptionKeyRequestRequestTypeDef(TypedDict):
    resourceType: ResourceTypeType,  # (1)
    scanType: ScanTypeType,  # (2)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: ScanTypeType](./literals.md#scantypetype) 
## ResourceMapFilterTypeDef

```python
# ResourceMapFilterTypeDef definition

class ResourceMapFilterTypeDef(TypedDict):
    comparison: ResourceMapComparisonType,  # (1)
    key: str,
    value: NotRequired[str],
```

1. See [:material-code-brackets: ResourceMapComparisonType](./literals.md#resourcemapcomparisontype) 
## ResourceStringFilterTypeDef

```python
# ResourceStringFilterTypeDef definition

class ResourceStringFilterTypeDef(TypedDict):
    comparison: ResourceStringComparisonType,  # (1)
    value: str,
```

1. See [:material-code-brackets: ResourceStringComparisonType](./literals.md#resourcestringcomparisontype) 
## SearchVulnerabilitiesFilterCriteriaTypeDef

```python
# SearchVulnerabilitiesFilterCriteriaTypeDef definition

class SearchVulnerabilitiesFilterCriteriaTypeDef(TypedDict):
    vulnerabilityIds: Sequence[str],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateEc2DeepInspectionConfigurationRequestRequestTypeDef

```python
# UpdateEc2DeepInspectionConfigurationRequestRequestTypeDef definition

class UpdateEc2DeepInspectionConfigurationRequestRequestTypeDef(TypedDict):
    activateDeepInspection: NotRequired[bool],
    packagePaths: NotRequired[Sequence[str]],
```

## UpdateEncryptionKeyRequestRequestTypeDef

```python
# UpdateEncryptionKeyRequestRequestTypeDef definition

class UpdateEncryptionKeyRequestRequestTypeDef(TypedDict):
    kmsKeyId: str,
    resourceType: ResourceTypeType,  # (1)
    scanType: ScanTypeType,  # (2)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: ScanTypeType](./literals.md#scantypetype) 
## UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef

```python
# UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef definition

class UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef(TypedDict):
    orgPackagePaths: Sequence[str],
```

## UsageTypeDef

```python
# UsageTypeDef definition

class UsageTypeDef(TypedDict):
    currency: NotRequired[CurrencyType],  # (1)
    estimatedMonthlyCost: NotRequired[float],
    total: NotRequired[float],
    type: NotRequired[UsageTypeType],  # (2)
```

1. See [:material-code-brackets: CurrencyType](./literals.md#currencytype) 
2. See [:material-code-brackets: UsageTypeType](./literals.md#usagetypetype) 
## AccountAggregationResponseTypeDef

```python
# AccountAggregationResponseTypeDef definition

class AccountAggregationResponseTypeDef(TypedDict):
    accountId: NotRequired[str],
    severityCounts: NotRequired[SeverityCountsTypeDef],  # (1)
```

1. See [:material-code-braces: SeverityCountsTypeDef](./type_defs.md#severitycountstypedef) 
## AmiAggregationResponseTypeDef

```python
# AmiAggregationResponseTypeDef definition

class AmiAggregationResponseTypeDef(TypedDict):
    ami: str,
    accountId: NotRequired[str],
    affectedInstances: NotRequired[int],
    severityCounts: NotRequired[SeverityCountsTypeDef],  # (1)
```

1. See [:material-code-braces: SeverityCountsTypeDef](./type_defs.md#severitycountstypedef) 
## AwsEcrContainerAggregationResponseTypeDef

```python
# AwsEcrContainerAggregationResponseTypeDef definition

class AwsEcrContainerAggregationResponseTypeDef(TypedDict):
    resourceId: str,
    accountId: NotRequired[str],
    architecture: NotRequired[str],
    imageSha: NotRequired[str],
    imageTags: NotRequired[List[str]],
    repository: NotRequired[str],
    severityCounts: NotRequired[SeverityCountsTypeDef],  # (1)
```

1. See [:material-code-braces: SeverityCountsTypeDef](./type_defs.md#severitycountstypedef) 
## Ec2InstanceAggregationResponseTypeDef

```python
# Ec2InstanceAggregationResponseTypeDef definition

class Ec2InstanceAggregationResponseTypeDef(TypedDict):
    instanceId: str,
    accountId: NotRequired[str],
    ami: NotRequired[str],
    instanceTags: NotRequired[Dict[str, str]],
    networkFindings: NotRequired[int],
    operatingSystem: NotRequired[str],
    severityCounts: NotRequired[SeverityCountsTypeDef],  # (1)
```

1. See [:material-code-braces: SeverityCountsTypeDef](./type_defs.md#severitycountstypedef) 
## FindingTypeAggregationResponseTypeDef

```python
# FindingTypeAggregationResponseTypeDef definition

class FindingTypeAggregationResponseTypeDef(TypedDict):
    accountId: NotRequired[str],
    severityCounts: NotRequired[SeverityCountsTypeDef],  # (1)
```

1. See [:material-code-braces: SeverityCountsTypeDef](./type_defs.md#severitycountstypedef) 
## ImageLayerAggregationResponseTypeDef

```python
# ImageLayerAggregationResponseTypeDef definition

class ImageLayerAggregationResponseTypeDef(TypedDict):
    accountId: str,
    layerHash: str,
    repository: str,
    resourceId: str,
    severityCounts: NotRequired[SeverityCountsTypeDef],  # (1)
```

1. See [:material-code-braces: SeverityCountsTypeDef](./type_defs.md#severitycountstypedef) 
## LambdaFunctionAggregationResponseTypeDef

```python
# LambdaFunctionAggregationResponseTypeDef definition

class LambdaFunctionAggregationResponseTypeDef(TypedDict):
    resourceId: str,
    accountId: NotRequired[str],
    functionName: NotRequired[str],
    lambdaTags: NotRequired[Dict[str, str]],
    lastModifiedAt: NotRequired[datetime],
    runtime: NotRequired[str],
    severityCounts: NotRequired[SeverityCountsTypeDef],  # (1)
```

1. See [:material-code-braces: SeverityCountsTypeDef](./type_defs.md#severitycountstypedef) 
## LambdaLayerAggregationResponseTypeDef

```python
# LambdaLayerAggregationResponseTypeDef definition

class LambdaLayerAggregationResponseTypeDef(TypedDict):
    accountId: str,
    functionName: str,
    layerArn: str,
    resourceId: str,
    severityCounts: NotRequired[SeverityCountsTypeDef],  # (1)
```

1. See [:material-code-braces: SeverityCountsTypeDef](./type_defs.md#severitycountstypedef) 
## PackageAggregationResponseTypeDef

```python
# PackageAggregationResponseTypeDef definition

class PackageAggregationResponseTypeDef(TypedDict):
    packageName: str,
    accountId: NotRequired[str],
    severityCounts: NotRequired[SeverityCountsTypeDef],  # (1)
```

1. See [:material-code-braces: SeverityCountsTypeDef](./type_defs.md#severitycountstypedef) 
## RepositoryAggregationResponseTypeDef

```python
# RepositoryAggregationResponseTypeDef definition

class RepositoryAggregationResponseTypeDef(TypedDict):
    repository: str,
    accountId: NotRequired[str],
    affectedImages: NotRequired[int],
    severityCounts: NotRequired[SeverityCountsTypeDef],  # (1)
```

1. See [:material-code-braces: SeverityCountsTypeDef](./type_defs.md#severitycountstypedef) 
## TitleAggregationResponseTypeDef

```python
# TitleAggregationResponseTypeDef definition

class TitleAggregationResponseTypeDef(TypedDict):
    title: str,
    accountId: NotRequired[str],
    severityCounts: NotRequired[SeverityCountsTypeDef],  # (1)
    vulnerabilityId: NotRequired[str],
```

1. See [:material-code-braces: SeverityCountsTypeDef](./type_defs.md#severitycountstypedef) 
## ResourceStateTypeDef

```python
# ResourceStateTypeDef definition

class ResourceStateTypeDef(TypedDict):
    ec2: StateTypeDef,  # (1)
    ecr: StateTypeDef,  # (1)
    lambda: NotRequired[StateTypeDef],  # (1)
    lambdaCode: NotRequired[StateTypeDef],  # (1)
```

1. See [:material-code-braces: StateTypeDef](./type_defs.md#statetypedef) 
2. See [:material-code-braces: StateTypeDef](./type_defs.md#statetypedef) 
3. See [:material-code-braces: StateTypeDef](./type_defs.md#statetypedef) 
4. See [:material-code-braces: StateTypeDef](./type_defs.md#statetypedef) 
## AccountTypeDef

```python
# AccountTypeDef definition

class AccountTypeDef(TypedDict):
    accountId: str,
    resourceStatus: ResourceStatusTypeDef,  # (1)
    status: StatusType,  # (2)
```

1. See [:material-code-braces: ResourceStatusTypeDef](./type_defs.md#resourcestatustypedef) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## FailedAccountTypeDef

```python
# FailedAccountTypeDef definition

class FailedAccountTypeDef(TypedDict):
    accountId: str,
    errorCode: ErrorCodeType,  # (1)
    errorMessage: str,
    resourceStatus: NotRequired[ResourceStatusTypeDef],  # (2)
    status: NotRequired[StatusType],  # (3)
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
2. See [:material-code-braces: ResourceStatusTypeDef](./type_defs.md#resourcestatustypedef) 
3. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## AmiAggregationTypeDef

```python
# AmiAggregationTypeDef definition

class AmiAggregationTypeDef(TypedDict):
    amis: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    sortBy: NotRequired[AmiSortByType],  # (2)
    sortOrder: NotRequired[SortOrderType],  # (3)
```

1. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
2. See [:material-code-brackets: AmiSortByType](./literals.md#amisortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## AwsEcrContainerAggregationTypeDef

```python
# AwsEcrContainerAggregationTypeDef definition

class AwsEcrContainerAggregationTypeDef(TypedDict):
    architectures: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    imageShas: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    imageTags: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    repositories: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    resourceIds: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    sortBy: NotRequired[AwsEcrContainerSortByType],  # (6)
    sortOrder: NotRequired[SortOrderType],  # (7)
```

1. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
2. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
3. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
4. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
5. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
6. See [:material-code-brackets: AwsEcrContainerSortByType](./literals.md#awsecrcontainersortbytype) 
7. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ImageLayerAggregationTypeDef

```python
# ImageLayerAggregationTypeDef definition

class ImageLayerAggregationTypeDef(TypedDict):
    layerHashes: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    repositories: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    resourceIds: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    sortBy: NotRequired[ImageLayerSortByType],  # (4)
    sortOrder: NotRequired[SortOrderType],  # (5)
```

1. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
2. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
3. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
4. See [:material-code-brackets: ImageLayerSortByType](./literals.md#imagelayersortbytype) 
5. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## LambdaLayerAggregationTypeDef

```python
# LambdaLayerAggregationTypeDef definition

class LambdaLayerAggregationTypeDef(TypedDict):
    functionNames: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    layerArns: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    resourceIds: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    sortBy: NotRequired[LambdaLayerSortByType],  # (4)
    sortOrder: NotRequired[SortOrderType],  # (5)
```

1. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
2. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
3. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
4. See [:material-code-brackets: LambdaLayerSortByType](./literals.md#lambdalayersortbytype) 
5. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## PackageAggregationTypeDef

```python
# PackageAggregationTypeDef definition

class PackageAggregationTypeDef(TypedDict):
    packageNames: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    sortBy: NotRequired[PackageSortByType],  # (2)
    sortOrder: NotRequired[SortOrderType],  # (3)
```

1. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
2. See [:material-code-brackets: PackageSortByType](./literals.md#packagesortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## RepositoryAggregationTypeDef

```python
# RepositoryAggregationTypeDef definition

class RepositoryAggregationTypeDef(TypedDict):
    repositories: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    sortBy: NotRequired[RepositorySortByType],  # (2)
    sortOrder: NotRequired[SortOrderType],  # (3)
```

1. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
2. See [:material-code-brackets: RepositorySortByType](./literals.md#repositorysortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## TitleAggregationTypeDef

```python
# TitleAggregationTypeDef definition

class TitleAggregationTypeDef(TypedDict):
    findingType: NotRequired[AggregationFindingTypeType],  # (1)
    resourceType: NotRequired[AggregationResourceTypeType],  # (2)
    sortBy: NotRequired[TitleSortByType],  # (3)
    sortOrder: NotRequired[SortOrderType],  # (4)
    titles: NotRequired[Sequence[StringFilterTypeDef]],  # (5)
    vulnerabilityIds: NotRequired[Sequence[StringFilterTypeDef]],  # (5)
```

1. See [:material-code-brackets: AggregationFindingTypeType](./literals.md#aggregationfindingtypetype) 
2. See [:material-code-brackets: AggregationResourceTypeType](./literals.md#aggregationresourcetypetype) 
3. See [:material-code-brackets: TitleSortByType](./literals.md#titlesortbytype) 
4. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
5. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
6. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
## AssociateMemberResponseTypeDef

```python
# AssociateMemberResponseTypeDef definition

class AssociateMemberResponseTypeDef(TypedDict):
    accountId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CancelFindingsReportResponseTypeDef

```python
# CancelFindingsReportResponseTypeDef definition

class CancelFindingsReportResponseTypeDef(TypedDict):
    reportId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CancelSbomExportResponseTypeDef

```python
# CancelSbomExportResponseTypeDef definition

class CancelSbomExportResponseTypeDef(TypedDict):
    reportId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFilterResponseTypeDef

```python
# CreateFilterResponseTypeDef definition

class CreateFilterResponseTypeDef(TypedDict):
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFindingsReportResponseTypeDef

```python
# CreateFindingsReportResponseTypeDef definition

class CreateFindingsReportResponseTypeDef(TypedDict):
    reportId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSbomExportResponseTypeDef

```python
# CreateSbomExportResponseTypeDef definition

class CreateSbomExportResponseTypeDef(TypedDict):
    reportId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteFilterResponseTypeDef

```python
# DeleteFilterResponseTypeDef definition

class DeleteFilterResponseTypeDef(TypedDict):
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisableDelegatedAdminAccountResponseTypeDef

```python
# DisableDelegatedAdminAccountResponseTypeDef definition

class DisableDelegatedAdminAccountResponseTypeDef(TypedDict):
    delegatedAdminAccountId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateMemberResponseTypeDef

```python
# DisassociateMemberResponseTypeDef definition

class DisassociateMemberResponseTypeDef(TypedDict):
    accountId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnableDelegatedAdminAccountResponseTypeDef

```python
# EnableDelegatedAdminAccountResponseTypeDef definition

class EnableDelegatedAdminAccountResponseTypeDef(TypedDict):
    delegatedAdminAccountId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEc2DeepInspectionConfigurationResponseTypeDef

```python
# GetEc2DeepInspectionConfigurationResponseTypeDef definition

class GetEc2DeepInspectionConfigurationResponseTypeDef(TypedDict):
    errorMessage: str,
    orgPackagePaths: List[str],
    packagePaths: List[str],
    status: Ec2DeepInspectionStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: Ec2DeepInspectionStatusType](./literals.md#ec2deepinspectionstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEncryptionKeyResponseTypeDef

```python
# GetEncryptionKeyResponseTypeDef definition

class GetEncryptionKeyResponseTypeDef(TypedDict):
    kmsKeyId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEc2DeepInspectionConfigurationResponseTypeDef

```python
# UpdateEc2DeepInspectionConfigurationResponseTypeDef definition

class UpdateEc2DeepInspectionConfigurationResponseTypeDef(TypedDict):
    errorMessage: str,
    orgPackagePaths: List[str],
    packagePaths: List[str],
    status: Ec2DeepInspectionStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: Ec2DeepInspectionStatusType](./literals.md#ec2deepinspectionstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFilterResponseTypeDef

```python
# UpdateFilterResponseTypeDef definition

class UpdateFilterResponseTypeDef(TypedDict):
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeOrganizationConfigurationResponseTypeDef

```python
# DescribeOrganizationConfigurationResponseTypeDef definition

class DescribeOrganizationConfigurationResponseTypeDef(TypedDict):
    autoEnable: AutoEnableTypeDef,  # (1)
    maxAccountLimitReached: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AutoEnableTypeDef](./type_defs.md#autoenabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateOrganizationConfigurationRequestRequestTypeDef

```python
# UpdateOrganizationConfigurationRequestRequestTypeDef definition

class UpdateOrganizationConfigurationRequestRequestTypeDef(TypedDict):
    autoEnable: AutoEnableTypeDef,  # (1)
```

1. See [:material-code-braces: AutoEnableTypeDef](./type_defs.md#autoenabletypedef) 
## UpdateOrganizationConfigurationResponseTypeDef

```python
# UpdateOrganizationConfigurationResponseTypeDef definition

class UpdateOrganizationConfigurationResponseTypeDef(TypedDict):
    autoEnable: AutoEnableTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AutoEnableTypeDef](./type_defs.md#autoenabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AwsLambdaFunctionDetailsTypeDef

```python
# AwsLambdaFunctionDetailsTypeDef definition

class AwsLambdaFunctionDetailsTypeDef(TypedDict):
    codeSha256: str,
    executionRoleArn: str,
    functionName: str,
    runtime: RuntimeType,  # (3)
    version: str,
    architectures: NotRequired[List[ArchitectureType]],  # (1)
    lastModifiedAt: NotRequired[datetime],
    layers: NotRequired[List[str]],
    packageType: NotRequired[PackageTypeType],  # (2)
    vpcConfig: NotRequired[LambdaVpcConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: ArchitectureType](./literals.md#architecturetype) 
2. See [:material-code-brackets: PackageTypeType](./literals.md#packagetypetype) 
3. See [:material-code-brackets: RuntimeType](./literals.md#runtimetype) 
4. See [:material-code-braces: LambdaVpcConfigTypeDef](./type_defs.md#lambdavpcconfigtypedef) 
## BatchGetMemberEc2DeepInspectionStatusResponseTypeDef

```python
# BatchGetMemberEc2DeepInspectionStatusResponseTypeDef definition

class BatchGetMemberEc2DeepInspectionStatusResponseTypeDef(TypedDict):
    accountIds: List[MemberAccountEc2DeepInspectionStatusStateTypeDef],  # (1)
    failedAccountIds: List[FailedMemberAccountEc2DeepInspectionStatusStateTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: MemberAccountEc2DeepInspectionStatusStateTypeDef](./type_defs.md#memberaccountec2deepinspectionstatusstatetypedef) 
2. See [:material-code-braces: FailedMemberAccountEc2DeepInspectionStatusStateTypeDef](./type_defs.md#failedmemberaccountec2deepinspectionstatusstatetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef

```python
# BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef definition

class BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef(TypedDict):
    accountIds: List[MemberAccountEc2DeepInspectionStatusStateTypeDef],  # (1)
    failedAccountIds: List[FailedMemberAccountEc2DeepInspectionStatusStateTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: MemberAccountEc2DeepInspectionStatusStateTypeDef](./type_defs.md#memberaccountec2deepinspectionstatusstatetypedef) 
2. See [:material-code-braces: FailedMemberAccountEc2DeepInspectionStatusStateTypeDef](./type_defs.md#failedmemberaccountec2deepinspectionstatusstatetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef

```python
# BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef definition

class BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef(TypedDict):
    accountIds: Sequence[MemberAccountEc2DeepInspectionStatusTypeDef],  # (1)
```

1. See [:material-code-braces: MemberAccountEc2DeepInspectionStatusTypeDef](./type_defs.md#memberaccountec2deepinspectionstatustypedef) 
## CodeVulnerabilityDetailsTypeDef

```python
# CodeVulnerabilityDetailsTypeDef definition

class CodeVulnerabilityDetailsTypeDef(TypedDict):
    cwes: List[str],
    detectorId: str,
    detectorName: str,
    filePath: CodeFilePathTypeDef,  # (1)
    detectorTags: NotRequired[List[str]],
    referenceUrls: NotRequired[List[str]],
    ruleId: NotRequired[str],
    sourceLambdaLayerArn: NotRequired[str],
```

1. See [:material-code-braces: CodeFilePathTypeDef](./type_defs.md#codefilepathtypedef) 
## CodeSnippetResultTypeDef

```python
# CodeSnippetResultTypeDef definition

class CodeSnippetResultTypeDef(TypedDict):
    codeSnippet: NotRequired[List[CodeLineTypeDef]],  # (1)
    endLine: NotRequired[int],
    findingArn: NotRequired[str],
    startLine: NotRequired[int],
    suggestedFixes: NotRequired[List[SuggestedFixTypeDef]],  # (2)
```

1. See [:material-code-braces: CodeLineTypeDef](./type_defs.md#codelinetypedef) 
2. See [:material-code-braces: SuggestedFixTypeDef](./type_defs.md#suggestedfixtypedef) 
## ListCoverageStatisticsResponseTypeDef

```python
# ListCoverageStatisticsResponseTypeDef definition

class ListCoverageStatisticsResponseTypeDef(TypedDict):
    countsByGroup: List[CountsTypeDef],  # (1)
    nextToken: str,
    totalCounts: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CountsTypeDef](./type_defs.md#countstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CoverageDateFilterTypeDef

```python
# CoverageDateFilterTypeDef definition

class CoverageDateFilterTypeDef(TypedDict):
    endInclusive: NotRequired[Union[datetime, str]],
    startInclusive: NotRequired[Union[datetime, str]],
```

## DateFilterTypeDef

```python
# DateFilterTypeDef definition

class DateFilterTypeDef(TypedDict):
    endInclusive: NotRequired[Union[datetime, str]],
    startInclusive: NotRequired[Union[datetime, str]],
```

## CvssScoreDetailsTypeDef

```python
# CvssScoreDetailsTypeDef definition

class CvssScoreDetailsTypeDef(TypedDict):
    score: float,
    scoreSource: str,
    scoringVector: str,
    version: str,
    adjustments: NotRequired[List[CvssScoreAdjustmentTypeDef]],  # (1)
    cvssSource: NotRequired[str],
```

1. See [:material-code-braces: CvssScoreAdjustmentTypeDef](./type_defs.md#cvssscoreadjustmenttypedef) 
## ListDelegatedAdminAccountsResponseTypeDef

```python
# ListDelegatedAdminAccountsResponseTypeDef definition

class ListDelegatedAdminAccountsResponseTypeDef(TypedDict):
    delegatedAdminAccounts: List[DelegatedAdminAccountTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DelegatedAdminAccountTypeDef](./type_defs.md#delegatedadminaccounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDelegatedAdminAccountResponseTypeDef

```python
# GetDelegatedAdminAccountResponseTypeDef definition

class GetDelegatedAdminAccountResponseTypeDef(TypedDict):
    delegatedAdmin: DelegatedAdminTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DelegatedAdminTypeDef](./type_defs.md#delegatedadmintypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## Ec2InstanceAggregationTypeDef

```python
# Ec2InstanceAggregationTypeDef definition

class Ec2InstanceAggregationTypeDef(TypedDict):
    amis: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    instanceIds: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    instanceTags: NotRequired[Sequence[MapFilterTypeDef]],  # (3)
    operatingSystems: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    sortBy: NotRequired[Ec2InstanceSortByType],  # (5)
    sortOrder: NotRequired[SortOrderType],  # (6)
```

1. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
2. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
3. See [:material-code-braces: MapFilterTypeDef](./type_defs.md#mapfiltertypedef) 
4. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
5. See [:material-code-brackets: Ec2InstanceSortByType](./literals.md#ec2instancesortbytype) 
6. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## LambdaFunctionAggregationTypeDef

```python
# LambdaFunctionAggregationTypeDef definition

class LambdaFunctionAggregationTypeDef(TypedDict):
    functionNames: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    functionTags: NotRequired[Sequence[MapFilterTypeDef]],  # (2)
    resourceIds: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    runtimes: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    sortBy: NotRequired[LambdaFunctionSortByType],  # (5)
    sortOrder: NotRequired[SortOrderType],  # (6)
```

1. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
2. See [:material-code-braces: MapFilterTypeDef](./type_defs.md#mapfiltertypedef) 
3. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
4. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
5. See [:material-code-brackets: LambdaFunctionSortByType](./literals.md#lambdafunctionsortbytype) 
6. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## EcrConfigurationStateTypeDef

```python
# EcrConfigurationStateTypeDef definition

class EcrConfigurationStateTypeDef(TypedDict):
    rescanDurationState: NotRequired[EcrRescanDurationStateTypeDef],  # (1)
```

1. See [:material-code-braces: EcrRescanDurationStateTypeDef](./type_defs.md#ecrrescandurationstatetypedef) 
## UpdateConfigurationRequestRequestTypeDef

```python
# UpdateConfigurationRequestRequestTypeDef definition

class UpdateConfigurationRequestRequestTypeDef(TypedDict):
    ecrConfiguration: EcrConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: EcrConfigurationTypeDef](./type_defs.md#ecrconfigurationtypedef) 
## FindingDetailTypeDef

```python
# FindingDetailTypeDef definition

class FindingDetailTypeDef(TypedDict):
    cisaData: NotRequired[CisaDataTypeDef],  # (1)
    cwes: NotRequired[List[str]],
    epssScore: NotRequired[float],
    evidences: NotRequired[List[EvidenceTypeDef]],  # (2)
    exploitObserved: NotRequired[ExploitObservedTypeDef],  # (3)
    findingArn: NotRequired[str],
    referenceUrls: NotRequired[List[str]],
    riskScore: NotRequired[int],
    tools: NotRequired[List[str]],
    ttps: NotRequired[List[str]],
```

1. See [:material-code-braces: CisaDataTypeDef](./type_defs.md#cisadatatypedef) 
2. See [:material-code-braces: EvidenceTypeDef](./type_defs.md#evidencetypedef) 
3. See [:material-code-braces: ExploitObservedTypeDef](./type_defs.md#exploitobservedtypedef) 
## VulnerabilityTypeDef

```python
# VulnerabilityTypeDef definition

class VulnerabilityTypeDef(TypedDict):
    id: str,
    atigData: NotRequired[AtigDataTypeDef],  # (1)
    cisaData: NotRequired[CisaDataTypeDef],  # (2)
    cvss2: NotRequired[Cvss2TypeDef],  # (3)
    cvss3: NotRequired[Cvss3TypeDef],  # (4)
    cwes: NotRequired[List[str]],
    description: NotRequired[str],
    detectionPlatforms: NotRequired[List[str]],
    epss: NotRequired[EpssTypeDef],  # (5)
    exploitObserved: NotRequired[ExploitObservedTypeDef],  # (6)
    referenceUrls: NotRequired[List[str]],
    relatedVulnerabilities: NotRequired[List[str]],
    source: NotRequired[VulnerabilitySourceType],  # (7)
    sourceUrl: NotRequired[str],
    vendorCreatedAt: NotRequired[datetime],
    vendorSeverity: NotRequired[str],
    vendorUpdatedAt: NotRequired[datetime],
```

1. See [:material-code-braces: AtigDataTypeDef](./type_defs.md#atigdatatypedef) 
2. See [:material-code-braces: CisaDataTypeDef](./type_defs.md#cisadatatypedef) 
3. See [:material-code-braces: Cvss2TypeDef](./type_defs.md#cvss2typedef) 
4. See [:material-code-braces: Cvss3TypeDef](./type_defs.md#cvss3typedef) 
5. See [:material-code-braces: EpssTypeDef](./type_defs.md#epsstypedef) 
6. See [:material-code-braces: ExploitObservedTypeDef](./type_defs.md#exploitobservedtypedef) 
7. See [:material-code-brackets: VulnerabilitySourceType](./literals.md#vulnerabilitysourcetype) 
## PackageFilterTypeDef

```python
# PackageFilterTypeDef definition

class PackageFilterTypeDef(TypedDict):
    architecture: NotRequired[StringFilterTypeDef],  # (1)
    epoch: NotRequired[NumberFilterTypeDef],  # (2)
    name: NotRequired[StringFilterTypeDef],  # (1)
    release: NotRequired[StringFilterTypeDef],  # (1)
    sourceLambdaLayerArn: NotRequired[StringFilterTypeDef],  # (1)
    sourceLayerHash: NotRequired[StringFilterTypeDef],  # (1)
    version: NotRequired[StringFilterTypeDef],  # (1)
```

1. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
2. See [:material-code-braces: NumberFilterTypeDef](./type_defs.md#numberfiltertypedef) 
3. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
4. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
5. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
6. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
7. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
## FreeTrialAccountInfoTypeDef

```python
# FreeTrialAccountInfoTypeDef definition

class FreeTrialAccountInfoTypeDef(TypedDict):
    accountId: str,
    freeTrialInfo: List[FreeTrialInfoTypeDef],  # (1)
```

1. See [:material-code-braces: FreeTrialInfoTypeDef](./type_defs.md#freetrialinfotypedef) 
## GetMemberResponseTypeDef

```python
# GetMemberResponseTypeDef definition

class GetMemberResponseTypeDef(TypedDict):
    member: MemberTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MemberTypeDef](./type_defs.md#membertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMembersResponseTypeDef

```python
# ListMembersResponseTypeDef definition

class ListMembersResponseTypeDef(TypedDict):
    members: List[MemberTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MemberTypeDef](./type_defs.md#membertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResourceScanMetadataTypeDef

```python
# ResourceScanMetadataTypeDef definition

class ResourceScanMetadataTypeDef(TypedDict):
    ec2: NotRequired[Ec2MetadataTypeDef],  # (1)
    ecrImage: NotRequired[EcrContainerImageMetadataTypeDef],  # (2)
    ecrRepository: NotRequired[EcrRepositoryMetadataTypeDef],  # (3)
    lambdaFunction: NotRequired[LambdaFunctionMetadataTypeDef],  # (4)
```

1. See [:material-code-braces: Ec2MetadataTypeDef](./type_defs.md#ec2metadatatypedef) 
2. See [:material-code-braces: EcrContainerImageMetadataTypeDef](./type_defs.md#ecrcontainerimagemetadatatypedef) 
3. See [:material-code-braces: EcrRepositoryMetadataTypeDef](./type_defs.md#ecrrepositorymetadatatypedef) 
4. See [:material-code-braces: LambdaFunctionMetadataTypeDef](./type_defs.md#lambdafunctionmetadatatypedef) 
## ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef

```python
# ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef definition

class ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef(TypedDict):
    service: NotRequired[ServiceType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ServiceType](./literals.md#servicetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef

```python
# ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef definition

class ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFiltersRequestListFiltersPaginateTypeDef

```python
# ListFiltersRequestListFiltersPaginateTypeDef definition

class ListFiltersRequestListFiltersPaginateTypeDef(TypedDict):
    action: NotRequired[FilterActionType],  # (1)
    arns: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: FilterActionType](./literals.md#filteractiontype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMembersRequestListMembersPaginateTypeDef

```python
# ListMembersRequestListMembersPaginateTypeDef definition

class ListMembersRequestListMembersPaginateTypeDef(TypedDict):
    onlyAssociated: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUsageTotalsRequestListUsageTotalsPaginateTypeDef

```python
# ListUsageTotalsRequestListUsageTotalsPaginateTypeDef definition

class ListUsageTotalsRequestListUsageTotalsPaginateTypeDef(TypedDict):
    accountIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAccountPermissionsResponseTypeDef

```python
# ListAccountPermissionsResponseTypeDef definition

class ListAccountPermissionsResponseTypeDef(TypedDict):
    nextToken: str,
    permissions: List[PermissionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PermissionTypeDef](./type_defs.md#permissiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NetworkPathTypeDef

```python
# NetworkPathTypeDef definition

class NetworkPathTypeDef(TypedDict):
    steps: NotRequired[List[StepTypeDef]],  # (1)
```

1. See [:material-code-braces: StepTypeDef](./type_defs.md#steptypedef) 
## PackageVulnerabilityDetailsTypeDef

```python
# PackageVulnerabilityDetailsTypeDef definition

class PackageVulnerabilityDetailsTypeDef(TypedDict):
    source: str,
    vulnerabilityId: str,
    cvss: NotRequired[List[CvssScoreTypeDef]],  # (1)
    referenceUrls: NotRequired[List[str]],
    relatedVulnerabilities: NotRequired[List[str]],
    sourceUrl: NotRequired[str],
    vendorCreatedAt: NotRequired[datetime],
    vendorSeverity: NotRequired[str],
    vendorUpdatedAt: NotRequired[datetime],
    vulnerablePackages: NotRequired[List[VulnerablePackageTypeDef]],  # (2)
```

1. See [:material-code-braces: CvssScoreTypeDef](./type_defs.md#cvssscoretypedef) 
2. See [:material-code-braces: VulnerablePackageTypeDef](./type_defs.md#vulnerablepackagetypedef) 
## RemediationTypeDef

```python
# RemediationTypeDef definition

class RemediationTypeDef(TypedDict):
    recommendation: NotRequired[RecommendationTypeDef],  # (1)
```

1. See [:material-code-braces: RecommendationTypeDef](./type_defs.md#recommendationtypedef) 
## ResourceFilterCriteriaTypeDef

```python
# ResourceFilterCriteriaTypeDef definition

class ResourceFilterCriteriaTypeDef(TypedDict):
    accountId: NotRequired[Sequence[ResourceStringFilterTypeDef]],  # (1)
    ec2InstanceTags: NotRequired[Sequence[ResourceMapFilterTypeDef]],  # (2)
    ecrImageTags: NotRequired[Sequence[ResourceStringFilterTypeDef]],  # (1)
    ecrRepositoryName: NotRequired[Sequence[ResourceStringFilterTypeDef]],  # (1)
    lambdaFunctionName: NotRequired[Sequence[ResourceStringFilterTypeDef]],  # (1)
    lambdaFunctionTags: NotRequired[Sequence[ResourceMapFilterTypeDef]],  # (2)
    resourceId: NotRequired[Sequence[ResourceStringFilterTypeDef]],  # (1)
    resourceType: NotRequired[Sequence[ResourceStringFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: ResourceStringFilterTypeDef](./type_defs.md#resourcestringfiltertypedef) 
2. See [:material-code-braces: ResourceMapFilterTypeDef](./type_defs.md#resourcemapfiltertypedef) 
3. See [:material-code-braces: ResourceStringFilterTypeDef](./type_defs.md#resourcestringfiltertypedef) 
4. See [:material-code-braces: ResourceStringFilterTypeDef](./type_defs.md#resourcestringfiltertypedef) 
5. See [:material-code-braces: ResourceStringFilterTypeDef](./type_defs.md#resourcestringfiltertypedef) 
6. See [:material-code-braces: ResourceMapFilterTypeDef](./type_defs.md#resourcemapfiltertypedef) 
7. See [:material-code-braces: ResourceStringFilterTypeDef](./type_defs.md#resourcestringfiltertypedef) 
8. See [:material-code-braces: ResourceStringFilterTypeDef](./type_defs.md#resourcestringfiltertypedef) 
## SearchVulnerabilitiesRequestRequestTypeDef

```python
# SearchVulnerabilitiesRequestRequestTypeDef definition

class SearchVulnerabilitiesRequestRequestTypeDef(TypedDict):
    filterCriteria: SearchVulnerabilitiesFilterCriteriaTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SearchVulnerabilitiesFilterCriteriaTypeDef](./type_defs.md#searchvulnerabilitiesfiltercriteriatypedef) 
## SearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef

```python
# SearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef definition

class SearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef(TypedDict):
    filterCriteria: SearchVulnerabilitiesFilterCriteriaTypeDef,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: SearchVulnerabilitiesFilterCriteriaTypeDef](./type_defs.md#searchvulnerabilitiesfiltercriteriatypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## UsageTotalTypeDef

```python
# UsageTotalTypeDef definition

class UsageTotalTypeDef(TypedDict):
    accountId: NotRequired[str],
    usage: NotRequired[List[UsageTypeDef]],  # (1)
```

1. See [:material-code-braces: UsageTypeDef](./type_defs.md#usagetypedef) 
## AggregationResponseTypeDef

```python
# AggregationResponseTypeDef definition

class AggregationResponseTypeDef(TypedDict):
    accountAggregation: NotRequired[AccountAggregationResponseTypeDef],  # (1)
    amiAggregation: NotRequired[AmiAggregationResponseTypeDef],  # (2)
    awsEcrContainerAggregation: NotRequired[AwsEcrContainerAggregationResponseTypeDef],  # (3)
    ec2InstanceAggregation: NotRequired[Ec2InstanceAggregationResponseTypeDef],  # (4)
    findingTypeAggregation: NotRequired[FindingTypeAggregationResponseTypeDef],  # (5)
    imageLayerAggregation: NotRequired[ImageLayerAggregationResponseTypeDef],  # (6)
    lambdaFunctionAggregation: NotRequired[LambdaFunctionAggregationResponseTypeDef],  # (7)
    lambdaLayerAggregation: NotRequired[LambdaLayerAggregationResponseTypeDef],  # (8)
    packageAggregation: NotRequired[PackageAggregationResponseTypeDef],  # (9)
    repositoryAggregation: NotRequired[RepositoryAggregationResponseTypeDef],  # (10)
    titleAggregation: NotRequired[TitleAggregationResponseTypeDef],  # (11)
```

1. See [:material-code-braces: AccountAggregationResponseTypeDef](./type_defs.md#accountaggregationresponsetypedef) 
2. See [:material-code-braces: AmiAggregationResponseTypeDef](./type_defs.md#amiaggregationresponsetypedef) 
3. See [:material-code-braces: AwsEcrContainerAggregationResponseTypeDef](./type_defs.md#awsecrcontaineraggregationresponsetypedef) 
4. See [:material-code-braces: Ec2InstanceAggregationResponseTypeDef](./type_defs.md#ec2instanceaggregationresponsetypedef) 
5. See [:material-code-braces: FindingTypeAggregationResponseTypeDef](./type_defs.md#findingtypeaggregationresponsetypedef) 
6. See [:material-code-braces: ImageLayerAggregationResponseTypeDef](./type_defs.md#imagelayeraggregationresponsetypedef) 
7. See [:material-code-braces: LambdaFunctionAggregationResponseTypeDef](./type_defs.md#lambdafunctionaggregationresponsetypedef) 
8. See [:material-code-braces: LambdaLayerAggregationResponseTypeDef](./type_defs.md#lambdalayeraggregationresponsetypedef) 
9. See [:material-code-braces: PackageAggregationResponseTypeDef](./type_defs.md#packageaggregationresponsetypedef) 
10. See [:material-code-braces: RepositoryAggregationResponseTypeDef](./type_defs.md#repositoryaggregationresponsetypedef) 
11. See [:material-code-braces: TitleAggregationResponseTypeDef](./type_defs.md#titleaggregationresponsetypedef) 
## AccountStateTypeDef

```python
# AccountStateTypeDef definition

class AccountStateTypeDef(TypedDict):
    accountId: str,
    resourceState: ResourceStateTypeDef,  # (1)
    state: StateTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceStateTypeDef](./type_defs.md#resourcestatetypedef) 
2. See [:material-code-braces: StateTypeDef](./type_defs.md#statetypedef) 
## DisableResponseTypeDef

```python
# DisableResponseTypeDef definition

class DisableResponseTypeDef(TypedDict):
    accounts: List[AccountTypeDef],  # (1)
    failedAccounts: List[FailedAccountTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AccountTypeDef](./type_defs.md#accounttypedef) 
2. See [:material-code-braces: FailedAccountTypeDef](./type_defs.md#failedaccounttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnableResponseTypeDef

```python
# EnableResponseTypeDef definition

class EnableResponseTypeDef(TypedDict):
    accounts: List[AccountTypeDef],  # (1)
    failedAccounts: List[FailedAccountTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AccountTypeDef](./type_defs.md#accounttypedef) 
2. See [:material-code-braces: FailedAccountTypeDef](./type_defs.md#failedaccounttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResourceDetailsTypeDef

```python
# ResourceDetailsTypeDef definition

class ResourceDetailsTypeDef(TypedDict):
    awsEc2Instance: NotRequired[AwsEc2InstanceDetailsTypeDef],  # (1)
    awsEcrContainerImage: NotRequired[AwsEcrContainerImageDetailsTypeDef],  # (2)
    awsLambdaFunction: NotRequired[AwsLambdaFunctionDetailsTypeDef],  # (3)
```

1. See [:material-code-braces: AwsEc2InstanceDetailsTypeDef](./type_defs.md#awsec2instancedetailstypedef) 
2. See [:material-code-braces: AwsEcrContainerImageDetailsTypeDef](./type_defs.md#awsecrcontainerimagedetailstypedef) 
3. See [:material-code-braces: AwsLambdaFunctionDetailsTypeDef](./type_defs.md#awslambdafunctiondetailstypedef) 
## BatchGetCodeSnippetResponseTypeDef

```python
# BatchGetCodeSnippetResponseTypeDef definition

class BatchGetCodeSnippetResponseTypeDef(TypedDict):
    codeSnippetResults: List[CodeSnippetResultTypeDef],  # (1)
    errors: List[CodeSnippetErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: CodeSnippetResultTypeDef](./type_defs.md#codesnippetresulttypedef) 
2. See [:material-code-braces: CodeSnippetErrorTypeDef](./type_defs.md#codesnippeterrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CoverageFilterCriteriaTypeDef

```python
# CoverageFilterCriteriaTypeDef definition

class CoverageFilterCriteriaTypeDef(TypedDict):
    accountId: NotRequired[Sequence[CoverageStringFilterTypeDef]],  # (1)
    ec2InstanceTags: NotRequired[Sequence[CoverageMapFilterTypeDef]],  # (2)
    ecrImageTags: NotRequired[Sequence[CoverageStringFilterTypeDef]],  # (1)
    ecrRepositoryName: NotRequired[Sequence[CoverageStringFilterTypeDef]],  # (1)
    lambdaFunctionName: NotRequired[Sequence[CoverageStringFilterTypeDef]],  # (1)
    lambdaFunctionRuntime: NotRequired[Sequence[CoverageStringFilterTypeDef]],  # (1)
    lambdaFunctionTags: NotRequired[Sequence[CoverageMapFilterTypeDef]],  # (2)
    lastScannedAt: NotRequired[Sequence[CoverageDateFilterTypeDef]],  # (8)
    resourceId: NotRequired[Sequence[CoverageStringFilterTypeDef]],  # (1)
    resourceType: NotRequired[Sequence[CoverageStringFilterTypeDef]],  # (1)
    scanStatusCode: NotRequired[Sequence[CoverageStringFilterTypeDef]],  # (1)
    scanStatusReason: NotRequired[Sequence[CoverageStringFilterTypeDef]],  # (1)
    scanType: NotRequired[Sequence[CoverageStringFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: CoverageStringFilterTypeDef](./type_defs.md#coveragestringfiltertypedef) 
2. See [:material-code-braces: CoverageMapFilterTypeDef](./type_defs.md#coveragemapfiltertypedef) 
3. See [:material-code-braces: CoverageStringFilterTypeDef](./type_defs.md#coveragestringfiltertypedef) 
4. See [:material-code-braces: CoverageStringFilterTypeDef](./type_defs.md#coveragestringfiltertypedef) 
5. See [:material-code-braces: CoverageStringFilterTypeDef](./type_defs.md#coveragestringfiltertypedef) 
6. See [:material-code-braces: CoverageStringFilterTypeDef](./type_defs.md#coveragestringfiltertypedef) 
7. See [:material-code-braces: CoverageMapFilterTypeDef](./type_defs.md#coveragemapfiltertypedef) 
8. See [:material-code-braces: CoverageDateFilterTypeDef](./type_defs.md#coveragedatefiltertypedef) 
9. See [:material-code-braces: CoverageStringFilterTypeDef](./type_defs.md#coveragestringfiltertypedef) 
10. See [:material-code-braces: CoverageStringFilterTypeDef](./type_defs.md#coveragestringfiltertypedef) 
11. See [:material-code-braces: CoverageStringFilterTypeDef](./type_defs.md#coveragestringfiltertypedef) 
12. See [:material-code-braces: CoverageStringFilterTypeDef](./type_defs.md#coveragestringfiltertypedef) 
13. See [:material-code-braces: CoverageStringFilterTypeDef](./type_defs.md#coveragestringfiltertypedef) 
## InspectorScoreDetailsTypeDef

```python
# InspectorScoreDetailsTypeDef definition

class InspectorScoreDetailsTypeDef(TypedDict):
    adjustedCvss: NotRequired[CvssScoreDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: CvssScoreDetailsTypeDef](./type_defs.md#cvssscoredetailstypedef) 
## AggregationRequestTypeDef

```python
# AggregationRequestTypeDef definition

class AggregationRequestTypeDef(TypedDict):
    accountAggregation: NotRequired[AccountAggregationTypeDef],  # (1)
    amiAggregation: NotRequired[AmiAggregationTypeDef],  # (2)
    awsEcrContainerAggregation: NotRequired[AwsEcrContainerAggregationTypeDef],  # (3)
    ec2InstanceAggregation: NotRequired[Ec2InstanceAggregationTypeDef],  # (4)
    findingTypeAggregation: NotRequired[FindingTypeAggregationTypeDef],  # (5)
    imageLayerAggregation: NotRequired[ImageLayerAggregationTypeDef],  # (6)
    lambdaFunctionAggregation: NotRequired[LambdaFunctionAggregationTypeDef],  # (7)
    lambdaLayerAggregation: NotRequired[LambdaLayerAggregationTypeDef],  # (8)
    packageAggregation: NotRequired[PackageAggregationTypeDef],  # (9)
    repositoryAggregation: NotRequired[RepositoryAggregationTypeDef],  # (10)
    titleAggregation: NotRequired[TitleAggregationTypeDef],  # (11)
```

1. See [:material-code-braces: AccountAggregationTypeDef](./type_defs.md#accountaggregationtypedef) 
2. See [:material-code-braces: AmiAggregationTypeDef](./type_defs.md#amiaggregationtypedef) 
3. See [:material-code-braces: AwsEcrContainerAggregationTypeDef](./type_defs.md#awsecrcontaineraggregationtypedef) 
4. See [:material-code-braces: Ec2InstanceAggregationTypeDef](./type_defs.md#ec2instanceaggregationtypedef) 
5. See [:material-code-braces: FindingTypeAggregationTypeDef](./type_defs.md#findingtypeaggregationtypedef) 
6. See [:material-code-braces: ImageLayerAggregationTypeDef](./type_defs.md#imagelayeraggregationtypedef) 
7. See [:material-code-braces: LambdaFunctionAggregationTypeDef](./type_defs.md#lambdafunctionaggregationtypedef) 
8. See [:material-code-braces: LambdaLayerAggregationTypeDef](./type_defs.md#lambdalayeraggregationtypedef) 
9. See [:material-code-braces: PackageAggregationTypeDef](./type_defs.md#packageaggregationtypedef) 
10. See [:material-code-braces: RepositoryAggregationTypeDef](./type_defs.md#repositoryaggregationtypedef) 
11. See [:material-code-braces: TitleAggregationTypeDef](./type_defs.md#titleaggregationtypedef) 
## GetConfigurationResponseTypeDef

```python
# GetConfigurationResponseTypeDef definition

class GetConfigurationResponseTypeDef(TypedDict):
    ecrConfiguration: EcrConfigurationStateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EcrConfigurationStateTypeDef](./type_defs.md#ecrconfigurationstatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetFindingDetailsResponseTypeDef

```python
# BatchGetFindingDetailsResponseTypeDef definition

class BatchGetFindingDetailsResponseTypeDef(TypedDict):
    errors: List[FindingDetailsErrorTypeDef],  # (1)
    findingDetails: List[FindingDetailTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FindingDetailsErrorTypeDef](./type_defs.md#findingdetailserrortypedef) 
2. See [:material-code-braces: FindingDetailTypeDef](./type_defs.md#findingdetailtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchVulnerabilitiesResponseTypeDef

```python
# SearchVulnerabilitiesResponseTypeDef definition

class SearchVulnerabilitiesResponseTypeDef(TypedDict):
    nextToken: str,
    vulnerabilities: List[VulnerabilityTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VulnerabilityTypeDef](./type_defs.md#vulnerabilitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FilterCriteriaTypeDef

```python
# FilterCriteriaTypeDef definition

class FilterCriteriaTypeDef(TypedDict):
    awsAccountId: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    codeVulnerabilityDetectorName: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    codeVulnerabilityDetectorTags: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    codeVulnerabilityFilePath: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    componentId: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    componentType: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ec2InstanceImageId: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ec2InstanceSubnetId: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ec2InstanceVpcId: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ecrImageArchitecture: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ecrImageHash: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ecrImagePushedAt: NotRequired[Sequence[DateFilterTypeDef]],  # (12)
    ecrImageRegistry: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ecrImageRepositoryName: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    ecrImageTags: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    epssScore: NotRequired[Sequence[NumberFilterTypeDef]],  # (16)
    exploitAvailable: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    findingArn: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    findingStatus: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    findingType: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    firstObservedAt: NotRequired[Sequence[DateFilterTypeDef]],  # (12)
    fixAvailable: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    inspectorScore: NotRequired[Sequence[NumberFilterTypeDef]],  # (16)
    lambdaFunctionExecutionRoleArn: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    lambdaFunctionLastModifiedAt: NotRequired[Sequence[DateFilterTypeDef]],  # (12)
    lambdaFunctionLayers: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    lambdaFunctionName: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    lambdaFunctionRuntime: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    lastObservedAt: NotRequired[Sequence[DateFilterTypeDef]],  # (12)
    networkProtocol: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    portRange: NotRequired[Sequence[PortRangeFilterTypeDef]],  # (31)
    relatedVulnerabilities: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    resourceId: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    resourceTags: NotRequired[Sequence[MapFilterTypeDef]],  # (34)
    resourceType: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    severity: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    title: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    updatedAt: NotRequired[Sequence[DateFilterTypeDef]],  # (12)
    vendorSeverity: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    vulnerabilityId: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    vulnerabilitySource: NotRequired[Sequence[StringFilterTypeDef]],  # (1)
    vulnerablePackages: NotRequired[Sequence[PackageFilterTypeDef]],  # (42)
```

1. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
2. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
3. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
4. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
5. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
6. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
7. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
8. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
9. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
10. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
11. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
12. See [:material-code-braces: DateFilterTypeDef](./type_defs.md#datefiltertypedef) 
13. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
14. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
15. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
16. See [:material-code-braces: NumberFilterTypeDef](./type_defs.md#numberfiltertypedef) 
17. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
18. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
19. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
20. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
21. See [:material-code-braces: DateFilterTypeDef](./type_defs.md#datefiltertypedef) 
22. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
23. See [:material-code-braces: NumberFilterTypeDef](./type_defs.md#numberfiltertypedef) 
24. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
25. See [:material-code-braces: DateFilterTypeDef](./type_defs.md#datefiltertypedef) 
26. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
27. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
28. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
29. See [:material-code-braces: DateFilterTypeDef](./type_defs.md#datefiltertypedef) 
30. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
31. See [:material-code-braces: PortRangeFilterTypeDef](./type_defs.md#portrangefiltertypedef) 
32. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
33. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
34. See [:material-code-braces: MapFilterTypeDef](./type_defs.md#mapfiltertypedef) 
35. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
36. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
37. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
38. See [:material-code-braces: DateFilterTypeDef](./type_defs.md#datefiltertypedef) 
39. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
40. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
41. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
42. See [:material-code-braces: PackageFilterTypeDef](./type_defs.md#packagefiltertypedef) 
## BatchGetFreeTrialInfoResponseTypeDef

```python
# BatchGetFreeTrialInfoResponseTypeDef definition

class BatchGetFreeTrialInfoResponseTypeDef(TypedDict):
    accounts: List[FreeTrialAccountInfoTypeDef],  # (1)
    failedAccounts: List[FreeTrialInfoErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FreeTrialAccountInfoTypeDef](./type_defs.md#freetrialaccountinfotypedef) 
2. See [:material-code-braces: FreeTrialInfoErrorTypeDef](./type_defs.md#freetrialinfoerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CoveredResourceTypeDef

```python
# CoveredResourceTypeDef definition

class CoveredResourceTypeDef(TypedDict):
    accountId: str,
    resourceId: str,
    resourceType: CoverageResourceTypeType,  # (2)
    scanType: ScanTypeType,  # (4)
    lastScannedAt: NotRequired[datetime],
    resourceMetadata: NotRequired[ResourceScanMetadataTypeDef],  # (1)
    scanStatus: NotRequired[ScanStatusTypeDef],  # (3)
```

1. See [:material-code-braces: ResourceScanMetadataTypeDef](./type_defs.md#resourcescanmetadatatypedef) 
2. See [:material-code-brackets: CoverageResourceTypeType](./literals.md#coverageresourcetypetype) 
3. See [:material-code-braces: ScanStatusTypeDef](./type_defs.md#scanstatustypedef) 
4. See [:material-code-brackets: ScanTypeType](./literals.md#scantypetype) 
## NetworkReachabilityDetailsTypeDef

```python
# NetworkReachabilityDetailsTypeDef definition

class NetworkReachabilityDetailsTypeDef(TypedDict):
    networkPath: NetworkPathTypeDef,  # (1)
    openPortRange: PortRangeTypeDef,  # (2)
    protocol: NetworkProtocolType,  # (3)
```

1. See [:material-code-braces: NetworkPathTypeDef](./type_defs.md#networkpathtypedef) 
2. See [:material-code-braces: PortRangeTypeDef](./type_defs.md#portrangetypedef) 
3. See [:material-code-brackets: NetworkProtocolType](./literals.md#networkprotocoltype) 
## CreateSbomExportRequestRequestTypeDef

```python
# CreateSbomExportRequestRequestTypeDef definition

class CreateSbomExportRequestRequestTypeDef(TypedDict):
    reportFormat: SbomReportFormatType,  # (1)
    s3Destination: DestinationTypeDef,  # (2)
    resourceFilterCriteria: NotRequired[ResourceFilterCriteriaTypeDef],  # (3)
```

1. See [:material-code-brackets: SbomReportFormatType](./literals.md#sbomreportformattype) 
2. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
3. See [:material-code-braces: ResourceFilterCriteriaTypeDef](./type_defs.md#resourcefiltercriteriatypedef) 
## GetSbomExportResponseTypeDef

```python
# GetSbomExportResponseTypeDef definition

class GetSbomExportResponseTypeDef(TypedDict):
    errorCode: ReportingErrorCodeType,  # (1)
    errorMessage: str,
    filterCriteria: ResourceFilterCriteriaTypeDef,  # (2)
    format: SbomReportFormatType,  # (3)
    reportId: str,
    s3Destination: DestinationTypeDef,  # (4)
    status: ExternalReportStatusType,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: ReportingErrorCodeType](./literals.md#reportingerrorcodetype) 
2. See [:material-code-braces: ResourceFilterCriteriaTypeDef](./type_defs.md#resourcefiltercriteriatypedef) 
3. See [:material-code-brackets: SbomReportFormatType](./literals.md#sbomreportformattype) 
4. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
5. See [:material-code-brackets: ExternalReportStatusType](./literals.md#externalreportstatustype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUsageTotalsResponseTypeDef

```python
# ListUsageTotalsResponseTypeDef definition

class ListUsageTotalsResponseTypeDef(TypedDict):
    nextToken: str,
    totals: List[UsageTotalTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UsageTotalTypeDef](./type_defs.md#usagetotaltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFindingAggregationsResponseTypeDef

```python
# ListFindingAggregationsResponseTypeDef definition

class ListFindingAggregationsResponseTypeDef(TypedDict):
    aggregationType: AggregationTypeType,  # (1)
    nextToken: str,
    responses: List[AggregationResponseTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: AggregationTypeType](./literals.md#aggregationtypetype) 
2. See [:material-code-braces: AggregationResponseTypeDef](./type_defs.md#aggregationresponsetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetAccountStatusResponseTypeDef

```python
# BatchGetAccountStatusResponseTypeDef definition

class BatchGetAccountStatusResponseTypeDef(TypedDict):
    accounts: List[AccountStateTypeDef],  # (1)
    failedAccounts: List[FailedAccountTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AccountStateTypeDef](./type_defs.md#accountstatetypedef) 
2. See [:material-code-braces: FailedAccountTypeDef](./type_defs.md#failedaccounttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResourceTypeDef

```python
# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    id: str,
    type: ResourceTypeType,  # (2)
    details: NotRequired[ResourceDetailsTypeDef],  # (1)
    partition: NotRequired[str],
    region: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: ResourceDetailsTypeDef](./type_defs.md#resourcedetailstypedef) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## ListCoverageRequestListCoveragePaginateTypeDef

```python
# ListCoverageRequestListCoveragePaginateTypeDef definition

class ListCoverageRequestListCoveragePaginateTypeDef(TypedDict):
    filterCriteria: NotRequired[CoverageFilterCriteriaTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: CoverageFilterCriteriaTypeDef](./type_defs.md#coveragefiltercriteriatypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCoverageRequestRequestTypeDef

```python
# ListCoverageRequestRequestTypeDef definition

class ListCoverageRequestRequestTypeDef(TypedDict):
    filterCriteria: NotRequired[CoverageFilterCriteriaTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CoverageFilterCriteriaTypeDef](./type_defs.md#coveragefiltercriteriatypedef) 
## ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef

```python
# ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef definition

class ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef(TypedDict):
    filterCriteria: NotRequired[CoverageFilterCriteriaTypeDef],  # (1)
    groupBy: NotRequired[GroupKeyType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: CoverageFilterCriteriaTypeDef](./type_defs.md#coveragefiltercriteriatypedef) 
2. See [:material-code-brackets: GroupKeyType](./literals.md#groupkeytype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCoverageStatisticsRequestRequestTypeDef

```python
# ListCoverageStatisticsRequestRequestTypeDef definition

class ListCoverageStatisticsRequestRequestTypeDef(TypedDict):
    filterCriteria: NotRequired[CoverageFilterCriteriaTypeDef],  # (1)
    groupBy: NotRequired[GroupKeyType],  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CoverageFilterCriteriaTypeDef](./type_defs.md#coveragefiltercriteriatypedef) 
2. See [:material-code-brackets: GroupKeyType](./literals.md#groupkeytype) 
## ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef

```python
# ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef definition

class ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef(TypedDict):
    aggregationType: AggregationTypeType,  # (1)
    accountIds: NotRequired[Sequence[StringFilterTypeDef]],  # (2)
    aggregationRequest: NotRequired[AggregationRequestTypeDef],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: AggregationTypeType](./literals.md#aggregationtypetype) 
2. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
3. See [:material-code-braces: AggregationRequestTypeDef](./type_defs.md#aggregationrequesttypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFindingAggregationsRequestRequestTypeDef

```python
# ListFindingAggregationsRequestRequestTypeDef definition

class ListFindingAggregationsRequestRequestTypeDef(TypedDict):
    aggregationType: AggregationTypeType,  # (1)
    accountIds: NotRequired[Sequence[StringFilterTypeDef]],  # (2)
    aggregationRequest: NotRequired[AggregationRequestTypeDef],  # (3)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: AggregationTypeType](./literals.md#aggregationtypetype) 
2. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
3. See [:material-code-braces: AggregationRequestTypeDef](./type_defs.md#aggregationrequesttypedef) 
## CreateFilterRequestRequestTypeDef

```python
# CreateFilterRequestRequestTypeDef definition

class CreateFilterRequestRequestTypeDef(TypedDict):
    action: FilterActionType,  # (1)
    filterCriteria: FilterCriteriaTypeDef,  # (2)
    name: str,
    description: NotRequired[str],
    reason: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: FilterActionType](./literals.md#filteractiontype) 
2. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) 
## CreateFindingsReportRequestRequestTypeDef

```python
# CreateFindingsReportRequestRequestTypeDef definition

class CreateFindingsReportRequestRequestTypeDef(TypedDict):
    reportFormat: ReportFormatType,  # (1)
    s3Destination: DestinationTypeDef,  # (2)
    filterCriteria: NotRequired[FilterCriteriaTypeDef],  # (3)
```

1. See [:material-code-brackets: ReportFormatType](./literals.md#reportformattype) 
2. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
3. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) 
## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    action: FilterActionType,  # (1)
    arn: str,
    createdAt: datetime,
    criteria: FilterCriteriaTypeDef,  # (2)
    name: str,
    ownerId: str,
    updatedAt: datetime,
    description: NotRequired[str],
    reason: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: FilterActionType](./literals.md#filteractiontype) 
2. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) 
## GetFindingsReportStatusResponseTypeDef

```python
# GetFindingsReportStatusResponseTypeDef definition

class GetFindingsReportStatusResponseTypeDef(TypedDict):
    destination: DestinationTypeDef,  # (1)
    errorCode: ReportingErrorCodeType,  # (2)
    errorMessage: str,
    filterCriteria: FilterCriteriaTypeDef,  # (3)
    reportId: str,
    status: ExternalReportStatusType,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
2. See [:material-code-brackets: ReportingErrorCodeType](./literals.md#reportingerrorcodetype) 
3. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) 
4. See [:material-code-brackets: ExternalReportStatusType](./literals.md#externalreportstatustype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFindingsRequestListFindingsPaginateTypeDef

```python
# ListFindingsRequestListFindingsPaginateTypeDef definition

class ListFindingsRequestListFindingsPaginateTypeDef(TypedDict):
    filterCriteria: NotRequired[FilterCriteriaTypeDef],  # (1)
    sortCriteria: NotRequired[SortCriteriaTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) 
2. See [:material-code-braces: SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFindingsRequestRequestTypeDef

```python
# ListFindingsRequestRequestTypeDef definition

class ListFindingsRequestRequestTypeDef(TypedDict):
    filterCriteria: NotRequired[FilterCriteriaTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    sortCriteria: NotRequired[SortCriteriaTypeDef],  # (2)
```

1. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) 
2. See [:material-code-braces: SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef) 
## UpdateFilterRequestRequestTypeDef

```python
# UpdateFilterRequestRequestTypeDef definition

class UpdateFilterRequestRequestTypeDef(TypedDict):
    filterArn: str,
    action: NotRequired[FilterActionType],  # (1)
    description: NotRequired[str],
    filterCriteria: NotRequired[FilterCriteriaTypeDef],  # (2)
    name: NotRequired[str],
    reason: NotRequired[str],
```

1. See [:material-code-brackets: FilterActionType](./literals.md#filteractiontype) 
2. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) 
## ListCoverageResponseTypeDef

```python
# ListCoverageResponseTypeDef definition

class ListCoverageResponseTypeDef(TypedDict):
    coveredResources: List[CoveredResourceTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CoveredResourceTypeDef](./type_defs.md#coveredresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FindingTypeDef

```python
# FindingTypeDef definition

class FindingTypeDef(TypedDict):
    awsAccountId: str,
    description: str,
    findingArn: str,
    firstObservedAt: datetime,
    lastObservedAt: datetime,
    remediation: RemediationTypeDef,  # (9)
    resources: List[ResourceTypeDef],  # (10)
    severity: SeverityType,  # (11)
    status: FindingStatusType,  # (12)
    type: FindingTypeType,  # (13)
    codeVulnerabilityDetails: NotRequired[CodeVulnerabilityDetailsTypeDef],  # (1)
    epss: NotRequired[EpssDetailsTypeDef],  # (2)
    exploitAvailable: NotRequired[ExploitAvailableType],  # (3)
    exploitabilityDetails: NotRequired[ExploitabilityDetailsTypeDef],  # (4)
    fixAvailable: NotRequired[FixAvailableType],  # (5)
    inspectorScore: NotRequired[float],
    inspectorScoreDetails: NotRequired[InspectorScoreDetailsTypeDef],  # (6)
    networkReachabilityDetails: NotRequired[NetworkReachabilityDetailsTypeDef],  # (7)
    packageVulnerabilityDetails: NotRequired[PackageVulnerabilityDetailsTypeDef],  # (8)
    title: NotRequired[str],
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-braces: CodeVulnerabilityDetailsTypeDef](./type_defs.md#codevulnerabilitydetailstypedef) 
2. See [:material-code-braces: EpssDetailsTypeDef](./type_defs.md#epssdetailstypedef) 
3. See [:material-code-brackets: ExploitAvailableType](./literals.md#exploitavailabletype) 
4. See [:material-code-braces: ExploitabilityDetailsTypeDef](./type_defs.md#exploitabilitydetailstypedef) 
5. See [:material-code-brackets: FixAvailableType](./literals.md#fixavailabletype) 
6. See [:material-code-braces: InspectorScoreDetailsTypeDef](./type_defs.md#inspectorscoredetailstypedef) 
7. See [:material-code-braces: NetworkReachabilityDetailsTypeDef](./type_defs.md#networkreachabilitydetailstypedef) 
8. See [:material-code-braces: PackageVulnerabilityDetailsTypeDef](./type_defs.md#packagevulnerabilitydetailstypedef) 
9. See [:material-code-braces: RemediationTypeDef](./type_defs.md#remediationtypedef) 
10. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
11. See [:material-code-brackets: SeverityType](./literals.md#severitytype) 
12. See [:material-code-brackets: FindingStatusType](./literals.md#findingstatustype) 
13. See [:material-code-brackets: FindingTypeType](./literals.md#findingtypetype) 
## ListFiltersResponseTypeDef

```python
# ListFiltersResponseTypeDef definition

class ListFiltersResponseTypeDef(TypedDict):
    filters: List[FilterTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFindingsResponseTypeDef

```python
# ListFindingsResponseTypeDef definition

class ListFindingsResponseTypeDef(TypedDict):
    findings: List[FindingTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FindingTypeDef](./type_defs.md#findingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
