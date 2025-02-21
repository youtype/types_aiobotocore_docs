# Type definitions

> [Index](../README.md) > [IoTSiteWise](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [IoTSiteWise](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#iotsitewise)
    type annotations stubs module [types-aiobotocore-iotsitewise](https://pypi.org/project/types-aiobotocore-iotsitewise/).

## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_iotsitewise.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## BlobTypeDef

```python
# BlobTypeDef Union usage example

from types_aiobotocore_iotsitewise.type_defs import BlobTypeDef


def get_value() -> BlobTypeDef:
    return ...


# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```


## PortalTypeEntryUnionTypeDef

```python
# PortalTypeEntryUnionTypeDef Union usage example

from types_aiobotocore_iotsitewise.type_defs import PortalTypeEntryUnionTypeDef


def get_value() -> PortalTypeEntryUnionTypeDef:
    return ...


# PortalTypeEntryUnionTypeDef definition

PortalTypeEntryUnionTypeDef = Union[
    PortalTypeEntryTypeDef,  # (1)
    PortalTypeEntryOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PortalTypeEntryTypeDef](./type_defs.md#portaltypeentrytypedef) 
2. See [:material-code-braces: PortalTypeEntryOutputTypeDef](./type_defs.md#portaltypeentryoutputtypedef) 

## VariableValueUnionTypeDef

```python
# VariableValueUnionTypeDef Union usage example

from types_aiobotocore_iotsitewise.type_defs import VariableValueUnionTypeDef


def get_value() -> VariableValueUnionTypeDef:
    return ...


# VariableValueUnionTypeDef definition

VariableValueUnionTypeDef = Union[
    VariableValueTypeDef,  # (1)
    VariableValueOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: VariableValueTypeDef](./type_defs.md#variablevaluetypedef) 
2. See [:material-code-braces: VariableValueOutputTypeDef](./type_defs.md#variablevalueoutputtypedef) 

## JobConfigurationUnionTypeDef

```python
# JobConfigurationUnionTypeDef Union usage example

from types_aiobotocore_iotsitewise.type_defs import JobConfigurationUnionTypeDef


def get_value() -> JobConfigurationUnionTypeDef:
    return ...


# JobConfigurationUnionTypeDef definition

JobConfigurationUnionTypeDef = Union[
    JobConfigurationTypeDef,  # (1)
    JobConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: JobConfigurationTypeDef](./type_defs.md#jobconfigurationtypedef) 
2. See [:material-code-braces: JobConfigurationOutputTypeDef](./type_defs.md#jobconfigurationoutputtypedef) 

## ExpressionVariableUnionTypeDef

```python
# ExpressionVariableUnionTypeDef Union usage example

from types_aiobotocore_iotsitewise.type_defs import ExpressionVariableUnionTypeDef


def get_value() -> ExpressionVariableUnionTypeDef:
    return ...


# ExpressionVariableUnionTypeDef definition

ExpressionVariableUnionTypeDef = Union[
    ExpressionVariableTypeDef,  # (1)
    ExpressionVariableOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ExpressionVariableTypeDef](./type_defs.md#expressionvariabletypedef) 
2. See [:material-code-braces: ExpressionVariableOutputTypeDef](./type_defs.md#expressionvariableoutputtypedef) 

## MetricUnionTypeDef

```python
# MetricUnionTypeDef Union usage example

from types_aiobotocore_iotsitewise.type_defs import MetricUnionTypeDef


def get_value() -> MetricUnionTypeDef:
    return ...


# MetricUnionTypeDef definition

MetricUnionTypeDef = Union[
    MetricTypeDef,  # (1)
    MetricOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MetricTypeDef](./type_defs.md#metrictypedef) 
2. See [:material-code-braces: MetricOutputTypeDef](./type_defs.md#metricoutputtypedef) 

## TransformUnionTypeDef

```python
# TransformUnionTypeDef Union usage example

from types_aiobotocore_iotsitewise.type_defs import TransformUnionTypeDef


def get_value() -> TransformUnionTypeDef:
    return ...


# TransformUnionTypeDef definition

TransformUnionTypeDef = Union[
    TransformTypeDef,  # (1)
    TransformOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TransformTypeDef](./type_defs.md#transformtypedef) 
2. See [:material-code-braces: TransformOutputTypeDef](./type_defs.md#transformoutputtypedef) 

## PropertyTypeUnionTypeDef

```python
# PropertyTypeUnionTypeDef Union usage example

from types_aiobotocore_iotsitewise.type_defs import PropertyTypeUnionTypeDef


def get_value() -> PropertyTypeUnionTypeDef:
    return ...


# PropertyTypeUnionTypeDef definition

PropertyTypeUnionTypeDef = Union[
    PropertyTypeTypeDef,  # (1)
    PropertyTypeOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PropertyTypeTypeDef](./type_defs.md#propertytypetypedef) 
2. See [:material-code-braces: PropertyTypeOutputTypeDef](./type_defs.md#propertytypeoutputtypedef) 

## AssetModelPropertyUnionTypeDef

```python
# AssetModelPropertyUnionTypeDef Union usage example

from types_aiobotocore_iotsitewise.type_defs import AssetModelPropertyUnionTypeDef


def get_value() -> AssetModelPropertyUnionTypeDef:
    return ...


# AssetModelPropertyUnionTypeDef definition

AssetModelPropertyUnionTypeDef = Union[
    AssetModelPropertyTypeDef,  # (1)
    AssetModelPropertyOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AssetModelPropertyTypeDef](./type_defs.md#assetmodelpropertytypedef) 
2. See [:material-code-braces: AssetModelPropertyOutputTypeDef](./type_defs.md#assetmodelpropertyoutputtypedef) 

## AssetModelCompositeModelUnionTypeDef

```python
# AssetModelCompositeModelUnionTypeDef Union usage example

from types_aiobotocore_iotsitewise.type_defs import AssetModelCompositeModelUnionTypeDef


def get_value() -> AssetModelCompositeModelUnionTypeDef:
    return ...


# AssetModelCompositeModelUnionTypeDef definition

AssetModelCompositeModelUnionTypeDef = Union[
    AssetModelCompositeModelTypeDef,  # (1)
    AssetModelCompositeModelOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AssetModelCompositeModelTypeDef](./type_defs.md#assetmodelcompositemodeltypedef) 
2. See [:material-code-braces: AssetModelCompositeModelOutputTypeDef](./type_defs.md#assetmodelcompositemodeloutputtypedef) 



## AccessDeniedExceptionTypeDef

```python
# AccessDeniedExceptionTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AccessDeniedExceptionTypeDef


def get_value() -> AccessDeniedExceptionTypeDef:
    return {
        "message": ...,
    }


# AccessDeniedExceptionTypeDef definition

class AccessDeniedExceptionTypeDef(TypedDict):
    message: NotRequired[str],
```

## ActionDefinitionTypeDef

```python
# ActionDefinitionTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ActionDefinitionTypeDef


def get_value() -> ActionDefinitionTypeDef:
    return {
        "actionDefinitionId": ...,
    }


# ActionDefinitionTypeDef definition

class ActionDefinitionTypeDef(TypedDict):
    actionDefinitionId: str,
    actionName: str,
    actionType: str,
```

## ActionPayloadTypeDef

```python
# ActionPayloadTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ActionPayloadTypeDef


def get_value() -> ActionPayloadTypeDef:
    return {
        "stringValue": ...,
    }


# ActionPayloadTypeDef definition

class ActionPayloadTypeDef(TypedDict):
    stringValue: str,
```

## TargetResourceTypeDef

```python
# TargetResourceTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import TargetResourceTypeDef


def get_value() -> TargetResourceTypeDef:
    return {
        "assetId": ...,
    }


# TargetResourceTypeDef definition

class TargetResourceTypeDef(TypedDict):
    assetId: str,
```

## AggregatesTypeDef

```python
# AggregatesTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AggregatesTypeDef


def get_value() -> AggregatesTypeDef:
    return {
        "average": ...,
    }


# AggregatesTypeDef definition

class AggregatesTypeDef(TypedDict):
    average: NotRequired[float],
    count: NotRequired[float],
    maximum: NotRequired[float],
    minimum: NotRequired[float],
    sum: NotRequired[float],
    standardDeviation: NotRequired[float],
```

## AlarmsTypeDef

```python
# AlarmsTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AlarmsTypeDef


def get_value() -> AlarmsTypeDef:
    return {
        "alarmRoleArn": ...,
    }


# AlarmsTypeDef definition

class AlarmsTypeDef(TypedDict):
    alarmRoleArn: str,
    notificationLambdaArn: NotRequired[str],
```

## AssetCompositeModelPathSegmentTypeDef

```python
# AssetCompositeModelPathSegmentTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AssetCompositeModelPathSegmentTypeDef


def get_value() -> AssetCompositeModelPathSegmentTypeDef:
    return {
        "id": ...,
    }


# AssetCompositeModelPathSegmentTypeDef definition

class AssetCompositeModelPathSegmentTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
```

## AssetErrorDetailsTypeDef

```python
# AssetErrorDetailsTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AssetErrorDetailsTypeDef


def get_value() -> AssetErrorDetailsTypeDef:
    return {
        "assetId": ...,
    }


# AssetErrorDetailsTypeDef definition

class AssetErrorDetailsTypeDef(TypedDict):
    assetId: str,
    code: AssetErrorCodeType,  # (1)
    message: str,
```

1. See [:material-code-brackets: AssetErrorCodeType](./literals.md#asseterrorcodetype) 
## AssetHierarchyInfoTypeDef

```python
# AssetHierarchyInfoTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AssetHierarchyInfoTypeDef


def get_value() -> AssetHierarchyInfoTypeDef:
    return {
        "parentAssetId": ...,
    }


# AssetHierarchyInfoTypeDef definition

class AssetHierarchyInfoTypeDef(TypedDict):
    parentAssetId: NotRequired[str],
    childAssetId: NotRequired[str],
```

## AssetHierarchyTypeDef

```python
# AssetHierarchyTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AssetHierarchyTypeDef


def get_value() -> AssetHierarchyTypeDef:
    return {
        "id": ...,
    }


# AssetHierarchyTypeDef definition

class AssetHierarchyTypeDef(TypedDict):
    name: str,
    id: NotRequired[str],
    externalId: NotRequired[str],
```

## AssetModelCompositeModelPathSegmentTypeDef

```python
# AssetModelCompositeModelPathSegmentTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AssetModelCompositeModelPathSegmentTypeDef


def get_value() -> AssetModelCompositeModelPathSegmentTypeDef:
    return {
        "id": ...,
    }


# AssetModelCompositeModelPathSegmentTypeDef definition

class AssetModelCompositeModelPathSegmentTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
```

## AssetModelHierarchyDefinitionTypeDef

```python
# AssetModelHierarchyDefinitionTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AssetModelHierarchyDefinitionTypeDef


def get_value() -> AssetModelHierarchyDefinitionTypeDef:
    return {
        "id": ...,
    }


# AssetModelHierarchyDefinitionTypeDef definition

class AssetModelHierarchyDefinitionTypeDef(TypedDict):
    name: str,
    childAssetModelId: str,
    id: NotRequired[str],
    externalId: NotRequired[str],
```

## AssetModelHierarchyTypeDef

```python
# AssetModelHierarchyTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AssetModelHierarchyTypeDef


def get_value() -> AssetModelHierarchyTypeDef:
    return {
        "id": ...,
    }


# AssetModelHierarchyTypeDef definition

class AssetModelHierarchyTypeDef(TypedDict):
    name: str,
    childAssetModelId: str,
    id: NotRequired[str],
    externalId: NotRequired[str],
```

## AssetModelPropertyPathSegmentTypeDef

```python
# AssetModelPropertyPathSegmentTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AssetModelPropertyPathSegmentTypeDef


def get_value() -> AssetModelPropertyPathSegmentTypeDef:
    return {
        "id": ...,
    }


# AssetModelPropertyPathSegmentTypeDef definition

class AssetModelPropertyPathSegmentTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
```

## AssetPropertyPathSegmentTypeDef

```python
# AssetPropertyPathSegmentTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AssetPropertyPathSegmentTypeDef


def get_value() -> AssetPropertyPathSegmentTypeDef:
    return {
        "id": ...,
    }


# AssetPropertyPathSegmentTypeDef definition

class AssetPropertyPathSegmentTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
```

## PropertyNotificationTypeDef

```python
# PropertyNotificationTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import PropertyNotificationTypeDef


def get_value() -> PropertyNotificationTypeDef:
    return {
        "topic": ...,
    }


# PropertyNotificationTypeDef definition

class PropertyNotificationTypeDef(TypedDict):
    topic: str,
    state: PropertyNotificationStateType,  # (1)
```

1. See [:material-code-brackets: PropertyNotificationStateType](./literals.md#propertynotificationstatetype) 
## TimeInNanosTypeDef

```python
# TimeInNanosTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import TimeInNanosTypeDef


def get_value() -> TimeInNanosTypeDef:
    return {
        "timeInSeconds": ...,
    }


# TimeInNanosTypeDef definition

class TimeInNanosTypeDef(TypedDict):
    timeInSeconds: int,
    offsetInNanos: NotRequired[int],
```

## AssociateAssetsRequestTypeDef

```python
# AssociateAssetsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AssociateAssetsRequestTypeDef


def get_value() -> AssociateAssetsRequestTypeDef:
    return {
        "assetId": ...,
    }


# AssociateAssetsRequestTypeDef definition

class AssociateAssetsRequestTypeDef(TypedDict):
    assetId: str,
    hierarchyId: str,
    childAssetId: str,
    clientToken: NotRequired[str],
```

## AssociateTimeSeriesToAssetPropertyRequestTypeDef

```python
# AssociateTimeSeriesToAssetPropertyRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AssociateTimeSeriesToAssetPropertyRequestTypeDef


def get_value() -> AssociateTimeSeriesToAssetPropertyRequestTypeDef:
    return {
        "alias": ...,
    }


# AssociateTimeSeriesToAssetPropertyRequestTypeDef definition

class AssociateTimeSeriesToAssetPropertyRequestTypeDef(TypedDict):
    alias: str,
    assetId: str,
    propertyId: str,
    clientToken: NotRequired[str],
```

## AttributeTypeDef

```python
# AttributeTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AttributeTypeDef


def get_value() -> AttributeTypeDef:
    return {
        "defaultValue": ...,
    }


# AttributeTypeDef definition

class AttributeTypeDef(TypedDict):
    defaultValue: NotRequired[str],
```

## BatchAssociateProjectAssetsRequestTypeDef

```python
# BatchAssociateProjectAssetsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import BatchAssociateProjectAssetsRequestTypeDef


def get_value() -> BatchAssociateProjectAssetsRequestTypeDef:
    return {
        "projectId": ...,
    }


# BatchAssociateProjectAssetsRequestTypeDef definition

class BatchAssociateProjectAssetsRequestTypeDef(TypedDict):
    projectId: str,
    assetIds: Sequence[str],
    clientToken: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ResponseMetadataTypeDef


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

## BatchDisassociateProjectAssetsRequestTypeDef

```python
# BatchDisassociateProjectAssetsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import BatchDisassociateProjectAssetsRequestTypeDef


def get_value() -> BatchDisassociateProjectAssetsRequestTypeDef:
    return {
        "projectId": ...,
    }


# BatchDisassociateProjectAssetsRequestTypeDef definition

class BatchDisassociateProjectAssetsRequestTypeDef(TypedDict):
    projectId: str,
    assetIds: Sequence[str],
    clientToken: NotRequired[str],
```

## BatchGetAssetPropertyAggregatesErrorEntryTypeDef

```python
# BatchGetAssetPropertyAggregatesErrorEntryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import BatchGetAssetPropertyAggregatesErrorEntryTypeDef


def get_value() -> BatchGetAssetPropertyAggregatesErrorEntryTypeDef:
    return {
        "errorCode": ...,
    }


# BatchGetAssetPropertyAggregatesErrorEntryTypeDef definition

class BatchGetAssetPropertyAggregatesErrorEntryTypeDef(TypedDict):
    errorCode: BatchGetAssetPropertyAggregatesErrorCodeType,  # (1)
    errorMessage: str,
    entryId: str,
```

1. See [:material-code-brackets: BatchGetAssetPropertyAggregatesErrorCodeType](./literals.md#batchgetassetpropertyaggregateserrorcodetype) 
## BatchGetAssetPropertyAggregatesErrorInfoTypeDef

```python
# BatchGetAssetPropertyAggregatesErrorInfoTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import BatchGetAssetPropertyAggregatesErrorInfoTypeDef


def get_value() -> BatchGetAssetPropertyAggregatesErrorInfoTypeDef:
    return {
        "errorCode": ...,
    }


# BatchGetAssetPropertyAggregatesErrorInfoTypeDef definition

class BatchGetAssetPropertyAggregatesErrorInfoTypeDef(TypedDict):
    errorCode: BatchGetAssetPropertyAggregatesErrorCodeType,  # (1)
    errorTimestamp: datetime,
```

1. See [:material-code-brackets: BatchGetAssetPropertyAggregatesErrorCodeType](./literals.md#batchgetassetpropertyaggregateserrorcodetype) 
## BatchGetAssetPropertyValueEntryTypeDef

```python
# BatchGetAssetPropertyValueEntryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import BatchGetAssetPropertyValueEntryTypeDef


def get_value() -> BatchGetAssetPropertyValueEntryTypeDef:
    return {
        "entryId": ...,
    }


# BatchGetAssetPropertyValueEntryTypeDef definition

class BatchGetAssetPropertyValueEntryTypeDef(TypedDict):
    entryId: str,
    assetId: NotRequired[str],
    propertyId: NotRequired[str],
    propertyAlias: NotRequired[str],
```

## BatchGetAssetPropertyValueErrorEntryTypeDef

```python
# BatchGetAssetPropertyValueErrorEntryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import BatchGetAssetPropertyValueErrorEntryTypeDef


def get_value() -> BatchGetAssetPropertyValueErrorEntryTypeDef:
    return {
        "errorCode": ...,
    }


# BatchGetAssetPropertyValueErrorEntryTypeDef definition

class BatchGetAssetPropertyValueErrorEntryTypeDef(TypedDict):
    errorCode: BatchGetAssetPropertyValueErrorCodeType,  # (1)
    errorMessage: str,
    entryId: str,
```

1. See [:material-code-brackets: BatchGetAssetPropertyValueErrorCodeType](./literals.md#batchgetassetpropertyvalueerrorcodetype) 
## BatchGetAssetPropertyValueErrorInfoTypeDef

```python
# BatchGetAssetPropertyValueErrorInfoTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import BatchGetAssetPropertyValueErrorInfoTypeDef


def get_value() -> BatchGetAssetPropertyValueErrorInfoTypeDef:
    return {
        "errorCode": ...,
    }


# BatchGetAssetPropertyValueErrorInfoTypeDef definition

class BatchGetAssetPropertyValueErrorInfoTypeDef(TypedDict):
    errorCode: BatchGetAssetPropertyValueErrorCodeType,  # (1)
    errorTimestamp: datetime,
```

1. See [:material-code-brackets: BatchGetAssetPropertyValueErrorCodeType](./literals.md#batchgetassetpropertyvalueerrorcodetype) 
## BatchGetAssetPropertyValueHistoryErrorEntryTypeDef

```python
# BatchGetAssetPropertyValueHistoryErrorEntryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import BatchGetAssetPropertyValueHistoryErrorEntryTypeDef


def get_value() -> BatchGetAssetPropertyValueHistoryErrorEntryTypeDef:
    return {
        "errorCode": ...,
    }


# BatchGetAssetPropertyValueHistoryErrorEntryTypeDef definition

class BatchGetAssetPropertyValueHistoryErrorEntryTypeDef(TypedDict):
    errorCode: BatchGetAssetPropertyValueHistoryErrorCodeType,  # (1)
    errorMessage: str,
    entryId: str,
```

1. See [:material-code-brackets: BatchGetAssetPropertyValueHistoryErrorCodeType](./literals.md#batchgetassetpropertyvaluehistoryerrorcodetype) 
## BatchGetAssetPropertyValueHistoryErrorInfoTypeDef

```python
# BatchGetAssetPropertyValueHistoryErrorInfoTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import BatchGetAssetPropertyValueHistoryErrorInfoTypeDef


def get_value() -> BatchGetAssetPropertyValueHistoryErrorInfoTypeDef:
    return {
        "errorCode": ...,
    }


# BatchGetAssetPropertyValueHistoryErrorInfoTypeDef definition

class BatchGetAssetPropertyValueHistoryErrorInfoTypeDef(TypedDict):
    errorCode: BatchGetAssetPropertyValueHistoryErrorCodeType,  # (1)
    errorTimestamp: datetime,
```

1. See [:material-code-brackets: BatchGetAssetPropertyValueHistoryErrorCodeType](./literals.md#batchgetassetpropertyvaluehistoryerrorcodetype) 
## ContentTypeDef

```python
# ContentTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ContentTypeDef


def get_value() -> ContentTypeDef:
    return {
        "text": ...,
    }


# ContentTypeDef definition

class ContentTypeDef(TypedDict):
    text: NotRequired[str],
```

## ColumnTypeTypeDef

```python
# ColumnTypeTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ColumnTypeTypeDef


def get_value() -> ColumnTypeTypeDef:
    return {
        "scalarType": ...,
    }


# ColumnTypeTypeDef definition

class ColumnTypeTypeDef(TypedDict):
    scalarType: NotRequired[ScalarTypeType],  # (1)
```

1. See [:material-code-brackets: ScalarTypeType](./literals.md#scalartypetype) 
## CompositionRelationshipItemTypeDef

```python
# CompositionRelationshipItemTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import CompositionRelationshipItemTypeDef


def get_value() -> CompositionRelationshipItemTypeDef:
    return {
        "id": ...,
    }


# CompositionRelationshipItemTypeDef definition

class CompositionRelationshipItemTypeDef(TypedDict):
    id: NotRequired[str],
```

## CompositionRelationshipSummaryTypeDef

```python
# CompositionRelationshipSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import CompositionRelationshipSummaryTypeDef


def get_value() -> CompositionRelationshipSummaryTypeDef:
    return {
        "assetModelId": ...,
    }


# CompositionRelationshipSummaryTypeDef definition

class CompositionRelationshipSummaryTypeDef(TypedDict):
    assetModelId: str,
    assetModelCompositeModelId: str,
    assetModelCompositeModelType: str,
```

## ConfigurationErrorDetailsTypeDef

```python
# ConfigurationErrorDetailsTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ConfigurationErrorDetailsTypeDef


def get_value() -> ConfigurationErrorDetailsTypeDef:
    return {
        "code": ...,
    }


# ConfigurationErrorDetailsTypeDef definition

class ConfigurationErrorDetailsTypeDef(TypedDict):
    code: ErrorCodeType,  # (1)
    message: str,
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
## ConflictingOperationExceptionTypeDef

```python
# ConflictingOperationExceptionTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ConflictingOperationExceptionTypeDef


def get_value() -> ConflictingOperationExceptionTypeDef:
    return {
        "message": ...,
    }


# ConflictingOperationExceptionTypeDef definition

class ConflictingOperationExceptionTypeDef(TypedDict):
    message: str,
    resourceId: str,
    resourceArn: str,
```

## CreateAssetRequestTypeDef

```python
# CreateAssetRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import CreateAssetRequestTypeDef


def get_value() -> CreateAssetRequestTypeDef:
    return {
        "assetName": ...,
    }


# CreateAssetRequestTypeDef definition

class CreateAssetRequestTypeDef(TypedDict):
    assetName: str,
    assetModelId: str,
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    assetDescription: NotRequired[str],
    assetId: NotRequired[str],
    assetExternalId: NotRequired[str],
```

## ErrorReportLocationTypeDef

```python
# ErrorReportLocationTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ErrorReportLocationTypeDef


def get_value() -> ErrorReportLocationTypeDef:
    return {
        "bucket": ...,
    }


# ErrorReportLocationTypeDef definition

class ErrorReportLocationTypeDef(TypedDict):
    bucket: str,
    prefix: str,
```

## FileTypeDef

```python
# FileTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import FileTypeDef


def get_value() -> FileTypeDef:
    return {
        "bucket": ...,
    }


# FileTypeDef definition

class FileTypeDef(TypedDict):
    bucket: str,
    key: str,
    versionId: NotRequired[str],
```

## CreateDashboardRequestTypeDef

```python
# CreateDashboardRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import CreateDashboardRequestTypeDef


def get_value() -> CreateDashboardRequestTypeDef:
    return {
        "projectId": ...,
    }


# CreateDashboardRequestTypeDef definition

class CreateDashboardRequestTypeDef(TypedDict):
    projectId: str,
    dashboardName: str,
    dashboardDefinition: str,
    dashboardDescription: NotRequired[str],
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## CreateProjectRequestTypeDef

```python
# CreateProjectRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import CreateProjectRequestTypeDef


def get_value() -> CreateProjectRequestTypeDef:
    return {
        "portalId": ...,
    }


# CreateProjectRequestTypeDef definition

class CreateProjectRequestTypeDef(TypedDict):
    portalId: str,
    projectName: str,
    projectDescription: NotRequired[str],
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## CsvOutputTypeDef

```python
# CsvOutputTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import CsvOutputTypeDef


def get_value() -> CsvOutputTypeDef:
    return {
        "columnNames": ...,
    }


# CsvOutputTypeDef definition

class CsvOutputTypeDef(TypedDict):
    columnNames: List[ColumnNameType],  # (1)
```

1. See [:material-code-brackets: ColumnNameType](./literals.md#columnnametype) 
## CsvTypeDef

```python
# CsvTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import CsvTypeDef


def get_value() -> CsvTypeDef:
    return {
        "columnNames": ...,
    }


# CsvTypeDef definition

class CsvTypeDef(TypedDict):
    columnNames: Sequence[ColumnNameType],  # (1)
```

1. See [:material-code-brackets: ColumnNameType](./literals.md#columnnametype) 
## CustomerManagedS3StorageTypeDef

```python
# CustomerManagedS3StorageTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import CustomerManagedS3StorageTypeDef


def get_value() -> CustomerManagedS3StorageTypeDef:
    return {
        "s3ResourceArn": ...,
    }


# CustomerManagedS3StorageTypeDef definition

class CustomerManagedS3StorageTypeDef(TypedDict):
    s3ResourceArn: str,
    roleArn: str,
```

## DashboardSummaryTypeDef

```python
# DashboardSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DashboardSummaryTypeDef


def get_value() -> DashboardSummaryTypeDef:
    return {
        "id": ...,
    }


# DashboardSummaryTypeDef definition

class DashboardSummaryTypeDef(TypedDict):
    id: str,
    name: str,
    description: NotRequired[str],
    creationDate: NotRequired[datetime],
    lastUpdateDate: NotRequired[datetime],
```

## DatumPaginatorTypeDef

```python
# DatumPaginatorTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DatumPaginatorTypeDef


def get_value() -> DatumPaginatorTypeDef:
    return {
        "scalarValue": ...,
    }


# DatumPaginatorTypeDef definition

class DatumPaginatorTypeDef(TypedDict):
    scalarValue: NotRequired[str],
    arrayValue: NotRequired[List[Dict[str, Any]]],
    rowValue: NotRequired[Dict[str, Any]],
    nullValue: NotRequired[bool],
```

## DatumTypeDef

```python
# DatumTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DatumTypeDef


def get_value() -> DatumTypeDef:
    return {
        "scalarValue": ...,
    }


# DatumTypeDef definition

class DatumTypeDef(TypedDict):
    scalarValue: NotRequired[str],
    arrayValue: NotRequired[List[Dict[str, Any]]],
    rowValue: NotRequired[Dict[str, Any]],
    nullValue: NotRequired[bool],
```

## DatumWaiterTypeDef

```python
# DatumWaiterTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DatumWaiterTypeDef


def get_value() -> DatumWaiterTypeDef:
    return {
        "scalarValue": ...,
    }


# DatumWaiterTypeDef definition

class DatumWaiterTypeDef(TypedDict):
    scalarValue: NotRequired[str],
    arrayValue: NotRequired[List[Dict[str, Any]]],
    rowValue: NotRequired[Dict[str, Any]],
    nullValue: NotRequired[bool],
```

## DeleteAccessPolicyRequestTypeDef

```python
# DeleteAccessPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DeleteAccessPolicyRequestTypeDef


def get_value() -> DeleteAccessPolicyRequestTypeDef:
    return {
        "accessPolicyId": ...,
    }


# DeleteAccessPolicyRequestTypeDef definition

class DeleteAccessPolicyRequestTypeDef(TypedDict):
    accessPolicyId: str,
    clientToken: NotRequired[str],
```

## DeleteAssetModelCompositeModelRequestTypeDef

```python
# DeleteAssetModelCompositeModelRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DeleteAssetModelCompositeModelRequestTypeDef


def get_value() -> DeleteAssetModelCompositeModelRequestTypeDef:
    return {
        "assetModelId": ...,
    }


# DeleteAssetModelCompositeModelRequestTypeDef definition

class DeleteAssetModelCompositeModelRequestTypeDef(TypedDict):
    assetModelId: str,
    assetModelCompositeModelId: str,
    clientToken: NotRequired[str],
    ifMatch: NotRequired[str],
    ifNoneMatch: NotRequired[str],
    matchForVersionType: NotRequired[AssetModelVersionTypeType],  # (1)
```

1. See [:material-code-brackets: AssetModelVersionTypeType](./literals.md#assetmodelversiontypetype) 
## DeleteAssetModelRequestTypeDef

```python
# DeleteAssetModelRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DeleteAssetModelRequestTypeDef


def get_value() -> DeleteAssetModelRequestTypeDef:
    return {
        "assetModelId": ...,
    }


# DeleteAssetModelRequestTypeDef definition

class DeleteAssetModelRequestTypeDef(TypedDict):
    assetModelId: str,
    clientToken: NotRequired[str],
    ifMatch: NotRequired[str],
    ifNoneMatch: NotRequired[str],
    matchForVersionType: NotRequired[AssetModelVersionTypeType],  # (1)
```

1. See [:material-code-brackets: AssetModelVersionTypeType](./literals.md#assetmodelversiontypetype) 
## DeleteAssetRequestTypeDef

```python
# DeleteAssetRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DeleteAssetRequestTypeDef


def get_value() -> DeleteAssetRequestTypeDef:
    return {
        "assetId": ...,
    }


# DeleteAssetRequestTypeDef definition

class DeleteAssetRequestTypeDef(TypedDict):
    assetId: str,
    clientToken: NotRequired[str],
```

## DeleteDashboardRequestTypeDef

```python
# DeleteDashboardRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DeleteDashboardRequestTypeDef


def get_value() -> DeleteDashboardRequestTypeDef:
    return {
        "dashboardId": ...,
    }


# DeleteDashboardRequestTypeDef definition

class DeleteDashboardRequestTypeDef(TypedDict):
    dashboardId: str,
    clientToken: NotRequired[str],
```

## DeleteDatasetRequestTypeDef

```python
# DeleteDatasetRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DeleteDatasetRequestTypeDef


def get_value() -> DeleteDatasetRequestTypeDef:
    return {
        "datasetId": ...,
    }


# DeleteDatasetRequestTypeDef definition

class DeleteDatasetRequestTypeDef(TypedDict):
    datasetId: str,
    clientToken: NotRequired[str],
```

## DeleteGatewayRequestTypeDef

```python
# DeleteGatewayRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DeleteGatewayRequestTypeDef


def get_value() -> DeleteGatewayRequestTypeDef:
    return {
        "gatewayId": ...,
    }


# DeleteGatewayRequestTypeDef definition

class DeleteGatewayRequestTypeDef(TypedDict):
    gatewayId: str,
```

## DeletePortalRequestTypeDef

```python
# DeletePortalRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DeletePortalRequestTypeDef


def get_value() -> DeletePortalRequestTypeDef:
    return {
        "portalId": ...,
    }


# DeletePortalRequestTypeDef definition

class DeletePortalRequestTypeDef(TypedDict):
    portalId: str,
    clientToken: NotRequired[str],
```

## DeleteProjectRequestTypeDef

```python
# DeleteProjectRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DeleteProjectRequestTypeDef


def get_value() -> DeleteProjectRequestTypeDef:
    return {
        "projectId": ...,
    }


# DeleteProjectRequestTypeDef definition

class DeleteProjectRequestTypeDef(TypedDict):
    projectId: str,
    clientToken: NotRequired[str],
```

## DeleteTimeSeriesRequestTypeDef

```python
# DeleteTimeSeriesRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DeleteTimeSeriesRequestTypeDef


def get_value() -> DeleteTimeSeriesRequestTypeDef:
    return {
        "alias": ...,
    }


# DeleteTimeSeriesRequestTypeDef definition

class DeleteTimeSeriesRequestTypeDef(TypedDict):
    alias: NotRequired[str],
    assetId: NotRequired[str],
    propertyId: NotRequired[str],
    clientToken: NotRequired[str],
```

## DescribeAccessPolicyRequestTypeDef

```python
# DescribeAccessPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeAccessPolicyRequestTypeDef


def get_value() -> DescribeAccessPolicyRequestTypeDef:
    return {
        "accessPolicyId": ...,
    }


# DescribeAccessPolicyRequestTypeDef definition

class DescribeAccessPolicyRequestTypeDef(TypedDict):
    accessPolicyId: str,
```

## DescribeActionRequestTypeDef

```python
# DescribeActionRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeActionRequestTypeDef


def get_value() -> DescribeActionRequestTypeDef:
    return {
        "actionId": ...,
    }


# DescribeActionRequestTypeDef definition

class DescribeActionRequestTypeDef(TypedDict):
    actionId: str,
```

## DescribeAssetCompositeModelRequestTypeDef

```python
# DescribeAssetCompositeModelRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeAssetCompositeModelRequestTypeDef


def get_value() -> DescribeAssetCompositeModelRequestTypeDef:
    return {
        "assetId": ...,
    }


# DescribeAssetCompositeModelRequestTypeDef definition

class DescribeAssetCompositeModelRequestTypeDef(TypedDict):
    assetId: str,
    assetCompositeModelId: str,
```

## DescribeAssetModelCompositeModelRequestTypeDef

```python
# DescribeAssetModelCompositeModelRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeAssetModelCompositeModelRequestTypeDef


def get_value() -> DescribeAssetModelCompositeModelRequestTypeDef:
    return {
        "assetModelId": ...,
    }


# DescribeAssetModelCompositeModelRequestTypeDef definition

class DescribeAssetModelCompositeModelRequestTypeDef(TypedDict):
    assetModelId: str,
    assetModelCompositeModelId: str,
    assetModelVersion: NotRequired[str],
```

## DescribeAssetModelRequestTypeDef

```python
# DescribeAssetModelRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeAssetModelRequestTypeDef


def get_value() -> DescribeAssetModelRequestTypeDef:
    return {
        "assetModelId": ...,
    }


# DescribeAssetModelRequestTypeDef definition

class DescribeAssetModelRequestTypeDef(TypedDict):
    assetModelId: str,
    excludeProperties: NotRequired[bool],
    assetModelVersion: NotRequired[str],
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import WaiterConfigTypeDef


def get_value() -> WaiterConfigTypeDef:
    return {
        "Delay": ...,
    }


# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeAssetPropertyRequestTypeDef

```python
# DescribeAssetPropertyRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeAssetPropertyRequestTypeDef


def get_value() -> DescribeAssetPropertyRequestTypeDef:
    return {
        "assetId": ...,
    }


# DescribeAssetPropertyRequestTypeDef definition

class DescribeAssetPropertyRequestTypeDef(TypedDict):
    assetId: str,
    propertyId: str,
```

## DescribeAssetRequestTypeDef

```python
# DescribeAssetRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeAssetRequestTypeDef


def get_value() -> DescribeAssetRequestTypeDef:
    return {
        "assetId": ...,
    }


# DescribeAssetRequestTypeDef definition

class DescribeAssetRequestTypeDef(TypedDict):
    assetId: str,
    excludeProperties: NotRequired[bool],
```

## DescribeBulkImportJobRequestTypeDef

```python
# DescribeBulkImportJobRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeBulkImportJobRequestTypeDef


def get_value() -> DescribeBulkImportJobRequestTypeDef:
    return {
        "jobId": ...,
    }


# DescribeBulkImportJobRequestTypeDef definition

class DescribeBulkImportJobRequestTypeDef(TypedDict):
    jobId: str,
```

## DescribeDashboardRequestTypeDef

```python
# DescribeDashboardRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeDashboardRequestTypeDef


def get_value() -> DescribeDashboardRequestTypeDef:
    return {
        "dashboardId": ...,
    }


# DescribeDashboardRequestTypeDef definition

class DescribeDashboardRequestTypeDef(TypedDict):
    dashboardId: str,
```

## DescribeDatasetRequestTypeDef

```python
# DescribeDatasetRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeDatasetRequestTypeDef


def get_value() -> DescribeDatasetRequestTypeDef:
    return {
        "datasetId": ...,
    }


# DescribeDatasetRequestTypeDef definition

class DescribeDatasetRequestTypeDef(TypedDict):
    datasetId: str,
```

## DescribeGatewayCapabilityConfigurationRequestTypeDef

```python
# DescribeGatewayCapabilityConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeGatewayCapabilityConfigurationRequestTypeDef


def get_value() -> DescribeGatewayCapabilityConfigurationRequestTypeDef:
    return {
        "gatewayId": ...,
    }


# DescribeGatewayCapabilityConfigurationRequestTypeDef definition

class DescribeGatewayCapabilityConfigurationRequestTypeDef(TypedDict):
    gatewayId: str,
    capabilityNamespace: str,
```

## DescribeGatewayRequestTypeDef

```python
# DescribeGatewayRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeGatewayRequestTypeDef


def get_value() -> DescribeGatewayRequestTypeDef:
    return {
        "gatewayId": ...,
    }


# DescribeGatewayRequestTypeDef definition

class DescribeGatewayRequestTypeDef(TypedDict):
    gatewayId: str,
```

## GatewayCapabilitySummaryTypeDef

```python
# GatewayCapabilitySummaryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import GatewayCapabilitySummaryTypeDef


def get_value() -> GatewayCapabilitySummaryTypeDef:
    return {
        "capabilityNamespace": ...,
    }


# GatewayCapabilitySummaryTypeDef definition

class GatewayCapabilitySummaryTypeDef(TypedDict):
    capabilityNamespace: str,
    capabilitySyncStatus: CapabilitySyncStatusType,  # (1)
```

1. See [:material-code-brackets: CapabilitySyncStatusType](./literals.md#capabilitysyncstatustype) 
## LoggingOptionsTypeDef

```python
# LoggingOptionsTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import LoggingOptionsTypeDef


def get_value() -> LoggingOptionsTypeDef:
    return {
        "level": ...,
    }


# LoggingOptionsTypeDef definition

class LoggingOptionsTypeDef(TypedDict):
    level: LoggingLevelType,  # (1)
```

1. See [:material-code-brackets: LoggingLevelType](./literals.md#loggingleveltype) 
## DescribePortalRequestTypeDef

```python
# DescribePortalRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribePortalRequestTypeDef


def get_value() -> DescribePortalRequestTypeDef:
    return {
        "portalId": ...,
    }


# DescribePortalRequestTypeDef definition

class DescribePortalRequestTypeDef(TypedDict):
    portalId: str,
```

## ImageLocationTypeDef

```python
# ImageLocationTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ImageLocationTypeDef


def get_value() -> ImageLocationTypeDef:
    return {
        "id": ...,
    }


# ImageLocationTypeDef definition

class ImageLocationTypeDef(TypedDict):
    id: str,
    url: str,
```

## PortalTypeEntryOutputTypeDef

```python
# PortalTypeEntryOutputTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import PortalTypeEntryOutputTypeDef


def get_value() -> PortalTypeEntryOutputTypeDef:
    return {
        "portalTools": ...,
    }


# PortalTypeEntryOutputTypeDef definition

class PortalTypeEntryOutputTypeDef(TypedDict):
    portalTools: NotRequired[List[str]],
```

## DescribeProjectRequestTypeDef

```python
# DescribeProjectRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeProjectRequestTypeDef


def get_value() -> DescribeProjectRequestTypeDef:
    return {
        "projectId": ...,
    }


# DescribeProjectRequestTypeDef definition

class DescribeProjectRequestTypeDef(TypedDict):
    projectId: str,
```

## RetentionPeriodTypeDef

```python
# RetentionPeriodTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import RetentionPeriodTypeDef


def get_value() -> RetentionPeriodTypeDef:
    return {
        "numberOfDays": ...,
    }


# RetentionPeriodTypeDef definition

class RetentionPeriodTypeDef(TypedDict):
    numberOfDays: NotRequired[int],
    unlimited: NotRequired[bool],
```

## WarmTierRetentionPeriodTypeDef

```python
# WarmTierRetentionPeriodTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import WarmTierRetentionPeriodTypeDef


def get_value() -> WarmTierRetentionPeriodTypeDef:
    return {
        "numberOfDays": ...,
    }


# WarmTierRetentionPeriodTypeDef definition

class WarmTierRetentionPeriodTypeDef(TypedDict):
    numberOfDays: NotRequired[int],
    unlimited: NotRequired[bool],
```

## DescribeTimeSeriesRequestTypeDef

```python
# DescribeTimeSeriesRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeTimeSeriesRequestTypeDef


def get_value() -> DescribeTimeSeriesRequestTypeDef:
    return {
        "alias": ...,
    }


# DescribeTimeSeriesRequestTypeDef definition

class DescribeTimeSeriesRequestTypeDef(TypedDict):
    alias: NotRequired[str],
    assetId: NotRequired[str],
    propertyId: NotRequired[str],
```

## DetailedErrorTypeDef

```python
# DetailedErrorTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DetailedErrorTypeDef


def get_value() -> DetailedErrorTypeDef:
    return {
        "code": ...,
    }


# DetailedErrorTypeDef definition

class DetailedErrorTypeDef(TypedDict):
    code: DetailedErrorCodeType,  # (1)
    message: str,
```

1. See [:material-code-brackets: DetailedErrorCodeType](./literals.md#detailederrorcodetype) 
## DisassociateAssetsRequestTypeDef

```python
# DisassociateAssetsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DisassociateAssetsRequestTypeDef


def get_value() -> DisassociateAssetsRequestTypeDef:
    return {
        "assetId": ...,
    }


# DisassociateAssetsRequestTypeDef definition

class DisassociateAssetsRequestTypeDef(TypedDict):
    assetId: str,
    hierarchyId: str,
    childAssetId: str,
    clientToken: NotRequired[str],
```

## DisassociateTimeSeriesFromAssetPropertyRequestTypeDef

```python
# DisassociateTimeSeriesFromAssetPropertyRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DisassociateTimeSeriesFromAssetPropertyRequestTypeDef


def get_value() -> DisassociateTimeSeriesFromAssetPropertyRequestTypeDef:
    return {
        "alias": ...,
    }


# DisassociateTimeSeriesFromAssetPropertyRequestTypeDef definition

class DisassociateTimeSeriesFromAssetPropertyRequestTypeDef(TypedDict):
    alias: str,
    assetId: str,
    propertyId: str,
    clientToken: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import PaginatorConfigTypeDef


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

## ExecuteQueryRequestTypeDef

```python
# ExecuteQueryRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ExecuteQueryRequestTypeDef


def get_value() -> ExecuteQueryRequestTypeDef:
    return {
        "queryStatement": ...,
    }


# ExecuteQueryRequestTypeDef definition

class ExecuteQueryRequestTypeDef(TypedDict):
    queryStatement: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    clientToken: NotRequired[str],
```

## ForwardingConfigTypeDef

```python
# ForwardingConfigTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ForwardingConfigTypeDef


def get_value() -> ForwardingConfigTypeDef:
    return {
        "state": ...,
    }


# ForwardingConfigTypeDef definition

class ForwardingConfigTypeDef(TypedDict):
    state: ForwardingConfigStateType,  # (1)
```

1. See [:material-code-brackets: ForwardingConfigStateType](./literals.md#forwardingconfigstatetype) 
## GreengrassTypeDef

```python
# GreengrassTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import GreengrassTypeDef


def get_value() -> GreengrassTypeDef:
    return {
        "groupArn": ...,
    }


# GreengrassTypeDef definition

class GreengrassTypeDef(TypedDict):
    groupArn: str,
```

## GreengrassV2TypeDef

```python
# GreengrassV2TypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import GreengrassV2TypeDef


def get_value() -> GreengrassV2TypeDef:
    return {
        "coreDeviceThingName": ...,
    }


# GreengrassV2TypeDef definition

class GreengrassV2TypeDef(TypedDict):
    coreDeviceThingName: str,
```

## SiemensIETypeDef

```python
# SiemensIETypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import SiemensIETypeDef


def get_value() -> SiemensIETypeDef:
    return {
        "iotCoreThingName": ...,
    }


# SiemensIETypeDef definition

class SiemensIETypeDef(TypedDict):
    iotCoreThingName: str,
```

## GetAssetPropertyValueRequestTypeDef

```python
# GetAssetPropertyValueRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import GetAssetPropertyValueRequestTypeDef


def get_value() -> GetAssetPropertyValueRequestTypeDef:
    return {
        "assetId": ...,
    }


# GetAssetPropertyValueRequestTypeDef definition

class GetAssetPropertyValueRequestTypeDef(TypedDict):
    assetId: NotRequired[str],
    propertyId: NotRequired[str],
    propertyAlias: NotRequired[str],
```

## GetInterpolatedAssetPropertyValuesRequestTypeDef

```python
# GetInterpolatedAssetPropertyValuesRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import GetInterpolatedAssetPropertyValuesRequestTypeDef


def get_value() -> GetInterpolatedAssetPropertyValuesRequestTypeDef:
    return {
        "startTimeInSeconds": ...,
    }


# GetInterpolatedAssetPropertyValuesRequestTypeDef definition

class GetInterpolatedAssetPropertyValuesRequestTypeDef(TypedDict):
    startTimeInSeconds: int,
    endTimeInSeconds: int,
    quality: QualityType,  # (1)
    intervalInSeconds: int,
    type: str,
    assetId: NotRequired[str],
    propertyId: NotRequired[str],
    propertyAlias: NotRequired[str],
    startTimeOffsetInNanos: NotRequired[int],
    endTimeOffsetInNanos: NotRequired[int],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    intervalWindowInSeconds: NotRequired[int],
```

1. See [:material-code-brackets: QualityType](./literals.md#qualitytype) 
## GroupIdentityTypeDef

```python
# GroupIdentityTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import GroupIdentityTypeDef


def get_value() -> GroupIdentityTypeDef:
    return {
        "id": ...,
    }


# GroupIdentityTypeDef definition

class GroupIdentityTypeDef(TypedDict):
    id: str,
```

## IAMRoleIdentityTypeDef

```python
# IAMRoleIdentityTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import IAMRoleIdentityTypeDef


def get_value() -> IAMRoleIdentityTypeDef:
    return {
        "arn": ...,
    }


# IAMRoleIdentityTypeDef definition

class IAMRoleIdentityTypeDef(TypedDict):
    arn: str,
```

## IAMUserIdentityTypeDef

```python
# IAMUserIdentityTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import IAMUserIdentityTypeDef


def get_value() -> IAMUserIdentityTypeDef:
    return {
        "arn": ...,
    }


# IAMUserIdentityTypeDef definition

class IAMUserIdentityTypeDef(TypedDict):
    arn: str,
```

## UserIdentityTypeDef

```python
# UserIdentityTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import UserIdentityTypeDef


def get_value() -> UserIdentityTypeDef:
    return {
        "id": ...,
    }


# UserIdentityTypeDef definition

class UserIdentityTypeDef(TypedDict):
    id: str,
```

## InternalFailureExceptionTypeDef

```python
# InternalFailureExceptionTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import InternalFailureExceptionTypeDef


def get_value() -> InternalFailureExceptionTypeDef:
    return {
        "message": ...,
    }


# InternalFailureExceptionTypeDef definition

class InternalFailureExceptionTypeDef(TypedDict):
    message: str,
```

## InvalidRequestExceptionTypeDef

```python
# InvalidRequestExceptionTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import InvalidRequestExceptionTypeDef


def get_value() -> InvalidRequestExceptionTypeDef:
    return {
        "message": ...,
    }


# InvalidRequestExceptionTypeDef definition

class InvalidRequestExceptionTypeDef(TypedDict):
    message: str,
```

## InvokeAssistantRequestTypeDef

```python
# InvokeAssistantRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import InvokeAssistantRequestTypeDef


def get_value() -> InvokeAssistantRequestTypeDef:
    return {
        "message": ...,
    }


# InvokeAssistantRequestTypeDef definition

class InvokeAssistantRequestTypeDef(TypedDict):
    message: str,
    conversationId: NotRequired[str],
    enableTrace: NotRequired[bool],
```

## JobSummaryTypeDef

```python
# JobSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import JobSummaryTypeDef


def get_value() -> JobSummaryTypeDef:
    return {
        "id": ...,
    }


# JobSummaryTypeDef definition

class JobSummaryTypeDef(TypedDict):
    id: str,
    name: str,
    status: JobStatusType,  # (1)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## KendraSourceDetailTypeDef

```python
# KendraSourceDetailTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import KendraSourceDetailTypeDef


def get_value() -> KendraSourceDetailTypeDef:
    return {
        "knowledgeBaseArn": ...,
    }


# KendraSourceDetailTypeDef definition

class KendraSourceDetailTypeDef(TypedDict):
    knowledgeBaseArn: str,
    roleArn: str,
```

## LimitExceededExceptionTypeDef

```python
# LimitExceededExceptionTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import LimitExceededExceptionTypeDef


def get_value() -> LimitExceededExceptionTypeDef:
    return {
        "message": ...,
    }


# LimitExceededExceptionTypeDef definition

class LimitExceededExceptionTypeDef(TypedDict):
    message: str,
```

## ListAccessPoliciesRequestTypeDef

```python
# ListAccessPoliciesRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListAccessPoliciesRequestTypeDef


def get_value() -> ListAccessPoliciesRequestTypeDef:
    return {
        "identityType": ...,
    }


# ListAccessPoliciesRequestTypeDef definition

class ListAccessPoliciesRequestTypeDef(TypedDict):
    identityType: NotRequired[IdentityTypeType],  # (1)
    identityId: NotRequired[str],
    resourceType: NotRequired[ResourceTypeType],  # (2)
    resourceId: NotRequired[str],
    iamArn: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## ListActionsRequestTypeDef

```python
# ListActionsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListActionsRequestTypeDef


def get_value() -> ListActionsRequestTypeDef:
    return {
        "targetResourceType": ...,
    }


# ListActionsRequestTypeDef definition

class ListActionsRequestTypeDef(TypedDict):
    targetResourceType: TargetResourceTypeType,  # (1)
    targetResourceId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: TargetResourceTypeType](./literals.md#targetresourcetypetype) 
## ListAssetModelCompositeModelsRequestTypeDef

```python
# ListAssetModelCompositeModelsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListAssetModelCompositeModelsRequestTypeDef


def get_value() -> ListAssetModelCompositeModelsRequestTypeDef:
    return {
        "assetModelId": ...,
    }


# ListAssetModelCompositeModelsRequestTypeDef definition

class ListAssetModelCompositeModelsRequestTypeDef(TypedDict):
    assetModelId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    assetModelVersion: NotRequired[str],
```

## ListAssetModelPropertiesRequestTypeDef

```python
# ListAssetModelPropertiesRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListAssetModelPropertiesRequestTypeDef


def get_value() -> ListAssetModelPropertiesRequestTypeDef:
    return {
        "assetModelId": ...,
    }


# ListAssetModelPropertiesRequestTypeDef definition

class ListAssetModelPropertiesRequestTypeDef(TypedDict):
    assetModelId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filter: NotRequired[ListAssetModelPropertiesFilterType],  # (1)
    assetModelVersion: NotRequired[str],
```

1. See [:material-code-brackets: ListAssetModelPropertiesFilterType](./literals.md#listassetmodelpropertiesfiltertype) 
## ListAssetModelsRequestTypeDef

```python
# ListAssetModelsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListAssetModelsRequestTypeDef


def get_value() -> ListAssetModelsRequestTypeDef:
    return {
        "assetModelTypes": ...,
    }


# ListAssetModelsRequestTypeDef definition

class ListAssetModelsRequestTypeDef(TypedDict):
    assetModelTypes: NotRequired[Sequence[AssetModelTypeType]],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    assetModelVersion: NotRequired[str],
```

1. See [:material-code-brackets: AssetModelTypeType](./literals.md#assetmodeltypetype) 
## ListAssetPropertiesRequestTypeDef

```python
# ListAssetPropertiesRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListAssetPropertiesRequestTypeDef


def get_value() -> ListAssetPropertiesRequestTypeDef:
    return {
        "assetId": ...,
    }


# ListAssetPropertiesRequestTypeDef definition

class ListAssetPropertiesRequestTypeDef(TypedDict):
    assetId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filter: NotRequired[ListAssetPropertiesFilterType],  # (1)
```

1. See [:material-code-brackets: ListAssetPropertiesFilterType](./literals.md#listassetpropertiesfiltertype) 
## ListAssetRelationshipsRequestTypeDef

```python
# ListAssetRelationshipsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListAssetRelationshipsRequestTypeDef


def get_value() -> ListAssetRelationshipsRequestTypeDef:
    return {
        "assetId": ...,
    }


# ListAssetRelationshipsRequestTypeDef definition

class ListAssetRelationshipsRequestTypeDef(TypedDict):
    assetId: str,
    traversalType: TraversalTypeType,  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: TraversalTypeType](./literals.md#traversaltypetype) 
## ListAssetsRequestTypeDef

```python
# ListAssetsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListAssetsRequestTypeDef


def get_value() -> ListAssetsRequestTypeDef:
    return {
        "nextToken": ...,
    }


# ListAssetsRequestTypeDef definition

class ListAssetsRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    assetModelId: NotRequired[str],
    filter: NotRequired[ListAssetsFilterType],  # (1)
```

1. See [:material-code-brackets: ListAssetsFilterType](./literals.md#listassetsfiltertype) 
## ListAssociatedAssetsRequestTypeDef

```python
# ListAssociatedAssetsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListAssociatedAssetsRequestTypeDef


def get_value() -> ListAssociatedAssetsRequestTypeDef:
    return {
        "assetId": ...,
    }


# ListAssociatedAssetsRequestTypeDef definition

class ListAssociatedAssetsRequestTypeDef(TypedDict):
    assetId: str,
    hierarchyId: NotRequired[str],
    traversalDirection: NotRequired[TraversalDirectionType],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: TraversalDirectionType](./literals.md#traversaldirectiontype) 
## ListBulkImportJobsRequestTypeDef

```python
# ListBulkImportJobsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListBulkImportJobsRequestTypeDef


def get_value() -> ListBulkImportJobsRequestTypeDef:
    return {
        "nextToken": ...,
    }


# ListBulkImportJobsRequestTypeDef definition

class ListBulkImportJobsRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filter: NotRequired[ListBulkImportJobsFilterType],  # (1)
```

1. See [:material-code-brackets: ListBulkImportJobsFilterType](./literals.md#listbulkimportjobsfiltertype) 
## ListCompositionRelationshipsRequestTypeDef

```python
# ListCompositionRelationshipsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListCompositionRelationshipsRequestTypeDef


def get_value() -> ListCompositionRelationshipsRequestTypeDef:
    return {
        "assetModelId": ...,
    }


# ListCompositionRelationshipsRequestTypeDef definition

class ListCompositionRelationshipsRequestTypeDef(TypedDict):
    assetModelId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListDashboardsRequestTypeDef

```python
# ListDashboardsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListDashboardsRequestTypeDef


def get_value() -> ListDashboardsRequestTypeDef:
    return {
        "projectId": ...,
    }


# ListDashboardsRequestTypeDef definition

class ListDashboardsRequestTypeDef(TypedDict):
    projectId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListDatasetsRequestTypeDef

```python
# ListDatasetsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListDatasetsRequestTypeDef


def get_value() -> ListDatasetsRequestTypeDef:
    return {
        "sourceType": ...,
    }


# ListDatasetsRequestTypeDef definition

class ListDatasetsRequestTypeDef(TypedDict):
    sourceType: DatasetSourceTypeType,  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: DatasetSourceTypeType](./literals.md#datasetsourcetypetype) 
## ListGatewaysRequestTypeDef

```python
# ListGatewaysRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListGatewaysRequestTypeDef


def get_value() -> ListGatewaysRequestTypeDef:
    return {
        "nextToken": ...,
    }


# ListGatewaysRequestTypeDef definition

class ListGatewaysRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListPortalsRequestTypeDef

```python
# ListPortalsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListPortalsRequestTypeDef


def get_value() -> ListPortalsRequestTypeDef:
    return {
        "nextToken": ...,
    }


# ListPortalsRequestTypeDef definition

class ListPortalsRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListProjectAssetsRequestTypeDef

```python
# ListProjectAssetsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListProjectAssetsRequestTypeDef


def get_value() -> ListProjectAssetsRequestTypeDef:
    return {
        "projectId": ...,
    }


# ListProjectAssetsRequestTypeDef definition

class ListProjectAssetsRequestTypeDef(TypedDict):
    projectId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListProjectsRequestTypeDef

```python
# ListProjectsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListProjectsRequestTypeDef


def get_value() -> ListProjectsRequestTypeDef:
    return {
        "portalId": ...,
    }


# ListProjectsRequestTypeDef definition

class ListProjectsRequestTypeDef(TypedDict):
    portalId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ProjectSummaryTypeDef

```python
# ProjectSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ProjectSummaryTypeDef


def get_value() -> ProjectSummaryTypeDef:
    return {
        "id": ...,
    }


# ProjectSummaryTypeDef definition

class ProjectSummaryTypeDef(TypedDict):
    id: str,
    name: str,
    description: NotRequired[str],
    creationDate: NotRequired[datetime],
    lastUpdateDate: NotRequired[datetime],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListTimeSeriesRequestTypeDef

```python
# ListTimeSeriesRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListTimeSeriesRequestTypeDef


def get_value() -> ListTimeSeriesRequestTypeDef:
    return {
        "nextToken": ...,
    }


# ListTimeSeriesRequestTypeDef definition

class ListTimeSeriesRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    assetId: NotRequired[str],
    aliasPrefix: NotRequired[str],
    timeSeriesType: NotRequired[ListTimeSeriesTypeType],  # (1)
```

1. See [:material-code-brackets: ListTimeSeriesTypeType](./literals.md#listtimeseriestypetype) 
## TimeSeriesSummaryTypeDef

```python
# TimeSeriesSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import TimeSeriesSummaryTypeDef


def get_value() -> TimeSeriesSummaryTypeDef:
    return {
        "assetId": ...,
    }


# TimeSeriesSummaryTypeDef definition

class TimeSeriesSummaryTypeDef(TypedDict):
    timeSeriesId: str,
    dataType: PropertyDataTypeType,  # (1)
    timeSeriesCreationDate: datetime,
    timeSeriesLastUpdateDate: datetime,
    timeSeriesArn: str,
    assetId: NotRequired[str],
    propertyId: NotRequired[str],
    alias: NotRequired[str],
    dataTypeSpec: NotRequired[str],
```

1. See [:material-code-brackets: PropertyDataTypeType](./literals.md#propertydatatypetype) 
## LocationTypeDef

```python
# LocationTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import LocationTypeDef


def get_value() -> LocationTypeDef:
    return {
        "uri": ...,
    }


# LocationTypeDef definition

class LocationTypeDef(TypedDict):
    uri: NotRequired[str],
```

## MetricProcessingConfigTypeDef

```python
# MetricProcessingConfigTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import MetricProcessingConfigTypeDef


def get_value() -> MetricProcessingConfigTypeDef:
    return {
        "computeLocation": ...,
    }


# MetricProcessingConfigTypeDef definition

class MetricProcessingConfigTypeDef(TypedDict):
    computeLocation: ComputeLocationType,  # (1)
```

1. See [:material-code-brackets: ComputeLocationType](./literals.md#computelocationtype) 
## TumblingWindowTypeDef

```python
# TumblingWindowTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import TumblingWindowTypeDef


def get_value() -> TumblingWindowTypeDef:
    return {
        "interval": ...,
    }


# TumblingWindowTypeDef definition

class TumblingWindowTypeDef(TypedDict):
    interval: str,
    offset: NotRequired[str],
```

## MonitorErrorDetailsTypeDef

```python
# MonitorErrorDetailsTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import MonitorErrorDetailsTypeDef


def get_value() -> MonitorErrorDetailsTypeDef:
    return {
        "code": ...,
    }


# MonitorErrorDetailsTypeDef definition

class MonitorErrorDetailsTypeDef(TypedDict):
    code: NotRequired[MonitorErrorCodeType],  # (1)
    message: NotRequired[str],
```

1. See [:material-code-brackets: MonitorErrorCodeType](./literals.md#monitorerrorcodetype) 
## PortalResourceTypeDef

```python
# PortalResourceTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import PortalResourceTypeDef


def get_value() -> PortalResourceTypeDef:
    return {
        "id": ...,
    }


# PortalResourceTypeDef definition

class PortalResourceTypeDef(TypedDict):
    id: str,
```

## PortalTypeEntryTypeDef

```python
# PortalTypeEntryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import PortalTypeEntryTypeDef


def get_value() -> PortalTypeEntryTypeDef:
    return {
        "portalTools": ...,
    }


# PortalTypeEntryTypeDef definition

class PortalTypeEntryTypeDef(TypedDict):
    portalTools: NotRequired[Sequence[str]],
```

## ProjectResourceTypeDef

```python
# ProjectResourceTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ProjectResourceTypeDef


def get_value() -> ProjectResourceTypeDef:
    return {
        "id": ...,
    }


# ProjectResourceTypeDef definition

class ProjectResourceTypeDef(TypedDict):
    id: str,
```

## PropertyValueNullValueTypeDef

```python
# PropertyValueNullValueTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import PropertyValueNullValueTypeDef


def get_value() -> PropertyValueNullValueTypeDef:
    return {
        "valueType": ...,
    }


# PropertyValueNullValueTypeDef definition

class PropertyValueNullValueTypeDef(TypedDict):
    valueType: RawValueTypeType,  # (1)
```

1. See [:material-code-brackets: RawValueTypeType](./literals.md#rawvaluetypetype) 
## PutDefaultEncryptionConfigurationRequestTypeDef

```python
# PutDefaultEncryptionConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import PutDefaultEncryptionConfigurationRequestTypeDef


def get_value() -> PutDefaultEncryptionConfigurationRequestTypeDef:
    return {
        "encryptionType": ...,
    }


# PutDefaultEncryptionConfigurationRequestTypeDef definition

class PutDefaultEncryptionConfigurationRequestTypeDef(TypedDict):
    encryptionType: EncryptionTypeType,  # (1)
    kmsKeyId: NotRequired[str],
```

1. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
## ResourceNotFoundExceptionTypeDef

```python
# ResourceNotFoundExceptionTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ResourceNotFoundExceptionTypeDef


def get_value() -> ResourceNotFoundExceptionTypeDef:
    return {
        "message": ...,
    }


# ResourceNotFoundExceptionTypeDef definition

class ResourceNotFoundExceptionTypeDef(TypedDict):
    message: str,
```

## ThrottlingExceptionTypeDef

```python
# ThrottlingExceptionTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ThrottlingExceptionTypeDef


def get_value() -> ThrottlingExceptionTypeDef:
    return {
        "message": ...,
    }


# ThrottlingExceptionTypeDef definition

class ThrottlingExceptionTypeDef(TypedDict):
    message: str,
```

## TraceTypeDef

```python
# TraceTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import TraceTypeDef


def get_value() -> TraceTypeDef:
    return {
        "text": ...,
    }


# TraceTypeDef definition

class TraceTypeDef(TypedDict):
    text: NotRequired[str],
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateAssetPropertyRequestTypeDef

```python
# UpdateAssetPropertyRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import UpdateAssetPropertyRequestTypeDef


def get_value() -> UpdateAssetPropertyRequestTypeDef:
    return {
        "assetId": ...,
    }


# UpdateAssetPropertyRequestTypeDef definition

class UpdateAssetPropertyRequestTypeDef(TypedDict):
    assetId: str,
    propertyId: str,
    propertyAlias: NotRequired[str],
    propertyNotificationState: NotRequired[PropertyNotificationStateType],  # (1)
    clientToken: NotRequired[str],
    propertyUnit: NotRequired[str],
```

1. See [:material-code-brackets: PropertyNotificationStateType](./literals.md#propertynotificationstatetype) 
## UpdateAssetRequestTypeDef

```python
# UpdateAssetRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import UpdateAssetRequestTypeDef


def get_value() -> UpdateAssetRequestTypeDef:
    return {
        "assetId": ...,
    }


# UpdateAssetRequestTypeDef definition

class UpdateAssetRequestTypeDef(TypedDict):
    assetId: str,
    assetName: str,
    clientToken: NotRequired[str],
    assetDescription: NotRequired[str],
    assetExternalId: NotRequired[str],
```

## UpdateDashboardRequestTypeDef

```python
# UpdateDashboardRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import UpdateDashboardRequestTypeDef


def get_value() -> UpdateDashboardRequestTypeDef:
    return {
        "dashboardId": ...,
    }


# UpdateDashboardRequestTypeDef definition

class UpdateDashboardRequestTypeDef(TypedDict):
    dashboardId: str,
    dashboardName: str,
    dashboardDefinition: str,
    dashboardDescription: NotRequired[str],
    clientToken: NotRequired[str],
```

## UpdateGatewayCapabilityConfigurationRequestTypeDef

```python
# UpdateGatewayCapabilityConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import UpdateGatewayCapabilityConfigurationRequestTypeDef


def get_value() -> UpdateGatewayCapabilityConfigurationRequestTypeDef:
    return {
        "gatewayId": ...,
    }


# UpdateGatewayCapabilityConfigurationRequestTypeDef definition

class UpdateGatewayCapabilityConfigurationRequestTypeDef(TypedDict):
    gatewayId: str,
    capabilityNamespace: str,
    capabilityConfiguration: str,
```

## UpdateGatewayRequestTypeDef

```python
# UpdateGatewayRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import UpdateGatewayRequestTypeDef


def get_value() -> UpdateGatewayRequestTypeDef:
    return {
        "gatewayId": ...,
    }


# UpdateGatewayRequestTypeDef definition

class UpdateGatewayRequestTypeDef(TypedDict):
    gatewayId: str,
    gatewayName: str,
```

## UpdateProjectRequestTypeDef

```python
# UpdateProjectRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import UpdateProjectRequestTypeDef


def get_value() -> UpdateProjectRequestTypeDef:
    return {
        "projectId": ...,
    }


# UpdateProjectRequestTypeDef definition

class UpdateProjectRequestTypeDef(TypedDict):
    projectId: str,
    projectName: str,
    projectDescription: NotRequired[str],
    clientToken: NotRequired[str],
```

## ActionSummaryTypeDef

```python
# ActionSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ActionSummaryTypeDef


def get_value() -> ActionSummaryTypeDef:
    return {
        "actionId": ...,
    }


# ActionSummaryTypeDef definition

class ActionSummaryTypeDef(TypedDict):
    actionId: NotRequired[str],
    actionDefinitionId: NotRequired[str],
    targetResource: NotRequired[TargetResourceTypeDef],  # (1)
```

1. See [:material-code-braces: TargetResourceTypeDef](./type_defs.md#targetresourcetypedef) 
## ExecuteActionRequestTypeDef

```python
# ExecuteActionRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ExecuteActionRequestTypeDef


def get_value() -> ExecuteActionRequestTypeDef:
    return {
        "targetResource": ...,
    }


# ExecuteActionRequestTypeDef definition

class ExecuteActionRequestTypeDef(TypedDict):
    targetResource: TargetResourceTypeDef,  # (1)
    actionDefinitionId: str,
    actionPayload: ActionPayloadTypeDef,  # (2)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: TargetResourceTypeDef](./type_defs.md#targetresourcetypedef) 
2. See [:material-code-braces: ActionPayloadTypeDef](./type_defs.md#actionpayloadtypedef) 
## AggregatedValueTypeDef

```python
# AggregatedValueTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AggregatedValueTypeDef


def get_value() -> AggregatedValueTypeDef:
    return {
        "timestamp": ...,
    }


# AggregatedValueTypeDef definition

class AggregatedValueTypeDef(TypedDict):
    timestamp: datetime,
    value: AggregatesTypeDef,  # (2)
    quality: NotRequired[QualityType],  # (1)
```

1. See [:material-code-brackets: QualityType](./literals.md#qualitytype) 
2. See [:material-code-braces: AggregatesTypeDef](./type_defs.md#aggregatestypedef) 
## AssetCompositeModelSummaryTypeDef

```python
# AssetCompositeModelSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AssetCompositeModelSummaryTypeDef


def get_value() -> AssetCompositeModelSummaryTypeDef:
    return {
        "id": ...,
    }


# AssetCompositeModelSummaryTypeDef definition

class AssetCompositeModelSummaryTypeDef(TypedDict):
    id: str,
    name: str,
    type: str,
    description: str,
    path: List[AssetCompositeModelPathSegmentTypeDef],  # (1)
    externalId: NotRequired[str],
```

1. See [:material-code-braces: AssetCompositeModelPathSegmentTypeDef](./type_defs.md#assetcompositemodelpathsegmenttypedef) 
## AssetRelationshipSummaryTypeDef

```python
# AssetRelationshipSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AssetRelationshipSummaryTypeDef


def get_value() -> AssetRelationshipSummaryTypeDef:
    return {
        "hierarchyInfo": ...,
    }


# AssetRelationshipSummaryTypeDef definition

class AssetRelationshipSummaryTypeDef(TypedDict):
    relationshipType: AssetRelationshipTypeType,  # (2)
    hierarchyInfo: NotRequired[AssetHierarchyInfoTypeDef],  # (1)
```

1. See [:material-code-braces: AssetHierarchyInfoTypeDef](./type_defs.md#assethierarchyinfotypedef) 
2. See [:material-code-brackets: AssetRelationshipTypeType](./literals.md#assetrelationshiptypetype) 
## AssetModelCompositeModelSummaryTypeDef

```python
# AssetModelCompositeModelSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AssetModelCompositeModelSummaryTypeDef


def get_value() -> AssetModelCompositeModelSummaryTypeDef:
    return {
        "id": ...,
    }


# AssetModelCompositeModelSummaryTypeDef definition

class AssetModelCompositeModelSummaryTypeDef(TypedDict):
    id: str,
    name: str,
    type: str,
    externalId: NotRequired[str],
    description: NotRequired[str],
    path: NotRequired[List[AssetModelCompositeModelPathSegmentTypeDef]],  # (1)
```

1. See [:material-code-braces: AssetModelCompositeModelPathSegmentTypeDef](./type_defs.md#assetmodelcompositemodelpathsegmenttypedef) 
## VariableValueOutputTypeDef

```python
# VariableValueOutputTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import VariableValueOutputTypeDef


def get_value() -> VariableValueOutputTypeDef:
    return {
        "propertyId": ...,
    }


# VariableValueOutputTypeDef definition

class VariableValueOutputTypeDef(TypedDict):
    propertyId: NotRequired[str],
    hierarchyId: NotRequired[str],
    propertyPath: NotRequired[List[AssetModelPropertyPathSegmentTypeDef]],  # (1)
```

1. See [:material-code-braces: AssetModelPropertyPathSegmentTypeDef](./type_defs.md#assetmodelpropertypathsegmenttypedef) 
## VariableValueTypeDef

```python
# VariableValueTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import VariableValueTypeDef


def get_value() -> VariableValueTypeDef:
    return {
        "propertyId": ...,
    }


# VariableValueTypeDef definition

class VariableValueTypeDef(TypedDict):
    propertyId: NotRequired[str],
    hierarchyId: NotRequired[str],
    propertyPath: NotRequired[Sequence[AssetModelPropertyPathSegmentTypeDef]],  # (1)
```

1. See [:material-code-braces: AssetModelPropertyPathSegmentTypeDef](./type_defs.md#assetmodelpropertypathsegmenttypedef) 
## AssetPropertySummaryTypeDef

```python
# AssetPropertySummaryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AssetPropertySummaryTypeDef


def get_value() -> AssetPropertySummaryTypeDef:
    return {
        "id": ...,
    }


# AssetPropertySummaryTypeDef definition

class AssetPropertySummaryTypeDef(TypedDict):
    id: str,
    alias: NotRequired[str],
    unit: NotRequired[str],
    notification: NotRequired[PropertyNotificationTypeDef],  # (1)
    assetCompositeModelId: NotRequired[str],
    path: NotRequired[List[AssetPropertyPathSegmentTypeDef]],  # (2)
    externalId: NotRequired[str],
```

1. See [:material-code-braces: PropertyNotificationTypeDef](./type_defs.md#propertynotificationtypedef) 
2. See [:material-code-braces: AssetPropertyPathSegmentTypeDef](./type_defs.md#assetpropertypathsegmenttypedef) 
## AssetPropertyTypeDef

```python
# AssetPropertyTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AssetPropertyTypeDef


def get_value() -> AssetPropertyTypeDef:
    return {
        "id": ...,
    }


# AssetPropertyTypeDef definition

class AssetPropertyTypeDef(TypedDict):
    id: str,
    name: str,
    dataType: PropertyDataTypeType,  # (2)
    alias: NotRequired[str],
    notification: NotRequired[PropertyNotificationTypeDef],  # (1)
    dataTypeSpec: NotRequired[str],
    unit: NotRequired[str],
    path: NotRequired[List[AssetPropertyPathSegmentTypeDef]],  # (3)
    externalId: NotRequired[str],
```

1. See [:material-code-braces: PropertyNotificationTypeDef](./type_defs.md#propertynotificationtypedef) 
2. See [:material-code-brackets: PropertyDataTypeType](./literals.md#propertydatatypetype) 
3. See [:material-code-braces: AssetPropertyPathSegmentTypeDef](./type_defs.md#assetpropertypathsegmenttypedef) 
## BatchPutAssetPropertyErrorTypeDef

```python
# BatchPutAssetPropertyErrorTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import BatchPutAssetPropertyErrorTypeDef


def get_value() -> BatchPutAssetPropertyErrorTypeDef:
    return {
        "errorCode": ...,
    }


# BatchPutAssetPropertyErrorTypeDef definition

class BatchPutAssetPropertyErrorTypeDef(TypedDict):
    errorCode: BatchPutAssetPropertyValueErrorCodeType,  # (1)
    errorMessage: str,
    timestamps: List[TimeInNanosTypeDef],  # (2)
```

1. See [:material-code-brackets: BatchPutAssetPropertyValueErrorCodeType](./literals.md#batchputassetpropertyvalueerrorcodetype) 
2. See [:material-code-braces: TimeInNanosTypeDef](./type_defs.md#timeinnanostypedef) 
## BatchAssociateProjectAssetsResponseTypeDef

```python
# BatchAssociateProjectAssetsResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import BatchAssociateProjectAssetsResponseTypeDef


def get_value() -> BatchAssociateProjectAssetsResponseTypeDef:
    return {
        "errors": ...,
    }


# BatchAssociateProjectAssetsResponseTypeDef definition

class BatchAssociateProjectAssetsResponseTypeDef(TypedDict):
    errors: List[AssetErrorDetailsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssetErrorDetailsTypeDef](./type_defs.md#asseterrordetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDisassociateProjectAssetsResponseTypeDef

```python
# BatchDisassociateProjectAssetsResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import BatchDisassociateProjectAssetsResponseTypeDef


def get_value() -> BatchDisassociateProjectAssetsResponseTypeDef:
    return {
        "errors": ...,
    }


# BatchDisassociateProjectAssetsResponseTypeDef definition

class BatchDisassociateProjectAssetsResponseTypeDef(TypedDict):
    errors: List[AssetErrorDetailsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssetErrorDetailsTypeDef](./type_defs.md#asseterrordetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAccessPolicyResponseTypeDef

```python
# CreateAccessPolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import CreateAccessPolicyResponseTypeDef


def get_value() -> CreateAccessPolicyResponseTypeDef:
    return {
        "accessPolicyId": ...,
    }


# CreateAccessPolicyResponseTypeDef definition

class CreateAccessPolicyResponseTypeDef(TypedDict):
    accessPolicyId: str,
    accessPolicyArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBulkImportJobResponseTypeDef

```python
# CreateBulkImportJobResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import CreateBulkImportJobResponseTypeDef


def get_value() -> CreateBulkImportJobResponseTypeDef:
    return {
        "jobId": ...,
    }


# CreateBulkImportJobResponseTypeDef definition

class CreateBulkImportJobResponseTypeDef(TypedDict):
    jobId: str,
    jobName: str,
    jobStatus: JobStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDashboardResponseTypeDef

```python
# CreateDashboardResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import CreateDashboardResponseTypeDef


def get_value() -> CreateDashboardResponseTypeDef:
    return {
        "dashboardId": ...,
    }


# CreateDashboardResponseTypeDef definition

class CreateDashboardResponseTypeDef(TypedDict):
    dashboardId: str,
    dashboardArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGatewayResponseTypeDef

```python
# CreateGatewayResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import CreateGatewayResponseTypeDef


def get_value() -> CreateGatewayResponseTypeDef:
    return {
        "gatewayId": ...,
    }


# CreateGatewayResponseTypeDef definition

class CreateGatewayResponseTypeDef(TypedDict):
    gatewayId: str,
    gatewayArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProjectResponseTypeDef

```python
# CreateProjectResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import CreateProjectResponseTypeDef


def get_value() -> CreateProjectResponseTypeDef:
    return {
        "projectId": ...,
    }


# CreateProjectResponseTypeDef definition

class CreateProjectResponseTypeDef(TypedDict):
    projectId: str,
    projectArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeActionResponseTypeDef

```python
# DescribeActionResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeActionResponseTypeDef


def get_value() -> DescribeActionResponseTypeDef:
    return {
        "actionId": ...,
    }


# DescribeActionResponseTypeDef definition

class DescribeActionResponseTypeDef(TypedDict):
    actionId: str,
    targetResource: TargetResourceTypeDef,  # (1)
    actionDefinitionId: str,
    actionPayload: ActionPayloadTypeDef,  # (2)
    executionTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: TargetResourceTypeDef](./type_defs.md#targetresourcetypedef) 
2. See [:material-code-braces: ActionPayloadTypeDef](./type_defs.md#actionpayloadtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDashboardResponseTypeDef

```python
# DescribeDashboardResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeDashboardResponseTypeDef


def get_value() -> DescribeDashboardResponseTypeDef:
    return {
        "dashboardId": ...,
    }


# DescribeDashboardResponseTypeDef definition

class DescribeDashboardResponseTypeDef(TypedDict):
    dashboardId: str,
    dashboardArn: str,
    dashboardName: str,
    projectId: str,
    dashboardDescription: str,
    dashboardDefinition: str,
    dashboardCreationDate: datetime,
    dashboardLastUpdateDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeGatewayCapabilityConfigurationResponseTypeDef

```python
# DescribeGatewayCapabilityConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeGatewayCapabilityConfigurationResponseTypeDef


def get_value() -> DescribeGatewayCapabilityConfigurationResponseTypeDef:
    return {
        "gatewayId": ...,
    }


# DescribeGatewayCapabilityConfigurationResponseTypeDef definition

class DescribeGatewayCapabilityConfigurationResponseTypeDef(TypedDict):
    gatewayId: str,
    capabilityNamespace: str,
    capabilityConfiguration: str,
    capabilitySyncStatus: CapabilitySyncStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: CapabilitySyncStatusType](./literals.md#capabilitysyncstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeProjectResponseTypeDef

```python
# DescribeProjectResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeProjectResponseTypeDef


def get_value() -> DescribeProjectResponseTypeDef:
    return {
        "projectId": ...,
    }


# DescribeProjectResponseTypeDef definition

class DescribeProjectResponseTypeDef(TypedDict):
    projectId: str,
    projectArn: str,
    projectName: str,
    portalId: str,
    projectDescription: str,
    projectCreationDate: datetime,
    projectLastUpdateDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTimeSeriesResponseTypeDef

```python
# DescribeTimeSeriesResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeTimeSeriesResponseTypeDef


def get_value() -> DescribeTimeSeriesResponseTypeDef:
    return {
        "assetId": ...,
    }


# DescribeTimeSeriesResponseTypeDef definition

class DescribeTimeSeriesResponseTypeDef(TypedDict):
    assetId: str,
    propertyId: str,
    alias: str,
    timeSeriesId: str,
    dataType: PropertyDataTypeType,  # (1)
    dataTypeSpec: str,
    timeSeriesCreationDate: datetime,
    timeSeriesLastUpdateDate: datetime,
    timeSeriesArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: PropertyDataTypeType](./literals.md#propertydatatypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExecuteActionResponseTypeDef

```python
# ExecuteActionResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ExecuteActionResponseTypeDef


def get_value() -> ExecuteActionResponseTypeDef:
    return {
        "actionId": ...,
    }


# ExecuteActionResponseTypeDef definition

class ExecuteActionResponseTypeDef(TypedDict):
    actionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProjectAssetsResponseTypeDef

```python
# ListProjectAssetsResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListProjectAssetsResponseTypeDef


def get_value() -> ListProjectAssetsResponseTypeDef:
    return {
        "assetIds": ...,
    }


# ListProjectAssetsResponseTypeDef definition

class ListProjectAssetsResponseTypeDef(TypedDict):
    assetIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGatewayCapabilityConfigurationResponseTypeDef

```python
# UpdateGatewayCapabilityConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import UpdateGatewayCapabilityConfigurationResponseTypeDef


def get_value() -> UpdateGatewayCapabilityConfigurationResponseTypeDef:
    return {
        "capabilityNamespace": ...,
    }


# UpdateGatewayCapabilityConfigurationResponseTypeDef definition

class UpdateGatewayCapabilityConfigurationResponseTypeDef(TypedDict):
    capabilityNamespace: str,
    capabilitySyncStatus: CapabilitySyncStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: CapabilitySyncStatusType](./literals.md#capabilitysyncstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetAssetPropertyAggregatesEntryTypeDef

```python
# BatchGetAssetPropertyAggregatesEntryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import BatchGetAssetPropertyAggregatesEntryTypeDef


def get_value() -> BatchGetAssetPropertyAggregatesEntryTypeDef:
    return {
        "entryId": ...,
    }


# BatchGetAssetPropertyAggregatesEntryTypeDef definition

class BatchGetAssetPropertyAggregatesEntryTypeDef(TypedDict):
    entryId: str,
    aggregateTypes: Sequence[AggregateTypeType],  # (1)
    resolution: str,
    startDate: TimestampTypeDef,
    endDate: TimestampTypeDef,
    assetId: NotRequired[str],
    propertyId: NotRequired[str],
    propertyAlias: NotRequired[str],
    qualities: NotRequired[Sequence[QualityType]],  # (2)
    timeOrdering: NotRequired[TimeOrderingType],  # (3)
```

1. See [:material-code-brackets: AggregateTypeType](./literals.md#aggregatetypetype) 
2. See [:material-code-brackets: QualityType](./literals.md#qualitytype) 
3. See [:material-code-brackets: TimeOrderingType](./literals.md#timeorderingtype) 
## BatchGetAssetPropertyValueHistoryEntryTypeDef

```python
# BatchGetAssetPropertyValueHistoryEntryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import BatchGetAssetPropertyValueHistoryEntryTypeDef


def get_value() -> BatchGetAssetPropertyValueHistoryEntryTypeDef:
    return {
        "entryId": ...,
    }


# BatchGetAssetPropertyValueHistoryEntryTypeDef definition

class BatchGetAssetPropertyValueHistoryEntryTypeDef(TypedDict):
    entryId: str,
    assetId: NotRequired[str],
    propertyId: NotRequired[str],
    propertyAlias: NotRequired[str],
    startDate: NotRequired[TimestampTypeDef],
    endDate: NotRequired[TimestampTypeDef],
    qualities: NotRequired[Sequence[QualityType]],  # (1)
    timeOrdering: NotRequired[TimeOrderingType],  # (2)
```

1. See [:material-code-brackets: QualityType](./literals.md#qualitytype) 
2. See [:material-code-brackets: TimeOrderingType](./literals.md#timeorderingtype) 
## GetAssetPropertyAggregatesRequestTypeDef

```python
# GetAssetPropertyAggregatesRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import GetAssetPropertyAggregatesRequestTypeDef


def get_value() -> GetAssetPropertyAggregatesRequestTypeDef:
    return {
        "aggregateTypes": ...,
    }


# GetAssetPropertyAggregatesRequestTypeDef definition

class GetAssetPropertyAggregatesRequestTypeDef(TypedDict):
    aggregateTypes: Sequence[AggregateTypeType],  # (1)
    resolution: str,
    startDate: TimestampTypeDef,
    endDate: TimestampTypeDef,
    assetId: NotRequired[str],
    propertyId: NotRequired[str],
    propertyAlias: NotRequired[str],
    qualities: NotRequired[Sequence[QualityType]],  # (2)
    timeOrdering: NotRequired[TimeOrderingType],  # (3)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: AggregateTypeType](./literals.md#aggregatetypetype) 
2. See [:material-code-brackets: QualityType](./literals.md#qualitytype) 
3. See [:material-code-brackets: TimeOrderingType](./literals.md#timeorderingtype) 
## GetAssetPropertyValueHistoryRequestTypeDef

```python
# GetAssetPropertyValueHistoryRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import GetAssetPropertyValueHistoryRequestTypeDef


def get_value() -> GetAssetPropertyValueHistoryRequestTypeDef:
    return {
        "assetId": ...,
    }


# GetAssetPropertyValueHistoryRequestTypeDef definition

class GetAssetPropertyValueHistoryRequestTypeDef(TypedDict):
    assetId: NotRequired[str],
    propertyId: NotRequired[str],
    propertyAlias: NotRequired[str],
    startDate: NotRequired[TimestampTypeDef],
    endDate: NotRequired[TimestampTypeDef],
    qualities: NotRequired[Sequence[QualityType]],  # (1)
    timeOrdering: NotRequired[TimeOrderingType],  # (2)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: QualityType](./literals.md#qualitytype) 
2. See [:material-code-brackets: TimeOrderingType](./literals.md#timeorderingtype) 
## BatchGetAssetPropertyAggregatesSkippedEntryTypeDef

```python
# BatchGetAssetPropertyAggregatesSkippedEntryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import BatchGetAssetPropertyAggregatesSkippedEntryTypeDef


def get_value() -> BatchGetAssetPropertyAggregatesSkippedEntryTypeDef:
    return {
        "entryId": ...,
    }


# BatchGetAssetPropertyAggregatesSkippedEntryTypeDef definition

class BatchGetAssetPropertyAggregatesSkippedEntryTypeDef(TypedDict):
    entryId: str,
    completionStatus: BatchEntryCompletionStatusType,  # (1)
    errorInfo: NotRequired[BatchGetAssetPropertyAggregatesErrorInfoTypeDef],  # (2)
```

1. See [:material-code-brackets: BatchEntryCompletionStatusType](./literals.md#batchentrycompletionstatustype) 
2. See [:material-code-braces: BatchGetAssetPropertyAggregatesErrorInfoTypeDef](./type_defs.md#batchgetassetpropertyaggregateserrorinfotypedef) 
## BatchGetAssetPropertyValueRequestTypeDef

```python
# BatchGetAssetPropertyValueRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import BatchGetAssetPropertyValueRequestTypeDef


def get_value() -> BatchGetAssetPropertyValueRequestTypeDef:
    return {
        "entries": ...,
    }


# BatchGetAssetPropertyValueRequestTypeDef definition

class BatchGetAssetPropertyValueRequestTypeDef(TypedDict):
    entries: Sequence[BatchGetAssetPropertyValueEntryTypeDef],  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BatchGetAssetPropertyValueEntryTypeDef](./type_defs.md#batchgetassetpropertyvalueentrytypedef) 
## BatchGetAssetPropertyValueSkippedEntryTypeDef

```python
# BatchGetAssetPropertyValueSkippedEntryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import BatchGetAssetPropertyValueSkippedEntryTypeDef


def get_value() -> BatchGetAssetPropertyValueSkippedEntryTypeDef:
    return {
        "entryId": ...,
    }


# BatchGetAssetPropertyValueSkippedEntryTypeDef definition

class BatchGetAssetPropertyValueSkippedEntryTypeDef(TypedDict):
    entryId: str,
    completionStatus: BatchEntryCompletionStatusType,  # (1)
    errorInfo: NotRequired[BatchGetAssetPropertyValueErrorInfoTypeDef],  # (2)
```

1. See [:material-code-brackets: BatchEntryCompletionStatusType](./literals.md#batchentrycompletionstatustype) 
2. See [:material-code-braces: BatchGetAssetPropertyValueErrorInfoTypeDef](./type_defs.md#batchgetassetpropertyvalueerrorinfotypedef) 
## BatchGetAssetPropertyValueHistorySkippedEntryTypeDef

```python
# BatchGetAssetPropertyValueHistorySkippedEntryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import BatchGetAssetPropertyValueHistorySkippedEntryTypeDef


def get_value() -> BatchGetAssetPropertyValueHistorySkippedEntryTypeDef:
    return {
        "entryId": ...,
    }


# BatchGetAssetPropertyValueHistorySkippedEntryTypeDef definition

class BatchGetAssetPropertyValueHistorySkippedEntryTypeDef(TypedDict):
    entryId: str,
    completionStatus: BatchEntryCompletionStatusType,  # (1)
    errorInfo: NotRequired[BatchGetAssetPropertyValueHistoryErrorInfoTypeDef],  # (2)
```

1. See [:material-code-brackets: BatchEntryCompletionStatusType](./literals.md#batchentrycompletionstatustype) 
2. See [:material-code-braces: BatchGetAssetPropertyValueHistoryErrorInfoTypeDef](./type_defs.md#batchgetassetpropertyvaluehistoryerrorinfotypedef) 
## ImageFileTypeDef

```python
# ImageFileTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ImageFileTypeDef


def get_value() -> ImageFileTypeDef:
    return {
        "data": ...,
    }


# ImageFileTypeDef definition

class ImageFileTypeDef(TypedDict):
    data: BlobTypeDef,
    type: ImageFileTypeType,  # (1)
```

1. See [:material-code-brackets: ImageFileTypeType](./literals.md#imagefiletypetype) 
## ColumnInfoTypeDef

```python
# ColumnInfoTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ColumnInfoTypeDef


def get_value() -> ColumnInfoTypeDef:
    return {
        "name": ...,
    }


# ColumnInfoTypeDef definition

class ColumnInfoTypeDef(TypedDict):
    name: NotRequired[str],
    type: NotRequired[ColumnTypeTypeDef],  # (1)
```

1. See [:material-code-braces: ColumnTypeTypeDef](./type_defs.md#columntypetypedef) 
## CompositionDetailsTypeDef

```python
# CompositionDetailsTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import CompositionDetailsTypeDef


def get_value() -> CompositionDetailsTypeDef:
    return {
        "compositionRelationship": ...,
    }


# CompositionDetailsTypeDef definition

class CompositionDetailsTypeDef(TypedDict):
    compositionRelationship: NotRequired[List[CompositionRelationshipItemTypeDef]],  # (1)
```

1. See [:material-code-braces: CompositionRelationshipItemTypeDef](./type_defs.md#compositionrelationshipitemtypedef) 
## ListCompositionRelationshipsResponseTypeDef

```python
# ListCompositionRelationshipsResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListCompositionRelationshipsResponseTypeDef


def get_value() -> ListCompositionRelationshipsResponseTypeDef:
    return {
        "compositionRelationshipSummaries": ...,
    }


# ListCompositionRelationshipsResponseTypeDef definition

class ListCompositionRelationshipsResponseTypeDef(TypedDict):
    compositionRelationshipSummaries: List[CompositionRelationshipSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CompositionRelationshipSummaryTypeDef](./type_defs.md#compositionrelationshipsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConfigurationStatusTypeDef

```python
# ConfigurationStatusTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ConfigurationStatusTypeDef


def get_value() -> ConfigurationStatusTypeDef:
    return {
        "state": ...,
    }


# ConfigurationStatusTypeDef definition

class ConfigurationStatusTypeDef(TypedDict):
    state: ConfigurationStateType,  # (1)
    error: NotRequired[ConfigurationErrorDetailsTypeDef],  # (2)
```

1. See [:material-code-brackets: ConfigurationStateType](./literals.md#configurationstatetype) 
2. See [:material-code-braces: ConfigurationErrorDetailsTypeDef](./type_defs.md#configurationerrordetailstypedef) 
## FileFormatOutputTypeDef

```python
# FileFormatOutputTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import FileFormatOutputTypeDef


def get_value() -> FileFormatOutputTypeDef:
    return {
        "csv": ...,
    }


# FileFormatOutputTypeDef definition

class FileFormatOutputTypeDef(TypedDict):
    csv: NotRequired[CsvOutputTypeDef],  # (1)
    parquet: NotRequired[Dict[str, Any]],
```

1. See [:material-code-braces: CsvOutputTypeDef](./type_defs.md#csvoutputtypedef) 
## FileFormatTypeDef

```python
# FileFormatTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import FileFormatTypeDef


def get_value() -> FileFormatTypeDef:
    return {
        "csv": ...,
    }


# FileFormatTypeDef definition

class FileFormatTypeDef(TypedDict):
    csv: NotRequired[CsvTypeDef],  # (1)
    parquet: NotRequired[Mapping[str, Any]],
```

1. See [:material-code-braces: CsvTypeDef](./type_defs.md#csvtypedef) 
## MultiLayerStorageTypeDef

```python
# MultiLayerStorageTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import MultiLayerStorageTypeDef


def get_value() -> MultiLayerStorageTypeDef:
    return {
        "customerManagedS3Storage": ...,
    }


# MultiLayerStorageTypeDef definition

class MultiLayerStorageTypeDef(TypedDict):
    customerManagedS3Storage: CustomerManagedS3StorageTypeDef,  # (1)
```

1. See [:material-code-braces: CustomerManagedS3StorageTypeDef](./type_defs.md#customermanageds3storagetypedef) 
## ListDashboardsResponseTypeDef

```python
# ListDashboardsResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListDashboardsResponseTypeDef


def get_value() -> ListDashboardsResponseTypeDef:
    return {
        "dashboardSummaries": ...,
    }


# ListDashboardsResponseTypeDef definition

class ListDashboardsResponseTypeDef(TypedDict):
    dashboardSummaries: List[DashboardSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DashboardSummaryTypeDef](./type_defs.md#dashboardsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RowPaginatorTypeDef

```python
# RowPaginatorTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import RowPaginatorTypeDef


def get_value() -> RowPaginatorTypeDef:
    return {
        "data": ...,
    }


# RowPaginatorTypeDef definition

class RowPaginatorTypeDef(TypedDict):
    data: List[DatumPaginatorTypeDef],  # (1)
```

1. See [:material-code-braces: DatumPaginatorTypeDef](./type_defs.md#datumpaginatortypedef) 
## RowTypeDef

```python
# RowTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import RowTypeDef


def get_value() -> RowTypeDef:
    return {
        "data": ...,
    }


# RowTypeDef definition

class RowTypeDef(TypedDict):
    data: List[DatumTypeDef],  # (1)
```

1. See [:material-code-braces: DatumTypeDef](./type_defs.md#datumtypedef) 
## RowWaiterTypeDef

```python
# RowWaiterTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import RowWaiterTypeDef


def get_value() -> RowWaiterTypeDef:
    return {
        "data": ...,
    }


# RowWaiterTypeDef definition

class RowWaiterTypeDef(TypedDict):
    data: List[DatumWaiterTypeDef],  # (1)
```

1. See [:material-code-braces: DatumWaiterTypeDef](./type_defs.md#datumwaitertypedef) 
## DescribeAssetModelRequestWaitExtraTypeDef

```python
# DescribeAssetModelRequestWaitExtraTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeAssetModelRequestWaitExtraTypeDef


def get_value() -> DescribeAssetModelRequestWaitExtraTypeDef:
    return {
        "assetModelId": ...,
    }


# DescribeAssetModelRequestWaitExtraTypeDef definition

class DescribeAssetModelRequestWaitExtraTypeDef(TypedDict):
    assetModelId: str,
    excludeProperties: NotRequired[bool],
    assetModelVersion: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeAssetModelRequestWaitTypeDef

```python
# DescribeAssetModelRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeAssetModelRequestWaitTypeDef


def get_value() -> DescribeAssetModelRequestWaitTypeDef:
    return {
        "assetModelId": ...,
    }


# DescribeAssetModelRequestWaitTypeDef definition

class DescribeAssetModelRequestWaitTypeDef(TypedDict):
    assetModelId: str,
    excludeProperties: NotRequired[bool],
    assetModelVersion: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeAssetRequestWaitExtraTypeDef

```python
# DescribeAssetRequestWaitExtraTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeAssetRequestWaitExtraTypeDef


def get_value() -> DescribeAssetRequestWaitExtraTypeDef:
    return {
        "assetId": ...,
    }


# DescribeAssetRequestWaitExtraTypeDef definition

class DescribeAssetRequestWaitExtraTypeDef(TypedDict):
    assetId: str,
    excludeProperties: NotRequired[bool],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeAssetRequestWaitTypeDef

```python
# DescribeAssetRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeAssetRequestWaitTypeDef


def get_value() -> DescribeAssetRequestWaitTypeDef:
    return {
        "assetId": ...,
    }


# DescribeAssetRequestWaitTypeDef definition

class DescribeAssetRequestWaitTypeDef(TypedDict):
    assetId: str,
    excludeProperties: NotRequired[bool],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribePortalRequestWaitExtraTypeDef

```python
# DescribePortalRequestWaitExtraTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribePortalRequestWaitExtraTypeDef


def get_value() -> DescribePortalRequestWaitExtraTypeDef:
    return {
        "portalId": ...,
    }


# DescribePortalRequestWaitExtraTypeDef definition

class DescribePortalRequestWaitExtraTypeDef(TypedDict):
    portalId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribePortalRequestWaitTypeDef

```python
# DescribePortalRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribePortalRequestWaitTypeDef


def get_value() -> DescribePortalRequestWaitTypeDef:
    return {
        "portalId": ...,
    }


# DescribePortalRequestWaitTypeDef definition

class DescribePortalRequestWaitTypeDef(TypedDict):
    portalId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeLoggingOptionsResponseTypeDef

```python
# DescribeLoggingOptionsResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeLoggingOptionsResponseTypeDef


def get_value() -> DescribeLoggingOptionsResponseTypeDef:
    return {
        "loggingOptions": ...,
    }


# DescribeLoggingOptionsResponseTypeDef definition

class DescribeLoggingOptionsResponseTypeDef(TypedDict):
    loggingOptions: LoggingOptionsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoggingOptionsTypeDef](./type_defs.md#loggingoptionstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutLoggingOptionsRequestTypeDef

```python
# PutLoggingOptionsRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import PutLoggingOptionsRequestTypeDef


def get_value() -> PutLoggingOptionsRequestTypeDef:
    return {
        "loggingOptions": ...,
    }


# PutLoggingOptionsRequestTypeDef definition

class PutLoggingOptionsRequestTypeDef(TypedDict):
    loggingOptions: LoggingOptionsTypeDef,  # (1)
```

1. See [:material-code-braces: LoggingOptionsTypeDef](./type_defs.md#loggingoptionstypedef) 
## ErrorDetailsTypeDef

```python
# ErrorDetailsTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ErrorDetailsTypeDef


def get_value() -> ErrorDetailsTypeDef:
    return {
        "code": ...,
    }


# ErrorDetailsTypeDef definition

class ErrorDetailsTypeDef(TypedDict):
    code: ErrorCodeType,  # (1)
    message: str,
    details: NotRequired[List[DetailedErrorTypeDef]],  # (2)
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
2. See [:material-code-braces: DetailedErrorTypeDef](./type_defs.md#detailederrortypedef) 
## ExecuteQueryRequestPaginateTypeDef

```python
# ExecuteQueryRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ExecuteQueryRequestPaginateTypeDef


def get_value() -> ExecuteQueryRequestPaginateTypeDef:
    return {
        "queryStatement": ...,
    }


# ExecuteQueryRequestPaginateTypeDef definition

class ExecuteQueryRequestPaginateTypeDef(TypedDict):
    queryStatement: str,
    clientToken: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetAssetPropertyAggregatesRequestPaginateTypeDef

```python
# GetAssetPropertyAggregatesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import GetAssetPropertyAggregatesRequestPaginateTypeDef


def get_value() -> GetAssetPropertyAggregatesRequestPaginateTypeDef:
    return {
        "aggregateTypes": ...,
    }


# GetAssetPropertyAggregatesRequestPaginateTypeDef definition

class GetAssetPropertyAggregatesRequestPaginateTypeDef(TypedDict):
    aggregateTypes: Sequence[AggregateTypeType],  # (1)
    resolution: str,
    startDate: TimestampTypeDef,
    endDate: TimestampTypeDef,
    assetId: NotRequired[str],
    propertyId: NotRequired[str],
    propertyAlias: NotRequired[str],
    qualities: NotRequired[Sequence[QualityType]],  # (2)
    timeOrdering: NotRequired[TimeOrderingType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: AggregateTypeType](./literals.md#aggregatetypetype) 
2. See [:material-code-brackets: QualityType](./literals.md#qualitytype) 
3. See [:material-code-brackets: TimeOrderingType](./literals.md#timeorderingtype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetAssetPropertyValueHistoryRequestPaginateTypeDef

```python
# GetAssetPropertyValueHistoryRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import GetAssetPropertyValueHistoryRequestPaginateTypeDef


def get_value() -> GetAssetPropertyValueHistoryRequestPaginateTypeDef:
    return {
        "assetId": ...,
    }


# GetAssetPropertyValueHistoryRequestPaginateTypeDef definition

class GetAssetPropertyValueHistoryRequestPaginateTypeDef(TypedDict):
    assetId: NotRequired[str],
    propertyId: NotRequired[str],
    propertyAlias: NotRequired[str],
    startDate: NotRequired[TimestampTypeDef],
    endDate: NotRequired[TimestampTypeDef],
    qualities: NotRequired[Sequence[QualityType]],  # (1)
    timeOrdering: NotRequired[TimeOrderingType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: QualityType](./literals.md#qualitytype) 
2. See [:material-code-brackets: TimeOrderingType](./literals.md#timeorderingtype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetInterpolatedAssetPropertyValuesRequestPaginateTypeDef

```python
# GetInterpolatedAssetPropertyValuesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import GetInterpolatedAssetPropertyValuesRequestPaginateTypeDef


def get_value() -> GetInterpolatedAssetPropertyValuesRequestPaginateTypeDef:
    return {
        "startTimeInSeconds": ...,
    }


# GetInterpolatedAssetPropertyValuesRequestPaginateTypeDef definition

class GetInterpolatedAssetPropertyValuesRequestPaginateTypeDef(TypedDict):
    startTimeInSeconds: int,
    endTimeInSeconds: int,
    quality: QualityType,  # (1)
    intervalInSeconds: int,
    type: str,
    assetId: NotRequired[str],
    propertyId: NotRequired[str],
    propertyAlias: NotRequired[str],
    startTimeOffsetInNanos: NotRequired[int],
    endTimeOffsetInNanos: NotRequired[int],
    intervalWindowInSeconds: NotRequired[int],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: QualityType](./literals.md#qualitytype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAccessPoliciesRequestPaginateTypeDef

```python
# ListAccessPoliciesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListAccessPoliciesRequestPaginateTypeDef


def get_value() -> ListAccessPoliciesRequestPaginateTypeDef:
    return {
        "identityType": ...,
    }


# ListAccessPoliciesRequestPaginateTypeDef definition

class ListAccessPoliciesRequestPaginateTypeDef(TypedDict):
    identityType: NotRequired[IdentityTypeType],  # (1)
    identityId: NotRequired[str],
    resourceType: NotRequired[ResourceTypeType],  # (2)
    resourceId: NotRequired[str],
    iamArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListActionsRequestPaginateTypeDef

```python
# ListActionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListActionsRequestPaginateTypeDef


def get_value() -> ListActionsRequestPaginateTypeDef:
    return {
        "targetResourceType": ...,
    }


# ListActionsRequestPaginateTypeDef definition

class ListActionsRequestPaginateTypeDef(TypedDict):
    targetResourceType: TargetResourceTypeType,  # (1)
    targetResourceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: TargetResourceTypeType](./literals.md#targetresourcetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssetModelCompositeModelsRequestPaginateTypeDef

```python
# ListAssetModelCompositeModelsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListAssetModelCompositeModelsRequestPaginateTypeDef


def get_value() -> ListAssetModelCompositeModelsRequestPaginateTypeDef:
    return {
        "assetModelId": ...,
    }


# ListAssetModelCompositeModelsRequestPaginateTypeDef definition

class ListAssetModelCompositeModelsRequestPaginateTypeDef(TypedDict):
    assetModelId: str,
    assetModelVersion: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssetModelPropertiesRequestPaginateTypeDef

```python
# ListAssetModelPropertiesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListAssetModelPropertiesRequestPaginateTypeDef


def get_value() -> ListAssetModelPropertiesRequestPaginateTypeDef:
    return {
        "assetModelId": ...,
    }


# ListAssetModelPropertiesRequestPaginateTypeDef definition

class ListAssetModelPropertiesRequestPaginateTypeDef(TypedDict):
    assetModelId: str,
    filter: NotRequired[ListAssetModelPropertiesFilterType],  # (1)
    assetModelVersion: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ListAssetModelPropertiesFilterType](./literals.md#listassetmodelpropertiesfiltertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssetModelsRequestPaginateTypeDef

```python
# ListAssetModelsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListAssetModelsRequestPaginateTypeDef


def get_value() -> ListAssetModelsRequestPaginateTypeDef:
    return {
        "assetModelTypes": ...,
    }


# ListAssetModelsRequestPaginateTypeDef definition

class ListAssetModelsRequestPaginateTypeDef(TypedDict):
    assetModelTypes: NotRequired[Sequence[AssetModelTypeType]],  # (1)
    assetModelVersion: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: AssetModelTypeType](./literals.md#assetmodeltypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssetPropertiesRequestPaginateTypeDef

```python
# ListAssetPropertiesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListAssetPropertiesRequestPaginateTypeDef


def get_value() -> ListAssetPropertiesRequestPaginateTypeDef:
    return {
        "assetId": ...,
    }


# ListAssetPropertiesRequestPaginateTypeDef definition

class ListAssetPropertiesRequestPaginateTypeDef(TypedDict):
    assetId: str,
    filter: NotRequired[ListAssetPropertiesFilterType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ListAssetPropertiesFilterType](./literals.md#listassetpropertiesfiltertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssetRelationshipsRequestPaginateTypeDef

```python
# ListAssetRelationshipsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListAssetRelationshipsRequestPaginateTypeDef


def get_value() -> ListAssetRelationshipsRequestPaginateTypeDef:
    return {
        "assetId": ...,
    }


# ListAssetRelationshipsRequestPaginateTypeDef definition

class ListAssetRelationshipsRequestPaginateTypeDef(TypedDict):
    assetId: str,
    traversalType: TraversalTypeType,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: TraversalTypeType](./literals.md#traversaltypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssetsRequestPaginateTypeDef

```python
# ListAssetsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListAssetsRequestPaginateTypeDef


def get_value() -> ListAssetsRequestPaginateTypeDef:
    return {
        "assetModelId": ...,
    }


# ListAssetsRequestPaginateTypeDef definition

class ListAssetsRequestPaginateTypeDef(TypedDict):
    assetModelId: NotRequired[str],
    filter: NotRequired[ListAssetsFilterType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ListAssetsFilterType](./literals.md#listassetsfiltertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssociatedAssetsRequestPaginateTypeDef

```python
# ListAssociatedAssetsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListAssociatedAssetsRequestPaginateTypeDef


def get_value() -> ListAssociatedAssetsRequestPaginateTypeDef:
    return {
        "assetId": ...,
    }


# ListAssociatedAssetsRequestPaginateTypeDef definition

class ListAssociatedAssetsRequestPaginateTypeDef(TypedDict):
    assetId: str,
    hierarchyId: NotRequired[str],
    traversalDirection: NotRequired[TraversalDirectionType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: TraversalDirectionType](./literals.md#traversaldirectiontype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBulkImportJobsRequestPaginateTypeDef

```python
# ListBulkImportJobsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListBulkImportJobsRequestPaginateTypeDef


def get_value() -> ListBulkImportJobsRequestPaginateTypeDef:
    return {
        "filter": ...,
    }


# ListBulkImportJobsRequestPaginateTypeDef definition

class ListBulkImportJobsRequestPaginateTypeDef(TypedDict):
    filter: NotRequired[ListBulkImportJobsFilterType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ListBulkImportJobsFilterType](./literals.md#listbulkimportjobsfiltertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCompositionRelationshipsRequestPaginateTypeDef

```python
# ListCompositionRelationshipsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListCompositionRelationshipsRequestPaginateTypeDef


def get_value() -> ListCompositionRelationshipsRequestPaginateTypeDef:
    return {
        "assetModelId": ...,
    }


# ListCompositionRelationshipsRequestPaginateTypeDef definition

class ListCompositionRelationshipsRequestPaginateTypeDef(TypedDict):
    assetModelId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDashboardsRequestPaginateTypeDef

```python
# ListDashboardsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListDashboardsRequestPaginateTypeDef


def get_value() -> ListDashboardsRequestPaginateTypeDef:
    return {
        "projectId": ...,
    }


# ListDashboardsRequestPaginateTypeDef definition

class ListDashboardsRequestPaginateTypeDef(TypedDict):
    projectId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDatasetsRequestPaginateTypeDef

```python
# ListDatasetsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListDatasetsRequestPaginateTypeDef


def get_value() -> ListDatasetsRequestPaginateTypeDef:
    return {
        "sourceType": ...,
    }


# ListDatasetsRequestPaginateTypeDef definition

class ListDatasetsRequestPaginateTypeDef(TypedDict):
    sourceType: DatasetSourceTypeType,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: DatasetSourceTypeType](./literals.md#datasetsourcetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGatewaysRequestPaginateTypeDef

```python
# ListGatewaysRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListGatewaysRequestPaginateTypeDef


def get_value() -> ListGatewaysRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListGatewaysRequestPaginateTypeDef definition

class ListGatewaysRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPortalsRequestPaginateTypeDef

```python
# ListPortalsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListPortalsRequestPaginateTypeDef


def get_value() -> ListPortalsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListPortalsRequestPaginateTypeDef definition

class ListPortalsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProjectAssetsRequestPaginateTypeDef

```python
# ListProjectAssetsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListProjectAssetsRequestPaginateTypeDef


def get_value() -> ListProjectAssetsRequestPaginateTypeDef:
    return {
        "projectId": ...,
    }


# ListProjectAssetsRequestPaginateTypeDef definition

class ListProjectAssetsRequestPaginateTypeDef(TypedDict):
    projectId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProjectsRequestPaginateTypeDef

```python
# ListProjectsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListProjectsRequestPaginateTypeDef


def get_value() -> ListProjectsRequestPaginateTypeDef:
    return {
        "portalId": ...,
    }


# ListProjectsRequestPaginateTypeDef definition

class ListProjectsRequestPaginateTypeDef(TypedDict):
    portalId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTimeSeriesRequestPaginateTypeDef

```python
# ListTimeSeriesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListTimeSeriesRequestPaginateTypeDef


def get_value() -> ListTimeSeriesRequestPaginateTypeDef:
    return {
        "assetId": ...,
    }


# ListTimeSeriesRequestPaginateTypeDef definition

class ListTimeSeriesRequestPaginateTypeDef(TypedDict):
    assetId: NotRequired[str],
    aliasPrefix: NotRequired[str],
    timeSeriesType: NotRequired[ListTimeSeriesTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ListTimeSeriesTypeType](./literals.md#listtimeseriestypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## MeasurementProcessingConfigTypeDef

```python
# MeasurementProcessingConfigTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import MeasurementProcessingConfigTypeDef


def get_value() -> MeasurementProcessingConfigTypeDef:
    return {
        "forwardingConfig": ...,
    }


# MeasurementProcessingConfigTypeDef definition

class MeasurementProcessingConfigTypeDef(TypedDict):
    forwardingConfig: ForwardingConfigTypeDef,  # (1)
```

1. See [:material-code-braces: ForwardingConfigTypeDef](./type_defs.md#forwardingconfigtypedef) 
## TransformProcessingConfigTypeDef

```python
# TransformProcessingConfigTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import TransformProcessingConfigTypeDef


def get_value() -> TransformProcessingConfigTypeDef:
    return {
        "computeLocation": ...,
    }


# TransformProcessingConfigTypeDef definition

class TransformProcessingConfigTypeDef(TypedDict):
    computeLocation: ComputeLocationType,  # (1)
    forwardingConfig: NotRequired[ForwardingConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ComputeLocationType](./literals.md#computelocationtype) 
2. See [:material-code-braces: ForwardingConfigTypeDef](./type_defs.md#forwardingconfigtypedef) 
## GatewayPlatformTypeDef

```python
# GatewayPlatformTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import GatewayPlatformTypeDef


def get_value() -> GatewayPlatformTypeDef:
    return {
        "greengrass": ...,
    }


# GatewayPlatformTypeDef definition

class GatewayPlatformTypeDef(TypedDict):
    greengrass: NotRequired[GreengrassTypeDef],  # (1)
    greengrassV2: NotRequired[GreengrassV2TypeDef],  # (2)
    siemensIE: NotRequired[SiemensIETypeDef],  # (3)
```

1. See [:material-code-braces: GreengrassTypeDef](./type_defs.md#greengrasstypedef) 
2. See [:material-code-braces: GreengrassV2TypeDef](./type_defs.md#greengrassv2typedef) 
3. See [:material-code-braces: SiemensIETypeDef](./type_defs.md#siemensietypedef) 
## IdentityTypeDef

```python
# IdentityTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import IdentityTypeDef


def get_value() -> IdentityTypeDef:
    return {
        "user": ...,
    }


# IdentityTypeDef definition

class IdentityTypeDef(TypedDict):
    user: NotRequired[UserIdentityTypeDef],  # (1)
    group: NotRequired[GroupIdentityTypeDef],  # (2)
    iamUser: NotRequired[IAMUserIdentityTypeDef],  # (3)
    iamRole: NotRequired[IAMRoleIdentityTypeDef],  # (4)
```

1. See [:material-code-braces: UserIdentityTypeDef](./type_defs.md#useridentitytypedef) 
2. See [:material-code-braces: GroupIdentityTypeDef](./type_defs.md#groupidentitytypedef) 
3. See [:material-code-braces: IAMUserIdentityTypeDef](./type_defs.md#iamuseridentitytypedef) 
4. See [:material-code-braces: IAMRoleIdentityTypeDef](./type_defs.md#iamroleidentitytypedef) 
## ListBulkImportJobsResponseTypeDef

```python
# ListBulkImportJobsResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListBulkImportJobsResponseTypeDef


def get_value() -> ListBulkImportJobsResponseTypeDef:
    return {
        "jobSummaries": ...,
    }


# ListBulkImportJobsResponseTypeDef definition

class ListBulkImportJobsResponseTypeDef(TypedDict):
    jobSummaries: List[JobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: JobSummaryTypeDef](./type_defs.md#jobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SourceDetailTypeDef

```python
# SourceDetailTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import SourceDetailTypeDef


def get_value() -> SourceDetailTypeDef:
    return {
        "kendra": ...,
    }


# SourceDetailTypeDef definition

class SourceDetailTypeDef(TypedDict):
    kendra: NotRequired[KendraSourceDetailTypeDef],  # (1)
```

1. See [:material-code-braces: KendraSourceDetailTypeDef](./type_defs.md#kendrasourcedetailtypedef) 
## ListProjectsResponseTypeDef

```python
# ListProjectsResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListProjectsResponseTypeDef


def get_value() -> ListProjectsResponseTypeDef:
    return {
        "projectSummaries": ...,
    }


# ListProjectsResponseTypeDef definition

class ListProjectsResponseTypeDef(TypedDict):
    projectSummaries: List[ProjectSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ProjectSummaryTypeDef](./type_defs.md#projectsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTimeSeriesResponseTypeDef

```python
# ListTimeSeriesResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListTimeSeriesResponseTypeDef


def get_value() -> ListTimeSeriesResponseTypeDef:
    return {
        "TimeSeriesSummaries": ...,
    }


# ListTimeSeriesResponseTypeDef definition

class ListTimeSeriesResponseTypeDef(TypedDict):
    TimeSeriesSummaries: List[TimeSeriesSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TimeSeriesSummaryTypeDef](./type_defs.md#timeseriessummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SourceTypeDef

```python
# SourceTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import SourceTypeDef


def get_value() -> SourceTypeDef:
    return {
        "arn": ...,
    }


# SourceTypeDef definition

class SourceTypeDef(TypedDict):
    arn: NotRequired[str],
    location: NotRequired[LocationTypeDef],  # (1)
```

1. See [:material-code-braces: LocationTypeDef](./type_defs.md#locationtypedef) 
## MetricWindowTypeDef

```python
# MetricWindowTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import MetricWindowTypeDef


def get_value() -> MetricWindowTypeDef:
    return {
        "tumbling": ...,
    }


# MetricWindowTypeDef definition

class MetricWindowTypeDef(TypedDict):
    tumbling: NotRequired[TumblingWindowTypeDef],  # (1)
```

1. See [:material-code-braces: TumblingWindowTypeDef](./type_defs.md#tumblingwindowtypedef) 
## PortalStatusTypeDef

```python
# PortalStatusTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import PortalStatusTypeDef


def get_value() -> PortalStatusTypeDef:
    return {
        "state": ...,
    }


# PortalStatusTypeDef definition

class PortalStatusTypeDef(TypedDict):
    state: PortalStateType,  # (1)
    error: NotRequired[MonitorErrorDetailsTypeDef],  # (2)
```

1. See [:material-code-brackets: PortalStateType](./literals.md#portalstatetype) 
2. See [:material-code-braces: MonitorErrorDetailsTypeDef](./type_defs.md#monitorerrordetailstypedef) 
## ResourceTypeDef

```python
# ResourceTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ResourceTypeDef


def get_value() -> ResourceTypeDef:
    return {
        "portal": ...,
    }


# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    portal: NotRequired[PortalResourceTypeDef],  # (1)
    project: NotRequired[ProjectResourceTypeDef],  # (2)
```

1. See [:material-code-braces: PortalResourceTypeDef](./type_defs.md#portalresourcetypedef) 
2. See [:material-code-braces: ProjectResourceTypeDef](./type_defs.md#projectresourcetypedef) 
## VariantTypeDef

```python
# VariantTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import VariantTypeDef


def get_value() -> VariantTypeDef:
    return {
        "stringValue": ...,
    }


# VariantTypeDef definition

class VariantTypeDef(TypedDict):
    stringValue: NotRequired[str],
    integerValue: NotRequired[int],
    doubleValue: NotRequired[float],
    booleanValue: NotRequired[bool],
    nullValue: NotRequired[PropertyValueNullValueTypeDef],  # (1)
```

1. See [:material-code-braces: PropertyValueNullValueTypeDef](./type_defs.md#propertyvaluenullvaluetypedef) 
## ListActionsResponseTypeDef

```python
# ListActionsResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListActionsResponseTypeDef


def get_value() -> ListActionsResponseTypeDef:
    return {
        "actionSummaries": ...,
    }


# ListActionsResponseTypeDef definition

class ListActionsResponseTypeDef(TypedDict):
    actionSummaries: List[ActionSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ActionSummaryTypeDef](./type_defs.md#actionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetAssetPropertyAggregatesSuccessEntryTypeDef

```python
# BatchGetAssetPropertyAggregatesSuccessEntryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import BatchGetAssetPropertyAggregatesSuccessEntryTypeDef


def get_value() -> BatchGetAssetPropertyAggregatesSuccessEntryTypeDef:
    return {
        "entryId": ...,
    }


# BatchGetAssetPropertyAggregatesSuccessEntryTypeDef definition

class BatchGetAssetPropertyAggregatesSuccessEntryTypeDef(TypedDict):
    entryId: str,
    aggregatedValues: List[AggregatedValueTypeDef],  # (1)
```

1. See [:material-code-braces: AggregatedValueTypeDef](./type_defs.md#aggregatedvaluetypedef) 
## GetAssetPropertyAggregatesResponseTypeDef

```python
# GetAssetPropertyAggregatesResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import GetAssetPropertyAggregatesResponseTypeDef


def get_value() -> GetAssetPropertyAggregatesResponseTypeDef:
    return {
        "aggregatedValues": ...,
    }


# GetAssetPropertyAggregatesResponseTypeDef definition

class GetAssetPropertyAggregatesResponseTypeDef(TypedDict):
    aggregatedValues: List[AggregatedValueTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AggregatedValueTypeDef](./type_defs.md#aggregatedvaluetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssetRelationshipsResponseTypeDef

```python
# ListAssetRelationshipsResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListAssetRelationshipsResponseTypeDef


def get_value() -> ListAssetRelationshipsResponseTypeDef:
    return {
        "assetRelationshipSummaries": ...,
    }


# ListAssetRelationshipsResponseTypeDef definition

class ListAssetRelationshipsResponseTypeDef(TypedDict):
    assetRelationshipSummaries: List[AssetRelationshipSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AssetRelationshipSummaryTypeDef](./type_defs.md#assetrelationshipsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssetModelCompositeModelsResponseTypeDef

```python
# ListAssetModelCompositeModelsResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListAssetModelCompositeModelsResponseTypeDef


def get_value() -> ListAssetModelCompositeModelsResponseTypeDef:
    return {
        "assetModelCompositeModelSummaries": ...,
    }


# ListAssetModelCompositeModelsResponseTypeDef definition

class ListAssetModelCompositeModelsResponseTypeDef(TypedDict):
    assetModelCompositeModelSummaries: List[AssetModelCompositeModelSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AssetModelCompositeModelSummaryTypeDef](./type_defs.md#assetmodelcompositemodelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExpressionVariableOutputTypeDef

```python
# ExpressionVariableOutputTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ExpressionVariableOutputTypeDef


def get_value() -> ExpressionVariableOutputTypeDef:
    return {
        "name": ...,
    }


# ExpressionVariableOutputTypeDef definition

class ExpressionVariableOutputTypeDef(TypedDict):
    name: str,
    value: VariableValueOutputTypeDef,  # (1)
```

1. See [:material-code-braces: VariableValueOutputTypeDef](./type_defs.md#variablevalueoutputtypedef) 
## ListAssetPropertiesResponseTypeDef

```python
# ListAssetPropertiesResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListAssetPropertiesResponseTypeDef


def get_value() -> ListAssetPropertiesResponseTypeDef:
    return {
        "assetPropertySummaries": ...,
    }


# ListAssetPropertiesResponseTypeDef definition

class ListAssetPropertiesResponseTypeDef(TypedDict):
    assetPropertySummaries: List[AssetPropertySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AssetPropertySummaryTypeDef](./type_defs.md#assetpropertysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssetCompositeModelTypeDef

```python
# AssetCompositeModelTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AssetCompositeModelTypeDef


def get_value() -> AssetCompositeModelTypeDef:
    return {
        "name": ...,
    }


# AssetCompositeModelTypeDef definition

class AssetCompositeModelTypeDef(TypedDict):
    name: str,
    type: str,
    properties: List[AssetPropertyTypeDef],  # (1)
    description: NotRequired[str],
    id: NotRequired[str],
    externalId: NotRequired[str],
```

1. See [:material-code-braces: AssetPropertyTypeDef](./type_defs.md#assetpropertytypedef) 
## DescribeAssetCompositeModelResponseTypeDef

```python
# DescribeAssetCompositeModelResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeAssetCompositeModelResponseTypeDef


def get_value() -> DescribeAssetCompositeModelResponseTypeDef:
    return {
        "assetId": ...,
    }


# DescribeAssetCompositeModelResponseTypeDef definition

class DescribeAssetCompositeModelResponseTypeDef(TypedDict):
    assetId: str,
    assetCompositeModelId: str,
    assetCompositeModelExternalId: str,
    assetCompositeModelPath: List[AssetCompositeModelPathSegmentTypeDef],  # (1)
    assetCompositeModelName: str,
    assetCompositeModelDescription: str,
    assetCompositeModelType: str,
    assetCompositeModelProperties: List[AssetPropertyTypeDef],  # (2)
    assetCompositeModelSummaries: List[AssetCompositeModelSummaryTypeDef],  # (3)
    actionDefinitions: List[ActionDefinitionTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: AssetCompositeModelPathSegmentTypeDef](./type_defs.md#assetcompositemodelpathsegmenttypedef) 
2. See [:material-code-braces: AssetPropertyTypeDef](./type_defs.md#assetpropertytypedef) 
3. See [:material-code-braces: AssetCompositeModelSummaryTypeDef](./type_defs.md#assetcompositemodelsummarytypedef) 
4. See [:material-code-braces: ActionDefinitionTypeDef](./type_defs.md#actiondefinitiontypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchPutAssetPropertyErrorEntryTypeDef

```python
# BatchPutAssetPropertyErrorEntryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import BatchPutAssetPropertyErrorEntryTypeDef


def get_value() -> BatchPutAssetPropertyErrorEntryTypeDef:
    return {
        "entryId": ...,
    }


# BatchPutAssetPropertyErrorEntryTypeDef definition

class BatchPutAssetPropertyErrorEntryTypeDef(TypedDict):
    entryId: str,
    errors: List[BatchPutAssetPropertyErrorTypeDef],  # (1)
```

1. See [:material-code-braces: BatchPutAssetPropertyErrorTypeDef](./type_defs.md#batchputassetpropertyerrortypedef) 
## BatchGetAssetPropertyAggregatesRequestTypeDef

```python
# BatchGetAssetPropertyAggregatesRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import BatchGetAssetPropertyAggregatesRequestTypeDef


def get_value() -> BatchGetAssetPropertyAggregatesRequestTypeDef:
    return {
        "entries": ...,
    }


# BatchGetAssetPropertyAggregatesRequestTypeDef definition

class BatchGetAssetPropertyAggregatesRequestTypeDef(TypedDict):
    entries: Sequence[BatchGetAssetPropertyAggregatesEntryTypeDef],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: BatchGetAssetPropertyAggregatesEntryTypeDef](./type_defs.md#batchgetassetpropertyaggregatesentrytypedef) 
## BatchGetAssetPropertyValueHistoryRequestTypeDef

```python
# BatchGetAssetPropertyValueHistoryRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import BatchGetAssetPropertyValueHistoryRequestTypeDef


def get_value() -> BatchGetAssetPropertyValueHistoryRequestTypeDef:
    return {
        "entries": ...,
    }


# BatchGetAssetPropertyValueHistoryRequestTypeDef definition

class BatchGetAssetPropertyValueHistoryRequestTypeDef(TypedDict):
    entries: Sequence[BatchGetAssetPropertyValueHistoryEntryTypeDef],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: BatchGetAssetPropertyValueHistoryEntryTypeDef](./type_defs.md#batchgetassetpropertyvaluehistoryentrytypedef) 
## ImageTypeDef

```python
# ImageTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ImageTypeDef


def get_value() -> ImageTypeDef:
    return {
        "id": ...,
    }


# ImageTypeDef definition

class ImageTypeDef(TypedDict):
    id: NotRequired[str],
    file: NotRequired[ImageFileTypeDef],  # (1)
```

1. See [:material-code-braces: ImageFileTypeDef](./type_defs.md#imagefiletypedef) 
## DescribeDefaultEncryptionConfigurationResponseTypeDef

```python
# DescribeDefaultEncryptionConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeDefaultEncryptionConfigurationResponseTypeDef


def get_value() -> DescribeDefaultEncryptionConfigurationResponseTypeDef:
    return {
        "encryptionType": ...,
    }


# DescribeDefaultEncryptionConfigurationResponseTypeDef definition

class DescribeDefaultEncryptionConfigurationResponseTypeDef(TypedDict):
    encryptionType: EncryptionTypeType,  # (1)
    kmsKeyArn: str,
    configurationStatus: ConfigurationStatusTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
2. See [:material-code-braces: ConfigurationStatusTypeDef](./type_defs.md#configurationstatustypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutDefaultEncryptionConfigurationResponseTypeDef

```python
# PutDefaultEncryptionConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import PutDefaultEncryptionConfigurationResponseTypeDef


def get_value() -> PutDefaultEncryptionConfigurationResponseTypeDef:
    return {
        "encryptionType": ...,
    }


# PutDefaultEncryptionConfigurationResponseTypeDef definition

class PutDefaultEncryptionConfigurationResponseTypeDef(TypedDict):
    encryptionType: EncryptionTypeType,  # (1)
    kmsKeyArn: str,
    configurationStatus: ConfigurationStatusTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
2. See [:material-code-braces: ConfigurationStatusTypeDef](./type_defs.md#configurationstatustypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## JobConfigurationOutputTypeDef

```python
# JobConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import JobConfigurationOutputTypeDef


def get_value() -> JobConfigurationOutputTypeDef:
    return {
        "fileFormat": ...,
    }


# JobConfigurationOutputTypeDef definition

class JobConfigurationOutputTypeDef(TypedDict):
    fileFormat: FileFormatOutputTypeDef,  # (1)
```

1. See [:material-code-braces: FileFormatOutputTypeDef](./type_defs.md#fileformatoutputtypedef) 
## JobConfigurationTypeDef

```python
# JobConfigurationTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import JobConfigurationTypeDef


def get_value() -> JobConfigurationTypeDef:
    return {
        "fileFormat": ...,
    }


# JobConfigurationTypeDef definition

class JobConfigurationTypeDef(TypedDict):
    fileFormat: FileFormatTypeDef,  # (1)
```

1. See [:material-code-braces: FileFormatTypeDef](./type_defs.md#fileformattypedef) 
## DescribeStorageConfigurationResponseTypeDef

```python
# DescribeStorageConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeStorageConfigurationResponseTypeDef


def get_value() -> DescribeStorageConfigurationResponseTypeDef:
    return {
        "storageType": ...,
    }


# DescribeStorageConfigurationResponseTypeDef definition

class DescribeStorageConfigurationResponseTypeDef(TypedDict):
    storageType: StorageTypeType,  # (1)
    multiLayerStorage: MultiLayerStorageTypeDef,  # (2)
    disassociatedDataStorage: DisassociatedDataStorageStateType,  # (3)
    retentionPeriod: RetentionPeriodTypeDef,  # (4)
    configurationStatus: ConfigurationStatusTypeDef,  # (5)
    lastUpdateDate: datetime,
    warmTier: WarmTierStateType,  # (6)
    warmTierRetentionPeriod: WarmTierRetentionPeriodTypeDef,  # (7)
    disallowIngestNullNaN: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-brackets: StorageTypeType](./literals.md#storagetypetype) 
2. See [:material-code-braces: MultiLayerStorageTypeDef](./type_defs.md#multilayerstoragetypedef) 
3. See [:material-code-brackets: DisassociatedDataStorageStateType](./literals.md#disassociateddatastoragestatetype) 
4. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
5. See [:material-code-braces: ConfigurationStatusTypeDef](./type_defs.md#configurationstatustypedef) 
6. See [:material-code-brackets: WarmTierStateType](./literals.md#warmtierstatetype) 
7. See [:material-code-braces: WarmTierRetentionPeriodTypeDef](./type_defs.md#warmtierretentionperiodtypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutStorageConfigurationRequestTypeDef

```python
# PutStorageConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import PutStorageConfigurationRequestTypeDef


def get_value() -> PutStorageConfigurationRequestTypeDef:
    return {
        "storageType": ...,
    }


# PutStorageConfigurationRequestTypeDef definition

class PutStorageConfigurationRequestTypeDef(TypedDict):
    storageType: StorageTypeType,  # (1)
    multiLayerStorage: NotRequired[MultiLayerStorageTypeDef],  # (2)
    disassociatedDataStorage: NotRequired[DisassociatedDataStorageStateType],  # (3)
    retentionPeriod: NotRequired[RetentionPeriodTypeDef],  # (4)
    warmTier: NotRequired[WarmTierStateType],  # (5)
    warmTierRetentionPeriod: NotRequired[WarmTierRetentionPeriodTypeDef],  # (6)
    disallowIngestNullNaN: NotRequired[bool],
```

1. See [:material-code-brackets: StorageTypeType](./literals.md#storagetypetype) 
2. See [:material-code-braces: MultiLayerStorageTypeDef](./type_defs.md#multilayerstoragetypedef) 
3. See [:material-code-brackets: DisassociatedDataStorageStateType](./literals.md#disassociateddatastoragestatetype) 
4. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
5. See [:material-code-brackets: WarmTierStateType](./literals.md#warmtierstatetype) 
6. See [:material-code-braces: WarmTierRetentionPeriodTypeDef](./type_defs.md#warmtierretentionperiodtypedef) 
## PutStorageConfigurationResponseTypeDef

```python
# PutStorageConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import PutStorageConfigurationResponseTypeDef


def get_value() -> PutStorageConfigurationResponseTypeDef:
    return {
        "storageType": ...,
    }


# PutStorageConfigurationResponseTypeDef definition

class PutStorageConfigurationResponseTypeDef(TypedDict):
    storageType: StorageTypeType,  # (1)
    multiLayerStorage: MultiLayerStorageTypeDef,  # (2)
    disassociatedDataStorage: DisassociatedDataStorageStateType,  # (3)
    retentionPeriod: RetentionPeriodTypeDef,  # (4)
    configurationStatus: ConfigurationStatusTypeDef,  # (5)
    warmTier: WarmTierStateType,  # (6)
    warmTierRetentionPeriod: WarmTierRetentionPeriodTypeDef,  # (7)
    disallowIngestNullNaN: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-brackets: StorageTypeType](./literals.md#storagetypetype) 
2. See [:material-code-braces: MultiLayerStorageTypeDef](./type_defs.md#multilayerstoragetypedef) 
3. See [:material-code-brackets: DisassociatedDataStorageStateType](./literals.md#disassociateddatastoragestatetype) 
4. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
5. See [:material-code-braces: ConfigurationStatusTypeDef](./type_defs.md#configurationstatustypedef) 
6. See [:material-code-brackets: WarmTierStateType](./literals.md#warmtierstatetype) 
7. See [:material-code-braces: WarmTierRetentionPeriodTypeDef](./type_defs.md#warmtierretentionperiodtypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExecuteQueryResponsePaginatorTypeDef

```python
# ExecuteQueryResponsePaginatorTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ExecuteQueryResponsePaginatorTypeDef


def get_value() -> ExecuteQueryResponsePaginatorTypeDef:
    return {
        "columns": ...,
    }


# ExecuteQueryResponsePaginatorTypeDef definition

class ExecuteQueryResponsePaginatorTypeDef(TypedDict):
    columns: List[ColumnInfoTypeDef],  # (1)
    rows: List[RowPaginatorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ColumnInfoTypeDef](./type_defs.md#columninfotypedef) 
2. See [:material-code-braces: RowPaginatorTypeDef](./type_defs.md#rowpaginatortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExecuteQueryResponseTypeDef

```python
# ExecuteQueryResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ExecuteQueryResponseTypeDef


def get_value() -> ExecuteQueryResponseTypeDef:
    return {
        "columns": ...,
    }


# ExecuteQueryResponseTypeDef definition

class ExecuteQueryResponseTypeDef(TypedDict):
    columns: List[ColumnInfoTypeDef],  # (1)
    rows: List[RowTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ColumnInfoTypeDef](./type_defs.md#columninfotypedef) 
2. See [:material-code-braces: RowTypeDef](./type_defs.md#rowtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExecuteQueryResponseWaiterTypeDef

```python
# ExecuteQueryResponseWaiterTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ExecuteQueryResponseWaiterTypeDef


def get_value() -> ExecuteQueryResponseWaiterTypeDef:
    return {
        "columns": ...,
    }


# ExecuteQueryResponseWaiterTypeDef definition

class ExecuteQueryResponseWaiterTypeDef(TypedDict):
    columns: List[ColumnInfoTypeDef],  # (1)
    rows: List[RowWaiterTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ColumnInfoTypeDef](./type_defs.md#columninfotypedef) 
2. See [:material-code-braces: RowWaiterTypeDef](./type_defs.md#rowwaitertypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssetModelStatusTypeDef

```python
# AssetModelStatusTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AssetModelStatusTypeDef


def get_value() -> AssetModelStatusTypeDef:
    return {
        "state": ...,
    }


# AssetModelStatusTypeDef definition

class AssetModelStatusTypeDef(TypedDict):
    state: AssetModelStateType,  # (1)
    error: NotRequired[ErrorDetailsTypeDef],  # (2)
```

1. See [:material-code-brackets: AssetModelStateType](./literals.md#assetmodelstatetype) 
2. See [:material-code-braces: ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef) 
## AssetStatusTypeDef

```python
# AssetStatusTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AssetStatusTypeDef


def get_value() -> AssetStatusTypeDef:
    return {
        "state": ...,
    }


# AssetStatusTypeDef definition

class AssetStatusTypeDef(TypedDict):
    state: AssetStateType,  # (1)
    error: NotRequired[ErrorDetailsTypeDef],  # (2)
```

1. See [:material-code-brackets: AssetStateType](./literals.md#assetstatetype) 
2. See [:material-code-braces: ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef) 
## DatasetStatusTypeDef

```python
# DatasetStatusTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DatasetStatusTypeDef


def get_value() -> DatasetStatusTypeDef:
    return {
        "state": ...,
    }


# DatasetStatusTypeDef definition

class DatasetStatusTypeDef(TypedDict):
    state: DatasetStateType,  # (1)
    error: NotRequired[ErrorDetailsTypeDef],  # (2)
```

1. See [:material-code-brackets: DatasetStateType](./literals.md#datasetstatetype) 
2. See [:material-code-braces: ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef) 
## MeasurementTypeDef

```python
# MeasurementTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import MeasurementTypeDef


def get_value() -> MeasurementTypeDef:
    return {
        "processingConfig": ...,
    }


# MeasurementTypeDef definition

class MeasurementTypeDef(TypedDict):
    processingConfig: NotRequired[MeasurementProcessingConfigTypeDef],  # (1)
```

1. See [:material-code-braces: MeasurementProcessingConfigTypeDef](./type_defs.md#measurementprocessingconfigtypedef) 
## CreateGatewayRequestTypeDef

```python
# CreateGatewayRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import CreateGatewayRequestTypeDef


def get_value() -> CreateGatewayRequestTypeDef:
    return {
        "gatewayName": ...,
    }


# CreateGatewayRequestTypeDef definition

class CreateGatewayRequestTypeDef(TypedDict):
    gatewayName: str,
    gatewayPlatform: GatewayPlatformTypeDef,  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: GatewayPlatformTypeDef](./type_defs.md#gatewayplatformtypedef) 
## DescribeGatewayResponseTypeDef

```python
# DescribeGatewayResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeGatewayResponseTypeDef


def get_value() -> DescribeGatewayResponseTypeDef:
    return {
        "gatewayId": ...,
    }


# DescribeGatewayResponseTypeDef definition

class DescribeGatewayResponseTypeDef(TypedDict):
    gatewayId: str,
    gatewayName: str,
    gatewayArn: str,
    gatewayPlatform: GatewayPlatformTypeDef,  # (1)
    gatewayCapabilitySummaries: List[GatewayCapabilitySummaryTypeDef],  # (2)
    creationDate: datetime,
    lastUpdateDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: GatewayPlatformTypeDef](./type_defs.md#gatewayplatformtypedef) 
2. See [:material-code-braces: GatewayCapabilitySummaryTypeDef](./type_defs.md#gatewaycapabilitysummarytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GatewaySummaryTypeDef

```python
# GatewaySummaryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import GatewaySummaryTypeDef


def get_value() -> GatewaySummaryTypeDef:
    return {
        "gatewayId": ...,
    }


# GatewaySummaryTypeDef definition

class GatewaySummaryTypeDef(TypedDict):
    gatewayId: str,
    gatewayName: str,
    creationDate: datetime,
    lastUpdateDate: datetime,
    gatewayPlatform: NotRequired[GatewayPlatformTypeDef],  # (1)
    gatewayCapabilitySummaries: NotRequired[List[GatewayCapabilitySummaryTypeDef]],  # (2)
```

1. See [:material-code-braces: GatewayPlatformTypeDef](./type_defs.md#gatewayplatformtypedef) 
2. See [:material-code-braces: GatewayCapabilitySummaryTypeDef](./type_defs.md#gatewaycapabilitysummarytypedef) 
## DatasetSourceTypeDef

```python
# DatasetSourceTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DatasetSourceTypeDef


def get_value() -> DatasetSourceTypeDef:
    return {
        "sourceType": ...,
    }


# DatasetSourceTypeDef definition

class DatasetSourceTypeDef(TypedDict):
    sourceType: DatasetSourceTypeType,  # (1)
    sourceFormat: DatasetSourceFormatType,  # (2)
    sourceDetail: NotRequired[SourceDetailTypeDef],  # (3)
```

1. See [:material-code-brackets: DatasetSourceTypeType](./literals.md#datasetsourcetypetype) 
2. See [:material-code-brackets: DatasetSourceFormatType](./literals.md#datasetsourceformattype) 
3. See [:material-code-braces: SourceDetailTypeDef](./type_defs.md#sourcedetailtypedef) 
## DataSetReferenceTypeDef

```python
# DataSetReferenceTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DataSetReferenceTypeDef


def get_value() -> DataSetReferenceTypeDef:
    return {
        "datasetArn": ...,
    }


# DataSetReferenceTypeDef definition

class DataSetReferenceTypeDef(TypedDict):
    datasetArn: NotRequired[str],
    source: NotRequired[SourceTypeDef],  # (1)
```

1. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
## CreatePortalResponseTypeDef

```python
# CreatePortalResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import CreatePortalResponseTypeDef


def get_value() -> CreatePortalResponseTypeDef:
    return {
        "portalId": ...,
    }


# CreatePortalResponseTypeDef definition

class CreatePortalResponseTypeDef(TypedDict):
    portalId: str,
    portalArn: str,
    portalStartUrl: str,
    portalStatus: PortalStatusTypeDef,  # (1)
    ssoApplicationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PortalStatusTypeDef](./type_defs.md#portalstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeletePortalResponseTypeDef

```python
# DeletePortalResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DeletePortalResponseTypeDef


def get_value() -> DeletePortalResponseTypeDef:
    return {
        "portalStatus": ...,
    }


# DeletePortalResponseTypeDef definition

class DeletePortalResponseTypeDef(TypedDict):
    portalStatus: PortalStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PortalStatusTypeDef](./type_defs.md#portalstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePortalResponseTypeDef

```python
# DescribePortalResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribePortalResponseTypeDef


def get_value() -> DescribePortalResponseTypeDef:
    return {
        "portalId": ...,
    }


# DescribePortalResponseTypeDef definition

class DescribePortalResponseTypeDef(TypedDict):
    portalId: str,
    portalArn: str,
    portalName: str,
    portalDescription: str,
    portalClientId: str,
    portalStartUrl: str,
    portalContactEmail: str,
    portalStatus: PortalStatusTypeDef,  # (1)
    portalCreationDate: datetime,
    portalLastUpdateDate: datetime,
    portalLogoImageLocation: ImageLocationTypeDef,  # (2)
    roleArn: str,
    portalAuthMode: AuthModeType,  # (3)
    notificationSenderEmail: str,
    alarms: AlarmsTypeDef,  # (4)
    portalType: PortalTypeType,  # (5)
    portalTypeConfiguration: Dict[str, PortalTypeEntryOutputTypeDef],  # (6)
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-braces: PortalStatusTypeDef](./type_defs.md#portalstatustypedef) 
2. See [:material-code-braces: ImageLocationTypeDef](./type_defs.md#imagelocationtypedef) 
3. See [:material-code-brackets: AuthModeType](./literals.md#authmodetype) 
4. See [:material-code-braces: AlarmsTypeDef](./type_defs.md#alarmstypedef) 
5. See [:material-code-brackets: PortalTypeType](./literals.md#portaltypetype) 
6. See [:material-code-braces: PortalTypeEntryOutputTypeDef](./type_defs.md#portaltypeentryoutputtypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PortalSummaryTypeDef

```python
# PortalSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import PortalSummaryTypeDef


def get_value() -> PortalSummaryTypeDef:
    return {
        "id": ...,
    }


# PortalSummaryTypeDef definition

class PortalSummaryTypeDef(TypedDict):
    id: str,
    name: str,
    startUrl: str,
    status: PortalStatusTypeDef,  # (1)
    description: NotRequired[str],
    creationDate: NotRequired[datetime],
    lastUpdateDate: NotRequired[datetime],
    roleArn: NotRequired[str],
    portalType: NotRequired[PortalTypeType],  # (2)
```

1. See [:material-code-braces: PortalStatusTypeDef](./type_defs.md#portalstatustypedef) 
2. See [:material-code-brackets: PortalTypeType](./literals.md#portaltypetype) 
## UpdatePortalResponseTypeDef

```python
# UpdatePortalResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import UpdatePortalResponseTypeDef


def get_value() -> UpdatePortalResponseTypeDef:
    return {
        "portalStatus": ...,
    }


# UpdatePortalResponseTypeDef definition

class UpdatePortalResponseTypeDef(TypedDict):
    portalStatus: PortalStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PortalStatusTypeDef](./type_defs.md#portalstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePortalRequestTypeDef

```python
# CreatePortalRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import CreatePortalRequestTypeDef


def get_value() -> CreatePortalRequestTypeDef:
    return {
        "portalName": ...,
    }


# CreatePortalRequestTypeDef definition

class CreatePortalRequestTypeDef(TypedDict):
    portalName: str,
    portalContactEmail: str,
    roleArn: str,
    portalDescription: NotRequired[str],
    clientToken: NotRequired[str],
    portalLogoImageFile: NotRequired[ImageFileTypeDef],  # (1)
    tags: NotRequired[Mapping[str, str]],
    portalAuthMode: NotRequired[AuthModeType],  # (2)
    notificationSenderEmail: NotRequired[str],
    alarms: NotRequired[AlarmsTypeDef],  # (3)
    portalType: NotRequired[PortalTypeType],  # (4)
    portalTypeConfiguration: NotRequired[Mapping[str, PortalTypeEntryUnionTypeDef]],  # (5)
```

1. See [:material-code-braces: ImageFileTypeDef](./type_defs.md#imagefiletypedef) 
2. See [:material-code-brackets: AuthModeType](./literals.md#authmodetype) 
3. See [:material-code-braces: AlarmsTypeDef](./type_defs.md#alarmstypedef) 
4. See [:material-code-brackets: PortalTypeType](./literals.md#portaltypetype) 
5. See [:material-code-braces: PortalTypeEntryTypeDef](./type_defs.md#portaltypeentrytypedef) [:material-code-braces: PortalTypeEntryOutputTypeDef](./type_defs.md#portaltypeentryoutputtypedef) 
## AccessPolicySummaryTypeDef

```python
# AccessPolicySummaryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AccessPolicySummaryTypeDef


def get_value() -> AccessPolicySummaryTypeDef:
    return {
        "id": ...,
    }


# AccessPolicySummaryTypeDef definition

class AccessPolicySummaryTypeDef(TypedDict):
    id: str,
    identity: IdentityTypeDef,  # (1)
    resource: ResourceTypeDef,  # (2)
    permission: PermissionType,  # (3)
    creationDate: NotRequired[datetime],
    lastUpdateDate: NotRequired[datetime],
```

1. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
2. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
3. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
## CreateAccessPolicyRequestTypeDef

```python
# CreateAccessPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import CreateAccessPolicyRequestTypeDef


def get_value() -> CreateAccessPolicyRequestTypeDef:
    return {
        "accessPolicyIdentity": ...,
    }


# CreateAccessPolicyRequestTypeDef definition

class CreateAccessPolicyRequestTypeDef(TypedDict):
    accessPolicyIdentity: IdentityTypeDef,  # (1)
    accessPolicyResource: ResourceTypeDef,  # (2)
    accessPolicyPermission: PermissionType,  # (3)
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
2. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
3. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
## DescribeAccessPolicyResponseTypeDef

```python
# DescribeAccessPolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeAccessPolicyResponseTypeDef


def get_value() -> DescribeAccessPolicyResponseTypeDef:
    return {
        "accessPolicyId": ...,
    }


# DescribeAccessPolicyResponseTypeDef definition

class DescribeAccessPolicyResponseTypeDef(TypedDict):
    accessPolicyId: str,
    accessPolicyArn: str,
    accessPolicyIdentity: IdentityTypeDef,  # (1)
    accessPolicyResource: ResourceTypeDef,  # (2)
    accessPolicyPermission: PermissionType,  # (3)
    accessPolicyCreationDate: datetime,
    accessPolicyLastUpdateDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
2. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
3. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAccessPolicyRequestTypeDef

```python
# UpdateAccessPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import UpdateAccessPolicyRequestTypeDef


def get_value() -> UpdateAccessPolicyRequestTypeDef:
    return {
        "accessPolicyId": ...,
    }


# UpdateAccessPolicyRequestTypeDef definition

class UpdateAccessPolicyRequestTypeDef(TypedDict):
    accessPolicyId: str,
    accessPolicyIdentity: IdentityTypeDef,  # (1)
    accessPolicyResource: ResourceTypeDef,  # (2)
    accessPolicyPermission: PermissionType,  # (3)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
2. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
3. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
## AssetPropertyValueTypeDef

```python
# AssetPropertyValueTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AssetPropertyValueTypeDef


def get_value() -> AssetPropertyValueTypeDef:
    return {
        "value": ...,
    }


# AssetPropertyValueTypeDef definition

class AssetPropertyValueTypeDef(TypedDict):
    value: VariantTypeDef,  # (1)
    timestamp: TimeInNanosTypeDef,  # (2)
    quality: NotRequired[QualityType],  # (3)
```

1. See [:material-code-braces: VariantTypeDef](./type_defs.md#varianttypedef) 
2. See [:material-code-braces: TimeInNanosTypeDef](./type_defs.md#timeinnanostypedef) 
3. See [:material-code-brackets: QualityType](./literals.md#qualitytype) 
## InterpolatedAssetPropertyValueTypeDef

```python
# InterpolatedAssetPropertyValueTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import InterpolatedAssetPropertyValueTypeDef


def get_value() -> InterpolatedAssetPropertyValueTypeDef:
    return {
        "timestamp": ...,
    }


# InterpolatedAssetPropertyValueTypeDef definition

class InterpolatedAssetPropertyValueTypeDef(TypedDict):
    timestamp: TimeInNanosTypeDef,  # (1)
    value: VariantTypeDef,  # (2)
```

1. See [:material-code-braces: TimeInNanosTypeDef](./type_defs.md#timeinnanostypedef) 
2. See [:material-code-braces: VariantTypeDef](./type_defs.md#varianttypedef) 
## BatchGetAssetPropertyAggregatesResponseTypeDef

```python
# BatchGetAssetPropertyAggregatesResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import BatchGetAssetPropertyAggregatesResponseTypeDef


def get_value() -> BatchGetAssetPropertyAggregatesResponseTypeDef:
    return {
        "errorEntries": ...,
    }


# BatchGetAssetPropertyAggregatesResponseTypeDef definition

class BatchGetAssetPropertyAggregatesResponseTypeDef(TypedDict):
    errorEntries: List[BatchGetAssetPropertyAggregatesErrorEntryTypeDef],  # (1)
    successEntries: List[BatchGetAssetPropertyAggregatesSuccessEntryTypeDef],  # (2)
    skippedEntries: List[BatchGetAssetPropertyAggregatesSkippedEntryTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BatchGetAssetPropertyAggregatesErrorEntryTypeDef](./type_defs.md#batchgetassetpropertyaggregateserrorentrytypedef) 
2. See [:material-code-braces: BatchGetAssetPropertyAggregatesSuccessEntryTypeDef](./type_defs.md#batchgetassetpropertyaggregatessuccessentrytypedef) 
3. See [:material-code-braces: BatchGetAssetPropertyAggregatesSkippedEntryTypeDef](./type_defs.md#batchgetassetpropertyaggregatesskippedentrytypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MetricOutputTypeDef

```python
# MetricOutputTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import MetricOutputTypeDef


def get_value() -> MetricOutputTypeDef:
    return {
        "expression": ...,
    }


# MetricOutputTypeDef definition

class MetricOutputTypeDef(TypedDict):
    expression: str,
    variables: List[ExpressionVariableOutputTypeDef],  # (1)
    window: MetricWindowTypeDef,  # (2)
    processingConfig: NotRequired[MetricProcessingConfigTypeDef],  # (3)
```

1. See [:material-code-braces: ExpressionVariableOutputTypeDef](./type_defs.md#expressionvariableoutputtypedef) 
2. See [:material-code-braces: MetricWindowTypeDef](./type_defs.md#metricwindowtypedef) 
3. See [:material-code-braces: MetricProcessingConfigTypeDef](./type_defs.md#metricprocessingconfigtypedef) 
## TransformOutputTypeDef

```python
# TransformOutputTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import TransformOutputTypeDef


def get_value() -> TransformOutputTypeDef:
    return {
        "expression": ...,
    }


# TransformOutputTypeDef definition

class TransformOutputTypeDef(TypedDict):
    expression: str,
    variables: List[ExpressionVariableOutputTypeDef],  # (1)
    processingConfig: NotRequired[TransformProcessingConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ExpressionVariableOutputTypeDef](./type_defs.md#expressionvariableoutputtypedef) 
2. See [:material-code-braces: TransformProcessingConfigTypeDef](./type_defs.md#transformprocessingconfigtypedef) 
## ExpressionVariableTypeDef

```python
# ExpressionVariableTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ExpressionVariableTypeDef


def get_value() -> ExpressionVariableTypeDef:
    return {
        "name": ...,
    }


# ExpressionVariableTypeDef definition

class ExpressionVariableTypeDef(TypedDict):
    name: str,
    value: VariableValueUnionTypeDef,  # (1)
```

1. See [:material-code-braces: VariableValueTypeDef](./type_defs.md#variablevaluetypedef) [:material-code-braces: VariableValueOutputTypeDef](./type_defs.md#variablevalueoutputtypedef) 
## BatchPutAssetPropertyValueResponseTypeDef

```python
# BatchPutAssetPropertyValueResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import BatchPutAssetPropertyValueResponseTypeDef


def get_value() -> BatchPutAssetPropertyValueResponseTypeDef:
    return {
        "errorEntries": ...,
    }


# BatchPutAssetPropertyValueResponseTypeDef definition

class BatchPutAssetPropertyValueResponseTypeDef(TypedDict):
    errorEntries: List[BatchPutAssetPropertyErrorEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchPutAssetPropertyErrorEntryTypeDef](./type_defs.md#batchputassetpropertyerrorentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePortalRequestTypeDef

```python
# UpdatePortalRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import UpdatePortalRequestTypeDef


def get_value() -> UpdatePortalRequestTypeDef:
    return {
        "portalId": ...,
    }


# UpdatePortalRequestTypeDef definition

class UpdatePortalRequestTypeDef(TypedDict):
    portalId: str,
    portalName: str,
    portalContactEmail: str,
    roleArn: str,
    portalDescription: NotRequired[str],
    portalLogoImage: NotRequired[ImageTypeDef],  # (1)
    clientToken: NotRequired[str],
    notificationSenderEmail: NotRequired[str],
    alarms: NotRequired[AlarmsTypeDef],  # (2)
    portalType: NotRequired[PortalTypeType],  # (3)
    portalTypeConfiguration: NotRequired[Mapping[str, PortalTypeEntryUnionTypeDef]],  # (4)
```

1. See [:material-code-braces: ImageTypeDef](./type_defs.md#imagetypedef) 
2. See [:material-code-braces: AlarmsTypeDef](./type_defs.md#alarmstypedef) 
3. See [:material-code-brackets: PortalTypeType](./literals.md#portaltypetype) 
4. See [:material-code-braces: PortalTypeEntryTypeDef](./type_defs.md#portaltypeentrytypedef) [:material-code-braces: PortalTypeEntryOutputTypeDef](./type_defs.md#portaltypeentryoutputtypedef) 
## DescribeBulkImportJobResponseTypeDef

```python
# DescribeBulkImportJobResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeBulkImportJobResponseTypeDef


def get_value() -> DescribeBulkImportJobResponseTypeDef:
    return {
        "jobId": ...,
    }


# DescribeBulkImportJobResponseTypeDef definition

class DescribeBulkImportJobResponseTypeDef(TypedDict):
    jobId: str,
    jobName: str,
    jobStatus: JobStatusType,  # (1)
    jobRoleArn: str,
    files: List[FileTypeDef],  # (2)
    errorReportLocation: ErrorReportLocationTypeDef,  # (3)
    jobConfiguration: JobConfigurationOutputTypeDef,  # (4)
    jobCreationDate: datetime,
    jobLastUpdateDate: datetime,
    adaptiveIngestion: bool,
    deleteFilesAfterImport: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: FileTypeDef](./type_defs.md#filetypedef) 
3. See [:material-code-braces: ErrorReportLocationTypeDef](./type_defs.md#errorreportlocationtypedef) 
4. See [:material-code-braces: JobConfigurationOutputTypeDef](./type_defs.md#jobconfigurationoutputtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssetModelSummaryTypeDef

```python
# AssetModelSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AssetModelSummaryTypeDef


def get_value() -> AssetModelSummaryTypeDef:
    return {
        "id": ...,
    }


# AssetModelSummaryTypeDef definition

class AssetModelSummaryTypeDef(TypedDict):
    id: str,
    arn: str,
    name: str,
    description: str,
    creationDate: datetime,
    lastUpdateDate: datetime,
    status: AssetModelStatusTypeDef,  # (2)
    externalId: NotRequired[str],
    assetModelType: NotRequired[AssetModelTypeType],  # (1)
    version: NotRequired[str],
```

1. See [:material-code-brackets: AssetModelTypeType](./literals.md#assetmodeltypetype) 
2. See [:material-code-braces: AssetModelStatusTypeDef](./type_defs.md#assetmodelstatustypedef) 
## CreateAssetModelCompositeModelResponseTypeDef

```python
# CreateAssetModelCompositeModelResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import CreateAssetModelCompositeModelResponseTypeDef


def get_value() -> CreateAssetModelCompositeModelResponseTypeDef:
    return {
        "assetModelCompositeModelId": ...,
    }


# CreateAssetModelCompositeModelResponseTypeDef definition

class CreateAssetModelCompositeModelResponseTypeDef(TypedDict):
    assetModelCompositeModelId: str,
    assetModelCompositeModelPath: List[AssetModelCompositeModelPathSegmentTypeDef],  # (1)
    assetModelStatus: AssetModelStatusTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AssetModelCompositeModelPathSegmentTypeDef](./type_defs.md#assetmodelcompositemodelpathsegmenttypedef) 
2. See [:material-code-braces: AssetModelStatusTypeDef](./type_defs.md#assetmodelstatustypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAssetModelResponseTypeDef

```python
# CreateAssetModelResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import CreateAssetModelResponseTypeDef


def get_value() -> CreateAssetModelResponseTypeDef:
    return {
        "assetModelId": ...,
    }


# CreateAssetModelResponseTypeDef definition

class CreateAssetModelResponseTypeDef(TypedDict):
    assetModelId: str,
    assetModelArn: str,
    assetModelStatus: AssetModelStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssetModelStatusTypeDef](./type_defs.md#assetmodelstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAssetModelCompositeModelResponseTypeDef

```python
# DeleteAssetModelCompositeModelResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DeleteAssetModelCompositeModelResponseTypeDef


def get_value() -> DeleteAssetModelCompositeModelResponseTypeDef:
    return {
        "assetModelStatus": ...,
    }


# DeleteAssetModelCompositeModelResponseTypeDef definition

class DeleteAssetModelCompositeModelResponseTypeDef(TypedDict):
    assetModelStatus: AssetModelStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssetModelStatusTypeDef](./type_defs.md#assetmodelstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAssetModelResponseTypeDef

```python
# DeleteAssetModelResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DeleteAssetModelResponseTypeDef


def get_value() -> DeleteAssetModelResponseTypeDef:
    return {
        "assetModelStatus": ...,
    }


# DeleteAssetModelResponseTypeDef definition

class DeleteAssetModelResponseTypeDef(TypedDict):
    assetModelStatus: AssetModelStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssetModelStatusTypeDef](./type_defs.md#assetmodelstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAssetModelCompositeModelResponseTypeDef

```python
# UpdateAssetModelCompositeModelResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import UpdateAssetModelCompositeModelResponseTypeDef


def get_value() -> UpdateAssetModelCompositeModelResponseTypeDef:
    return {
        "assetModelCompositeModelPath": ...,
    }


# UpdateAssetModelCompositeModelResponseTypeDef definition

class UpdateAssetModelCompositeModelResponseTypeDef(TypedDict):
    assetModelCompositeModelPath: List[AssetModelCompositeModelPathSegmentTypeDef],  # (1)
    assetModelStatus: AssetModelStatusTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AssetModelCompositeModelPathSegmentTypeDef](./type_defs.md#assetmodelcompositemodelpathsegmenttypedef) 
2. See [:material-code-braces: AssetModelStatusTypeDef](./type_defs.md#assetmodelstatustypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAssetModelResponseTypeDef

```python
# UpdateAssetModelResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import UpdateAssetModelResponseTypeDef


def get_value() -> UpdateAssetModelResponseTypeDef:
    return {
        "assetModelStatus": ...,
    }


# UpdateAssetModelResponseTypeDef definition

class UpdateAssetModelResponseTypeDef(TypedDict):
    assetModelStatus: AssetModelStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssetModelStatusTypeDef](./type_defs.md#assetmodelstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssetSummaryTypeDef

```python
# AssetSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AssetSummaryTypeDef


def get_value() -> AssetSummaryTypeDef:
    return {
        "id": ...,
    }


# AssetSummaryTypeDef definition

class AssetSummaryTypeDef(TypedDict):
    id: str,
    arn: str,
    name: str,
    assetModelId: str,
    creationDate: datetime,
    lastUpdateDate: datetime,
    status: AssetStatusTypeDef,  # (1)
    hierarchies: List[AssetHierarchyTypeDef],  # (2)
    description: NotRequired[str],
    externalId: NotRequired[str],
```

1. See [:material-code-braces: AssetStatusTypeDef](./type_defs.md#assetstatustypedef) 
2. See [:material-code-braces: AssetHierarchyTypeDef](./type_defs.md#assethierarchytypedef) 
## AssociatedAssetsSummaryTypeDef

```python
# AssociatedAssetsSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AssociatedAssetsSummaryTypeDef


def get_value() -> AssociatedAssetsSummaryTypeDef:
    return {
        "id": ...,
    }


# AssociatedAssetsSummaryTypeDef definition

class AssociatedAssetsSummaryTypeDef(TypedDict):
    id: str,
    arn: str,
    name: str,
    assetModelId: str,
    creationDate: datetime,
    lastUpdateDate: datetime,
    status: AssetStatusTypeDef,  # (1)
    hierarchies: List[AssetHierarchyTypeDef],  # (2)
    description: NotRequired[str],
    externalId: NotRequired[str],
```

1. See [:material-code-braces: AssetStatusTypeDef](./type_defs.md#assetstatustypedef) 
2. See [:material-code-braces: AssetHierarchyTypeDef](./type_defs.md#assethierarchytypedef) 
## CreateAssetResponseTypeDef

```python
# CreateAssetResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import CreateAssetResponseTypeDef


def get_value() -> CreateAssetResponseTypeDef:
    return {
        "assetId": ...,
    }


# CreateAssetResponseTypeDef definition

class CreateAssetResponseTypeDef(TypedDict):
    assetId: str,
    assetArn: str,
    assetStatus: AssetStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssetStatusTypeDef](./type_defs.md#assetstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAssetResponseTypeDef

```python
# DeleteAssetResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DeleteAssetResponseTypeDef


def get_value() -> DeleteAssetResponseTypeDef:
    return {
        "assetStatus": ...,
    }


# DeleteAssetResponseTypeDef definition

class DeleteAssetResponseTypeDef(TypedDict):
    assetStatus: AssetStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssetStatusTypeDef](./type_defs.md#assetstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAssetResponseTypeDef

```python
# DescribeAssetResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeAssetResponseTypeDef


def get_value() -> DescribeAssetResponseTypeDef:
    return {
        "assetId": ...,
    }


# DescribeAssetResponseTypeDef definition

class DescribeAssetResponseTypeDef(TypedDict):
    assetId: str,
    assetArn: str,
    assetName: str,
    assetModelId: str,
    assetProperties: List[AssetPropertyTypeDef],  # (1)
    assetHierarchies: List[AssetHierarchyTypeDef],  # (2)
    assetCompositeModels: List[AssetCompositeModelTypeDef],  # (3)
    assetCreationDate: datetime,
    assetLastUpdateDate: datetime,
    assetStatus: AssetStatusTypeDef,  # (4)
    assetDescription: str,
    assetCompositeModelSummaries: List[AssetCompositeModelSummaryTypeDef],  # (5)
    assetExternalId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: AssetPropertyTypeDef](./type_defs.md#assetpropertytypedef) 
2. See [:material-code-braces: AssetHierarchyTypeDef](./type_defs.md#assethierarchytypedef) 
3. See [:material-code-braces: AssetCompositeModelTypeDef](./type_defs.md#assetcompositemodeltypedef) 
4. See [:material-code-braces: AssetStatusTypeDef](./type_defs.md#assetstatustypedef) 
5. See [:material-code-braces: AssetCompositeModelSummaryTypeDef](./type_defs.md#assetcompositemodelsummarytypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAssetResponseTypeDef

```python
# UpdateAssetResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import UpdateAssetResponseTypeDef


def get_value() -> UpdateAssetResponseTypeDef:
    return {
        "assetStatus": ...,
    }


# UpdateAssetResponseTypeDef definition

class UpdateAssetResponseTypeDef(TypedDict):
    assetStatus: AssetStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssetStatusTypeDef](./type_defs.md#assetstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDatasetResponseTypeDef

```python
# CreateDatasetResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import CreateDatasetResponseTypeDef


def get_value() -> CreateDatasetResponseTypeDef:
    return {
        "datasetId": ...,
    }


# CreateDatasetResponseTypeDef definition

class CreateDatasetResponseTypeDef(TypedDict):
    datasetId: str,
    datasetArn: str,
    datasetStatus: DatasetStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DatasetStatusTypeDef](./type_defs.md#datasetstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DatasetSummaryTypeDef

```python
# DatasetSummaryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DatasetSummaryTypeDef


def get_value() -> DatasetSummaryTypeDef:
    return {
        "id": ...,
    }


# DatasetSummaryTypeDef definition

class DatasetSummaryTypeDef(TypedDict):
    id: str,
    arn: str,
    name: str,
    description: str,
    creationDate: datetime,
    lastUpdateDate: datetime,
    status: DatasetStatusTypeDef,  # (1)
```

1. See [:material-code-braces: DatasetStatusTypeDef](./type_defs.md#datasetstatustypedef) 
## DeleteDatasetResponseTypeDef

```python
# DeleteDatasetResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DeleteDatasetResponseTypeDef


def get_value() -> DeleteDatasetResponseTypeDef:
    return {
        "datasetStatus": ...,
    }


# DeleteDatasetResponseTypeDef definition

class DeleteDatasetResponseTypeDef(TypedDict):
    datasetStatus: DatasetStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DatasetStatusTypeDef](./type_defs.md#datasetstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDatasetResponseTypeDef

```python
# UpdateDatasetResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import UpdateDatasetResponseTypeDef


def get_value() -> UpdateDatasetResponseTypeDef:
    return {
        "datasetId": ...,
    }


# UpdateDatasetResponseTypeDef definition

class UpdateDatasetResponseTypeDef(TypedDict):
    datasetId: str,
    datasetArn: str,
    datasetStatus: DatasetStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DatasetStatusTypeDef](./type_defs.md#datasetstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGatewaysResponseTypeDef

```python
# ListGatewaysResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListGatewaysResponseTypeDef


def get_value() -> ListGatewaysResponseTypeDef:
    return {
        "gatewaySummaries": ...,
    }


# ListGatewaysResponseTypeDef definition

class ListGatewaysResponseTypeDef(TypedDict):
    gatewaySummaries: List[GatewaySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: GatewaySummaryTypeDef](./type_defs.md#gatewaysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDatasetRequestTypeDef

```python
# CreateDatasetRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import CreateDatasetRequestTypeDef


def get_value() -> CreateDatasetRequestTypeDef:
    return {
        "datasetName": ...,
    }


# CreateDatasetRequestTypeDef definition

class CreateDatasetRequestTypeDef(TypedDict):
    datasetName: str,
    datasetSource: DatasetSourceTypeDef,  # (1)
    datasetId: NotRequired[str],
    datasetDescription: NotRequired[str],
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: DatasetSourceTypeDef](./type_defs.md#datasetsourcetypedef) 
## DescribeDatasetResponseTypeDef

```python
# DescribeDatasetResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeDatasetResponseTypeDef


def get_value() -> DescribeDatasetResponseTypeDef:
    return {
        "datasetId": ...,
    }


# DescribeDatasetResponseTypeDef definition

class DescribeDatasetResponseTypeDef(TypedDict):
    datasetId: str,
    datasetArn: str,
    datasetName: str,
    datasetDescription: str,
    datasetSource: DatasetSourceTypeDef,  # (1)
    datasetStatus: DatasetStatusTypeDef,  # (2)
    datasetCreationDate: datetime,
    datasetLastUpdateDate: datetime,
    datasetVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: DatasetSourceTypeDef](./type_defs.md#datasetsourcetypedef) 
2. See [:material-code-braces: DatasetStatusTypeDef](./type_defs.md#datasetstatustypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDatasetRequestTypeDef

```python
# UpdateDatasetRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import UpdateDatasetRequestTypeDef


def get_value() -> UpdateDatasetRequestTypeDef:
    return {
        "datasetId": ...,
    }


# UpdateDatasetRequestTypeDef definition

class UpdateDatasetRequestTypeDef(TypedDict):
    datasetId: str,
    datasetName: str,
    datasetSource: DatasetSourceTypeDef,  # (1)
    datasetDescription: NotRequired[str],
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: DatasetSourceTypeDef](./type_defs.md#datasetsourcetypedef) 
## ReferenceTypeDef

```python
# ReferenceTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ReferenceTypeDef


def get_value() -> ReferenceTypeDef:
    return {
        "dataset": ...,
    }


# ReferenceTypeDef definition

class ReferenceTypeDef(TypedDict):
    dataset: NotRequired[DataSetReferenceTypeDef],  # (1)
```

1. See [:material-code-braces: DataSetReferenceTypeDef](./type_defs.md#datasetreferencetypedef) 
## ListPortalsResponseTypeDef

```python
# ListPortalsResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListPortalsResponseTypeDef


def get_value() -> ListPortalsResponseTypeDef:
    return {
        "portalSummaries": ...,
    }


# ListPortalsResponseTypeDef definition

class ListPortalsResponseTypeDef(TypedDict):
    portalSummaries: List[PortalSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PortalSummaryTypeDef](./type_defs.md#portalsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccessPoliciesResponseTypeDef

```python
# ListAccessPoliciesResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListAccessPoliciesResponseTypeDef


def get_value() -> ListAccessPoliciesResponseTypeDef:
    return {
        "accessPolicySummaries": ...,
    }


# ListAccessPoliciesResponseTypeDef definition

class ListAccessPoliciesResponseTypeDef(TypedDict):
    accessPolicySummaries: List[AccessPolicySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AccessPolicySummaryTypeDef](./type_defs.md#accesspolicysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetAssetPropertyValueHistorySuccessEntryTypeDef

```python
# BatchGetAssetPropertyValueHistorySuccessEntryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import BatchGetAssetPropertyValueHistorySuccessEntryTypeDef


def get_value() -> BatchGetAssetPropertyValueHistorySuccessEntryTypeDef:
    return {
        "entryId": ...,
    }


# BatchGetAssetPropertyValueHistorySuccessEntryTypeDef definition

class BatchGetAssetPropertyValueHistorySuccessEntryTypeDef(TypedDict):
    entryId: str,
    assetPropertyValueHistory: List[AssetPropertyValueTypeDef],  # (1)
```

1. See [:material-code-braces: AssetPropertyValueTypeDef](./type_defs.md#assetpropertyvaluetypedef) 
## BatchGetAssetPropertyValueSuccessEntryTypeDef

```python
# BatchGetAssetPropertyValueSuccessEntryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import BatchGetAssetPropertyValueSuccessEntryTypeDef


def get_value() -> BatchGetAssetPropertyValueSuccessEntryTypeDef:
    return {
        "entryId": ...,
    }


# BatchGetAssetPropertyValueSuccessEntryTypeDef definition

class BatchGetAssetPropertyValueSuccessEntryTypeDef(TypedDict):
    entryId: str,
    assetPropertyValue: NotRequired[AssetPropertyValueTypeDef],  # (1)
```

1. See [:material-code-braces: AssetPropertyValueTypeDef](./type_defs.md#assetpropertyvaluetypedef) 
## GetAssetPropertyValueHistoryResponseTypeDef

```python
# GetAssetPropertyValueHistoryResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import GetAssetPropertyValueHistoryResponseTypeDef


def get_value() -> GetAssetPropertyValueHistoryResponseTypeDef:
    return {
        "assetPropertyValueHistory": ...,
    }


# GetAssetPropertyValueHistoryResponseTypeDef definition

class GetAssetPropertyValueHistoryResponseTypeDef(TypedDict):
    assetPropertyValueHistory: List[AssetPropertyValueTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AssetPropertyValueTypeDef](./type_defs.md#assetpropertyvaluetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAssetPropertyValueResponseTypeDef

```python
# GetAssetPropertyValueResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import GetAssetPropertyValueResponseTypeDef


def get_value() -> GetAssetPropertyValueResponseTypeDef:
    return {
        "propertyValue": ...,
    }


# GetAssetPropertyValueResponseTypeDef definition

class GetAssetPropertyValueResponseTypeDef(TypedDict):
    propertyValue: AssetPropertyValueTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssetPropertyValueTypeDef](./type_defs.md#assetpropertyvaluetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutAssetPropertyValueEntryTypeDef

```python
# PutAssetPropertyValueEntryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import PutAssetPropertyValueEntryTypeDef


def get_value() -> PutAssetPropertyValueEntryTypeDef:
    return {
        "entryId": ...,
    }


# PutAssetPropertyValueEntryTypeDef definition

class PutAssetPropertyValueEntryTypeDef(TypedDict):
    entryId: str,
    propertyValues: Sequence[AssetPropertyValueTypeDef],  # (1)
    assetId: NotRequired[str],
    propertyId: NotRequired[str],
    propertyAlias: NotRequired[str],
```

1. See [:material-code-braces: AssetPropertyValueTypeDef](./type_defs.md#assetpropertyvaluetypedef) 
## GetInterpolatedAssetPropertyValuesResponseTypeDef

```python
# GetInterpolatedAssetPropertyValuesResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import GetInterpolatedAssetPropertyValuesResponseTypeDef


def get_value() -> GetInterpolatedAssetPropertyValuesResponseTypeDef:
    return {
        "interpolatedAssetPropertyValues": ...,
    }


# GetInterpolatedAssetPropertyValuesResponseTypeDef definition

class GetInterpolatedAssetPropertyValuesResponseTypeDef(TypedDict):
    interpolatedAssetPropertyValues: List[InterpolatedAssetPropertyValueTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: InterpolatedAssetPropertyValueTypeDef](./type_defs.md#interpolatedassetpropertyvaluetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PropertyTypeOutputTypeDef

```python
# PropertyTypeOutputTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import PropertyTypeOutputTypeDef


def get_value() -> PropertyTypeOutputTypeDef:
    return {
        "attribute": ...,
    }


# PropertyTypeOutputTypeDef definition

class PropertyTypeOutputTypeDef(TypedDict):
    attribute: NotRequired[AttributeTypeDef],  # (1)
    measurement: NotRequired[MeasurementTypeDef],  # (2)
    transform: NotRequired[TransformOutputTypeDef],  # (3)
    metric: NotRequired[MetricOutputTypeDef],  # (4)
```

1. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
2. See [:material-code-braces: MeasurementTypeDef](./type_defs.md#measurementtypedef) 
3. See [:material-code-braces: TransformOutputTypeDef](./type_defs.md#transformoutputtypedef) 
4. See [:material-code-braces: MetricOutputTypeDef](./type_defs.md#metricoutputtypedef) 
## CreateBulkImportJobRequestTypeDef

```python
# CreateBulkImportJobRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import CreateBulkImportJobRequestTypeDef


def get_value() -> CreateBulkImportJobRequestTypeDef:
    return {
        "jobName": ...,
    }


# CreateBulkImportJobRequestTypeDef definition

class CreateBulkImportJobRequestTypeDef(TypedDict):
    jobName: str,
    jobRoleArn: str,
    files: Sequence[FileTypeDef],  # (1)
    errorReportLocation: ErrorReportLocationTypeDef,  # (2)
    jobConfiguration: JobConfigurationUnionTypeDef,  # (3)
    adaptiveIngestion: NotRequired[bool],
    deleteFilesAfterImport: NotRequired[bool],
```

1. See [:material-code-braces: FileTypeDef](./type_defs.md#filetypedef) 
2. See [:material-code-braces: ErrorReportLocationTypeDef](./type_defs.md#errorreportlocationtypedef) 
3. See [:material-code-braces: JobConfigurationTypeDef](./type_defs.md#jobconfigurationtypedef) [:material-code-braces: JobConfigurationOutputTypeDef](./type_defs.md#jobconfigurationoutputtypedef) 
## ListAssetModelsResponseTypeDef

```python
# ListAssetModelsResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListAssetModelsResponseTypeDef


def get_value() -> ListAssetModelsResponseTypeDef:
    return {
        "assetModelSummaries": ...,
    }


# ListAssetModelsResponseTypeDef definition

class ListAssetModelsResponseTypeDef(TypedDict):
    assetModelSummaries: List[AssetModelSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AssetModelSummaryTypeDef](./type_defs.md#assetmodelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssetsResponseTypeDef

```python
# ListAssetsResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListAssetsResponseTypeDef


def get_value() -> ListAssetsResponseTypeDef:
    return {
        "assetSummaries": ...,
    }


# ListAssetsResponseTypeDef definition

class ListAssetsResponseTypeDef(TypedDict):
    assetSummaries: List[AssetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AssetSummaryTypeDef](./type_defs.md#assetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssociatedAssetsResponseTypeDef

```python
# ListAssociatedAssetsResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListAssociatedAssetsResponseTypeDef


def get_value() -> ListAssociatedAssetsResponseTypeDef:
    return {
        "assetSummaries": ...,
    }


# ListAssociatedAssetsResponseTypeDef definition

class ListAssociatedAssetsResponseTypeDef(TypedDict):
    assetSummaries: List[AssociatedAssetsSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AssociatedAssetsSummaryTypeDef](./type_defs.md#associatedassetssummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDatasetsResponseTypeDef

```python
# ListDatasetsResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListDatasetsResponseTypeDef


def get_value() -> ListDatasetsResponseTypeDef:
    return {
        "datasetSummaries": ...,
    }


# ListDatasetsResponseTypeDef definition

class ListDatasetsResponseTypeDef(TypedDict):
    datasetSummaries: List[DatasetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DatasetSummaryTypeDef](./type_defs.md#datasetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CitationTypeDef

```python
# CitationTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import CitationTypeDef


def get_value() -> CitationTypeDef:
    return {
        "reference": ...,
    }


# CitationTypeDef definition

class CitationTypeDef(TypedDict):
    reference: NotRequired[ReferenceTypeDef],  # (1)
    content: NotRequired[ContentTypeDef],  # (2)
```

1. See [:material-code-braces: ReferenceTypeDef](./type_defs.md#referencetypedef) 
2. See [:material-code-braces: ContentTypeDef](./type_defs.md#contenttypedef) 
## BatchGetAssetPropertyValueHistoryResponseTypeDef

```python
# BatchGetAssetPropertyValueHistoryResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import BatchGetAssetPropertyValueHistoryResponseTypeDef


def get_value() -> BatchGetAssetPropertyValueHistoryResponseTypeDef:
    return {
        "errorEntries": ...,
    }


# BatchGetAssetPropertyValueHistoryResponseTypeDef definition

class BatchGetAssetPropertyValueHistoryResponseTypeDef(TypedDict):
    errorEntries: List[BatchGetAssetPropertyValueHistoryErrorEntryTypeDef],  # (1)
    successEntries: List[BatchGetAssetPropertyValueHistorySuccessEntryTypeDef],  # (2)
    skippedEntries: List[BatchGetAssetPropertyValueHistorySkippedEntryTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BatchGetAssetPropertyValueHistoryErrorEntryTypeDef](./type_defs.md#batchgetassetpropertyvaluehistoryerrorentrytypedef) 
2. See [:material-code-braces: BatchGetAssetPropertyValueHistorySuccessEntryTypeDef](./type_defs.md#batchgetassetpropertyvaluehistorysuccessentrytypedef) 
3. See [:material-code-braces: BatchGetAssetPropertyValueHistorySkippedEntryTypeDef](./type_defs.md#batchgetassetpropertyvaluehistoryskippedentrytypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetAssetPropertyValueResponseTypeDef

```python
# BatchGetAssetPropertyValueResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import BatchGetAssetPropertyValueResponseTypeDef


def get_value() -> BatchGetAssetPropertyValueResponseTypeDef:
    return {
        "errorEntries": ...,
    }


# BatchGetAssetPropertyValueResponseTypeDef definition

class BatchGetAssetPropertyValueResponseTypeDef(TypedDict):
    errorEntries: List[BatchGetAssetPropertyValueErrorEntryTypeDef],  # (1)
    successEntries: List[BatchGetAssetPropertyValueSuccessEntryTypeDef],  # (2)
    skippedEntries: List[BatchGetAssetPropertyValueSkippedEntryTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BatchGetAssetPropertyValueErrorEntryTypeDef](./type_defs.md#batchgetassetpropertyvalueerrorentrytypedef) 
2. See [:material-code-braces: BatchGetAssetPropertyValueSuccessEntryTypeDef](./type_defs.md#batchgetassetpropertyvaluesuccessentrytypedef) 
3. See [:material-code-braces: BatchGetAssetPropertyValueSkippedEntryTypeDef](./type_defs.md#batchgetassetpropertyvalueskippedentrytypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchPutAssetPropertyValueRequestTypeDef

```python
# BatchPutAssetPropertyValueRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import BatchPutAssetPropertyValueRequestTypeDef


def get_value() -> BatchPutAssetPropertyValueRequestTypeDef:
    return {
        "entries": ...,
    }


# BatchPutAssetPropertyValueRequestTypeDef definition

class BatchPutAssetPropertyValueRequestTypeDef(TypedDict):
    entries: Sequence[PutAssetPropertyValueEntryTypeDef],  # (1)
    enablePartialEntryProcessing: NotRequired[bool],
```

1. See [:material-code-braces: PutAssetPropertyValueEntryTypeDef](./type_defs.md#putassetpropertyvalueentrytypedef) 
## AssetModelPropertyOutputTypeDef

```python
# AssetModelPropertyOutputTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AssetModelPropertyOutputTypeDef


def get_value() -> AssetModelPropertyOutputTypeDef:
    return {
        "id": ...,
    }


# AssetModelPropertyOutputTypeDef definition

class AssetModelPropertyOutputTypeDef(TypedDict):
    name: str,
    dataType: PropertyDataTypeType,  # (1)
    type: PropertyTypeOutputTypeDef,  # (2)
    id: NotRequired[str],
    externalId: NotRequired[str],
    dataTypeSpec: NotRequired[str],
    unit: NotRequired[str],
    path: NotRequired[List[AssetModelPropertyPathSegmentTypeDef]],  # (3)
```

1. See [:material-code-brackets: PropertyDataTypeType](./literals.md#propertydatatypetype) 
2. See [:material-code-braces: PropertyTypeOutputTypeDef](./type_defs.md#propertytypeoutputtypedef) 
3. See [:material-code-braces: AssetModelPropertyPathSegmentTypeDef](./type_defs.md#assetmodelpropertypathsegmenttypedef) 
## AssetModelPropertySummaryTypeDef

```python
# AssetModelPropertySummaryTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AssetModelPropertySummaryTypeDef


def get_value() -> AssetModelPropertySummaryTypeDef:
    return {
        "id": ...,
    }


# AssetModelPropertySummaryTypeDef definition

class AssetModelPropertySummaryTypeDef(TypedDict):
    name: str,
    dataType: PropertyDataTypeType,  # (1)
    type: PropertyTypeOutputTypeDef,  # (2)
    id: NotRequired[str],
    externalId: NotRequired[str],
    dataTypeSpec: NotRequired[str],
    unit: NotRequired[str],
    assetModelCompositeModelId: NotRequired[str],
    path: NotRequired[List[AssetModelPropertyPathSegmentTypeDef]],  # (3)
```

1. See [:material-code-brackets: PropertyDataTypeType](./literals.md#propertydatatypetype) 
2. See [:material-code-braces: PropertyTypeOutputTypeDef](./type_defs.md#propertytypeoutputtypedef) 
3. See [:material-code-braces: AssetModelPropertyPathSegmentTypeDef](./type_defs.md#assetmodelpropertypathsegmenttypedef) 
## PropertyTypeDef

```python
# PropertyTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import PropertyTypeDef


def get_value() -> PropertyTypeDef:
    return {
        "id": ...,
    }


# PropertyTypeDef definition

class PropertyTypeDef(TypedDict):
    id: str,
    name: str,
    dataType: PropertyDataTypeType,  # (2)
    alias: NotRequired[str],
    notification: NotRequired[PropertyNotificationTypeDef],  # (1)
    unit: NotRequired[str],
    type: NotRequired[PropertyTypeOutputTypeDef],  # (3)
    path: NotRequired[List[AssetPropertyPathSegmentTypeDef]],  # (4)
    externalId: NotRequired[str],
```

1. See [:material-code-braces: PropertyNotificationTypeDef](./type_defs.md#propertynotificationtypedef) 
2. See [:material-code-brackets: PropertyDataTypeType](./literals.md#propertydatatypetype) 
3. See [:material-code-braces: PropertyTypeOutputTypeDef](./type_defs.md#propertytypeoutputtypedef) 
4. See [:material-code-braces: AssetPropertyPathSegmentTypeDef](./type_defs.md#assetpropertypathsegmenttypedef) 
## MetricTypeDef

```python
# MetricTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import MetricTypeDef


def get_value() -> MetricTypeDef:
    return {
        "expression": ...,
    }


# MetricTypeDef definition

class MetricTypeDef(TypedDict):
    expression: str,
    variables: Sequence[ExpressionVariableUnionTypeDef],  # (1)
    window: MetricWindowTypeDef,  # (2)
    processingConfig: NotRequired[MetricProcessingConfigTypeDef],  # (3)
```

1. See [:material-code-braces: ExpressionVariableTypeDef](./type_defs.md#expressionvariabletypedef) [:material-code-braces: ExpressionVariableOutputTypeDef](./type_defs.md#expressionvariableoutputtypedef) 
2. See [:material-code-braces: MetricWindowTypeDef](./type_defs.md#metricwindowtypedef) 
3. See [:material-code-braces: MetricProcessingConfigTypeDef](./type_defs.md#metricprocessingconfigtypedef) 
## TransformTypeDef

```python
# TransformTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import TransformTypeDef


def get_value() -> TransformTypeDef:
    return {
        "expression": ...,
    }


# TransformTypeDef definition

class TransformTypeDef(TypedDict):
    expression: str,
    variables: Sequence[ExpressionVariableUnionTypeDef],  # (1)
    processingConfig: NotRequired[TransformProcessingConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ExpressionVariableTypeDef](./type_defs.md#expressionvariabletypedef) [:material-code-braces: ExpressionVariableOutputTypeDef](./type_defs.md#expressionvariableoutputtypedef) 
2. See [:material-code-braces: TransformProcessingConfigTypeDef](./type_defs.md#transformprocessingconfigtypedef) 
## InvocationOutputTypeDef

```python
# InvocationOutputTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import InvocationOutputTypeDef


def get_value() -> InvocationOutputTypeDef:
    return {
        "message": ...,
    }


# InvocationOutputTypeDef definition

class InvocationOutputTypeDef(TypedDict):
    message: NotRequired[str],
    citations: NotRequired[List[CitationTypeDef]],  # (1)
```

1. See [:material-code-braces: CitationTypeDef](./type_defs.md#citationtypedef) 
## AssetModelCompositeModelOutputTypeDef

```python
# AssetModelCompositeModelOutputTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AssetModelCompositeModelOutputTypeDef


def get_value() -> AssetModelCompositeModelOutputTypeDef:
    return {
        "name": ...,
    }


# AssetModelCompositeModelOutputTypeDef definition

class AssetModelCompositeModelOutputTypeDef(TypedDict):
    name: str,
    type: str,
    description: NotRequired[str],
    properties: NotRequired[List[AssetModelPropertyOutputTypeDef]],  # (1)
    id: NotRequired[str],
    externalId: NotRequired[str],
```

1. See [:material-code-braces: AssetModelPropertyOutputTypeDef](./type_defs.md#assetmodelpropertyoutputtypedef) 
## DescribeAssetModelCompositeModelResponseTypeDef

```python
# DescribeAssetModelCompositeModelResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeAssetModelCompositeModelResponseTypeDef


def get_value() -> DescribeAssetModelCompositeModelResponseTypeDef:
    return {
        "assetModelId": ...,
    }


# DescribeAssetModelCompositeModelResponseTypeDef definition

class DescribeAssetModelCompositeModelResponseTypeDef(TypedDict):
    assetModelId: str,
    assetModelCompositeModelId: str,
    assetModelCompositeModelExternalId: str,
    assetModelCompositeModelPath: List[AssetModelCompositeModelPathSegmentTypeDef],  # (1)
    assetModelCompositeModelName: str,
    assetModelCompositeModelDescription: str,
    assetModelCompositeModelType: str,
    assetModelCompositeModelProperties: List[AssetModelPropertyOutputTypeDef],  # (2)
    compositionDetails: CompositionDetailsTypeDef,  # (3)
    assetModelCompositeModelSummaries: List[AssetModelCompositeModelSummaryTypeDef],  # (4)
    actionDefinitions: List[ActionDefinitionTypeDef],  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: AssetModelCompositeModelPathSegmentTypeDef](./type_defs.md#assetmodelcompositemodelpathsegmenttypedef) 
2. See [:material-code-braces: AssetModelPropertyOutputTypeDef](./type_defs.md#assetmodelpropertyoutputtypedef) 
3. See [:material-code-braces: CompositionDetailsTypeDef](./type_defs.md#compositiondetailstypedef) 
4. See [:material-code-braces: AssetModelCompositeModelSummaryTypeDef](./type_defs.md#assetmodelcompositemodelsummarytypedef) 
5. See [:material-code-braces: ActionDefinitionTypeDef](./type_defs.md#actiondefinitiontypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssetModelPropertiesResponseTypeDef

```python
# ListAssetModelPropertiesResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ListAssetModelPropertiesResponseTypeDef


def get_value() -> ListAssetModelPropertiesResponseTypeDef:
    return {
        "assetModelPropertySummaries": ...,
    }


# ListAssetModelPropertiesResponseTypeDef definition

class ListAssetModelPropertiesResponseTypeDef(TypedDict):
    assetModelPropertySummaries: List[AssetModelPropertySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AssetModelPropertySummaryTypeDef](./type_defs.md#assetmodelpropertysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CompositeModelPropertyTypeDef

```python
# CompositeModelPropertyTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import CompositeModelPropertyTypeDef


def get_value() -> CompositeModelPropertyTypeDef:
    return {
        "name": ...,
    }


# CompositeModelPropertyTypeDef definition

class CompositeModelPropertyTypeDef(TypedDict):
    name: str,
    type: str,
    assetProperty: PropertyTypeDef,  # (1)
    id: NotRequired[str],
    externalId: NotRequired[str],
```

1. See [:material-code-braces: PropertyTypeDef](./type_defs.md#propertytypedef) 
## ResponseStreamTypeDef

```python
# ResponseStreamTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import ResponseStreamTypeDef


def get_value() -> ResponseStreamTypeDef:
    return {
        "trace": ...,
    }


# ResponseStreamTypeDef definition

class ResponseStreamTypeDef(TypedDict):
    trace: NotRequired[TraceTypeDef],  # (1)
    output: NotRequired[InvocationOutputTypeDef],  # (2)
    accessDeniedException: NotRequired[AccessDeniedExceptionTypeDef],  # (3)
    conflictingOperationException: NotRequired[ConflictingOperationExceptionTypeDef],  # (4)
    internalFailureException: NotRequired[InternalFailureExceptionTypeDef],  # (5)
    invalidRequestException: NotRequired[InvalidRequestExceptionTypeDef],  # (6)
    limitExceededException: NotRequired[LimitExceededExceptionTypeDef],  # (7)
    resourceNotFoundException: NotRequired[ResourceNotFoundExceptionTypeDef],  # (8)
    throttlingException: NotRequired[ThrottlingExceptionTypeDef],  # (9)
```

1. See [:material-code-braces: TraceTypeDef](./type_defs.md#tracetypedef) 
2. See [:material-code-braces: InvocationOutputTypeDef](./type_defs.md#invocationoutputtypedef) 
3. See [:material-code-braces: AccessDeniedExceptionTypeDef](./type_defs.md#accessdeniedexceptiontypedef) 
4. See [:material-code-braces: ConflictingOperationExceptionTypeDef](./type_defs.md#conflictingoperationexceptiontypedef) 
5. See [:material-code-braces: InternalFailureExceptionTypeDef](./type_defs.md#internalfailureexceptiontypedef) 
6. See [:material-code-braces: InvalidRequestExceptionTypeDef](./type_defs.md#invalidrequestexceptiontypedef) 
7. See [:material-code-braces: LimitExceededExceptionTypeDef](./type_defs.md#limitexceededexceptiontypedef) 
8. See [:material-code-braces: ResourceNotFoundExceptionTypeDef](./type_defs.md#resourcenotfoundexceptiontypedef) 
9. See [:material-code-braces: ThrottlingExceptionTypeDef](./type_defs.md#throttlingexceptiontypedef) 
## DescribeAssetModelResponseTypeDef

```python
# DescribeAssetModelResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeAssetModelResponseTypeDef


def get_value() -> DescribeAssetModelResponseTypeDef:
    return {
        "assetModelId": ...,
    }


# DescribeAssetModelResponseTypeDef definition

class DescribeAssetModelResponseTypeDef(TypedDict):
    assetModelId: str,
    assetModelExternalId: str,
    assetModelArn: str,
    assetModelName: str,
    assetModelType: AssetModelTypeType,  # (1)
    assetModelDescription: str,
    assetModelProperties: List[AssetModelPropertyOutputTypeDef],  # (2)
    assetModelHierarchies: List[AssetModelHierarchyTypeDef],  # (3)
    assetModelCompositeModels: List[AssetModelCompositeModelOutputTypeDef],  # (4)
    assetModelCompositeModelSummaries: List[AssetModelCompositeModelSummaryTypeDef],  # (5)
    assetModelCreationDate: datetime,
    assetModelLastUpdateDate: datetime,
    assetModelStatus: AssetModelStatusTypeDef,  # (6)
    assetModelVersion: str,
    eTag: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-brackets: AssetModelTypeType](./literals.md#assetmodeltypetype) 
2. See [:material-code-braces: AssetModelPropertyOutputTypeDef](./type_defs.md#assetmodelpropertyoutputtypedef) 
3. See [:material-code-braces: AssetModelHierarchyTypeDef](./type_defs.md#assetmodelhierarchytypedef) 
4. See [:material-code-braces: AssetModelCompositeModelOutputTypeDef](./type_defs.md#assetmodelcompositemodeloutputtypedef) 
5. See [:material-code-braces: AssetModelCompositeModelSummaryTypeDef](./type_defs.md#assetmodelcompositemodelsummarytypedef) 
6. See [:material-code-braces: AssetModelStatusTypeDef](./type_defs.md#assetmodelstatustypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAssetPropertyResponseTypeDef

```python
# DescribeAssetPropertyResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import DescribeAssetPropertyResponseTypeDef


def get_value() -> DescribeAssetPropertyResponseTypeDef:
    return {
        "assetId": ...,
    }


# DescribeAssetPropertyResponseTypeDef definition

class DescribeAssetPropertyResponseTypeDef(TypedDict):
    assetId: str,
    assetName: str,
    assetModelId: str,
    assetProperty: PropertyTypeDef,  # (1)
    compositeModel: CompositeModelPropertyTypeDef,  # (2)
    assetExternalId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: PropertyTypeDef](./type_defs.md#propertytypedef) 
2. See [:material-code-braces: CompositeModelPropertyTypeDef](./type_defs.md#compositemodelpropertytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PropertyTypeTypeDef

```python
# PropertyTypeTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import PropertyTypeTypeDef


def get_value() -> PropertyTypeTypeDef:
    return {
        "attribute": ...,
    }


# PropertyTypeTypeDef definition

class PropertyTypeTypeDef(TypedDict):
    attribute: NotRequired[AttributeTypeDef],  # (1)
    measurement: NotRequired[MeasurementTypeDef],  # (2)
    transform: NotRequired[TransformUnionTypeDef],  # (3)
    metric: NotRequired[MetricUnionTypeDef],  # (4)
```

1. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
2. See [:material-code-braces: MeasurementTypeDef](./type_defs.md#measurementtypedef) 
3. See [:material-code-braces: TransformTypeDef](./type_defs.md#transformtypedef) [:material-code-braces: TransformOutputTypeDef](./type_defs.md#transformoutputtypedef) 
4. See [:material-code-braces: MetricTypeDef](./type_defs.md#metrictypedef) [:material-code-braces: MetricOutputTypeDef](./type_defs.md#metricoutputtypedef) 
## InvokeAssistantResponseTypeDef

```python
# InvokeAssistantResponseTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import InvokeAssistantResponseTypeDef


def get_value() -> InvokeAssistantResponseTypeDef:
    return {
        "body": ...,
    }


# InvokeAssistantResponseTypeDef definition

class InvokeAssistantResponseTypeDef(TypedDict):
    body: AioEventStream[ResponseStreamTypeDef],  # (1)
    conversationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResponseStreamTypeDef](./type_defs.md#responsestreamtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssetModelPropertyDefinitionTypeDef

```python
# AssetModelPropertyDefinitionTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AssetModelPropertyDefinitionTypeDef


def get_value() -> AssetModelPropertyDefinitionTypeDef:
    return {
        "id": ...,
    }


# AssetModelPropertyDefinitionTypeDef definition

class AssetModelPropertyDefinitionTypeDef(TypedDict):
    name: str,
    dataType: PropertyDataTypeType,  # (1)
    type: PropertyTypeUnionTypeDef,  # (2)
    id: NotRequired[str],
    externalId: NotRequired[str],
    dataTypeSpec: NotRequired[str],
    unit: NotRequired[str],
```

1. See [:material-code-brackets: PropertyDataTypeType](./literals.md#propertydatatypetype) 
2. See [:material-code-braces: PropertyTypeTypeDef](./type_defs.md#propertytypetypedef) [:material-code-braces: PropertyTypeOutputTypeDef](./type_defs.md#propertytypeoutputtypedef) 
## AssetModelPropertyTypeDef

```python
# AssetModelPropertyTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AssetModelPropertyTypeDef


def get_value() -> AssetModelPropertyTypeDef:
    return {
        "id": ...,
    }


# AssetModelPropertyTypeDef definition

class AssetModelPropertyTypeDef(TypedDict):
    name: str,
    dataType: PropertyDataTypeType,  # (1)
    type: PropertyTypeUnionTypeDef,  # (2)
    id: NotRequired[str],
    externalId: NotRequired[str],
    dataTypeSpec: NotRequired[str],
    unit: NotRequired[str],
    path: NotRequired[Sequence[AssetModelPropertyPathSegmentTypeDef]],  # (3)
```

1. See [:material-code-brackets: PropertyDataTypeType](./literals.md#propertydatatypetype) 
2. See [:material-code-braces: PropertyTypeTypeDef](./type_defs.md#propertytypetypedef) [:material-code-braces: PropertyTypeOutputTypeDef](./type_defs.md#propertytypeoutputtypedef) 
3. See [:material-code-braces: AssetModelPropertyPathSegmentTypeDef](./type_defs.md#assetmodelpropertypathsegmenttypedef) 
## AssetModelCompositeModelDefinitionTypeDef

```python
# AssetModelCompositeModelDefinitionTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AssetModelCompositeModelDefinitionTypeDef


def get_value() -> AssetModelCompositeModelDefinitionTypeDef:
    return {
        "id": ...,
    }


# AssetModelCompositeModelDefinitionTypeDef definition

class AssetModelCompositeModelDefinitionTypeDef(TypedDict):
    name: str,
    type: str,
    id: NotRequired[str],
    externalId: NotRequired[str],
    description: NotRequired[str],
    properties: NotRequired[Sequence[AssetModelPropertyDefinitionTypeDef]],  # (1)
```

1. See [:material-code-braces: AssetModelPropertyDefinitionTypeDef](./type_defs.md#assetmodelpropertydefinitiontypedef) 
## CreateAssetModelCompositeModelRequestTypeDef

```python
# CreateAssetModelCompositeModelRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import CreateAssetModelCompositeModelRequestTypeDef


def get_value() -> CreateAssetModelCompositeModelRequestTypeDef:
    return {
        "assetModelId": ...,
    }


# CreateAssetModelCompositeModelRequestTypeDef definition

class CreateAssetModelCompositeModelRequestTypeDef(TypedDict):
    assetModelId: str,
    assetModelCompositeModelName: str,
    assetModelCompositeModelType: str,
    assetModelCompositeModelExternalId: NotRequired[str],
    parentAssetModelCompositeModelId: NotRequired[str],
    assetModelCompositeModelId: NotRequired[str],
    assetModelCompositeModelDescription: NotRequired[str],
    clientToken: NotRequired[str],
    composedAssetModelId: NotRequired[str],
    assetModelCompositeModelProperties: NotRequired[Sequence[AssetModelPropertyDefinitionTypeDef]],  # (1)
    ifMatch: NotRequired[str],
    ifNoneMatch: NotRequired[str],
    matchForVersionType: NotRequired[AssetModelVersionTypeType],  # (2)
```

1. See [:material-code-braces: AssetModelPropertyDefinitionTypeDef](./type_defs.md#assetmodelpropertydefinitiontypedef) 
2. See [:material-code-brackets: AssetModelVersionTypeType](./literals.md#assetmodelversiontypetype) 
## CreateAssetModelRequestTypeDef

```python
# CreateAssetModelRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import CreateAssetModelRequestTypeDef


def get_value() -> CreateAssetModelRequestTypeDef:
    return {
        "assetModelName": ...,
    }


# CreateAssetModelRequestTypeDef definition

class CreateAssetModelRequestTypeDef(TypedDict):
    assetModelName: str,
    assetModelType: NotRequired[AssetModelTypeType],  # (1)
    assetModelId: NotRequired[str],
    assetModelExternalId: NotRequired[str],
    assetModelDescription: NotRequired[str],
    assetModelProperties: NotRequired[Sequence[AssetModelPropertyDefinitionTypeDef]],  # (2)
    assetModelHierarchies: NotRequired[Sequence[AssetModelHierarchyDefinitionTypeDef]],  # (3)
    assetModelCompositeModels: NotRequired[Sequence[AssetModelCompositeModelDefinitionTypeDef]],  # (4)
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: AssetModelTypeType](./literals.md#assetmodeltypetype) 
2. See [:material-code-braces: AssetModelPropertyDefinitionTypeDef](./type_defs.md#assetmodelpropertydefinitiontypedef) 
3. See [:material-code-braces: AssetModelHierarchyDefinitionTypeDef](./type_defs.md#assetmodelhierarchydefinitiontypedef) 
4. See [:material-code-braces: AssetModelCompositeModelDefinitionTypeDef](./type_defs.md#assetmodelcompositemodeldefinitiontypedef) 
## AssetModelCompositeModelTypeDef

```python
# AssetModelCompositeModelTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import AssetModelCompositeModelTypeDef


def get_value() -> AssetModelCompositeModelTypeDef:
    return {
        "name": ...,
    }


# AssetModelCompositeModelTypeDef definition

class AssetModelCompositeModelTypeDef(TypedDict):
    name: str,
    type: str,
    description: NotRequired[str],
    properties: NotRequired[Sequence[AssetModelPropertyUnionTypeDef]],  # (1)
    id: NotRequired[str],
    externalId: NotRequired[str],
```

1. See [:material-code-braces: AssetModelPropertyTypeDef](./type_defs.md#assetmodelpropertytypedef) [:material-code-braces: AssetModelPropertyOutputTypeDef](./type_defs.md#assetmodelpropertyoutputtypedef) 
## UpdateAssetModelCompositeModelRequestTypeDef

```python
# UpdateAssetModelCompositeModelRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import UpdateAssetModelCompositeModelRequestTypeDef


def get_value() -> UpdateAssetModelCompositeModelRequestTypeDef:
    return {
        "assetModelId": ...,
    }


# UpdateAssetModelCompositeModelRequestTypeDef definition

class UpdateAssetModelCompositeModelRequestTypeDef(TypedDict):
    assetModelId: str,
    assetModelCompositeModelId: str,
    assetModelCompositeModelName: str,
    assetModelCompositeModelExternalId: NotRequired[str],
    assetModelCompositeModelDescription: NotRequired[str],
    clientToken: NotRequired[str],
    assetModelCompositeModelProperties: NotRequired[Sequence[AssetModelPropertyUnionTypeDef]],  # (1)
    ifMatch: NotRequired[str],
    ifNoneMatch: NotRequired[str],
    matchForVersionType: NotRequired[AssetModelVersionTypeType],  # (2)
```

1. See [:material-code-braces: AssetModelPropertyTypeDef](./type_defs.md#assetmodelpropertytypedef) [:material-code-braces: AssetModelPropertyOutputTypeDef](./type_defs.md#assetmodelpropertyoutputtypedef) 
2. See [:material-code-brackets: AssetModelVersionTypeType](./literals.md#assetmodelversiontypetype) 
## UpdateAssetModelRequestTypeDef

```python
# UpdateAssetModelRequestTypeDef TypedDict usage example

from types_aiobotocore_iotsitewise.type_defs import UpdateAssetModelRequestTypeDef


def get_value() -> UpdateAssetModelRequestTypeDef:
    return {
        "assetModelId": ...,
    }


# UpdateAssetModelRequestTypeDef definition

class UpdateAssetModelRequestTypeDef(TypedDict):
    assetModelId: str,
    assetModelName: str,
    assetModelExternalId: NotRequired[str],
    assetModelDescription: NotRequired[str],
    assetModelProperties: NotRequired[Sequence[AssetModelPropertyUnionTypeDef]],  # (1)
    assetModelHierarchies: NotRequired[Sequence[AssetModelHierarchyTypeDef]],  # (2)
    assetModelCompositeModels: NotRequired[Sequence[AssetModelCompositeModelUnionTypeDef]],  # (3)
    clientToken: NotRequired[str],
    ifMatch: NotRequired[str],
    ifNoneMatch: NotRequired[str],
    matchForVersionType: NotRequired[AssetModelVersionTypeType],  # (4)
```

1. See [:material-code-braces: AssetModelPropertyTypeDef](./type_defs.md#assetmodelpropertytypedef) [:material-code-braces: AssetModelPropertyOutputTypeDef](./type_defs.md#assetmodelpropertyoutputtypedef) 
2. See [:material-code-braces: AssetModelHierarchyTypeDef](./type_defs.md#assetmodelhierarchytypedef) 
3. See [:material-code-braces: AssetModelCompositeModelTypeDef](./type_defs.md#assetmodelcompositemodeltypedef) [:material-code-braces: AssetModelCompositeModelOutputTypeDef](./type_defs.md#assetmodelcompositemodeloutputtypedef) 
4. See [:material-code-brackets: AssetModelVersionTypeType](./literals.md#assetmodelversiontypetype) 
