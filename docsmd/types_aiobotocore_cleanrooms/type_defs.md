# Type definitions

> [Index](../README.md) > [CleanRoomsService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CleanRoomsService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#cleanroomsservice)
    type annotations stubs module [types-aiobotocore-cleanrooms](https://pypi.org/project/types-aiobotocore-cleanrooms/).

## MLMemberAbilitiesUnionTypeDef

```python
# MLMemberAbilitiesUnionTypeDef Union usage example

from types_aiobotocore_cleanrooms.type_defs import MLMemberAbilitiesUnionTypeDef


def get_value() -> MLMemberAbilitiesUnionTypeDef:
    return ...


# MLMemberAbilitiesUnionTypeDef definition

MLMemberAbilitiesUnionTypeDef = Union[
    MLMemberAbilitiesTypeDef,  # (1)
    MLMemberAbilitiesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MLMemberAbilitiesTypeDef](./type_defs.md#mlmemberabilitiestypedef) 
2. See [:material-code-braces: MLMemberAbilitiesOutputTypeDef](./type_defs.md#mlmemberabilitiesoutputtypedef) 

## ProtectedQuerySQLParametersUnionTypeDef

```python
# ProtectedQuerySQLParametersUnionTypeDef Union usage example

from types_aiobotocore_cleanrooms.type_defs import ProtectedQuerySQLParametersUnionTypeDef


def get_value() -> ProtectedQuerySQLParametersUnionTypeDef:
    return ...


# ProtectedQuerySQLParametersUnionTypeDef definition

ProtectedQuerySQLParametersUnionTypeDef = Union[
    ProtectedQuerySQLParametersTypeDef,  # (1)
    ProtectedQuerySQLParametersOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ProtectedQuerySQLParametersTypeDef](./type_defs.md#protectedquerysqlparameterstypedef) 
2. See [:material-code-braces: ProtectedQuerySQLParametersOutputTypeDef](./type_defs.md#protectedquerysqlparametersoutputtypedef) 

## ConfiguredTableAssociationAnalysisRulePolicyUnionTypeDef

```python
# ConfiguredTableAssociationAnalysisRulePolicyUnionTypeDef Union usage example

from types_aiobotocore_cleanrooms.type_defs import ConfiguredTableAssociationAnalysisRulePolicyUnionTypeDef


def get_value() -> ConfiguredTableAssociationAnalysisRulePolicyUnionTypeDef:
    return ...


# ConfiguredTableAssociationAnalysisRulePolicyUnionTypeDef definition

ConfiguredTableAssociationAnalysisRulePolicyUnionTypeDef = Union[
    ConfiguredTableAssociationAnalysisRulePolicyTypeDef,  # (1)
    ConfiguredTableAssociationAnalysisRulePolicyOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ConfiguredTableAssociationAnalysisRulePolicyTypeDef](./type_defs.md#configuredtableassociationanalysisrulepolicytypedef) 
2. See [:material-code-braces: ConfiguredTableAssociationAnalysisRulePolicyOutputTypeDef](./type_defs.md#configuredtableassociationanalysisrulepolicyoutputtypedef) 

## TableReferenceUnionTypeDef

```python
# TableReferenceUnionTypeDef Union usage example

from types_aiobotocore_cleanrooms.type_defs import TableReferenceUnionTypeDef


def get_value() -> TableReferenceUnionTypeDef:
    return ...


# TableReferenceUnionTypeDef definition

TableReferenceUnionTypeDef = Union[
    TableReferenceTypeDef,  # (1)
    TableReferenceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TableReferenceTypeDef](./type_defs.md#tablereferencetypedef) 
2. See [:material-code-braces: TableReferenceOutputTypeDef](./type_defs.md#tablereferenceoutputtypedef) 

## ConfiguredTableAnalysisRulePolicyUnionTypeDef

```python
# ConfiguredTableAnalysisRulePolicyUnionTypeDef Union usage example

from types_aiobotocore_cleanrooms.type_defs import ConfiguredTableAnalysisRulePolicyUnionTypeDef


def get_value() -> ConfiguredTableAnalysisRulePolicyUnionTypeDef:
    return ...


# ConfiguredTableAnalysisRulePolicyUnionTypeDef definition

ConfiguredTableAnalysisRulePolicyUnionTypeDef = Union[
    ConfiguredTableAnalysisRulePolicyTypeDef,  # (1)
    ConfiguredTableAnalysisRulePolicyOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ConfiguredTableAnalysisRulePolicyTypeDef](./type_defs.md#configuredtableanalysisrulepolicytypedef) 
2. See [:material-code-braces: ConfiguredTableAnalysisRulePolicyOutputTypeDef](./type_defs.md#configuredtableanalysisrulepolicyoutputtypedef) 



## AggregateColumnOutputTypeDef

```python
# AggregateColumnOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import AggregateColumnOutputTypeDef


def get_value() -> AggregateColumnOutputTypeDef:
    return {
        "columnNames": ...,
    }


# AggregateColumnOutputTypeDef definition

class AggregateColumnOutputTypeDef(TypedDict):
    columnNames: List[str],
    function: AggregateFunctionNameType,  # (1)
```

1. See [:material-code-brackets: AggregateFunctionNameType](./literals.md#aggregatefunctionnametype) 
## AggregateColumnTypeDef

```python
# AggregateColumnTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import AggregateColumnTypeDef


def get_value() -> AggregateColumnTypeDef:
    return {
        "columnNames": ...,
    }


# AggregateColumnTypeDef definition

class AggregateColumnTypeDef(TypedDict):
    columnNames: Sequence[str],
    function: AggregateFunctionNameType,  # (1)
```

1. See [:material-code-brackets: AggregateFunctionNameType](./literals.md#aggregatefunctionnametype) 
## AggregationConstraintTypeDef

```python
# AggregationConstraintTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import AggregationConstraintTypeDef


def get_value() -> AggregationConstraintTypeDef:
    return {
        "columnName": ...,
    }


# AggregationConstraintTypeDef definition

class AggregationConstraintTypeDef(TypedDict):
    columnName: str,
    minimum: int,
    type: AggregationTypeType,  # (1)
```

1. See [:material-code-brackets: AggregationTypeType](./literals.md#aggregationtypetype) 
## AnalysisParameterTypeDef

```python
# AnalysisParameterTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import AnalysisParameterTypeDef


def get_value() -> AnalysisParameterTypeDef:
    return {
        "name": ...,
    }


# AnalysisParameterTypeDef definition

class AnalysisParameterTypeDef(TypedDict):
    name: str,
    type: ParameterTypeType,  # (1)
    defaultValue: NotRequired[str],
```

1. See [:material-code-brackets: ParameterTypeType](./literals.md#parametertypetype) 
## AnalysisRuleListOutputTypeDef

```python
# AnalysisRuleListOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import AnalysisRuleListOutputTypeDef


def get_value() -> AnalysisRuleListOutputTypeDef:
    return {
        "joinColumns": ...,
    }


# AnalysisRuleListOutputTypeDef definition

class AnalysisRuleListOutputTypeDef(TypedDict):
    joinColumns: List[str],
    listColumns: List[str],
    allowedJoinOperators: NotRequired[List[JoinOperatorType]],  # (1)
    additionalAnalyses: NotRequired[AdditionalAnalysesType],  # (2)
```

1. See [:material-code-brackets: JoinOperatorType](./literals.md#joinoperatortype) 
2. See [:material-code-brackets: AdditionalAnalysesType](./literals.md#additionalanalysestype) 
## AnalysisRuleListTypeDef

```python
# AnalysisRuleListTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import AnalysisRuleListTypeDef


def get_value() -> AnalysisRuleListTypeDef:
    return {
        "joinColumns": ...,
    }


# AnalysisRuleListTypeDef definition

class AnalysisRuleListTypeDef(TypedDict):
    joinColumns: Sequence[str],
    listColumns: Sequence[str],
    allowedJoinOperators: NotRequired[Sequence[JoinOperatorType]],  # (1)
    additionalAnalyses: NotRequired[AdditionalAnalysesType],  # (2)
```

1. See [:material-code-brackets: JoinOperatorType](./literals.md#joinoperatortype) 
2. See [:material-code-brackets: AdditionalAnalysesType](./literals.md#additionalanalysestype) 
## AnalysisSchemaTypeDef

```python
# AnalysisSchemaTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import AnalysisSchemaTypeDef


def get_value() -> AnalysisSchemaTypeDef:
    return {
        "referencedTables": ...,
    }


# AnalysisSchemaTypeDef definition

class AnalysisSchemaTypeDef(TypedDict):
    referencedTables: NotRequired[List[str]],
```

## AnalysisSourceTypeDef

```python
# AnalysisSourceTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import AnalysisSourceTypeDef


def get_value() -> AnalysisSourceTypeDef:
    return {
        "text": ...,
    }


# AnalysisSourceTypeDef definition

class AnalysisSourceTypeDef(TypedDict):
    text: NotRequired[str],
```

## AnalysisTemplateSummaryTypeDef

```python
# AnalysisTemplateSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import AnalysisTemplateSummaryTypeDef


def get_value() -> AnalysisTemplateSummaryTypeDef:
    return {
        "arn": ...,
    }


# AnalysisTemplateSummaryTypeDef definition

class AnalysisTemplateSummaryTypeDef(TypedDict):
    arn: str,
    createTime: datetime,
    id: str,
    name: str,
    updateTime: datetime,
    membershipArn: str,
    membershipId: str,
    collaborationArn: str,
    collaborationId: str,
    description: NotRequired[str],
```

## AnalysisTemplateValidationStatusReasonTypeDef

```python
# AnalysisTemplateValidationStatusReasonTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import AnalysisTemplateValidationStatusReasonTypeDef


def get_value() -> AnalysisTemplateValidationStatusReasonTypeDef:
    return {
        "message": ...,
    }


# AnalysisTemplateValidationStatusReasonTypeDef definition

class AnalysisTemplateValidationStatusReasonTypeDef(TypedDict):
    message: str,
```

## AthenaTableReferenceTypeDef

```python
# AthenaTableReferenceTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import AthenaTableReferenceTypeDef


def get_value() -> AthenaTableReferenceTypeDef:
    return {
        "workGroup": ...,
    }


# AthenaTableReferenceTypeDef definition

class AthenaTableReferenceTypeDef(TypedDict):
    workGroup: str,
    databaseName: str,
    tableName: str,
    outputLocation: NotRequired[str],
```

## BatchGetCollaborationAnalysisTemplateErrorTypeDef

```python
# BatchGetCollaborationAnalysisTemplateErrorTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import BatchGetCollaborationAnalysisTemplateErrorTypeDef


def get_value() -> BatchGetCollaborationAnalysisTemplateErrorTypeDef:
    return {
        "arn": ...,
    }


# BatchGetCollaborationAnalysisTemplateErrorTypeDef definition

class BatchGetCollaborationAnalysisTemplateErrorTypeDef(TypedDict):
    arn: str,
    code: str,
    message: str,
```

## BatchGetCollaborationAnalysisTemplateInputTypeDef

```python
# BatchGetCollaborationAnalysisTemplateInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import BatchGetCollaborationAnalysisTemplateInputTypeDef


def get_value() -> BatchGetCollaborationAnalysisTemplateInputTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# BatchGetCollaborationAnalysisTemplateInputTypeDef definition

class BatchGetCollaborationAnalysisTemplateInputTypeDef(TypedDict):
    collaborationIdentifier: str,
    analysisTemplateArns: Sequence[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ResponseMetadataTypeDef


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

## BatchGetSchemaAnalysisRuleErrorTypeDef

```python
# BatchGetSchemaAnalysisRuleErrorTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import BatchGetSchemaAnalysisRuleErrorTypeDef


def get_value() -> BatchGetSchemaAnalysisRuleErrorTypeDef:
    return {
        "name": ...,
    }


# BatchGetSchemaAnalysisRuleErrorTypeDef definition

class BatchGetSchemaAnalysisRuleErrorTypeDef(TypedDict):
    name: str,
    type: AnalysisRuleTypeType,  # (1)
    code: str,
    message: str,
```

1. See [:material-code-brackets: AnalysisRuleTypeType](./literals.md#analysisruletypetype) 
## SchemaAnalysisRuleRequestTypeDef

```python
# SchemaAnalysisRuleRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import SchemaAnalysisRuleRequestTypeDef


def get_value() -> SchemaAnalysisRuleRequestTypeDef:
    return {
        "name": ...,
    }


# SchemaAnalysisRuleRequestTypeDef definition

class SchemaAnalysisRuleRequestTypeDef(TypedDict):
    name: str,
    type: AnalysisRuleTypeType,  # (1)
```

1. See [:material-code-brackets: AnalysisRuleTypeType](./literals.md#analysisruletypetype) 
## BatchGetSchemaErrorTypeDef

```python
# BatchGetSchemaErrorTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import BatchGetSchemaErrorTypeDef


def get_value() -> BatchGetSchemaErrorTypeDef:
    return {
        "name": ...,
    }


# BatchGetSchemaErrorTypeDef definition

class BatchGetSchemaErrorTypeDef(TypedDict):
    name: str,
    code: str,
    message: str,
```

## BatchGetSchemaInputTypeDef

```python
# BatchGetSchemaInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import BatchGetSchemaInputTypeDef


def get_value() -> BatchGetSchemaInputTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# BatchGetSchemaInputTypeDef definition

class BatchGetSchemaInputTypeDef(TypedDict):
    collaborationIdentifier: str,
    names: Sequence[str],
```

## BilledResourceUtilizationTypeDef

```python
# BilledResourceUtilizationTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import BilledResourceUtilizationTypeDef


def get_value() -> BilledResourceUtilizationTypeDef:
    return {
        "units": ...,
    }


# BilledResourceUtilizationTypeDef definition

class BilledResourceUtilizationTypeDef(TypedDict):
    units: float,
```

## CollaborationAnalysisTemplateSummaryTypeDef

```python
# CollaborationAnalysisTemplateSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CollaborationAnalysisTemplateSummaryTypeDef


def get_value() -> CollaborationAnalysisTemplateSummaryTypeDef:
    return {
        "arn": ...,
    }


# CollaborationAnalysisTemplateSummaryTypeDef definition

class CollaborationAnalysisTemplateSummaryTypeDef(TypedDict):
    arn: str,
    createTime: datetime,
    id: str,
    name: str,
    updateTime: datetime,
    collaborationArn: str,
    collaborationId: str,
    creatorAccountId: str,
    description: NotRequired[str],
```

## CollaborationConfiguredAudienceModelAssociationSummaryTypeDef

```python
# CollaborationConfiguredAudienceModelAssociationSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CollaborationConfiguredAudienceModelAssociationSummaryTypeDef


def get_value() -> CollaborationConfiguredAudienceModelAssociationSummaryTypeDef:
    return {
        "arn": ...,
    }


# CollaborationConfiguredAudienceModelAssociationSummaryTypeDef definition

class CollaborationConfiguredAudienceModelAssociationSummaryTypeDef(TypedDict):
    arn: str,
    createTime: datetime,
    id: str,
    name: str,
    updateTime: datetime,
    collaborationArn: str,
    collaborationId: str,
    creatorAccountId: str,
    description: NotRequired[str],
```

## CollaborationConfiguredAudienceModelAssociationTypeDef

```python
# CollaborationConfiguredAudienceModelAssociationTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CollaborationConfiguredAudienceModelAssociationTypeDef


def get_value() -> CollaborationConfiguredAudienceModelAssociationTypeDef:
    return {
        "id": ...,
    }


# CollaborationConfiguredAudienceModelAssociationTypeDef definition

class CollaborationConfiguredAudienceModelAssociationTypeDef(TypedDict):
    id: str,
    arn: str,
    collaborationId: str,
    collaborationArn: str,
    configuredAudienceModelArn: str,
    name: str,
    creatorAccountId: str,
    createTime: datetime,
    updateTime: datetime,
    description: NotRequired[str],
```

## IdNamespaceAssociationInputReferenceConfigTypeDef

```python
# IdNamespaceAssociationInputReferenceConfigTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import IdNamespaceAssociationInputReferenceConfigTypeDef


def get_value() -> IdNamespaceAssociationInputReferenceConfigTypeDef:
    return {
        "inputReferenceArn": ...,
    }


# IdNamespaceAssociationInputReferenceConfigTypeDef definition

class IdNamespaceAssociationInputReferenceConfigTypeDef(TypedDict):
    inputReferenceArn: str,
    manageResourcePolicies: bool,
```

## IdNamespaceAssociationInputReferencePropertiesSummaryTypeDef

```python
# IdNamespaceAssociationInputReferencePropertiesSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import IdNamespaceAssociationInputReferencePropertiesSummaryTypeDef


def get_value() -> IdNamespaceAssociationInputReferencePropertiesSummaryTypeDef:
    return {
        "idNamespaceType": ...,
    }


# IdNamespaceAssociationInputReferencePropertiesSummaryTypeDef definition

class IdNamespaceAssociationInputReferencePropertiesSummaryTypeDef(TypedDict):
    idNamespaceType: IdNamespaceTypeType,  # (1)
```

1. See [:material-code-brackets: IdNamespaceTypeType](./literals.md#idnamespacetypetype) 
## IdMappingConfigTypeDef

```python
# IdMappingConfigTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import IdMappingConfigTypeDef


def get_value() -> IdMappingConfigTypeDef:
    return {
        "allowUseAsDimensionColumn": ...,
    }


# IdMappingConfigTypeDef definition

class IdMappingConfigTypeDef(TypedDict):
    allowUseAsDimensionColumn: bool,
```

## IdNamespaceAssociationInputReferencePropertiesTypeDef

```python
# IdNamespaceAssociationInputReferencePropertiesTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import IdNamespaceAssociationInputReferencePropertiesTypeDef


def get_value() -> IdNamespaceAssociationInputReferencePropertiesTypeDef:
    return {
        "idNamespaceType": ...,
    }


# IdNamespaceAssociationInputReferencePropertiesTypeDef definition

class IdNamespaceAssociationInputReferencePropertiesTypeDef(TypedDict):
    idNamespaceType: IdNamespaceTypeType,  # (1)
    idMappingWorkflowsSupported: List[Dict[str, Any]],
```

1. See [:material-code-brackets: IdNamespaceTypeType](./literals.md#idnamespacetypetype) 
## CollaborationPrivacyBudgetTemplateSummaryTypeDef

```python
# CollaborationPrivacyBudgetTemplateSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CollaborationPrivacyBudgetTemplateSummaryTypeDef


def get_value() -> CollaborationPrivacyBudgetTemplateSummaryTypeDef:
    return {
        "id": ...,
    }


# CollaborationPrivacyBudgetTemplateSummaryTypeDef definition

class CollaborationPrivacyBudgetTemplateSummaryTypeDef(TypedDict):
    id: str,
    arn: str,
    collaborationId: str,
    collaborationArn: str,
    creatorAccountId: str,
    privacyBudgetType: PrivacyBudgetTypeType,  # (1)
    createTime: datetime,
    updateTime: datetime,
```

1. See [:material-code-brackets: PrivacyBudgetTypeType](./literals.md#privacybudgettypetype) 
## CollaborationSummaryTypeDef

```python
# CollaborationSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CollaborationSummaryTypeDef


def get_value() -> CollaborationSummaryTypeDef:
    return {
        "id": ...,
    }


# CollaborationSummaryTypeDef definition

class CollaborationSummaryTypeDef(TypedDict):
    id: str,
    arn: str,
    name: str,
    creatorAccountId: str,
    creatorDisplayName: str,
    createTime: datetime,
    updateTime: datetime,
    memberStatus: MemberStatusType,  # (1)
    membershipId: NotRequired[str],
    membershipArn: NotRequired[str],
    analyticsEngine: NotRequired[AnalyticsEngineType],  # (2)
```

1. See [:material-code-brackets: MemberStatusType](./literals.md#memberstatustype) 
2. See [:material-code-brackets: AnalyticsEngineType](./literals.md#analyticsenginetype) 
## DataEncryptionMetadataTypeDef

```python
# DataEncryptionMetadataTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import DataEncryptionMetadataTypeDef


def get_value() -> DataEncryptionMetadataTypeDef:
    return {
        "allowCleartext": ...,
    }


# DataEncryptionMetadataTypeDef definition

class DataEncryptionMetadataTypeDef(TypedDict):
    allowCleartext: bool,
    allowDuplicates: bool,
    allowJoinsOnColumnsWithDifferentNames: bool,
    preserveNulls: bool,
```

## ColumnTypeDef

```python
# ColumnTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ColumnTypeDef


def get_value() -> ColumnTypeDef:
    return {
        "name": ...,
    }


# ColumnTypeDef definition

class ColumnTypeDef(TypedDict):
    name: str,
    type: str,
```

## WorkerComputeConfigurationTypeDef

```python
# WorkerComputeConfigurationTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import WorkerComputeConfigurationTypeDef


def get_value() -> WorkerComputeConfigurationTypeDef:
    return {
        "type": ...,
    }


# WorkerComputeConfigurationTypeDef definition

class WorkerComputeConfigurationTypeDef(TypedDict):
    type: NotRequired[WorkerComputeTypeType],  # (1)
    number: NotRequired[int],
```

1. See [:material-code-brackets: WorkerComputeTypeType](./literals.md#workercomputetypetype) 
## DirectAnalysisConfigurationDetailsTypeDef

```python
# DirectAnalysisConfigurationDetailsTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import DirectAnalysisConfigurationDetailsTypeDef


def get_value() -> DirectAnalysisConfigurationDetailsTypeDef:
    return {
        "receiverAccountIds": ...,
    }


# DirectAnalysisConfigurationDetailsTypeDef definition

class DirectAnalysisConfigurationDetailsTypeDef(TypedDict):
    receiverAccountIds: NotRequired[List[str]],
```

## ConfiguredAudienceModelAssociationSummaryTypeDef

```python
# ConfiguredAudienceModelAssociationSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ConfiguredAudienceModelAssociationSummaryTypeDef


def get_value() -> ConfiguredAudienceModelAssociationSummaryTypeDef:
    return {
        "membershipId": ...,
    }


# ConfiguredAudienceModelAssociationSummaryTypeDef definition

class ConfiguredAudienceModelAssociationSummaryTypeDef(TypedDict):
    membershipId: str,
    membershipArn: str,
    collaborationArn: str,
    collaborationId: str,
    createTime: datetime,
    updateTime: datetime,
    id: str,
    arn: str,
    name: str,
    configuredAudienceModelArn: str,
    description: NotRequired[str],
```

## ConfiguredAudienceModelAssociationTypeDef

```python
# ConfiguredAudienceModelAssociationTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ConfiguredAudienceModelAssociationTypeDef


def get_value() -> ConfiguredAudienceModelAssociationTypeDef:
    return {
        "id": ...,
    }


# ConfiguredAudienceModelAssociationTypeDef definition

class ConfiguredAudienceModelAssociationTypeDef(TypedDict):
    id: str,
    arn: str,
    configuredAudienceModelArn: str,
    membershipId: str,
    membershipArn: str,
    collaborationId: str,
    collaborationArn: str,
    name: str,
    manageResourcePolicies: bool,
    createTime: datetime,
    updateTime: datetime,
    description: NotRequired[str],
```

## ConfiguredTableAssociationAnalysisRuleAggregationOutputTypeDef

```python
# ConfiguredTableAssociationAnalysisRuleAggregationOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ConfiguredTableAssociationAnalysisRuleAggregationOutputTypeDef


def get_value() -> ConfiguredTableAssociationAnalysisRuleAggregationOutputTypeDef:
    return {
        "allowedResultReceivers": ...,
    }


# ConfiguredTableAssociationAnalysisRuleAggregationOutputTypeDef definition

class ConfiguredTableAssociationAnalysisRuleAggregationOutputTypeDef(TypedDict):
    allowedResultReceivers: NotRequired[List[str]],
    allowedAdditionalAnalyses: NotRequired[List[str]],
```

## ConfiguredTableAssociationAnalysisRuleAggregationTypeDef

```python
# ConfiguredTableAssociationAnalysisRuleAggregationTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ConfiguredTableAssociationAnalysisRuleAggregationTypeDef


def get_value() -> ConfiguredTableAssociationAnalysisRuleAggregationTypeDef:
    return {
        "allowedResultReceivers": ...,
    }


# ConfiguredTableAssociationAnalysisRuleAggregationTypeDef definition

class ConfiguredTableAssociationAnalysisRuleAggregationTypeDef(TypedDict):
    allowedResultReceivers: NotRequired[Sequence[str]],
    allowedAdditionalAnalyses: NotRequired[Sequence[str]],
```

## ConfiguredTableAssociationAnalysisRuleCustomOutputTypeDef

```python
# ConfiguredTableAssociationAnalysisRuleCustomOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ConfiguredTableAssociationAnalysisRuleCustomOutputTypeDef


def get_value() -> ConfiguredTableAssociationAnalysisRuleCustomOutputTypeDef:
    return {
        "allowedResultReceivers": ...,
    }


# ConfiguredTableAssociationAnalysisRuleCustomOutputTypeDef definition

class ConfiguredTableAssociationAnalysisRuleCustomOutputTypeDef(TypedDict):
    allowedResultReceivers: NotRequired[List[str]],
    allowedAdditionalAnalyses: NotRequired[List[str]],
```

## ConfiguredTableAssociationAnalysisRuleCustomTypeDef

```python
# ConfiguredTableAssociationAnalysisRuleCustomTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ConfiguredTableAssociationAnalysisRuleCustomTypeDef


def get_value() -> ConfiguredTableAssociationAnalysisRuleCustomTypeDef:
    return {
        "allowedResultReceivers": ...,
    }


# ConfiguredTableAssociationAnalysisRuleCustomTypeDef definition

class ConfiguredTableAssociationAnalysisRuleCustomTypeDef(TypedDict):
    allowedResultReceivers: NotRequired[Sequence[str]],
    allowedAdditionalAnalyses: NotRequired[Sequence[str]],
```

## ConfiguredTableAssociationAnalysisRuleListOutputTypeDef

```python
# ConfiguredTableAssociationAnalysisRuleListOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ConfiguredTableAssociationAnalysisRuleListOutputTypeDef


def get_value() -> ConfiguredTableAssociationAnalysisRuleListOutputTypeDef:
    return {
        "allowedResultReceivers": ...,
    }


# ConfiguredTableAssociationAnalysisRuleListOutputTypeDef definition

class ConfiguredTableAssociationAnalysisRuleListOutputTypeDef(TypedDict):
    allowedResultReceivers: NotRequired[List[str]],
    allowedAdditionalAnalyses: NotRequired[List[str]],
```

## ConfiguredTableAssociationAnalysisRuleListTypeDef

```python
# ConfiguredTableAssociationAnalysisRuleListTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ConfiguredTableAssociationAnalysisRuleListTypeDef


def get_value() -> ConfiguredTableAssociationAnalysisRuleListTypeDef:
    return {
        "allowedResultReceivers": ...,
    }


# ConfiguredTableAssociationAnalysisRuleListTypeDef definition

class ConfiguredTableAssociationAnalysisRuleListTypeDef(TypedDict):
    allowedResultReceivers: NotRequired[Sequence[str]],
    allowedAdditionalAnalyses: NotRequired[Sequence[str]],
```

## ConfiguredTableAssociationSummaryTypeDef

```python
# ConfiguredTableAssociationSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ConfiguredTableAssociationSummaryTypeDef


def get_value() -> ConfiguredTableAssociationSummaryTypeDef:
    return {
        "configuredTableId": ...,
    }


# ConfiguredTableAssociationSummaryTypeDef definition

class ConfiguredTableAssociationSummaryTypeDef(TypedDict):
    configuredTableId: str,
    membershipId: str,
    membershipArn: str,
    name: str,
    createTime: datetime,
    updateTime: datetime,
    id: str,
    arn: str,
```

## ConfiguredTableAssociationTypeDef

```python
# ConfiguredTableAssociationTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ConfiguredTableAssociationTypeDef


def get_value() -> ConfiguredTableAssociationTypeDef:
    return {
        "arn": ...,
    }


# ConfiguredTableAssociationTypeDef definition

class ConfiguredTableAssociationTypeDef(TypedDict):
    arn: str,
    id: str,
    configuredTableId: str,
    configuredTableArn: str,
    membershipId: str,
    membershipArn: str,
    roleArn: str,
    name: str,
    createTime: datetime,
    updateTime: datetime,
    description: NotRequired[str],
    analysisRuleTypes: NotRequired[List[ConfiguredTableAssociationAnalysisRuleTypeType]],  # (1)
```

1. See [:material-code-brackets: ConfiguredTableAssociationAnalysisRuleTypeType](./literals.md#configuredtableassociationanalysisruletypetype) 
## ConfiguredTableSummaryTypeDef

```python
# ConfiguredTableSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ConfiguredTableSummaryTypeDef


def get_value() -> ConfiguredTableSummaryTypeDef:
    return {
        "id": ...,
    }


# ConfiguredTableSummaryTypeDef definition

class ConfiguredTableSummaryTypeDef(TypedDict):
    id: str,
    arn: str,
    name: str,
    createTime: datetime,
    updateTime: datetime,
    analysisRuleTypes: List[ConfiguredTableAnalysisRuleTypeType],  # (1)
    analysisMethod: AnalysisMethodType,  # (2)
```

1. See [:material-code-brackets: ConfiguredTableAnalysisRuleTypeType](./literals.md#configuredtableanalysisruletypetype) 
2. See [:material-code-brackets: AnalysisMethodType](./literals.md#analysismethodtype) 
## CreateConfiguredAudienceModelAssociationInputTypeDef

```python
# CreateConfiguredAudienceModelAssociationInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CreateConfiguredAudienceModelAssociationInputTypeDef


def get_value() -> CreateConfiguredAudienceModelAssociationInputTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# CreateConfiguredAudienceModelAssociationInputTypeDef definition

class CreateConfiguredAudienceModelAssociationInputTypeDef(TypedDict):
    membershipIdentifier: str,
    configuredAudienceModelArn: str,
    configuredAudienceModelAssociationName: str,
    manageResourcePolicies: bool,
    tags: NotRequired[Mapping[str, str]],
    description: NotRequired[str],
```

## CreateConfiguredTableAssociationInputTypeDef

```python
# CreateConfiguredTableAssociationInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CreateConfiguredTableAssociationInputTypeDef


def get_value() -> CreateConfiguredTableAssociationInputTypeDef:
    return {
        "name": ...,
    }


# CreateConfiguredTableAssociationInputTypeDef definition

class CreateConfiguredTableAssociationInputTypeDef(TypedDict):
    name: str,
    membershipIdentifier: str,
    configuredTableIdentifier: str,
    roleArn: str,
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## IdMappingTableInputReferenceConfigTypeDef

```python
# IdMappingTableInputReferenceConfigTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import IdMappingTableInputReferenceConfigTypeDef


def get_value() -> IdMappingTableInputReferenceConfigTypeDef:
    return {
        "inputReferenceArn": ...,
    }


# IdMappingTableInputReferenceConfigTypeDef definition

class IdMappingTableInputReferenceConfigTypeDef(TypedDict):
    inputReferenceArn: str,
    manageResourcePolicies: bool,
```

## DeleteAnalysisTemplateInputTypeDef

```python
# DeleteAnalysisTemplateInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import DeleteAnalysisTemplateInputTypeDef


def get_value() -> DeleteAnalysisTemplateInputTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# DeleteAnalysisTemplateInputTypeDef definition

class DeleteAnalysisTemplateInputTypeDef(TypedDict):
    membershipIdentifier: str,
    analysisTemplateIdentifier: str,
```

## DeleteCollaborationInputTypeDef

```python
# DeleteCollaborationInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import DeleteCollaborationInputTypeDef


def get_value() -> DeleteCollaborationInputTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# DeleteCollaborationInputTypeDef definition

class DeleteCollaborationInputTypeDef(TypedDict):
    collaborationIdentifier: str,
```

## DeleteConfiguredAudienceModelAssociationInputTypeDef

```python
# DeleteConfiguredAudienceModelAssociationInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import DeleteConfiguredAudienceModelAssociationInputTypeDef


def get_value() -> DeleteConfiguredAudienceModelAssociationInputTypeDef:
    return {
        "configuredAudienceModelAssociationIdentifier": ...,
    }


# DeleteConfiguredAudienceModelAssociationInputTypeDef definition

class DeleteConfiguredAudienceModelAssociationInputTypeDef(TypedDict):
    configuredAudienceModelAssociationIdentifier: str,
    membershipIdentifier: str,
```

## DeleteConfiguredTableAnalysisRuleInputTypeDef

```python
# DeleteConfiguredTableAnalysisRuleInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import DeleteConfiguredTableAnalysisRuleInputTypeDef


def get_value() -> DeleteConfiguredTableAnalysisRuleInputTypeDef:
    return {
        "configuredTableIdentifier": ...,
    }


# DeleteConfiguredTableAnalysisRuleInputTypeDef definition

class DeleteConfiguredTableAnalysisRuleInputTypeDef(TypedDict):
    configuredTableIdentifier: str,
    analysisRuleType: ConfiguredTableAnalysisRuleTypeType,  # (1)
```

1. See [:material-code-brackets: ConfiguredTableAnalysisRuleTypeType](./literals.md#configuredtableanalysisruletypetype) 
## DeleteConfiguredTableAssociationAnalysisRuleInputTypeDef

```python
# DeleteConfiguredTableAssociationAnalysisRuleInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import DeleteConfiguredTableAssociationAnalysisRuleInputTypeDef


def get_value() -> DeleteConfiguredTableAssociationAnalysisRuleInputTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# DeleteConfiguredTableAssociationAnalysisRuleInputTypeDef definition

class DeleteConfiguredTableAssociationAnalysisRuleInputTypeDef(TypedDict):
    membershipIdentifier: str,
    configuredTableAssociationIdentifier: str,
    analysisRuleType: ConfiguredTableAssociationAnalysisRuleTypeType,  # (1)
```

1. See [:material-code-brackets: ConfiguredTableAssociationAnalysisRuleTypeType](./literals.md#configuredtableassociationanalysisruletypetype) 
## DeleteConfiguredTableAssociationInputTypeDef

```python
# DeleteConfiguredTableAssociationInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import DeleteConfiguredTableAssociationInputTypeDef


def get_value() -> DeleteConfiguredTableAssociationInputTypeDef:
    return {
        "configuredTableAssociationIdentifier": ...,
    }


# DeleteConfiguredTableAssociationInputTypeDef definition

class DeleteConfiguredTableAssociationInputTypeDef(TypedDict):
    configuredTableAssociationIdentifier: str,
    membershipIdentifier: str,
```

## DeleteConfiguredTableInputTypeDef

```python
# DeleteConfiguredTableInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import DeleteConfiguredTableInputTypeDef


def get_value() -> DeleteConfiguredTableInputTypeDef:
    return {
        "configuredTableIdentifier": ...,
    }


# DeleteConfiguredTableInputTypeDef definition

class DeleteConfiguredTableInputTypeDef(TypedDict):
    configuredTableIdentifier: str,
```

## DeleteIdMappingTableInputTypeDef

```python
# DeleteIdMappingTableInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import DeleteIdMappingTableInputTypeDef


def get_value() -> DeleteIdMappingTableInputTypeDef:
    return {
        "idMappingTableIdentifier": ...,
    }


# DeleteIdMappingTableInputTypeDef definition

class DeleteIdMappingTableInputTypeDef(TypedDict):
    idMappingTableIdentifier: str,
    membershipIdentifier: str,
```

## DeleteIdNamespaceAssociationInputTypeDef

```python
# DeleteIdNamespaceAssociationInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import DeleteIdNamespaceAssociationInputTypeDef


def get_value() -> DeleteIdNamespaceAssociationInputTypeDef:
    return {
        "idNamespaceAssociationIdentifier": ...,
    }


# DeleteIdNamespaceAssociationInputTypeDef definition

class DeleteIdNamespaceAssociationInputTypeDef(TypedDict):
    idNamespaceAssociationIdentifier: str,
    membershipIdentifier: str,
```

## DeleteMemberInputTypeDef

```python
# DeleteMemberInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import DeleteMemberInputTypeDef


def get_value() -> DeleteMemberInputTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# DeleteMemberInputTypeDef definition

class DeleteMemberInputTypeDef(TypedDict):
    collaborationIdentifier: str,
    accountId: str,
```

## DeleteMembershipInputTypeDef

```python
# DeleteMembershipInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import DeleteMembershipInputTypeDef


def get_value() -> DeleteMembershipInputTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# DeleteMembershipInputTypeDef definition

class DeleteMembershipInputTypeDef(TypedDict):
    membershipIdentifier: str,
```

## DeletePrivacyBudgetTemplateInputTypeDef

```python
# DeletePrivacyBudgetTemplateInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import DeletePrivacyBudgetTemplateInputTypeDef


def get_value() -> DeletePrivacyBudgetTemplateInputTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# DeletePrivacyBudgetTemplateInputTypeDef definition

class DeletePrivacyBudgetTemplateInputTypeDef(TypedDict):
    membershipIdentifier: str,
    privacyBudgetTemplateIdentifier: str,
```

## DifferentialPrivacyColumnTypeDef

```python
# DifferentialPrivacyColumnTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import DifferentialPrivacyColumnTypeDef


def get_value() -> DifferentialPrivacyColumnTypeDef:
    return {
        "name": ...,
    }


# DifferentialPrivacyColumnTypeDef definition

class DifferentialPrivacyColumnTypeDef(TypedDict):
    name: str,
```

## DifferentialPrivacySensitivityParametersTypeDef

```python
# DifferentialPrivacySensitivityParametersTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import DifferentialPrivacySensitivityParametersTypeDef


def get_value() -> DifferentialPrivacySensitivityParametersTypeDef:
    return {
        "aggregationType": ...,
    }


# DifferentialPrivacySensitivityParametersTypeDef definition

class DifferentialPrivacySensitivityParametersTypeDef(TypedDict):
    aggregationType: DifferentialPrivacyAggregationTypeType,  # (1)
    aggregationExpression: str,
    userContributionLimit: int,
    minColumnValue: NotRequired[float],
    maxColumnValue: NotRequired[float],
```

1. See [:material-code-brackets: DifferentialPrivacyAggregationTypeType](./literals.md#differentialprivacyaggregationtypetype) 
## DifferentialPrivacyPreviewAggregationTypeDef

```python
# DifferentialPrivacyPreviewAggregationTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import DifferentialPrivacyPreviewAggregationTypeDef


def get_value() -> DifferentialPrivacyPreviewAggregationTypeDef:
    return {
        "type": ...,
    }


# DifferentialPrivacyPreviewAggregationTypeDef definition

class DifferentialPrivacyPreviewAggregationTypeDef(TypedDict):
    type: DifferentialPrivacyAggregationTypeType,  # (1)
    maxCount: int,
```

1. See [:material-code-brackets: DifferentialPrivacyAggregationTypeType](./literals.md#differentialprivacyaggregationtypetype) 
## DifferentialPrivacyPreviewParametersInputTypeDef

```python
# DifferentialPrivacyPreviewParametersInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import DifferentialPrivacyPreviewParametersInputTypeDef


def get_value() -> DifferentialPrivacyPreviewParametersInputTypeDef:
    return {
        "epsilon": ...,
    }


# DifferentialPrivacyPreviewParametersInputTypeDef definition

class DifferentialPrivacyPreviewParametersInputTypeDef(TypedDict):
    epsilon: int,
    usersNoisePerQuery: int,
```

## DifferentialPrivacyPrivacyBudgetAggregationTypeDef

```python
# DifferentialPrivacyPrivacyBudgetAggregationTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import DifferentialPrivacyPrivacyBudgetAggregationTypeDef


def get_value() -> DifferentialPrivacyPrivacyBudgetAggregationTypeDef:
    return {
        "type": ...,
    }


# DifferentialPrivacyPrivacyBudgetAggregationTypeDef definition

class DifferentialPrivacyPrivacyBudgetAggregationTypeDef(TypedDict):
    type: DifferentialPrivacyAggregationTypeType,  # (1)
    maxCount: int,
    remainingCount: int,
```

1. See [:material-code-brackets: DifferentialPrivacyAggregationTypeType](./literals.md#differentialprivacyaggregationtypetype) 
## DifferentialPrivacyTemplateParametersInputTypeDef

```python
# DifferentialPrivacyTemplateParametersInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import DifferentialPrivacyTemplateParametersInputTypeDef


def get_value() -> DifferentialPrivacyTemplateParametersInputTypeDef:
    return {
        "epsilon": ...,
    }


# DifferentialPrivacyTemplateParametersInputTypeDef definition

class DifferentialPrivacyTemplateParametersInputTypeDef(TypedDict):
    epsilon: int,
    usersNoisePerQuery: int,
```

## DifferentialPrivacyTemplateParametersOutputTypeDef

```python
# DifferentialPrivacyTemplateParametersOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import DifferentialPrivacyTemplateParametersOutputTypeDef


def get_value() -> DifferentialPrivacyTemplateParametersOutputTypeDef:
    return {
        "epsilon": ...,
    }


# DifferentialPrivacyTemplateParametersOutputTypeDef definition

class DifferentialPrivacyTemplateParametersOutputTypeDef(TypedDict):
    epsilon: int,
    usersNoisePerQuery: int,
```

## DifferentialPrivacyTemplateUpdateParametersTypeDef

```python
# DifferentialPrivacyTemplateUpdateParametersTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import DifferentialPrivacyTemplateUpdateParametersTypeDef


def get_value() -> DifferentialPrivacyTemplateUpdateParametersTypeDef:
    return {
        "epsilon": ...,
    }


# DifferentialPrivacyTemplateUpdateParametersTypeDef definition

class DifferentialPrivacyTemplateUpdateParametersTypeDef(TypedDict):
    epsilon: NotRequired[int],
    usersNoisePerQuery: NotRequired[int],
```

## GetAnalysisTemplateInputTypeDef

```python
# GetAnalysisTemplateInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetAnalysisTemplateInputTypeDef


def get_value() -> GetAnalysisTemplateInputTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# GetAnalysisTemplateInputTypeDef definition

class GetAnalysisTemplateInputTypeDef(TypedDict):
    membershipIdentifier: str,
    analysisTemplateIdentifier: str,
```

## GetCollaborationAnalysisTemplateInputTypeDef

```python
# GetCollaborationAnalysisTemplateInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetCollaborationAnalysisTemplateInputTypeDef


def get_value() -> GetCollaborationAnalysisTemplateInputTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# GetCollaborationAnalysisTemplateInputTypeDef definition

class GetCollaborationAnalysisTemplateInputTypeDef(TypedDict):
    collaborationIdentifier: str,
    analysisTemplateArn: str,
```

## GetCollaborationConfiguredAudienceModelAssociationInputTypeDef

```python
# GetCollaborationConfiguredAudienceModelAssociationInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetCollaborationConfiguredAudienceModelAssociationInputTypeDef


def get_value() -> GetCollaborationConfiguredAudienceModelAssociationInputTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# GetCollaborationConfiguredAudienceModelAssociationInputTypeDef definition

class GetCollaborationConfiguredAudienceModelAssociationInputTypeDef(TypedDict):
    collaborationIdentifier: str,
    configuredAudienceModelAssociationIdentifier: str,
```

## GetCollaborationIdNamespaceAssociationInputTypeDef

```python
# GetCollaborationIdNamespaceAssociationInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetCollaborationIdNamespaceAssociationInputTypeDef


def get_value() -> GetCollaborationIdNamespaceAssociationInputTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# GetCollaborationIdNamespaceAssociationInputTypeDef definition

class GetCollaborationIdNamespaceAssociationInputTypeDef(TypedDict):
    collaborationIdentifier: str,
    idNamespaceAssociationIdentifier: str,
```

## GetCollaborationInputTypeDef

```python
# GetCollaborationInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetCollaborationInputTypeDef


def get_value() -> GetCollaborationInputTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# GetCollaborationInputTypeDef definition

class GetCollaborationInputTypeDef(TypedDict):
    collaborationIdentifier: str,
```

## GetCollaborationPrivacyBudgetTemplateInputTypeDef

```python
# GetCollaborationPrivacyBudgetTemplateInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetCollaborationPrivacyBudgetTemplateInputTypeDef


def get_value() -> GetCollaborationPrivacyBudgetTemplateInputTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# GetCollaborationPrivacyBudgetTemplateInputTypeDef definition

class GetCollaborationPrivacyBudgetTemplateInputTypeDef(TypedDict):
    collaborationIdentifier: str,
    privacyBudgetTemplateIdentifier: str,
```

## GetConfiguredAudienceModelAssociationInputTypeDef

```python
# GetConfiguredAudienceModelAssociationInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetConfiguredAudienceModelAssociationInputTypeDef


def get_value() -> GetConfiguredAudienceModelAssociationInputTypeDef:
    return {
        "configuredAudienceModelAssociationIdentifier": ...,
    }


# GetConfiguredAudienceModelAssociationInputTypeDef definition

class GetConfiguredAudienceModelAssociationInputTypeDef(TypedDict):
    configuredAudienceModelAssociationIdentifier: str,
    membershipIdentifier: str,
```

## GetConfiguredTableAnalysisRuleInputTypeDef

```python
# GetConfiguredTableAnalysisRuleInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetConfiguredTableAnalysisRuleInputTypeDef


def get_value() -> GetConfiguredTableAnalysisRuleInputTypeDef:
    return {
        "configuredTableIdentifier": ...,
    }


# GetConfiguredTableAnalysisRuleInputTypeDef definition

class GetConfiguredTableAnalysisRuleInputTypeDef(TypedDict):
    configuredTableIdentifier: str,
    analysisRuleType: ConfiguredTableAnalysisRuleTypeType,  # (1)
```

1. See [:material-code-brackets: ConfiguredTableAnalysisRuleTypeType](./literals.md#configuredtableanalysisruletypetype) 
## GetConfiguredTableAssociationAnalysisRuleInputTypeDef

```python
# GetConfiguredTableAssociationAnalysisRuleInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetConfiguredTableAssociationAnalysisRuleInputTypeDef


def get_value() -> GetConfiguredTableAssociationAnalysisRuleInputTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# GetConfiguredTableAssociationAnalysisRuleInputTypeDef definition

class GetConfiguredTableAssociationAnalysisRuleInputTypeDef(TypedDict):
    membershipIdentifier: str,
    configuredTableAssociationIdentifier: str,
    analysisRuleType: ConfiguredTableAssociationAnalysisRuleTypeType,  # (1)
```

1. See [:material-code-brackets: ConfiguredTableAssociationAnalysisRuleTypeType](./literals.md#configuredtableassociationanalysisruletypetype) 
## GetConfiguredTableAssociationInputTypeDef

```python
# GetConfiguredTableAssociationInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetConfiguredTableAssociationInputTypeDef


def get_value() -> GetConfiguredTableAssociationInputTypeDef:
    return {
        "configuredTableAssociationIdentifier": ...,
    }


# GetConfiguredTableAssociationInputTypeDef definition

class GetConfiguredTableAssociationInputTypeDef(TypedDict):
    configuredTableAssociationIdentifier: str,
    membershipIdentifier: str,
```

## GetConfiguredTableInputTypeDef

```python
# GetConfiguredTableInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetConfiguredTableInputTypeDef


def get_value() -> GetConfiguredTableInputTypeDef:
    return {
        "configuredTableIdentifier": ...,
    }


# GetConfiguredTableInputTypeDef definition

class GetConfiguredTableInputTypeDef(TypedDict):
    configuredTableIdentifier: str,
```

## GetIdMappingTableInputTypeDef

```python
# GetIdMappingTableInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetIdMappingTableInputTypeDef


def get_value() -> GetIdMappingTableInputTypeDef:
    return {
        "idMappingTableIdentifier": ...,
    }


# GetIdMappingTableInputTypeDef definition

class GetIdMappingTableInputTypeDef(TypedDict):
    idMappingTableIdentifier: str,
    membershipIdentifier: str,
```

## GetIdNamespaceAssociationInputTypeDef

```python
# GetIdNamespaceAssociationInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetIdNamespaceAssociationInputTypeDef


def get_value() -> GetIdNamespaceAssociationInputTypeDef:
    return {
        "idNamespaceAssociationIdentifier": ...,
    }


# GetIdNamespaceAssociationInputTypeDef definition

class GetIdNamespaceAssociationInputTypeDef(TypedDict):
    idNamespaceAssociationIdentifier: str,
    membershipIdentifier: str,
```

## GetMembershipInputTypeDef

```python
# GetMembershipInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetMembershipInputTypeDef


def get_value() -> GetMembershipInputTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# GetMembershipInputTypeDef definition

class GetMembershipInputTypeDef(TypedDict):
    membershipIdentifier: str,
```

## GetPrivacyBudgetTemplateInputTypeDef

```python
# GetPrivacyBudgetTemplateInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetPrivacyBudgetTemplateInputTypeDef


def get_value() -> GetPrivacyBudgetTemplateInputTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# GetPrivacyBudgetTemplateInputTypeDef definition

class GetPrivacyBudgetTemplateInputTypeDef(TypedDict):
    membershipIdentifier: str,
    privacyBudgetTemplateIdentifier: str,
```

## GetProtectedQueryInputTypeDef

```python
# GetProtectedQueryInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetProtectedQueryInputTypeDef


def get_value() -> GetProtectedQueryInputTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# GetProtectedQueryInputTypeDef definition

class GetProtectedQueryInputTypeDef(TypedDict):
    membershipIdentifier: str,
    protectedQueryIdentifier: str,
```

## GetSchemaAnalysisRuleInputTypeDef

```python
# GetSchemaAnalysisRuleInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetSchemaAnalysisRuleInputTypeDef


def get_value() -> GetSchemaAnalysisRuleInputTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# GetSchemaAnalysisRuleInputTypeDef definition

class GetSchemaAnalysisRuleInputTypeDef(TypedDict):
    collaborationIdentifier: str,
    name: str,
    type: AnalysisRuleTypeType,  # (1)
```

1. See [:material-code-brackets: AnalysisRuleTypeType](./literals.md#analysisruletypetype) 
## GetSchemaInputTypeDef

```python
# GetSchemaInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetSchemaInputTypeDef


def get_value() -> GetSchemaInputTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# GetSchemaInputTypeDef definition

class GetSchemaInputTypeDef(TypedDict):
    collaborationIdentifier: str,
    name: str,
```

## GlueTableReferenceTypeDef

```python
# GlueTableReferenceTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GlueTableReferenceTypeDef


def get_value() -> GlueTableReferenceTypeDef:
    return {
        "tableName": ...,
    }


# GlueTableReferenceTypeDef definition

class GlueTableReferenceTypeDef(TypedDict):
    tableName: str,
    databaseName: str,
```

## IdMappingTableInputSourceTypeDef

```python
# IdMappingTableInputSourceTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import IdMappingTableInputSourceTypeDef


def get_value() -> IdMappingTableInputSourceTypeDef:
    return {
        "idNamespaceAssociationId": ...,
    }


# IdMappingTableInputSourceTypeDef definition

class IdMappingTableInputSourceTypeDef(TypedDict):
    idNamespaceAssociationId: str,
    type: IdNamespaceTypeType,  # (1)
```

1. See [:material-code-brackets: IdNamespaceTypeType](./literals.md#idnamespacetypetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import PaginatorConfigTypeDef


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

## ListAnalysisTemplatesInputTypeDef

```python
# ListAnalysisTemplatesInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListAnalysisTemplatesInputTypeDef


def get_value() -> ListAnalysisTemplatesInputTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# ListAnalysisTemplatesInputTypeDef definition

class ListAnalysisTemplatesInputTypeDef(TypedDict):
    membershipIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListCollaborationAnalysisTemplatesInputTypeDef

```python
# ListCollaborationAnalysisTemplatesInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListCollaborationAnalysisTemplatesInputTypeDef


def get_value() -> ListCollaborationAnalysisTemplatesInputTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# ListCollaborationAnalysisTemplatesInputTypeDef definition

class ListCollaborationAnalysisTemplatesInputTypeDef(TypedDict):
    collaborationIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListCollaborationConfiguredAudienceModelAssociationsInputTypeDef

```python
# ListCollaborationConfiguredAudienceModelAssociationsInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListCollaborationConfiguredAudienceModelAssociationsInputTypeDef


def get_value() -> ListCollaborationConfiguredAudienceModelAssociationsInputTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# ListCollaborationConfiguredAudienceModelAssociationsInputTypeDef definition

class ListCollaborationConfiguredAudienceModelAssociationsInputTypeDef(TypedDict):
    collaborationIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListCollaborationIdNamespaceAssociationsInputTypeDef

```python
# ListCollaborationIdNamespaceAssociationsInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListCollaborationIdNamespaceAssociationsInputTypeDef


def get_value() -> ListCollaborationIdNamespaceAssociationsInputTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# ListCollaborationIdNamespaceAssociationsInputTypeDef definition

class ListCollaborationIdNamespaceAssociationsInputTypeDef(TypedDict):
    collaborationIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListCollaborationPrivacyBudgetTemplatesInputTypeDef

```python
# ListCollaborationPrivacyBudgetTemplatesInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListCollaborationPrivacyBudgetTemplatesInputTypeDef


def get_value() -> ListCollaborationPrivacyBudgetTemplatesInputTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# ListCollaborationPrivacyBudgetTemplatesInputTypeDef definition

class ListCollaborationPrivacyBudgetTemplatesInputTypeDef(TypedDict):
    collaborationIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListCollaborationPrivacyBudgetsInputTypeDef

```python
# ListCollaborationPrivacyBudgetsInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListCollaborationPrivacyBudgetsInputTypeDef


def get_value() -> ListCollaborationPrivacyBudgetsInputTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# ListCollaborationPrivacyBudgetsInputTypeDef definition

class ListCollaborationPrivacyBudgetsInputTypeDef(TypedDict):
    collaborationIdentifier: str,
    privacyBudgetType: PrivacyBudgetTypeType,  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: PrivacyBudgetTypeType](./literals.md#privacybudgettypetype) 
## ListCollaborationsInputTypeDef

```python
# ListCollaborationsInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListCollaborationsInputTypeDef


def get_value() -> ListCollaborationsInputTypeDef:
    return {
        "nextToken": ...,
    }


# ListCollaborationsInputTypeDef definition

class ListCollaborationsInputTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    memberStatus: NotRequired[FilterableMemberStatusType],  # (1)
```

1. See [:material-code-brackets: FilterableMemberStatusType](./literals.md#filterablememberstatustype) 
## ListConfiguredAudienceModelAssociationsInputTypeDef

```python
# ListConfiguredAudienceModelAssociationsInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListConfiguredAudienceModelAssociationsInputTypeDef


def get_value() -> ListConfiguredAudienceModelAssociationsInputTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# ListConfiguredAudienceModelAssociationsInputTypeDef definition

class ListConfiguredAudienceModelAssociationsInputTypeDef(TypedDict):
    membershipIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListConfiguredTableAssociationsInputTypeDef

```python
# ListConfiguredTableAssociationsInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListConfiguredTableAssociationsInputTypeDef


def get_value() -> ListConfiguredTableAssociationsInputTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# ListConfiguredTableAssociationsInputTypeDef definition

class ListConfiguredTableAssociationsInputTypeDef(TypedDict):
    membershipIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListConfiguredTablesInputTypeDef

```python
# ListConfiguredTablesInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListConfiguredTablesInputTypeDef


def get_value() -> ListConfiguredTablesInputTypeDef:
    return {
        "nextToken": ...,
    }


# ListConfiguredTablesInputTypeDef definition

class ListConfiguredTablesInputTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListIdMappingTablesInputTypeDef

```python
# ListIdMappingTablesInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListIdMappingTablesInputTypeDef


def get_value() -> ListIdMappingTablesInputTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# ListIdMappingTablesInputTypeDef definition

class ListIdMappingTablesInputTypeDef(TypedDict):
    membershipIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListIdNamespaceAssociationsInputTypeDef

```python
# ListIdNamespaceAssociationsInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListIdNamespaceAssociationsInputTypeDef


def get_value() -> ListIdNamespaceAssociationsInputTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# ListIdNamespaceAssociationsInputTypeDef definition

class ListIdNamespaceAssociationsInputTypeDef(TypedDict):
    membershipIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListMembersInputTypeDef

```python
# ListMembersInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListMembersInputTypeDef


def get_value() -> ListMembersInputTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# ListMembersInputTypeDef definition

class ListMembersInputTypeDef(TypedDict):
    collaborationIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListMembershipsInputTypeDef

```python
# ListMembershipsInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListMembershipsInputTypeDef


def get_value() -> ListMembershipsInputTypeDef:
    return {
        "nextToken": ...,
    }


# ListMembershipsInputTypeDef definition

class ListMembershipsInputTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    status: NotRequired[MembershipStatusType],  # (1)
```

1. See [:material-code-brackets: MembershipStatusType](./literals.md#membershipstatustype) 
## ListPrivacyBudgetTemplatesInputTypeDef

```python
# ListPrivacyBudgetTemplatesInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListPrivacyBudgetTemplatesInputTypeDef


def get_value() -> ListPrivacyBudgetTemplatesInputTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# ListPrivacyBudgetTemplatesInputTypeDef definition

class ListPrivacyBudgetTemplatesInputTypeDef(TypedDict):
    membershipIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## PrivacyBudgetTemplateSummaryTypeDef

```python
# PrivacyBudgetTemplateSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import PrivacyBudgetTemplateSummaryTypeDef


def get_value() -> PrivacyBudgetTemplateSummaryTypeDef:
    return {
        "id": ...,
    }


# PrivacyBudgetTemplateSummaryTypeDef definition

class PrivacyBudgetTemplateSummaryTypeDef(TypedDict):
    id: str,
    arn: str,
    membershipId: str,
    membershipArn: str,
    collaborationId: str,
    collaborationArn: str,
    privacyBudgetType: PrivacyBudgetTypeType,  # (1)
    createTime: datetime,
    updateTime: datetime,
```

1. See [:material-code-brackets: PrivacyBudgetTypeType](./literals.md#privacybudgettypetype) 
## ListPrivacyBudgetsInputTypeDef

```python
# ListPrivacyBudgetsInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListPrivacyBudgetsInputTypeDef


def get_value() -> ListPrivacyBudgetsInputTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# ListPrivacyBudgetsInputTypeDef definition

class ListPrivacyBudgetsInputTypeDef(TypedDict):
    membershipIdentifier: str,
    privacyBudgetType: PrivacyBudgetTypeType,  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: PrivacyBudgetTypeType](./literals.md#privacybudgettypetype) 
## ListProtectedQueriesInputTypeDef

```python
# ListProtectedQueriesInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListProtectedQueriesInputTypeDef


def get_value() -> ListProtectedQueriesInputTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# ListProtectedQueriesInputTypeDef definition

class ListProtectedQueriesInputTypeDef(TypedDict):
    membershipIdentifier: str,
    status: NotRequired[ProtectedQueryStatusType],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: ProtectedQueryStatusType](./literals.md#protectedquerystatustype) 
## ListSchemasInputTypeDef

```python
# ListSchemasInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListSchemasInputTypeDef


def get_value() -> ListSchemasInputTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# ListSchemasInputTypeDef definition

class ListSchemasInputTypeDef(TypedDict):
    collaborationIdentifier: str,
    schemaType: NotRequired[SchemaTypeType],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: SchemaTypeType](./literals.md#schematypetype) 
## SchemaSummaryTypeDef

```python
# SchemaSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import SchemaSummaryTypeDef


def get_value() -> SchemaSummaryTypeDef:
    return {
        "name": ...,
    }


# SchemaSummaryTypeDef definition

class SchemaSummaryTypeDef(TypedDict):
    name: str,
    type: SchemaTypeType,  # (1)
    creatorAccountId: str,
    createTime: datetime,
    updateTime: datetime,
    collaborationId: str,
    collaborationArn: str,
    analysisRuleTypes: List[AnalysisRuleTypeType],  # (2)
    analysisMethod: NotRequired[AnalysisMethodType],  # (3)
```

1. See [:material-code-brackets: SchemaTypeType](./literals.md#schematypetype) 
2. See [:material-code-brackets: AnalysisRuleTypeType](./literals.md#analysisruletypetype) 
3. See [:material-code-brackets: AnalysisMethodType](./literals.md#analysismethodtype) 
## ListTagsForResourceInputTypeDef

```python
# ListTagsForResourceInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListTagsForResourceInputTypeDef


def get_value() -> ListTagsForResourceInputTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceInputTypeDef definition

class ListTagsForResourceInputTypeDef(TypedDict):
    resourceArn: str,
```

## MLMemberAbilitiesOutputTypeDef

```python
# MLMemberAbilitiesOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import MLMemberAbilitiesOutputTypeDef


def get_value() -> MLMemberAbilitiesOutputTypeDef:
    return {
        "customMLMemberAbilities": ...,
    }


# MLMemberAbilitiesOutputTypeDef definition

class MLMemberAbilitiesOutputTypeDef(TypedDict):
    customMLMemberAbilities: List[CustomMLMemberAbilityType],  # (1)
```

1. See [:material-code-brackets: CustomMLMemberAbilityType](./literals.md#custommlmemberabilitytype) 
## MLMemberAbilitiesTypeDef

```python
# MLMemberAbilitiesTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import MLMemberAbilitiesTypeDef


def get_value() -> MLMemberAbilitiesTypeDef:
    return {
        "customMLMemberAbilities": ...,
    }


# MLMemberAbilitiesTypeDef definition

class MLMemberAbilitiesTypeDef(TypedDict):
    customMLMemberAbilities: Sequence[CustomMLMemberAbilityType],  # (1)
```

1. See [:material-code-brackets: CustomMLMemberAbilityType](./literals.md#custommlmemberabilitytype) 
## ModelInferencePaymentConfigTypeDef

```python
# ModelInferencePaymentConfigTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ModelInferencePaymentConfigTypeDef


def get_value() -> ModelInferencePaymentConfigTypeDef:
    return {
        "isResponsible": ...,
    }


# ModelInferencePaymentConfigTypeDef definition

class ModelInferencePaymentConfigTypeDef(TypedDict):
    isResponsible: bool,
```

## ModelTrainingPaymentConfigTypeDef

```python
# ModelTrainingPaymentConfigTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ModelTrainingPaymentConfigTypeDef


def get_value() -> ModelTrainingPaymentConfigTypeDef:
    return {
        "isResponsible": ...,
    }


# ModelTrainingPaymentConfigTypeDef definition

class ModelTrainingPaymentConfigTypeDef(TypedDict):
    isResponsible: bool,
```

## MembershipModelInferencePaymentConfigTypeDef

```python
# MembershipModelInferencePaymentConfigTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import MembershipModelInferencePaymentConfigTypeDef


def get_value() -> MembershipModelInferencePaymentConfigTypeDef:
    return {
        "isResponsible": ...,
    }


# MembershipModelInferencePaymentConfigTypeDef definition

class MembershipModelInferencePaymentConfigTypeDef(TypedDict):
    isResponsible: bool,
```

## MembershipModelTrainingPaymentConfigTypeDef

```python
# MembershipModelTrainingPaymentConfigTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import MembershipModelTrainingPaymentConfigTypeDef


def get_value() -> MembershipModelTrainingPaymentConfigTypeDef:
    return {
        "isResponsible": ...,
    }


# MembershipModelTrainingPaymentConfigTypeDef definition

class MembershipModelTrainingPaymentConfigTypeDef(TypedDict):
    isResponsible: bool,
```

## MembershipQueryComputePaymentConfigTypeDef

```python
# MembershipQueryComputePaymentConfigTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import MembershipQueryComputePaymentConfigTypeDef


def get_value() -> MembershipQueryComputePaymentConfigTypeDef:
    return {
        "isResponsible": ...,
    }


# MembershipQueryComputePaymentConfigTypeDef definition

class MembershipQueryComputePaymentConfigTypeDef(TypedDict):
    isResponsible: bool,
```

## ProtectedQueryS3OutputConfigurationTypeDef

```python
# ProtectedQueryS3OutputConfigurationTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ProtectedQueryS3OutputConfigurationTypeDef


def get_value() -> ProtectedQueryS3OutputConfigurationTypeDef:
    return {
        "resultFormat": ...,
    }


# ProtectedQueryS3OutputConfigurationTypeDef definition

class ProtectedQueryS3OutputConfigurationTypeDef(TypedDict):
    resultFormat: ResultFormatType,  # (1)
    bucket: str,
    keyPrefix: NotRequired[str],
    singleFileOutput: NotRequired[bool],
```

1. See [:material-code-brackets: ResultFormatType](./literals.md#resultformattype) 
## QueryComputePaymentConfigTypeDef

```python
# QueryComputePaymentConfigTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import QueryComputePaymentConfigTypeDef


def get_value() -> QueryComputePaymentConfigTypeDef:
    return {
        "isResponsible": ...,
    }


# QueryComputePaymentConfigTypeDef definition

class QueryComputePaymentConfigTypeDef(TypedDict):
    isResponsible: bool,
```

## PopulateIdMappingTableInputTypeDef

```python
# PopulateIdMappingTableInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import PopulateIdMappingTableInputTypeDef


def get_value() -> PopulateIdMappingTableInputTypeDef:
    return {
        "idMappingTableIdentifier": ...,
    }


# PopulateIdMappingTableInputTypeDef definition

class PopulateIdMappingTableInputTypeDef(TypedDict):
    idMappingTableIdentifier: str,
    membershipIdentifier: str,
```

## ProtectedQueryErrorTypeDef

```python
# ProtectedQueryErrorTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ProtectedQueryErrorTypeDef


def get_value() -> ProtectedQueryErrorTypeDef:
    return {
        "message": ...,
    }


# ProtectedQueryErrorTypeDef definition

class ProtectedQueryErrorTypeDef(TypedDict):
    message: str,
    code: str,
```

## ProtectedQueryMemberOutputConfigurationTypeDef

```python
# ProtectedQueryMemberOutputConfigurationTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ProtectedQueryMemberOutputConfigurationTypeDef


def get_value() -> ProtectedQueryMemberOutputConfigurationTypeDef:
    return {
        "accountId": ...,
    }


# ProtectedQueryMemberOutputConfigurationTypeDef definition

class ProtectedQueryMemberOutputConfigurationTypeDef(TypedDict):
    accountId: str,
```

## ProtectedQueryS3OutputTypeDef

```python
# ProtectedQueryS3OutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ProtectedQueryS3OutputTypeDef


def get_value() -> ProtectedQueryS3OutputTypeDef:
    return {
        "location": ...,
    }


# ProtectedQueryS3OutputTypeDef definition

class ProtectedQueryS3OutputTypeDef(TypedDict):
    location: str,
```

## ProtectedQuerySingleMemberOutputTypeDef

```python
# ProtectedQuerySingleMemberOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ProtectedQuerySingleMemberOutputTypeDef


def get_value() -> ProtectedQuerySingleMemberOutputTypeDef:
    return {
        "accountId": ...,
    }


# ProtectedQuerySingleMemberOutputTypeDef definition

class ProtectedQuerySingleMemberOutputTypeDef(TypedDict):
    accountId: str,
```

## ProtectedQuerySQLParametersOutputTypeDef

```python
# ProtectedQuerySQLParametersOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ProtectedQuerySQLParametersOutputTypeDef


def get_value() -> ProtectedQuerySQLParametersOutputTypeDef:
    return {
        "queryString": ...,
    }


# ProtectedQuerySQLParametersOutputTypeDef definition

class ProtectedQuerySQLParametersOutputTypeDef(TypedDict):
    queryString: NotRequired[str],
    analysisTemplateArn: NotRequired[str],
    parameters: NotRequired[Dict[str, str]],
```

## ProtectedQuerySQLParametersTypeDef

```python
# ProtectedQuerySQLParametersTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ProtectedQuerySQLParametersTypeDef


def get_value() -> ProtectedQuerySQLParametersTypeDef:
    return {
        "queryString": ...,
    }


# ProtectedQuerySQLParametersTypeDef definition

class ProtectedQuerySQLParametersTypeDef(TypedDict):
    queryString: NotRequired[str],
    analysisTemplateArn: NotRequired[str],
    parameters: NotRequired[Mapping[str, str]],
```

## QueryConstraintRequireOverlapTypeDef

```python
# QueryConstraintRequireOverlapTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import QueryConstraintRequireOverlapTypeDef


def get_value() -> QueryConstraintRequireOverlapTypeDef:
    return {
        "columns": ...,
    }


# QueryConstraintRequireOverlapTypeDef definition

class QueryConstraintRequireOverlapTypeDef(TypedDict):
    columns: NotRequired[List[str]],
```

## SchemaStatusReasonTypeDef

```python
# SchemaStatusReasonTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import SchemaStatusReasonTypeDef


def get_value() -> SchemaStatusReasonTypeDef:
    return {
        "code": ...,
    }


# SchemaStatusReasonTypeDef definition

class SchemaStatusReasonTypeDef(TypedDict):
    code: SchemaStatusReasonCodeType,  # (1)
    message: str,
```

1. See [:material-code-brackets: SchemaStatusReasonCodeType](./literals.md#schemastatusreasoncodetype) 
## SnowflakeTableSchemaV1TypeDef

```python
# SnowflakeTableSchemaV1TypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import SnowflakeTableSchemaV1TypeDef


def get_value() -> SnowflakeTableSchemaV1TypeDef:
    return {
        "columnName": ...,
    }


# SnowflakeTableSchemaV1TypeDef definition

class SnowflakeTableSchemaV1TypeDef(TypedDict):
    columnName: str,
    columnType: str,
```

## TagResourceInputTypeDef

```python
# TagResourceInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import TagResourceInputTypeDef


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

from types_aiobotocore_cleanrooms.type_defs import UntagResourceInputTypeDef


def get_value() -> UntagResourceInputTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceInputTypeDef definition

class UntagResourceInputTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateAnalysisTemplateInputTypeDef

```python
# UpdateAnalysisTemplateInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import UpdateAnalysisTemplateInputTypeDef


def get_value() -> UpdateAnalysisTemplateInputTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# UpdateAnalysisTemplateInputTypeDef definition

class UpdateAnalysisTemplateInputTypeDef(TypedDict):
    membershipIdentifier: str,
    analysisTemplateIdentifier: str,
    description: NotRequired[str],
```

## UpdateCollaborationInputTypeDef

```python
# UpdateCollaborationInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import UpdateCollaborationInputTypeDef


def get_value() -> UpdateCollaborationInputTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# UpdateCollaborationInputTypeDef definition

class UpdateCollaborationInputTypeDef(TypedDict):
    collaborationIdentifier: str,
    name: NotRequired[str],
    description: NotRequired[str],
```

## UpdateConfiguredAudienceModelAssociationInputTypeDef

```python
# UpdateConfiguredAudienceModelAssociationInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import UpdateConfiguredAudienceModelAssociationInputTypeDef


def get_value() -> UpdateConfiguredAudienceModelAssociationInputTypeDef:
    return {
        "configuredAudienceModelAssociationIdentifier": ...,
    }


# UpdateConfiguredAudienceModelAssociationInputTypeDef definition

class UpdateConfiguredAudienceModelAssociationInputTypeDef(TypedDict):
    configuredAudienceModelAssociationIdentifier: str,
    membershipIdentifier: str,
    description: NotRequired[str],
    name: NotRequired[str],
```

## UpdateConfiguredTableAssociationInputTypeDef

```python
# UpdateConfiguredTableAssociationInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import UpdateConfiguredTableAssociationInputTypeDef


def get_value() -> UpdateConfiguredTableAssociationInputTypeDef:
    return {
        "configuredTableAssociationIdentifier": ...,
    }


# UpdateConfiguredTableAssociationInputTypeDef definition

class UpdateConfiguredTableAssociationInputTypeDef(TypedDict):
    configuredTableAssociationIdentifier: str,
    membershipIdentifier: str,
    description: NotRequired[str],
    roleArn: NotRequired[str],
```

## UpdateConfiguredTableInputTypeDef

```python
# UpdateConfiguredTableInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import UpdateConfiguredTableInputTypeDef


def get_value() -> UpdateConfiguredTableInputTypeDef:
    return {
        "configuredTableIdentifier": ...,
    }


# UpdateConfiguredTableInputTypeDef definition

class UpdateConfiguredTableInputTypeDef(TypedDict):
    configuredTableIdentifier: str,
    name: NotRequired[str],
    description: NotRequired[str],
```

## UpdateIdMappingTableInputTypeDef

```python
# UpdateIdMappingTableInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import UpdateIdMappingTableInputTypeDef


def get_value() -> UpdateIdMappingTableInputTypeDef:
    return {
        "idMappingTableIdentifier": ...,
    }


# UpdateIdMappingTableInputTypeDef definition

class UpdateIdMappingTableInputTypeDef(TypedDict):
    idMappingTableIdentifier: str,
    membershipIdentifier: str,
    description: NotRequired[str],
    kmsKeyArn: NotRequired[str],
```

## UpdateProtectedQueryInputTypeDef

```python
# UpdateProtectedQueryInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import UpdateProtectedQueryInputTypeDef


def get_value() -> UpdateProtectedQueryInputTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# UpdateProtectedQueryInputTypeDef definition

class UpdateProtectedQueryInputTypeDef(TypedDict):
    membershipIdentifier: str,
    protectedQueryIdentifier: str,
    targetStatus: TargetProtectedQueryStatusType,  # (1)
```

1. See [:material-code-brackets: TargetProtectedQueryStatusType](./literals.md#targetprotectedquerystatustype) 
## AnalysisRuleAggregationOutputTypeDef

```python
# AnalysisRuleAggregationOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import AnalysisRuleAggregationOutputTypeDef


def get_value() -> AnalysisRuleAggregationOutputTypeDef:
    return {
        "aggregateColumns": ...,
    }


# AnalysisRuleAggregationOutputTypeDef definition

class AnalysisRuleAggregationOutputTypeDef(TypedDict):
    aggregateColumns: List[AggregateColumnOutputTypeDef],  # (1)
    joinColumns: List[str],
    dimensionColumns: List[str],
    scalarFunctions: List[ScalarFunctionsType],  # (4)
    outputConstraints: List[AggregationConstraintTypeDef],  # (5)
    joinRequired: NotRequired[JoinRequiredOptionType],  # (2)
    allowedJoinOperators: NotRequired[List[JoinOperatorType]],  # (3)
    additionalAnalyses: NotRequired[AdditionalAnalysesType],  # (6)
```

1. See [:material-code-braces: AggregateColumnOutputTypeDef](./type_defs.md#aggregatecolumnoutputtypedef) 
2. See [:material-code-brackets: JoinRequiredOptionType](./literals.md#joinrequiredoptiontype) 
3. See [:material-code-brackets: JoinOperatorType](./literals.md#joinoperatortype) 
4. See [:material-code-brackets: ScalarFunctionsType](./literals.md#scalarfunctionstype) 
5. See [:material-code-braces: AggregationConstraintTypeDef](./type_defs.md#aggregationconstrainttypedef) 
6. See [:material-code-brackets: AdditionalAnalysesType](./literals.md#additionalanalysestype) 
## AnalysisRuleAggregationTypeDef

```python
# AnalysisRuleAggregationTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import AnalysisRuleAggregationTypeDef


def get_value() -> AnalysisRuleAggregationTypeDef:
    return {
        "aggregateColumns": ...,
    }


# AnalysisRuleAggregationTypeDef definition

class AnalysisRuleAggregationTypeDef(TypedDict):
    aggregateColumns: Sequence[AggregateColumnTypeDef],  # (1)
    joinColumns: Sequence[str],
    dimensionColumns: Sequence[str],
    scalarFunctions: Sequence[ScalarFunctionsType],  # (4)
    outputConstraints: Sequence[AggregationConstraintTypeDef],  # (5)
    joinRequired: NotRequired[JoinRequiredOptionType],  # (2)
    allowedJoinOperators: NotRequired[Sequence[JoinOperatorType]],  # (3)
    additionalAnalyses: NotRequired[AdditionalAnalysesType],  # (6)
```

1. See [:material-code-braces: AggregateColumnTypeDef](./type_defs.md#aggregatecolumntypedef) 
2. See [:material-code-brackets: JoinRequiredOptionType](./literals.md#joinrequiredoptiontype) 
3. See [:material-code-brackets: JoinOperatorType](./literals.md#joinoperatortype) 
4. See [:material-code-brackets: ScalarFunctionsType](./literals.md#scalarfunctionstype) 
5. See [:material-code-braces: AggregationConstraintTypeDef](./type_defs.md#aggregationconstrainttypedef) 
6. See [:material-code-brackets: AdditionalAnalysesType](./literals.md#additionalanalysestype) 
## CreateAnalysisTemplateInputTypeDef

```python
# CreateAnalysisTemplateInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CreateAnalysisTemplateInputTypeDef


def get_value() -> CreateAnalysisTemplateInputTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# CreateAnalysisTemplateInputTypeDef definition

class CreateAnalysisTemplateInputTypeDef(TypedDict):
    membershipIdentifier: str,
    name: str,
    format: AnalysisFormatType,  # (1)
    source: AnalysisSourceTypeDef,  # (2)
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    analysisParameters: NotRequired[Sequence[AnalysisParameterTypeDef]],  # (3)
```

1. See [:material-code-brackets: AnalysisFormatType](./literals.md#analysisformattype) 
2. See [:material-code-braces: AnalysisSourceTypeDef](./type_defs.md#analysissourcetypedef) 
3. See [:material-code-braces: AnalysisParameterTypeDef](./type_defs.md#analysisparametertypedef) 
## AnalysisTemplateValidationStatusDetailTypeDef

```python
# AnalysisTemplateValidationStatusDetailTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import AnalysisTemplateValidationStatusDetailTypeDef


def get_value() -> AnalysisTemplateValidationStatusDetailTypeDef:
    return {
        "type": ...,
    }


# AnalysisTemplateValidationStatusDetailTypeDef definition

class AnalysisTemplateValidationStatusDetailTypeDef(TypedDict):
    type: AnalysisTemplateValidationTypeType,  # (1)
    status: AnalysisTemplateValidationStatusType,  # (2)
    reasons: NotRequired[List[AnalysisTemplateValidationStatusReasonTypeDef]],  # (3)
```

1. See [:material-code-brackets: AnalysisTemplateValidationTypeType](./literals.md#analysistemplatevalidationtypetype) 
2. See [:material-code-brackets: AnalysisTemplateValidationStatusType](./literals.md#analysistemplatevalidationstatustype) 
3. See [:material-code-braces: AnalysisTemplateValidationStatusReasonTypeDef](./type_defs.md#analysistemplatevalidationstatusreasontypedef) 
## ListAnalysisTemplatesOutputTypeDef

```python
# ListAnalysisTemplatesOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListAnalysisTemplatesOutputTypeDef


def get_value() -> ListAnalysisTemplatesOutputTypeDef:
    return {
        "nextToken": ...,
    }


# ListAnalysisTemplatesOutputTypeDef definition

class ListAnalysisTemplatesOutputTypeDef(TypedDict):
    analysisTemplateSummaries: List[AnalysisTemplateSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AnalysisTemplateSummaryTypeDef](./type_defs.md#analysistemplatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListTagsForResourceOutputTypeDef


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
## PopulateIdMappingTableOutputTypeDef

```python
# PopulateIdMappingTableOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import PopulateIdMappingTableOutputTypeDef


def get_value() -> PopulateIdMappingTableOutputTypeDef:
    return {
        "idMappingJobId": ...,
    }


# PopulateIdMappingTableOutputTypeDef definition

class PopulateIdMappingTableOutputTypeDef(TypedDict):
    idMappingJobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetSchemaAnalysisRuleInputTypeDef

```python
# BatchGetSchemaAnalysisRuleInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import BatchGetSchemaAnalysisRuleInputTypeDef


def get_value() -> BatchGetSchemaAnalysisRuleInputTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# BatchGetSchemaAnalysisRuleInputTypeDef definition

class BatchGetSchemaAnalysisRuleInputTypeDef(TypedDict):
    collaborationIdentifier: str,
    schemaAnalysisRuleRequests: Sequence[SchemaAnalysisRuleRequestTypeDef],  # (1)
```

1. See [:material-code-braces: SchemaAnalysisRuleRequestTypeDef](./type_defs.md#schemaanalysisrulerequesttypedef) 
## ProtectedQueryStatisticsTypeDef

```python
# ProtectedQueryStatisticsTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ProtectedQueryStatisticsTypeDef


def get_value() -> ProtectedQueryStatisticsTypeDef:
    return {
        "totalDurationInMillis": ...,
    }


# ProtectedQueryStatisticsTypeDef definition

class ProtectedQueryStatisticsTypeDef(TypedDict):
    totalDurationInMillis: NotRequired[int],
    billedResourceUtilization: NotRequired[BilledResourceUtilizationTypeDef],  # (1)
```

1. See [:material-code-braces: BilledResourceUtilizationTypeDef](./type_defs.md#billedresourceutilizationtypedef) 
## ListCollaborationAnalysisTemplatesOutputTypeDef

```python
# ListCollaborationAnalysisTemplatesOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListCollaborationAnalysisTemplatesOutputTypeDef


def get_value() -> ListCollaborationAnalysisTemplatesOutputTypeDef:
    return {
        "nextToken": ...,
    }


# ListCollaborationAnalysisTemplatesOutputTypeDef definition

class ListCollaborationAnalysisTemplatesOutputTypeDef(TypedDict):
    collaborationAnalysisTemplateSummaries: List[CollaborationAnalysisTemplateSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CollaborationAnalysisTemplateSummaryTypeDef](./type_defs.md#collaborationanalysistemplatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCollaborationConfiguredAudienceModelAssociationsOutputTypeDef

```python
# ListCollaborationConfiguredAudienceModelAssociationsOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListCollaborationConfiguredAudienceModelAssociationsOutputTypeDef


def get_value() -> ListCollaborationConfiguredAudienceModelAssociationsOutputTypeDef:
    return {
        "collaborationConfiguredAudienceModelAssociationSummaries": ...,
    }


# ListCollaborationConfiguredAudienceModelAssociationsOutputTypeDef definition

class ListCollaborationConfiguredAudienceModelAssociationsOutputTypeDef(TypedDict):
    collaborationConfiguredAudienceModelAssociationSummaries: List[CollaborationConfiguredAudienceModelAssociationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CollaborationConfiguredAudienceModelAssociationSummaryTypeDef](./type_defs.md#collaborationconfiguredaudiencemodelassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCollaborationConfiguredAudienceModelAssociationOutputTypeDef

```python
# GetCollaborationConfiguredAudienceModelAssociationOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetCollaborationConfiguredAudienceModelAssociationOutputTypeDef


def get_value() -> GetCollaborationConfiguredAudienceModelAssociationOutputTypeDef:
    return {
        "collaborationConfiguredAudienceModelAssociation": ...,
    }


# GetCollaborationConfiguredAudienceModelAssociationOutputTypeDef definition

class GetCollaborationConfiguredAudienceModelAssociationOutputTypeDef(TypedDict):
    collaborationConfiguredAudienceModelAssociation: CollaborationConfiguredAudienceModelAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CollaborationConfiguredAudienceModelAssociationTypeDef](./type_defs.md#collaborationconfiguredaudiencemodelassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CollaborationIdNamespaceAssociationSummaryTypeDef

```python
# CollaborationIdNamespaceAssociationSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CollaborationIdNamespaceAssociationSummaryTypeDef


def get_value() -> CollaborationIdNamespaceAssociationSummaryTypeDef:
    return {
        "arn": ...,
    }


# CollaborationIdNamespaceAssociationSummaryTypeDef definition

class CollaborationIdNamespaceAssociationSummaryTypeDef(TypedDict):
    arn: str,
    createTime: datetime,
    id: str,
    updateTime: datetime,
    collaborationArn: str,
    collaborationId: str,
    creatorAccountId: str,
    inputReferenceConfig: IdNamespaceAssociationInputReferenceConfigTypeDef,  # (1)
    name: str,
    inputReferenceProperties: IdNamespaceAssociationInputReferencePropertiesSummaryTypeDef,  # (2)
    description: NotRequired[str],
```

1. See [:material-code-braces: IdNamespaceAssociationInputReferenceConfigTypeDef](./type_defs.md#idnamespaceassociationinputreferenceconfigtypedef) 
2. See [:material-code-braces: IdNamespaceAssociationInputReferencePropertiesSummaryTypeDef](./type_defs.md#idnamespaceassociationinputreferencepropertiessummarytypedef) 
## IdNamespaceAssociationSummaryTypeDef

```python
# IdNamespaceAssociationSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import IdNamespaceAssociationSummaryTypeDef


def get_value() -> IdNamespaceAssociationSummaryTypeDef:
    return {
        "membershipId": ...,
    }


# IdNamespaceAssociationSummaryTypeDef definition

class IdNamespaceAssociationSummaryTypeDef(TypedDict):
    membershipId: str,
    membershipArn: str,
    collaborationArn: str,
    collaborationId: str,
    createTime: datetime,
    updateTime: datetime,
    id: str,
    arn: str,
    inputReferenceConfig: IdNamespaceAssociationInputReferenceConfigTypeDef,  # (1)
    name: str,
    inputReferenceProperties: IdNamespaceAssociationInputReferencePropertiesSummaryTypeDef,  # (2)
    description: NotRequired[str],
```

1. See [:material-code-braces: IdNamespaceAssociationInputReferenceConfigTypeDef](./type_defs.md#idnamespaceassociationinputreferenceconfigtypedef) 
2. See [:material-code-braces: IdNamespaceAssociationInputReferencePropertiesSummaryTypeDef](./type_defs.md#idnamespaceassociationinputreferencepropertiessummarytypedef) 
## CreateIdNamespaceAssociationInputTypeDef

```python
# CreateIdNamespaceAssociationInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CreateIdNamespaceAssociationInputTypeDef


def get_value() -> CreateIdNamespaceAssociationInputTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# CreateIdNamespaceAssociationInputTypeDef definition

class CreateIdNamespaceAssociationInputTypeDef(TypedDict):
    membershipIdentifier: str,
    inputReferenceConfig: IdNamespaceAssociationInputReferenceConfigTypeDef,  # (1)
    name: str,
    tags: NotRequired[Mapping[str, str]],
    description: NotRequired[str],
    idMappingConfig: NotRequired[IdMappingConfigTypeDef],  # (2)
```

1. See [:material-code-braces: IdNamespaceAssociationInputReferenceConfigTypeDef](./type_defs.md#idnamespaceassociationinputreferenceconfigtypedef) 
2. See [:material-code-braces: IdMappingConfigTypeDef](./type_defs.md#idmappingconfigtypedef) 
## UpdateIdNamespaceAssociationInputTypeDef

```python
# UpdateIdNamespaceAssociationInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import UpdateIdNamespaceAssociationInputTypeDef


def get_value() -> UpdateIdNamespaceAssociationInputTypeDef:
    return {
        "idNamespaceAssociationIdentifier": ...,
    }


# UpdateIdNamespaceAssociationInputTypeDef definition

class UpdateIdNamespaceAssociationInputTypeDef(TypedDict):
    idNamespaceAssociationIdentifier: str,
    membershipIdentifier: str,
    name: NotRequired[str],
    description: NotRequired[str],
    idMappingConfig: NotRequired[IdMappingConfigTypeDef],  # (1)
```

1. See [:material-code-braces: IdMappingConfigTypeDef](./type_defs.md#idmappingconfigtypedef) 
## CollaborationIdNamespaceAssociationTypeDef

```python
# CollaborationIdNamespaceAssociationTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CollaborationIdNamespaceAssociationTypeDef


def get_value() -> CollaborationIdNamespaceAssociationTypeDef:
    return {
        "id": ...,
    }


# CollaborationIdNamespaceAssociationTypeDef definition

class CollaborationIdNamespaceAssociationTypeDef(TypedDict):
    id: str,
    arn: str,
    collaborationId: str,
    collaborationArn: str,
    name: str,
    creatorAccountId: str,
    createTime: datetime,
    updateTime: datetime,
    inputReferenceConfig: IdNamespaceAssociationInputReferenceConfigTypeDef,  # (1)
    inputReferenceProperties: IdNamespaceAssociationInputReferencePropertiesTypeDef,  # (2)
    description: NotRequired[str],
    idMappingConfig: NotRequired[IdMappingConfigTypeDef],  # (3)
```

1. See [:material-code-braces: IdNamespaceAssociationInputReferenceConfigTypeDef](./type_defs.md#idnamespaceassociationinputreferenceconfigtypedef) 
2. See [:material-code-braces: IdNamespaceAssociationInputReferencePropertiesTypeDef](./type_defs.md#idnamespaceassociationinputreferencepropertiestypedef) 
3. See [:material-code-braces: IdMappingConfigTypeDef](./type_defs.md#idmappingconfigtypedef) 
## IdNamespaceAssociationTypeDef

```python
# IdNamespaceAssociationTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import IdNamespaceAssociationTypeDef


def get_value() -> IdNamespaceAssociationTypeDef:
    return {
        "id": ...,
    }


# IdNamespaceAssociationTypeDef definition

class IdNamespaceAssociationTypeDef(TypedDict):
    id: str,
    arn: str,
    membershipId: str,
    membershipArn: str,
    collaborationId: str,
    collaborationArn: str,
    name: str,
    createTime: datetime,
    updateTime: datetime,
    inputReferenceConfig: IdNamespaceAssociationInputReferenceConfigTypeDef,  # (1)
    inputReferenceProperties: IdNamespaceAssociationInputReferencePropertiesTypeDef,  # (2)
    description: NotRequired[str],
    idMappingConfig: NotRequired[IdMappingConfigTypeDef],  # (3)
```

1. See [:material-code-braces: IdNamespaceAssociationInputReferenceConfigTypeDef](./type_defs.md#idnamespaceassociationinputreferenceconfigtypedef) 
2. See [:material-code-braces: IdNamespaceAssociationInputReferencePropertiesTypeDef](./type_defs.md#idnamespaceassociationinputreferencepropertiestypedef) 
3. See [:material-code-braces: IdMappingConfigTypeDef](./type_defs.md#idmappingconfigtypedef) 
## ListCollaborationPrivacyBudgetTemplatesOutputTypeDef

```python
# ListCollaborationPrivacyBudgetTemplatesOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListCollaborationPrivacyBudgetTemplatesOutputTypeDef


def get_value() -> ListCollaborationPrivacyBudgetTemplatesOutputTypeDef:
    return {
        "nextToken": ...,
    }


# ListCollaborationPrivacyBudgetTemplatesOutputTypeDef definition

class ListCollaborationPrivacyBudgetTemplatesOutputTypeDef(TypedDict):
    collaborationPrivacyBudgetTemplateSummaries: List[CollaborationPrivacyBudgetTemplateSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CollaborationPrivacyBudgetTemplateSummaryTypeDef](./type_defs.md#collaborationprivacybudgettemplatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCollaborationsOutputTypeDef

```python
# ListCollaborationsOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListCollaborationsOutputTypeDef


def get_value() -> ListCollaborationsOutputTypeDef:
    return {
        "nextToken": ...,
    }


# ListCollaborationsOutputTypeDef definition

class ListCollaborationsOutputTypeDef(TypedDict):
    collaborationList: List[CollaborationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CollaborationSummaryTypeDef](./type_defs.md#collaborationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CollaborationTypeDef

```python
# CollaborationTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CollaborationTypeDef


def get_value() -> CollaborationTypeDef:
    return {
        "id": ...,
    }


# CollaborationTypeDef definition

class CollaborationTypeDef(TypedDict):
    id: str,
    arn: str,
    name: str,
    creatorAccountId: str,
    creatorDisplayName: str,
    createTime: datetime,
    updateTime: datetime,
    memberStatus: MemberStatusType,  # (1)
    queryLogStatus: CollaborationQueryLogStatusType,  # (3)
    description: NotRequired[str],
    membershipId: NotRequired[str],
    membershipArn: NotRequired[str],
    dataEncryptionMetadata: NotRequired[DataEncryptionMetadataTypeDef],  # (2)
    analyticsEngine: NotRequired[AnalyticsEngineType],  # (4)
```

1. See [:material-code-brackets: MemberStatusType](./literals.md#memberstatustype) 
2. See [:material-code-braces: DataEncryptionMetadataTypeDef](./type_defs.md#dataencryptionmetadatatypedef) 
3. See [:material-code-brackets: CollaborationQueryLogStatusType](./literals.md#collaborationquerylogstatustype) 
4. See [:material-code-brackets: AnalyticsEngineType](./literals.md#analyticsenginetype) 
## ComputeConfigurationTypeDef

```python
# ComputeConfigurationTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ComputeConfigurationTypeDef


def get_value() -> ComputeConfigurationTypeDef:
    return {
        "worker": ...,
    }


# ComputeConfigurationTypeDef definition

class ComputeConfigurationTypeDef(TypedDict):
    worker: NotRequired[WorkerComputeConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: WorkerComputeConfigurationTypeDef](./type_defs.md#workercomputeconfigurationtypedef) 
## ConfigurationDetailsTypeDef

```python
# ConfigurationDetailsTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ConfigurationDetailsTypeDef


def get_value() -> ConfigurationDetailsTypeDef:
    return {
        "directAnalysisConfigurationDetails": ...,
    }


# ConfigurationDetailsTypeDef definition

class ConfigurationDetailsTypeDef(TypedDict):
    directAnalysisConfigurationDetails: NotRequired[DirectAnalysisConfigurationDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: DirectAnalysisConfigurationDetailsTypeDef](./type_defs.md#directanalysisconfigurationdetailstypedef) 
## ListConfiguredAudienceModelAssociationsOutputTypeDef

```python
# ListConfiguredAudienceModelAssociationsOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListConfiguredAudienceModelAssociationsOutputTypeDef


def get_value() -> ListConfiguredAudienceModelAssociationsOutputTypeDef:
    return {
        "configuredAudienceModelAssociationSummaries": ...,
    }


# ListConfiguredAudienceModelAssociationsOutputTypeDef definition

class ListConfiguredAudienceModelAssociationsOutputTypeDef(TypedDict):
    configuredAudienceModelAssociationSummaries: List[ConfiguredAudienceModelAssociationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ConfiguredAudienceModelAssociationSummaryTypeDef](./type_defs.md#configuredaudiencemodelassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConfiguredAudienceModelAssociationOutputTypeDef

```python
# CreateConfiguredAudienceModelAssociationOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CreateConfiguredAudienceModelAssociationOutputTypeDef


def get_value() -> CreateConfiguredAudienceModelAssociationOutputTypeDef:
    return {
        "configuredAudienceModelAssociation": ...,
    }


# CreateConfiguredAudienceModelAssociationOutputTypeDef definition

class CreateConfiguredAudienceModelAssociationOutputTypeDef(TypedDict):
    configuredAudienceModelAssociation: ConfiguredAudienceModelAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredAudienceModelAssociationTypeDef](./type_defs.md#configuredaudiencemodelassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConfiguredAudienceModelAssociationOutputTypeDef

```python
# GetConfiguredAudienceModelAssociationOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetConfiguredAudienceModelAssociationOutputTypeDef


def get_value() -> GetConfiguredAudienceModelAssociationOutputTypeDef:
    return {
        "configuredAudienceModelAssociation": ...,
    }


# GetConfiguredAudienceModelAssociationOutputTypeDef definition

class GetConfiguredAudienceModelAssociationOutputTypeDef(TypedDict):
    configuredAudienceModelAssociation: ConfiguredAudienceModelAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredAudienceModelAssociationTypeDef](./type_defs.md#configuredaudiencemodelassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateConfiguredAudienceModelAssociationOutputTypeDef

```python
# UpdateConfiguredAudienceModelAssociationOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import UpdateConfiguredAudienceModelAssociationOutputTypeDef


def get_value() -> UpdateConfiguredAudienceModelAssociationOutputTypeDef:
    return {
        "configuredAudienceModelAssociation": ...,
    }


# UpdateConfiguredAudienceModelAssociationOutputTypeDef definition

class UpdateConfiguredAudienceModelAssociationOutputTypeDef(TypedDict):
    configuredAudienceModelAssociation: ConfiguredAudienceModelAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredAudienceModelAssociationTypeDef](./type_defs.md#configuredaudiencemodelassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConfiguredTableAssociationAnalysisRulePolicyV1OutputTypeDef

```python
# ConfiguredTableAssociationAnalysisRulePolicyV1OutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ConfiguredTableAssociationAnalysisRulePolicyV1OutputTypeDef


def get_value() -> ConfiguredTableAssociationAnalysisRulePolicyV1OutputTypeDef:
    return {
        "list": ...,
    }


# ConfiguredTableAssociationAnalysisRulePolicyV1OutputTypeDef definition

class ConfiguredTableAssociationAnalysisRulePolicyV1OutputTypeDef(TypedDict):
    list: NotRequired[ConfiguredTableAssociationAnalysisRuleListOutputTypeDef],  # (1)
    aggregation: NotRequired[ConfiguredTableAssociationAnalysisRuleAggregationOutputTypeDef],  # (2)
    custom: NotRequired[ConfiguredTableAssociationAnalysisRuleCustomOutputTypeDef],  # (3)
```

1. See [:material-code-braces: ConfiguredTableAssociationAnalysisRuleListOutputTypeDef](./type_defs.md#configuredtableassociationanalysisrulelistoutputtypedef) 
2. See [:material-code-braces: ConfiguredTableAssociationAnalysisRuleAggregationOutputTypeDef](./type_defs.md#configuredtableassociationanalysisruleaggregationoutputtypedef) 
3. See [:material-code-braces: ConfiguredTableAssociationAnalysisRuleCustomOutputTypeDef](./type_defs.md#configuredtableassociationanalysisrulecustomoutputtypedef) 
## ConfiguredTableAssociationAnalysisRulePolicyV1TypeDef

```python
# ConfiguredTableAssociationAnalysisRulePolicyV1TypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ConfiguredTableAssociationAnalysisRulePolicyV1TypeDef


def get_value() -> ConfiguredTableAssociationAnalysisRulePolicyV1TypeDef:
    return {
        "list": ...,
    }


# ConfiguredTableAssociationAnalysisRulePolicyV1TypeDef definition

class ConfiguredTableAssociationAnalysisRulePolicyV1TypeDef(TypedDict):
    list: NotRequired[ConfiguredTableAssociationAnalysisRuleListTypeDef],  # (1)
    aggregation: NotRequired[ConfiguredTableAssociationAnalysisRuleAggregationTypeDef],  # (2)
    custom: NotRequired[ConfiguredTableAssociationAnalysisRuleCustomTypeDef],  # (3)
```

1. See [:material-code-braces: ConfiguredTableAssociationAnalysisRuleListTypeDef](./type_defs.md#configuredtableassociationanalysisrulelisttypedef) 
2. See [:material-code-braces: ConfiguredTableAssociationAnalysisRuleAggregationTypeDef](./type_defs.md#configuredtableassociationanalysisruleaggregationtypedef) 
3. See [:material-code-braces: ConfiguredTableAssociationAnalysisRuleCustomTypeDef](./type_defs.md#configuredtableassociationanalysisrulecustomtypedef) 
## ListConfiguredTableAssociationsOutputTypeDef

```python
# ListConfiguredTableAssociationsOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListConfiguredTableAssociationsOutputTypeDef


def get_value() -> ListConfiguredTableAssociationsOutputTypeDef:
    return {
        "configuredTableAssociationSummaries": ...,
    }


# ListConfiguredTableAssociationsOutputTypeDef definition

class ListConfiguredTableAssociationsOutputTypeDef(TypedDict):
    configuredTableAssociationSummaries: List[ConfiguredTableAssociationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ConfiguredTableAssociationSummaryTypeDef](./type_defs.md#configuredtableassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConfiguredTableAssociationOutputTypeDef

```python
# CreateConfiguredTableAssociationOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CreateConfiguredTableAssociationOutputTypeDef


def get_value() -> CreateConfiguredTableAssociationOutputTypeDef:
    return {
        "configuredTableAssociation": ...,
    }


# CreateConfiguredTableAssociationOutputTypeDef definition

class CreateConfiguredTableAssociationOutputTypeDef(TypedDict):
    configuredTableAssociation: ConfiguredTableAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableAssociationTypeDef](./type_defs.md#configuredtableassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConfiguredTableAssociationOutputTypeDef

```python
# GetConfiguredTableAssociationOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetConfiguredTableAssociationOutputTypeDef


def get_value() -> GetConfiguredTableAssociationOutputTypeDef:
    return {
        "configuredTableAssociation": ...,
    }


# GetConfiguredTableAssociationOutputTypeDef definition

class GetConfiguredTableAssociationOutputTypeDef(TypedDict):
    configuredTableAssociation: ConfiguredTableAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableAssociationTypeDef](./type_defs.md#configuredtableassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateConfiguredTableAssociationOutputTypeDef

```python
# UpdateConfiguredTableAssociationOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import UpdateConfiguredTableAssociationOutputTypeDef


def get_value() -> UpdateConfiguredTableAssociationOutputTypeDef:
    return {
        "configuredTableAssociation": ...,
    }


# UpdateConfiguredTableAssociationOutputTypeDef definition

class UpdateConfiguredTableAssociationOutputTypeDef(TypedDict):
    configuredTableAssociation: ConfiguredTableAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableAssociationTypeDef](./type_defs.md#configuredtableassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConfiguredTablesOutputTypeDef

```python
# ListConfiguredTablesOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListConfiguredTablesOutputTypeDef


def get_value() -> ListConfiguredTablesOutputTypeDef:
    return {
        "configuredTableSummaries": ...,
    }


# ListConfiguredTablesOutputTypeDef definition

class ListConfiguredTablesOutputTypeDef(TypedDict):
    configuredTableSummaries: List[ConfiguredTableSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ConfiguredTableSummaryTypeDef](./type_defs.md#configuredtablesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateIdMappingTableInputTypeDef

```python
# CreateIdMappingTableInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CreateIdMappingTableInputTypeDef


def get_value() -> CreateIdMappingTableInputTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# CreateIdMappingTableInputTypeDef definition

class CreateIdMappingTableInputTypeDef(TypedDict):
    membershipIdentifier: str,
    name: str,
    inputReferenceConfig: IdMappingTableInputReferenceConfigTypeDef,  # (1)
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    kmsKeyArn: NotRequired[str],
```

1. See [:material-code-braces: IdMappingTableInputReferenceConfigTypeDef](./type_defs.md#idmappingtableinputreferenceconfigtypedef) 
## IdMappingTableSummaryTypeDef

```python
# IdMappingTableSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import IdMappingTableSummaryTypeDef


def get_value() -> IdMappingTableSummaryTypeDef:
    return {
        "collaborationArn": ...,
    }


# IdMappingTableSummaryTypeDef definition

class IdMappingTableSummaryTypeDef(TypedDict):
    collaborationArn: str,
    collaborationId: str,
    membershipId: str,
    membershipArn: str,
    createTime: datetime,
    updateTime: datetime,
    id: str,
    arn: str,
    inputReferenceConfig: IdMappingTableInputReferenceConfigTypeDef,  # (1)
    name: str,
    description: NotRequired[str],
```

1. See [:material-code-braces: IdMappingTableInputReferenceConfigTypeDef](./type_defs.md#idmappingtableinputreferenceconfigtypedef) 
## DifferentialPrivacyConfigurationOutputTypeDef

```python
# DifferentialPrivacyConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import DifferentialPrivacyConfigurationOutputTypeDef


def get_value() -> DifferentialPrivacyConfigurationOutputTypeDef:
    return {
        "columns": ...,
    }


# DifferentialPrivacyConfigurationOutputTypeDef definition

class DifferentialPrivacyConfigurationOutputTypeDef(TypedDict):
    columns: List[DifferentialPrivacyColumnTypeDef],  # (1)
```

1. See [:material-code-braces: DifferentialPrivacyColumnTypeDef](./type_defs.md#differentialprivacycolumntypedef) 
## DifferentialPrivacyConfigurationTypeDef

```python
# DifferentialPrivacyConfigurationTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import DifferentialPrivacyConfigurationTypeDef


def get_value() -> DifferentialPrivacyConfigurationTypeDef:
    return {
        "columns": ...,
    }


# DifferentialPrivacyConfigurationTypeDef definition

class DifferentialPrivacyConfigurationTypeDef(TypedDict):
    columns: Sequence[DifferentialPrivacyColumnTypeDef],  # (1)
```

1. See [:material-code-braces: DifferentialPrivacyColumnTypeDef](./type_defs.md#differentialprivacycolumntypedef) 
## DifferentialPrivacyParametersTypeDef

```python
# DifferentialPrivacyParametersTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import DifferentialPrivacyParametersTypeDef


def get_value() -> DifferentialPrivacyParametersTypeDef:
    return {
        "sensitivityParameters": ...,
    }


# DifferentialPrivacyParametersTypeDef definition

class DifferentialPrivacyParametersTypeDef(TypedDict):
    sensitivityParameters: List[DifferentialPrivacySensitivityParametersTypeDef],  # (1)
```

1. See [:material-code-braces: DifferentialPrivacySensitivityParametersTypeDef](./type_defs.md#differentialprivacysensitivityparameterstypedef) 
## DifferentialPrivacyPrivacyImpactTypeDef

```python
# DifferentialPrivacyPrivacyImpactTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import DifferentialPrivacyPrivacyImpactTypeDef


def get_value() -> DifferentialPrivacyPrivacyImpactTypeDef:
    return {
        "aggregations": ...,
    }


# DifferentialPrivacyPrivacyImpactTypeDef definition

class DifferentialPrivacyPrivacyImpactTypeDef(TypedDict):
    aggregations: List[DifferentialPrivacyPreviewAggregationTypeDef],  # (1)
```

1. See [:material-code-braces: DifferentialPrivacyPreviewAggregationTypeDef](./type_defs.md#differentialprivacypreviewaggregationtypedef) 
## PreviewPrivacyImpactParametersInputTypeDef

```python
# PreviewPrivacyImpactParametersInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import PreviewPrivacyImpactParametersInputTypeDef


def get_value() -> PreviewPrivacyImpactParametersInputTypeDef:
    return {
        "differentialPrivacy": ...,
    }


# PreviewPrivacyImpactParametersInputTypeDef definition

class PreviewPrivacyImpactParametersInputTypeDef(TypedDict):
    differentialPrivacy: NotRequired[DifferentialPrivacyPreviewParametersInputTypeDef],  # (1)
```

1. See [:material-code-braces: DifferentialPrivacyPreviewParametersInputTypeDef](./type_defs.md#differentialprivacypreviewparametersinputtypedef) 
## DifferentialPrivacyPrivacyBudgetTypeDef

```python
# DifferentialPrivacyPrivacyBudgetTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import DifferentialPrivacyPrivacyBudgetTypeDef


def get_value() -> DifferentialPrivacyPrivacyBudgetTypeDef:
    return {
        "aggregations": ...,
    }


# DifferentialPrivacyPrivacyBudgetTypeDef definition

class DifferentialPrivacyPrivacyBudgetTypeDef(TypedDict):
    aggregations: List[DifferentialPrivacyPrivacyBudgetAggregationTypeDef],  # (1)
    epsilon: int,
```

1. See [:material-code-braces: DifferentialPrivacyPrivacyBudgetAggregationTypeDef](./type_defs.md#differentialprivacyprivacybudgetaggregationtypedef) 
## PrivacyBudgetTemplateParametersInputTypeDef

```python
# PrivacyBudgetTemplateParametersInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import PrivacyBudgetTemplateParametersInputTypeDef


def get_value() -> PrivacyBudgetTemplateParametersInputTypeDef:
    return {
        "differentialPrivacy": ...,
    }


# PrivacyBudgetTemplateParametersInputTypeDef definition

class PrivacyBudgetTemplateParametersInputTypeDef(TypedDict):
    differentialPrivacy: NotRequired[DifferentialPrivacyTemplateParametersInputTypeDef],  # (1)
```

1. See [:material-code-braces: DifferentialPrivacyTemplateParametersInputTypeDef](./type_defs.md#differentialprivacytemplateparametersinputtypedef) 
## PrivacyBudgetTemplateParametersOutputTypeDef

```python
# PrivacyBudgetTemplateParametersOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import PrivacyBudgetTemplateParametersOutputTypeDef


def get_value() -> PrivacyBudgetTemplateParametersOutputTypeDef:
    return {
        "differentialPrivacy": ...,
    }


# PrivacyBudgetTemplateParametersOutputTypeDef definition

class PrivacyBudgetTemplateParametersOutputTypeDef(TypedDict):
    differentialPrivacy: NotRequired[DifferentialPrivacyTemplateParametersOutputTypeDef],  # (1)
```

1. See [:material-code-braces: DifferentialPrivacyTemplateParametersOutputTypeDef](./type_defs.md#differentialprivacytemplateparametersoutputtypedef) 
## PrivacyBudgetTemplateUpdateParametersTypeDef

```python
# PrivacyBudgetTemplateUpdateParametersTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import PrivacyBudgetTemplateUpdateParametersTypeDef


def get_value() -> PrivacyBudgetTemplateUpdateParametersTypeDef:
    return {
        "differentialPrivacy": ...,
    }


# PrivacyBudgetTemplateUpdateParametersTypeDef definition

class PrivacyBudgetTemplateUpdateParametersTypeDef(TypedDict):
    differentialPrivacy: NotRequired[DifferentialPrivacyTemplateUpdateParametersTypeDef],  # (1)
```

1. See [:material-code-braces: DifferentialPrivacyTemplateUpdateParametersTypeDef](./type_defs.md#differentialprivacytemplateupdateparameterstypedef) 
## IdMappingTableInputReferencePropertiesTypeDef

```python
# IdMappingTableInputReferencePropertiesTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import IdMappingTableInputReferencePropertiesTypeDef


def get_value() -> IdMappingTableInputReferencePropertiesTypeDef:
    return {
        "idMappingTableInputSource": ...,
    }


# IdMappingTableInputReferencePropertiesTypeDef definition

class IdMappingTableInputReferencePropertiesTypeDef(TypedDict):
    idMappingTableInputSource: List[IdMappingTableInputSourceTypeDef],  # (1)
```

1. See [:material-code-braces: IdMappingTableInputSourceTypeDef](./type_defs.md#idmappingtableinputsourcetypedef) 
## IdMappingTableSchemaTypePropertiesTypeDef

```python
# IdMappingTableSchemaTypePropertiesTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import IdMappingTableSchemaTypePropertiesTypeDef


def get_value() -> IdMappingTableSchemaTypePropertiesTypeDef:
    return {
        "idMappingTableInputSource": ...,
    }


# IdMappingTableSchemaTypePropertiesTypeDef definition

class IdMappingTableSchemaTypePropertiesTypeDef(TypedDict):
    idMappingTableInputSource: List[IdMappingTableInputSourceTypeDef],  # (1)
```

1. See [:material-code-braces: IdMappingTableInputSourceTypeDef](./type_defs.md#idmappingtableinputsourcetypedef) 
## ListAnalysisTemplatesInputPaginateTypeDef

```python
# ListAnalysisTemplatesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListAnalysisTemplatesInputPaginateTypeDef


def get_value() -> ListAnalysisTemplatesInputPaginateTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# ListAnalysisTemplatesInputPaginateTypeDef definition

class ListAnalysisTemplatesInputPaginateTypeDef(TypedDict):
    membershipIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCollaborationAnalysisTemplatesInputPaginateTypeDef

```python
# ListCollaborationAnalysisTemplatesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListCollaborationAnalysisTemplatesInputPaginateTypeDef


def get_value() -> ListCollaborationAnalysisTemplatesInputPaginateTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# ListCollaborationAnalysisTemplatesInputPaginateTypeDef definition

class ListCollaborationAnalysisTemplatesInputPaginateTypeDef(TypedDict):
    collaborationIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCollaborationConfiguredAudienceModelAssociationsInputPaginateTypeDef

```python
# ListCollaborationConfiguredAudienceModelAssociationsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListCollaborationConfiguredAudienceModelAssociationsInputPaginateTypeDef


def get_value() -> ListCollaborationConfiguredAudienceModelAssociationsInputPaginateTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# ListCollaborationConfiguredAudienceModelAssociationsInputPaginateTypeDef definition

class ListCollaborationConfiguredAudienceModelAssociationsInputPaginateTypeDef(TypedDict):
    collaborationIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCollaborationIdNamespaceAssociationsInputPaginateTypeDef

```python
# ListCollaborationIdNamespaceAssociationsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListCollaborationIdNamespaceAssociationsInputPaginateTypeDef


def get_value() -> ListCollaborationIdNamespaceAssociationsInputPaginateTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# ListCollaborationIdNamespaceAssociationsInputPaginateTypeDef definition

class ListCollaborationIdNamespaceAssociationsInputPaginateTypeDef(TypedDict):
    collaborationIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCollaborationPrivacyBudgetTemplatesInputPaginateTypeDef

```python
# ListCollaborationPrivacyBudgetTemplatesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListCollaborationPrivacyBudgetTemplatesInputPaginateTypeDef


def get_value() -> ListCollaborationPrivacyBudgetTemplatesInputPaginateTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# ListCollaborationPrivacyBudgetTemplatesInputPaginateTypeDef definition

class ListCollaborationPrivacyBudgetTemplatesInputPaginateTypeDef(TypedDict):
    collaborationIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCollaborationPrivacyBudgetsInputPaginateTypeDef

```python
# ListCollaborationPrivacyBudgetsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListCollaborationPrivacyBudgetsInputPaginateTypeDef


def get_value() -> ListCollaborationPrivacyBudgetsInputPaginateTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# ListCollaborationPrivacyBudgetsInputPaginateTypeDef definition

class ListCollaborationPrivacyBudgetsInputPaginateTypeDef(TypedDict):
    collaborationIdentifier: str,
    privacyBudgetType: PrivacyBudgetTypeType,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: PrivacyBudgetTypeType](./literals.md#privacybudgettypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCollaborationsInputPaginateTypeDef

```python
# ListCollaborationsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListCollaborationsInputPaginateTypeDef


def get_value() -> ListCollaborationsInputPaginateTypeDef:
    return {
        "memberStatus": ...,
    }


# ListCollaborationsInputPaginateTypeDef definition

class ListCollaborationsInputPaginateTypeDef(TypedDict):
    memberStatus: NotRequired[FilterableMemberStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: FilterableMemberStatusType](./literals.md#filterablememberstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConfiguredAudienceModelAssociationsInputPaginateTypeDef

```python
# ListConfiguredAudienceModelAssociationsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListConfiguredAudienceModelAssociationsInputPaginateTypeDef


def get_value() -> ListConfiguredAudienceModelAssociationsInputPaginateTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# ListConfiguredAudienceModelAssociationsInputPaginateTypeDef definition

class ListConfiguredAudienceModelAssociationsInputPaginateTypeDef(TypedDict):
    membershipIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConfiguredTableAssociationsInputPaginateTypeDef

```python
# ListConfiguredTableAssociationsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListConfiguredTableAssociationsInputPaginateTypeDef


def get_value() -> ListConfiguredTableAssociationsInputPaginateTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# ListConfiguredTableAssociationsInputPaginateTypeDef definition

class ListConfiguredTableAssociationsInputPaginateTypeDef(TypedDict):
    membershipIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConfiguredTablesInputPaginateTypeDef

```python
# ListConfiguredTablesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListConfiguredTablesInputPaginateTypeDef


def get_value() -> ListConfiguredTablesInputPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListConfiguredTablesInputPaginateTypeDef definition

class ListConfiguredTablesInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIdMappingTablesInputPaginateTypeDef

```python
# ListIdMappingTablesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListIdMappingTablesInputPaginateTypeDef


def get_value() -> ListIdMappingTablesInputPaginateTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# ListIdMappingTablesInputPaginateTypeDef definition

class ListIdMappingTablesInputPaginateTypeDef(TypedDict):
    membershipIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIdNamespaceAssociationsInputPaginateTypeDef

```python
# ListIdNamespaceAssociationsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListIdNamespaceAssociationsInputPaginateTypeDef


def get_value() -> ListIdNamespaceAssociationsInputPaginateTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# ListIdNamespaceAssociationsInputPaginateTypeDef definition

class ListIdNamespaceAssociationsInputPaginateTypeDef(TypedDict):
    membershipIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMembersInputPaginateTypeDef

```python
# ListMembersInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListMembersInputPaginateTypeDef


def get_value() -> ListMembersInputPaginateTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# ListMembersInputPaginateTypeDef definition

class ListMembersInputPaginateTypeDef(TypedDict):
    collaborationIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMembershipsInputPaginateTypeDef

```python
# ListMembershipsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListMembershipsInputPaginateTypeDef


def get_value() -> ListMembershipsInputPaginateTypeDef:
    return {
        "status": ...,
    }


# ListMembershipsInputPaginateTypeDef definition

class ListMembershipsInputPaginateTypeDef(TypedDict):
    status: NotRequired[MembershipStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: MembershipStatusType](./literals.md#membershipstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPrivacyBudgetTemplatesInputPaginateTypeDef

```python
# ListPrivacyBudgetTemplatesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListPrivacyBudgetTemplatesInputPaginateTypeDef


def get_value() -> ListPrivacyBudgetTemplatesInputPaginateTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# ListPrivacyBudgetTemplatesInputPaginateTypeDef definition

class ListPrivacyBudgetTemplatesInputPaginateTypeDef(TypedDict):
    membershipIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPrivacyBudgetsInputPaginateTypeDef

```python
# ListPrivacyBudgetsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListPrivacyBudgetsInputPaginateTypeDef


def get_value() -> ListPrivacyBudgetsInputPaginateTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# ListPrivacyBudgetsInputPaginateTypeDef definition

class ListPrivacyBudgetsInputPaginateTypeDef(TypedDict):
    membershipIdentifier: str,
    privacyBudgetType: PrivacyBudgetTypeType,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: PrivacyBudgetTypeType](./literals.md#privacybudgettypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProtectedQueriesInputPaginateTypeDef

```python
# ListProtectedQueriesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListProtectedQueriesInputPaginateTypeDef


def get_value() -> ListProtectedQueriesInputPaginateTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# ListProtectedQueriesInputPaginateTypeDef definition

class ListProtectedQueriesInputPaginateTypeDef(TypedDict):
    membershipIdentifier: str,
    status: NotRequired[ProtectedQueryStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ProtectedQueryStatusType](./literals.md#protectedquerystatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSchemasInputPaginateTypeDef

```python
# ListSchemasInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListSchemasInputPaginateTypeDef


def get_value() -> ListSchemasInputPaginateTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# ListSchemasInputPaginateTypeDef definition

class ListSchemasInputPaginateTypeDef(TypedDict):
    collaborationIdentifier: str,
    schemaType: NotRequired[SchemaTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: SchemaTypeType](./literals.md#schematypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPrivacyBudgetTemplatesOutputTypeDef

```python
# ListPrivacyBudgetTemplatesOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListPrivacyBudgetTemplatesOutputTypeDef


def get_value() -> ListPrivacyBudgetTemplatesOutputTypeDef:
    return {
        "nextToken": ...,
    }


# ListPrivacyBudgetTemplatesOutputTypeDef definition

class ListPrivacyBudgetTemplatesOutputTypeDef(TypedDict):
    privacyBudgetTemplateSummaries: List[PrivacyBudgetTemplateSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PrivacyBudgetTemplateSummaryTypeDef](./type_defs.md#privacybudgettemplatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSchemasOutputTypeDef

```python
# ListSchemasOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListSchemasOutputTypeDef


def get_value() -> ListSchemasOutputTypeDef:
    return {
        "schemaSummaries": ...,
    }


# ListSchemasOutputTypeDef definition

class ListSchemasOutputTypeDef(TypedDict):
    schemaSummaries: List[SchemaSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SchemaSummaryTypeDef](./type_defs.md#schemasummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MLPaymentConfigTypeDef

```python
# MLPaymentConfigTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import MLPaymentConfigTypeDef


def get_value() -> MLPaymentConfigTypeDef:
    return {
        "modelTraining": ...,
    }


# MLPaymentConfigTypeDef definition

class MLPaymentConfigTypeDef(TypedDict):
    modelTraining: NotRequired[ModelTrainingPaymentConfigTypeDef],  # (1)
    modelInference: NotRequired[ModelInferencePaymentConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ModelTrainingPaymentConfigTypeDef](./type_defs.md#modeltrainingpaymentconfigtypedef) 
2. See [:material-code-braces: ModelInferencePaymentConfigTypeDef](./type_defs.md#modelinferencepaymentconfigtypedef) 
## MembershipMLPaymentConfigTypeDef

```python
# MembershipMLPaymentConfigTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import MembershipMLPaymentConfigTypeDef


def get_value() -> MembershipMLPaymentConfigTypeDef:
    return {
        "modelTraining": ...,
    }


# MembershipMLPaymentConfigTypeDef definition

class MembershipMLPaymentConfigTypeDef(TypedDict):
    modelTraining: NotRequired[MembershipModelTrainingPaymentConfigTypeDef],  # (1)
    modelInference: NotRequired[MembershipModelInferencePaymentConfigTypeDef],  # (2)
```

1. See [:material-code-braces: MembershipModelTrainingPaymentConfigTypeDef](./type_defs.md#membershipmodeltrainingpaymentconfigtypedef) 
2. See [:material-code-braces: MembershipModelInferencePaymentConfigTypeDef](./type_defs.md#membershipmodelinferencepaymentconfigtypedef) 
## MembershipProtectedQueryOutputConfigurationTypeDef

```python
# MembershipProtectedQueryOutputConfigurationTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import MembershipProtectedQueryOutputConfigurationTypeDef


def get_value() -> MembershipProtectedQueryOutputConfigurationTypeDef:
    return {
        "s3": ...,
    }


# MembershipProtectedQueryOutputConfigurationTypeDef definition

class MembershipProtectedQueryOutputConfigurationTypeDef(TypedDict):
    s3: NotRequired[ProtectedQueryS3OutputConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ProtectedQueryS3OutputConfigurationTypeDef](./type_defs.md#protectedquerys3outputconfigurationtypedef) 
## ProtectedQueryOutputConfigurationTypeDef

```python
# ProtectedQueryOutputConfigurationTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ProtectedQueryOutputConfigurationTypeDef


def get_value() -> ProtectedQueryOutputConfigurationTypeDef:
    return {
        "s3": ...,
    }


# ProtectedQueryOutputConfigurationTypeDef definition

class ProtectedQueryOutputConfigurationTypeDef(TypedDict):
    s3: NotRequired[ProtectedQueryS3OutputConfigurationTypeDef],  # (1)
    member: NotRequired[ProtectedQueryMemberOutputConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: ProtectedQueryS3OutputConfigurationTypeDef](./type_defs.md#protectedquerys3outputconfigurationtypedef) 
2. See [:material-code-braces: ProtectedQueryMemberOutputConfigurationTypeDef](./type_defs.md#protectedquerymemberoutputconfigurationtypedef) 
## ProtectedQueryOutputTypeDef

```python
# ProtectedQueryOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ProtectedQueryOutputTypeDef


def get_value() -> ProtectedQueryOutputTypeDef:
    return {
        "s3": ...,
    }


# ProtectedQueryOutputTypeDef definition

class ProtectedQueryOutputTypeDef(TypedDict):
    s3: NotRequired[ProtectedQueryS3OutputTypeDef],  # (1)
    memberList: NotRequired[List[ProtectedQuerySingleMemberOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: ProtectedQueryS3OutputTypeDef](./type_defs.md#protectedquerys3outputtypedef) 
2. See [:material-code-braces: ProtectedQuerySingleMemberOutputTypeDef](./type_defs.md#protectedquerysinglememberoutputtypedef) 
## QueryConstraintTypeDef

```python
# QueryConstraintTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import QueryConstraintTypeDef


def get_value() -> QueryConstraintTypeDef:
    return {
        "requireOverlap": ...,
    }


# QueryConstraintTypeDef definition

class QueryConstraintTypeDef(TypedDict):
    requireOverlap: NotRequired[QueryConstraintRequireOverlapTypeDef],  # (1)
```

1. See [:material-code-braces: QueryConstraintRequireOverlapTypeDef](./type_defs.md#queryconstraintrequireoverlaptypedef) 
## SchemaStatusDetailTypeDef

```python
# SchemaStatusDetailTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import SchemaStatusDetailTypeDef


def get_value() -> SchemaStatusDetailTypeDef:
    return {
        "status": ...,
    }


# SchemaStatusDetailTypeDef definition

class SchemaStatusDetailTypeDef(TypedDict):
    status: SchemaStatusType,  # (1)
    analysisType: AnalysisTypeType,  # (5)
    reasons: NotRequired[List[SchemaStatusReasonTypeDef]],  # (2)
    analysisRuleType: NotRequired[AnalysisRuleTypeType],  # (3)
    configurations: NotRequired[List[SchemaConfigurationType]],  # (4)
```

1. See [:material-code-brackets: SchemaStatusType](./literals.md#schemastatustype) 
2. See [:material-code-braces: SchemaStatusReasonTypeDef](./type_defs.md#schemastatusreasontypedef) 
3. See [:material-code-brackets: AnalysisRuleTypeType](./literals.md#analysisruletypetype) 
4. See [:material-code-brackets: SchemaConfigurationType](./literals.md#schemaconfigurationtype) 
5. See [:material-code-brackets: AnalysisTypeType](./literals.md#analysistypetype) 
## SnowflakeTableSchemaOutputTypeDef

```python
# SnowflakeTableSchemaOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import SnowflakeTableSchemaOutputTypeDef


def get_value() -> SnowflakeTableSchemaOutputTypeDef:
    return {
        "v1": ...,
    }


# SnowflakeTableSchemaOutputTypeDef definition

class SnowflakeTableSchemaOutputTypeDef(TypedDict):
    v1: NotRequired[List[SnowflakeTableSchemaV1TypeDef]],  # (1)
```

1. See [:material-code-braces: SnowflakeTableSchemaV1TypeDef](./type_defs.md#snowflaketableschemav1typedef) 
## SnowflakeTableSchemaTypeDef

```python
# SnowflakeTableSchemaTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import SnowflakeTableSchemaTypeDef


def get_value() -> SnowflakeTableSchemaTypeDef:
    return {
        "v1": ...,
    }


# SnowflakeTableSchemaTypeDef definition

class SnowflakeTableSchemaTypeDef(TypedDict):
    v1: NotRequired[Sequence[SnowflakeTableSchemaV1TypeDef]],  # (1)
```

1. See [:material-code-braces: SnowflakeTableSchemaV1TypeDef](./type_defs.md#snowflaketableschemav1typedef) 
## AnalysisTemplateTypeDef

```python
# AnalysisTemplateTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import AnalysisTemplateTypeDef


def get_value() -> AnalysisTemplateTypeDef:
    return {
        "id": ...,
    }


# AnalysisTemplateTypeDef definition

class AnalysisTemplateTypeDef(TypedDict):
    id: str,
    arn: str,
    collaborationId: str,
    collaborationArn: str,
    membershipId: str,
    membershipArn: str,
    name: str,
    createTime: datetime,
    updateTime: datetime,
    schema: AnalysisSchemaTypeDef,  # (1)
    format: AnalysisFormatType,  # (2)
    source: AnalysisSourceTypeDef,  # (3)
    description: NotRequired[str],
    analysisParameters: NotRequired[List[AnalysisParameterTypeDef]],  # (4)
    validations: NotRequired[List[AnalysisTemplateValidationStatusDetailTypeDef]],  # (5)
```

1. See [:material-code-braces: AnalysisSchemaTypeDef](./type_defs.md#analysisschematypedef) 
2. See [:material-code-brackets: AnalysisFormatType](./literals.md#analysisformattype) 
3. See [:material-code-braces: AnalysisSourceTypeDef](./type_defs.md#analysissourcetypedef) 
4. See [:material-code-braces: AnalysisParameterTypeDef](./type_defs.md#analysisparametertypedef) 
5. See [:material-code-braces: AnalysisTemplateValidationStatusDetailTypeDef](./type_defs.md#analysistemplatevalidationstatusdetailtypedef) 
## CollaborationAnalysisTemplateTypeDef

```python
# CollaborationAnalysisTemplateTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CollaborationAnalysisTemplateTypeDef


def get_value() -> CollaborationAnalysisTemplateTypeDef:
    return {
        "id": ...,
    }


# CollaborationAnalysisTemplateTypeDef definition

class CollaborationAnalysisTemplateTypeDef(TypedDict):
    id: str,
    arn: str,
    collaborationId: str,
    collaborationArn: str,
    creatorAccountId: str,
    name: str,
    createTime: datetime,
    updateTime: datetime,
    schema: AnalysisSchemaTypeDef,  # (1)
    format: AnalysisFormatType,  # (2)
    source: AnalysisSourceTypeDef,  # (3)
    description: NotRequired[str],
    analysisParameters: NotRequired[List[AnalysisParameterTypeDef]],  # (4)
    validations: NotRequired[List[AnalysisTemplateValidationStatusDetailTypeDef]],  # (5)
```

1. See [:material-code-braces: AnalysisSchemaTypeDef](./type_defs.md#analysisschematypedef) 
2. See [:material-code-brackets: AnalysisFormatType](./literals.md#analysisformattype) 
3. See [:material-code-braces: AnalysisSourceTypeDef](./type_defs.md#analysissourcetypedef) 
4. See [:material-code-braces: AnalysisParameterTypeDef](./type_defs.md#analysisparametertypedef) 
5. See [:material-code-braces: AnalysisTemplateValidationStatusDetailTypeDef](./type_defs.md#analysistemplatevalidationstatusdetailtypedef) 
## ListCollaborationIdNamespaceAssociationsOutputTypeDef

```python
# ListCollaborationIdNamespaceAssociationsOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListCollaborationIdNamespaceAssociationsOutputTypeDef


def get_value() -> ListCollaborationIdNamespaceAssociationsOutputTypeDef:
    return {
        "nextToken": ...,
    }


# ListCollaborationIdNamespaceAssociationsOutputTypeDef definition

class ListCollaborationIdNamespaceAssociationsOutputTypeDef(TypedDict):
    collaborationIdNamespaceAssociationSummaries: List[CollaborationIdNamespaceAssociationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CollaborationIdNamespaceAssociationSummaryTypeDef](./type_defs.md#collaborationidnamespaceassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListIdNamespaceAssociationsOutputTypeDef

```python
# ListIdNamespaceAssociationsOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListIdNamespaceAssociationsOutputTypeDef


def get_value() -> ListIdNamespaceAssociationsOutputTypeDef:
    return {
        "nextToken": ...,
    }


# ListIdNamespaceAssociationsOutputTypeDef definition

class ListIdNamespaceAssociationsOutputTypeDef(TypedDict):
    idNamespaceAssociationSummaries: List[IdNamespaceAssociationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: IdNamespaceAssociationSummaryTypeDef](./type_defs.md#idnamespaceassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCollaborationIdNamespaceAssociationOutputTypeDef

```python
# GetCollaborationIdNamespaceAssociationOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetCollaborationIdNamespaceAssociationOutputTypeDef


def get_value() -> GetCollaborationIdNamespaceAssociationOutputTypeDef:
    return {
        "collaborationIdNamespaceAssociation": ...,
    }


# GetCollaborationIdNamespaceAssociationOutputTypeDef definition

class GetCollaborationIdNamespaceAssociationOutputTypeDef(TypedDict):
    collaborationIdNamespaceAssociation: CollaborationIdNamespaceAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CollaborationIdNamespaceAssociationTypeDef](./type_defs.md#collaborationidnamespaceassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateIdNamespaceAssociationOutputTypeDef

```python
# CreateIdNamespaceAssociationOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CreateIdNamespaceAssociationOutputTypeDef


def get_value() -> CreateIdNamespaceAssociationOutputTypeDef:
    return {
        "idNamespaceAssociation": ...,
    }


# CreateIdNamespaceAssociationOutputTypeDef definition

class CreateIdNamespaceAssociationOutputTypeDef(TypedDict):
    idNamespaceAssociation: IdNamespaceAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdNamespaceAssociationTypeDef](./type_defs.md#idnamespaceassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIdNamespaceAssociationOutputTypeDef

```python
# GetIdNamespaceAssociationOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetIdNamespaceAssociationOutputTypeDef


def get_value() -> GetIdNamespaceAssociationOutputTypeDef:
    return {
        "idNamespaceAssociation": ...,
    }


# GetIdNamespaceAssociationOutputTypeDef definition

class GetIdNamespaceAssociationOutputTypeDef(TypedDict):
    idNamespaceAssociation: IdNamespaceAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdNamespaceAssociationTypeDef](./type_defs.md#idnamespaceassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateIdNamespaceAssociationOutputTypeDef

```python
# UpdateIdNamespaceAssociationOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import UpdateIdNamespaceAssociationOutputTypeDef


def get_value() -> UpdateIdNamespaceAssociationOutputTypeDef:
    return {
        "idNamespaceAssociation": ...,
    }


# UpdateIdNamespaceAssociationOutputTypeDef definition

class UpdateIdNamespaceAssociationOutputTypeDef(TypedDict):
    idNamespaceAssociation: IdNamespaceAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdNamespaceAssociationTypeDef](./type_defs.md#idnamespaceassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCollaborationOutputTypeDef

```python
# CreateCollaborationOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CreateCollaborationOutputTypeDef


def get_value() -> CreateCollaborationOutputTypeDef:
    return {
        "collaboration": ...,
    }


# CreateCollaborationOutputTypeDef definition

class CreateCollaborationOutputTypeDef(TypedDict):
    collaboration: CollaborationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CollaborationTypeDef](./type_defs.md#collaborationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCollaborationOutputTypeDef

```python
# GetCollaborationOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetCollaborationOutputTypeDef


def get_value() -> GetCollaborationOutputTypeDef:
    return {
        "collaboration": ...,
    }


# GetCollaborationOutputTypeDef definition

class GetCollaborationOutputTypeDef(TypedDict):
    collaboration: CollaborationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CollaborationTypeDef](./type_defs.md#collaborationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCollaborationOutputTypeDef

```python
# UpdateCollaborationOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import UpdateCollaborationOutputTypeDef


def get_value() -> UpdateCollaborationOutputTypeDef:
    return {
        "collaboration": ...,
    }


# UpdateCollaborationOutputTypeDef definition

class UpdateCollaborationOutputTypeDef(TypedDict):
    collaboration: CollaborationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CollaborationTypeDef](./type_defs.md#collaborationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReceiverConfigurationTypeDef

```python
# ReceiverConfigurationTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ReceiverConfigurationTypeDef


def get_value() -> ReceiverConfigurationTypeDef:
    return {
        "analysisType": ...,
    }


# ReceiverConfigurationTypeDef definition

class ReceiverConfigurationTypeDef(TypedDict):
    analysisType: AnalysisTypeType,  # (1)
    configurationDetails: NotRequired[ConfigurationDetailsTypeDef],  # (2)
```

1. See [:material-code-brackets: AnalysisTypeType](./literals.md#analysistypetype) 
2. See [:material-code-braces: ConfigurationDetailsTypeDef](./type_defs.md#configurationdetailstypedef) 
## ConfiguredTableAssociationAnalysisRulePolicyOutputTypeDef

```python
# ConfiguredTableAssociationAnalysisRulePolicyOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ConfiguredTableAssociationAnalysisRulePolicyOutputTypeDef


def get_value() -> ConfiguredTableAssociationAnalysisRulePolicyOutputTypeDef:
    return {
        "v1": ...,
    }


# ConfiguredTableAssociationAnalysisRulePolicyOutputTypeDef definition

class ConfiguredTableAssociationAnalysisRulePolicyOutputTypeDef(TypedDict):
    v1: NotRequired[ConfiguredTableAssociationAnalysisRulePolicyV1OutputTypeDef],  # (1)
```

1. See [:material-code-braces: ConfiguredTableAssociationAnalysisRulePolicyV1OutputTypeDef](./type_defs.md#configuredtableassociationanalysisrulepolicyv1outputtypedef) 
## ConfiguredTableAssociationAnalysisRulePolicyTypeDef

```python
# ConfiguredTableAssociationAnalysisRulePolicyTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ConfiguredTableAssociationAnalysisRulePolicyTypeDef


def get_value() -> ConfiguredTableAssociationAnalysisRulePolicyTypeDef:
    return {
        "v1": ...,
    }


# ConfiguredTableAssociationAnalysisRulePolicyTypeDef definition

class ConfiguredTableAssociationAnalysisRulePolicyTypeDef(TypedDict):
    v1: NotRequired[ConfiguredTableAssociationAnalysisRulePolicyV1TypeDef],  # (1)
```

1. See [:material-code-braces: ConfiguredTableAssociationAnalysisRulePolicyV1TypeDef](./type_defs.md#configuredtableassociationanalysisrulepolicyv1typedef) 
## ListIdMappingTablesOutputTypeDef

```python
# ListIdMappingTablesOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListIdMappingTablesOutputTypeDef


def get_value() -> ListIdMappingTablesOutputTypeDef:
    return {
        "idMappingTableSummaries": ...,
    }


# ListIdMappingTablesOutputTypeDef definition

class ListIdMappingTablesOutputTypeDef(TypedDict):
    idMappingTableSummaries: List[IdMappingTableSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: IdMappingTableSummaryTypeDef](./type_defs.md#idmappingtablesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AnalysisRuleCustomOutputTypeDef

```python
# AnalysisRuleCustomOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import AnalysisRuleCustomOutputTypeDef


def get_value() -> AnalysisRuleCustomOutputTypeDef:
    return {
        "allowedAnalyses": ...,
    }


# AnalysisRuleCustomOutputTypeDef definition

class AnalysisRuleCustomOutputTypeDef(TypedDict):
    allowedAnalyses: List[str],
    allowedAnalysisProviders: NotRequired[List[str]],
    additionalAnalyses: NotRequired[AdditionalAnalysesType],  # (1)
    disallowedOutputColumns: NotRequired[List[str]],
    differentialPrivacy: NotRequired[DifferentialPrivacyConfigurationOutputTypeDef],  # (2)
```

1. See [:material-code-brackets: AdditionalAnalysesType](./literals.md#additionalanalysestype) 
2. See [:material-code-braces: DifferentialPrivacyConfigurationOutputTypeDef](./type_defs.md#differentialprivacyconfigurationoutputtypedef) 
## AnalysisRuleCustomTypeDef

```python
# AnalysisRuleCustomTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import AnalysisRuleCustomTypeDef


def get_value() -> AnalysisRuleCustomTypeDef:
    return {
        "allowedAnalyses": ...,
    }


# AnalysisRuleCustomTypeDef definition

class AnalysisRuleCustomTypeDef(TypedDict):
    allowedAnalyses: Sequence[str],
    allowedAnalysisProviders: NotRequired[Sequence[str]],
    additionalAnalyses: NotRequired[AdditionalAnalysesType],  # (1)
    disallowedOutputColumns: NotRequired[Sequence[str]],
    differentialPrivacy: NotRequired[DifferentialPrivacyConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: AdditionalAnalysesType](./literals.md#additionalanalysestype) 
2. See [:material-code-braces: DifferentialPrivacyConfigurationTypeDef](./type_defs.md#differentialprivacyconfigurationtypedef) 
## PrivacyImpactTypeDef

```python
# PrivacyImpactTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import PrivacyImpactTypeDef


def get_value() -> PrivacyImpactTypeDef:
    return {
        "differentialPrivacy": ...,
    }


# PrivacyImpactTypeDef definition

class PrivacyImpactTypeDef(TypedDict):
    differentialPrivacy: NotRequired[DifferentialPrivacyPrivacyImpactTypeDef],  # (1)
```

1. See [:material-code-braces: DifferentialPrivacyPrivacyImpactTypeDef](./type_defs.md#differentialprivacyprivacyimpacttypedef) 
## PreviewPrivacyImpactInputTypeDef

```python
# PreviewPrivacyImpactInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import PreviewPrivacyImpactInputTypeDef


def get_value() -> PreviewPrivacyImpactInputTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# PreviewPrivacyImpactInputTypeDef definition

class PreviewPrivacyImpactInputTypeDef(TypedDict):
    membershipIdentifier: str,
    parameters: PreviewPrivacyImpactParametersInputTypeDef,  # (1)
```

1. See [:material-code-braces: PreviewPrivacyImpactParametersInputTypeDef](./type_defs.md#previewprivacyimpactparametersinputtypedef) 
## PrivacyBudgetTypeDef

```python
# PrivacyBudgetTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import PrivacyBudgetTypeDef


def get_value() -> PrivacyBudgetTypeDef:
    return {
        "differentialPrivacy": ...,
    }


# PrivacyBudgetTypeDef definition

class PrivacyBudgetTypeDef(TypedDict):
    differentialPrivacy: NotRequired[DifferentialPrivacyPrivacyBudgetTypeDef],  # (1)
```

1. See [:material-code-braces: DifferentialPrivacyPrivacyBudgetTypeDef](./type_defs.md#differentialprivacyprivacybudgettypedef) 
## CreatePrivacyBudgetTemplateInputTypeDef

```python
# CreatePrivacyBudgetTemplateInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CreatePrivacyBudgetTemplateInputTypeDef


def get_value() -> CreatePrivacyBudgetTemplateInputTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# CreatePrivacyBudgetTemplateInputTypeDef definition

class CreatePrivacyBudgetTemplateInputTypeDef(TypedDict):
    membershipIdentifier: str,
    autoRefresh: PrivacyBudgetTemplateAutoRefreshType,  # (1)
    privacyBudgetType: PrivacyBudgetTypeType,  # (2)
    parameters: PrivacyBudgetTemplateParametersInputTypeDef,  # (3)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: PrivacyBudgetTemplateAutoRefreshType](./literals.md#privacybudgettemplateautorefreshtype) 
2. See [:material-code-brackets: PrivacyBudgetTypeType](./literals.md#privacybudgettypetype) 
3. See [:material-code-braces: PrivacyBudgetTemplateParametersInputTypeDef](./type_defs.md#privacybudgettemplateparametersinputtypedef) 
## CollaborationPrivacyBudgetTemplateTypeDef

```python
# CollaborationPrivacyBudgetTemplateTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CollaborationPrivacyBudgetTemplateTypeDef


def get_value() -> CollaborationPrivacyBudgetTemplateTypeDef:
    return {
        "id": ...,
    }


# CollaborationPrivacyBudgetTemplateTypeDef definition

class CollaborationPrivacyBudgetTemplateTypeDef(TypedDict):
    id: str,
    arn: str,
    collaborationId: str,
    collaborationArn: str,
    creatorAccountId: str,
    createTime: datetime,
    updateTime: datetime,
    privacyBudgetType: PrivacyBudgetTypeType,  # (1)
    autoRefresh: PrivacyBudgetTemplateAutoRefreshType,  # (2)
    parameters: PrivacyBudgetTemplateParametersOutputTypeDef,  # (3)
```

1. See [:material-code-brackets: PrivacyBudgetTypeType](./literals.md#privacybudgettypetype) 
2. See [:material-code-brackets: PrivacyBudgetTemplateAutoRefreshType](./literals.md#privacybudgettemplateautorefreshtype) 
3. See [:material-code-braces: PrivacyBudgetTemplateParametersOutputTypeDef](./type_defs.md#privacybudgettemplateparametersoutputtypedef) 
## PrivacyBudgetTemplateTypeDef

```python
# PrivacyBudgetTemplateTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import PrivacyBudgetTemplateTypeDef


def get_value() -> PrivacyBudgetTemplateTypeDef:
    return {
        "id": ...,
    }


# PrivacyBudgetTemplateTypeDef definition

class PrivacyBudgetTemplateTypeDef(TypedDict):
    id: str,
    arn: str,
    membershipId: str,
    membershipArn: str,
    collaborationId: str,
    collaborationArn: str,
    createTime: datetime,
    updateTime: datetime,
    privacyBudgetType: PrivacyBudgetTypeType,  # (1)
    autoRefresh: PrivacyBudgetTemplateAutoRefreshType,  # (2)
    parameters: PrivacyBudgetTemplateParametersOutputTypeDef,  # (3)
```

1. See [:material-code-brackets: PrivacyBudgetTypeType](./literals.md#privacybudgettypetype) 
2. See [:material-code-brackets: PrivacyBudgetTemplateAutoRefreshType](./literals.md#privacybudgettemplateautorefreshtype) 
3. See [:material-code-braces: PrivacyBudgetTemplateParametersOutputTypeDef](./type_defs.md#privacybudgettemplateparametersoutputtypedef) 
## UpdatePrivacyBudgetTemplateInputTypeDef

```python
# UpdatePrivacyBudgetTemplateInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import UpdatePrivacyBudgetTemplateInputTypeDef


def get_value() -> UpdatePrivacyBudgetTemplateInputTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# UpdatePrivacyBudgetTemplateInputTypeDef definition

class UpdatePrivacyBudgetTemplateInputTypeDef(TypedDict):
    membershipIdentifier: str,
    privacyBudgetTemplateIdentifier: str,
    privacyBudgetType: PrivacyBudgetTypeType,  # (1)
    parameters: NotRequired[PrivacyBudgetTemplateUpdateParametersTypeDef],  # (2)
```

1. See [:material-code-brackets: PrivacyBudgetTypeType](./literals.md#privacybudgettypetype) 
2. See [:material-code-braces: PrivacyBudgetTemplateUpdateParametersTypeDef](./type_defs.md#privacybudgettemplateupdateparameterstypedef) 
## IdMappingTableTypeDef

```python
# IdMappingTableTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import IdMappingTableTypeDef


def get_value() -> IdMappingTableTypeDef:
    return {
        "id": ...,
    }


# IdMappingTableTypeDef definition

class IdMappingTableTypeDef(TypedDict):
    id: str,
    arn: str,
    inputReferenceConfig: IdMappingTableInputReferenceConfigTypeDef,  # (1)
    membershipId: str,
    membershipArn: str,
    collaborationId: str,
    collaborationArn: str,
    name: str,
    createTime: datetime,
    updateTime: datetime,
    inputReferenceProperties: IdMappingTableInputReferencePropertiesTypeDef,  # (2)
    description: NotRequired[str],
    kmsKeyArn: NotRequired[str],
```

1. See [:material-code-braces: IdMappingTableInputReferenceConfigTypeDef](./type_defs.md#idmappingtableinputreferenceconfigtypedef) 
2. See [:material-code-braces: IdMappingTableInputReferencePropertiesTypeDef](./type_defs.md#idmappingtableinputreferencepropertiestypedef) 
## SchemaTypePropertiesTypeDef

```python
# SchemaTypePropertiesTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import SchemaTypePropertiesTypeDef


def get_value() -> SchemaTypePropertiesTypeDef:
    return {
        "idMappingTable": ...,
    }


# SchemaTypePropertiesTypeDef definition

class SchemaTypePropertiesTypeDef(TypedDict):
    idMappingTable: NotRequired[IdMappingTableSchemaTypePropertiesTypeDef],  # (1)
```

1. See [:material-code-braces: IdMappingTableSchemaTypePropertiesTypeDef](./type_defs.md#idmappingtableschematypepropertiestypedef) 
## PaymentConfigurationTypeDef

```python
# PaymentConfigurationTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import PaymentConfigurationTypeDef


def get_value() -> PaymentConfigurationTypeDef:
    return {
        "queryCompute": ...,
    }


# PaymentConfigurationTypeDef definition

class PaymentConfigurationTypeDef(TypedDict):
    queryCompute: QueryComputePaymentConfigTypeDef,  # (1)
    machineLearning: NotRequired[MLPaymentConfigTypeDef],  # (2)
```

1. See [:material-code-braces: QueryComputePaymentConfigTypeDef](./type_defs.md#querycomputepaymentconfigtypedef) 
2. See [:material-code-braces: MLPaymentConfigTypeDef](./type_defs.md#mlpaymentconfigtypedef) 
## MembershipPaymentConfigurationTypeDef

```python
# MembershipPaymentConfigurationTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import MembershipPaymentConfigurationTypeDef


def get_value() -> MembershipPaymentConfigurationTypeDef:
    return {
        "queryCompute": ...,
    }


# MembershipPaymentConfigurationTypeDef definition

class MembershipPaymentConfigurationTypeDef(TypedDict):
    queryCompute: MembershipQueryComputePaymentConfigTypeDef,  # (1)
    machineLearning: NotRequired[MembershipMLPaymentConfigTypeDef],  # (2)
```

1. See [:material-code-braces: MembershipQueryComputePaymentConfigTypeDef](./type_defs.md#membershipquerycomputepaymentconfigtypedef) 
2. See [:material-code-braces: MembershipMLPaymentConfigTypeDef](./type_defs.md#membershipmlpaymentconfigtypedef) 
## MembershipProtectedQueryResultConfigurationTypeDef

```python
# MembershipProtectedQueryResultConfigurationTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import MembershipProtectedQueryResultConfigurationTypeDef


def get_value() -> MembershipProtectedQueryResultConfigurationTypeDef:
    return {
        "outputConfiguration": ...,
    }


# MembershipProtectedQueryResultConfigurationTypeDef definition

class MembershipProtectedQueryResultConfigurationTypeDef(TypedDict):
    outputConfiguration: MembershipProtectedQueryOutputConfigurationTypeDef,  # (1)
    roleArn: NotRequired[str],
```

1. See [:material-code-braces: MembershipProtectedQueryOutputConfigurationTypeDef](./type_defs.md#membershipprotectedqueryoutputconfigurationtypedef) 
## ProtectedQueryResultConfigurationTypeDef

```python
# ProtectedQueryResultConfigurationTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ProtectedQueryResultConfigurationTypeDef


def get_value() -> ProtectedQueryResultConfigurationTypeDef:
    return {
        "outputConfiguration": ...,
    }


# ProtectedQueryResultConfigurationTypeDef definition

class ProtectedQueryResultConfigurationTypeDef(TypedDict):
    outputConfiguration: ProtectedQueryOutputConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: ProtectedQueryOutputConfigurationTypeDef](./type_defs.md#protectedqueryoutputconfigurationtypedef) 
## ProtectedQueryResultTypeDef

```python
# ProtectedQueryResultTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ProtectedQueryResultTypeDef


def get_value() -> ProtectedQueryResultTypeDef:
    return {
        "output": ...,
    }


# ProtectedQueryResultTypeDef definition

class ProtectedQueryResultTypeDef(TypedDict):
    output: ProtectedQueryOutputTypeDef,  # (1)
```

1. See [:material-code-braces: ProtectedQueryOutputTypeDef](./type_defs.md#protectedqueryoutputtypedef) 
## AnalysisRuleIdMappingTableTypeDef

```python
# AnalysisRuleIdMappingTableTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import AnalysisRuleIdMappingTableTypeDef


def get_value() -> AnalysisRuleIdMappingTableTypeDef:
    return {
        "joinColumns": ...,
    }


# AnalysisRuleIdMappingTableTypeDef definition

class AnalysisRuleIdMappingTableTypeDef(TypedDict):
    joinColumns: List[str],
    queryConstraints: List[QueryConstraintTypeDef],  # (1)
    dimensionColumns: NotRequired[List[str]],
```

1. See [:material-code-braces: QueryConstraintTypeDef](./type_defs.md#queryconstrainttypedef) 
## SnowflakeTableReferenceOutputTypeDef

```python
# SnowflakeTableReferenceOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import SnowflakeTableReferenceOutputTypeDef


def get_value() -> SnowflakeTableReferenceOutputTypeDef:
    return {
        "secretArn": ...,
    }


# SnowflakeTableReferenceOutputTypeDef definition

class SnowflakeTableReferenceOutputTypeDef(TypedDict):
    secretArn: str,
    accountIdentifier: str,
    databaseName: str,
    tableName: str,
    schemaName: str,
    tableSchema: SnowflakeTableSchemaOutputTypeDef,  # (1)
```

1. See [:material-code-braces: SnowflakeTableSchemaOutputTypeDef](./type_defs.md#snowflaketableschemaoutputtypedef) 
## SnowflakeTableReferenceTypeDef

```python
# SnowflakeTableReferenceTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import SnowflakeTableReferenceTypeDef


def get_value() -> SnowflakeTableReferenceTypeDef:
    return {
        "secretArn": ...,
    }


# SnowflakeTableReferenceTypeDef definition

class SnowflakeTableReferenceTypeDef(TypedDict):
    secretArn: str,
    accountIdentifier: str,
    databaseName: str,
    tableName: str,
    schemaName: str,
    tableSchema: SnowflakeTableSchemaTypeDef,  # (1)
```

1. See [:material-code-braces: SnowflakeTableSchemaTypeDef](./type_defs.md#snowflaketableschematypedef) 
## CreateAnalysisTemplateOutputTypeDef

```python
# CreateAnalysisTemplateOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CreateAnalysisTemplateOutputTypeDef


def get_value() -> CreateAnalysisTemplateOutputTypeDef:
    return {
        "analysisTemplate": ...,
    }


# CreateAnalysisTemplateOutputTypeDef definition

class CreateAnalysisTemplateOutputTypeDef(TypedDict):
    analysisTemplate: AnalysisTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalysisTemplateTypeDef](./type_defs.md#analysistemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAnalysisTemplateOutputTypeDef

```python
# GetAnalysisTemplateOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetAnalysisTemplateOutputTypeDef


def get_value() -> GetAnalysisTemplateOutputTypeDef:
    return {
        "analysisTemplate": ...,
    }


# GetAnalysisTemplateOutputTypeDef definition

class GetAnalysisTemplateOutputTypeDef(TypedDict):
    analysisTemplate: AnalysisTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalysisTemplateTypeDef](./type_defs.md#analysistemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAnalysisTemplateOutputTypeDef

```python
# UpdateAnalysisTemplateOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import UpdateAnalysisTemplateOutputTypeDef


def get_value() -> UpdateAnalysisTemplateOutputTypeDef:
    return {
        "analysisTemplate": ...,
    }


# UpdateAnalysisTemplateOutputTypeDef definition

class UpdateAnalysisTemplateOutputTypeDef(TypedDict):
    analysisTemplate: AnalysisTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalysisTemplateTypeDef](./type_defs.md#analysistemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetCollaborationAnalysisTemplateOutputTypeDef

```python
# BatchGetCollaborationAnalysisTemplateOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import BatchGetCollaborationAnalysisTemplateOutputTypeDef


def get_value() -> BatchGetCollaborationAnalysisTemplateOutputTypeDef:
    return {
        "collaborationAnalysisTemplates": ...,
    }


# BatchGetCollaborationAnalysisTemplateOutputTypeDef definition

class BatchGetCollaborationAnalysisTemplateOutputTypeDef(TypedDict):
    collaborationAnalysisTemplates: List[CollaborationAnalysisTemplateTypeDef],  # (1)
    errors: List[BatchGetCollaborationAnalysisTemplateErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: CollaborationAnalysisTemplateTypeDef](./type_defs.md#collaborationanalysistemplatetypedef) 
2. See [:material-code-braces: BatchGetCollaborationAnalysisTemplateErrorTypeDef](./type_defs.md#batchgetcollaborationanalysistemplateerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCollaborationAnalysisTemplateOutputTypeDef

```python
# GetCollaborationAnalysisTemplateOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetCollaborationAnalysisTemplateOutputTypeDef


def get_value() -> GetCollaborationAnalysisTemplateOutputTypeDef:
    return {
        "collaborationAnalysisTemplate": ...,
    }


# GetCollaborationAnalysisTemplateOutputTypeDef definition

class GetCollaborationAnalysisTemplateOutputTypeDef(TypedDict):
    collaborationAnalysisTemplate: CollaborationAnalysisTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CollaborationAnalysisTemplateTypeDef](./type_defs.md#collaborationanalysistemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProtectedQuerySummaryTypeDef

```python
# ProtectedQuerySummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ProtectedQuerySummaryTypeDef


def get_value() -> ProtectedQuerySummaryTypeDef:
    return {
        "id": ...,
    }


# ProtectedQuerySummaryTypeDef definition

class ProtectedQuerySummaryTypeDef(TypedDict):
    id: str,
    membershipId: str,
    membershipArn: str,
    createTime: datetime,
    status: ProtectedQueryStatusType,  # (1)
    receiverConfigurations: List[ReceiverConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: ProtectedQueryStatusType](./literals.md#protectedquerystatustype) 
2. See [:material-code-braces: ReceiverConfigurationTypeDef](./type_defs.md#receiverconfigurationtypedef) 
## ConfiguredTableAssociationAnalysisRuleTypeDef

```python
# ConfiguredTableAssociationAnalysisRuleTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ConfiguredTableAssociationAnalysisRuleTypeDef


def get_value() -> ConfiguredTableAssociationAnalysisRuleTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# ConfiguredTableAssociationAnalysisRuleTypeDef definition

class ConfiguredTableAssociationAnalysisRuleTypeDef(TypedDict):
    membershipIdentifier: str,
    configuredTableAssociationId: str,
    configuredTableAssociationArn: str,
    policy: ConfiguredTableAssociationAnalysisRulePolicyOutputTypeDef,  # (1)
    type: ConfiguredTableAssociationAnalysisRuleTypeType,  # (2)
    createTime: datetime,
    updateTime: datetime,
```

1. See [:material-code-braces: ConfiguredTableAssociationAnalysisRulePolicyOutputTypeDef](./type_defs.md#configuredtableassociationanalysisrulepolicyoutputtypedef) 
2. See [:material-code-brackets: ConfiguredTableAssociationAnalysisRuleTypeType](./literals.md#configuredtableassociationanalysisruletypetype) 
## ConfiguredTableAnalysisRulePolicyV1OutputTypeDef

```python
# ConfiguredTableAnalysisRulePolicyV1OutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ConfiguredTableAnalysisRulePolicyV1OutputTypeDef


def get_value() -> ConfiguredTableAnalysisRulePolicyV1OutputTypeDef:
    return {
        "list": ...,
    }


# ConfiguredTableAnalysisRulePolicyV1OutputTypeDef definition

class ConfiguredTableAnalysisRulePolicyV1OutputTypeDef(TypedDict):
    list: NotRequired[AnalysisRuleListOutputTypeDef],  # (1)
    aggregation: NotRequired[AnalysisRuleAggregationOutputTypeDef],  # (2)
    custom: NotRequired[AnalysisRuleCustomOutputTypeDef],  # (3)
```

1. See [:material-code-braces: AnalysisRuleListOutputTypeDef](./type_defs.md#analysisrulelistoutputtypedef) 
2. See [:material-code-braces: AnalysisRuleAggregationOutputTypeDef](./type_defs.md#analysisruleaggregationoutputtypedef) 
3. See [:material-code-braces: AnalysisRuleCustomOutputTypeDef](./type_defs.md#analysisrulecustomoutputtypedef) 
## ConfiguredTableAnalysisRulePolicyV1TypeDef

```python
# ConfiguredTableAnalysisRulePolicyV1TypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ConfiguredTableAnalysisRulePolicyV1TypeDef


def get_value() -> ConfiguredTableAnalysisRulePolicyV1TypeDef:
    return {
        "list": ...,
    }


# ConfiguredTableAnalysisRulePolicyV1TypeDef definition

class ConfiguredTableAnalysisRulePolicyV1TypeDef(TypedDict):
    list: NotRequired[AnalysisRuleListTypeDef],  # (1)
    aggregation: NotRequired[AnalysisRuleAggregationTypeDef],  # (2)
    custom: NotRequired[AnalysisRuleCustomTypeDef],  # (3)
```

1. See [:material-code-braces: AnalysisRuleListTypeDef](./type_defs.md#analysisrulelisttypedef) 
2. See [:material-code-braces: AnalysisRuleAggregationTypeDef](./type_defs.md#analysisruleaggregationtypedef) 
3. See [:material-code-braces: AnalysisRuleCustomTypeDef](./type_defs.md#analysisrulecustomtypedef) 
## PreviewPrivacyImpactOutputTypeDef

```python
# PreviewPrivacyImpactOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import PreviewPrivacyImpactOutputTypeDef


def get_value() -> PreviewPrivacyImpactOutputTypeDef:
    return {
        "privacyImpact": ...,
    }


# PreviewPrivacyImpactOutputTypeDef definition

class PreviewPrivacyImpactOutputTypeDef(TypedDict):
    privacyImpact: PrivacyImpactTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PrivacyImpactTypeDef](./type_defs.md#privacyimpacttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CollaborationPrivacyBudgetSummaryTypeDef

```python
# CollaborationPrivacyBudgetSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CollaborationPrivacyBudgetSummaryTypeDef


def get_value() -> CollaborationPrivacyBudgetSummaryTypeDef:
    return {
        "id": ...,
    }


# CollaborationPrivacyBudgetSummaryTypeDef definition

class CollaborationPrivacyBudgetSummaryTypeDef(TypedDict):
    id: str,
    privacyBudgetTemplateId: str,
    privacyBudgetTemplateArn: str,
    collaborationId: str,
    collaborationArn: str,
    creatorAccountId: str,
    type: PrivacyBudgetTypeType,  # (1)
    createTime: datetime,
    updateTime: datetime,
    budget: PrivacyBudgetTypeDef,  # (2)
```

1. See [:material-code-brackets: PrivacyBudgetTypeType](./literals.md#privacybudgettypetype) 
2. See [:material-code-braces: PrivacyBudgetTypeDef](./type_defs.md#privacybudgettypedef) 
## PrivacyBudgetSummaryTypeDef

```python
# PrivacyBudgetSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import PrivacyBudgetSummaryTypeDef


def get_value() -> PrivacyBudgetSummaryTypeDef:
    return {
        "id": ...,
    }


# PrivacyBudgetSummaryTypeDef definition

class PrivacyBudgetSummaryTypeDef(TypedDict):
    id: str,
    privacyBudgetTemplateId: str,
    privacyBudgetTemplateArn: str,
    membershipId: str,
    membershipArn: str,
    collaborationId: str,
    collaborationArn: str,
    type: PrivacyBudgetTypeType,  # (1)
    createTime: datetime,
    updateTime: datetime,
    budget: PrivacyBudgetTypeDef,  # (2)
```

1. See [:material-code-brackets: PrivacyBudgetTypeType](./literals.md#privacybudgettypetype) 
2. See [:material-code-braces: PrivacyBudgetTypeDef](./type_defs.md#privacybudgettypedef) 
## GetCollaborationPrivacyBudgetTemplateOutputTypeDef

```python
# GetCollaborationPrivacyBudgetTemplateOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetCollaborationPrivacyBudgetTemplateOutputTypeDef


def get_value() -> GetCollaborationPrivacyBudgetTemplateOutputTypeDef:
    return {
        "collaborationPrivacyBudgetTemplate": ...,
    }


# GetCollaborationPrivacyBudgetTemplateOutputTypeDef definition

class GetCollaborationPrivacyBudgetTemplateOutputTypeDef(TypedDict):
    collaborationPrivacyBudgetTemplate: CollaborationPrivacyBudgetTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CollaborationPrivacyBudgetTemplateTypeDef](./type_defs.md#collaborationprivacybudgettemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePrivacyBudgetTemplateOutputTypeDef

```python
# CreatePrivacyBudgetTemplateOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CreatePrivacyBudgetTemplateOutputTypeDef


def get_value() -> CreatePrivacyBudgetTemplateOutputTypeDef:
    return {
        "privacyBudgetTemplate": ...,
    }


# CreatePrivacyBudgetTemplateOutputTypeDef definition

class CreatePrivacyBudgetTemplateOutputTypeDef(TypedDict):
    privacyBudgetTemplate: PrivacyBudgetTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PrivacyBudgetTemplateTypeDef](./type_defs.md#privacybudgettemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPrivacyBudgetTemplateOutputTypeDef

```python
# GetPrivacyBudgetTemplateOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetPrivacyBudgetTemplateOutputTypeDef


def get_value() -> GetPrivacyBudgetTemplateOutputTypeDef:
    return {
        "privacyBudgetTemplate": ...,
    }


# GetPrivacyBudgetTemplateOutputTypeDef definition

class GetPrivacyBudgetTemplateOutputTypeDef(TypedDict):
    privacyBudgetTemplate: PrivacyBudgetTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PrivacyBudgetTemplateTypeDef](./type_defs.md#privacybudgettemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePrivacyBudgetTemplateOutputTypeDef

```python
# UpdatePrivacyBudgetTemplateOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import UpdatePrivacyBudgetTemplateOutputTypeDef


def get_value() -> UpdatePrivacyBudgetTemplateOutputTypeDef:
    return {
        "privacyBudgetTemplate": ...,
    }


# UpdatePrivacyBudgetTemplateOutputTypeDef definition

class UpdatePrivacyBudgetTemplateOutputTypeDef(TypedDict):
    privacyBudgetTemplate: PrivacyBudgetTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PrivacyBudgetTemplateTypeDef](./type_defs.md#privacybudgettemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateIdMappingTableOutputTypeDef

```python
# CreateIdMappingTableOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CreateIdMappingTableOutputTypeDef


def get_value() -> CreateIdMappingTableOutputTypeDef:
    return {
        "idMappingTable": ...,
    }


# CreateIdMappingTableOutputTypeDef definition

class CreateIdMappingTableOutputTypeDef(TypedDict):
    idMappingTable: IdMappingTableTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdMappingTableTypeDef](./type_defs.md#idmappingtabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIdMappingTableOutputTypeDef

```python
# GetIdMappingTableOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetIdMappingTableOutputTypeDef


def get_value() -> GetIdMappingTableOutputTypeDef:
    return {
        "idMappingTable": ...,
    }


# GetIdMappingTableOutputTypeDef definition

class GetIdMappingTableOutputTypeDef(TypedDict):
    idMappingTable: IdMappingTableTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdMappingTableTypeDef](./type_defs.md#idmappingtabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateIdMappingTableOutputTypeDef

```python
# UpdateIdMappingTableOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import UpdateIdMappingTableOutputTypeDef


def get_value() -> UpdateIdMappingTableOutputTypeDef:
    return {
        "idMappingTable": ...,
    }


# UpdateIdMappingTableOutputTypeDef definition

class UpdateIdMappingTableOutputTypeDef(TypedDict):
    idMappingTable: IdMappingTableTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdMappingTableTypeDef](./type_defs.md#idmappingtabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SchemaTypeDef

```python
# SchemaTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import SchemaTypeDef


def get_value() -> SchemaTypeDef:
    return {
        "columns": ...,
    }


# SchemaTypeDef definition

class SchemaTypeDef(TypedDict):
    columns: List[ColumnTypeDef],  # (1)
    partitionKeys: List[ColumnTypeDef],  # (1)
    analysisRuleTypes: List[AnalysisRuleTypeType],  # (3)
    creatorAccountId: str,
    name: str,
    collaborationId: str,
    collaborationArn: str,
    description: str,
    createTime: datetime,
    updateTime: datetime,
    type: SchemaTypeType,  # (5)
    schemaStatusDetails: List[SchemaStatusDetailTypeDef],  # (6)
    analysisMethod: NotRequired[AnalysisMethodType],  # (4)
    schemaTypeProperties: NotRequired[SchemaTypePropertiesTypeDef],  # (7)
```

1. See [:material-code-braces: ColumnTypeDef](./type_defs.md#columntypedef) 
2. See [:material-code-braces: ColumnTypeDef](./type_defs.md#columntypedef) 
3. See [:material-code-brackets: AnalysisRuleTypeType](./literals.md#analysisruletypetype) 
4. See [:material-code-brackets: AnalysisMethodType](./literals.md#analysismethodtype) 
5. See [:material-code-brackets: SchemaTypeType](./literals.md#schematypetype) 
6. See [:material-code-braces: SchemaStatusDetailTypeDef](./type_defs.md#schemastatusdetailtypedef) 
7. See [:material-code-braces: SchemaTypePropertiesTypeDef](./type_defs.md#schematypepropertiestypedef) 
## MemberSpecificationTypeDef

```python
# MemberSpecificationTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import MemberSpecificationTypeDef


def get_value() -> MemberSpecificationTypeDef:
    return {
        "accountId": ...,
    }


# MemberSpecificationTypeDef definition

class MemberSpecificationTypeDef(TypedDict):
    accountId: str,
    memberAbilities: Sequence[MemberAbilityType],  # (1)
    displayName: str,
    mlMemberAbilities: NotRequired[MLMemberAbilitiesUnionTypeDef],  # (2)
    paymentConfiguration: NotRequired[PaymentConfigurationTypeDef],  # (3)
```

1. See [:material-code-brackets: MemberAbilityType](./literals.md#memberabilitytype) 
2. See [:material-code-braces: MLMemberAbilitiesTypeDef](./type_defs.md#mlmemberabilitiestypedef) [:material-code-braces: MLMemberAbilitiesOutputTypeDef](./type_defs.md#mlmemberabilitiesoutputtypedef) 
3. See [:material-code-braces: PaymentConfigurationTypeDef](./type_defs.md#paymentconfigurationtypedef) 
## MemberSummaryTypeDef

```python
# MemberSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import MemberSummaryTypeDef


def get_value() -> MemberSummaryTypeDef:
    return {
        "accountId": ...,
    }


# MemberSummaryTypeDef definition

class MemberSummaryTypeDef(TypedDict):
    accountId: str,
    status: MemberStatusType,  # (1)
    displayName: str,
    abilities: List[MemberAbilityType],  # (2)
    createTime: datetime,
    updateTime: datetime,
    paymentConfiguration: PaymentConfigurationTypeDef,  # (4)
    mlAbilities: NotRequired[MLMemberAbilitiesOutputTypeDef],  # (3)
    membershipId: NotRequired[str],
    membershipArn: NotRequired[str],
```

1. See [:material-code-brackets: MemberStatusType](./literals.md#memberstatustype) 
2. See [:material-code-brackets: MemberAbilityType](./literals.md#memberabilitytype) 
3. See [:material-code-braces: MLMemberAbilitiesOutputTypeDef](./type_defs.md#mlmemberabilitiesoutputtypedef) 
4. See [:material-code-braces: PaymentConfigurationTypeDef](./type_defs.md#paymentconfigurationtypedef) 
## MembershipSummaryTypeDef

```python
# MembershipSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import MembershipSummaryTypeDef


def get_value() -> MembershipSummaryTypeDef:
    return {
        "id": ...,
    }


# MembershipSummaryTypeDef definition

class MembershipSummaryTypeDef(TypedDict):
    id: str,
    arn: str,
    collaborationArn: str,
    collaborationId: str,
    collaborationCreatorAccountId: str,
    collaborationCreatorDisplayName: str,
    collaborationName: str,
    createTime: datetime,
    updateTime: datetime,
    status: MembershipStatusType,  # (1)
    memberAbilities: List[MemberAbilityType],  # (2)
    paymentConfiguration: MembershipPaymentConfigurationTypeDef,  # (4)
    mlMemberAbilities: NotRequired[MLMemberAbilitiesOutputTypeDef],  # (3)
```

1. See [:material-code-brackets: MembershipStatusType](./literals.md#membershipstatustype) 
2. See [:material-code-brackets: MemberAbilityType](./literals.md#memberabilitytype) 
3. See [:material-code-braces: MLMemberAbilitiesOutputTypeDef](./type_defs.md#mlmemberabilitiesoutputtypedef) 
4. See [:material-code-braces: MembershipPaymentConfigurationTypeDef](./type_defs.md#membershippaymentconfigurationtypedef) 
## CreateMembershipInputTypeDef

```python
# CreateMembershipInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CreateMembershipInputTypeDef


def get_value() -> CreateMembershipInputTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# CreateMembershipInputTypeDef definition

class CreateMembershipInputTypeDef(TypedDict):
    collaborationIdentifier: str,
    queryLogStatus: MembershipQueryLogStatusType,  # (1)
    tags: NotRequired[Mapping[str, str]],
    defaultResultConfiguration: NotRequired[MembershipProtectedQueryResultConfigurationTypeDef],  # (2)
    paymentConfiguration: NotRequired[MembershipPaymentConfigurationTypeDef],  # (3)
```

1. See [:material-code-brackets: MembershipQueryLogStatusType](./literals.md#membershipquerylogstatustype) 
2. See [:material-code-braces: MembershipProtectedQueryResultConfigurationTypeDef](./type_defs.md#membershipprotectedqueryresultconfigurationtypedef) 
3. See [:material-code-braces: MembershipPaymentConfigurationTypeDef](./type_defs.md#membershippaymentconfigurationtypedef) 
## MembershipTypeDef

```python
# MembershipTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import MembershipTypeDef


def get_value() -> MembershipTypeDef:
    return {
        "id": ...,
    }


# MembershipTypeDef definition

class MembershipTypeDef(TypedDict):
    id: str,
    arn: str,
    collaborationArn: str,
    collaborationId: str,
    collaborationCreatorAccountId: str,
    collaborationCreatorDisplayName: str,
    collaborationName: str,
    createTime: datetime,
    updateTime: datetime,
    status: MembershipStatusType,  # (1)
    memberAbilities: List[MemberAbilityType],  # (2)
    queryLogStatus: MembershipQueryLogStatusType,  # (4)
    paymentConfiguration: MembershipPaymentConfigurationTypeDef,  # (6)
    mlMemberAbilities: NotRequired[MLMemberAbilitiesOutputTypeDef],  # (3)
    defaultResultConfiguration: NotRequired[MembershipProtectedQueryResultConfigurationTypeDef],  # (5)
```

1. See [:material-code-brackets: MembershipStatusType](./literals.md#membershipstatustype) 
2. See [:material-code-brackets: MemberAbilityType](./literals.md#memberabilitytype) 
3. See [:material-code-braces: MLMemberAbilitiesOutputTypeDef](./type_defs.md#mlmemberabilitiesoutputtypedef) 
4. See [:material-code-brackets: MembershipQueryLogStatusType](./literals.md#membershipquerylogstatustype) 
5. See [:material-code-braces: MembershipProtectedQueryResultConfigurationTypeDef](./type_defs.md#membershipprotectedqueryresultconfigurationtypedef) 
6. See [:material-code-braces: MembershipPaymentConfigurationTypeDef](./type_defs.md#membershippaymentconfigurationtypedef) 
## UpdateMembershipInputTypeDef

```python
# UpdateMembershipInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import UpdateMembershipInputTypeDef


def get_value() -> UpdateMembershipInputTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# UpdateMembershipInputTypeDef definition

class UpdateMembershipInputTypeDef(TypedDict):
    membershipIdentifier: str,
    queryLogStatus: NotRequired[MembershipQueryLogStatusType],  # (1)
    defaultResultConfiguration: NotRequired[MembershipProtectedQueryResultConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: MembershipQueryLogStatusType](./literals.md#membershipquerylogstatustype) 
2. See [:material-code-braces: MembershipProtectedQueryResultConfigurationTypeDef](./type_defs.md#membershipprotectedqueryresultconfigurationtypedef) 
## StartProtectedQueryInputTypeDef

```python
# StartProtectedQueryInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import StartProtectedQueryInputTypeDef


def get_value() -> StartProtectedQueryInputTypeDef:
    return {
        "type": ...,
    }


# StartProtectedQueryInputTypeDef definition

class StartProtectedQueryInputTypeDef(TypedDict):
    type: ProtectedQueryTypeType,  # (1)
    membershipIdentifier: str,
    sqlParameters: ProtectedQuerySQLParametersUnionTypeDef,  # (2)
    resultConfiguration: NotRequired[ProtectedQueryResultConfigurationTypeDef],  # (3)
    computeConfiguration: NotRequired[ComputeConfigurationTypeDef],  # (4)
```

1. See [:material-code-brackets: ProtectedQueryTypeType](./literals.md#protectedquerytypetype) 
2. See [:material-code-braces: ProtectedQuerySQLParametersTypeDef](./type_defs.md#protectedquerysqlparameterstypedef) [:material-code-braces: ProtectedQuerySQLParametersOutputTypeDef](./type_defs.md#protectedquerysqlparametersoutputtypedef) 
3. See [:material-code-braces: ProtectedQueryResultConfigurationTypeDef](./type_defs.md#protectedqueryresultconfigurationtypedef) 
4. See [:material-code-braces: ComputeConfigurationTypeDef](./type_defs.md#computeconfigurationtypedef) 
## ProtectedQueryTypeDef

```python
# ProtectedQueryTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ProtectedQueryTypeDef


def get_value() -> ProtectedQueryTypeDef:
    return {
        "id": ...,
    }


# ProtectedQueryTypeDef definition

class ProtectedQueryTypeDef(TypedDict):
    id: str,
    membershipId: str,
    membershipArn: str,
    createTime: datetime,
    status: ProtectedQueryStatusType,  # (2)
    sqlParameters: NotRequired[ProtectedQuerySQLParametersOutputTypeDef],  # (1)
    resultConfiguration: NotRequired[ProtectedQueryResultConfigurationTypeDef],  # (3)
    statistics: NotRequired[ProtectedQueryStatisticsTypeDef],  # (4)
    result: NotRequired[ProtectedQueryResultTypeDef],  # (5)
    error: NotRequired[ProtectedQueryErrorTypeDef],  # (6)
    differentialPrivacy: NotRequired[DifferentialPrivacyParametersTypeDef],  # (7)
    computeConfiguration: NotRequired[ComputeConfigurationTypeDef],  # (8)
```

1. See [:material-code-braces: ProtectedQuerySQLParametersOutputTypeDef](./type_defs.md#protectedquerysqlparametersoutputtypedef) 
2. See [:material-code-brackets: ProtectedQueryStatusType](./literals.md#protectedquerystatustype) 
3. See [:material-code-braces: ProtectedQueryResultConfigurationTypeDef](./type_defs.md#protectedqueryresultconfigurationtypedef) 
4. See [:material-code-braces: ProtectedQueryStatisticsTypeDef](./type_defs.md#protectedquerystatisticstypedef) 
5. See [:material-code-braces: ProtectedQueryResultTypeDef](./type_defs.md#protectedqueryresulttypedef) 
6. See [:material-code-braces: ProtectedQueryErrorTypeDef](./type_defs.md#protectedqueryerrortypedef) 
7. See [:material-code-braces: DifferentialPrivacyParametersTypeDef](./type_defs.md#differentialprivacyparameterstypedef) 
8. See [:material-code-braces: ComputeConfigurationTypeDef](./type_defs.md#computeconfigurationtypedef) 
## AnalysisRulePolicyV1TypeDef

```python
# AnalysisRulePolicyV1TypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import AnalysisRulePolicyV1TypeDef


def get_value() -> AnalysisRulePolicyV1TypeDef:
    return {
        "list": ...,
    }


# AnalysisRulePolicyV1TypeDef definition

class AnalysisRulePolicyV1TypeDef(TypedDict):
    list: NotRequired[AnalysisRuleListOutputTypeDef],  # (1)
    aggregation: NotRequired[AnalysisRuleAggregationOutputTypeDef],  # (2)
    custom: NotRequired[AnalysisRuleCustomOutputTypeDef],  # (3)
    idMappingTable: NotRequired[AnalysisRuleIdMappingTableTypeDef],  # (4)
```

1. See [:material-code-braces: AnalysisRuleListOutputTypeDef](./type_defs.md#analysisrulelistoutputtypedef) 
2. See [:material-code-braces: AnalysisRuleAggregationOutputTypeDef](./type_defs.md#analysisruleaggregationoutputtypedef) 
3. See [:material-code-braces: AnalysisRuleCustomOutputTypeDef](./type_defs.md#analysisrulecustomoutputtypedef) 
4. See [:material-code-braces: AnalysisRuleIdMappingTableTypeDef](./type_defs.md#analysisruleidmappingtabletypedef) 
## TableReferenceOutputTypeDef

```python
# TableReferenceOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import TableReferenceOutputTypeDef


def get_value() -> TableReferenceOutputTypeDef:
    return {
        "glue": ...,
    }


# TableReferenceOutputTypeDef definition

class TableReferenceOutputTypeDef(TypedDict):
    glue: NotRequired[GlueTableReferenceTypeDef],  # (1)
    snowflake: NotRequired[SnowflakeTableReferenceOutputTypeDef],  # (2)
    athena: NotRequired[AthenaTableReferenceTypeDef],  # (3)
```

1. See [:material-code-braces: GlueTableReferenceTypeDef](./type_defs.md#gluetablereferencetypedef) 
2. See [:material-code-braces: SnowflakeTableReferenceOutputTypeDef](./type_defs.md#snowflaketablereferenceoutputtypedef) 
3. See [:material-code-braces: AthenaTableReferenceTypeDef](./type_defs.md#athenatablereferencetypedef) 
## TableReferenceTypeDef

```python
# TableReferenceTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import TableReferenceTypeDef


def get_value() -> TableReferenceTypeDef:
    return {
        "glue": ...,
    }


# TableReferenceTypeDef definition

class TableReferenceTypeDef(TypedDict):
    glue: NotRequired[GlueTableReferenceTypeDef],  # (1)
    snowflake: NotRequired[SnowflakeTableReferenceTypeDef],  # (2)
    athena: NotRequired[AthenaTableReferenceTypeDef],  # (3)
```

1. See [:material-code-braces: GlueTableReferenceTypeDef](./type_defs.md#gluetablereferencetypedef) 
2. See [:material-code-braces: SnowflakeTableReferenceTypeDef](./type_defs.md#snowflaketablereferencetypedef) 
3. See [:material-code-braces: AthenaTableReferenceTypeDef](./type_defs.md#athenatablereferencetypedef) 
## ListProtectedQueriesOutputTypeDef

```python
# ListProtectedQueriesOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListProtectedQueriesOutputTypeDef


def get_value() -> ListProtectedQueriesOutputTypeDef:
    return {
        "nextToken": ...,
    }


# ListProtectedQueriesOutputTypeDef definition

class ListProtectedQueriesOutputTypeDef(TypedDict):
    protectedQueries: List[ProtectedQuerySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ProtectedQuerySummaryTypeDef](./type_defs.md#protectedquerysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConfiguredTableAssociationAnalysisRuleOutputTypeDef

```python
# CreateConfiguredTableAssociationAnalysisRuleOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CreateConfiguredTableAssociationAnalysisRuleOutputTypeDef


def get_value() -> CreateConfiguredTableAssociationAnalysisRuleOutputTypeDef:
    return {
        "analysisRule": ...,
    }


# CreateConfiguredTableAssociationAnalysisRuleOutputTypeDef definition

class CreateConfiguredTableAssociationAnalysisRuleOutputTypeDef(TypedDict):
    analysisRule: ConfiguredTableAssociationAnalysisRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableAssociationAnalysisRuleTypeDef](./type_defs.md#configuredtableassociationanalysisruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConfiguredTableAssociationAnalysisRuleOutputTypeDef

```python
# GetConfiguredTableAssociationAnalysisRuleOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetConfiguredTableAssociationAnalysisRuleOutputTypeDef


def get_value() -> GetConfiguredTableAssociationAnalysisRuleOutputTypeDef:
    return {
        "analysisRule": ...,
    }


# GetConfiguredTableAssociationAnalysisRuleOutputTypeDef definition

class GetConfiguredTableAssociationAnalysisRuleOutputTypeDef(TypedDict):
    analysisRule: ConfiguredTableAssociationAnalysisRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableAssociationAnalysisRuleTypeDef](./type_defs.md#configuredtableassociationanalysisruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateConfiguredTableAssociationAnalysisRuleOutputTypeDef

```python
# UpdateConfiguredTableAssociationAnalysisRuleOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import UpdateConfiguredTableAssociationAnalysisRuleOutputTypeDef


def get_value() -> UpdateConfiguredTableAssociationAnalysisRuleOutputTypeDef:
    return {
        "analysisRule": ...,
    }


# UpdateConfiguredTableAssociationAnalysisRuleOutputTypeDef definition

class UpdateConfiguredTableAssociationAnalysisRuleOutputTypeDef(TypedDict):
    analysisRule: ConfiguredTableAssociationAnalysisRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableAssociationAnalysisRuleTypeDef](./type_defs.md#configuredtableassociationanalysisruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConfiguredTableAssociationAnalysisRuleInputTypeDef

```python
# CreateConfiguredTableAssociationAnalysisRuleInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CreateConfiguredTableAssociationAnalysisRuleInputTypeDef


def get_value() -> CreateConfiguredTableAssociationAnalysisRuleInputTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# CreateConfiguredTableAssociationAnalysisRuleInputTypeDef definition

class CreateConfiguredTableAssociationAnalysisRuleInputTypeDef(TypedDict):
    membershipIdentifier: str,
    configuredTableAssociationIdentifier: str,
    analysisRuleType: ConfiguredTableAssociationAnalysisRuleTypeType,  # (1)
    analysisRulePolicy: ConfiguredTableAssociationAnalysisRulePolicyUnionTypeDef,  # (2)
```

1. See [:material-code-brackets: ConfiguredTableAssociationAnalysisRuleTypeType](./literals.md#configuredtableassociationanalysisruletypetype) 
2. See [:material-code-braces: ConfiguredTableAssociationAnalysisRulePolicyTypeDef](./type_defs.md#configuredtableassociationanalysisrulepolicytypedef) [:material-code-braces: ConfiguredTableAssociationAnalysisRulePolicyOutputTypeDef](./type_defs.md#configuredtableassociationanalysisrulepolicyoutputtypedef) 
## UpdateConfiguredTableAssociationAnalysisRuleInputTypeDef

```python
# UpdateConfiguredTableAssociationAnalysisRuleInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import UpdateConfiguredTableAssociationAnalysisRuleInputTypeDef


def get_value() -> UpdateConfiguredTableAssociationAnalysisRuleInputTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# UpdateConfiguredTableAssociationAnalysisRuleInputTypeDef definition

class UpdateConfiguredTableAssociationAnalysisRuleInputTypeDef(TypedDict):
    membershipIdentifier: str,
    configuredTableAssociationIdentifier: str,
    analysisRuleType: ConfiguredTableAssociationAnalysisRuleTypeType,  # (1)
    analysisRulePolicy: ConfiguredTableAssociationAnalysisRulePolicyUnionTypeDef,  # (2)
```

1. See [:material-code-brackets: ConfiguredTableAssociationAnalysisRuleTypeType](./literals.md#configuredtableassociationanalysisruletypetype) 
2. See [:material-code-braces: ConfiguredTableAssociationAnalysisRulePolicyTypeDef](./type_defs.md#configuredtableassociationanalysisrulepolicytypedef) [:material-code-braces: ConfiguredTableAssociationAnalysisRulePolicyOutputTypeDef](./type_defs.md#configuredtableassociationanalysisrulepolicyoutputtypedef) 
## ConfiguredTableAnalysisRulePolicyOutputTypeDef

```python
# ConfiguredTableAnalysisRulePolicyOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ConfiguredTableAnalysisRulePolicyOutputTypeDef


def get_value() -> ConfiguredTableAnalysisRulePolicyOutputTypeDef:
    return {
        "v1": ...,
    }


# ConfiguredTableAnalysisRulePolicyOutputTypeDef definition

class ConfiguredTableAnalysisRulePolicyOutputTypeDef(TypedDict):
    v1: NotRequired[ConfiguredTableAnalysisRulePolicyV1OutputTypeDef],  # (1)
```

1. See [:material-code-braces: ConfiguredTableAnalysisRulePolicyV1OutputTypeDef](./type_defs.md#configuredtableanalysisrulepolicyv1outputtypedef) 
## ConfiguredTableAnalysisRulePolicyTypeDef

```python
# ConfiguredTableAnalysisRulePolicyTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ConfiguredTableAnalysisRulePolicyTypeDef


def get_value() -> ConfiguredTableAnalysisRulePolicyTypeDef:
    return {
        "v1": ...,
    }


# ConfiguredTableAnalysisRulePolicyTypeDef definition

class ConfiguredTableAnalysisRulePolicyTypeDef(TypedDict):
    v1: NotRequired[ConfiguredTableAnalysisRulePolicyV1TypeDef],  # (1)
```

1. See [:material-code-braces: ConfiguredTableAnalysisRulePolicyV1TypeDef](./type_defs.md#configuredtableanalysisrulepolicyv1typedef) 
## ListCollaborationPrivacyBudgetsOutputTypeDef

```python
# ListCollaborationPrivacyBudgetsOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListCollaborationPrivacyBudgetsOutputTypeDef


def get_value() -> ListCollaborationPrivacyBudgetsOutputTypeDef:
    return {
        "collaborationPrivacyBudgetSummaries": ...,
    }


# ListCollaborationPrivacyBudgetsOutputTypeDef definition

class ListCollaborationPrivacyBudgetsOutputTypeDef(TypedDict):
    collaborationPrivacyBudgetSummaries: List[CollaborationPrivacyBudgetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CollaborationPrivacyBudgetSummaryTypeDef](./type_defs.md#collaborationprivacybudgetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPrivacyBudgetsOutputTypeDef

```python
# ListPrivacyBudgetsOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListPrivacyBudgetsOutputTypeDef


def get_value() -> ListPrivacyBudgetsOutputTypeDef:
    return {
        "privacyBudgetSummaries": ...,
    }


# ListPrivacyBudgetsOutputTypeDef definition

class ListPrivacyBudgetsOutputTypeDef(TypedDict):
    privacyBudgetSummaries: List[PrivacyBudgetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PrivacyBudgetSummaryTypeDef](./type_defs.md#privacybudgetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetSchemaOutputTypeDef

```python
# BatchGetSchemaOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import BatchGetSchemaOutputTypeDef


def get_value() -> BatchGetSchemaOutputTypeDef:
    return {
        "schemas": ...,
    }


# BatchGetSchemaOutputTypeDef definition

class BatchGetSchemaOutputTypeDef(TypedDict):
    schemas: List[SchemaTypeDef],  # (1)
    errors: List[BatchGetSchemaErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SchemaTypeDef](./type_defs.md#schematypedef) 
2. See [:material-code-braces: BatchGetSchemaErrorTypeDef](./type_defs.md#batchgetschemaerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSchemaOutputTypeDef

```python
# GetSchemaOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetSchemaOutputTypeDef


def get_value() -> GetSchemaOutputTypeDef:
    return {
        "schema": ...,
    }


# GetSchemaOutputTypeDef definition

class GetSchemaOutputTypeDef(TypedDict):
    schema: SchemaTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SchemaTypeDef](./type_defs.md#schematypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCollaborationInputTypeDef

```python
# CreateCollaborationInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CreateCollaborationInputTypeDef


def get_value() -> CreateCollaborationInputTypeDef:
    return {
        "members": ...,
    }


# CreateCollaborationInputTypeDef definition

class CreateCollaborationInputTypeDef(TypedDict):
    members: Sequence[MemberSpecificationTypeDef],  # (1)
    name: str,
    description: str,
    creatorMemberAbilities: Sequence[MemberAbilityType],  # (2)
    creatorDisplayName: str,
    queryLogStatus: CollaborationQueryLogStatusType,  # (3)
    creatorMLMemberAbilities: NotRequired[MLMemberAbilitiesUnionTypeDef],  # (4)
    dataEncryptionMetadata: NotRequired[DataEncryptionMetadataTypeDef],  # (5)
    tags: NotRequired[Mapping[str, str]],
    creatorPaymentConfiguration: NotRequired[PaymentConfigurationTypeDef],  # (6)
    analyticsEngine: NotRequired[AnalyticsEngineType],  # (7)
```

1. See [:material-code-braces: MemberSpecificationTypeDef](./type_defs.md#memberspecificationtypedef) 
2. See [:material-code-brackets: MemberAbilityType](./literals.md#memberabilitytype) 
3. See [:material-code-brackets: CollaborationQueryLogStatusType](./literals.md#collaborationquerylogstatustype) 
4. See [:material-code-braces: MLMemberAbilitiesTypeDef](./type_defs.md#mlmemberabilitiestypedef) [:material-code-braces: MLMemberAbilitiesOutputTypeDef](./type_defs.md#mlmemberabilitiesoutputtypedef) 
5. See [:material-code-braces: DataEncryptionMetadataTypeDef](./type_defs.md#dataencryptionmetadatatypedef) 
6. See [:material-code-braces: PaymentConfigurationTypeDef](./type_defs.md#paymentconfigurationtypedef) 
7. See [:material-code-brackets: AnalyticsEngineType](./literals.md#analyticsenginetype) 
## ListMembersOutputTypeDef

```python
# ListMembersOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListMembersOutputTypeDef


def get_value() -> ListMembersOutputTypeDef:
    return {
        "nextToken": ...,
    }


# ListMembersOutputTypeDef definition

class ListMembersOutputTypeDef(TypedDict):
    memberSummaries: List[MemberSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: MemberSummaryTypeDef](./type_defs.md#membersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMembershipsOutputTypeDef

```python
# ListMembershipsOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ListMembershipsOutputTypeDef


def get_value() -> ListMembershipsOutputTypeDef:
    return {
        "nextToken": ...,
    }


# ListMembershipsOutputTypeDef definition

class ListMembershipsOutputTypeDef(TypedDict):
    membershipSummaries: List[MembershipSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: MembershipSummaryTypeDef](./type_defs.md#membershipsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMembershipOutputTypeDef

```python
# CreateMembershipOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CreateMembershipOutputTypeDef


def get_value() -> CreateMembershipOutputTypeDef:
    return {
        "membership": ...,
    }


# CreateMembershipOutputTypeDef definition

class CreateMembershipOutputTypeDef(TypedDict):
    membership: MembershipTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MembershipTypeDef](./type_defs.md#membershiptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMembershipOutputTypeDef

```python
# GetMembershipOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetMembershipOutputTypeDef


def get_value() -> GetMembershipOutputTypeDef:
    return {
        "membership": ...,
    }


# GetMembershipOutputTypeDef definition

class GetMembershipOutputTypeDef(TypedDict):
    membership: MembershipTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MembershipTypeDef](./type_defs.md#membershiptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMembershipOutputTypeDef

```python
# UpdateMembershipOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import UpdateMembershipOutputTypeDef


def get_value() -> UpdateMembershipOutputTypeDef:
    return {
        "membership": ...,
    }


# UpdateMembershipOutputTypeDef definition

class UpdateMembershipOutputTypeDef(TypedDict):
    membership: MembershipTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MembershipTypeDef](./type_defs.md#membershiptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetProtectedQueryOutputTypeDef

```python
# GetProtectedQueryOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetProtectedQueryOutputTypeDef


def get_value() -> GetProtectedQueryOutputTypeDef:
    return {
        "protectedQuery": ...,
    }


# GetProtectedQueryOutputTypeDef definition

class GetProtectedQueryOutputTypeDef(TypedDict):
    protectedQuery: ProtectedQueryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProtectedQueryTypeDef](./type_defs.md#protectedquerytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartProtectedQueryOutputTypeDef

```python
# StartProtectedQueryOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import StartProtectedQueryOutputTypeDef


def get_value() -> StartProtectedQueryOutputTypeDef:
    return {
        "protectedQuery": ...,
    }


# StartProtectedQueryOutputTypeDef definition

class StartProtectedQueryOutputTypeDef(TypedDict):
    protectedQuery: ProtectedQueryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProtectedQueryTypeDef](./type_defs.md#protectedquerytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProtectedQueryOutputTypeDef

```python
# UpdateProtectedQueryOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import UpdateProtectedQueryOutputTypeDef


def get_value() -> UpdateProtectedQueryOutputTypeDef:
    return {
        "protectedQuery": ...,
    }


# UpdateProtectedQueryOutputTypeDef definition

class UpdateProtectedQueryOutputTypeDef(TypedDict):
    protectedQuery: ProtectedQueryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProtectedQueryTypeDef](./type_defs.md#protectedquerytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AnalysisRulePolicyTypeDef

```python
# AnalysisRulePolicyTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import AnalysisRulePolicyTypeDef


def get_value() -> AnalysisRulePolicyTypeDef:
    return {
        "v1": ...,
    }


# AnalysisRulePolicyTypeDef definition

class AnalysisRulePolicyTypeDef(TypedDict):
    v1: NotRequired[AnalysisRulePolicyV1TypeDef],  # (1)
```

1. See [:material-code-braces: AnalysisRulePolicyV1TypeDef](./type_defs.md#analysisrulepolicyv1typedef) 
## ConfiguredTableTypeDef

```python
# ConfiguredTableTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ConfiguredTableTypeDef


def get_value() -> ConfiguredTableTypeDef:
    return {
        "id": ...,
    }


# ConfiguredTableTypeDef definition

class ConfiguredTableTypeDef(TypedDict):
    id: str,
    arn: str,
    name: str,
    tableReference: TableReferenceOutputTypeDef,  # (1)
    createTime: datetime,
    updateTime: datetime,
    analysisRuleTypes: List[ConfiguredTableAnalysisRuleTypeType],  # (2)
    analysisMethod: AnalysisMethodType,  # (3)
    allowedColumns: List[str],
    description: NotRequired[str],
```

1. See [:material-code-braces: TableReferenceOutputTypeDef](./type_defs.md#tablereferenceoutputtypedef) 
2. See [:material-code-brackets: ConfiguredTableAnalysisRuleTypeType](./literals.md#configuredtableanalysisruletypetype) 
3. See [:material-code-brackets: AnalysisMethodType](./literals.md#analysismethodtype) 
## ConfiguredTableAnalysisRuleTypeDef

```python
# ConfiguredTableAnalysisRuleTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import ConfiguredTableAnalysisRuleTypeDef


def get_value() -> ConfiguredTableAnalysisRuleTypeDef:
    return {
        "configuredTableId": ...,
    }


# ConfiguredTableAnalysisRuleTypeDef definition

class ConfiguredTableAnalysisRuleTypeDef(TypedDict):
    configuredTableId: str,
    configuredTableArn: str,
    policy: ConfiguredTableAnalysisRulePolicyOutputTypeDef,  # (1)
    type: ConfiguredTableAnalysisRuleTypeType,  # (2)
    createTime: datetime,
    updateTime: datetime,
```

1. See [:material-code-braces: ConfiguredTableAnalysisRulePolicyOutputTypeDef](./type_defs.md#configuredtableanalysisrulepolicyoutputtypedef) 
2. See [:material-code-brackets: ConfiguredTableAnalysisRuleTypeType](./literals.md#configuredtableanalysisruletypetype) 
## AnalysisRuleTypeDef

```python
# AnalysisRuleTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import AnalysisRuleTypeDef


def get_value() -> AnalysisRuleTypeDef:
    return {
        "collaborationId": ...,
    }


# AnalysisRuleTypeDef definition

class AnalysisRuleTypeDef(TypedDict):
    collaborationId: str,
    type: AnalysisRuleTypeType,  # (1)
    name: str,
    createTime: datetime,
    updateTime: datetime,
    policy: AnalysisRulePolicyTypeDef,  # (2)
```

1. See [:material-code-brackets: AnalysisRuleTypeType](./literals.md#analysisruletypetype) 
2. See [:material-code-braces: AnalysisRulePolicyTypeDef](./type_defs.md#analysisrulepolicytypedef) 
## CreateConfiguredTableOutputTypeDef

```python
# CreateConfiguredTableOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CreateConfiguredTableOutputTypeDef


def get_value() -> CreateConfiguredTableOutputTypeDef:
    return {
        "configuredTable": ...,
    }


# CreateConfiguredTableOutputTypeDef definition

class CreateConfiguredTableOutputTypeDef(TypedDict):
    configuredTable: ConfiguredTableTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableTypeDef](./type_defs.md#configuredtabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConfiguredTableOutputTypeDef

```python
# GetConfiguredTableOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetConfiguredTableOutputTypeDef


def get_value() -> GetConfiguredTableOutputTypeDef:
    return {
        "configuredTable": ...,
    }


# GetConfiguredTableOutputTypeDef definition

class GetConfiguredTableOutputTypeDef(TypedDict):
    configuredTable: ConfiguredTableTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableTypeDef](./type_defs.md#configuredtabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateConfiguredTableOutputTypeDef

```python
# UpdateConfiguredTableOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import UpdateConfiguredTableOutputTypeDef


def get_value() -> UpdateConfiguredTableOutputTypeDef:
    return {
        "configuredTable": ...,
    }


# UpdateConfiguredTableOutputTypeDef definition

class UpdateConfiguredTableOutputTypeDef(TypedDict):
    configuredTable: ConfiguredTableTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableTypeDef](./type_defs.md#configuredtabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConfiguredTableInputTypeDef

```python
# CreateConfiguredTableInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CreateConfiguredTableInputTypeDef


def get_value() -> CreateConfiguredTableInputTypeDef:
    return {
        "name": ...,
    }


# CreateConfiguredTableInputTypeDef definition

class CreateConfiguredTableInputTypeDef(TypedDict):
    name: str,
    tableReference: TableReferenceUnionTypeDef,  # (1)
    allowedColumns: Sequence[str],
    analysisMethod: AnalysisMethodType,  # (2)
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: TableReferenceTypeDef](./type_defs.md#tablereferencetypedef) [:material-code-braces: TableReferenceOutputTypeDef](./type_defs.md#tablereferenceoutputtypedef) 
2. See [:material-code-brackets: AnalysisMethodType](./literals.md#analysismethodtype) 
## CreateConfiguredTableAnalysisRuleOutputTypeDef

```python
# CreateConfiguredTableAnalysisRuleOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CreateConfiguredTableAnalysisRuleOutputTypeDef


def get_value() -> CreateConfiguredTableAnalysisRuleOutputTypeDef:
    return {
        "analysisRule": ...,
    }


# CreateConfiguredTableAnalysisRuleOutputTypeDef definition

class CreateConfiguredTableAnalysisRuleOutputTypeDef(TypedDict):
    analysisRule: ConfiguredTableAnalysisRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableAnalysisRuleTypeDef](./type_defs.md#configuredtableanalysisruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConfiguredTableAnalysisRuleOutputTypeDef

```python
# GetConfiguredTableAnalysisRuleOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetConfiguredTableAnalysisRuleOutputTypeDef


def get_value() -> GetConfiguredTableAnalysisRuleOutputTypeDef:
    return {
        "analysisRule": ...,
    }


# GetConfiguredTableAnalysisRuleOutputTypeDef definition

class GetConfiguredTableAnalysisRuleOutputTypeDef(TypedDict):
    analysisRule: ConfiguredTableAnalysisRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableAnalysisRuleTypeDef](./type_defs.md#configuredtableanalysisruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateConfiguredTableAnalysisRuleOutputTypeDef

```python
# UpdateConfiguredTableAnalysisRuleOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import UpdateConfiguredTableAnalysisRuleOutputTypeDef


def get_value() -> UpdateConfiguredTableAnalysisRuleOutputTypeDef:
    return {
        "analysisRule": ...,
    }


# UpdateConfiguredTableAnalysisRuleOutputTypeDef definition

class UpdateConfiguredTableAnalysisRuleOutputTypeDef(TypedDict):
    analysisRule: ConfiguredTableAnalysisRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfiguredTableAnalysisRuleTypeDef](./type_defs.md#configuredtableanalysisruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConfiguredTableAnalysisRuleInputTypeDef

```python
# CreateConfiguredTableAnalysisRuleInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import CreateConfiguredTableAnalysisRuleInputTypeDef


def get_value() -> CreateConfiguredTableAnalysisRuleInputTypeDef:
    return {
        "configuredTableIdentifier": ...,
    }


# CreateConfiguredTableAnalysisRuleInputTypeDef definition

class CreateConfiguredTableAnalysisRuleInputTypeDef(TypedDict):
    configuredTableIdentifier: str,
    analysisRuleType: ConfiguredTableAnalysisRuleTypeType,  # (1)
    analysisRulePolicy: ConfiguredTableAnalysisRulePolicyUnionTypeDef,  # (2)
```

1. See [:material-code-brackets: ConfiguredTableAnalysisRuleTypeType](./literals.md#configuredtableanalysisruletypetype) 
2. See [:material-code-braces: ConfiguredTableAnalysisRulePolicyTypeDef](./type_defs.md#configuredtableanalysisrulepolicytypedef) [:material-code-braces: ConfiguredTableAnalysisRulePolicyOutputTypeDef](./type_defs.md#configuredtableanalysisrulepolicyoutputtypedef) 
## UpdateConfiguredTableAnalysisRuleInputTypeDef

```python
# UpdateConfiguredTableAnalysisRuleInputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import UpdateConfiguredTableAnalysisRuleInputTypeDef


def get_value() -> UpdateConfiguredTableAnalysisRuleInputTypeDef:
    return {
        "configuredTableIdentifier": ...,
    }


# UpdateConfiguredTableAnalysisRuleInputTypeDef definition

class UpdateConfiguredTableAnalysisRuleInputTypeDef(TypedDict):
    configuredTableIdentifier: str,
    analysisRuleType: ConfiguredTableAnalysisRuleTypeType,  # (1)
    analysisRulePolicy: ConfiguredTableAnalysisRulePolicyUnionTypeDef,  # (2)
```

1. See [:material-code-brackets: ConfiguredTableAnalysisRuleTypeType](./literals.md#configuredtableanalysisruletypetype) 
2. See [:material-code-braces: ConfiguredTableAnalysisRulePolicyTypeDef](./type_defs.md#configuredtableanalysisrulepolicytypedef) [:material-code-braces: ConfiguredTableAnalysisRulePolicyOutputTypeDef](./type_defs.md#configuredtableanalysisrulepolicyoutputtypedef) 
## BatchGetSchemaAnalysisRuleOutputTypeDef

```python
# BatchGetSchemaAnalysisRuleOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import BatchGetSchemaAnalysisRuleOutputTypeDef


def get_value() -> BatchGetSchemaAnalysisRuleOutputTypeDef:
    return {
        "analysisRules": ...,
    }


# BatchGetSchemaAnalysisRuleOutputTypeDef definition

class BatchGetSchemaAnalysisRuleOutputTypeDef(TypedDict):
    analysisRules: List[AnalysisRuleTypeDef],  # (1)
    errors: List[BatchGetSchemaAnalysisRuleErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AnalysisRuleTypeDef](./type_defs.md#analysisruletypedef) 
2. See [:material-code-braces: BatchGetSchemaAnalysisRuleErrorTypeDef](./type_defs.md#batchgetschemaanalysisruleerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSchemaAnalysisRuleOutputTypeDef

```python
# GetSchemaAnalysisRuleOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanrooms.type_defs import GetSchemaAnalysisRuleOutputTypeDef


def get_value() -> GetSchemaAnalysisRuleOutputTypeDef:
    return {
        "analysisRule": ...,
    }


# GetSchemaAnalysisRuleOutputTypeDef definition

class GetSchemaAnalysisRuleOutputTypeDef(TypedDict):
    analysisRule: AnalysisRuleTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnalysisRuleTypeDef](./type_defs.md#analysisruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
