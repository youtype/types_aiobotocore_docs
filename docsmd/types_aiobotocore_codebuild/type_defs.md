# Type definitions

> [Index](../README.md) > [CodeBuild](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CodeBuild](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#codebuild)
    type annotations stubs module [types-aiobotocore-codebuild](https://pypi.org/project/types-aiobotocore-codebuild/).

## BatchRestrictionsUnionTypeDef

```python
# BatchRestrictionsUnionTypeDef definition

BatchRestrictionsUnionTypeDef = Union[
    BatchRestrictionsTypeDef,  # (1)
    BatchRestrictionsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: BatchRestrictionsTypeDef](./type_defs.md#batchrestrictionstypedef) 
2. See [:material-code-braces: BatchRestrictionsOutputTypeDef](./type_defs.md#batchrestrictionsoutputtypedef) 

## FleetProxyRuleUnionTypeDef

```python
# FleetProxyRuleUnionTypeDef definition

FleetProxyRuleUnionTypeDef = Union[
    FleetProxyRuleTypeDef,  # (1)
    FleetProxyRuleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FleetProxyRuleTypeDef](./type_defs.md#fleetproxyruletypedef) 
2. See [:material-code-braces: FleetProxyRuleOutputTypeDef](./type_defs.md#fleetproxyruleoutputtypedef) 



## AutoRetryConfigTypeDef

```python
# AutoRetryConfigTypeDef definition

class AutoRetryConfigTypeDef(TypedDict):
    autoRetryLimit: NotRequired[int],
    autoRetryNumber: NotRequired[int],
    nextAutoRetry: NotRequired[str],
    previousAutoRetry: NotRequired[str],
```

## BatchDeleteBuildsInputRequestTypeDef

```python
# BatchDeleteBuildsInputRequestTypeDef definition

class BatchDeleteBuildsInputRequestTypeDef(TypedDict):
    ids: Sequence[str],
```

## BuildNotDeletedTypeDef

```python
# BuildNotDeletedTypeDef definition

class BuildNotDeletedTypeDef(TypedDict):
    id: NotRequired[str],
    statusCode: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## BatchGetBuildBatchesInputRequestTypeDef

```python
# BatchGetBuildBatchesInputRequestTypeDef definition

class BatchGetBuildBatchesInputRequestTypeDef(TypedDict):
    ids: Sequence[str],
```

## BatchGetBuildsInputRequestTypeDef

```python
# BatchGetBuildsInputRequestTypeDef definition

class BatchGetBuildsInputRequestTypeDef(TypedDict):
    ids: Sequence[str],
```

## BatchGetFleetsInputRequestTypeDef

```python
# BatchGetFleetsInputRequestTypeDef definition

class BatchGetFleetsInputRequestTypeDef(TypedDict):
    names: Sequence[str],
```

## BatchGetProjectsInputRequestTypeDef

```python
# BatchGetProjectsInputRequestTypeDef definition

class BatchGetProjectsInputRequestTypeDef(TypedDict):
    names: Sequence[str],
```

## BatchGetReportGroupsInputRequestTypeDef

```python
# BatchGetReportGroupsInputRequestTypeDef definition

class BatchGetReportGroupsInputRequestTypeDef(TypedDict):
    reportGroupArns: Sequence[str],
```

## BatchGetReportsInputRequestTypeDef

```python
# BatchGetReportsInputRequestTypeDef definition

class BatchGetReportsInputRequestTypeDef(TypedDict):
    reportArns: Sequence[str],
```

## BatchRestrictionsOutputTypeDef

```python
# BatchRestrictionsOutputTypeDef definition

class BatchRestrictionsOutputTypeDef(TypedDict):
    maximumBuildsAllowed: NotRequired[int],
    computeTypesAllowed: NotRequired[List[str]],
    fleetsAllowed: NotRequired[List[str]],
```

## BatchRestrictionsTypeDef

```python
# BatchRestrictionsTypeDef definition

class BatchRestrictionsTypeDef(TypedDict):
    maximumBuildsAllowed: NotRequired[int],
    computeTypesAllowed: NotRequired[Sequence[str]],
    fleetsAllowed: NotRequired[Sequence[str]],
```

## BuildArtifactsTypeDef

```python
# BuildArtifactsTypeDef definition

class BuildArtifactsTypeDef(TypedDict):
    location: NotRequired[str],
    sha256sum: NotRequired[str],
    md5sum: NotRequired[str],
    overrideArtifactName: NotRequired[bool],
    encryptionDisabled: NotRequired[bool],
    artifactIdentifier: NotRequired[str],
    bucketOwnerAccess: NotRequired[BucketOwnerAccessType],  # (1)
```

1. See [:material-code-brackets: BucketOwnerAccessType](./literals.md#bucketowneraccesstype) 
## BuildBatchFilterTypeDef

```python
# BuildBatchFilterTypeDef definition

class BuildBatchFilterTypeDef(TypedDict):
    status: NotRequired[StatusTypeType],  # (1)
```

1. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
## PhaseContextTypeDef

```python
# PhaseContextTypeDef definition

class PhaseContextTypeDef(TypedDict):
    statusCode: NotRequired[str],
    message: NotRequired[str],
```

## ProjectCacheOutputTypeDef

```python
# ProjectCacheOutputTypeDef definition

class ProjectCacheOutputTypeDef(TypedDict):
    type: CacheTypeType,  # (1)
    location: NotRequired[str],
    modes: NotRequired[List[CacheModeType]],  # (2)
```

1. See [:material-code-brackets: CacheTypeType](./literals.md#cachetypetype) 
2. See [:material-code-brackets: CacheModeType](./literals.md#cachemodetype) 
## ProjectFileSystemLocationTypeDef

```python
# ProjectFileSystemLocationTypeDef definition

class ProjectFileSystemLocationTypeDef(TypedDict):
    type: NotRequired[FileSystemTypeType],  # (1)
    location: NotRequired[str],
    mountPoint: NotRequired[str],
    identifier: NotRequired[str],
    mountOptions: NotRequired[str],
```

1. See [:material-code-brackets: FileSystemTypeType](./literals.md#filesystemtypetype) 
## ProjectSourceVersionTypeDef

```python
# ProjectSourceVersionTypeDef definition

class ProjectSourceVersionTypeDef(TypedDict):
    sourceIdentifier: str,
    sourceVersion: str,
```

## VpcConfigOutputTypeDef

```python
# VpcConfigOutputTypeDef definition

class VpcConfigOutputTypeDef(TypedDict):
    vpcId: NotRequired[str],
    subnets: NotRequired[List[str]],
    securityGroupIds: NotRequired[List[str]],
```

## BuildStatusConfigTypeDef

```python
# BuildStatusConfigTypeDef definition

class BuildStatusConfigTypeDef(TypedDict):
    context: NotRequired[str],
    targetUrl: NotRequired[str],
```

## ResolvedArtifactTypeDef

```python
# ResolvedArtifactTypeDef definition

class ResolvedArtifactTypeDef(TypedDict):
    type: NotRequired[ArtifactsTypeType],  # (1)
    location: NotRequired[str],
    identifier: NotRequired[str],
```

1. See [:material-code-brackets: ArtifactsTypeType](./literals.md#artifactstypetype) 
## DebugSessionTypeDef

```python
# DebugSessionTypeDef definition

class DebugSessionTypeDef(TypedDict):
    sessionEnabled: NotRequired[bool],
    sessionTarget: NotRequired[str],
```

## ExportedEnvironmentVariableTypeDef

```python
# ExportedEnvironmentVariableTypeDef definition

class ExportedEnvironmentVariableTypeDef(TypedDict):
    name: NotRequired[str],
    value: NotRequired[str],
```

## NetworkInterfaceTypeDef

```python
# NetworkInterfaceTypeDef definition

class NetworkInterfaceTypeDef(TypedDict):
    subnetId: NotRequired[str],
    networkInterfaceId: NotRequired[str],
```

## CloudWatchLogsConfigTypeDef

```python
# CloudWatchLogsConfigTypeDef definition

class CloudWatchLogsConfigTypeDef(TypedDict):
    status: LogsConfigStatusTypeType,  # (1)
    groupName: NotRequired[str],
    streamName: NotRequired[str],
```

1. See [:material-code-brackets: LogsConfigStatusTypeType](./literals.md#logsconfigstatustypetype) 
## CodeCoverageReportSummaryTypeDef

```python
# CodeCoverageReportSummaryTypeDef definition

class CodeCoverageReportSummaryTypeDef(TypedDict):
    lineCoveragePercentage: NotRequired[float],
    linesCovered: NotRequired[int],
    linesMissed: NotRequired[int],
    branchCoveragePercentage: NotRequired[float],
    branchesCovered: NotRequired[int],
    branchesMissed: NotRequired[int],
```

## CodeCoverageTypeDef

```python
# CodeCoverageTypeDef definition

class CodeCoverageTypeDef(TypedDict):
    id: NotRequired[str],
    reportARN: NotRequired[str],
    filePath: NotRequired[str],
    lineCoveragePercentage: NotRequired[float],
    linesCovered: NotRequired[int],
    linesMissed: NotRequired[int],
    branchCoveragePercentage: NotRequired[float],
    branchesCovered: NotRequired[int],
    branchesMissed: NotRequired[int],
    expired: NotRequired[datetime],
```

## ComputeConfigurationTypeDef

```python
# ComputeConfigurationTypeDef definition

class ComputeConfigurationTypeDef(TypedDict):
    vCpu: NotRequired[int],
    memory: NotRequired[int],
    disk: NotRequired[int],
    machineType: NotRequired[MachineTypeType],  # (1)
```

1. See [:material-code-brackets: MachineTypeType](./literals.md#machinetypetype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: NotRequired[str],
    value: NotRequired[str],
```

## VpcConfigTypeDef

```python
# VpcConfigTypeDef definition

class VpcConfigTypeDef(TypedDict):
    vpcId: NotRequired[str],
    subnets: NotRequired[Sequence[str]],
    securityGroupIds: NotRequired[Sequence[str]],
```

## ProjectArtifactsTypeDef

```python
# ProjectArtifactsTypeDef definition

class ProjectArtifactsTypeDef(TypedDict):
    type: ArtifactsTypeType,  # (1)
    location: NotRequired[str],
    path: NotRequired[str],
    namespaceType: NotRequired[ArtifactNamespaceType],  # (2)
    name: NotRequired[str],
    packaging: NotRequired[ArtifactPackagingType],  # (3)
    overrideArtifactName: NotRequired[bool],
    encryptionDisabled: NotRequired[bool],
    artifactIdentifier: NotRequired[str],
    bucketOwnerAccess: NotRequired[BucketOwnerAccessType],  # (4)
```

1. See [:material-code-brackets: ArtifactsTypeType](./literals.md#artifactstypetype) 
2. See [:material-code-brackets: ArtifactNamespaceType](./literals.md#artifactnamespacetype) 
3. See [:material-code-brackets: ArtifactPackagingType](./literals.md#artifactpackagingtype) 
4. See [:material-code-brackets: BucketOwnerAccessType](./literals.md#bucketowneraccesstype) 
## ProjectCacheTypeDef

```python
# ProjectCacheTypeDef definition

class ProjectCacheTypeDef(TypedDict):
    type: CacheTypeType,  # (1)
    location: NotRequired[str],
    modes: NotRequired[Sequence[CacheModeType]],  # (2)
```

1. See [:material-code-brackets: CacheTypeType](./literals.md#cachetypetype) 
2. See [:material-code-brackets: CacheModeType](./literals.md#cachemodetype) 
## ScopeConfigurationTypeDef

```python
# ScopeConfigurationTypeDef definition

class ScopeConfigurationTypeDef(TypedDict):
    name: str,
    scope: WebhookScopeTypeType,  # (1)
    domain: NotRequired[str],
```

1. See [:material-code-brackets: WebhookScopeTypeType](./literals.md#webhookscopetypetype) 
## WebhookFilterTypeDef

```python
# WebhookFilterTypeDef definition

class WebhookFilterTypeDef(TypedDict):
    type: WebhookFilterTypeType,  # (1)
    pattern: str,
    excludeMatchedPattern: NotRequired[bool],
```

1. See [:material-code-brackets: WebhookFilterTypeType](./literals.md#webhookfiltertypetype) 
## DeleteBuildBatchInputRequestTypeDef

```python
# DeleteBuildBatchInputRequestTypeDef definition

class DeleteBuildBatchInputRequestTypeDef(TypedDict):
    id: str,
```

## DeleteFleetInputRequestTypeDef

```python
# DeleteFleetInputRequestTypeDef definition

class DeleteFleetInputRequestTypeDef(TypedDict):
    arn: str,
```

## DeleteProjectInputRequestTypeDef

```python
# DeleteProjectInputRequestTypeDef definition

class DeleteProjectInputRequestTypeDef(TypedDict):
    name: str,
```

## DeleteReportGroupInputRequestTypeDef

```python
# DeleteReportGroupInputRequestTypeDef definition

class DeleteReportGroupInputRequestTypeDef(TypedDict):
    arn: str,
    deleteReports: NotRequired[bool],
```

## DeleteReportInputRequestTypeDef

```python
# DeleteReportInputRequestTypeDef definition

class DeleteReportInputRequestTypeDef(TypedDict):
    arn: str,
```

## DeleteResourcePolicyInputRequestTypeDef

```python
# DeleteResourcePolicyInputRequestTypeDef definition

class DeleteResourcePolicyInputRequestTypeDef(TypedDict):
    resourceArn: str,
```

## DeleteSourceCredentialsInputRequestTypeDef

```python
# DeleteSourceCredentialsInputRequestTypeDef definition

class DeleteSourceCredentialsInputRequestTypeDef(TypedDict):
    arn: str,
```

## DeleteWebhookInputRequestTypeDef

```python
# DeleteWebhookInputRequestTypeDef definition

class DeleteWebhookInputRequestTypeDef(TypedDict):
    projectName: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeCodeCoveragesInputRequestTypeDef

```python
# DescribeCodeCoveragesInputRequestTypeDef definition

class DescribeCodeCoveragesInputRequestTypeDef(TypedDict):
    reportArn: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    sortOrder: NotRequired[SortOrderTypeType],  # (1)
    sortBy: NotRequired[ReportCodeCoverageSortByTypeType],  # (2)
    minLineCoveragePercentage: NotRequired[float],
    maxLineCoveragePercentage: NotRequired[float],
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
2. See [:material-code-brackets: ReportCodeCoverageSortByTypeType](./literals.md#reportcodecoveragesortbytypetype) 
## TestCaseFilterTypeDef

```python
# TestCaseFilterTypeDef definition

class TestCaseFilterTypeDef(TypedDict):
    status: NotRequired[str],
    keyword: NotRequired[str],
```

## TestCaseTypeDef

```python
# TestCaseTypeDef definition

class TestCaseTypeDef(TypedDict):
    reportArn: NotRequired[str],
    testRawDataPath: NotRequired[str],
    prefix: NotRequired[str],
    name: NotRequired[str],
    status: NotRequired[str],
    durationInNanoSeconds: NotRequired[int],
    message: NotRequired[str],
    expired: NotRequired[datetime],
```

## EnvironmentImageTypeDef

```python
# EnvironmentImageTypeDef definition

class EnvironmentImageTypeDef(TypedDict):
    name: NotRequired[str],
    description: NotRequired[str],
    versions: NotRequired[List[str]],
```

## EnvironmentVariableTypeDef

```python
# EnvironmentVariableTypeDef definition

class EnvironmentVariableTypeDef(TypedDict):
    name: str,
    value: str,
    type: NotRequired[EnvironmentVariableTypeType],  # (1)
```

1. See [:material-code-brackets: EnvironmentVariableTypeType](./literals.md#environmentvariabletypetype) 
## FleetProxyRuleOutputTypeDef

```python
# FleetProxyRuleOutputTypeDef definition

class FleetProxyRuleOutputTypeDef(TypedDict):
    type: FleetProxyRuleTypeType,  # (1)
    effect: FleetProxyRuleEffectTypeType,  # (2)
    entities: List[str],
```

1. See [:material-code-brackets: FleetProxyRuleTypeType](./literals.md#fleetproxyruletypetype) 
2. See [:material-code-brackets: FleetProxyRuleEffectTypeType](./literals.md#fleetproxyruleeffecttypetype) 
## FleetProxyRuleTypeDef

```python
# FleetProxyRuleTypeDef definition

class FleetProxyRuleTypeDef(TypedDict):
    type: FleetProxyRuleTypeType,  # (1)
    effect: FleetProxyRuleEffectTypeType,  # (2)
    entities: Sequence[str],
```

1. See [:material-code-brackets: FleetProxyRuleTypeType](./literals.md#fleetproxyruletypetype) 
2. See [:material-code-brackets: FleetProxyRuleEffectTypeType](./literals.md#fleetproxyruleeffecttypetype) 
## FleetStatusTypeDef

```python
# FleetStatusTypeDef definition

class FleetStatusTypeDef(TypedDict):
    statusCode: NotRequired[FleetStatusCodeType],  # (1)
    context: NotRequired[FleetContextCodeType],  # (2)
    message: NotRequired[str],
```

1. See [:material-code-brackets: FleetStatusCodeType](./literals.md#fleetstatuscodetype) 
2. See [:material-code-brackets: FleetContextCodeType](./literals.md#fleetcontextcodetype) 
## GetReportGroupTrendInputRequestTypeDef

```python
# GetReportGroupTrendInputRequestTypeDef definition

class GetReportGroupTrendInputRequestTypeDef(TypedDict):
    reportGroupArn: str,
    trendField: ReportGroupTrendFieldTypeType,  # (1)
    numOfReports: NotRequired[int],
```

1. See [:material-code-brackets: ReportGroupTrendFieldTypeType](./literals.md#reportgrouptrendfieldtypetype) 
## ReportGroupTrendStatsTypeDef

```python
# ReportGroupTrendStatsTypeDef definition

class ReportGroupTrendStatsTypeDef(TypedDict):
    average: NotRequired[str],
    max: NotRequired[str],
    min: NotRequired[str],
```

## ReportWithRawDataTypeDef

```python
# ReportWithRawDataTypeDef definition

class ReportWithRawDataTypeDef(TypedDict):
    reportArn: NotRequired[str],
    data: NotRequired[str],
```

## GetResourcePolicyInputRequestTypeDef

```python
# GetResourcePolicyInputRequestTypeDef definition

class GetResourcePolicyInputRequestTypeDef(TypedDict):
    resourceArn: str,
```

## GitSubmodulesConfigTypeDef

```python
# GitSubmodulesConfigTypeDef definition

class GitSubmodulesConfigTypeDef(TypedDict):
    fetchSubmodules: bool,
```

## ImportSourceCredentialsInputRequestTypeDef

```python
# ImportSourceCredentialsInputRequestTypeDef definition

class ImportSourceCredentialsInputRequestTypeDef(TypedDict):
    token: str,
    serverType: ServerTypeType,  # (1)
    authType: AuthTypeType,  # (2)
    username: NotRequired[str],
    shouldOverwrite: NotRequired[bool],
```

1. See [:material-code-brackets: ServerTypeType](./literals.md#servertypetype) 
2. See [:material-code-brackets: AuthTypeType](./literals.md#authtypetype) 
## InvalidateProjectCacheInputRequestTypeDef

```python
# InvalidateProjectCacheInputRequestTypeDef definition

class InvalidateProjectCacheInputRequestTypeDef(TypedDict):
    projectName: str,
```

## ListBuildsForProjectInputRequestTypeDef

```python
# ListBuildsForProjectInputRequestTypeDef definition

class ListBuildsForProjectInputRequestTypeDef(TypedDict):
    projectName: str,
    sortOrder: NotRequired[SortOrderTypeType],  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
## ListBuildsInputRequestTypeDef

```python
# ListBuildsInputRequestTypeDef definition

class ListBuildsInputRequestTypeDef(TypedDict):
    sortOrder: NotRequired[SortOrderTypeType],  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
## ListFleetsInputRequestTypeDef

```python
# ListFleetsInputRequestTypeDef definition

class ListFleetsInputRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    sortOrder: NotRequired[SortOrderTypeType],  # (1)
    sortBy: NotRequired[FleetSortByTypeType],  # (2)
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
2. See [:material-code-brackets: FleetSortByTypeType](./literals.md#fleetsortbytypetype) 
## ListProjectsInputRequestTypeDef

```python
# ListProjectsInputRequestTypeDef definition

class ListProjectsInputRequestTypeDef(TypedDict):
    sortBy: NotRequired[ProjectSortByTypeType],  # (1)
    sortOrder: NotRequired[SortOrderTypeType],  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: ProjectSortByTypeType](./literals.md#projectsortbytypetype) 
2. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
## ListReportGroupsInputRequestTypeDef

```python
# ListReportGroupsInputRequestTypeDef definition

class ListReportGroupsInputRequestTypeDef(TypedDict):
    sortOrder: NotRequired[SortOrderTypeType],  # (1)
    sortBy: NotRequired[ReportGroupSortByTypeType],  # (2)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
2. See [:material-code-brackets: ReportGroupSortByTypeType](./literals.md#reportgroupsortbytypetype) 
## ReportFilterTypeDef

```python
# ReportFilterTypeDef definition

class ReportFilterTypeDef(TypedDict):
    status: NotRequired[ReportStatusTypeType],  # (1)
```

1. See [:material-code-brackets: ReportStatusTypeType](./literals.md#reportstatustypetype) 
## ListSharedProjectsInputRequestTypeDef

```python
# ListSharedProjectsInputRequestTypeDef definition

class ListSharedProjectsInputRequestTypeDef(TypedDict):
    sortBy: NotRequired[SharedResourceSortByTypeType],  # (1)
    sortOrder: NotRequired[SortOrderTypeType],  # (2)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: SharedResourceSortByTypeType](./literals.md#sharedresourcesortbytypetype) 
2. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
## ListSharedReportGroupsInputRequestTypeDef

```python
# ListSharedReportGroupsInputRequestTypeDef definition

class ListSharedReportGroupsInputRequestTypeDef(TypedDict):
    sortOrder: NotRequired[SortOrderTypeType],  # (1)
    sortBy: NotRequired[SharedResourceSortByTypeType],  # (2)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
2. See [:material-code-brackets: SharedResourceSortByTypeType](./literals.md#sharedresourcesortbytypetype) 
## SourceCredentialsInfoTypeDef

```python
# SourceCredentialsInfoTypeDef definition

class SourceCredentialsInfoTypeDef(TypedDict):
    arn: NotRequired[str],
    serverType: NotRequired[ServerTypeType],  # (1)
    authType: NotRequired[AuthTypeType],  # (2)
    resource: NotRequired[str],
```

1. See [:material-code-brackets: ServerTypeType](./literals.md#servertypetype) 
2. See [:material-code-brackets: AuthTypeType](./literals.md#authtypetype) 
## S3LogsConfigTypeDef

```python
# S3LogsConfigTypeDef definition

class S3LogsConfigTypeDef(TypedDict):
    status: LogsConfigStatusTypeType,  # (1)
    location: NotRequired[str],
    encryptionDisabled: NotRequired[bool],
    bucketOwnerAccess: NotRequired[BucketOwnerAccessType],  # (2)
```

1. See [:material-code-brackets: LogsConfigStatusTypeType](./literals.md#logsconfigstatustypetype) 
2. See [:material-code-brackets: BucketOwnerAccessType](./literals.md#bucketowneraccesstype) 
## ProjectBadgeTypeDef

```python
# ProjectBadgeTypeDef definition

class ProjectBadgeTypeDef(TypedDict):
    badgeEnabled: NotRequired[bool],
    badgeRequestUrl: NotRequired[str],
```

## ProjectFleetTypeDef

```python
# ProjectFleetTypeDef definition

class ProjectFleetTypeDef(TypedDict):
    fleetArn: NotRequired[str],
```

## RegistryCredentialTypeDef

```python
# RegistryCredentialTypeDef definition

class RegistryCredentialTypeDef(TypedDict):
    credential: str,
    credentialProvider: CredentialProviderTypeType,  # (1)
```

1. See [:material-code-brackets: CredentialProviderTypeType](./literals.md#credentialprovidertypetype) 
## SourceAuthTypeDef

```python
# SourceAuthTypeDef definition

class SourceAuthTypeDef(TypedDict):
    type: SourceAuthTypeType,  # (1)
    resource: NotRequired[str],
```

1. See [:material-code-brackets: SourceAuthTypeType](./literals.md#sourceauthtypetype) 
## PutResourcePolicyInputRequestTypeDef

```python
# PutResourcePolicyInputRequestTypeDef definition

class PutResourcePolicyInputRequestTypeDef(TypedDict):
    policy: str,
    resourceArn: str,
```

## S3ReportExportConfigTypeDef

```python
# S3ReportExportConfigTypeDef definition

class S3ReportExportConfigTypeDef(TypedDict):
    bucket: NotRequired[str],
    bucketOwner: NotRequired[str],
    path: NotRequired[str],
    packaging: NotRequired[ReportPackagingTypeType],  # (1)
    encryptionKey: NotRequired[str],
    encryptionDisabled: NotRequired[bool],
```

1. See [:material-code-brackets: ReportPackagingTypeType](./literals.md#reportpackagingtypetype) 
## TestReportSummaryTypeDef

```python
# TestReportSummaryTypeDef definition

class TestReportSummaryTypeDef(TypedDict):
    total: int,
    statusCounts: Dict[str, int],
    durationInNanoSeconds: int,
```

## RetryBuildBatchInputRequestTypeDef

```python
# RetryBuildBatchInputRequestTypeDef definition

class RetryBuildBatchInputRequestTypeDef(TypedDict):
    id: NotRequired[str],
    idempotencyToken: NotRequired[str],
    retryType: NotRequired[RetryBuildBatchTypeType],  # (1)
```

1. See [:material-code-brackets: RetryBuildBatchTypeType](./literals.md#retrybuildbatchtypetype) 
## RetryBuildInputRequestTypeDef

```python
# RetryBuildInputRequestTypeDef definition

class RetryBuildInputRequestTypeDef(TypedDict):
    id: NotRequired[str],
    idempotencyToken: NotRequired[str],
```

## TargetTrackingScalingConfigurationTypeDef

```python
# TargetTrackingScalingConfigurationTypeDef definition

class TargetTrackingScalingConfigurationTypeDef(TypedDict):
    metricType: NotRequired[FleetScalingMetricTypeType],  # (1)
    targetValue: NotRequired[float],
```

1. See [:material-code-brackets: FleetScalingMetricTypeType](./literals.md#fleetscalingmetrictypetype) 
## StopBuildBatchInputRequestTypeDef

```python
# StopBuildBatchInputRequestTypeDef definition

class StopBuildBatchInputRequestTypeDef(TypedDict):
    id: str,
```

## StopBuildInputRequestTypeDef

```python
# StopBuildInputRequestTypeDef definition

class StopBuildInputRequestTypeDef(TypedDict):
    id: str,
```

## UpdateProjectVisibilityInputRequestTypeDef

```python
# UpdateProjectVisibilityInputRequestTypeDef definition

class UpdateProjectVisibilityInputRequestTypeDef(TypedDict):
    projectArn: str,
    projectVisibility: ProjectVisibilityTypeType,  # (1)
    resourceAccessRole: NotRequired[str],
```

1. See [:material-code-brackets: ProjectVisibilityTypeType](./literals.md#projectvisibilitytypetype) 
## BatchDeleteBuildsOutputTypeDef

```python
# BatchDeleteBuildsOutputTypeDef definition

class BatchDeleteBuildsOutputTypeDef(TypedDict):
    buildsDeleted: List[str],
    buildsNotDeleted: List[BuildNotDeletedTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BuildNotDeletedTypeDef](./type_defs.md#buildnotdeletedtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteBuildBatchOutputTypeDef

```python
# DeleteBuildBatchOutputTypeDef definition

class DeleteBuildBatchOutputTypeDef(TypedDict):
    statusCode: str,
    buildsDeleted: List[str],
    buildsNotDeleted: List[BuildNotDeletedTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BuildNotDeletedTypeDef](./type_defs.md#buildnotdeletedtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteSourceCredentialsOutputTypeDef

```python
# DeleteSourceCredentialsOutputTypeDef definition

class DeleteSourceCredentialsOutputTypeDef(TypedDict):
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourcePolicyOutputTypeDef

```python
# GetResourcePolicyOutputTypeDef definition

class GetResourcePolicyOutputTypeDef(TypedDict):
    policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportSourceCredentialsOutputTypeDef

```python
# ImportSourceCredentialsOutputTypeDef definition

class ImportSourceCredentialsOutputTypeDef(TypedDict):
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBuildBatchesForProjectOutputTypeDef

```python
# ListBuildBatchesForProjectOutputTypeDef definition

class ListBuildBatchesForProjectOutputTypeDef(TypedDict):
    ids: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBuildBatchesOutputTypeDef

```python
# ListBuildBatchesOutputTypeDef definition

class ListBuildBatchesOutputTypeDef(TypedDict):
    ids: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBuildsForProjectOutputTypeDef

```python
# ListBuildsForProjectOutputTypeDef definition

class ListBuildsForProjectOutputTypeDef(TypedDict):
    ids: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBuildsOutputTypeDef

```python
# ListBuildsOutputTypeDef definition

class ListBuildsOutputTypeDef(TypedDict):
    ids: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFleetsOutputTypeDef

```python
# ListFleetsOutputTypeDef definition

class ListFleetsOutputTypeDef(TypedDict):
    fleets: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProjectsOutputTypeDef

```python
# ListProjectsOutputTypeDef definition

class ListProjectsOutputTypeDef(TypedDict):
    projects: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListReportGroupsOutputTypeDef

```python
# ListReportGroupsOutputTypeDef definition

class ListReportGroupsOutputTypeDef(TypedDict):
    reportGroups: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListReportsForReportGroupOutputTypeDef

```python
# ListReportsForReportGroupOutputTypeDef definition

class ListReportsForReportGroupOutputTypeDef(TypedDict):
    reports: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListReportsOutputTypeDef

```python
# ListReportsOutputTypeDef definition

class ListReportsOutputTypeDef(TypedDict):
    reports: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSharedProjectsOutputTypeDef

```python
# ListSharedProjectsOutputTypeDef definition

class ListSharedProjectsOutputTypeDef(TypedDict):
    projects: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSharedReportGroupsOutputTypeDef

```python
# ListSharedReportGroupsOutputTypeDef definition

class ListSharedReportGroupsOutputTypeDef(TypedDict):
    reportGroups: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutResourcePolicyOutputTypeDef

```python
# PutResourcePolicyOutputTypeDef definition

class PutResourcePolicyOutputTypeDef(TypedDict):
    resourceArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProjectVisibilityOutputTypeDef

```python
# UpdateProjectVisibilityOutputTypeDef definition

class UpdateProjectVisibilityOutputTypeDef(TypedDict):
    projectArn: str,
    publicProjectAlias: str,
    projectVisibility: ProjectVisibilityTypeType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ProjectVisibilityTypeType](./literals.md#projectvisibilitytypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProjectBuildBatchConfigOutputTypeDef

```python
# ProjectBuildBatchConfigOutputTypeDef definition

class ProjectBuildBatchConfigOutputTypeDef(TypedDict):
    serviceRole: NotRequired[str],
    combineArtifacts: NotRequired[bool],
    restrictions: NotRequired[BatchRestrictionsOutputTypeDef],  # (1)
    timeoutInMins: NotRequired[int],
    batchReportMode: NotRequired[BatchReportModeTypeType],  # (2)
```

1. See [:material-code-braces: BatchRestrictionsOutputTypeDef](./type_defs.md#batchrestrictionsoutputtypedef) 
2. See [:material-code-brackets: BatchReportModeTypeType](./literals.md#batchreportmodetypetype) 
## ListBuildBatchesForProjectInputRequestTypeDef

```python
# ListBuildBatchesForProjectInputRequestTypeDef definition

class ListBuildBatchesForProjectInputRequestTypeDef(TypedDict):
    projectName: NotRequired[str],
    filter: NotRequired[BuildBatchFilterTypeDef],  # (1)
    maxResults: NotRequired[int],
    sortOrder: NotRequired[SortOrderTypeType],  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BuildBatchFilterTypeDef](./type_defs.md#buildbatchfiltertypedef) 
2. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
## ListBuildBatchesInputRequestTypeDef

```python
# ListBuildBatchesInputRequestTypeDef definition

class ListBuildBatchesInputRequestTypeDef(TypedDict):
    filter: NotRequired[BuildBatchFilterTypeDef],  # (1)
    maxResults: NotRequired[int],
    sortOrder: NotRequired[SortOrderTypeType],  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BuildBatchFilterTypeDef](./type_defs.md#buildbatchfiltertypedef) 
2. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
## BuildBatchPhaseTypeDef

```python
# BuildBatchPhaseTypeDef definition

class BuildBatchPhaseTypeDef(TypedDict):
    phaseType: NotRequired[BuildBatchPhaseTypeType],  # (1)
    phaseStatus: NotRequired[StatusTypeType],  # (2)
    startTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
    durationInSeconds: NotRequired[int],
    contexts: NotRequired[List[PhaseContextTypeDef]],  # (3)
```

1. See [:material-code-brackets: BuildBatchPhaseTypeType](./literals.md#buildbatchphasetypetype) 
2. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
3. See [:material-code-braces: PhaseContextTypeDef](./type_defs.md#phasecontexttypedef) 
## BuildPhaseTypeDef

```python
# BuildPhaseTypeDef definition

class BuildPhaseTypeDef(TypedDict):
    phaseType: NotRequired[BuildPhaseTypeType],  # (1)
    phaseStatus: NotRequired[StatusTypeType],  # (2)
    startTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
    durationInSeconds: NotRequired[int],
    contexts: NotRequired[List[PhaseContextTypeDef]],  # (3)
```

1. See [:material-code-brackets: BuildPhaseTypeType](./literals.md#buildphasetypetype) 
2. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
3. See [:material-code-braces: PhaseContextTypeDef](./type_defs.md#phasecontexttypedef) 
## BuildSummaryTypeDef

```python
# BuildSummaryTypeDef definition

class BuildSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    requestedOn: NotRequired[datetime],
    buildStatus: NotRequired[StatusTypeType],  # (1)
    primaryArtifact: NotRequired[ResolvedArtifactTypeDef],  # (2)
    secondaryArtifacts: NotRequired[List[ResolvedArtifactTypeDef]],  # (3)
```

1. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
2. See [:material-code-braces: ResolvedArtifactTypeDef](./type_defs.md#resolvedartifacttypedef) 
3. See [:material-code-braces: ResolvedArtifactTypeDef](./type_defs.md#resolvedartifacttypedef) 
## DescribeCodeCoveragesOutputTypeDef

```python
# DescribeCodeCoveragesOutputTypeDef definition

class DescribeCodeCoveragesOutputTypeDef(TypedDict):
    codeCoverages: List[CodeCoverageTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CodeCoverageTypeDef](./type_defs.md#codecoveragetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWebhookInputRequestTypeDef

```python
# CreateWebhookInputRequestTypeDef definition

class CreateWebhookInputRequestTypeDef(TypedDict):
    projectName: str,
    branchFilter: NotRequired[str],
    filterGroups: NotRequired[Sequence[Sequence[WebhookFilterTypeDef]]],  # (1)
    buildType: NotRequired[WebhookBuildTypeType],  # (2)
    manualCreation: NotRequired[bool],
    scopeConfiguration: NotRequired[ScopeConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: WebhookFilterTypeDef](./type_defs.md#webhookfiltertypedef) 
2. See [:material-code-brackets: WebhookBuildTypeType](./literals.md#webhookbuildtypetype) 
3. See [:material-code-braces: ScopeConfigurationTypeDef](./type_defs.md#scopeconfigurationtypedef) 
## UpdateWebhookInputRequestTypeDef

```python
# UpdateWebhookInputRequestTypeDef definition

class UpdateWebhookInputRequestTypeDef(TypedDict):
    projectName: str,
    branchFilter: NotRequired[str],
    rotateSecret: NotRequired[bool],
    filterGroups: NotRequired[Sequence[Sequence[WebhookFilterTypeDef]]],  # (1)
    buildType: NotRequired[WebhookBuildTypeType],  # (2)
```

1. See [:material-code-braces: WebhookFilterTypeDef](./type_defs.md#webhookfiltertypedef) 
2. See [:material-code-brackets: WebhookBuildTypeType](./literals.md#webhookbuildtypetype) 
## WebhookTypeDef

```python
# WebhookTypeDef definition

class WebhookTypeDef(TypedDict):
    url: NotRequired[str],
    payloadUrl: NotRequired[str],
    secret: NotRequired[str],
    branchFilter: NotRequired[str],
    filterGroups: NotRequired[List[List[WebhookFilterTypeDef]]],  # (1)
    buildType: NotRequired[WebhookBuildTypeType],  # (2)
    manualCreation: NotRequired[bool],
    lastModifiedSecret: NotRequired[datetime],
    scopeConfiguration: NotRequired[ScopeConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: WebhookFilterTypeDef](./type_defs.md#webhookfiltertypedef) 
2. See [:material-code-brackets: WebhookBuildTypeType](./literals.md#webhookbuildtypetype) 
3. See [:material-code-braces: ScopeConfigurationTypeDef](./type_defs.md#scopeconfigurationtypedef) 
## DescribeCodeCoveragesInputPaginateTypeDef

```python
# DescribeCodeCoveragesInputPaginateTypeDef definition

class DescribeCodeCoveragesInputPaginateTypeDef(TypedDict):
    reportArn: str,
    sortOrder: NotRequired[SortOrderTypeType],  # (1)
    sortBy: NotRequired[ReportCodeCoverageSortByTypeType],  # (2)
    minLineCoveragePercentage: NotRequired[float],
    maxLineCoveragePercentage: NotRequired[float],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
2. See [:material-code-brackets: ReportCodeCoverageSortByTypeType](./literals.md#reportcodecoveragesortbytypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBuildBatchesForProjectInputPaginateTypeDef

```python
# ListBuildBatchesForProjectInputPaginateTypeDef definition

class ListBuildBatchesForProjectInputPaginateTypeDef(TypedDict):
    projectName: NotRequired[str],
    filter: NotRequired[BuildBatchFilterTypeDef],  # (1)
    sortOrder: NotRequired[SortOrderTypeType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: BuildBatchFilterTypeDef](./type_defs.md#buildbatchfiltertypedef) 
2. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBuildBatchesInputPaginateTypeDef

```python
# ListBuildBatchesInputPaginateTypeDef definition

class ListBuildBatchesInputPaginateTypeDef(TypedDict):
    filter: NotRequired[BuildBatchFilterTypeDef],  # (1)
    sortOrder: NotRequired[SortOrderTypeType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: BuildBatchFilterTypeDef](./type_defs.md#buildbatchfiltertypedef) 
2. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBuildsForProjectInputPaginateTypeDef

```python
# ListBuildsForProjectInputPaginateTypeDef definition

class ListBuildsForProjectInputPaginateTypeDef(TypedDict):
    projectName: str,
    sortOrder: NotRequired[SortOrderTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBuildsInputPaginateTypeDef

```python
# ListBuildsInputPaginateTypeDef definition

class ListBuildsInputPaginateTypeDef(TypedDict):
    sortOrder: NotRequired[SortOrderTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProjectsInputPaginateTypeDef

```python
# ListProjectsInputPaginateTypeDef definition

class ListProjectsInputPaginateTypeDef(TypedDict):
    sortBy: NotRequired[ProjectSortByTypeType],  # (1)
    sortOrder: NotRequired[SortOrderTypeType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ProjectSortByTypeType](./literals.md#projectsortbytypetype) 
2. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListReportGroupsInputPaginateTypeDef

```python
# ListReportGroupsInputPaginateTypeDef definition

class ListReportGroupsInputPaginateTypeDef(TypedDict):
    sortOrder: NotRequired[SortOrderTypeType],  # (1)
    sortBy: NotRequired[ReportGroupSortByTypeType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
2. See [:material-code-brackets: ReportGroupSortByTypeType](./literals.md#reportgroupsortbytypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSharedProjectsInputPaginateTypeDef

```python
# ListSharedProjectsInputPaginateTypeDef definition

class ListSharedProjectsInputPaginateTypeDef(TypedDict):
    sortBy: NotRequired[SharedResourceSortByTypeType],  # (1)
    sortOrder: NotRequired[SortOrderTypeType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SharedResourceSortByTypeType](./literals.md#sharedresourcesortbytypetype) 
2. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSharedReportGroupsInputPaginateTypeDef

```python
# ListSharedReportGroupsInputPaginateTypeDef definition

class ListSharedReportGroupsInputPaginateTypeDef(TypedDict):
    sortOrder: NotRequired[SortOrderTypeType],  # (1)
    sortBy: NotRequired[SharedResourceSortByTypeType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
2. See [:material-code-brackets: SharedResourceSortByTypeType](./literals.md#sharedresourcesortbytypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeTestCasesInputPaginateTypeDef

```python
# DescribeTestCasesInputPaginateTypeDef definition

class DescribeTestCasesInputPaginateTypeDef(TypedDict):
    reportArn: str,
    filter: NotRequired[TestCaseFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: TestCaseFilterTypeDef](./type_defs.md#testcasefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeTestCasesInputRequestTypeDef

```python
# DescribeTestCasesInputRequestTypeDef definition

class DescribeTestCasesInputRequestTypeDef(TypedDict):
    reportArn: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filter: NotRequired[TestCaseFilterTypeDef],  # (1)
```

1. See [:material-code-braces: TestCaseFilterTypeDef](./type_defs.md#testcasefiltertypedef) 
## DescribeTestCasesOutputTypeDef

```python
# DescribeTestCasesOutputTypeDef definition

class DescribeTestCasesOutputTypeDef(TypedDict):
    testCases: List[TestCaseTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TestCaseTypeDef](./type_defs.md#testcasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnvironmentLanguageTypeDef

```python
# EnvironmentLanguageTypeDef definition

class EnvironmentLanguageTypeDef(TypedDict):
    language: NotRequired[LanguageTypeType],  # (1)
    images: NotRequired[List[EnvironmentImageTypeDef]],  # (2)
```

1. See [:material-code-brackets: LanguageTypeType](./literals.md#languagetypetype) 
2. See [:material-code-braces: EnvironmentImageTypeDef](./type_defs.md#environmentimagetypedef) 
## ProxyConfigurationOutputTypeDef

```python
# ProxyConfigurationOutputTypeDef definition

class ProxyConfigurationOutputTypeDef(TypedDict):
    defaultBehavior: NotRequired[FleetProxyRuleBehaviorType],  # (1)
    orderedProxyRules: NotRequired[List[FleetProxyRuleOutputTypeDef]],  # (2)
```

1. See [:material-code-brackets: FleetProxyRuleBehaviorType](./literals.md#fleetproxyrulebehaviortype) 
2. See [:material-code-braces: FleetProxyRuleOutputTypeDef](./type_defs.md#fleetproxyruleoutputtypedef) 
## GetReportGroupTrendOutputTypeDef

```python
# GetReportGroupTrendOutputTypeDef definition

class GetReportGroupTrendOutputTypeDef(TypedDict):
    stats: ReportGroupTrendStatsTypeDef,  # (1)
    rawData: List[ReportWithRawDataTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ReportGroupTrendStatsTypeDef](./type_defs.md#reportgrouptrendstatstypedef) 
2. See [:material-code-braces: ReportWithRawDataTypeDef](./type_defs.md#reportwithrawdatatypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListReportsForReportGroupInputPaginateTypeDef

```python
# ListReportsForReportGroupInputPaginateTypeDef definition

class ListReportsForReportGroupInputPaginateTypeDef(TypedDict):
    reportGroupArn: str,
    sortOrder: NotRequired[SortOrderTypeType],  # (1)
    filter: NotRequired[ReportFilterTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
2. See [:material-code-braces: ReportFilterTypeDef](./type_defs.md#reportfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListReportsForReportGroupInputRequestTypeDef

```python
# ListReportsForReportGroupInputRequestTypeDef definition

class ListReportsForReportGroupInputRequestTypeDef(TypedDict):
    reportGroupArn: str,
    nextToken: NotRequired[str],
    sortOrder: NotRequired[SortOrderTypeType],  # (1)
    maxResults: NotRequired[int],
    filter: NotRequired[ReportFilterTypeDef],  # (2)
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
2. See [:material-code-braces: ReportFilterTypeDef](./type_defs.md#reportfiltertypedef) 
## ListReportsInputPaginateTypeDef

```python
# ListReportsInputPaginateTypeDef definition

class ListReportsInputPaginateTypeDef(TypedDict):
    sortOrder: NotRequired[SortOrderTypeType],  # (1)
    filter: NotRequired[ReportFilterTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
2. See [:material-code-braces: ReportFilterTypeDef](./type_defs.md#reportfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListReportsInputRequestTypeDef

```python
# ListReportsInputRequestTypeDef definition

class ListReportsInputRequestTypeDef(TypedDict):
    sortOrder: NotRequired[SortOrderTypeType],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filter: NotRequired[ReportFilterTypeDef],  # (2)
```

1. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
2. See [:material-code-braces: ReportFilterTypeDef](./type_defs.md#reportfiltertypedef) 
## ListSourceCredentialsOutputTypeDef

```python
# ListSourceCredentialsOutputTypeDef definition

class ListSourceCredentialsOutputTypeDef(TypedDict):
    sourceCredentialsInfos: List[SourceCredentialsInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SourceCredentialsInfoTypeDef](./type_defs.md#sourcecredentialsinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LogsConfigTypeDef

```python
# LogsConfigTypeDef definition

class LogsConfigTypeDef(TypedDict):
    cloudWatchLogs: NotRequired[CloudWatchLogsConfigTypeDef],  # (1)
    s3Logs: NotRequired[S3LogsConfigTypeDef],  # (2)
```

1. See [:material-code-braces: CloudWatchLogsConfigTypeDef](./type_defs.md#cloudwatchlogsconfigtypedef) 
2. See [:material-code-braces: S3LogsConfigTypeDef](./type_defs.md#s3logsconfigtypedef) 
## LogsLocationTypeDef

```python
# LogsLocationTypeDef definition

class LogsLocationTypeDef(TypedDict):
    groupName: NotRequired[str],
    streamName: NotRequired[str],
    deepLink: NotRequired[str],
    s3DeepLink: NotRequired[str],
    cloudWatchLogsArn: NotRequired[str],
    s3LogsArn: NotRequired[str],
    cloudWatchLogs: NotRequired[CloudWatchLogsConfigTypeDef],  # (1)
    s3Logs: NotRequired[S3LogsConfigTypeDef],  # (2)
```

1. See [:material-code-braces: CloudWatchLogsConfigTypeDef](./type_defs.md#cloudwatchlogsconfigtypedef) 
2. See [:material-code-braces: S3LogsConfigTypeDef](./type_defs.md#s3logsconfigtypedef) 
## ProjectEnvironmentOutputTypeDef

```python
# ProjectEnvironmentOutputTypeDef definition

class ProjectEnvironmentOutputTypeDef(TypedDict):
    type: EnvironmentTypeType,  # (1)
    image: str,
    computeType: ComputeTypeType,  # (2)
    computeConfiguration: NotRequired[ComputeConfigurationTypeDef],  # (3)
    fleet: NotRequired[ProjectFleetTypeDef],  # (4)
    environmentVariables: NotRequired[List[EnvironmentVariableTypeDef]],  # (5)
    privilegedMode: NotRequired[bool],
    certificate: NotRequired[str],
    registryCredential: NotRequired[RegistryCredentialTypeDef],  # (6)
    imagePullCredentialsType: NotRequired[ImagePullCredentialsTypeType],  # (7)
```

1. See [:material-code-brackets: EnvironmentTypeType](./literals.md#environmenttypetype) 
2. See [:material-code-brackets: ComputeTypeType](./literals.md#computetypetype) 
3. See [:material-code-braces: ComputeConfigurationTypeDef](./type_defs.md#computeconfigurationtypedef) 
4. See [:material-code-braces: ProjectFleetTypeDef](./type_defs.md#projectfleettypedef) 
5. See [:material-code-braces: EnvironmentVariableTypeDef](./type_defs.md#environmentvariabletypedef) 
6. See [:material-code-braces: RegistryCredentialTypeDef](./type_defs.md#registrycredentialtypedef) 
7. See [:material-code-brackets: ImagePullCredentialsTypeType](./literals.md#imagepullcredentialstypetype) 
## ProjectEnvironmentTypeDef

```python
# ProjectEnvironmentTypeDef definition

class ProjectEnvironmentTypeDef(TypedDict):
    type: EnvironmentTypeType,  # (1)
    image: str,
    computeType: ComputeTypeType,  # (2)
    computeConfiguration: NotRequired[ComputeConfigurationTypeDef],  # (3)
    fleet: NotRequired[ProjectFleetTypeDef],  # (4)
    environmentVariables: NotRequired[Sequence[EnvironmentVariableTypeDef]],  # (5)
    privilegedMode: NotRequired[bool],
    certificate: NotRequired[str],
    registryCredential: NotRequired[RegistryCredentialTypeDef],  # (6)
    imagePullCredentialsType: NotRequired[ImagePullCredentialsTypeType],  # (7)
```

1. See [:material-code-brackets: EnvironmentTypeType](./literals.md#environmenttypetype) 
2. See [:material-code-brackets: ComputeTypeType](./literals.md#computetypetype) 
3. See [:material-code-braces: ComputeConfigurationTypeDef](./type_defs.md#computeconfigurationtypedef) 
4. See [:material-code-braces: ProjectFleetTypeDef](./type_defs.md#projectfleettypedef) 
5. See [:material-code-braces: EnvironmentVariableTypeDef](./type_defs.md#environmentvariabletypedef) 
6. See [:material-code-braces: RegistryCredentialTypeDef](./type_defs.md#registrycredentialtypedef) 
7. See [:material-code-brackets: ImagePullCredentialsTypeType](./literals.md#imagepullcredentialstypetype) 
## ProjectSourceTypeDef

```python
# ProjectSourceTypeDef definition

class ProjectSourceTypeDef(TypedDict):
    type: SourceTypeType,  # (1)
    location: NotRequired[str],
    gitCloneDepth: NotRequired[int],
    gitSubmodulesConfig: NotRequired[GitSubmodulesConfigTypeDef],  # (2)
    buildspec: NotRequired[str],
    auth: NotRequired[SourceAuthTypeDef],  # (3)
    reportBuildStatus: NotRequired[bool],
    buildStatusConfig: NotRequired[BuildStatusConfigTypeDef],  # (4)
    insecureSsl: NotRequired[bool],
    sourceIdentifier: NotRequired[str],
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
2. See [:material-code-braces: GitSubmodulesConfigTypeDef](./type_defs.md#gitsubmodulesconfigtypedef) 
3. See [:material-code-braces: SourceAuthTypeDef](./type_defs.md#sourceauthtypedef) 
4. See [:material-code-braces: BuildStatusConfigTypeDef](./type_defs.md#buildstatusconfigtypedef) 
## ReportExportConfigTypeDef

```python
# ReportExportConfigTypeDef definition

class ReportExportConfigTypeDef(TypedDict):
    exportConfigType: NotRequired[ReportExportConfigTypeType],  # (1)
    s3Destination: NotRequired[S3ReportExportConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ReportExportConfigTypeType](./literals.md#reportexportconfigtypetype) 
2. See [:material-code-braces: S3ReportExportConfigTypeDef](./type_defs.md#s3reportexportconfigtypedef) 
## ScalingConfigurationInputTypeDef

```python
# ScalingConfigurationInputTypeDef definition

class ScalingConfigurationInputTypeDef(TypedDict):
    scalingType: NotRequired[FleetScalingTypeType],  # (1)
    targetTrackingScalingConfigs: NotRequired[Sequence[TargetTrackingScalingConfigurationTypeDef]],  # (2)
    maxCapacity: NotRequired[int],
```

1. See [:material-code-brackets: FleetScalingTypeType](./literals.md#fleetscalingtypetype) 
2. See [:material-code-braces: TargetTrackingScalingConfigurationTypeDef](./type_defs.md#targettrackingscalingconfigurationtypedef) 
## ScalingConfigurationOutputTypeDef

```python
# ScalingConfigurationOutputTypeDef definition

class ScalingConfigurationOutputTypeDef(TypedDict):
    scalingType: NotRequired[FleetScalingTypeType],  # (1)
    targetTrackingScalingConfigs: NotRequired[List[TargetTrackingScalingConfigurationTypeDef]],  # (2)
    maxCapacity: NotRequired[int],
    desiredCapacity: NotRequired[int],
```

1. See [:material-code-brackets: FleetScalingTypeType](./literals.md#fleetscalingtypetype) 
2. See [:material-code-braces: TargetTrackingScalingConfigurationTypeDef](./type_defs.md#targettrackingscalingconfigurationtypedef) 
## ProjectBuildBatchConfigTypeDef

```python
# ProjectBuildBatchConfigTypeDef definition

class ProjectBuildBatchConfigTypeDef(TypedDict):
    serviceRole: NotRequired[str],
    combineArtifacts: NotRequired[bool],
    restrictions: NotRequired[BatchRestrictionsUnionTypeDef],  # (1)
    timeoutInMins: NotRequired[int],
    batchReportMode: NotRequired[BatchReportModeTypeType],  # (2)
```

1. See [:material-code-braces: BatchRestrictionsTypeDef](./type_defs.md#batchrestrictionstypedef) [:material-code-braces: BatchRestrictionsOutputTypeDef](./type_defs.md#batchrestrictionsoutputtypedef) 
2. See [:material-code-brackets: BatchReportModeTypeType](./literals.md#batchreportmodetypetype) 
## BuildGroupTypeDef

```python
# BuildGroupTypeDef definition

class BuildGroupTypeDef(TypedDict):
    identifier: NotRequired[str],
    dependsOn: NotRequired[List[str]],
    ignoreFailure: NotRequired[bool],
    currentBuildSummary: NotRequired[BuildSummaryTypeDef],  # (1)
    priorBuildSummaryList: NotRequired[List[BuildSummaryTypeDef]],  # (2)
```

1. See [:material-code-braces: BuildSummaryTypeDef](./type_defs.md#buildsummarytypedef) 
2. See [:material-code-braces: BuildSummaryTypeDef](./type_defs.md#buildsummarytypedef) 
## CreateWebhookOutputTypeDef

```python
# CreateWebhookOutputTypeDef definition

class CreateWebhookOutputTypeDef(TypedDict):
    webhook: WebhookTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WebhookTypeDef](./type_defs.md#webhooktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWebhookOutputTypeDef

```python
# UpdateWebhookOutputTypeDef definition

class UpdateWebhookOutputTypeDef(TypedDict):
    webhook: WebhookTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WebhookTypeDef](./type_defs.md#webhooktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnvironmentPlatformTypeDef

```python
# EnvironmentPlatformTypeDef definition

class EnvironmentPlatformTypeDef(TypedDict):
    platform: NotRequired[PlatformTypeType],  # (1)
    languages: NotRequired[List[EnvironmentLanguageTypeDef]],  # (2)
```

1. See [:material-code-brackets: PlatformTypeType](./literals.md#platformtypetype) 
2. See [:material-code-braces: EnvironmentLanguageTypeDef](./type_defs.md#environmentlanguagetypedef) 
## ProxyConfigurationTypeDef

```python
# ProxyConfigurationTypeDef definition

class ProxyConfigurationTypeDef(TypedDict):
    defaultBehavior: NotRequired[FleetProxyRuleBehaviorType],  # (1)
    orderedProxyRules: NotRequired[Sequence[FleetProxyRuleUnionTypeDef]],  # (2)
```

1. See [:material-code-brackets: FleetProxyRuleBehaviorType](./literals.md#fleetproxyrulebehaviortype) 
2. See [:material-code-braces: FleetProxyRuleTypeDef](./type_defs.md#fleetproxyruletypedef) [:material-code-braces: FleetProxyRuleOutputTypeDef](./type_defs.md#fleetproxyruleoutputtypedef) 
## BuildTypeDef

```python
# BuildTypeDef definition

class BuildTypeDef(TypedDict):
    id: NotRequired[str],
    arn: NotRequired[str],
    buildNumber: NotRequired[int],
    startTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
    currentPhase: NotRequired[str],
    buildStatus: NotRequired[StatusTypeType],  # (1)
    sourceVersion: NotRequired[str],
    resolvedSourceVersion: NotRequired[str],
    projectName: NotRequired[str],
    phases: NotRequired[List[BuildPhaseTypeDef]],  # (2)
    source: NotRequired[ProjectSourceTypeDef],  # (3)
    secondarySources: NotRequired[List[ProjectSourceTypeDef]],  # (4)
    secondarySourceVersions: NotRequired[List[ProjectSourceVersionTypeDef]],  # (5)
    artifacts: NotRequired[BuildArtifactsTypeDef],  # (6)
    secondaryArtifacts: NotRequired[List[BuildArtifactsTypeDef]],  # (7)
    cache: NotRequired[ProjectCacheOutputTypeDef],  # (8)
    environment: NotRequired[ProjectEnvironmentOutputTypeDef],  # (9)
    serviceRole: NotRequired[str],
    logs: NotRequired[LogsLocationTypeDef],  # (10)
    timeoutInMinutes: NotRequired[int],
    queuedTimeoutInMinutes: NotRequired[int],
    buildComplete: NotRequired[bool],
    initiator: NotRequired[str],
    vpcConfig: NotRequired[VpcConfigOutputTypeDef],  # (11)
    networkInterface: NotRequired[NetworkInterfaceTypeDef],  # (12)
    encryptionKey: NotRequired[str],
    exportedEnvironmentVariables: NotRequired[List[ExportedEnvironmentVariableTypeDef]],  # (13)
    reportArns: NotRequired[List[str]],
    fileSystemLocations: NotRequired[List[ProjectFileSystemLocationTypeDef]],  # (14)
    debugSession: NotRequired[DebugSessionTypeDef],  # (15)
    buildBatchArn: NotRequired[str],
    autoRetryConfig: NotRequired[AutoRetryConfigTypeDef],  # (16)
```

1. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
2. See [:material-code-braces: BuildPhaseTypeDef](./type_defs.md#buildphasetypedef) 
3. See [:material-code-braces: ProjectSourceTypeDef](./type_defs.md#projectsourcetypedef) 
4. See [:material-code-braces: ProjectSourceTypeDef](./type_defs.md#projectsourcetypedef) 
5. See [:material-code-braces: ProjectSourceVersionTypeDef](./type_defs.md#projectsourceversiontypedef) 
6. See [:material-code-braces: BuildArtifactsTypeDef](./type_defs.md#buildartifactstypedef) 
7. See [:material-code-braces: BuildArtifactsTypeDef](./type_defs.md#buildartifactstypedef) 
8. See [:material-code-braces: ProjectCacheOutputTypeDef](./type_defs.md#projectcacheoutputtypedef) 
9. See [:material-code-braces: ProjectEnvironmentOutputTypeDef](./type_defs.md#projectenvironmentoutputtypedef) 
10. See [:material-code-braces: LogsLocationTypeDef](./type_defs.md#logslocationtypedef) 
11. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
12. See [:material-code-braces: NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef) 
13. See [:material-code-braces: ExportedEnvironmentVariableTypeDef](./type_defs.md#exportedenvironmentvariabletypedef) 
14. See [:material-code-braces: ProjectFileSystemLocationTypeDef](./type_defs.md#projectfilesystemlocationtypedef) 
15. See [:material-code-braces: DebugSessionTypeDef](./type_defs.md#debugsessiontypedef) 
16. See [:material-code-braces: AutoRetryConfigTypeDef](./type_defs.md#autoretryconfigtypedef) 
## ProjectTypeDef

```python
# ProjectTypeDef definition

class ProjectTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
    description: NotRequired[str],
    source: NotRequired[ProjectSourceTypeDef],  # (1)
    secondarySources: NotRequired[List[ProjectSourceTypeDef]],  # (2)
    sourceVersion: NotRequired[str],
    secondarySourceVersions: NotRequired[List[ProjectSourceVersionTypeDef]],  # (3)
    artifacts: NotRequired[ProjectArtifactsTypeDef],  # (4)
    secondaryArtifacts: NotRequired[List[ProjectArtifactsTypeDef]],  # (5)
    cache: NotRequired[ProjectCacheOutputTypeDef],  # (6)
    environment: NotRequired[ProjectEnvironmentOutputTypeDef],  # (7)
    serviceRole: NotRequired[str],
    timeoutInMinutes: NotRequired[int],
    queuedTimeoutInMinutes: NotRequired[int],
    encryptionKey: NotRequired[str],
    tags: NotRequired[List[TagTypeDef]],  # (8)
    created: NotRequired[datetime],
    lastModified: NotRequired[datetime],
    webhook: NotRequired[WebhookTypeDef],  # (9)
    vpcConfig: NotRequired[VpcConfigOutputTypeDef],  # (10)
    badge: NotRequired[ProjectBadgeTypeDef],  # (11)
    logsConfig: NotRequired[LogsConfigTypeDef],  # (12)
    fileSystemLocations: NotRequired[List[ProjectFileSystemLocationTypeDef]],  # (13)
    buildBatchConfig: NotRequired[ProjectBuildBatchConfigOutputTypeDef],  # (14)
    concurrentBuildLimit: NotRequired[int],
    projectVisibility: NotRequired[ProjectVisibilityTypeType],  # (15)
    publicProjectAlias: NotRequired[str],
    resourceAccessRole: NotRequired[str],
    autoRetryLimit: NotRequired[int],
```

1. See [:material-code-braces: ProjectSourceTypeDef](./type_defs.md#projectsourcetypedef) 
2. See [:material-code-braces: ProjectSourceTypeDef](./type_defs.md#projectsourcetypedef) 
3. See [:material-code-braces: ProjectSourceVersionTypeDef](./type_defs.md#projectsourceversiontypedef) 
4. See [:material-code-braces: ProjectArtifactsTypeDef](./type_defs.md#projectartifactstypedef) 
5. See [:material-code-braces: ProjectArtifactsTypeDef](./type_defs.md#projectartifactstypedef) 
6. See [:material-code-braces: ProjectCacheOutputTypeDef](./type_defs.md#projectcacheoutputtypedef) 
7. See [:material-code-braces: ProjectEnvironmentOutputTypeDef](./type_defs.md#projectenvironmentoutputtypedef) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
9. See [:material-code-braces: WebhookTypeDef](./type_defs.md#webhooktypedef) 
10. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
11. See [:material-code-braces: ProjectBadgeTypeDef](./type_defs.md#projectbadgetypedef) 
12. See [:material-code-braces: LogsConfigTypeDef](./type_defs.md#logsconfigtypedef) 
13. See [:material-code-braces: ProjectFileSystemLocationTypeDef](./type_defs.md#projectfilesystemlocationtypedef) 
14. See [:material-code-braces: ProjectBuildBatchConfigOutputTypeDef](./type_defs.md#projectbuildbatchconfigoutputtypedef) 
15. See [:material-code-brackets: ProjectVisibilityTypeType](./literals.md#projectvisibilitytypetype) 
## StartBuildInputRequestTypeDef

```python
# StartBuildInputRequestTypeDef definition

class StartBuildInputRequestTypeDef(TypedDict):
    projectName: str,
    secondarySourcesOverride: NotRequired[Sequence[ProjectSourceTypeDef]],  # (1)
    secondarySourcesVersionOverride: NotRequired[Sequence[ProjectSourceVersionTypeDef]],  # (2)
    sourceVersion: NotRequired[str],
    artifactsOverride: NotRequired[ProjectArtifactsTypeDef],  # (3)
    secondaryArtifactsOverride: NotRequired[Sequence[ProjectArtifactsTypeDef]],  # (4)
    environmentVariablesOverride: NotRequired[Sequence[EnvironmentVariableTypeDef]],  # (5)
    sourceTypeOverride: NotRequired[SourceTypeType],  # (6)
    sourceLocationOverride: NotRequired[str],
    sourceAuthOverride: NotRequired[SourceAuthTypeDef],  # (7)
    gitCloneDepthOverride: NotRequired[int],
    gitSubmodulesConfigOverride: NotRequired[GitSubmodulesConfigTypeDef],  # (8)
    buildspecOverride: NotRequired[str],
    insecureSslOverride: NotRequired[bool],
    reportBuildStatusOverride: NotRequired[bool],
    buildStatusConfigOverride: NotRequired[BuildStatusConfigTypeDef],  # (9)
    environmentTypeOverride: NotRequired[EnvironmentTypeType],  # (10)
    imageOverride: NotRequired[str],
    computeTypeOverride: NotRequired[ComputeTypeType],  # (11)
    certificateOverride: NotRequired[str],
    cacheOverride: NotRequired[ProjectCacheTypeDef],  # (12)
    serviceRoleOverride: NotRequired[str],
    privilegedModeOverride: NotRequired[bool],
    timeoutInMinutesOverride: NotRequired[int],
    queuedTimeoutInMinutesOverride: NotRequired[int],
    encryptionKeyOverride: NotRequired[str],
    idempotencyToken: NotRequired[str],
    logsConfigOverride: NotRequired[LogsConfigTypeDef],  # (13)
    registryCredentialOverride: NotRequired[RegistryCredentialTypeDef],  # (14)
    imagePullCredentialsTypeOverride: NotRequired[ImagePullCredentialsTypeType],  # (15)
    debugSessionEnabled: NotRequired[bool],
    fleetOverride: NotRequired[ProjectFleetTypeDef],  # (16)
    autoRetryLimitOverride: NotRequired[int],
```

1. See [:material-code-braces: ProjectSourceTypeDef](./type_defs.md#projectsourcetypedef) 
2. See [:material-code-braces: ProjectSourceVersionTypeDef](./type_defs.md#projectsourceversiontypedef) 
3. See [:material-code-braces: ProjectArtifactsTypeDef](./type_defs.md#projectartifactstypedef) 
4. See [:material-code-braces: ProjectArtifactsTypeDef](./type_defs.md#projectartifactstypedef) 
5. See [:material-code-braces: EnvironmentVariableTypeDef](./type_defs.md#environmentvariabletypedef) 
6. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
7. See [:material-code-braces: SourceAuthTypeDef](./type_defs.md#sourceauthtypedef) 
8. See [:material-code-braces: GitSubmodulesConfigTypeDef](./type_defs.md#gitsubmodulesconfigtypedef) 
9. See [:material-code-braces: BuildStatusConfigTypeDef](./type_defs.md#buildstatusconfigtypedef) 
10. See [:material-code-brackets: EnvironmentTypeType](./literals.md#environmenttypetype) 
11. See [:material-code-brackets: ComputeTypeType](./literals.md#computetypetype) 
12. See [:material-code-braces: ProjectCacheTypeDef](./type_defs.md#projectcachetypedef) 
13. See [:material-code-braces: LogsConfigTypeDef](./type_defs.md#logsconfigtypedef) 
14. See [:material-code-braces: RegistryCredentialTypeDef](./type_defs.md#registrycredentialtypedef) 
15. See [:material-code-brackets: ImagePullCredentialsTypeType](./literals.md#imagepullcredentialstypetype) 
16. See [:material-code-braces: ProjectFleetTypeDef](./type_defs.md#projectfleettypedef) 
## CreateReportGroupInputRequestTypeDef

```python
# CreateReportGroupInputRequestTypeDef definition

class CreateReportGroupInputRequestTypeDef(TypedDict):
    name: str,
    type: ReportTypeType,  # (1)
    exportConfig: ReportExportConfigTypeDef,  # (2)
    tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-brackets: ReportTypeType](./literals.md#reporttypetype) 
2. See [:material-code-braces: ReportExportConfigTypeDef](./type_defs.md#reportexportconfigtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ReportGroupTypeDef

```python
# ReportGroupTypeDef definition

class ReportGroupTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    type: NotRequired[ReportTypeType],  # (1)
    exportConfig: NotRequired[ReportExportConfigTypeDef],  # (2)
    created: NotRequired[datetime],
    lastModified: NotRequired[datetime],
    tags: NotRequired[List[TagTypeDef]],  # (3)
    status: NotRequired[ReportGroupStatusTypeType],  # (4)
```

1. See [:material-code-brackets: ReportTypeType](./literals.md#reporttypetype) 
2. See [:material-code-braces: ReportExportConfigTypeDef](./type_defs.md#reportexportconfigtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-brackets: ReportGroupStatusTypeType](./literals.md#reportgroupstatustypetype) 
## ReportTypeDef

```python
# ReportTypeDef definition

class ReportTypeDef(TypedDict):
    arn: NotRequired[str],
    type: NotRequired[ReportTypeType],  # (1)
    name: NotRequired[str],
    reportGroupArn: NotRequired[str],
    executionId: NotRequired[str],
    status: NotRequired[ReportStatusTypeType],  # (2)
    created: NotRequired[datetime],
    expired: NotRequired[datetime],
    exportConfig: NotRequired[ReportExportConfigTypeDef],  # (3)
    truncated: NotRequired[bool],
    testSummary: NotRequired[TestReportSummaryTypeDef],  # (4)
    codeCoverageSummary: NotRequired[CodeCoverageReportSummaryTypeDef],  # (5)
```

1. See [:material-code-brackets: ReportTypeType](./literals.md#reporttypetype) 
2. See [:material-code-brackets: ReportStatusTypeType](./literals.md#reportstatustypetype) 
3. See [:material-code-braces: ReportExportConfigTypeDef](./type_defs.md#reportexportconfigtypedef) 
4. See [:material-code-braces: TestReportSummaryTypeDef](./type_defs.md#testreportsummarytypedef) 
5. See [:material-code-braces: CodeCoverageReportSummaryTypeDef](./type_defs.md#codecoveragereportsummarytypedef) 
## UpdateReportGroupInputRequestTypeDef

```python
# UpdateReportGroupInputRequestTypeDef definition

class UpdateReportGroupInputRequestTypeDef(TypedDict):
    arn: str,
    exportConfig: NotRequired[ReportExportConfigTypeDef],  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: ReportExportConfigTypeDef](./type_defs.md#reportexportconfigtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## FleetTypeDef

```python
# FleetTypeDef definition

class FleetTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    id: NotRequired[str],
    created: NotRequired[datetime],
    lastModified: NotRequired[datetime],
    status: NotRequired[FleetStatusTypeDef],  # (1)
    baseCapacity: NotRequired[int],
    environmentType: NotRequired[EnvironmentTypeType],  # (2)
    computeType: NotRequired[ComputeTypeType],  # (3)
    computeConfiguration: NotRequired[ComputeConfigurationTypeDef],  # (4)
    scalingConfiguration: NotRequired[ScalingConfigurationOutputTypeDef],  # (5)
    overflowBehavior: NotRequired[FleetOverflowBehaviorType],  # (6)
    vpcConfig: NotRequired[VpcConfigOutputTypeDef],  # (7)
    proxyConfiguration: NotRequired[ProxyConfigurationOutputTypeDef],  # (8)
    imageId: NotRequired[str],
    fleetServiceRole: NotRequired[str],
    tags: NotRequired[List[TagTypeDef]],  # (9)
```

1. See [:material-code-braces: FleetStatusTypeDef](./type_defs.md#fleetstatustypedef) 
2. See [:material-code-brackets: EnvironmentTypeType](./literals.md#environmenttypetype) 
3. See [:material-code-brackets: ComputeTypeType](./literals.md#computetypetype) 
4. See [:material-code-braces: ComputeConfigurationTypeDef](./type_defs.md#computeconfigurationtypedef) 
5. See [:material-code-braces: ScalingConfigurationOutputTypeDef](./type_defs.md#scalingconfigurationoutputtypedef) 
6. See [:material-code-brackets: FleetOverflowBehaviorType](./literals.md#fleetoverflowbehaviortype) 
7. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
8. See [:material-code-braces: ProxyConfigurationOutputTypeDef](./type_defs.md#proxyconfigurationoutputtypedef) 
9. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateProjectInputRequestTypeDef

```python
# CreateProjectInputRequestTypeDef definition

class CreateProjectInputRequestTypeDef(TypedDict):
    name: str,
    source: ProjectSourceTypeDef,  # (1)
    artifacts: ProjectArtifactsTypeDef,  # (2)
    environment: ProjectEnvironmentTypeDef,  # (3)
    serviceRole: str,
    description: NotRequired[str],
    secondarySources: NotRequired[Sequence[ProjectSourceTypeDef]],  # (4)
    sourceVersion: NotRequired[str],
    secondarySourceVersions: NotRequired[Sequence[ProjectSourceVersionTypeDef]],  # (5)
    secondaryArtifacts: NotRequired[Sequence[ProjectArtifactsTypeDef]],  # (6)
    cache: NotRequired[ProjectCacheTypeDef],  # (7)
    timeoutInMinutes: NotRequired[int],
    queuedTimeoutInMinutes: NotRequired[int],
    encryptionKey: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (8)
    vpcConfig: NotRequired[VpcConfigTypeDef],  # (9)
    badgeEnabled: NotRequired[bool],
    logsConfig: NotRequired[LogsConfigTypeDef],  # (10)
    fileSystemLocations: NotRequired[Sequence[ProjectFileSystemLocationTypeDef]],  # (11)
    buildBatchConfig: NotRequired[ProjectBuildBatchConfigTypeDef],  # (12)
    concurrentBuildLimit: NotRequired[int],
    autoRetryLimit: NotRequired[int],
```

1. See [:material-code-braces: ProjectSourceTypeDef](./type_defs.md#projectsourcetypedef) 
2. See [:material-code-braces: ProjectArtifactsTypeDef](./type_defs.md#projectartifactstypedef) 
3. See [:material-code-braces: ProjectEnvironmentTypeDef](./type_defs.md#projectenvironmenttypedef) 
4. See [:material-code-braces: ProjectSourceTypeDef](./type_defs.md#projectsourcetypedef) 
5. See [:material-code-braces: ProjectSourceVersionTypeDef](./type_defs.md#projectsourceversiontypedef) 
6. See [:material-code-braces: ProjectArtifactsTypeDef](./type_defs.md#projectartifactstypedef) 
7. See [:material-code-braces: ProjectCacheTypeDef](./type_defs.md#projectcachetypedef) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
9. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
10. See [:material-code-braces: LogsConfigTypeDef](./type_defs.md#logsconfigtypedef) 
11. See [:material-code-braces: ProjectFileSystemLocationTypeDef](./type_defs.md#projectfilesystemlocationtypedef) 
12. See [:material-code-braces: ProjectBuildBatchConfigTypeDef](./type_defs.md#projectbuildbatchconfigtypedef) 
## StartBuildBatchInputRequestTypeDef

```python
# StartBuildBatchInputRequestTypeDef definition

class StartBuildBatchInputRequestTypeDef(TypedDict):
    projectName: str,
    secondarySourcesOverride: NotRequired[Sequence[ProjectSourceTypeDef]],  # (1)
    secondarySourcesVersionOverride: NotRequired[Sequence[ProjectSourceVersionTypeDef]],  # (2)
    sourceVersion: NotRequired[str],
    artifactsOverride: NotRequired[ProjectArtifactsTypeDef],  # (3)
    secondaryArtifactsOverride: NotRequired[Sequence[ProjectArtifactsTypeDef]],  # (4)
    environmentVariablesOverride: NotRequired[Sequence[EnvironmentVariableTypeDef]],  # (5)
    sourceTypeOverride: NotRequired[SourceTypeType],  # (6)
    sourceLocationOverride: NotRequired[str],
    sourceAuthOverride: NotRequired[SourceAuthTypeDef],  # (7)
    gitCloneDepthOverride: NotRequired[int],
    gitSubmodulesConfigOverride: NotRequired[GitSubmodulesConfigTypeDef],  # (8)
    buildspecOverride: NotRequired[str],
    insecureSslOverride: NotRequired[bool],
    reportBuildBatchStatusOverride: NotRequired[bool],
    environmentTypeOverride: NotRequired[EnvironmentTypeType],  # (9)
    imageOverride: NotRequired[str],
    computeTypeOverride: NotRequired[ComputeTypeType],  # (10)
    certificateOverride: NotRequired[str],
    cacheOverride: NotRequired[ProjectCacheTypeDef],  # (11)
    serviceRoleOverride: NotRequired[str],
    privilegedModeOverride: NotRequired[bool],
    buildTimeoutInMinutesOverride: NotRequired[int],
    queuedTimeoutInMinutesOverride: NotRequired[int],
    encryptionKeyOverride: NotRequired[str],
    idempotencyToken: NotRequired[str],
    logsConfigOverride: NotRequired[LogsConfigTypeDef],  # (12)
    registryCredentialOverride: NotRequired[RegistryCredentialTypeDef],  # (13)
    imagePullCredentialsTypeOverride: NotRequired[ImagePullCredentialsTypeType],  # (14)
    buildBatchConfigOverride: NotRequired[ProjectBuildBatchConfigTypeDef],  # (15)
    debugSessionEnabled: NotRequired[bool],
```

1. See [:material-code-braces: ProjectSourceTypeDef](./type_defs.md#projectsourcetypedef) 
2. See [:material-code-braces: ProjectSourceVersionTypeDef](./type_defs.md#projectsourceversiontypedef) 
3. See [:material-code-braces: ProjectArtifactsTypeDef](./type_defs.md#projectartifactstypedef) 
4. See [:material-code-braces: ProjectArtifactsTypeDef](./type_defs.md#projectartifactstypedef) 
5. See [:material-code-braces: EnvironmentVariableTypeDef](./type_defs.md#environmentvariabletypedef) 
6. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
7. See [:material-code-braces: SourceAuthTypeDef](./type_defs.md#sourceauthtypedef) 
8. See [:material-code-braces: GitSubmodulesConfigTypeDef](./type_defs.md#gitsubmodulesconfigtypedef) 
9. See [:material-code-brackets: EnvironmentTypeType](./literals.md#environmenttypetype) 
10. See [:material-code-brackets: ComputeTypeType](./literals.md#computetypetype) 
11. See [:material-code-braces: ProjectCacheTypeDef](./type_defs.md#projectcachetypedef) 
12. See [:material-code-braces: LogsConfigTypeDef](./type_defs.md#logsconfigtypedef) 
13. See [:material-code-braces: RegistryCredentialTypeDef](./type_defs.md#registrycredentialtypedef) 
14. See [:material-code-brackets: ImagePullCredentialsTypeType](./literals.md#imagepullcredentialstypetype) 
15. See [:material-code-braces: ProjectBuildBatchConfigTypeDef](./type_defs.md#projectbuildbatchconfigtypedef) 
## UpdateProjectInputRequestTypeDef

```python
# UpdateProjectInputRequestTypeDef definition

class UpdateProjectInputRequestTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    source: NotRequired[ProjectSourceTypeDef],  # (1)
    secondarySources: NotRequired[Sequence[ProjectSourceTypeDef]],  # (2)
    sourceVersion: NotRequired[str],
    secondarySourceVersions: NotRequired[Sequence[ProjectSourceVersionTypeDef]],  # (3)
    artifacts: NotRequired[ProjectArtifactsTypeDef],  # (4)
    secondaryArtifacts: NotRequired[Sequence[ProjectArtifactsTypeDef]],  # (5)
    cache: NotRequired[ProjectCacheTypeDef],  # (6)
    environment: NotRequired[ProjectEnvironmentTypeDef],  # (7)
    serviceRole: NotRequired[str],
    timeoutInMinutes: NotRequired[int],
    queuedTimeoutInMinutes: NotRequired[int],
    encryptionKey: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (8)
    vpcConfig: NotRequired[VpcConfigTypeDef],  # (9)
    badgeEnabled: NotRequired[bool],
    logsConfig: NotRequired[LogsConfigTypeDef],  # (10)
    fileSystemLocations: NotRequired[Sequence[ProjectFileSystemLocationTypeDef]],  # (11)
    buildBatchConfig: NotRequired[ProjectBuildBatchConfigTypeDef],  # (12)
    concurrentBuildLimit: NotRequired[int],
    autoRetryLimit: NotRequired[int],
```

1. See [:material-code-braces: ProjectSourceTypeDef](./type_defs.md#projectsourcetypedef) 
2. See [:material-code-braces: ProjectSourceTypeDef](./type_defs.md#projectsourcetypedef) 
3. See [:material-code-braces: ProjectSourceVersionTypeDef](./type_defs.md#projectsourceversiontypedef) 
4. See [:material-code-braces: ProjectArtifactsTypeDef](./type_defs.md#projectartifactstypedef) 
5. See [:material-code-braces: ProjectArtifactsTypeDef](./type_defs.md#projectartifactstypedef) 
6. See [:material-code-braces: ProjectCacheTypeDef](./type_defs.md#projectcachetypedef) 
7. See [:material-code-braces: ProjectEnvironmentTypeDef](./type_defs.md#projectenvironmenttypedef) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
9. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
10. See [:material-code-braces: LogsConfigTypeDef](./type_defs.md#logsconfigtypedef) 
11. See [:material-code-braces: ProjectFileSystemLocationTypeDef](./type_defs.md#projectfilesystemlocationtypedef) 
12. See [:material-code-braces: ProjectBuildBatchConfigTypeDef](./type_defs.md#projectbuildbatchconfigtypedef) 
## BuildBatchTypeDef

```python
# BuildBatchTypeDef definition

class BuildBatchTypeDef(TypedDict):
    id: NotRequired[str],
    arn: NotRequired[str],
    startTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
    currentPhase: NotRequired[str],
    buildBatchStatus: NotRequired[StatusTypeType],  # (1)
    sourceVersion: NotRequired[str],
    resolvedSourceVersion: NotRequired[str],
    projectName: NotRequired[str],
    phases: NotRequired[List[BuildBatchPhaseTypeDef]],  # (2)
    source: NotRequired[ProjectSourceTypeDef],  # (3)
    secondarySources: NotRequired[List[ProjectSourceTypeDef]],  # (4)
    secondarySourceVersions: NotRequired[List[ProjectSourceVersionTypeDef]],  # (5)
    artifacts: NotRequired[BuildArtifactsTypeDef],  # (6)
    secondaryArtifacts: NotRequired[List[BuildArtifactsTypeDef]],  # (7)
    cache: NotRequired[ProjectCacheOutputTypeDef],  # (8)
    environment: NotRequired[ProjectEnvironmentOutputTypeDef],  # (9)
    serviceRole: NotRequired[str],
    logConfig: NotRequired[LogsConfigTypeDef],  # (10)
    buildTimeoutInMinutes: NotRequired[int],
    queuedTimeoutInMinutes: NotRequired[int],
    complete: NotRequired[bool],
    initiator: NotRequired[str],
    vpcConfig: NotRequired[VpcConfigOutputTypeDef],  # (11)
    encryptionKey: NotRequired[str],
    buildBatchNumber: NotRequired[int],
    fileSystemLocations: NotRequired[List[ProjectFileSystemLocationTypeDef]],  # (12)
    buildBatchConfig: NotRequired[ProjectBuildBatchConfigOutputTypeDef],  # (13)
    buildGroups: NotRequired[List[BuildGroupTypeDef]],  # (14)
    debugSessionEnabled: NotRequired[bool],
```

1. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
2. See [:material-code-braces: BuildBatchPhaseTypeDef](./type_defs.md#buildbatchphasetypedef) 
3. See [:material-code-braces: ProjectSourceTypeDef](./type_defs.md#projectsourcetypedef) 
4. See [:material-code-braces: ProjectSourceTypeDef](./type_defs.md#projectsourcetypedef) 
5. See [:material-code-braces: ProjectSourceVersionTypeDef](./type_defs.md#projectsourceversiontypedef) 
6. See [:material-code-braces: BuildArtifactsTypeDef](./type_defs.md#buildartifactstypedef) 
7. See [:material-code-braces: BuildArtifactsTypeDef](./type_defs.md#buildartifactstypedef) 
8. See [:material-code-braces: ProjectCacheOutputTypeDef](./type_defs.md#projectcacheoutputtypedef) 
9. See [:material-code-braces: ProjectEnvironmentOutputTypeDef](./type_defs.md#projectenvironmentoutputtypedef) 
10. See [:material-code-braces: LogsConfigTypeDef](./type_defs.md#logsconfigtypedef) 
11. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
12. See [:material-code-braces: ProjectFileSystemLocationTypeDef](./type_defs.md#projectfilesystemlocationtypedef) 
13. See [:material-code-braces: ProjectBuildBatchConfigOutputTypeDef](./type_defs.md#projectbuildbatchconfigoutputtypedef) 
14. See [:material-code-braces: BuildGroupTypeDef](./type_defs.md#buildgrouptypedef) 
## ListCuratedEnvironmentImagesOutputTypeDef

```python
# ListCuratedEnvironmentImagesOutputTypeDef definition

class ListCuratedEnvironmentImagesOutputTypeDef(TypedDict):
    platforms: List[EnvironmentPlatformTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentPlatformTypeDef](./type_defs.md#environmentplatformtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFleetInputRequestTypeDef

```python
# CreateFleetInputRequestTypeDef definition

class CreateFleetInputRequestTypeDef(TypedDict):
    name: str,
    baseCapacity: int,
    environmentType: EnvironmentTypeType,  # (1)
    computeType: ComputeTypeType,  # (2)
    computeConfiguration: NotRequired[ComputeConfigurationTypeDef],  # (3)
    scalingConfiguration: NotRequired[ScalingConfigurationInputTypeDef],  # (4)
    overflowBehavior: NotRequired[FleetOverflowBehaviorType],  # (5)
    vpcConfig: NotRequired[VpcConfigTypeDef],  # (6)
    proxyConfiguration: NotRequired[ProxyConfigurationTypeDef],  # (7)
    imageId: NotRequired[str],
    fleetServiceRole: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (8)
```

1. See [:material-code-brackets: EnvironmentTypeType](./literals.md#environmenttypetype) 
2. See [:material-code-brackets: ComputeTypeType](./literals.md#computetypetype) 
3. See [:material-code-braces: ComputeConfigurationTypeDef](./type_defs.md#computeconfigurationtypedef) 
4. See [:material-code-braces: ScalingConfigurationInputTypeDef](./type_defs.md#scalingconfigurationinputtypedef) 
5. See [:material-code-brackets: FleetOverflowBehaviorType](./literals.md#fleetoverflowbehaviortype) 
6. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
7. See [:material-code-braces: ProxyConfigurationTypeDef](./type_defs.md#proxyconfigurationtypedef) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateFleetInputRequestTypeDef

```python
# UpdateFleetInputRequestTypeDef definition

class UpdateFleetInputRequestTypeDef(TypedDict):
    arn: str,
    baseCapacity: NotRequired[int],
    environmentType: NotRequired[EnvironmentTypeType],  # (1)
    computeType: NotRequired[ComputeTypeType],  # (2)
    computeConfiguration: NotRequired[ComputeConfigurationTypeDef],  # (3)
    scalingConfiguration: NotRequired[ScalingConfigurationInputTypeDef],  # (4)
    overflowBehavior: NotRequired[FleetOverflowBehaviorType],  # (5)
    vpcConfig: NotRequired[VpcConfigTypeDef],  # (6)
    proxyConfiguration: NotRequired[ProxyConfigurationTypeDef],  # (7)
    imageId: NotRequired[str],
    fleetServiceRole: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (8)
```

1. See [:material-code-brackets: EnvironmentTypeType](./literals.md#environmenttypetype) 
2. See [:material-code-brackets: ComputeTypeType](./literals.md#computetypetype) 
3. See [:material-code-braces: ComputeConfigurationTypeDef](./type_defs.md#computeconfigurationtypedef) 
4. See [:material-code-braces: ScalingConfigurationInputTypeDef](./type_defs.md#scalingconfigurationinputtypedef) 
5. See [:material-code-brackets: FleetOverflowBehaviorType](./literals.md#fleetoverflowbehaviortype) 
6. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
7. See [:material-code-braces: ProxyConfigurationTypeDef](./type_defs.md#proxyconfigurationtypedef) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## BatchGetBuildsOutputTypeDef

```python
# BatchGetBuildsOutputTypeDef definition

class BatchGetBuildsOutputTypeDef(TypedDict):
    builds: List[BuildTypeDef],  # (1)
    buildsNotFound: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BuildTypeDef](./type_defs.md#buildtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RetryBuildOutputTypeDef

```python
# RetryBuildOutputTypeDef definition

class RetryBuildOutputTypeDef(TypedDict):
    build: BuildTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BuildTypeDef](./type_defs.md#buildtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartBuildOutputTypeDef

```python
# StartBuildOutputTypeDef definition

class StartBuildOutputTypeDef(TypedDict):
    build: BuildTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BuildTypeDef](./type_defs.md#buildtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopBuildOutputTypeDef

```python
# StopBuildOutputTypeDef definition

class StopBuildOutputTypeDef(TypedDict):
    build: BuildTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BuildTypeDef](./type_defs.md#buildtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetProjectsOutputTypeDef

```python
# BatchGetProjectsOutputTypeDef definition

class BatchGetProjectsOutputTypeDef(TypedDict):
    projects: List[ProjectTypeDef],  # (1)
    projectsNotFound: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProjectTypeDef](./type_defs.md#projecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProjectOutputTypeDef

```python
# CreateProjectOutputTypeDef definition

class CreateProjectOutputTypeDef(TypedDict):
    project: ProjectTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProjectTypeDef](./type_defs.md#projecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProjectOutputTypeDef

```python
# UpdateProjectOutputTypeDef definition

class UpdateProjectOutputTypeDef(TypedDict):
    project: ProjectTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProjectTypeDef](./type_defs.md#projecttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetReportGroupsOutputTypeDef

```python
# BatchGetReportGroupsOutputTypeDef definition

class BatchGetReportGroupsOutputTypeDef(TypedDict):
    reportGroups: List[ReportGroupTypeDef],  # (1)
    reportGroupsNotFound: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReportGroupTypeDef](./type_defs.md#reportgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateReportGroupOutputTypeDef

```python
# CreateReportGroupOutputTypeDef definition

class CreateReportGroupOutputTypeDef(TypedDict):
    reportGroup: ReportGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReportGroupTypeDef](./type_defs.md#reportgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateReportGroupOutputTypeDef

```python
# UpdateReportGroupOutputTypeDef definition

class UpdateReportGroupOutputTypeDef(TypedDict):
    reportGroup: ReportGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReportGroupTypeDef](./type_defs.md#reportgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetReportsOutputTypeDef

```python
# BatchGetReportsOutputTypeDef definition

class BatchGetReportsOutputTypeDef(TypedDict):
    reports: List[ReportTypeDef],  # (1)
    reportsNotFound: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReportTypeDef](./type_defs.md#reporttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetFleetsOutputTypeDef

```python
# BatchGetFleetsOutputTypeDef definition

class BatchGetFleetsOutputTypeDef(TypedDict):
    fleets: List[FleetTypeDef],  # (1)
    fleetsNotFound: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FleetTypeDef](./type_defs.md#fleettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFleetOutputTypeDef

```python
# CreateFleetOutputTypeDef definition

class CreateFleetOutputTypeDef(TypedDict):
    fleet: FleetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FleetTypeDef](./type_defs.md#fleettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFleetOutputTypeDef

```python
# UpdateFleetOutputTypeDef definition

class UpdateFleetOutputTypeDef(TypedDict):
    fleet: FleetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FleetTypeDef](./type_defs.md#fleettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetBuildBatchesOutputTypeDef

```python
# BatchGetBuildBatchesOutputTypeDef definition

class BatchGetBuildBatchesOutputTypeDef(TypedDict):
    buildBatches: List[BuildBatchTypeDef],  # (1)
    buildBatchesNotFound: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BuildBatchTypeDef](./type_defs.md#buildbatchtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RetryBuildBatchOutputTypeDef

```python
# RetryBuildBatchOutputTypeDef definition

class RetryBuildBatchOutputTypeDef(TypedDict):
    buildBatch: BuildBatchTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BuildBatchTypeDef](./type_defs.md#buildbatchtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartBuildBatchOutputTypeDef

```python
# StartBuildBatchOutputTypeDef definition

class StartBuildBatchOutputTypeDef(TypedDict):
    buildBatch: BuildBatchTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BuildBatchTypeDef](./type_defs.md#buildbatchtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopBuildBatchOutputTypeDef

```python
# StopBuildBatchOutputTypeDef definition

class StopBuildBatchOutputTypeDef(TypedDict):
    buildBatch: BuildBatchTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BuildBatchTypeDef](./type_defs.md#buildbatchtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
