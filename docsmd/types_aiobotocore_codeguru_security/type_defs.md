# Type definitions

> [Index](../README.md) > [CodeGuruSecurity](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CodeGuruSecurity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#CodeGuruSecurity)
    type annotations stubs module [types-aiobotocore-codeguru-security](https://pypi.org/project/types-aiobotocore-codeguru-security/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## FindingMetricsValuePerSeverityTypeDef

```python
# FindingMetricsValuePerSeverityTypeDef definition

class FindingMetricsValuePerSeverityTypeDef(TypedDict):
    critical: NotRequired[float],
    high: NotRequired[float],
    info: NotRequired[float],
    low: NotRequired[float],
    medium: NotRequired[float],
```

## BatchGetFindingsErrorTypeDef

```python
# BatchGetFindingsErrorTypeDef definition

class BatchGetFindingsErrorTypeDef(TypedDict):
    errorCode: ErrorCodeType,  # (1)
    findingId: str,
    message: str,
    scanName: str,
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
## FindingIdentifierTypeDef

```python
# FindingIdentifierTypeDef definition

class FindingIdentifierTypeDef(TypedDict):
    findingId: str,
    scanName: str,
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

## CategoryWithFindingNumTypeDef

```python
# CategoryWithFindingNumTypeDef definition

class CategoryWithFindingNumTypeDef(TypedDict):
    categoryName: NotRequired[str],
    findingNumber: NotRequired[int],
```

## CodeLineTypeDef

```python
# CodeLineTypeDef definition

class CodeLineTypeDef(TypedDict):
    content: NotRequired[str],
    number: NotRequired[int],
```

## ResourceIdTypeDef

```python
# ResourceIdTypeDef definition

class ResourceIdTypeDef(TypedDict):
    codeArtifactId: NotRequired[str],
```

## CreateUploadUrlRequestRequestTypeDef

```python
# CreateUploadUrlRequestRequestTypeDef definition

class CreateUploadUrlRequestRequestTypeDef(TypedDict):
    scanName: str,
```

## EncryptionConfigTypeDef

```python
# EncryptionConfigTypeDef definition

class EncryptionConfigTypeDef(TypedDict):
    kmsKeyArn: NotRequired[str],
```

## ResourceTypeDef

```python
# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    id: NotRequired[str],
    subResourceId: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetFindingsRequestRequestTypeDef

```python
# GetFindingsRequestRequestTypeDef definition

class GetFindingsRequestRequestTypeDef(TypedDict):
    scanName: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    status: NotRequired[StatusType],  # (1)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## GetScanRequestRequestTypeDef

```python
# GetScanRequestRequestTypeDef definition

class GetScanRequestRequestTypeDef(TypedDict):
    scanName: str,
    runId: NotRequired[str],
```

## ListScansRequestRequestTypeDef

```python
# ListScansRequestRequestTypeDef definition

class ListScansRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ScanSummaryTypeDef

```python
# ScanSummaryTypeDef definition

class ScanSummaryTypeDef(TypedDict):
    createdAt: datetime,
    runId: str,
    scanName: str,
    scanState: ScanStateType,  # (1)
    scanNameArn: NotRequired[str],
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: ScanStateType](./literals.md#scanstatetype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ScanNameWithFindingNumTypeDef

```python
# ScanNameWithFindingNumTypeDef definition

class ScanNameWithFindingNumTypeDef(TypedDict):
    findingNumber: NotRequired[int],
    scanName: NotRequired[str],
```

## RecommendationTypeDef

```python
# RecommendationTypeDef definition

class RecommendationTypeDef(TypedDict):
    text: NotRequired[str],
    url: NotRequired[str],
```

## SuggestedFixTypeDef

```python
# SuggestedFixTypeDef definition

class SuggestedFixTypeDef(TypedDict):
    code: NotRequired[str],
    description: NotRequired[str],
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

## AccountFindingsMetricTypeDef

```python
# AccountFindingsMetricTypeDef definition

class AccountFindingsMetricTypeDef(TypedDict):
    closedFindings: NotRequired[FindingMetricsValuePerSeverityTypeDef],  # (1)
    date: NotRequired[datetime],
    meanTimeToClose: NotRequired[FindingMetricsValuePerSeverityTypeDef],  # (1)
    newFindings: NotRequired[FindingMetricsValuePerSeverityTypeDef],  # (1)
    openFindings: NotRequired[FindingMetricsValuePerSeverityTypeDef],  # (1)
```

1. See [:material-code-braces: FindingMetricsValuePerSeverityTypeDef](./type_defs.md#findingmetricsvalueperseveritytypedef) 
2. See [:material-code-braces: FindingMetricsValuePerSeverityTypeDef](./type_defs.md#findingmetricsvalueperseveritytypedef) 
3. See [:material-code-braces: FindingMetricsValuePerSeverityTypeDef](./type_defs.md#findingmetricsvalueperseveritytypedef) 
4. See [:material-code-braces: FindingMetricsValuePerSeverityTypeDef](./type_defs.md#findingmetricsvalueperseveritytypedef) 
## BatchGetFindingsRequestRequestTypeDef

```python
# BatchGetFindingsRequestRequestTypeDef definition

class BatchGetFindingsRequestRequestTypeDef(TypedDict):
    findingIdentifiers: Sequence[FindingIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: FindingIdentifierTypeDef](./type_defs.md#findingidentifiertypedef) 
## CreateUploadUrlResponseTypeDef

```python
# CreateUploadUrlResponseTypeDef definition

class CreateUploadUrlResponseTypeDef(TypedDict):
    codeArtifactId: str,
    requestHeaders: Dict[str, str],
    s3Url: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetScanResponseTypeDef

```python
# GetScanResponseTypeDef definition

class GetScanResponseTypeDef(TypedDict):
    analysisType: AnalysisTypeType,  # (1)
    createdAt: datetime,
    numberOfRevisions: int,
    runId: str,
    scanName: str,
    scanNameArn: str,
    scanState: ScanStateType,  # (2)
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: AnalysisTypeType](./literals.md#analysistypetype) 
2. See [:material-code-brackets: ScanStateType](./literals.md#scanstatetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FilePathTypeDef

```python
# FilePathTypeDef definition

class FilePathTypeDef(TypedDict):
    codeSnippet: NotRequired[List[CodeLineTypeDef]],  # (1)
    endLine: NotRequired[int],
    name: NotRequired[str],
    path: NotRequired[str],
    startLine: NotRequired[int],
```

1. See [:material-code-braces: CodeLineTypeDef](./type_defs.md#codelinetypedef) 
## CreateScanRequestRequestTypeDef

```python
# CreateScanRequestRequestTypeDef definition

class CreateScanRequestRequestTypeDef(TypedDict):
    resourceId: ResourceIdTypeDef,  # (1)
    scanName: str,
    analysisType: NotRequired[AnalysisTypeType],  # (2)
    clientToken: NotRequired[str],
    scanType: NotRequired[ScanTypeType],  # (3)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ResourceIdTypeDef](./type_defs.md#resourceidtypedef) 
2. See [:material-code-brackets: AnalysisTypeType](./literals.md#analysistypetype) 
3. See [:material-code-brackets: ScanTypeType](./literals.md#scantypetype) 
## CreateScanResponseTypeDef

```python
# CreateScanResponseTypeDef definition

class CreateScanResponseTypeDef(TypedDict):
    resourceId: ResourceIdTypeDef,  # (1)
    runId: str,
    scanName: str,
    scanNameArn: str,
    scanState: ScanStateType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ResourceIdTypeDef](./type_defs.md#resourceidtypedef) 
2. See [:material-code-brackets: ScanStateType](./literals.md#scanstatetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAccountConfigurationResponseTypeDef

```python
# GetAccountConfigurationResponseTypeDef definition

class GetAccountConfigurationResponseTypeDef(TypedDict):
    encryptionConfig: EncryptionConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAccountConfigurationRequestRequestTypeDef

```python
# UpdateAccountConfigurationRequestRequestTypeDef definition

class UpdateAccountConfigurationRequestRequestTypeDef(TypedDict):
    encryptionConfig: EncryptionConfigTypeDef,  # (1)
```

1. See [:material-code-braces: EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef) 
## UpdateAccountConfigurationResponseTypeDef

```python
# UpdateAccountConfigurationResponseTypeDef definition

class UpdateAccountConfigurationResponseTypeDef(TypedDict):
    encryptionConfig: EncryptionConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFindingsRequestGetFindingsPaginateTypeDef

```python
# GetFindingsRequestGetFindingsPaginateTypeDef definition

class GetFindingsRequestGetFindingsPaginateTypeDef(TypedDict):
    scanName: str,
    status: NotRequired[StatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListScansRequestListScansPaginateTypeDef

```python
# ListScansRequestListScansPaginateTypeDef definition

class ListScansRequestListScansPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetMetricsSummaryRequestRequestTypeDef

```python
# GetMetricsSummaryRequestRequestTypeDef definition

class GetMetricsSummaryRequestRequestTypeDef(TypedDict):
    date: Union[datetime, str],
```

## ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef

```python
# ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef definition

class ListFindingsMetricsRequestListFindingsMetricsPaginateTypeDef(TypedDict):
    endDate: Union[datetime, str],
    startDate: Union[datetime, str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFindingsMetricsRequestRequestTypeDef

```python
# ListFindingsMetricsRequestRequestTypeDef definition

class ListFindingsMetricsRequestRequestTypeDef(TypedDict):
    endDate: Union[datetime, str],
    startDate: Union[datetime, str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListScansResponseTypeDef

```python
# ListScansResponseTypeDef definition

class ListScansResponseTypeDef(TypedDict):
    nextToken: str,
    summaries: List[ScanSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ScanSummaryTypeDef](./type_defs.md#scansummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MetricsSummaryTypeDef

```python
# MetricsSummaryTypeDef definition

class MetricsSummaryTypeDef(TypedDict):
    categoriesWithMostFindings: NotRequired[List[CategoryWithFindingNumTypeDef]],  # (1)
    date: NotRequired[datetime],
    openFindings: NotRequired[FindingMetricsValuePerSeverityTypeDef],  # (2)
    scansWithMostOpenCriticalFindings: NotRequired[List[ScanNameWithFindingNumTypeDef]],  # (3)
    scansWithMostOpenFindings: NotRequired[List[ScanNameWithFindingNumTypeDef]],  # (3)
```

1. See [:material-code-braces: CategoryWithFindingNumTypeDef](./type_defs.md#categorywithfindingnumtypedef) 
2. See [:material-code-braces: FindingMetricsValuePerSeverityTypeDef](./type_defs.md#findingmetricsvalueperseveritytypedef) 
3. See [:material-code-braces: ScanNameWithFindingNumTypeDef](./type_defs.md#scannamewithfindingnumtypedef) 
4. See [:material-code-braces: ScanNameWithFindingNumTypeDef](./type_defs.md#scannamewithfindingnumtypedef) 
## RemediationTypeDef

```python
# RemediationTypeDef definition

class RemediationTypeDef(TypedDict):
    recommendation: NotRequired[RecommendationTypeDef],  # (1)
    suggestedFixes: NotRequired[List[SuggestedFixTypeDef]],  # (2)
```

1. See [:material-code-braces: RecommendationTypeDef](./type_defs.md#recommendationtypedef) 
2. See [:material-code-braces: SuggestedFixTypeDef](./type_defs.md#suggestedfixtypedef) 
## ListFindingsMetricsResponseTypeDef

```python
# ListFindingsMetricsResponseTypeDef definition

class ListFindingsMetricsResponseTypeDef(TypedDict):
    findingsMetrics: List[AccountFindingsMetricTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountFindingsMetricTypeDef](./type_defs.md#accountfindingsmetrictypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VulnerabilityTypeDef

```python
# VulnerabilityTypeDef definition

class VulnerabilityTypeDef(TypedDict):
    filePath: NotRequired[FilePathTypeDef],  # (1)
    id: NotRequired[str],
    itemCount: NotRequired[int],
    referenceUrls: NotRequired[List[str]],
    relatedVulnerabilities: NotRequired[List[str]],
```

1. See [:material-code-braces: FilePathTypeDef](./type_defs.md#filepathtypedef) 
## GetMetricsSummaryResponseTypeDef

```python
# GetMetricsSummaryResponseTypeDef definition

class GetMetricsSummaryResponseTypeDef(TypedDict):
    metricsSummary: MetricsSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MetricsSummaryTypeDef](./type_defs.md#metricssummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FindingTypeDef

```python
# FindingTypeDef definition

class FindingTypeDef(TypedDict):
    createdAt: NotRequired[datetime],
    description: NotRequired[str],
    detectorId: NotRequired[str],
    detectorName: NotRequired[str],
    detectorTags: NotRequired[List[str]],
    generatorId: NotRequired[str],
    id: NotRequired[str],
    remediation: NotRequired[RemediationTypeDef],  # (1)
    resource: NotRequired[ResourceTypeDef],  # (2)
    ruleId: NotRequired[str],
    severity: NotRequired[SeverityType],  # (3)
    status: NotRequired[StatusType],  # (4)
    title: NotRequired[str],
    type: NotRequired[str],
    updatedAt: NotRequired[datetime],
    vulnerability: NotRequired[VulnerabilityTypeDef],  # (5)
```

1. See [:material-code-braces: RemediationTypeDef](./type_defs.md#remediationtypedef) 
2. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
3. See [:material-code-brackets: SeverityType](./literals.md#severitytype) 
4. See [:material-code-brackets: StatusType](./literals.md#statustype) 
5. See [:material-code-braces: VulnerabilityTypeDef](./type_defs.md#vulnerabilitytypedef) 
## BatchGetFindingsResponseTypeDef

```python
# BatchGetFindingsResponseTypeDef definition

class BatchGetFindingsResponseTypeDef(TypedDict):
    failedFindings: List[BatchGetFindingsErrorTypeDef],  # (1)
    findings: List[FindingTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchGetFindingsErrorTypeDef](./type_defs.md#batchgetfindingserrortypedef) 
2. See [:material-code-braces: FindingTypeDef](./type_defs.md#findingtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFindingsResponseTypeDef

```python
# GetFindingsResponseTypeDef definition

class GetFindingsResponseTypeDef(TypedDict):
    findings: List[FindingTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FindingTypeDef](./type_defs.md#findingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
