# Type definitions

> [Index](../README.md) > [EntityResolution](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [EntityResolution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#entityresolution)
    type annotations stubs module [types-aiobotocore-entityresolution](https://pypi.org/project/types-aiobotocore-entityresolution/).

## RuleUnionTypeDef

```python
# RuleUnionTypeDef Union usage example

from types_aiobotocore_entityresolution.type_defs import RuleUnionTypeDef


def get_value() -> RuleUnionTypeDef:
    return ...


# RuleUnionTypeDef definition

RuleUnionTypeDef = Union[
    RuleTypeDef,  # (1)
    RuleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
2. See [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 

## NamespaceProviderPropertiesUnionTypeDef

```python
# NamespaceProviderPropertiesUnionTypeDef Union usage example

from types_aiobotocore_entityresolution.type_defs import NamespaceProviderPropertiesUnionTypeDef


def get_value() -> NamespaceProviderPropertiesUnionTypeDef:
    return ...


# NamespaceProviderPropertiesUnionTypeDef definition

NamespaceProviderPropertiesUnionTypeDef = Union[
    NamespaceProviderPropertiesTypeDef,  # (1)
    NamespaceProviderPropertiesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: NamespaceProviderPropertiesTypeDef](./type_defs.md#namespaceproviderpropertiestypedef) 
2. See [:material-code-braces: NamespaceProviderPropertiesOutputTypeDef](./type_defs.md#namespaceproviderpropertiesoutputtypedef) 

## OutputSourceUnionTypeDef

```python
# OutputSourceUnionTypeDef Union usage example

from types_aiobotocore_entityresolution.type_defs import OutputSourceUnionTypeDef


def get_value() -> OutputSourceUnionTypeDef:
    return ...


# OutputSourceUnionTypeDef definition

OutputSourceUnionTypeDef = Union[
    OutputSourceTypeDef,  # (1)
    OutputSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: OutputSourceTypeDef](./type_defs.md#outputsourcetypedef) 
2. See [:material-code-braces: OutputSourceOutputTypeDef](./type_defs.md#outputsourceoutputtypedef) 

## NamespaceRuleBasedPropertiesUnionTypeDef

```python
# NamespaceRuleBasedPropertiesUnionTypeDef Union usage example

from types_aiobotocore_entityresolution.type_defs import NamespaceRuleBasedPropertiesUnionTypeDef


def get_value() -> NamespaceRuleBasedPropertiesUnionTypeDef:
    return ...


# NamespaceRuleBasedPropertiesUnionTypeDef definition

NamespaceRuleBasedPropertiesUnionTypeDef = Union[
    NamespaceRuleBasedPropertiesTypeDef,  # (1)
    NamespaceRuleBasedPropertiesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: NamespaceRuleBasedPropertiesTypeDef](./type_defs.md#namespacerulebasedpropertiestypedef) 
2. See [:material-code-braces: NamespaceRuleBasedPropertiesOutputTypeDef](./type_defs.md#namespacerulebasedpropertiesoutputtypedef) 

## IdMappingTechniquesUnionTypeDef

```python
# IdMappingTechniquesUnionTypeDef Union usage example

from types_aiobotocore_entityresolution.type_defs import IdMappingTechniquesUnionTypeDef


def get_value() -> IdMappingTechniquesUnionTypeDef:
    return ...


# IdMappingTechniquesUnionTypeDef definition

IdMappingTechniquesUnionTypeDef = Union[
    IdMappingTechniquesTypeDef,  # (1)
    IdMappingTechniquesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: IdMappingTechniquesTypeDef](./type_defs.md#idmappingtechniquestypedef) 
2. See [:material-code-braces: IdMappingTechniquesOutputTypeDef](./type_defs.md#idmappingtechniquesoutputtypedef) 

## ResolutionTechniquesUnionTypeDef

```python
# ResolutionTechniquesUnionTypeDef Union usage example

from types_aiobotocore_entityresolution.type_defs import ResolutionTechniquesUnionTypeDef


def get_value() -> ResolutionTechniquesUnionTypeDef:
    return ...


# ResolutionTechniquesUnionTypeDef definition

ResolutionTechniquesUnionTypeDef = Union[
    ResolutionTechniquesTypeDef,  # (1)
    ResolutionTechniquesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ResolutionTechniquesTypeDef](./type_defs.md#resolutiontechniquestypedef) 
2. See [:material-code-braces: ResolutionTechniquesOutputTypeDef](./type_defs.md#resolutiontechniquesoutputtypedef) 

## IdNamespaceIdMappingWorkflowPropertiesUnionTypeDef

```python
# IdNamespaceIdMappingWorkflowPropertiesUnionTypeDef Union usage example

from types_aiobotocore_entityresolution.type_defs import IdNamespaceIdMappingWorkflowPropertiesUnionTypeDef


def get_value() -> IdNamespaceIdMappingWorkflowPropertiesUnionTypeDef:
    return ...


# IdNamespaceIdMappingWorkflowPropertiesUnionTypeDef definition

IdNamespaceIdMappingWorkflowPropertiesUnionTypeDef = Union[
    IdNamespaceIdMappingWorkflowPropertiesTypeDef,  # (1)
    IdNamespaceIdMappingWorkflowPropertiesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: IdNamespaceIdMappingWorkflowPropertiesTypeDef](./type_defs.md#idnamespaceidmappingworkflowpropertiestypedef) 
2. See [:material-code-braces: IdNamespaceIdMappingWorkflowPropertiesOutputTypeDef](./type_defs.md#idnamespaceidmappingworkflowpropertiesoutputtypedef) 



## AddPolicyStatementInputTypeDef

```python
# AddPolicyStatementInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import AddPolicyStatementInputTypeDef


def get_value() -> AddPolicyStatementInputTypeDef:
    return {
        "action": ...,
    }


# AddPolicyStatementInputTypeDef definition

class AddPolicyStatementInputTypeDef(TypedDict):
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
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## BatchDeleteUniqueIdInputTypeDef

```python
# BatchDeleteUniqueIdInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import BatchDeleteUniqueIdInputTypeDef


def get_value() -> BatchDeleteUniqueIdInputTypeDef:
    return {
        "uniqueIds": ...,
    }


# BatchDeleteUniqueIdInputTypeDef definition

class BatchDeleteUniqueIdInputTypeDef(TypedDict):
    uniqueIds: Sequence[str],
    workflowName: str,
    inputSource: NotRequired[str],
```

## DeleteUniqueIdErrorTypeDef

```python
# DeleteUniqueIdErrorTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import DeleteUniqueIdErrorTypeDef


def get_value() -> DeleteUniqueIdErrorTypeDef:
    return {
        "errorType": ...,
    }


# DeleteUniqueIdErrorTypeDef definition

class DeleteUniqueIdErrorTypeDef(TypedDict):
    errorType: DeleteUniqueIdErrorTypeType,  # (1)
    uniqueId: str,
```

1. See [:material-code-brackets: DeleteUniqueIdErrorTypeType](./literals.md#deleteuniqueiderrortypetype) 
## DeletedUniqueIdTypeDef

```python
# DeletedUniqueIdTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import DeletedUniqueIdTypeDef


def get_value() -> DeletedUniqueIdTypeDef:
    return {
        "uniqueId": ...,
    }


# DeletedUniqueIdTypeDef definition

class DeletedUniqueIdTypeDef(TypedDict):
    uniqueId: str,
```

## IdMappingWorkflowInputSourceTypeDef

```python
# IdMappingWorkflowInputSourceTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import IdMappingWorkflowInputSourceTypeDef


def get_value() -> IdMappingWorkflowInputSourceTypeDef:
    return {
        "inputSourceARN": ...,
    }


# IdMappingWorkflowInputSourceTypeDef definition

class IdMappingWorkflowInputSourceTypeDef(TypedDict):
    inputSourceARN: str,
    schemaName: NotRequired[str],
    type: NotRequired[IdNamespaceTypeType],  # (1)
```

1. See [:material-code-brackets: IdNamespaceTypeType](./literals.md#idnamespacetypetype) 
## IdMappingWorkflowOutputSourceTypeDef

```python
# IdMappingWorkflowOutputSourceTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import IdMappingWorkflowOutputSourceTypeDef


def get_value() -> IdMappingWorkflowOutputSourceTypeDef:
    return {
        "KMSArn": ...,
    }


# IdMappingWorkflowOutputSourceTypeDef definition

class IdMappingWorkflowOutputSourceTypeDef(TypedDict):
    outputS3Path: str,
    KMSArn: NotRequired[str],
```

## IdNamespaceInputSourceTypeDef

```python
# IdNamespaceInputSourceTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import IdNamespaceInputSourceTypeDef


def get_value() -> IdNamespaceInputSourceTypeDef:
    return {
        "inputSourceARN": ...,
    }


# IdNamespaceInputSourceTypeDef definition

class IdNamespaceInputSourceTypeDef(TypedDict):
    inputSourceARN: str,
    schemaName: NotRequired[str],
```

## IncrementalRunConfigTypeDef

```python
# IncrementalRunConfigTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import IncrementalRunConfigTypeDef


def get_value() -> IncrementalRunConfigTypeDef:
    return {
        "incrementalRunType": ...,
    }


# IncrementalRunConfigTypeDef definition

class IncrementalRunConfigTypeDef(TypedDict):
    incrementalRunType: NotRequired[IncrementalRunTypeType],  # (1)
```

1. See [:material-code-brackets: IncrementalRunTypeType](./literals.md#incrementalruntypetype) 
## InputSourceTypeDef

```python
# InputSourceTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import InputSourceTypeDef


def get_value() -> InputSourceTypeDef:
    return {
        "applyNormalization": ...,
    }


# InputSourceTypeDef definition

class InputSourceTypeDef(TypedDict):
    inputSourceARN: str,
    schemaName: str,
    applyNormalization: NotRequired[bool],
```

## SchemaInputAttributeTypeDef

```python
# SchemaInputAttributeTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import SchemaInputAttributeTypeDef


def get_value() -> SchemaInputAttributeTypeDef:
    return {
        "fieldName": ...,
    }


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
## DeleteIdMappingWorkflowInputTypeDef

```python
# DeleteIdMappingWorkflowInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import DeleteIdMappingWorkflowInputTypeDef


def get_value() -> DeleteIdMappingWorkflowInputTypeDef:
    return {
        "workflowName": ...,
    }


# DeleteIdMappingWorkflowInputTypeDef definition

class DeleteIdMappingWorkflowInputTypeDef(TypedDict):
    workflowName: str,
```

## DeleteIdNamespaceInputTypeDef

```python
# DeleteIdNamespaceInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import DeleteIdNamespaceInputTypeDef


def get_value() -> DeleteIdNamespaceInputTypeDef:
    return {
        "idNamespaceName": ...,
    }


# DeleteIdNamespaceInputTypeDef definition

class DeleteIdNamespaceInputTypeDef(TypedDict):
    idNamespaceName: str,
```

## DeleteMatchingWorkflowInputTypeDef

```python
# DeleteMatchingWorkflowInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import DeleteMatchingWorkflowInputTypeDef


def get_value() -> DeleteMatchingWorkflowInputTypeDef:
    return {
        "workflowName": ...,
    }


# DeleteMatchingWorkflowInputTypeDef definition

class DeleteMatchingWorkflowInputTypeDef(TypedDict):
    workflowName: str,
```

## DeletePolicyStatementInputTypeDef

```python
# DeletePolicyStatementInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import DeletePolicyStatementInputTypeDef


def get_value() -> DeletePolicyStatementInputTypeDef:
    return {
        "arn": ...,
    }


# DeletePolicyStatementInputTypeDef definition

class DeletePolicyStatementInputTypeDef(TypedDict):
    arn: str,
    statementId: str,
```

## DeleteSchemaMappingInputTypeDef

```python
# DeleteSchemaMappingInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import DeleteSchemaMappingInputTypeDef


def get_value() -> DeleteSchemaMappingInputTypeDef:
    return {
        "schemaName": ...,
    }


# DeleteSchemaMappingInputTypeDef definition

class DeleteSchemaMappingInputTypeDef(TypedDict):
    schemaName: str,
```

## ErrorDetailsTypeDef

```python
# ErrorDetailsTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ErrorDetailsTypeDef


def get_value() -> ErrorDetailsTypeDef:
    return {
        "errorMessage": ...,
    }


# ErrorDetailsTypeDef definition

class ErrorDetailsTypeDef(TypedDict):
    errorMessage: NotRequired[str],
```

## GetIdMappingJobInputTypeDef

```python
# GetIdMappingJobInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import GetIdMappingJobInputTypeDef


def get_value() -> GetIdMappingJobInputTypeDef:
    return {
        "jobId": ...,
    }


# GetIdMappingJobInputTypeDef definition

class GetIdMappingJobInputTypeDef(TypedDict):
    jobId: str,
    workflowName: str,
```

## IdMappingJobMetricsTypeDef

```python
# IdMappingJobMetricsTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import IdMappingJobMetricsTypeDef


def get_value() -> IdMappingJobMetricsTypeDef:
    return {
        "inputRecords": ...,
    }


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
# IdMappingJobOutputSourceTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import IdMappingJobOutputSourceTypeDef


def get_value() -> IdMappingJobOutputSourceTypeDef:
    return {
        "KMSArn": ...,
    }


# IdMappingJobOutputSourceTypeDef definition

class IdMappingJobOutputSourceTypeDef(TypedDict):
    outputS3Path: str,
    roleArn: str,
    KMSArn: NotRequired[str],
```

## GetIdMappingWorkflowInputTypeDef

```python
# GetIdMappingWorkflowInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import GetIdMappingWorkflowInputTypeDef


def get_value() -> GetIdMappingWorkflowInputTypeDef:
    return {
        "workflowName": ...,
    }


# GetIdMappingWorkflowInputTypeDef definition

class GetIdMappingWorkflowInputTypeDef(TypedDict):
    workflowName: str,
```

## GetIdNamespaceInputTypeDef

```python
# GetIdNamespaceInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import GetIdNamespaceInputTypeDef


def get_value() -> GetIdNamespaceInputTypeDef:
    return {
        "idNamespaceName": ...,
    }


# GetIdNamespaceInputTypeDef definition

class GetIdNamespaceInputTypeDef(TypedDict):
    idNamespaceName: str,
```

## GetMatchIdInputTypeDef

```python
# GetMatchIdInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import GetMatchIdInputTypeDef


def get_value() -> GetMatchIdInputTypeDef:
    return {
        "record": ...,
    }


# GetMatchIdInputTypeDef definition

class GetMatchIdInputTypeDef(TypedDict):
    record: Mapping[str, str],
    workflowName: str,
    applyNormalization: NotRequired[bool],
```

## GetMatchingJobInputTypeDef

```python
# GetMatchingJobInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import GetMatchingJobInputTypeDef


def get_value() -> GetMatchingJobInputTypeDef:
    return {
        "jobId": ...,
    }


# GetMatchingJobInputTypeDef definition

class GetMatchingJobInputTypeDef(TypedDict):
    jobId: str,
    workflowName: str,
```

## JobMetricsTypeDef

```python
# JobMetricsTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import JobMetricsTypeDef


def get_value() -> JobMetricsTypeDef:
    return {
        "inputRecords": ...,
    }


# JobMetricsTypeDef definition

class JobMetricsTypeDef(TypedDict):
    inputRecords: NotRequired[int],
    matchIDs: NotRequired[int],
    recordsNotProcessed: NotRequired[int],
    totalRecordsProcessed: NotRequired[int],
```

## JobOutputSourceTypeDef

```python
# JobOutputSourceTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import JobOutputSourceTypeDef


def get_value() -> JobOutputSourceTypeDef:
    return {
        "KMSArn": ...,
    }


# JobOutputSourceTypeDef definition

class JobOutputSourceTypeDef(TypedDict):
    outputS3Path: str,
    roleArn: str,
    KMSArn: NotRequired[str],
```

## GetMatchingWorkflowInputTypeDef

```python
# GetMatchingWorkflowInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import GetMatchingWorkflowInputTypeDef


def get_value() -> GetMatchingWorkflowInputTypeDef:
    return {
        "workflowName": ...,
    }


# GetMatchingWorkflowInputTypeDef definition

class GetMatchingWorkflowInputTypeDef(TypedDict):
    workflowName: str,
```

## GetPolicyInputTypeDef

```python
# GetPolicyInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import GetPolicyInputTypeDef


def get_value() -> GetPolicyInputTypeDef:
    return {
        "arn": ...,
    }


# GetPolicyInputTypeDef definition

class GetPolicyInputTypeDef(TypedDict):
    arn: str,
```

## GetProviderServiceInputTypeDef

```python
# GetProviderServiceInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import GetProviderServiceInputTypeDef


def get_value() -> GetProviderServiceInputTypeDef:
    return {
        "providerName": ...,
    }


# GetProviderServiceInputTypeDef definition

class GetProviderServiceInputTypeDef(TypedDict):
    providerName: str,
    providerServiceName: str,
```

## ProviderIdNameSpaceConfigurationTypeDef

```python
# ProviderIdNameSpaceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ProviderIdNameSpaceConfigurationTypeDef


def get_value() -> ProviderIdNameSpaceConfigurationTypeDef:
    return {
        "description": ...,
    }


# ProviderIdNameSpaceConfigurationTypeDef definition

class ProviderIdNameSpaceConfigurationTypeDef(TypedDict):
    description: NotRequired[str],
    providerSourceConfigurationDefinition: NotRequired[Dict[str, Any]],
    providerTargetConfigurationDefinition: NotRequired[Dict[str, Any]],
```

## ProviderIntermediateDataAccessConfigurationTypeDef

```python
# ProviderIntermediateDataAccessConfigurationTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ProviderIntermediateDataAccessConfigurationTypeDef


def get_value() -> ProviderIntermediateDataAccessConfigurationTypeDef:
    return {
        "awsAccountIds": ...,
    }


# ProviderIntermediateDataAccessConfigurationTypeDef definition

class ProviderIntermediateDataAccessConfigurationTypeDef(TypedDict):
    awsAccountIds: NotRequired[List[str]],
    requiredBucketActions: NotRequired[List[str]],
```

## GetSchemaMappingInputTypeDef

```python
# GetSchemaMappingInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import GetSchemaMappingInputTypeDef


def get_value() -> GetSchemaMappingInputTypeDef:
    return {
        "schemaName": ...,
    }


# GetSchemaMappingInputTypeDef definition

class GetSchemaMappingInputTypeDef(TypedDict):
    schemaName: str,
```

## RuleOutputTypeDef

```python
# RuleOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import RuleOutputTypeDef


def get_value() -> RuleOutputTypeDef:
    return {
        "matchingKeys": ...,
    }


# RuleOutputTypeDef definition

class RuleOutputTypeDef(TypedDict):
    matchingKeys: List[str],
    ruleName: str,
```

## RuleTypeDef

```python
# RuleTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import RuleTypeDef


def get_value() -> RuleTypeDef:
    return {
        "matchingKeys": ...,
    }


# RuleTypeDef definition

class RuleTypeDef(TypedDict):
    matchingKeys: Sequence[str],
    ruleName: str,
```

## IdMappingWorkflowSummaryTypeDef

```python
# IdMappingWorkflowSummaryTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import IdMappingWorkflowSummaryTypeDef


def get_value() -> IdMappingWorkflowSummaryTypeDef:
    return {
        "createdAt": ...,
    }


# IdMappingWorkflowSummaryTypeDef definition

class IdMappingWorkflowSummaryTypeDef(TypedDict):
    createdAt: datetime,
    updatedAt: datetime,
    workflowArn: str,
    workflowName: str,
```

## IdNamespaceIdMappingWorkflowMetadataTypeDef

```python
# IdNamespaceIdMappingWorkflowMetadataTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import IdNamespaceIdMappingWorkflowMetadataTypeDef


def get_value() -> IdNamespaceIdMappingWorkflowMetadataTypeDef:
    return {
        "idMappingType": ...,
    }


# IdNamespaceIdMappingWorkflowMetadataTypeDef definition

class IdNamespaceIdMappingWorkflowMetadataTypeDef(TypedDict):
    idMappingType: IdMappingTypeType,  # (1)
```

1. See [:material-code-brackets: IdMappingTypeType](./literals.md#idmappingtypetype) 
## NamespaceProviderPropertiesOutputTypeDef

```python
# NamespaceProviderPropertiesOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import NamespaceProviderPropertiesOutputTypeDef


def get_value() -> NamespaceProviderPropertiesOutputTypeDef:
    return {
        "providerConfiguration": ...,
    }


# NamespaceProviderPropertiesOutputTypeDef definition

class NamespaceProviderPropertiesOutputTypeDef(TypedDict):
    providerServiceArn: str,
    providerConfiguration: NotRequired[Dict[str, Any]],
```

## IntermediateSourceConfigurationTypeDef

```python
# IntermediateSourceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import IntermediateSourceConfigurationTypeDef


def get_value() -> IntermediateSourceConfigurationTypeDef:
    return {
        "intermediateS3Path": ...,
    }


# IntermediateSourceConfigurationTypeDef definition

class IntermediateSourceConfigurationTypeDef(TypedDict):
    intermediateS3Path: str,
```

## JobSummaryTypeDef

```python
# JobSummaryTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import JobSummaryTypeDef


def get_value() -> JobSummaryTypeDef:
    return {
        "endTime": ...,
    }


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
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListIdMappingJobsInputTypeDef

```python
# ListIdMappingJobsInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ListIdMappingJobsInputTypeDef


def get_value() -> ListIdMappingJobsInputTypeDef:
    return {
        "workflowName": ...,
    }


# ListIdMappingJobsInputTypeDef definition

class ListIdMappingJobsInputTypeDef(TypedDict):
    workflowName: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListIdMappingWorkflowsInputTypeDef

```python
# ListIdMappingWorkflowsInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ListIdMappingWorkflowsInputTypeDef


def get_value() -> ListIdMappingWorkflowsInputTypeDef:
    return {
        "maxResults": ...,
    }


# ListIdMappingWorkflowsInputTypeDef definition

class ListIdMappingWorkflowsInputTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListIdNamespacesInputTypeDef

```python
# ListIdNamespacesInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ListIdNamespacesInputTypeDef


def get_value() -> ListIdNamespacesInputTypeDef:
    return {
        "maxResults": ...,
    }


# ListIdNamespacesInputTypeDef definition

class ListIdNamespacesInputTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListMatchingJobsInputTypeDef

```python
# ListMatchingJobsInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ListMatchingJobsInputTypeDef


def get_value() -> ListMatchingJobsInputTypeDef:
    return {
        "workflowName": ...,
    }


# ListMatchingJobsInputTypeDef definition

class ListMatchingJobsInputTypeDef(TypedDict):
    workflowName: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListMatchingWorkflowsInputTypeDef

```python
# ListMatchingWorkflowsInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ListMatchingWorkflowsInputTypeDef


def get_value() -> ListMatchingWorkflowsInputTypeDef:
    return {
        "maxResults": ...,
    }


# ListMatchingWorkflowsInputTypeDef definition

class ListMatchingWorkflowsInputTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## MatchingWorkflowSummaryTypeDef

```python
# MatchingWorkflowSummaryTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import MatchingWorkflowSummaryTypeDef


def get_value() -> MatchingWorkflowSummaryTypeDef:
    return {
        "createdAt": ...,
    }


# MatchingWorkflowSummaryTypeDef definition

class MatchingWorkflowSummaryTypeDef(TypedDict):
    createdAt: datetime,
    resolutionType: ResolutionTypeType,  # (1)
    updatedAt: datetime,
    workflowArn: str,
    workflowName: str,
```

1. See [:material-code-brackets: ResolutionTypeType](./literals.md#resolutiontypetype) 
## ListProviderServicesInputTypeDef

```python
# ListProviderServicesInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ListProviderServicesInputTypeDef


def get_value() -> ListProviderServicesInputTypeDef:
    return {
        "maxResults": ...,
    }


# ListProviderServicesInputTypeDef definition

class ListProviderServicesInputTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    providerName: NotRequired[str],
```

## ProviderServiceSummaryTypeDef

```python
# ProviderServiceSummaryTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ProviderServiceSummaryTypeDef


def get_value() -> ProviderServiceSummaryTypeDef:
    return {
        "providerName": ...,
    }


# ProviderServiceSummaryTypeDef definition

class ProviderServiceSummaryTypeDef(TypedDict):
    providerName: str,
    providerServiceArn: str,
    providerServiceDisplayName: str,
    providerServiceName: str,
    providerServiceType: ServiceTypeType,  # (1)
```

1. See [:material-code-brackets: ServiceTypeType](./literals.md#servicetypetype) 
## ListSchemaMappingsInputTypeDef

```python
# ListSchemaMappingsInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ListSchemaMappingsInputTypeDef


def get_value() -> ListSchemaMappingsInputTypeDef:
    return {
        "maxResults": ...,
    }


# ListSchemaMappingsInputTypeDef definition

class ListSchemaMappingsInputTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## SchemaMappingSummaryTypeDef

```python
# SchemaMappingSummaryTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import SchemaMappingSummaryTypeDef


def get_value() -> SchemaMappingSummaryTypeDef:
    return {
        "createdAt": ...,
    }


# SchemaMappingSummaryTypeDef definition

class SchemaMappingSummaryTypeDef(TypedDict):
    createdAt: datetime,
    hasWorkflows: bool,
    schemaArn: str,
    schemaName: str,
    updatedAt: datetime,
```

## ListTagsForResourceInputTypeDef

```python
# ListTagsForResourceInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ListTagsForResourceInputTypeDef


def get_value() -> ListTagsForResourceInputTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceInputTypeDef definition

class ListTagsForResourceInputTypeDef(TypedDict):
    resourceArn: str,
```

## NamespaceProviderPropertiesTypeDef

```python
# NamespaceProviderPropertiesTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import NamespaceProviderPropertiesTypeDef


def get_value() -> NamespaceProviderPropertiesTypeDef:
    return {
        "providerConfiguration": ...,
    }


# NamespaceProviderPropertiesTypeDef definition

class NamespaceProviderPropertiesTypeDef(TypedDict):
    providerServiceArn: str,
    providerConfiguration: NotRequired[Mapping[str, Any]],
```

## OutputAttributeTypeDef

```python
# OutputAttributeTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import OutputAttributeTypeDef


def get_value() -> OutputAttributeTypeDef:
    return {
        "hashed": ...,
    }


# OutputAttributeTypeDef definition

class OutputAttributeTypeDef(TypedDict):
    name: str,
    hashed: NotRequired[bool],
```

## ProviderSchemaAttributeTypeDef

```python
# ProviderSchemaAttributeTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ProviderSchemaAttributeTypeDef


def get_value() -> ProviderSchemaAttributeTypeDef:
    return {
        "fieldName": ...,
    }


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
# ProviderMarketplaceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ProviderMarketplaceConfigurationTypeDef


def get_value() -> ProviderMarketplaceConfigurationTypeDef:
    return {
        "assetId": ...,
    }


# ProviderMarketplaceConfigurationTypeDef definition

class ProviderMarketplaceConfigurationTypeDef(TypedDict):
    assetId: str,
    dataSetId: str,
    listingId: str,
    revisionId: str,
```

## PutPolicyInputTypeDef

```python
# PutPolicyInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import PutPolicyInputTypeDef


def get_value() -> PutPolicyInputTypeDef:
    return {
        "arn": ...,
    }


# PutPolicyInputTypeDef definition

class PutPolicyInputTypeDef(TypedDict):
    arn: str,
    policy: str,
    token: NotRequired[str],
```

## StartMatchingJobInputTypeDef

```python
# StartMatchingJobInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import StartMatchingJobInputTypeDef


def get_value() -> StartMatchingJobInputTypeDef:
    return {
        "workflowName": ...,
    }


# StartMatchingJobInputTypeDef definition

class StartMatchingJobInputTypeDef(TypedDict):
    workflowName: str,
```

## TagResourceInputTypeDef

```python
# TagResourceInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import TagResourceInputTypeDef


def get_value() -> TagResourceInputTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceInputTypeDef definition

class TagResourceInputTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceInputTypeDef

```python
# UntagResourceInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import UntagResourceInputTypeDef


def get_value() -> UntagResourceInputTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceInputTypeDef definition

class UntagResourceInputTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## AddPolicyStatementOutputTypeDef

```python
# AddPolicyStatementOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import AddPolicyStatementOutputTypeDef


def get_value() -> AddPolicyStatementOutputTypeDef:
    return {
        "arn": ...,
    }


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
# DeleteIdMappingWorkflowOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import DeleteIdMappingWorkflowOutputTypeDef


def get_value() -> DeleteIdMappingWorkflowOutputTypeDef:
    return {
        "message": ...,
    }


# DeleteIdMappingWorkflowOutputTypeDef definition

class DeleteIdMappingWorkflowOutputTypeDef(TypedDict):
    message: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteIdNamespaceOutputTypeDef

```python
# DeleteIdNamespaceOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import DeleteIdNamespaceOutputTypeDef


def get_value() -> DeleteIdNamespaceOutputTypeDef:
    return {
        "message": ...,
    }


# DeleteIdNamespaceOutputTypeDef definition

class DeleteIdNamespaceOutputTypeDef(TypedDict):
    message: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteMatchingWorkflowOutputTypeDef

```python
# DeleteMatchingWorkflowOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import DeleteMatchingWorkflowOutputTypeDef


def get_value() -> DeleteMatchingWorkflowOutputTypeDef:
    return {
        "message": ...,
    }


# DeleteMatchingWorkflowOutputTypeDef definition

class DeleteMatchingWorkflowOutputTypeDef(TypedDict):
    message: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeletePolicyStatementOutputTypeDef

```python
# DeletePolicyStatementOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import DeletePolicyStatementOutputTypeDef


def get_value() -> DeletePolicyStatementOutputTypeDef:
    return {
        "arn": ...,
    }


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
# DeleteSchemaMappingOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import DeleteSchemaMappingOutputTypeDef


def get_value() -> DeleteSchemaMappingOutputTypeDef:
    return {
        "message": ...,
    }


# DeleteSchemaMappingOutputTypeDef definition

class DeleteSchemaMappingOutputTypeDef(TypedDict):
    message: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMatchIdOutputTypeDef

```python
# GetMatchIdOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import GetMatchIdOutputTypeDef


def get_value() -> GetMatchIdOutputTypeDef:
    return {
        "matchId": ...,
    }


# GetMatchIdOutputTypeDef definition

class GetMatchIdOutputTypeDef(TypedDict):
    matchId: str,
    matchRule: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPolicyOutputTypeDef

```python
# GetPolicyOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import GetPolicyOutputTypeDef


def get_value() -> GetPolicyOutputTypeDef:
    return {
        "arn": ...,
    }


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
# ListTagsForResourceOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ListTagsForResourceOutputTypeDef


def get_value() -> ListTagsForResourceOutputTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutPolicyOutputTypeDef

```python
# PutPolicyOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import PutPolicyOutputTypeDef


def get_value() -> PutPolicyOutputTypeDef:
    return {
        "arn": ...,
    }


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
# StartMatchingJobOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import StartMatchingJobOutputTypeDef


def get_value() -> StartMatchingJobOutputTypeDef:
    return {
        "jobId": ...,
    }


# StartMatchingJobOutputTypeDef definition

class StartMatchingJobOutputTypeDef(TypedDict):
    jobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDeleteUniqueIdOutputTypeDef

```python
# BatchDeleteUniqueIdOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import BatchDeleteUniqueIdOutputTypeDef


def get_value() -> BatchDeleteUniqueIdOutputTypeDef:
    return {
        "deleted": ...,
    }


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
## CreateSchemaMappingInputTypeDef

```python
# CreateSchemaMappingInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import CreateSchemaMappingInputTypeDef


def get_value() -> CreateSchemaMappingInputTypeDef:
    return {
        "mappedInputFields": ...,
    }


# CreateSchemaMappingInputTypeDef definition

class CreateSchemaMappingInputTypeDef(TypedDict):
    mappedInputFields: Sequence[SchemaInputAttributeTypeDef],  # (1)
    schemaName: str,
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: SchemaInputAttributeTypeDef](./type_defs.md#schemainputattributetypedef) 
## CreateSchemaMappingOutputTypeDef

```python
# CreateSchemaMappingOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import CreateSchemaMappingOutputTypeDef


def get_value() -> CreateSchemaMappingOutputTypeDef:
    return {
        "description": ...,
    }


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
# GetSchemaMappingOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import GetSchemaMappingOutputTypeDef


def get_value() -> GetSchemaMappingOutputTypeDef:
    return {
        "createdAt": ...,
    }


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
## UpdateSchemaMappingInputTypeDef

```python
# UpdateSchemaMappingInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import UpdateSchemaMappingInputTypeDef


def get_value() -> UpdateSchemaMappingInputTypeDef:
    return {
        "mappedInputFields": ...,
    }


# UpdateSchemaMappingInputTypeDef definition

class UpdateSchemaMappingInputTypeDef(TypedDict):
    mappedInputFields: Sequence[SchemaInputAttributeTypeDef],  # (1)
    schemaName: str,
    description: NotRequired[str],
```

1. See [:material-code-braces: SchemaInputAttributeTypeDef](./type_defs.md#schemainputattributetypedef) 
## UpdateSchemaMappingOutputTypeDef

```python
# UpdateSchemaMappingOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import UpdateSchemaMappingOutputTypeDef


def get_value() -> UpdateSchemaMappingOutputTypeDef:
    return {
        "description": ...,
    }


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
# GetIdMappingJobOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import GetIdMappingJobOutputTypeDef


def get_value() -> GetIdMappingJobOutputTypeDef:
    return {
        "endTime": ...,
    }


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
## StartIdMappingJobInputTypeDef

```python
# StartIdMappingJobInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import StartIdMappingJobInputTypeDef


def get_value() -> StartIdMappingJobInputTypeDef:
    return {
        "workflowName": ...,
    }


# StartIdMappingJobInputTypeDef definition

class StartIdMappingJobInputTypeDef(TypedDict):
    workflowName: str,
    outputSourceConfig: NotRequired[Sequence[IdMappingJobOutputSourceTypeDef]],  # (1)
```

1. See [:material-code-braces: IdMappingJobOutputSourceTypeDef](./type_defs.md#idmappingjoboutputsourcetypedef) 
## StartIdMappingJobOutputTypeDef

```python
# StartIdMappingJobOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import StartIdMappingJobOutputTypeDef


def get_value() -> StartIdMappingJobOutputTypeDef:
    return {
        "jobId": ...,
    }


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
# GetMatchingJobOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import GetMatchingJobOutputTypeDef


def get_value() -> GetMatchingJobOutputTypeDef:
    return {
        "endTime": ...,
    }


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
# IdMappingRuleBasedPropertiesOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import IdMappingRuleBasedPropertiesOutputTypeDef


def get_value() -> IdMappingRuleBasedPropertiesOutputTypeDef:
    return {
        "attributeMatchingModel": ...,
    }


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
# NamespaceRuleBasedPropertiesOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import NamespaceRuleBasedPropertiesOutputTypeDef


def get_value() -> NamespaceRuleBasedPropertiesOutputTypeDef:
    return {
        "attributeMatchingModel": ...,
    }


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
# RuleBasedPropertiesOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import RuleBasedPropertiesOutputTypeDef


def get_value() -> RuleBasedPropertiesOutputTypeDef:
    return {
        "attributeMatchingModel": ...,
    }


# RuleBasedPropertiesOutputTypeDef definition

class RuleBasedPropertiesOutputTypeDef(TypedDict):
    attributeMatchingModel: AttributeMatchingModelType,  # (1)
    rules: List[RuleOutputTypeDef],  # (3)
    matchPurpose: NotRequired[MatchPurposeType],  # (2)
```

1. See [:material-code-brackets: AttributeMatchingModelType](./literals.md#attributematchingmodeltype) 
2. See [:material-code-brackets: MatchPurposeType](./literals.md#matchpurposetype) 
3. See [:material-code-braces: RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef) 
## IdMappingRuleBasedPropertiesTypeDef

```python
# IdMappingRuleBasedPropertiesTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import IdMappingRuleBasedPropertiesTypeDef


def get_value() -> IdMappingRuleBasedPropertiesTypeDef:
    return {
        "attributeMatchingModel": ...,
    }


# IdMappingRuleBasedPropertiesTypeDef definition

class IdMappingRuleBasedPropertiesTypeDef(TypedDict):
    attributeMatchingModel: AttributeMatchingModelType,  # (1)
    recordMatchingModel: RecordMatchingModelType,  # (2)
    ruleDefinitionType: IdMappingWorkflowRuleDefinitionTypeType,  # (3)
    rules: NotRequired[Sequence[RuleTypeDef]],  # (4)
```

1. See [:material-code-brackets: AttributeMatchingModelType](./literals.md#attributematchingmodeltype) 
2. See [:material-code-brackets: RecordMatchingModelType](./literals.md#recordmatchingmodeltype) 
3. See [:material-code-brackets: IdMappingWorkflowRuleDefinitionTypeType](./literals.md#idmappingworkflowruledefinitiontypetype) 
4. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
## RuleBasedPropertiesTypeDef

```python
# RuleBasedPropertiesTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import RuleBasedPropertiesTypeDef


def get_value() -> RuleBasedPropertiesTypeDef:
    return {
        "attributeMatchingModel": ...,
    }


# RuleBasedPropertiesTypeDef definition

class RuleBasedPropertiesTypeDef(TypedDict):
    attributeMatchingModel: AttributeMatchingModelType,  # (1)
    rules: Sequence[RuleTypeDef],  # (3)
    matchPurpose: NotRequired[MatchPurposeType],  # (2)
```

1. See [:material-code-brackets: AttributeMatchingModelType](./literals.md#attributematchingmodeltype) 
2. See [:material-code-brackets: MatchPurposeType](./literals.md#matchpurposetype) 
3. See [:material-code-braces: RuleTypeDef](./type_defs.md#ruletypedef) 
## ListIdMappingWorkflowsOutputTypeDef

```python
# ListIdMappingWorkflowsOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ListIdMappingWorkflowsOutputTypeDef


def get_value() -> ListIdMappingWorkflowsOutputTypeDef:
    return {
        "nextToken": ...,
    }


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
# IdNamespaceSummaryTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import IdNamespaceSummaryTypeDef


def get_value() -> IdNamespaceSummaryTypeDef:
    return {
        "createdAt": ...,
    }


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
# ProviderPropertiesOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ProviderPropertiesOutputTypeDef


def get_value() -> ProviderPropertiesOutputTypeDef:
    return {
        "intermediateSourceConfiguration": ...,
    }


# ProviderPropertiesOutputTypeDef definition

class ProviderPropertiesOutputTypeDef(TypedDict):
    providerServiceArn: str,
    intermediateSourceConfiguration: NotRequired[IntermediateSourceConfigurationTypeDef],  # (1)
    providerConfiguration: NotRequired[Dict[str, Any]],
```

1. See [:material-code-braces: IntermediateSourceConfigurationTypeDef](./type_defs.md#intermediatesourceconfigurationtypedef) 
## ProviderPropertiesTypeDef

```python
# ProviderPropertiesTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ProviderPropertiesTypeDef


def get_value() -> ProviderPropertiesTypeDef:
    return {
        "intermediateSourceConfiguration": ...,
    }


# ProviderPropertiesTypeDef definition

class ProviderPropertiesTypeDef(TypedDict):
    providerServiceArn: str,
    intermediateSourceConfiguration: NotRequired[IntermediateSourceConfigurationTypeDef],  # (1)
    providerConfiguration: NotRequired[Mapping[str, Any]],
```

1. See [:material-code-braces: IntermediateSourceConfigurationTypeDef](./type_defs.md#intermediatesourceconfigurationtypedef) 
## ListIdMappingJobsOutputTypeDef

```python
# ListIdMappingJobsOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ListIdMappingJobsOutputTypeDef


def get_value() -> ListIdMappingJobsOutputTypeDef:
    return {
        "jobs": ...,
    }


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
# ListMatchingJobsOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ListMatchingJobsOutputTypeDef


def get_value() -> ListMatchingJobsOutputTypeDef:
    return {
        "jobs": ...,
    }


# ListMatchingJobsOutputTypeDef definition

class ListMatchingJobsOutputTypeDef(TypedDict):
    jobs: List[JobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: JobSummaryTypeDef](./type_defs.md#jobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIdMappingJobsInputPaginateTypeDef

```python
# ListIdMappingJobsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ListIdMappingJobsInputPaginateTypeDef


def get_value() -> ListIdMappingJobsInputPaginateTypeDef:
    return {
        "workflowName": ...,
    }


# ListIdMappingJobsInputPaginateTypeDef definition

class ListIdMappingJobsInputPaginateTypeDef(TypedDict):
    workflowName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIdMappingWorkflowsInputPaginateTypeDef

```python
# ListIdMappingWorkflowsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ListIdMappingWorkflowsInputPaginateTypeDef


def get_value() -> ListIdMappingWorkflowsInputPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListIdMappingWorkflowsInputPaginateTypeDef definition

class ListIdMappingWorkflowsInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIdNamespacesInputPaginateTypeDef

```python
# ListIdNamespacesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ListIdNamespacesInputPaginateTypeDef


def get_value() -> ListIdNamespacesInputPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListIdNamespacesInputPaginateTypeDef definition

class ListIdNamespacesInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMatchingJobsInputPaginateTypeDef

```python
# ListMatchingJobsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ListMatchingJobsInputPaginateTypeDef


def get_value() -> ListMatchingJobsInputPaginateTypeDef:
    return {
        "workflowName": ...,
    }


# ListMatchingJobsInputPaginateTypeDef definition

class ListMatchingJobsInputPaginateTypeDef(TypedDict):
    workflowName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMatchingWorkflowsInputPaginateTypeDef

```python
# ListMatchingWorkflowsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ListMatchingWorkflowsInputPaginateTypeDef


def get_value() -> ListMatchingWorkflowsInputPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListMatchingWorkflowsInputPaginateTypeDef definition

class ListMatchingWorkflowsInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProviderServicesInputPaginateTypeDef

```python
# ListProviderServicesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ListProviderServicesInputPaginateTypeDef


def get_value() -> ListProviderServicesInputPaginateTypeDef:
    return {
        "providerName": ...,
    }


# ListProviderServicesInputPaginateTypeDef definition

class ListProviderServicesInputPaginateTypeDef(TypedDict):
    providerName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSchemaMappingsInputPaginateTypeDef

```python
# ListSchemaMappingsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ListSchemaMappingsInputPaginateTypeDef


def get_value() -> ListSchemaMappingsInputPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListSchemaMappingsInputPaginateTypeDef definition

class ListSchemaMappingsInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMatchingWorkflowsOutputTypeDef

```python
# ListMatchingWorkflowsOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ListMatchingWorkflowsOutputTypeDef


def get_value() -> ListMatchingWorkflowsOutputTypeDef:
    return {
        "nextToken": ...,
    }


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
# ListProviderServicesOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ListProviderServicesOutputTypeDef


def get_value() -> ListProviderServicesOutputTypeDef:
    return {
        "nextToken": ...,
    }


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
# ListSchemaMappingsOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ListSchemaMappingsOutputTypeDef


def get_value() -> ListSchemaMappingsOutputTypeDef:
    return {
        "nextToken": ...,
    }


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
# OutputSourceOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import OutputSourceOutputTypeDef


def get_value() -> OutputSourceOutputTypeDef:
    return {
        "KMSArn": ...,
    }


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
# OutputSourceTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import OutputSourceTypeDef


def get_value() -> OutputSourceTypeDef:
    return {
        "KMSArn": ...,
    }


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
# ProviderComponentSchemaTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ProviderComponentSchemaTypeDef


def get_value() -> ProviderComponentSchemaTypeDef:
    return {
        "providerSchemaAttributes": ...,
    }


# ProviderComponentSchemaTypeDef definition

class ProviderComponentSchemaTypeDef(TypedDict):
    providerSchemaAttributes: NotRequired[List[ProviderSchemaAttributeTypeDef]],  # (1)
    schemas: NotRequired[List[List[str]]],
```

1. See [:material-code-braces: ProviderSchemaAttributeTypeDef](./type_defs.md#providerschemaattributetypedef) 
## ProviderEndpointConfigurationTypeDef

```python
# ProviderEndpointConfigurationTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ProviderEndpointConfigurationTypeDef


def get_value() -> ProviderEndpointConfigurationTypeDef:
    return {
        "marketplaceConfiguration": ...,
    }


# ProviderEndpointConfigurationTypeDef definition

class ProviderEndpointConfigurationTypeDef(TypedDict):
    marketplaceConfiguration: NotRequired[ProviderMarketplaceConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ProviderMarketplaceConfigurationTypeDef](./type_defs.md#providermarketplaceconfigurationtypedef) 
## IdNamespaceIdMappingWorkflowPropertiesOutputTypeDef

```python
# IdNamespaceIdMappingWorkflowPropertiesOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import IdNamespaceIdMappingWorkflowPropertiesOutputTypeDef


def get_value() -> IdNamespaceIdMappingWorkflowPropertiesOutputTypeDef:
    return {
        "idMappingType": ...,
    }


# IdNamespaceIdMappingWorkflowPropertiesOutputTypeDef definition

class IdNamespaceIdMappingWorkflowPropertiesOutputTypeDef(TypedDict):
    idMappingType: IdMappingTypeType,  # (1)
    providerProperties: NotRequired[NamespaceProviderPropertiesOutputTypeDef],  # (2)
    ruleBasedProperties: NotRequired[NamespaceRuleBasedPropertiesOutputTypeDef],  # (3)
```

1. See [:material-code-brackets: IdMappingTypeType](./literals.md#idmappingtypetype) 
2. See [:material-code-braces: NamespaceProviderPropertiesOutputTypeDef](./type_defs.md#namespaceproviderpropertiesoutputtypedef) 
3. See [:material-code-braces: NamespaceRuleBasedPropertiesOutputTypeDef](./type_defs.md#namespacerulebasedpropertiesoutputtypedef) 
## NamespaceRuleBasedPropertiesTypeDef

```python
# NamespaceRuleBasedPropertiesTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import NamespaceRuleBasedPropertiesTypeDef


def get_value() -> NamespaceRuleBasedPropertiesTypeDef:
    return {
        "attributeMatchingModel": ...,
    }


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
## ListIdNamespacesOutputTypeDef

```python
# ListIdNamespacesOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ListIdNamespacesOutputTypeDef


def get_value() -> ListIdNamespacesOutputTypeDef:
    return {
        "idNamespaceSummaries": ...,
    }


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
# IdMappingTechniquesOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import IdMappingTechniquesOutputTypeDef


def get_value() -> IdMappingTechniquesOutputTypeDef:
    return {
        "idMappingType": ...,
    }


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
# ResolutionTechniquesOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ResolutionTechniquesOutputTypeDef


def get_value() -> ResolutionTechniquesOutputTypeDef:
    return {
        "providerProperties": ...,
    }


# ResolutionTechniquesOutputTypeDef definition

class ResolutionTechniquesOutputTypeDef(TypedDict):
    resolutionType: ResolutionTypeType,  # (2)
    providerProperties: NotRequired[ProviderPropertiesOutputTypeDef],  # (1)
    ruleBasedProperties: NotRequired[RuleBasedPropertiesOutputTypeDef],  # (3)
```

1. See [:material-code-braces: ProviderPropertiesOutputTypeDef](./type_defs.md#providerpropertiesoutputtypedef) 
2. See [:material-code-brackets: ResolutionTypeType](./literals.md#resolutiontypetype) 
3. See [:material-code-braces: RuleBasedPropertiesOutputTypeDef](./type_defs.md#rulebasedpropertiesoutputtypedef) 
## IdMappingTechniquesTypeDef

```python
# IdMappingTechniquesTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import IdMappingTechniquesTypeDef


def get_value() -> IdMappingTechniquesTypeDef:
    return {
        "idMappingType": ...,
    }


# IdMappingTechniquesTypeDef definition

class IdMappingTechniquesTypeDef(TypedDict):
    idMappingType: IdMappingTypeType,  # (1)
    providerProperties: NotRequired[ProviderPropertiesTypeDef],  # (2)
    ruleBasedProperties: NotRequired[IdMappingRuleBasedPropertiesTypeDef],  # (3)
```

1. See [:material-code-brackets: IdMappingTypeType](./literals.md#idmappingtypetype) 
2. See [:material-code-braces: ProviderPropertiesTypeDef](./type_defs.md#providerpropertiestypedef) 
3. See [:material-code-braces: IdMappingRuleBasedPropertiesTypeDef](./type_defs.md#idmappingrulebasedpropertiestypedef) 
## ResolutionTechniquesTypeDef

```python
# ResolutionTechniquesTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import ResolutionTechniquesTypeDef


def get_value() -> ResolutionTechniquesTypeDef:
    return {
        "providerProperties": ...,
    }


# ResolutionTechniquesTypeDef definition

class ResolutionTechniquesTypeDef(TypedDict):
    resolutionType: ResolutionTypeType,  # (2)
    providerProperties: NotRequired[ProviderPropertiesTypeDef],  # (1)
    ruleBasedProperties: NotRequired[RuleBasedPropertiesTypeDef],  # (3)
```

1. See [:material-code-braces: ProviderPropertiesTypeDef](./type_defs.md#providerpropertiestypedef) 
2. See [:material-code-brackets: ResolutionTypeType](./literals.md#resolutiontypetype) 
3. See [:material-code-braces: RuleBasedPropertiesTypeDef](./type_defs.md#rulebasedpropertiestypedef) 
## GetProviderServiceOutputTypeDef

```python
# GetProviderServiceOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import GetProviderServiceOutputTypeDef


def get_value() -> GetProviderServiceOutputTypeDef:
    return {
        "anonymizedOutput": ...,
    }


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
## CreateIdNamespaceOutputTypeDef

```python
# CreateIdNamespaceOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import CreateIdNamespaceOutputTypeDef


def get_value() -> CreateIdNamespaceOutputTypeDef:
    return {
        "createdAt": ...,
    }


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
# GetIdNamespaceOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import GetIdNamespaceOutputTypeDef


def get_value() -> GetIdNamespaceOutputTypeDef:
    return {
        "createdAt": ...,
    }


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
# UpdateIdNamespaceOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import UpdateIdNamespaceOutputTypeDef


def get_value() -> UpdateIdNamespaceOutputTypeDef:
    return {
        "createdAt": ...,
    }


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
# CreateIdMappingWorkflowOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import CreateIdMappingWorkflowOutputTypeDef


def get_value() -> CreateIdMappingWorkflowOutputTypeDef:
    return {
        "description": ...,
    }


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
# GetIdMappingWorkflowOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import GetIdMappingWorkflowOutputTypeDef


def get_value() -> GetIdMappingWorkflowOutputTypeDef:
    return {
        "createdAt": ...,
    }


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
# UpdateIdMappingWorkflowOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import UpdateIdMappingWorkflowOutputTypeDef


def get_value() -> UpdateIdMappingWorkflowOutputTypeDef:
    return {
        "description": ...,
    }


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
# CreateMatchingWorkflowOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import CreateMatchingWorkflowOutputTypeDef


def get_value() -> CreateMatchingWorkflowOutputTypeDef:
    return {
        "description": ...,
    }


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
# GetMatchingWorkflowOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import GetMatchingWorkflowOutputTypeDef


def get_value() -> GetMatchingWorkflowOutputTypeDef:
    return {
        "createdAt": ...,
    }


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
# UpdateMatchingWorkflowOutputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import UpdateMatchingWorkflowOutputTypeDef


def get_value() -> UpdateMatchingWorkflowOutputTypeDef:
    return {
        "description": ...,
    }


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
## IdNamespaceIdMappingWorkflowPropertiesTypeDef

```python
# IdNamespaceIdMappingWorkflowPropertiesTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import IdNamespaceIdMappingWorkflowPropertiesTypeDef


def get_value() -> IdNamespaceIdMappingWorkflowPropertiesTypeDef:
    return {
        "idMappingType": ...,
    }


# IdNamespaceIdMappingWorkflowPropertiesTypeDef definition

class IdNamespaceIdMappingWorkflowPropertiesTypeDef(TypedDict):
    idMappingType: IdMappingTypeType,  # (1)
    providerProperties: NotRequired[NamespaceProviderPropertiesUnionTypeDef],  # (2)
    ruleBasedProperties: NotRequired[NamespaceRuleBasedPropertiesUnionTypeDef],  # (3)
```

1. See [:material-code-brackets: IdMappingTypeType](./literals.md#idmappingtypetype) 
2. See [:material-code-braces: NamespaceProviderPropertiesTypeDef](./type_defs.md#namespaceproviderpropertiestypedef) [:material-code-braces: NamespaceProviderPropertiesOutputTypeDef](./type_defs.md#namespaceproviderpropertiesoutputtypedef) 
3. See [:material-code-braces: NamespaceRuleBasedPropertiesTypeDef](./type_defs.md#namespacerulebasedpropertiestypedef) [:material-code-braces: NamespaceRuleBasedPropertiesOutputTypeDef](./type_defs.md#namespacerulebasedpropertiesoutputtypedef) 
## CreateIdMappingWorkflowInputTypeDef

```python
# CreateIdMappingWorkflowInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import CreateIdMappingWorkflowInputTypeDef


def get_value() -> CreateIdMappingWorkflowInputTypeDef:
    return {
        "idMappingTechniques": ...,
    }


# CreateIdMappingWorkflowInputTypeDef definition

class CreateIdMappingWorkflowInputTypeDef(TypedDict):
    idMappingTechniques: IdMappingTechniquesUnionTypeDef,  # (1)
    inputSourceConfig: Sequence[IdMappingWorkflowInputSourceTypeDef],  # (2)
    workflowName: str,
    description: NotRequired[str],
    outputSourceConfig: NotRequired[Sequence[IdMappingWorkflowOutputSourceTypeDef]],  # (3)
    roleArn: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: IdMappingTechniquesTypeDef](./type_defs.md#idmappingtechniquestypedef) [:material-code-braces: IdMappingTechniquesOutputTypeDef](./type_defs.md#idmappingtechniquesoutputtypedef) 
2. See [:material-code-braces: IdMappingWorkflowInputSourceTypeDef](./type_defs.md#idmappingworkflowinputsourcetypedef) 
3. See [:material-code-braces: IdMappingWorkflowOutputSourceTypeDef](./type_defs.md#idmappingworkflowoutputsourcetypedef) 
## UpdateIdMappingWorkflowInputTypeDef

```python
# UpdateIdMappingWorkflowInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import UpdateIdMappingWorkflowInputTypeDef


def get_value() -> UpdateIdMappingWorkflowInputTypeDef:
    return {
        "idMappingTechniques": ...,
    }


# UpdateIdMappingWorkflowInputTypeDef definition

class UpdateIdMappingWorkflowInputTypeDef(TypedDict):
    idMappingTechniques: IdMappingTechniquesUnionTypeDef,  # (1)
    inputSourceConfig: Sequence[IdMappingWorkflowInputSourceTypeDef],  # (2)
    workflowName: str,
    description: NotRequired[str],
    outputSourceConfig: NotRequired[Sequence[IdMappingWorkflowOutputSourceTypeDef]],  # (3)
    roleArn: NotRequired[str],
```

1. See [:material-code-braces: IdMappingTechniquesTypeDef](./type_defs.md#idmappingtechniquestypedef) [:material-code-braces: IdMappingTechniquesOutputTypeDef](./type_defs.md#idmappingtechniquesoutputtypedef) 
2. See [:material-code-braces: IdMappingWorkflowInputSourceTypeDef](./type_defs.md#idmappingworkflowinputsourcetypedef) 
3. See [:material-code-braces: IdMappingWorkflowOutputSourceTypeDef](./type_defs.md#idmappingworkflowoutputsourcetypedef) 
## CreateMatchingWorkflowInputTypeDef

```python
# CreateMatchingWorkflowInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import CreateMatchingWorkflowInputTypeDef


def get_value() -> CreateMatchingWorkflowInputTypeDef:
    return {
        "inputSourceConfig": ...,
    }


# CreateMatchingWorkflowInputTypeDef definition

class CreateMatchingWorkflowInputTypeDef(TypedDict):
    inputSourceConfig: Sequence[InputSourceTypeDef],  # (1)
    outputSourceConfig: Sequence[OutputSourceUnionTypeDef],  # (2)
    resolutionTechniques: ResolutionTechniquesUnionTypeDef,  # (3)
    roleArn: str,
    workflowName: str,
    description: NotRequired[str],
    incrementalRunConfig: NotRequired[IncrementalRunConfigTypeDef],  # (4)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: InputSourceTypeDef](./type_defs.md#inputsourcetypedef) 
2. See [:material-code-braces: OutputSourceTypeDef](./type_defs.md#outputsourcetypedef) [:material-code-braces: OutputSourceOutputTypeDef](./type_defs.md#outputsourceoutputtypedef) 
3. See [:material-code-braces: ResolutionTechniquesTypeDef](./type_defs.md#resolutiontechniquestypedef) [:material-code-braces: ResolutionTechniquesOutputTypeDef](./type_defs.md#resolutiontechniquesoutputtypedef) 
4. See [:material-code-braces: IncrementalRunConfigTypeDef](./type_defs.md#incrementalrunconfigtypedef) 
## UpdateMatchingWorkflowInputTypeDef

```python
# UpdateMatchingWorkflowInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import UpdateMatchingWorkflowInputTypeDef


def get_value() -> UpdateMatchingWorkflowInputTypeDef:
    return {
        "inputSourceConfig": ...,
    }


# UpdateMatchingWorkflowInputTypeDef definition

class UpdateMatchingWorkflowInputTypeDef(TypedDict):
    inputSourceConfig: Sequence[InputSourceTypeDef],  # (1)
    outputSourceConfig: Sequence[OutputSourceUnionTypeDef],  # (2)
    resolutionTechniques: ResolutionTechniquesUnionTypeDef,  # (3)
    roleArn: str,
    workflowName: str,
    description: NotRequired[str],
    incrementalRunConfig: NotRequired[IncrementalRunConfigTypeDef],  # (4)
```

1. See [:material-code-braces: InputSourceTypeDef](./type_defs.md#inputsourcetypedef) 
2. See [:material-code-braces: OutputSourceTypeDef](./type_defs.md#outputsourcetypedef) [:material-code-braces: OutputSourceOutputTypeDef](./type_defs.md#outputsourceoutputtypedef) 
3. See [:material-code-braces: ResolutionTechniquesTypeDef](./type_defs.md#resolutiontechniquestypedef) [:material-code-braces: ResolutionTechniquesOutputTypeDef](./type_defs.md#resolutiontechniquesoutputtypedef) 
4. See [:material-code-braces: IncrementalRunConfigTypeDef](./type_defs.md#incrementalrunconfigtypedef) 
## CreateIdNamespaceInputTypeDef

```python
# CreateIdNamespaceInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import CreateIdNamespaceInputTypeDef


def get_value() -> CreateIdNamespaceInputTypeDef:
    return {
        "idNamespaceName": ...,
    }


# CreateIdNamespaceInputTypeDef definition

class CreateIdNamespaceInputTypeDef(TypedDict):
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
## UpdateIdNamespaceInputTypeDef

```python
# UpdateIdNamespaceInputTypeDef TypedDict usage example

from types_aiobotocore_entityresolution.type_defs import UpdateIdNamespaceInputTypeDef


def get_value() -> UpdateIdNamespaceInputTypeDef:
    return {
        "idNamespaceName": ...,
    }


# UpdateIdNamespaceInputTypeDef definition

class UpdateIdNamespaceInputTypeDef(TypedDict):
    idNamespaceName: str,
    description: NotRequired[str],
    idMappingWorkflowProperties: NotRequired[Sequence[IdNamespaceIdMappingWorkflowPropertiesUnionTypeDef]],  # (1)
    inputSourceConfig: NotRequired[Sequence[IdNamespaceInputSourceTypeDef]],  # (2)
    roleArn: NotRequired[str],
```

1. See [:material-code-braces: IdNamespaceIdMappingWorkflowPropertiesTypeDef](./type_defs.md#idnamespaceidmappingworkflowpropertiestypedef) [:material-code-braces: IdNamespaceIdMappingWorkflowPropertiesOutputTypeDef](./type_defs.md#idnamespaceidmappingworkflowpropertiesoutputtypedef) 
2. See [:material-code-braces: IdNamespaceInputSourceTypeDef](./type_defs.md#idnamespaceinputsourcetypedef) 
