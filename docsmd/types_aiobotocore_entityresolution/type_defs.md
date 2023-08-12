# Type definitions

> [Index](../README.md) > [EntityResolution](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [EntityResolution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
    type annotations stubs module [types-aiobotocore-entityresolution](https://pypi.org/project/types-aiobotocore-entityresolution/).



## IncrementalRunConfigTypeDef

```python
# IncrementalRunConfigTypeDef definition

class IncrementalRunConfigTypeDef(TypedDict):
    incrementalRunType: NotRequired[IncrementalRunTypeType],  # (1)
```

1. See [:material-code-brackets: IncrementalRunTypeType](./literals.md#incrementalruntypetype) 
## InputSourceTypeDef

```python
# InputSourceTypeDef definition

class InputSourceTypeDef(TypedDict):
    inputSourceARN: str,
    schemaName: str,
    applyNormalization: NotRequired[bool],
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

## SchemaInputAttributeTypeDef

```python
# SchemaInputAttributeTypeDef definition

class SchemaInputAttributeTypeDef(TypedDict):
    fieldName: str,
    type: SchemaAttributeTypeType,  # (1)
    groupName: NotRequired[str],
    matchKey: NotRequired[str],
```

1. See [:material-code-brackets: SchemaAttributeTypeType](./literals.md#schemaattributetypetype) 
## DeleteMatchingWorkflowInputRequestTypeDef

```python
# DeleteMatchingWorkflowInputRequestTypeDef definition

class DeleteMatchingWorkflowInputRequestTypeDef(TypedDict):
    workflowName: str,
```

## DeleteSchemaMappingInputRequestTypeDef

```python
# DeleteSchemaMappingInputRequestTypeDef definition

class DeleteSchemaMappingInputRequestTypeDef(TypedDict):
    schemaName: str,
```

## ErrorDetailsTypeDef

```python
# ErrorDetailsTypeDef definition

class ErrorDetailsTypeDef(TypedDict):
    errorMessage: NotRequired[str],
```

## GetMatchIdInputRequestTypeDef

```python
# GetMatchIdInputRequestTypeDef definition

class GetMatchIdInputRequestTypeDef(TypedDict):
    record: Mapping[str, str],
    workflowName: str,
```

## GetMatchingJobInputRequestTypeDef

```python
# GetMatchingJobInputRequestTypeDef definition

class GetMatchingJobInputRequestTypeDef(TypedDict):
    jobId: str,
    workflowName: str,
```

## JobMetricsTypeDef

```python
# JobMetricsTypeDef definition

class JobMetricsTypeDef(TypedDict):
    inputRecords: NotRequired[int],
    matchIDs: NotRequired[int],
    recordsNotProcessed: NotRequired[int],
    totalRecordsProcessed: NotRequired[int],
```

## GetMatchingWorkflowInputRequestTypeDef

```python
# GetMatchingWorkflowInputRequestTypeDef definition

class GetMatchingWorkflowInputRequestTypeDef(TypedDict):
    workflowName: str,
```

## GetSchemaMappingInputRequestTypeDef

```python
# GetSchemaMappingInputRequestTypeDef definition

class GetSchemaMappingInputRequestTypeDef(TypedDict):
    schemaName: str,
```

## JobSummaryTypeDef

```python
# JobSummaryTypeDef definition

class JobSummaryTypeDef(TypedDict):
    jobId: str,
    startTime: datetime,
    status: JobStatusType,  # (1)
    endTime: NotRequired[datetime],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListMatchingJobsInputRequestTypeDef

```python
# ListMatchingJobsInputRequestTypeDef definition

class ListMatchingJobsInputRequestTypeDef(TypedDict):
    workflowName: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListMatchingWorkflowsInputRequestTypeDef

```python
# ListMatchingWorkflowsInputRequestTypeDef definition

class ListMatchingWorkflowsInputRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## MatchingWorkflowSummaryTypeDef

```python
# MatchingWorkflowSummaryTypeDef definition

class MatchingWorkflowSummaryTypeDef(TypedDict):
    createdAt: datetime,
    updatedAt: datetime,
    workflowArn: str,
    workflowName: str,
```

## ListSchemaMappingsInputRequestTypeDef

```python
# ListSchemaMappingsInputRequestTypeDef definition

class ListSchemaMappingsInputRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## SchemaMappingSummaryTypeDef

```python
# SchemaMappingSummaryTypeDef definition

class SchemaMappingSummaryTypeDef(TypedDict):
    createdAt: datetime,
    schemaArn: str,
    schemaName: str,
    updatedAt: datetime,
```

## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
```

## OutputAttributeTypeDef

```python
# OutputAttributeTypeDef definition

class OutputAttributeTypeDef(TypedDict):
    name: str,
    hashed: NotRequired[bool],
```

## RuleTypeDef

```python
# RuleTypeDef definition

class RuleTypeDef(TypedDict):
    matchingKeys: Sequence[str],
    ruleName: str,
```

## StartMatchingJobInputRequestTypeDef

```python
# StartMatchingJobInputRequestTypeDef definition

class StartMatchingJobInputRequestTypeDef(TypedDict):
    workflowName: str,
```

## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## DeleteMatchingWorkflowOutputTypeDef

```python
# DeleteMatchingWorkflowOutputTypeDef definition

class DeleteMatchingWorkflowOutputTypeDef(TypedDict):
    message: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteSchemaMappingOutputTypeDef

```python
# DeleteSchemaMappingOutputTypeDef definition

class DeleteSchemaMappingOutputTypeDef(TypedDict):
    message: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMatchIdOutputTypeDef

```python
# GetMatchIdOutputTypeDef definition

class GetMatchIdOutputTypeDef(TypedDict):
    matchId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMatchingJobOutputTypeDef

```python
# StartMatchingJobOutputTypeDef definition

class StartMatchingJobOutputTypeDef(TypedDict):
    jobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSchemaMappingInputRequestTypeDef

```python
# CreateSchemaMappingInputRequestTypeDef definition

class CreateSchemaMappingInputRequestTypeDef(TypedDict):
    schemaName: str,
    description: NotRequired[str],
    mappedInputFields: NotRequired[Sequence[SchemaInputAttributeTypeDef]],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: SchemaInputAttributeTypeDef](./type_defs.md#schemainputattributetypedef) 
## CreateSchemaMappingOutputTypeDef

```python
# CreateSchemaMappingOutputTypeDef definition

class CreateSchemaMappingOutputTypeDef(TypedDict):
    description: str,
    mappedInputFields: List[SchemaInputAttributeTypeDef],  # (1)
    schemaArn: str,
    schemaName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SchemaInputAttributeTypeDef](./type_defs.md#schemainputattributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSchemaMappingOutputTypeDef

```python
# GetSchemaMappingOutputTypeDef definition

class GetSchemaMappingOutputTypeDef(TypedDict):
    createdAt: datetime,
    description: str,
    mappedInputFields: List[SchemaInputAttributeTypeDef],  # (1)
    schemaArn: str,
    schemaName: str,
    tags: Dict[str, str],
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SchemaInputAttributeTypeDef](./type_defs.md#schemainputattributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMatchingJobOutputTypeDef

```python
# GetMatchingJobOutputTypeDef definition

class GetMatchingJobOutputTypeDef(TypedDict):
    endTime: datetime,
    errorDetails: ErrorDetailsTypeDef,  # (1)
    jobId: str,
    metrics: JobMetricsTypeDef,  # (2)
    startTime: datetime,
    status: JobStatusType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef) 
2. See [:material-code-braces: JobMetricsTypeDef](./type_defs.md#jobmetricstypedef) 
3. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMatchingJobsOutputTypeDef

```python
# ListMatchingJobsOutputTypeDef definition

class ListMatchingJobsOutputTypeDef(TypedDict):
    jobs: List[JobSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobSummaryTypeDef](./type_defs.md#jobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMatchingJobsInputListMatchingJobsPaginateTypeDef

```python
# ListMatchingJobsInputListMatchingJobsPaginateTypeDef definition

class ListMatchingJobsInputListMatchingJobsPaginateTypeDef(TypedDict):
    workflowName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMatchingWorkflowsInputListMatchingWorkflowsPaginateTypeDef

```python
# ListMatchingWorkflowsInputListMatchingWorkflowsPaginateTypeDef definition

class ListMatchingWorkflowsInputListMatchingWorkflowsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSchemaMappingsInputListSchemaMappingsPaginateTypeDef

```python
# ListSchemaMappingsInputListSchemaMappingsPaginateTypeDef definition

class ListSchemaMappingsInputListSchemaMappingsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMatchingWorkflowsOutputTypeDef

```python
# ListMatchingWorkflowsOutputTypeDef definition

class ListMatchingWorkflowsOutputTypeDef(TypedDict):
    nextToken: str,
    workflowSummaries: List[MatchingWorkflowSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MatchingWorkflowSummaryTypeDef](./type_defs.md#matchingworkflowsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSchemaMappingsOutputTypeDef

```python
# ListSchemaMappingsOutputTypeDef definition

class ListSchemaMappingsOutputTypeDef(TypedDict):
    nextToken: str,
    schemaList: List[SchemaMappingSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SchemaMappingSummaryTypeDef](./type_defs.md#schemamappingsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OutputSourceTypeDef

```python
# OutputSourceTypeDef definition

class OutputSourceTypeDef(TypedDict):
    output: Sequence[OutputAttributeTypeDef],  # (1)
    outputS3Path: str,
    KMSArn: NotRequired[str],
    applyNormalization: NotRequired[bool],
```

1. See [:material-code-braces: OutputAttributeTypeDef](./type_defs.md#outputattributetypedef) 
## RuleBasedPropertiesTypeDef

```python
# RuleBasedPropertiesTypeDef definition

class RuleBasedPropertiesTypeDef(TypedDict):
    attributeMatchingModel: AttributeMatchingModelType,  # (1)
    rules: Sequence[RuleTypeDef],  # (2)
```

1. See [:material-code-brackets: AttributeMatchingModelType](./literals.md#attributematchingmodeltype) 
2. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
## ResolutionTechniquesTypeDef

```python
# ResolutionTechniquesTypeDef definition

class ResolutionTechniquesTypeDef(TypedDict):
    resolutionType: NotRequired[ResolutionTypeType],  # (1)
    ruleBasedProperties: NotRequired[RuleBasedPropertiesTypeDef],  # (2)
```

1. See [:material-code-brackets: ResolutionTypeType](./literals.md#resolutiontypetype) 
2. See [:material-code-braces: RuleBasedPropertiesTypeDef](./type_defs.md#rulebasedpropertiestypedef) 
## CreateMatchingWorkflowInputRequestTypeDef

```python
# CreateMatchingWorkflowInputRequestTypeDef definition

class CreateMatchingWorkflowInputRequestTypeDef(TypedDict):
    inputSourceConfig: Sequence[InputSourceTypeDef],  # (1)
    outputSourceConfig: Sequence[OutputSourceTypeDef],  # (2)
    resolutionTechniques: ResolutionTechniquesTypeDef,  # (3)
    roleArn: str,
    workflowName: str,
    description: NotRequired[str],
    incrementalRunConfig: NotRequired[IncrementalRunConfigTypeDef],  # (4)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: InputSourceTypeDef](./type_defs.md#inputsourcetypedef) 
2. See [:material-code-braces: OutputSourceTypeDef](./type_defs.md#outputsourcetypedef) 
3. See [:material-code-braces: ResolutionTechniquesTypeDef](./type_defs.md#resolutiontechniquestypedef) 
4. See [:material-code-braces: IncrementalRunConfigTypeDef](./type_defs.md#incrementalrunconfigtypedef) 
## CreateMatchingWorkflowOutputTypeDef

```python
# CreateMatchingWorkflowOutputTypeDef definition

class CreateMatchingWorkflowOutputTypeDef(TypedDict):
    description: str,
    incrementalRunConfig: IncrementalRunConfigTypeDef,  # (1)
    inputSourceConfig: List[InputSourceTypeDef],  # (2)
    outputSourceConfig: List[OutputSourceTypeDef],  # (3)
    resolutionTechniques: ResolutionTechniquesTypeDef,  # (4)
    roleArn: str,
    workflowArn: str,
    workflowName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: IncrementalRunConfigTypeDef](./type_defs.md#incrementalrunconfigtypedef) 
2. See [:material-code-braces: InputSourceTypeDef](./type_defs.md#inputsourcetypedef) 
3. See [:material-code-braces: OutputSourceTypeDef](./type_defs.md#outputsourcetypedef) 
4. See [:material-code-braces: ResolutionTechniquesTypeDef](./type_defs.md#resolutiontechniquestypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMatchingWorkflowOutputTypeDef

```python
# GetMatchingWorkflowOutputTypeDef definition

class GetMatchingWorkflowOutputTypeDef(TypedDict):
    createdAt: datetime,
    description: str,
    incrementalRunConfig: IncrementalRunConfigTypeDef,  # (1)
    inputSourceConfig: List[InputSourceTypeDef],  # (2)
    outputSourceConfig: List[OutputSourceTypeDef],  # (3)
    resolutionTechniques: ResolutionTechniquesTypeDef,  # (4)
    roleArn: str,
    tags: Dict[str, str],
    updatedAt: datetime,
    workflowArn: str,
    workflowName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: IncrementalRunConfigTypeDef](./type_defs.md#incrementalrunconfigtypedef) 
2. See [:material-code-braces: InputSourceTypeDef](./type_defs.md#inputsourcetypedef) 
3. See [:material-code-braces: OutputSourceTypeDef](./type_defs.md#outputsourcetypedef) 
4. See [:material-code-braces: ResolutionTechniquesTypeDef](./type_defs.md#resolutiontechniquestypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMatchingWorkflowInputRequestTypeDef

```python
# UpdateMatchingWorkflowInputRequestTypeDef definition

class UpdateMatchingWorkflowInputRequestTypeDef(TypedDict):
    inputSourceConfig: Sequence[InputSourceTypeDef],  # (1)
    outputSourceConfig: Sequence[OutputSourceTypeDef],  # (2)
    resolutionTechniques: ResolutionTechniquesTypeDef,  # (3)
    roleArn: str,
    workflowName: str,
    description: NotRequired[str],
    incrementalRunConfig: NotRequired[IncrementalRunConfigTypeDef],  # (4)
```

1. See [:material-code-braces: InputSourceTypeDef](./type_defs.md#inputsourcetypedef) 
2. See [:material-code-braces: OutputSourceTypeDef](./type_defs.md#outputsourcetypedef) 
3. See [:material-code-braces: ResolutionTechniquesTypeDef](./type_defs.md#resolutiontechniquestypedef) 
4. See [:material-code-braces: IncrementalRunConfigTypeDef](./type_defs.md#incrementalrunconfigtypedef) 
## UpdateMatchingWorkflowOutputTypeDef

```python
# UpdateMatchingWorkflowOutputTypeDef definition

class UpdateMatchingWorkflowOutputTypeDef(TypedDict):
    description: str,
    incrementalRunConfig: IncrementalRunConfigTypeDef,  # (1)
    inputSourceConfig: List[InputSourceTypeDef],  # (2)
    outputSourceConfig: List[OutputSourceTypeDef],  # (3)
    resolutionTechniques: ResolutionTechniquesTypeDef,  # (4)
    roleArn: str,
    workflowName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: IncrementalRunConfigTypeDef](./type_defs.md#incrementalrunconfigtypedef) 
2. See [:material-code-braces: InputSourceTypeDef](./type_defs.md#inputsourcetypedef) 
3. See [:material-code-braces: OutputSourceTypeDef](./type_defs.md#outputsourcetypedef) 
4. See [:material-code-braces: ResolutionTechniquesTypeDef](./type_defs.md#resolutiontechniquestypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
