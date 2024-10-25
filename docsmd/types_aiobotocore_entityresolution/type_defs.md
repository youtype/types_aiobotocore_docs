# Type definitions

> [Index](../README.md) > [EntityResolution](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [EntityResolution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#EntityResolution)
    type annotations stubs module [types-aiobotocore-entityresolution](https://pypi.org/project/types-aiobotocore-entityresolution/).

## NamespaceProviderPropertiesUnionTypeDef

```python
# NamespaceProviderPropertiesUnionTypeDef definition

NamespaceProviderPropertiesUnionTypeDef = Union[
    NamespaceProviderPropertiesTypeDef,  # (1)
    NamespaceProviderPropertiesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: NamespaceProviderPropertiesTypeDef](./type_defs.md#namespaceproviderpropertiestypedef) 
2. See [:material-code-braces: NamespaceProviderPropertiesOutputTypeDef](./type_defs.md#namespaceproviderpropertiesoutputtypedef) 

## RuleUnionTypeDef

```python
# RuleUnionTypeDef definition

RuleUnionTypeDef = Union[
    RuleTypeDef,  # (1)
    RuleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
2. See [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 

## ProviderPropertiesUnionTypeDef

```python
# ProviderPropertiesUnionTypeDef definition

ProviderPropertiesUnionTypeDef = Union[
    ProviderPropertiesTypeDef,  # (1)
    ProviderPropertiesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ProviderPropertiesTypeDef](./type_defs.md#providerpropertiestypedef) 
2. See [:material-code-braces: ProviderPropertiesOutputTypeDef](./type_defs.md#providerpropertiesoutputtypedef) 

## OutputSourceUnionTypeDef

```python
# OutputSourceUnionTypeDef definition

OutputSourceUnionTypeDef = Union[
    OutputSourceTypeDef,  # (1)
    OutputSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: OutputSourceTypeDef](./type_defs.md#outputsourcetypedef) 
2. See [:material-code-braces: OutputSourceOutputTypeDef](./type_defs.md#outputsourceoutputtypedef) 

## IdMappingRuleBasedPropertiesUnionTypeDef

```python
# IdMappingRuleBasedPropertiesUnionTypeDef definition

IdMappingRuleBasedPropertiesUnionTypeDef = Union[
    IdMappingRuleBasedPropertiesTypeDef,  # (1)
    IdMappingRuleBasedPropertiesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: IdMappingRuleBasedPropertiesTypeDef](./type_defs.md#idmappingrulebasedpropertiestypedef) 
2. See [:material-code-braces: IdMappingRuleBasedPropertiesOutputTypeDef](./type_defs.md#idmappingrulebasedpropertiesoutputtypedef) 

## NamespaceRuleBasedPropertiesUnionTypeDef

```python
# NamespaceRuleBasedPropertiesUnionTypeDef definition

NamespaceRuleBasedPropertiesUnionTypeDef = Union[
    NamespaceRuleBasedPropertiesTypeDef,  # (1)
    NamespaceRuleBasedPropertiesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: NamespaceRuleBasedPropertiesTypeDef](./type_defs.md#namespacerulebasedpropertiestypedef) 
2. See [:material-code-braces: NamespaceRuleBasedPropertiesOutputTypeDef](./type_defs.md#namespacerulebasedpropertiesoutputtypedef) 

## RuleBasedPropertiesUnionTypeDef

```python
# RuleBasedPropertiesUnionTypeDef definition

RuleBasedPropertiesUnionTypeDef = Union[
    RuleBasedPropertiesTypeDef,  # (1)
    RuleBasedPropertiesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RuleBasedPropertiesTypeDef](./type_defs.md#rulebasedpropertiestypedef) 
2. See [:material-code-braces: RuleBasedPropertiesOutputTypeDef](./type_defs.md#rulebasedpropertiesoutputtypedef) 

## IdNamespaceIdMappingWorkflowPropertiesUnionTypeDef

```python
# IdNamespaceIdMappingWorkflowPropertiesUnionTypeDef definition

IdNamespaceIdMappingWorkflowPropertiesUnionTypeDef = Union[
    IdNamespaceIdMappingWorkflowPropertiesTypeDef,  # (1)
    IdNamespaceIdMappingWorkflowPropertiesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: IdNamespaceIdMappingWorkflowPropertiesTypeDef](./type_defs.md#idnamespaceidmappingworkflowpropertiestypedef) 
2. See [:material-code-braces: IdNamespaceIdMappingWorkflowPropertiesOutputTypeDef](./type_defs.md#idnamespaceidmappingworkflowpropertiesoutputtypedef) 



## AddPolicyStatementInputRequestTypeDef

```python
# AddPolicyStatementInputRequestTypeDef definition

class AddPolicyStatementInputRequestTypeDef(TypedDict):
    action: Sequence[str],
    arn: str,
    effect: StatementEffectType,  # (1)
    principal: Sequence[str],
    statementId: str,
    condition: NotRequired[str],
```

1. See [:material-code-brackets: StatementEffectType](./literals.md#statementeffecttype) 
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

## BatchDeleteUniqueIdInputRequestTypeDef

```python
# BatchDeleteUniqueIdInputRequestTypeDef definition

class BatchDeleteUniqueIdInputRequestTypeDef(TypedDict):
    uniqueIds: Sequence[str],
    workflowName: str,
    inputSource: NotRequired[str],
```

## DeleteUniqueIdErrorTypeDef

```python
# DeleteUniqueIdErrorTypeDef definition

class DeleteUniqueIdErrorTypeDef(TypedDict):
    errorType: DeleteUniqueIdErrorTypeType,  # (1)
    uniqueId: str,
```

1. See [:material-code-brackets: DeleteUniqueIdErrorTypeType](./literals.md#deleteuniqueiderrortypetype) 
## DeletedUniqueIdTypeDef

```python
# DeletedUniqueIdTypeDef definition

class DeletedUniqueIdTypeDef(TypedDict):
    uniqueId: str,
```

## IdMappingWorkflowInputSourceTypeDef

```python
# IdMappingWorkflowInputSourceTypeDef definition

class IdMappingWorkflowInputSourceTypeDef(TypedDict):
    inputSourceARN: str,
    schemaName: NotRequired[str],
    type: NotRequired[IdNamespaceTypeType],  # (1)
```

1. See [:material-code-brackets: IdNamespaceTypeType](./literals.md#idnamespacetypetype) 
## IdMappingWorkflowOutputSourceTypeDef

```python
# IdMappingWorkflowOutputSourceTypeDef definition

class IdMappingWorkflowOutputSourceTypeDef(TypedDict):
    outputS3Path: str,
    KMSArn: NotRequired[str],
```

## IdNamespaceInputSourceTypeDef

```python
# IdNamespaceInputSourceTypeDef definition

class IdNamespaceInputSourceTypeDef(TypedDict):
    inputSourceARN: str,
    schemaName: NotRequired[str],
```

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

## SchemaInputAttributeTypeDef

```python
# SchemaInputAttributeTypeDef definition

class SchemaInputAttributeTypeDef(TypedDict):
    fieldName: str,
    type: SchemaAttributeTypeType,  # (1)
    groupName: NotRequired[str],
    hashed: NotRequired[bool],
    matchKey: NotRequired[str],
    subType: NotRequired[str],
```

1. See [:material-code-brackets: SchemaAttributeTypeType](./literals.md#schemaattributetypetype) 
## DeleteIdMappingWorkflowInputRequestTypeDef

```python
# DeleteIdMappingWorkflowInputRequestTypeDef definition

class DeleteIdMappingWorkflowInputRequestTypeDef(TypedDict):
    workflowName: str,
```

## DeleteIdNamespaceInputRequestTypeDef

```python
# DeleteIdNamespaceInputRequestTypeDef definition

class DeleteIdNamespaceInputRequestTypeDef(TypedDict):
    idNamespaceName: str,
```

## DeleteMatchingWorkflowInputRequestTypeDef

```python
# DeleteMatchingWorkflowInputRequestTypeDef definition

class DeleteMatchingWorkflowInputRequestTypeDef(TypedDict):
    workflowName: str,
```

## DeletePolicyStatementInputRequestTypeDef

```python
# DeletePolicyStatementInputRequestTypeDef definition

class DeletePolicyStatementInputRequestTypeDef(TypedDict):
    arn: str,
    statementId: str,
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

## GetIdMappingJobInputRequestTypeDef

```python
# GetIdMappingJobInputRequestTypeDef definition

class GetIdMappingJobInputRequestTypeDef(TypedDict):
    jobId: str,
    workflowName: str,
```

## IdMappingJobMetricsTypeDef

```python
# IdMappingJobMetricsTypeDef definition

class IdMappingJobMetricsTypeDef(TypedDict):
    inputRecords: NotRequired[int],
    recordsNotProcessed: NotRequired[int],
    totalMappedRecords: NotRequired[int],
    totalMappedSourceRecords: NotRequired[int],
    totalMappedTargetRecords: NotRequired[int],
    totalRecordsProcessed: NotRequired[int],
```

## IdMappingJobOutputSourceTypeDef

```python
# IdMappingJobOutputSourceTypeDef definition

class IdMappingJobOutputSourceTypeDef(TypedDict):
    outputS3Path: str,
    roleArn: str,
    KMSArn: NotRequired[str],
```

## GetIdMappingWorkflowInputRequestTypeDef

```python
# GetIdMappingWorkflowInputRequestTypeDef definition

class GetIdMappingWorkflowInputRequestTypeDef(TypedDict):
    workflowName: str,
```

## GetIdNamespaceInputRequestTypeDef

```python
# GetIdNamespaceInputRequestTypeDef definition

class GetIdNamespaceInputRequestTypeDef(TypedDict):
    idNamespaceName: str,
```

## GetMatchIdInputRequestTypeDef

```python
# GetMatchIdInputRequestTypeDef definition

class GetMatchIdInputRequestTypeDef(TypedDict):
    record: Mapping[str, str],
    workflowName: str,
    applyNormalization: NotRequired[bool],
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

## JobOutputSourceTypeDef

```python
# JobOutputSourceTypeDef definition

class JobOutputSourceTypeDef(TypedDict):
    outputS3Path: str,
    roleArn: str,
    KMSArn: NotRequired[str],
```

## GetMatchingWorkflowInputRequestTypeDef

```python
# GetMatchingWorkflowInputRequestTypeDef definition

class GetMatchingWorkflowInputRequestTypeDef(TypedDict):
    workflowName: str,
```

## GetPolicyInputRequestTypeDef

```python
# GetPolicyInputRequestTypeDef definition

class GetPolicyInputRequestTypeDef(TypedDict):
    arn: str,
```

## GetProviderServiceInputRequestTypeDef

```python
# GetProviderServiceInputRequestTypeDef definition

class GetProviderServiceInputRequestTypeDef(TypedDict):
    providerName: str,
    providerServiceName: str,
```

## ProviderIdNameSpaceConfigurationTypeDef

```python
# ProviderIdNameSpaceConfigurationTypeDef definition

class ProviderIdNameSpaceConfigurationTypeDef(TypedDict):
    description: NotRequired[str],
    providerSourceConfigurationDefinition: NotRequired[Dict[str, Any]],
    providerTargetConfigurationDefinition: NotRequired[Dict[str, Any]],
```

## ProviderIntermediateDataAccessConfigurationTypeDef

```python
# ProviderIntermediateDataAccessConfigurationTypeDef definition

class ProviderIntermediateDataAccessConfigurationTypeDef(TypedDict):
    awsAccountIds: NotRequired[List[str]],
    requiredBucketActions: NotRequired[List[str]],
```

## GetSchemaMappingInputRequestTypeDef

```python
# GetSchemaMappingInputRequestTypeDef definition

class GetSchemaMappingInputRequestTypeDef(TypedDict):
    schemaName: str,
```

## RuleOutputTypeDef

```python
# RuleOutputTypeDef definition

class RuleOutputTypeDef(TypedDict):
    matchingKeys: List[str],
    ruleName: str,
```

## IdMappingWorkflowSummaryTypeDef

```python
# IdMappingWorkflowSummaryTypeDef definition

class IdMappingWorkflowSummaryTypeDef(TypedDict):
    createdAt: datetime,
    updatedAt: datetime,
    workflowArn: str,
    workflowName: str,
```

## IdNamespaceIdMappingWorkflowMetadataTypeDef

```python
# IdNamespaceIdMappingWorkflowMetadataTypeDef definition

class IdNamespaceIdMappingWorkflowMetadataTypeDef(TypedDict):
    idMappingType: IdMappingTypeType,  # (1)
```

1. See [:material-code-brackets: IdMappingTypeType](./literals.md#idmappingtypetype) 
## NamespaceProviderPropertiesOutputTypeDef

```python
# NamespaceProviderPropertiesOutputTypeDef definition

class NamespaceProviderPropertiesOutputTypeDef(TypedDict):
    providerServiceArn: str,
    providerConfiguration: NotRequired[Dict[str, Any]],
```

## IntermediateSourceConfigurationTypeDef

```python
# IntermediateSourceConfigurationTypeDef definition

class IntermediateSourceConfigurationTypeDef(TypedDict):
    intermediateS3Path: str,
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

## ListIdMappingJobsInputRequestTypeDef

```python
# ListIdMappingJobsInputRequestTypeDef definition

class ListIdMappingJobsInputRequestTypeDef(TypedDict):
    workflowName: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListIdMappingWorkflowsInputRequestTypeDef

```python
# ListIdMappingWorkflowsInputRequestTypeDef definition

class ListIdMappingWorkflowsInputRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListIdNamespacesInputRequestTypeDef

```python
# ListIdNamespacesInputRequestTypeDef definition

class ListIdNamespacesInputRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
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
    resolutionType: ResolutionTypeType,  # (1)
    updatedAt: datetime,
    workflowArn: str,
    workflowName: str,
```

1. See [:material-code-brackets: ResolutionTypeType](./literals.md#resolutiontypetype) 
## ListProviderServicesInputRequestTypeDef

```python
# ListProviderServicesInputRequestTypeDef definition

class ListProviderServicesInputRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    providerName: NotRequired[str],
```

## ProviderServiceSummaryTypeDef

```python
# ProviderServiceSummaryTypeDef definition

class ProviderServiceSummaryTypeDef(TypedDict):
    providerName: str,
    providerServiceArn: str,
    providerServiceDisplayName: str,
    providerServiceName: str,
    providerServiceType: ServiceTypeType,  # (1)
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
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
    hasWorkflows: bool,
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

## NamespaceProviderPropertiesTypeDef

```python
# NamespaceProviderPropertiesTypeDef definition

class NamespaceProviderPropertiesTypeDef(TypedDict):
    providerServiceArn: str,
    providerConfiguration: NotRequired[Mapping[str, Any]],
```

## OutputAttributeTypeDef

```python
# OutputAttributeTypeDef definition

class OutputAttributeTypeDef(TypedDict):
    name: str,
    hashed: NotRequired[bool],
```

## ProviderSchemaAttributeTypeDef

```python
# ProviderSchemaAttributeTypeDef definition

class ProviderSchemaAttributeTypeDef(TypedDict):
    fieldName: str,
    type: SchemaAttributeTypeType,  # (1)
    hashing: NotRequired[bool],
    subType: NotRequired[str],
```

1. See [:material-code-brackets: SchemaAttributeTypeType](./literals.md#schemaattributetypetype) 
## ProviderMarketplaceConfigurationTypeDef

```python
# ProviderMarketplaceConfigurationTypeDef definition

class ProviderMarketplaceConfigurationTypeDef(TypedDict):
    assetId: str,
    dataSetId: str,
    listingId: str,
    revisionId: str,
```

## PutPolicyInputRequestTypeDef

```python
# PutPolicyInputRequestTypeDef definition

class PutPolicyInputRequestTypeDef(TypedDict):
    arn: str,
    policy: str,
    token: NotRequired[str],
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

## AddPolicyStatementOutputTypeDef

```python
# AddPolicyStatementOutputTypeDef definition

class AddPolicyStatementOutputTypeDef(TypedDict):
    arn: str,
    policy: str,
    token: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteIdMappingWorkflowOutputTypeDef

```python
# DeleteIdMappingWorkflowOutputTypeDef definition

class DeleteIdMappingWorkflowOutputTypeDef(TypedDict):
    message: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteIdNamespaceOutputTypeDef

```python
# DeleteIdNamespaceOutputTypeDef definition

class DeleteIdNamespaceOutputTypeDef(TypedDict):
    message: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteMatchingWorkflowOutputTypeDef

```python
# DeleteMatchingWorkflowOutputTypeDef definition

class DeleteMatchingWorkflowOutputTypeDef(TypedDict):
    message: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeletePolicyStatementOutputTypeDef

```python
# DeletePolicyStatementOutputTypeDef definition

class DeletePolicyStatementOutputTypeDef(TypedDict):
    arn: str,
    policy: str,
    token: str,
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
    matchRule: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPolicyOutputTypeDef

```python
# GetPolicyOutputTypeDef definition

class GetPolicyOutputTypeDef(TypedDict):
    arn: str,
    policy: str,
    token: str,
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
## PutPolicyOutputTypeDef

```python
# PutPolicyOutputTypeDef definition

class PutPolicyOutputTypeDef(TypedDict):
    arn: str,
    policy: str,
    token: str,
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
## BatchDeleteUniqueIdOutputTypeDef

```python
# BatchDeleteUniqueIdOutputTypeDef definition

class BatchDeleteUniqueIdOutputTypeDef(TypedDict):
    deleted: List[DeletedUniqueIdTypeDef],  # (1)
    disconnectedUniqueIds: List[str],
    errors: List[DeleteUniqueIdErrorTypeDef],  # (2)
    status: DeleteUniqueIdStatusType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: DeletedUniqueIdTypeDef](./type_defs.md#deleteduniqueidtypedef) 
2. See [:material-code-braces: DeleteUniqueIdErrorTypeDef](./type_defs.md#deleteuniqueiderrortypedef) 
3. See [:material-code-brackets: DeleteUniqueIdStatusType](./literals.md#deleteuniqueidstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSchemaMappingInputRequestTypeDef

```python
# CreateSchemaMappingInputRequestTypeDef definition

class CreateSchemaMappingInputRequestTypeDef(TypedDict):
    mappedInputFields: Sequence[SchemaInputAttributeTypeDef],  # (1)
    schemaName: str,
    description: NotRequired[str],
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
    hasWorkflows: bool,
    mappedInputFields: List[SchemaInputAttributeTypeDef],  # (1)
    schemaArn: str,
    schemaName: str,
    tags: Dict[str, str],
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SchemaInputAttributeTypeDef](./type_defs.md#schemainputattributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSchemaMappingInputRequestTypeDef

```python
# UpdateSchemaMappingInputRequestTypeDef definition

class UpdateSchemaMappingInputRequestTypeDef(TypedDict):
    mappedInputFields: Sequence[SchemaInputAttributeTypeDef],  # (1)
    schemaName: str,
    description: NotRequired[str],
```

1. See [:material-code-braces: SchemaInputAttributeTypeDef](./type_defs.md#schemainputattributetypedef) 
## UpdateSchemaMappingOutputTypeDef

```python
# UpdateSchemaMappingOutputTypeDef definition

class UpdateSchemaMappingOutputTypeDef(TypedDict):
    description: str,
    mappedInputFields: List[SchemaInputAttributeTypeDef],  # (1)
    schemaArn: str,
    schemaName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SchemaInputAttributeTypeDef](./type_defs.md#schemainputattributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIdMappingJobOutputTypeDef

```python
# GetIdMappingJobOutputTypeDef definition

class GetIdMappingJobOutputTypeDef(TypedDict):
    endTime: datetime,
    errorDetails: ErrorDetailsTypeDef,  # (1)
    jobId: str,
    metrics: IdMappingJobMetricsTypeDef,  # (2)
    outputSourceConfig: List[IdMappingJobOutputSourceTypeDef],  # (3)
    startTime: datetime,
    status: JobStatusType,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef) 
2. See [:material-code-braces: IdMappingJobMetricsTypeDef](./type_defs.md#idmappingjobmetricstypedef) 
3. See [:material-code-braces: IdMappingJobOutputSourceTypeDef](./type_defs.md#idmappingjoboutputsourcetypedef) 
4. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartIdMappingJobInputRequestTypeDef

```python
# StartIdMappingJobInputRequestTypeDef definition

class StartIdMappingJobInputRequestTypeDef(TypedDict):
    workflowName: str,
    outputSourceConfig: NotRequired[Sequence[IdMappingJobOutputSourceTypeDef]],  # (1)
```

1. See [:material-code-braces: IdMappingJobOutputSourceTypeDef](./type_defs.md#idmappingjoboutputsourcetypedef) 
## StartIdMappingJobOutputTypeDef

```python
# StartIdMappingJobOutputTypeDef definition

class StartIdMappingJobOutputTypeDef(TypedDict):
    jobId: str,
    outputSourceConfig: List[IdMappingJobOutputSourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdMappingJobOutputSourceTypeDef](./type_defs.md#idmappingjoboutputsourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMatchingJobOutputTypeDef

```python
# GetMatchingJobOutputTypeDef definition

class GetMatchingJobOutputTypeDef(TypedDict):
    endTime: datetime,
    errorDetails: ErrorDetailsTypeDef,  # (1)
    jobId: str,
    metrics: JobMetricsTypeDef,  # (2)
    outputSourceConfig: List[JobOutputSourceTypeDef],  # (3)
    startTime: datetime,
    status: JobStatusType,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef) 
2. See [:material-code-braces: JobMetricsTypeDef](./type_defs.md#jobmetricstypedef) 
3. See [:material-code-braces: JobOutputSourceTypeDef](./type_defs.md#joboutputsourcetypedef) 
4. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IdMappingRuleBasedPropertiesOutputTypeDef

```python
# IdMappingRuleBasedPropertiesOutputTypeDef definition

class IdMappingRuleBasedPropertiesOutputTypeDef(TypedDict):
    attributeMatchingModel: AttributeMatchingModelType,  # (1)
    recordMatchingModel: RecordMatchingModelType,  # (2)
    ruleDefinitionType: IdMappingWorkflowRuleDefinitionTypeType,  # (3)
    rules: NotRequired[List[RuleOutputTypeDef]],  # (4)
```

1. See [:material-code-brackets: AttributeMatchingModelType](./literals.md#attributematchingmodeltype) 
2. See [:material-code-brackets: RecordMatchingModelType](./literals.md#recordmatchingmodeltype) 
3. See [:material-code-brackets: IdMappingWorkflowRuleDefinitionTypeType](./literals.md#idmappingworkflowruledefinitiontypetype) 
4. See [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 
## NamespaceRuleBasedPropertiesOutputTypeDef

```python
# NamespaceRuleBasedPropertiesOutputTypeDef definition

class NamespaceRuleBasedPropertiesOutputTypeDef(TypedDict):
    attributeMatchingModel: NotRequired[AttributeMatchingModelType],  # (1)
    recordMatchingModels: NotRequired[List[RecordMatchingModelType]],  # (2)
    ruleDefinitionTypes: NotRequired[List[IdMappingWorkflowRuleDefinitionTypeType]],  # (3)
    rules: NotRequired[List[RuleOutputTypeDef]],  # (4)
```

1. See [:material-code-brackets: AttributeMatchingModelType](./literals.md#attributematchingmodeltype) 
2. See [:material-code-brackets: RecordMatchingModelType](./literals.md#recordmatchingmodeltype) 
3. See [:material-code-brackets: IdMappingWorkflowRuleDefinitionTypeType](./literals.md#idmappingworkflowruledefinitiontypetype) 
4. See [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 
## RuleBasedPropertiesOutputTypeDef

```python
# RuleBasedPropertiesOutputTypeDef definition

class RuleBasedPropertiesOutputTypeDef(TypedDict):
    attributeMatchingModel: AttributeMatchingModelType,  # (1)
    rules: List[RuleOutputTypeDef],  # (3)
    matchPurpose: NotRequired[MatchPurposeType],  # (2)
```

1. See [:material-code-brackets: AttributeMatchingModelType](./literals.md#attributematchingmodeltype) 
2. See [:material-code-brackets: MatchPurposeType](./literals.md#matchpurposetype) 
3. See [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 
## ListIdMappingWorkflowsOutputTypeDef

```python
# ListIdMappingWorkflowsOutputTypeDef definition

class ListIdMappingWorkflowsOutputTypeDef(TypedDict):
    workflowSummaries: List[IdMappingWorkflowSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: IdMappingWorkflowSummaryTypeDef](./type_defs.md#idmappingworkflowsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IdNamespaceSummaryTypeDef

```python
# IdNamespaceSummaryTypeDef definition

class IdNamespaceSummaryTypeDef(TypedDict):
    createdAt: datetime,
    idNamespaceArn: str,
    idNamespaceName: str,
    type: IdNamespaceTypeType,  # (2)
    updatedAt: datetime,
    description: NotRequired[str],
    idMappingWorkflowProperties: NotRequired[List[IdNamespaceIdMappingWorkflowMetadataTypeDef]],  # (1)
```

1. See [:material-code-braces: IdNamespaceIdMappingWorkflowMetadataTypeDef](./type_defs.md#idnamespaceidmappingworkflowmetadatatypedef) 
2. See [:material-code-brackets: IdNamespaceTypeType](./literals.md#idnamespacetypetype) 
## ProviderPropertiesOutputTypeDef

```python
# ProviderPropertiesOutputTypeDef definition

class ProviderPropertiesOutputTypeDef(TypedDict):
    providerServiceArn: str,
    intermediateSourceConfiguration: NotRequired[IntermediateSourceConfigurationTypeDef],  # (1)
    providerConfiguration: NotRequired[Dict[str, Any]],
```

1. See [:material-code-braces: IntermediateSourceConfigurationTypeDef](./type_defs.md#intermediatesourceconfigurationtypedef) 
## ProviderPropertiesTypeDef

```python
# ProviderPropertiesTypeDef definition

class ProviderPropertiesTypeDef(TypedDict):
    providerServiceArn: str,
    intermediateSourceConfiguration: NotRequired[IntermediateSourceConfigurationTypeDef],  # (1)
    providerConfiguration: NotRequired[Mapping[str, Any]],
```

1. See [:material-code-braces: IntermediateSourceConfigurationTypeDef](./type_defs.md#intermediatesourceconfigurationtypedef) 
## ListIdMappingJobsOutputTypeDef

```python
# ListIdMappingJobsOutputTypeDef definition

class ListIdMappingJobsOutputTypeDef(TypedDict):
    jobs: List[JobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: JobSummaryTypeDef](./type_defs.md#jobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMatchingJobsOutputTypeDef

```python
# ListMatchingJobsOutputTypeDef definition

class ListMatchingJobsOutputTypeDef(TypedDict):
    jobs: List[JobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: JobSummaryTypeDef](./type_defs.md#jobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIdMappingJobsInputListIdMappingJobsPaginateTypeDef

```python
# ListIdMappingJobsInputListIdMappingJobsPaginateTypeDef definition

class ListIdMappingJobsInputListIdMappingJobsPaginateTypeDef(TypedDict):
    workflowName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIdMappingWorkflowsInputListIdMappingWorkflowsPaginateTypeDef

```python
# ListIdMappingWorkflowsInputListIdMappingWorkflowsPaginateTypeDef definition

class ListIdMappingWorkflowsInputListIdMappingWorkflowsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIdNamespacesInputListIdNamespacesPaginateTypeDef

```python
# ListIdNamespacesInputListIdNamespacesPaginateTypeDef definition

class ListIdNamespacesInputListIdNamespacesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
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
## ListProviderServicesInputListProviderServicesPaginateTypeDef

```python
# ListProviderServicesInputListProviderServicesPaginateTypeDef definition

class ListProviderServicesInputListProviderServicesPaginateTypeDef(TypedDict):
    providerName: NotRequired[str],
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
    workflowSummaries: List[MatchingWorkflowSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: MatchingWorkflowSummaryTypeDef](./type_defs.md#matchingworkflowsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProviderServicesOutputTypeDef

```python
# ListProviderServicesOutputTypeDef definition

class ListProviderServicesOutputTypeDef(TypedDict):
    providerServiceSummaries: List[ProviderServiceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ProviderServiceSummaryTypeDef](./type_defs.md#providerservicesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSchemaMappingsOutputTypeDef

```python
# ListSchemaMappingsOutputTypeDef definition

class ListSchemaMappingsOutputTypeDef(TypedDict):
    schemaList: List[SchemaMappingSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SchemaMappingSummaryTypeDef](./type_defs.md#schemamappingsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OutputSourceOutputTypeDef

```python
# OutputSourceOutputTypeDef definition

class OutputSourceOutputTypeDef(TypedDict):
    output: List[OutputAttributeTypeDef],  # (1)
    outputS3Path: str,
    KMSArn: NotRequired[str],
    applyNormalization: NotRequired[bool],
```

1. See [:material-code-braces: OutputAttributeTypeDef](./type_defs.md#outputattributetypedef) 
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
## ProviderComponentSchemaTypeDef

```python
# ProviderComponentSchemaTypeDef definition

class ProviderComponentSchemaTypeDef(TypedDict):
    providerSchemaAttributes: NotRequired[List[ProviderSchemaAttributeTypeDef]],  # (1)
    schemas: NotRequired[List[List[str]]],
```

1. See [:material-code-braces: ProviderSchemaAttributeTypeDef](./type_defs.md#providerschemaattributetypedef) 
## ProviderEndpointConfigurationTypeDef

```python
# ProviderEndpointConfigurationTypeDef definition

class ProviderEndpointConfigurationTypeDef(TypedDict):
    marketplaceConfiguration: NotRequired[ProviderMarketplaceConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ProviderMarketplaceConfigurationTypeDef](./type_defs.md#providermarketplaceconfigurationtypedef) 
## IdNamespaceIdMappingWorkflowPropertiesOutputTypeDef

```python
# IdNamespaceIdMappingWorkflowPropertiesOutputTypeDef definition

class IdNamespaceIdMappingWorkflowPropertiesOutputTypeDef(TypedDict):
    idMappingType: IdMappingTypeType,  # (1)
    providerProperties: NotRequired[NamespaceProviderPropertiesOutputTypeDef],  # (2)
    ruleBasedProperties: NotRequired[NamespaceRuleBasedPropertiesOutputTypeDef],  # (3)
```

1. See [:material-code-brackets: IdMappingTypeType](./literals.md#idmappingtypetype) 
2. See [:material-code-braces: NamespaceProviderPropertiesOutputTypeDef](./type_defs.md#namespaceproviderpropertiesoutputtypedef) 
3. See [:material-code-braces: NamespaceRuleBasedPropertiesOutputTypeDef](./type_defs.md#namespacerulebasedpropertiesoutputtypedef) 
## ListIdNamespacesOutputTypeDef

```python
# ListIdNamespacesOutputTypeDef definition

class ListIdNamespacesOutputTypeDef(TypedDict):
    idNamespaceSummaries: List[IdNamespaceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: IdNamespaceSummaryTypeDef](./type_defs.md#idnamespacesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IdMappingTechniquesOutputTypeDef

```python
# IdMappingTechniquesOutputTypeDef definition

class IdMappingTechniquesOutputTypeDef(TypedDict):
    idMappingType: IdMappingTypeType,  # (1)
    providerProperties: NotRequired[ProviderPropertiesOutputTypeDef],  # (2)
    ruleBasedProperties: NotRequired[IdMappingRuleBasedPropertiesOutputTypeDef],  # (3)
```

1. See [:material-code-brackets: IdMappingTypeType](./literals.md#idmappingtypetype) 
2. See [:material-code-braces: ProviderPropertiesOutputTypeDef](./type_defs.md#providerpropertiesoutputtypedef) 
3. See [:material-code-braces: IdMappingRuleBasedPropertiesOutputTypeDef](./type_defs.md#idmappingrulebasedpropertiesoutputtypedef) 
## ResolutionTechniquesOutputTypeDef

```python
# ResolutionTechniquesOutputTypeDef definition

class ResolutionTechniquesOutputTypeDef(TypedDict):
    resolutionType: ResolutionTypeType,  # (2)
    providerProperties: NotRequired[ProviderPropertiesOutputTypeDef],  # (1)
    ruleBasedProperties: NotRequired[RuleBasedPropertiesOutputTypeDef],  # (3)
```

1. See [:material-code-braces: ProviderPropertiesOutputTypeDef](./type_defs.md#providerpropertiesoutputtypedef) 
2. See [:material-code-brackets: ResolutionTypeType](./literals.md#resolutiontypetype) 
3. See [:material-code-braces: RuleBasedPropertiesOutputTypeDef](./type_defs.md#rulebasedpropertiesoutputtypedef) 
## GetProviderServiceOutputTypeDef

```python
# GetProviderServiceOutputTypeDef definition

class GetProviderServiceOutputTypeDef(TypedDict):
    anonymizedOutput: bool,
    providerComponentSchema: ProviderComponentSchemaTypeDef,  # (1)
    providerConfigurationDefinition: Dict[str, Any],
    providerEndpointConfiguration: ProviderEndpointConfigurationTypeDef,  # (2)
    providerEntityOutputDefinition: Dict[str, Any],
    providerIdNameSpaceConfiguration: ProviderIdNameSpaceConfigurationTypeDef,  # (3)
    providerIntermediateDataAccessConfiguration: ProviderIntermediateDataAccessConfigurationTypeDef,  # (4)
    providerJobConfiguration: Dict[str, Any],
    providerName: str,
    providerServiceArn: str,
    providerServiceDisplayName: str,
    providerServiceName: str,
    providerServiceType: ServiceTypeType,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: ProviderComponentSchemaTypeDef](./type_defs.md#providercomponentschematypedef) 
2. See [:material-code-braces: ProviderEndpointConfigurationTypeDef](./type_defs.md#providerendpointconfigurationtypedef) 
3. See [:material-code-braces: ProviderIdNameSpaceConfigurationTypeDef](./type_defs.md#provideridnamespaceconfigurationtypedef) 
4. See [:material-code-braces: ProviderIntermediateDataAccessConfigurationTypeDef](./type_defs.md#providerintermediatedataaccessconfigurationtypedef) 
5. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IdMappingRuleBasedPropertiesTypeDef

```python
# IdMappingRuleBasedPropertiesTypeDef definition

class IdMappingRuleBasedPropertiesTypeDef(TypedDict):
    attributeMatchingModel: AttributeMatchingModelType,  # (1)
    recordMatchingModel: RecordMatchingModelType,  # (2)
    ruleDefinitionType: IdMappingWorkflowRuleDefinitionTypeType,  # (3)
    rules: NotRequired[Sequence[RuleUnionTypeDef]],  # (4)
```

1. See [:material-code-brackets: AttributeMatchingModelType](./literals.md#attributematchingmodeltype) 
2. See [:material-code-brackets: RecordMatchingModelType](./literals.md#recordmatchingmodeltype) 
3. See [:material-code-brackets: IdMappingWorkflowRuleDefinitionTypeType](./literals.md#idmappingworkflowruledefinitiontypetype) 
4. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 
## NamespaceRuleBasedPropertiesTypeDef

```python
# NamespaceRuleBasedPropertiesTypeDef definition

class NamespaceRuleBasedPropertiesTypeDef(TypedDict):
    attributeMatchingModel: NotRequired[AttributeMatchingModelType],  # (1)
    recordMatchingModels: NotRequired[Sequence[RecordMatchingModelType]],  # (2)
    ruleDefinitionTypes: NotRequired[Sequence[IdMappingWorkflowRuleDefinitionTypeType]],  # (3)
    rules: NotRequired[Sequence[RuleUnionTypeDef]],  # (4)
```

1. See [:material-code-brackets: AttributeMatchingModelType](./literals.md#attributematchingmodeltype) 
2. See [:material-code-brackets: RecordMatchingModelType](./literals.md#recordmatchingmodeltype) 
3. See [:material-code-brackets: IdMappingWorkflowRuleDefinitionTypeType](./literals.md#idmappingworkflowruledefinitiontypetype) 
4. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 
## RuleBasedPropertiesTypeDef

```python
# RuleBasedPropertiesTypeDef definition

class RuleBasedPropertiesTypeDef(TypedDict):
    attributeMatchingModel: AttributeMatchingModelType,  # (1)
    rules: Sequence[RuleUnionTypeDef],  # (3)
    matchPurpose: NotRequired[MatchPurposeType],  # (2)
```

1. See [:material-code-brackets: AttributeMatchingModelType](./literals.md#attributematchingmodeltype) 
2. See [:material-code-brackets: MatchPurposeType](./literals.md#matchpurposetype) 
3. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 
## CreateIdNamespaceOutputTypeDef

```python
# CreateIdNamespaceOutputTypeDef definition

class CreateIdNamespaceOutputTypeDef(TypedDict):
    createdAt: datetime,
    description: str,
    idMappingWorkflowProperties: List[IdNamespaceIdMappingWorkflowPropertiesOutputTypeDef],  # (1)
    idNamespaceArn: str,
    idNamespaceName: str,
    inputSourceConfig: List[IdNamespaceInputSourceTypeDef],  # (2)
    roleArn: str,
    tags: Dict[str, str],
    type: IdNamespaceTypeType,  # (3)
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: IdNamespaceIdMappingWorkflowPropertiesOutputTypeDef](./type_defs.md#idnamespaceidmappingworkflowpropertiesoutputtypedef) 
2. See [:material-code-braces: IdNamespaceInputSourceTypeDef](./type_defs.md#idnamespaceinputsourcetypedef) 
3. See [:material-code-brackets: IdNamespaceTypeType](./literals.md#idnamespacetypetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIdNamespaceOutputTypeDef

```python
# GetIdNamespaceOutputTypeDef definition

class GetIdNamespaceOutputTypeDef(TypedDict):
    createdAt: datetime,
    description: str,
    idMappingWorkflowProperties: List[IdNamespaceIdMappingWorkflowPropertiesOutputTypeDef],  # (1)
    idNamespaceArn: str,
    idNamespaceName: str,
    inputSourceConfig: List[IdNamespaceInputSourceTypeDef],  # (2)
    roleArn: str,
    tags: Dict[str, str],
    type: IdNamespaceTypeType,  # (3)
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: IdNamespaceIdMappingWorkflowPropertiesOutputTypeDef](./type_defs.md#idnamespaceidmappingworkflowpropertiesoutputtypedef) 
2. See [:material-code-braces: IdNamespaceInputSourceTypeDef](./type_defs.md#idnamespaceinputsourcetypedef) 
3. See [:material-code-brackets: IdNamespaceTypeType](./literals.md#idnamespacetypetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateIdNamespaceOutputTypeDef

```python
# UpdateIdNamespaceOutputTypeDef definition

class UpdateIdNamespaceOutputTypeDef(TypedDict):
    createdAt: datetime,
    description: str,
    idMappingWorkflowProperties: List[IdNamespaceIdMappingWorkflowPropertiesOutputTypeDef],  # (1)
    idNamespaceArn: str,
    idNamespaceName: str,
    inputSourceConfig: List[IdNamespaceInputSourceTypeDef],  # (2)
    roleArn: str,
    type: IdNamespaceTypeType,  # (3)
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: IdNamespaceIdMappingWorkflowPropertiesOutputTypeDef](./type_defs.md#idnamespaceidmappingworkflowpropertiesoutputtypedef) 
2. See [:material-code-braces: IdNamespaceInputSourceTypeDef](./type_defs.md#idnamespaceinputsourcetypedef) 
3. See [:material-code-brackets: IdNamespaceTypeType](./literals.md#idnamespacetypetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateIdMappingWorkflowOutputTypeDef

```python
# CreateIdMappingWorkflowOutputTypeDef definition

class CreateIdMappingWorkflowOutputTypeDef(TypedDict):
    description: str,
    idMappingTechniques: IdMappingTechniquesOutputTypeDef,  # (1)
    inputSourceConfig: List[IdMappingWorkflowInputSourceTypeDef],  # (2)
    outputSourceConfig: List[IdMappingWorkflowOutputSourceTypeDef],  # (3)
    roleArn: str,
    workflowArn: str,
    workflowName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: IdMappingTechniquesOutputTypeDef](./type_defs.md#idmappingtechniquesoutputtypedef) 
2. See [:material-code-braces: IdMappingWorkflowInputSourceTypeDef](./type_defs.md#idmappingworkflowinputsourcetypedef) 
3. See [:material-code-braces: IdMappingWorkflowOutputSourceTypeDef](./type_defs.md#idmappingworkflowoutputsourcetypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIdMappingWorkflowOutputTypeDef

```python
# GetIdMappingWorkflowOutputTypeDef definition

class GetIdMappingWorkflowOutputTypeDef(TypedDict):
    createdAt: datetime,
    description: str,
    idMappingTechniques: IdMappingTechniquesOutputTypeDef,  # (1)
    inputSourceConfig: List[IdMappingWorkflowInputSourceTypeDef],  # (2)
    outputSourceConfig: List[IdMappingWorkflowOutputSourceTypeDef],  # (3)
    roleArn: str,
    tags: Dict[str, str],
    updatedAt: datetime,
    workflowArn: str,
    workflowName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: IdMappingTechniquesOutputTypeDef](./type_defs.md#idmappingtechniquesoutputtypedef) 
2. See [:material-code-braces: IdMappingWorkflowInputSourceTypeDef](./type_defs.md#idmappingworkflowinputsourcetypedef) 
3. See [:material-code-braces: IdMappingWorkflowOutputSourceTypeDef](./type_defs.md#idmappingworkflowoutputsourcetypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateIdMappingWorkflowOutputTypeDef

```python
# UpdateIdMappingWorkflowOutputTypeDef definition

class UpdateIdMappingWorkflowOutputTypeDef(TypedDict):
    description: str,
    idMappingTechniques: IdMappingTechniquesOutputTypeDef,  # (1)
    inputSourceConfig: List[IdMappingWorkflowInputSourceTypeDef],  # (2)
    outputSourceConfig: List[IdMappingWorkflowOutputSourceTypeDef],  # (3)
    roleArn: str,
    workflowArn: str,
    workflowName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: IdMappingTechniquesOutputTypeDef](./type_defs.md#idmappingtechniquesoutputtypedef) 
2. See [:material-code-braces: IdMappingWorkflowInputSourceTypeDef](./type_defs.md#idmappingworkflowinputsourcetypedef) 
3. See [:material-code-braces: IdMappingWorkflowOutputSourceTypeDef](./type_defs.md#idmappingworkflowoutputsourcetypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMatchingWorkflowOutputTypeDef

```python
# CreateMatchingWorkflowOutputTypeDef definition

class CreateMatchingWorkflowOutputTypeDef(TypedDict):
    description: str,
    incrementalRunConfig: IncrementalRunConfigTypeDef,  # (1)
    inputSourceConfig: List[InputSourceTypeDef],  # (2)
    outputSourceConfig: List[OutputSourceOutputTypeDef],  # (3)
    resolutionTechniques: ResolutionTechniquesOutputTypeDef,  # (4)
    roleArn: str,
    workflowArn: str,
    workflowName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: IncrementalRunConfigTypeDef](./type_defs.md#incrementalrunconfigtypedef) 
2. See [:material-code-braces: InputSourceTypeDef](./type_defs.md#inputsourcetypedef) 
3. See [:material-code-braces: OutputSourceOutputTypeDef](./type_defs.md#outputsourceoutputtypedef) 
4. See [:material-code-braces: ResolutionTechniquesOutputTypeDef](./type_defs.md#resolutiontechniquesoutputtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMatchingWorkflowOutputTypeDef

```python
# GetMatchingWorkflowOutputTypeDef definition

class GetMatchingWorkflowOutputTypeDef(TypedDict):
    createdAt: datetime,
    description: str,
    incrementalRunConfig: IncrementalRunConfigTypeDef,  # (1)
    inputSourceConfig: List[InputSourceTypeDef],  # (2)
    outputSourceConfig: List[OutputSourceOutputTypeDef],  # (3)
    resolutionTechniques: ResolutionTechniquesOutputTypeDef,  # (4)
    roleArn: str,
    tags: Dict[str, str],
    updatedAt: datetime,
    workflowArn: str,
    workflowName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: IncrementalRunConfigTypeDef](./type_defs.md#incrementalrunconfigtypedef) 
2. See [:material-code-braces: InputSourceTypeDef](./type_defs.md#inputsourcetypedef) 
3. See [:material-code-braces: OutputSourceOutputTypeDef](./type_defs.md#outputsourceoutputtypedef) 
4. See [:material-code-braces: ResolutionTechniquesOutputTypeDef](./type_defs.md#resolutiontechniquesoutputtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMatchingWorkflowOutputTypeDef

```python
# UpdateMatchingWorkflowOutputTypeDef definition

class UpdateMatchingWorkflowOutputTypeDef(TypedDict):
    description: str,
    incrementalRunConfig: IncrementalRunConfigTypeDef,  # (1)
    inputSourceConfig: List[InputSourceTypeDef],  # (2)
    outputSourceConfig: List[OutputSourceOutputTypeDef],  # (3)
    resolutionTechniques: ResolutionTechniquesOutputTypeDef,  # (4)
    roleArn: str,
    workflowName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: IncrementalRunConfigTypeDef](./type_defs.md#incrementalrunconfigtypedef) 
2. See [:material-code-braces: InputSourceTypeDef](./type_defs.md#inputsourcetypedef) 
3. See [:material-code-braces: OutputSourceOutputTypeDef](./type_defs.md#outputsourceoutputtypedef) 
4. See [:material-code-braces: ResolutionTechniquesOutputTypeDef](./type_defs.md#resolutiontechniquesoutputtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IdMappingTechniquesTypeDef

```python
# IdMappingTechniquesTypeDef definition

class IdMappingTechniquesTypeDef(TypedDict):
    idMappingType: IdMappingTypeType,  # (1)
    providerProperties: NotRequired[ProviderPropertiesUnionTypeDef],  # (2)
    ruleBasedProperties: NotRequired[IdMappingRuleBasedPropertiesUnionTypeDef],  # (3)
```

1. See [:material-code-brackets: IdMappingTypeType](./literals.md#idmappingtypetype) 
2. See [:material-code-braces: ProviderPropertiesTypeDef](./type_defs.md#providerpropertiestypedef) [:material-code-braces: ProviderPropertiesOutputTypeDef](./type_defs.md#providerpropertiesoutputtypedef) 
3. See [:material-code-braces: IdMappingRuleBasedPropertiesTypeDef](./type_defs.md#idmappingrulebasedpropertiestypedef) [:material-code-braces: IdMappingRuleBasedPropertiesOutputTypeDef](./type_defs.md#idmappingrulebasedpropertiesoutputtypedef) 
## IdNamespaceIdMappingWorkflowPropertiesTypeDef

```python
# IdNamespaceIdMappingWorkflowPropertiesTypeDef definition

class IdNamespaceIdMappingWorkflowPropertiesTypeDef(TypedDict):
    idMappingType: IdMappingTypeType,  # (1)
    providerProperties: NotRequired[NamespaceProviderPropertiesUnionTypeDef],  # (2)
    ruleBasedProperties: NotRequired[NamespaceRuleBasedPropertiesUnionTypeDef],  # (3)
```

1. See [:material-code-brackets: IdMappingTypeType](./literals.md#idmappingtypetype) 
2. See [:material-code-braces: NamespaceProviderPropertiesTypeDef](./type_defs.md#namespaceproviderpropertiestypedef) [:material-code-braces: NamespaceProviderPropertiesOutputTypeDef](./type_defs.md#namespaceproviderpropertiesoutputtypedef) 
3. See [:material-code-braces: NamespaceRuleBasedPropertiesTypeDef](./type_defs.md#namespacerulebasedpropertiestypedef) [:material-code-braces: NamespaceRuleBasedPropertiesOutputTypeDef](./type_defs.md#namespacerulebasedpropertiesoutputtypedef) 
## ResolutionTechniquesTypeDef

```python
# ResolutionTechniquesTypeDef definition

class ResolutionTechniquesTypeDef(TypedDict):
    resolutionType: ResolutionTypeType,  # (2)
    providerProperties: NotRequired[ProviderPropertiesUnionTypeDef],  # (1)
    ruleBasedProperties: NotRequired[RuleBasedPropertiesUnionTypeDef],  # (3)
```

1. See [:material-code-braces: ProviderPropertiesTypeDef](./type_defs.md#providerpropertiestypedef) [:material-code-braces: ProviderPropertiesOutputTypeDef](./type_defs.md#providerpropertiesoutputtypedef) 
2. See [:material-code-brackets: ResolutionTypeType](./literals.md#resolutiontypetype) 
3. See [:material-code-braces: RuleBasedPropertiesTypeDef](./type_defs.md#rulebasedpropertiestypedef) [:material-code-braces: RuleBasedPropertiesOutputTypeDef](./type_defs.md#rulebasedpropertiesoutputtypedef) 
## CreateIdMappingWorkflowInputRequestTypeDef

```python
# CreateIdMappingWorkflowInputRequestTypeDef definition

class CreateIdMappingWorkflowInputRequestTypeDef(TypedDict):
    idMappingTechniques: IdMappingTechniquesTypeDef,  # (1)
    inputSourceConfig: Sequence[IdMappingWorkflowInputSourceTypeDef],  # (2)
    workflowName: str,
    description: NotRequired[str],
    outputSourceConfig: NotRequired[Sequence[IdMappingWorkflowOutputSourceTypeDef]],  # (3)
    roleArn: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: IdMappingTechniquesTypeDef](./type_defs.md#idmappingtechniquestypedef) 
2. See [:material-code-braces: IdMappingWorkflowInputSourceTypeDef](./type_defs.md#idmappingworkflowinputsourcetypedef) 
3. See [:material-code-braces: IdMappingWorkflowOutputSourceTypeDef](./type_defs.md#idmappingworkflowoutputsourcetypedef) 
## UpdateIdMappingWorkflowInputRequestTypeDef

```python
# UpdateIdMappingWorkflowInputRequestTypeDef definition

class UpdateIdMappingWorkflowInputRequestTypeDef(TypedDict):
    idMappingTechniques: IdMappingTechniquesTypeDef,  # (1)
    inputSourceConfig: Sequence[IdMappingWorkflowInputSourceTypeDef],  # (2)
    workflowName: str,
    description: NotRequired[str],
    outputSourceConfig: NotRequired[Sequence[IdMappingWorkflowOutputSourceTypeDef]],  # (3)
    roleArn: NotRequired[str],
```

1. See [:material-code-braces: IdMappingTechniquesTypeDef](./type_defs.md#idmappingtechniquestypedef) 
2. See [:material-code-braces: IdMappingWorkflowInputSourceTypeDef](./type_defs.md#idmappingworkflowinputsourcetypedef) 
3. See [:material-code-braces: IdMappingWorkflowOutputSourceTypeDef](./type_defs.md#idmappingworkflowoutputsourcetypedef) 
## UpdateIdNamespaceInputRequestTypeDef

```python
# UpdateIdNamespaceInputRequestTypeDef definition

class UpdateIdNamespaceInputRequestTypeDef(TypedDict):
    idNamespaceName: str,
    description: NotRequired[str],
    idMappingWorkflowProperties: NotRequired[Sequence[IdNamespaceIdMappingWorkflowPropertiesTypeDef]],  # (1)
    inputSourceConfig: NotRequired[Sequence[IdNamespaceInputSourceTypeDef]],  # (2)
    roleArn: NotRequired[str],
```

1. See [:material-code-braces: IdNamespaceIdMappingWorkflowPropertiesTypeDef](./type_defs.md#idnamespaceidmappingworkflowpropertiestypedef) 
2. See [:material-code-braces: IdNamespaceInputSourceTypeDef](./type_defs.md#idnamespaceinputsourcetypedef) 
## CreateMatchingWorkflowInputRequestTypeDef

```python
# CreateMatchingWorkflowInputRequestTypeDef definition

class CreateMatchingWorkflowInputRequestTypeDef(TypedDict):
    inputSourceConfig: Sequence[InputSourceTypeDef],  # (1)
    outputSourceConfig: Sequence[OutputSourceUnionTypeDef],  # (2)
    resolutionTechniques: ResolutionTechniquesTypeDef,  # (3)
    roleArn: str,
    workflowName: str,
    description: NotRequired[str],
    incrementalRunConfig: NotRequired[IncrementalRunConfigTypeDef],  # (4)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: InputSourceTypeDef](./type_defs.md#inputsourcetypedef) 
2. See [:material-code-braces: OutputSourceTypeDef](./type_defs.md#outputsourcetypedef) [:material-code-braces: OutputSourceOutputTypeDef](./type_defs.md#outputsourceoutputtypedef) 
3. See [:material-code-braces: ResolutionTechniquesTypeDef](./type_defs.md#resolutiontechniquestypedef) 
4. See [:material-code-braces: IncrementalRunConfigTypeDef](./type_defs.md#incrementalrunconfigtypedef) 
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
## CreateIdNamespaceInputRequestTypeDef

```python
# CreateIdNamespaceInputRequestTypeDef definition

class CreateIdNamespaceInputRequestTypeDef(TypedDict):
    idNamespaceName: str,
    type: IdNamespaceTypeType,  # (1)
    description: NotRequired[str],
    idMappingWorkflowProperties: NotRequired[Sequence[IdNamespaceIdMappingWorkflowPropertiesUnionTypeDef]],  # (2)
    inputSourceConfig: NotRequired[Sequence[IdNamespaceInputSourceTypeDef]],  # (3)
    roleArn: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: IdNamespaceTypeType](./literals.md#idnamespacetypetype) 
2. See [:material-code-braces: IdNamespaceIdMappingWorkflowPropertiesTypeDef](./type_defs.md#idnamespaceidmappingworkflowpropertiestypedef) [:material-code-braces: IdNamespaceIdMappingWorkflowPropertiesOutputTypeDef](./type_defs.md#idnamespaceidmappingworkflowpropertiesoutputtypedef) 
3. See [:material-code-braces: IdNamespaceInputSourceTypeDef](./type_defs.md#idnamespaceinputsourcetypedef) 
