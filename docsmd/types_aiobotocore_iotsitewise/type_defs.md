# Type definitions

> [Index](../README.md) > [IoTSiteWise](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [IoTSiteWise](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#IoTSiteWise)
    type annotations stubs module [types-aiobotocore-iotsitewise](https://pypi.org/project/types-aiobotocore-iotsitewise/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```


## CsvUnionTypeDef

```python
# CsvUnionTypeDef definition

CsvUnionTypeDef = Union[
    CsvTypeDef,  # (1)
    CsvOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CsvTypeDef](./type_defs.md#csvtypedef) 
2. See [:material-code-braces: CsvOutputTypeDef](./type_defs.md#csvoutputtypedef) 

## VariableValueUnionTypeDef

```python
# VariableValueUnionTypeDef definition

VariableValueUnionTypeDef = Union[
    VariableValueTypeDef,  # (1)
    VariableValueOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: VariableValueTypeDef](./type_defs.md#variablevaluetypedef) 
2. See [:material-code-braces: VariableValueOutputTypeDef](./type_defs.md#variablevalueoutputtypedef) 

## FileFormatUnionTypeDef

```python
# FileFormatUnionTypeDef definition

FileFormatUnionTypeDef = Union[
    FileFormatTypeDef,  # (1)
    FileFormatOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FileFormatTypeDef](./type_defs.md#fileformattypedef) 
2. See [:material-code-braces: FileFormatOutputTypeDef](./type_defs.md#fileformatoutputtypedef) 

## ExpressionVariableUnionTypeDef

```python
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
# AssetModelCompositeModelUnionTypeDef definition

AssetModelCompositeModelUnionTypeDef = Union[
    AssetModelCompositeModelTypeDef,  # (1)
    AssetModelCompositeModelOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AssetModelCompositeModelTypeDef](./type_defs.md#assetmodelcompositemodeltypedef) 
2. See [:material-code-braces: AssetModelCompositeModelOutputTypeDef](./type_defs.md#assetmodelcompositemodeloutputtypedef) 



## ActionDefinitionTypeDef

```python
# ActionDefinitionTypeDef definition

class ActionDefinitionTypeDef(TypedDict):
    actionDefinitionId: str,
    actionName: str,
    actionType: str,
```

## ActionPayloadTypeDef

```python
# ActionPayloadTypeDef definition

class ActionPayloadTypeDef(TypedDict):
    stringValue: str,
```

## TargetResourceTypeDef

```python
# TargetResourceTypeDef definition

class TargetResourceTypeDef(TypedDict):
    assetId: str,
```

## AggregatesTypeDef

```python
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
# AlarmsTypeDef definition

class AlarmsTypeDef(TypedDict):
    alarmRoleArn: str,
    notificationLambdaArn: NotRequired[str],
```

## AssetCompositeModelPathSegmentTypeDef

```python
# AssetCompositeModelPathSegmentTypeDef definition

class AssetCompositeModelPathSegmentTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
```

## AssetErrorDetailsTypeDef

```python
# AssetErrorDetailsTypeDef definition

class AssetErrorDetailsTypeDef(TypedDict):
    assetId: str,
    code: AssetErrorCodeType,  # (1)
    message: str,
```

1. See [:material-code-brackets: AssetErrorCodeType](./literals.md#asseterrorcodetype) 
## AssetHierarchyInfoTypeDef

```python
# AssetHierarchyInfoTypeDef definition

class AssetHierarchyInfoTypeDef(TypedDict):
    parentAssetId: NotRequired[str],
    childAssetId: NotRequired[str],
```

## AssetHierarchyTypeDef

```python
# AssetHierarchyTypeDef definition

class AssetHierarchyTypeDef(TypedDict):
    name: str,
    id: NotRequired[str],
    externalId: NotRequired[str],
```

## AssetModelCompositeModelPathSegmentTypeDef

```python
# AssetModelCompositeModelPathSegmentTypeDef definition

class AssetModelCompositeModelPathSegmentTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
```

## AssetModelHierarchyDefinitionTypeDef

```python
# AssetModelHierarchyDefinitionTypeDef definition

class AssetModelHierarchyDefinitionTypeDef(TypedDict):
    name: str,
    childAssetModelId: str,
    id: NotRequired[str],
    externalId: NotRequired[str],
```

## AssetModelHierarchyTypeDef

```python
# AssetModelHierarchyTypeDef definition

class AssetModelHierarchyTypeDef(TypedDict):
    name: str,
    childAssetModelId: str,
    id: NotRequired[str],
    externalId: NotRequired[str],
```

## AssetModelPropertyPathSegmentTypeDef

```python
# AssetModelPropertyPathSegmentTypeDef definition

class AssetModelPropertyPathSegmentTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
```

## AssetPropertyPathSegmentTypeDef

```python
# AssetPropertyPathSegmentTypeDef definition

class AssetPropertyPathSegmentTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
```

## PropertyNotificationTypeDef

```python
# PropertyNotificationTypeDef definition

class PropertyNotificationTypeDef(TypedDict):
    topic: str,
    state: PropertyNotificationStateType,  # (1)
```

1. See [:material-code-brackets: PropertyNotificationStateType](./literals.md#propertynotificationstatetype) 
## TimeInNanosTypeDef

```python
# TimeInNanosTypeDef definition

class TimeInNanosTypeDef(TypedDict):
    timeInSeconds: int,
    offsetInNanos: NotRequired[int],
```

## VariantTypeDef

```python
# VariantTypeDef definition

class VariantTypeDef(TypedDict):
    stringValue: NotRequired[str],
    integerValue: NotRequired[int],
    doubleValue: NotRequired[float],
    booleanValue: NotRequired[bool],
```

## AssociateAssetsRequestRequestTypeDef

```python
# AssociateAssetsRequestRequestTypeDef definition

class AssociateAssetsRequestRequestTypeDef(TypedDict):
    assetId: str,
    hierarchyId: str,
    childAssetId: str,
    clientToken: NotRequired[str],
```

## AssociateTimeSeriesToAssetPropertyRequestRequestTypeDef

```python
# AssociateTimeSeriesToAssetPropertyRequestRequestTypeDef definition

class AssociateTimeSeriesToAssetPropertyRequestRequestTypeDef(TypedDict):
    alias: str,
    assetId: str,
    propertyId: str,
    clientToken: NotRequired[str],
```

## AttributeTypeDef

```python
# AttributeTypeDef definition

class AttributeTypeDef(TypedDict):
    defaultValue: NotRequired[str],
```

## BatchAssociateProjectAssetsRequestRequestTypeDef

```python
# BatchAssociateProjectAssetsRequestRequestTypeDef definition

class BatchAssociateProjectAssetsRequestRequestTypeDef(TypedDict):
    projectId: str,
    assetIds: Sequence[str],
    clientToken: NotRequired[str],
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

## BatchDisassociateProjectAssetsRequestRequestTypeDef

```python
# BatchDisassociateProjectAssetsRequestRequestTypeDef definition

class BatchDisassociateProjectAssetsRequestRequestTypeDef(TypedDict):
    projectId: str,
    assetIds: Sequence[str],
    clientToken: NotRequired[str],
```

## BatchGetAssetPropertyAggregatesErrorEntryTypeDef

```python
# BatchGetAssetPropertyAggregatesErrorEntryTypeDef definition

class BatchGetAssetPropertyAggregatesErrorEntryTypeDef(TypedDict):
    errorCode: BatchGetAssetPropertyAggregatesErrorCodeType,  # (1)
    errorMessage: str,
    entryId: str,
```

1. See [:material-code-brackets: BatchGetAssetPropertyAggregatesErrorCodeType](./literals.md#batchgetassetpropertyaggregateserrorcodetype) 
## BatchGetAssetPropertyAggregatesErrorInfoTypeDef

```python
# BatchGetAssetPropertyAggregatesErrorInfoTypeDef definition

class BatchGetAssetPropertyAggregatesErrorInfoTypeDef(TypedDict):
    errorCode: BatchGetAssetPropertyAggregatesErrorCodeType,  # (1)
    errorTimestamp: datetime,
```

1. See [:material-code-brackets: BatchGetAssetPropertyAggregatesErrorCodeType](./literals.md#batchgetassetpropertyaggregateserrorcodetype) 
## BatchGetAssetPropertyValueEntryTypeDef

```python
# BatchGetAssetPropertyValueEntryTypeDef definition

class BatchGetAssetPropertyValueEntryTypeDef(TypedDict):
    entryId: str,
    assetId: NotRequired[str],
    propertyId: NotRequired[str],
    propertyAlias: NotRequired[str],
```

## BatchGetAssetPropertyValueErrorEntryTypeDef

```python
# BatchGetAssetPropertyValueErrorEntryTypeDef definition

class BatchGetAssetPropertyValueErrorEntryTypeDef(TypedDict):
    errorCode: BatchGetAssetPropertyValueErrorCodeType,  # (1)
    errorMessage: str,
    entryId: str,
```

1. See [:material-code-brackets: BatchGetAssetPropertyValueErrorCodeType](./literals.md#batchgetassetpropertyvalueerrorcodetype) 
## BatchGetAssetPropertyValueErrorInfoTypeDef

```python
# BatchGetAssetPropertyValueErrorInfoTypeDef definition

class BatchGetAssetPropertyValueErrorInfoTypeDef(TypedDict):
    errorCode: BatchGetAssetPropertyValueErrorCodeType,  # (1)
    errorTimestamp: datetime,
```

1. See [:material-code-brackets: BatchGetAssetPropertyValueErrorCodeType](./literals.md#batchgetassetpropertyvalueerrorcodetype) 
## BatchGetAssetPropertyValueHistoryErrorEntryTypeDef

```python
# BatchGetAssetPropertyValueHistoryErrorEntryTypeDef definition

class BatchGetAssetPropertyValueHistoryErrorEntryTypeDef(TypedDict):
    errorCode: BatchGetAssetPropertyValueHistoryErrorCodeType,  # (1)
    errorMessage: str,
    entryId: str,
```

1. See [:material-code-brackets: BatchGetAssetPropertyValueHistoryErrorCodeType](./literals.md#batchgetassetpropertyvaluehistoryerrorcodetype) 
## BatchGetAssetPropertyValueHistoryErrorInfoTypeDef

```python
# BatchGetAssetPropertyValueHistoryErrorInfoTypeDef definition

class BatchGetAssetPropertyValueHistoryErrorInfoTypeDef(TypedDict):
    errorCode: BatchGetAssetPropertyValueHistoryErrorCodeType,  # (1)
    errorTimestamp: datetime,
```

1. See [:material-code-brackets: BatchGetAssetPropertyValueHistoryErrorCodeType](./literals.md#batchgetassetpropertyvaluehistoryerrorcodetype) 
## ColumnTypeTypeDef

```python
# ColumnTypeTypeDef definition

class ColumnTypeTypeDef(TypedDict):
    scalarType: NotRequired[ScalarTypeType],  # (1)
```

1. See [:material-code-brackets: ScalarTypeType](./literals.md#scalartypetype) 
## CompositionRelationshipItemTypeDef

```python
# CompositionRelationshipItemTypeDef definition

class CompositionRelationshipItemTypeDef(TypedDict):
    id: NotRequired[str],
```

## CompositionRelationshipSummaryTypeDef

```python
# CompositionRelationshipSummaryTypeDef definition

class CompositionRelationshipSummaryTypeDef(TypedDict):
    assetModelId: str,
    assetModelCompositeModelId: str,
    assetModelCompositeModelType: str,
```

## ConfigurationErrorDetailsTypeDef

```python
# ConfigurationErrorDetailsTypeDef definition

class ConfigurationErrorDetailsTypeDef(TypedDict):
    code: ErrorCodeType,  # (1)
    message: str,
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
## CreateAssetRequestRequestTypeDef

```python
# CreateAssetRequestRequestTypeDef definition

class CreateAssetRequestRequestTypeDef(TypedDict):
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
# ErrorReportLocationTypeDef definition

class ErrorReportLocationTypeDef(TypedDict):
    bucket: str,
    prefix: str,
```

## FileTypeDef

```python
# FileTypeDef definition

class FileTypeDef(TypedDict):
    bucket: str,
    key: str,
    versionId: NotRequired[str],
```

## CreateDashboardRequestRequestTypeDef

```python
# CreateDashboardRequestRequestTypeDef definition

class CreateDashboardRequestRequestTypeDef(TypedDict):
    projectId: str,
    dashboardName: str,
    dashboardDefinition: str,
    dashboardDescription: NotRequired[str],
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## CreateProjectRequestRequestTypeDef

```python
# CreateProjectRequestRequestTypeDef definition

class CreateProjectRequestRequestTypeDef(TypedDict):
    portalId: str,
    projectName: str,
    projectDescription: NotRequired[str],
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## CsvOutputTypeDef

```python
# CsvOutputTypeDef definition

class CsvOutputTypeDef(TypedDict):
    columnNames: List[ColumnNameType],  # (1)
```

1. See [:material-code-brackets: ColumnNameType](./literals.md#columnnametype) 
## CsvTypeDef

```python
# CsvTypeDef definition

class CsvTypeDef(TypedDict):
    columnNames: Sequence[ColumnNameType],  # (1)
```

1. See [:material-code-brackets: ColumnNameType](./literals.md#columnnametype) 
## CustomerManagedS3StorageTypeDef

```python
# CustomerManagedS3StorageTypeDef definition

class CustomerManagedS3StorageTypeDef(TypedDict):
    s3ResourceArn: str,
    roleArn: str,
```

## DashboardSummaryTypeDef

```python
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
# DatumPaginatorTypeDef definition

class DatumPaginatorTypeDef(TypedDict):
    scalarValue: NotRequired[str],
    arrayValue: NotRequired[List[Dict[str, Any]]],
    rowValue: NotRequired[Dict[str, Any]],
    nullValue: NotRequired[bool],
```

## DatumTypeDef

```python
# DatumTypeDef definition

class DatumTypeDef(TypedDict):
    scalarValue: NotRequired[str],
    arrayValue: NotRequired[List[Dict[str, Any]]],
    rowValue: NotRequired[Dict[str, Any]],
    nullValue: NotRequired[bool],
```

## DeleteAccessPolicyRequestRequestTypeDef

```python
# DeleteAccessPolicyRequestRequestTypeDef definition

class DeleteAccessPolicyRequestRequestTypeDef(TypedDict):
    accessPolicyId: str,
    clientToken: NotRequired[str],
```

## DeleteAssetModelCompositeModelRequestRequestTypeDef

```python
# DeleteAssetModelCompositeModelRequestRequestTypeDef definition

class DeleteAssetModelCompositeModelRequestRequestTypeDef(TypedDict):
    assetModelId: str,
    assetModelCompositeModelId: str,
    clientToken: NotRequired[str],
    ifMatch: NotRequired[str],
    ifNoneMatch: NotRequired[str],
    matchForVersionType: NotRequired[AssetModelVersionTypeType],  # (1)
```

1. See [:material-code-brackets: AssetModelVersionTypeType](./literals.md#assetmodelversiontypetype) 
## DeleteAssetModelRequestRequestTypeDef

```python
# DeleteAssetModelRequestRequestTypeDef definition

class DeleteAssetModelRequestRequestTypeDef(TypedDict):
    assetModelId: str,
    clientToken: NotRequired[str],
    ifMatch: NotRequired[str],
    ifNoneMatch: NotRequired[str],
    matchForVersionType: NotRequired[AssetModelVersionTypeType],  # (1)
```

1. See [:material-code-brackets: AssetModelVersionTypeType](./literals.md#assetmodelversiontypetype) 
## DeleteAssetRequestRequestTypeDef

```python
# DeleteAssetRequestRequestTypeDef definition

class DeleteAssetRequestRequestTypeDef(TypedDict):
    assetId: str,
    clientToken: NotRequired[str],
```

## DeleteDashboardRequestRequestTypeDef

```python
# DeleteDashboardRequestRequestTypeDef definition

class DeleteDashboardRequestRequestTypeDef(TypedDict):
    dashboardId: str,
    clientToken: NotRequired[str],
```

## DeleteGatewayRequestRequestTypeDef

```python
# DeleteGatewayRequestRequestTypeDef definition

class DeleteGatewayRequestRequestTypeDef(TypedDict):
    gatewayId: str,
```

## DeletePortalRequestRequestTypeDef

```python
# DeletePortalRequestRequestTypeDef definition

class DeletePortalRequestRequestTypeDef(TypedDict):
    portalId: str,
    clientToken: NotRequired[str],
```

## DeleteProjectRequestRequestTypeDef

```python
# DeleteProjectRequestRequestTypeDef definition

class DeleteProjectRequestRequestTypeDef(TypedDict):
    projectId: str,
    clientToken: NotRequired[str],
```

## DeleteTimeSeriesRequestRequestTypeDef

```python
# DeleteTimeSeriesRequestRequestTypeDef definition

class DeleteTimeSeriesRequestRequestTypeDef(TypedDict):
    alias: NotRequired[str],
    assetId: NotRequired[str],
    propertyId: NotRequired[str],
    clientToken: NotRequired[str],
```

## DescribeAccessPolicyRequestRequestTypeDef

```python
# DescribeAccessPolicyRequestRequestTypeDef definition

class DescribeAccessPolicyRequestRequestTypeDef(TypedDict):
    accessPolicyId: str,
```

## DescribeActionRequestRequestTypeDef

```python
# DescribeActionRequestRequestTypeDef definition

class DescribeActionRequestRequestTypeDef(TypedDict):
    actionId: str,
```

## DescribeAssetCompositeModelRequestRequestTypeDef

```python
# DescribeAssetCompositeModelRequestRequestTypeDef definition

class DescribeAssetCompositeModelRequestRequestTypeDef(TypedDict):
    assetId: str,
    assetCompositeModelId: str,
```

## DescribeAssetModelCompositeModelRequestRequestTypeDef

```python
# DescribeAssetModelCompositeModelRequestRequestTypeDef definition

class DescribeAssetModelCompositeModelRequestRequestTypeDef(TypedDict):
    assetModelId: str,
    assetModelCompositeModelId: str,
    assetModelVersion: NotRequired[str],
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeAssetModelRequestRequestTypeDef

```python
# DescribeAssetModelRequestRequestTypeDef definition

class DescribeAssetModelRequestRequestTypeDef(TypedDict):
    assetModelId: str,
    excludeProperties: NotRequired[bool],
    assetModelVersion: NotRequired[str],
```

## DescribeAssetPropertyRequestRequestTypeDef

```python
# DescribeAssetPropertyRequestRequestTypeDef definition

class DescribeAssetPropertyRequestRequestTypeDef(TypedDict):
    assetId: str,
    propertyId: str,
```

## DescribeAssetRequestRequestTypeDef

```python
# DescribeAssetRequestRequestTypeDef definition

class DescribeAssetRequestRequestTypeDef(TypedDict):
    assetId: str,
    excludeProperties: NotRequired[bool],
```

## DescribeBulkImportJobRequestRequestTypeDef

```python
# DescribeBulkImportJobRequestRequestTypeDef definition

class DescribeBulkImportJobRequestRequestTypeDef(TypedDict):
    jobId: str,
```

## DescribeDashboardRequestRequestTypeDef

```python
# DescribeDashboardRequestRequestTypeDef definition

class DescribeDashboardRequestRequestTypeDef(TypedDict):
    dashboardId: str,
```

## DescribeGatewayCapabilityConfigurationRequestRequestTypeDef

```python
# DescribeGatewayCapabilityConfigurationRequestRequestTypeDef definition

class DescribeGatewayCapabilityConfigurationRequestRequestTypeDef(TypedDict):
    gatewayId: str,
    capabilityNamespace: str,
```

## DescribeGatewayRequestRequestTypeDef

```python
# DescribeGatewayRequestRequestTypeDef definition

class DescribeGatewayRequestRequestTypeDef(TypedDict):
    gatewayId: str,
```

## GatewayCapabilitySummaryTypeDef

```python
# GatewayCapabilitySummaryTypeDef definition

class GatewayCapabilitySummaryTypeDef(TypedDict):
    capabilityNamespace: str,
    capabilitySyncStatus: CapabilitySyncStatusType,  # (1)
```

1. See [:material-code-brackets: CapabilitySyncStatusType](./literals.md#capabilitysyncstatustype) 
## LoggingOptionsTypeDef

```python
# LoggingOptionsTypeDef definition

class LoggingOptionsTypeDef(TypedDict):
    level: LoggingLevelType,  # (1)
```

1. See [:material-code-brackets: LoggingLevelType](./literals.md#loggingleveltype) 
## DescribePortalRequestRequestTypeDef

```python
# DescribePortalRequestRequestTypeDef definition

class DescribePortalRequestRequestTypeDef(TypedDict):
    portalId: str,
```

## ImageLocationTypeDef

```python
# ImageLocationTypeDef definition

class ImageLocationTypeDef(TypedDict):
    id: str,
    url: str,
```

## DescribeProjectRequestRequestTypeDef

```python
# DescribeProjectRequestRequestTypeDef definition

class DescribeProjectRequestRequestTypeDef(TypedDict):
    projectId: str,
```

## RetentionPeriodTypeDef

```python
# RetentionPeriodTypeDef definition

class RetentionPeriodTypeDef(TypedDict):
    numberOfDays: NotRequired[int],
    unlimited: NotRequired[bool],
```

## WarmTierRetentionPeriodTypeDef

```python
# WarmTierRetentionPeriodTypeDef definition

class WarmTierRetentionPeriodTypeDef(TypedDict):
    numberOfDays: NotRequired[int],
    unlimited: NotRequired[bool],
```

## DescribeTimeSeriesRequestRequestTypeDef

```python
# DescribeTimeSeriesRequestRequestTypeDef definition

class DescribeTimeSeriesRequestRequestTypeDef(TypedDict):
    alias: NotRequired[str],
    assetId: NotRequired[str],
    propertyId: NotRequired[str],
```

## DetailedErrorTypeDef

```python
# DetailedErrorTypeDef definition

class DetailedErrorTypeDef(TypedDict):
    code: DetailedErrorCodeType,  # (1)
    message: str,
```

1. See [:material-code-brackets: DetailedErrorCodeType](./literals.md#detailederrorcodetype) 
## DisassociateAssetsRequestRequestTypeDef

```python
# DisassociateAssetsRequestRequestTypeDef definition

class DisassociateAssetsRequestRequestTypeDef(TypedDict):
    assetId: str,
    hierarchyId: str,
    childAssetId: str,
    clientToken: NotRequired[str],
```

## DisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef

```python
# DisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef definition

class DisassociateTimeSeriesFromAssetPropertyRequestRequestTypeDef(TypedDict):
    alias: str,
    assetId: str,
    propertyId: str,
    clientToken: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ExecuteQueryRequestRequestTypeDef

```python
# ExecuteQueryRequestRequestTypeDef definition

class ExecuteQueryRequestRequestTypeDef(TypedDict):
    queryStatement: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ForwardingConfigTypeDef

```python
# ForwardingConfigTypeDef definition

class ForwardingConfigTypeDef(TypedDict):
    state: ForwardingConfigStateType,  # (1)
```

1. See [:material-code-brackets: ForwardingConfigStateType](./literals.md#forwardingconfigstatetype) 
## GreengrassTypeDef

```python
# GreengrassTypeDef definition

class GreengrassTypeDef(TypedDict):
    groupArn: str,
```

## GreengrassV2TypeDef

```python
# GreengrassV2TypeDef definition

class GreengrassV2TypeDef(TypedDict):
    coreDeviceThingName: str,
```

## SiemensIETypeDef

```python
# SiemensIETypeDef definition

class SiemensIETypeDef(TypedDict):
    iotCoreThingName: str,
```

## GetAssetPropertyValueRequestRequestTypeDef

```python
# GetAssetPropertyValueRequestRequestTypeDef definition

class GetAssetPropertyValueRequestRequestTypeDef(TypedDict):
    assetId: NotRequired[str],
    propertyId: NotRequired[str],
    propertyAlias: NotRequired[str],
```

## GetInterpolatedAssetPropertyValuesRequestRequestTypeDef

```python
# GetInterpolatedAssetPropertyValuesRequestRequestTypeDef definition

class GetInterpolatedAssetPropertyValuesRequestRequestTypeDef(TypedDict):
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
# GroupIdentityTypeDef definition

class GroupIdentityTypeDef(TypedDict):
    id: str,
```

## IAMRoleIdentityTypeDef

```python
# IAMRoleIdentityTypeDef definition

class IAMRoleIdentityTypeDef(TypedDict):
    arn: str,
```

## IAMUserIdentityTypeDef

```python
# IAMUserIdentityTypeDef definition

class IAMUserIdentityTypeDef(TypedDict):
    arn: str,
```

## UserIdentityTypeDef

```python
# UserIdentityTypeDef definition

class UserIdentityTypeDef(TypedDict):
    id: str,
```

## JobSummaryTypeDef

```python
# JobSummaryTypeDef definition

class JobSummaryTypeDef(TypedDict):
    id: str,
    name: str,
    status: JobStatusType,  # (1)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## ListAccessPoliciesRequestRequestTypeDef

```python
# ListAccessPoliciesRequestRequestTypeDef definition

class ListAccessPoliciesRequestRequestTypeDef(TypedDict):
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
## ListActionsRequestRequestTypeDef

```python
# ListActionsRequestRequestTypeDef definition

class ListActionsRequestRequestTypeDef(TypedDict):
    targetResourceType: TargetResourceTypeType,  # (1)
    targetResourceId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: TargetResourceTypeType](./literals.md#targetresourcetypetype) 
## ListAssetModelCompositeModelsRequestRequestTypeDef

```python
# ListAssetModelCompositeModelsRequestRequestTypeDef definition

class ListAssetModelCompositeModelsRequestRequestTypeDef(TypedDict):
    assetModelId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    assetModelVersion: NotRequired[str],
```

## ListAssetModelPropertiesRequestRequestTypeDef

```python
# ListAssetModelPropertiesRequestRequestTypeDef definition

class ListAssetModelPropertiesRequestRequestTypeDef(TypedDict):
    assetModelId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filter: NotRequired[ListAssetModelPropertiesFilterType],  # (1)
    assetModelVersion: NotRequired[str],
```

1. See [:material-code-brackets: ListAssetModelPropertiesFilterType](./literals.md#listassetmodelpropertiesfiltertype) 
## ListAssetModelsRequestRequestTypeDef

```python
# ListAssetModelsRequestRequestTypeDef definition

class ListAssetModelsRequestRequestTypeDef(TypedDict):
    assetModelTypes: NotRequired[Sequence[AssetModelTypeType]],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    assetModelVersion: NotRequired[str],
```

1. See [:material-code-brackets: AssetModelTypeType](./literals.md#assetmodeltypetype) 
## ListAssetPropertiesRequestRequestTypeDef

```python
# ListAssetPropertiesRequestRequestTypeDef definition

class ListAssetPropertiesRequestRequestTypeDef(TypedDict):
    assetId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filter: NotRequired[ListAssetPropertiesFilterType],  # (1)
```

1. See [:material-code-brackets: ListAssetPropertiesFilterType](./literals.md#listassetpropertiesfiltertype) 
## ListAssetRelationshipsRequestRequestTypeDef

```python
# ListAssetRelationshipsRequestRequestTypeDef definition

class ListAssetRelationshipsRequestRequestTypeDef(TypedDict):
    assetId: str,
    traversalType: TraversalTypeType,  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: TraversalTypeType](./literals.md#traversaltypetype) 
## ListAssetsRequestRequestTypeDef

```python
# ListAssetsRequestRequestTypeDef definition

class ListAssetsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    assetModelId: NotRequired[str],
    filter: NotRequired[ListAssetsFilterType],  # (1)
```

1. See [:material-code-brackets: ListAssetsFilterType](./literals.md#listassetsfiltertype) 
## ListAssociatedAssetsRequestRequestTypeDef

```python
# ListAssociatedAssetsRequestRequestTypeDef definition

class ListAssociatedAssetsRequestRequestTypeDef(TypedDict):
    assetId: str,
    hierarchyId: NotRequired[str],
    traversalDirection: NotRequired[TraversalDirectionType],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: TraversalDirectionType](./literals.md#traversaldirectiontype) 
## ListBulkImportJobsRequestRequestTypeDef

```python
# ListBulkImportJobsRequestRequestTypeDef definition

class ListBulkImportJobsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    filter: NotRequired[ListBulkImportJobsFilterType],  # (1)
```

1. See [:material-code-brackets: ListBulkImportJobsFilterType](./literals.md#listbulkimportjobsfiltertype) 
## ListCompositionRelationshipsRequestRequestTypeDef

```python
# ListCompositionRelationshipsRequestRequestTypeDef definition

class ListCompositionRelationshipsRequestRequestTypeDef(TypedDict):
    assetModelId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListDashboardsRequestRequestTypeDef

```python
# ListDashboardsRequestRequestTypeDef definition

class ListDashboardsRequestRequestTypeDef(TypedDict):
    projectId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListGatewaysRequestRequestTypeDef

```python
# ListGatewaysRequestRequestTypeDef definition

class ListGatewaysRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListPortalsRequestRequestTypeDef

```python
# ListPortalsRequestRequestTypeDef definition

class ListPortalsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListProjectAssetsRequestRequestTypeDef

```python
# ListProjectAssetsRequestRequestTypeDef definition

class ListProjectAssetsRequestRequestTypeDef(TypedDict):
    projectId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListProjectsRequestRequestTypeDef

```python
# ListProjectsRequestRequestTypeDef definition

class ListProjectsRequestRequestTypeDef(TypedDict):
    portalId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ProjectSummaryTypeDef

```python
# ProjectSummaryTypeDef definition

class ProjectSummaryTypeDef(TypedDict):
    id: str,
    name: str,
    description: NotRequired[str],
    creationDate: NotRequired[datetime],
    lastUpdateDate: NotRequired[datetime],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListTimeSeriesRequestRequestTypeDef

```python
# ListTimeSeriesRequestRequestTypeDef definition

class ListTimeSeriesRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    assetId: NotRequired[str],
    aliasPrefix: NotRequired[str],
    timeSeriesType: NotRequired[ListTimeSeriesTypeType],  # (1)
```

1. See [:material-code-brackets: ListTimeSeriesTypeType](./literals.md#listtimeseriestypetype) 
## TimeSeriesSummaryTypeDef

```python
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
## MetricProcessingConfigTypeDef

```python
# MetricProcessingConfigTypeDef definition

class MetricProcessingConfigTypeDef(TypedDict):
    computeLocation: ComputeLocationType,  # (1)
```

1. See [:material-code-brackets: ComputeLocationType](./literals.md#computelocationtype) 
## TumblingWindowTypeDef

```python
# TumblingWindowTypeDef definition

class TumblingWindowTypeDef(TypedDict):
    interval: str,
    offset: NotRequired[str],
```

## MonitorErrorDetailsTypeDef

```python
# MonitorErrorDetailsTypeDef definition

class MonitorErrorDetailsTypeDef(TypedDict):
    code: NotRequired[MonitorErrorCodeType],  # (1)
    message: NotRequired[str],
```

1. See [:material-code-brackets: MonitorErrorCodeType](./literals.md#monitorerrorcodetype) 
## PortalResourceTypeDef

```python
# PortalResourceTypeDef definition

class PortalResourceTypeDef(TypedDict):
    id: str,
```

## ProjectResourceTypeDef

```python
# ProjectResourceTypeDef definition

class ProjectResourceTypeDef(TypedDict):
    id: str,
```

## PutDefaultEncryptionConfigurationRequestRequestTypeDef

```python
# PutDefaultEncryptionConfigurationRequestRequestTypeDef definition

class PutDefaultEncryptionConfigurationRequestRequestTypeDef(TypedDict):
    encryptionType: EncryptionTypeType,  # (1)
    kmsKeyId: NotRequired[str],
```

1. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
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

## UpdateAssetPropertyRequestRequestTypeDef

```python
# UpdateAssetPropertyRequestRequestTypeDef definition

class UpdateAssetPropertyRequestRequestTypeDef(TypedDict):
    assetId: str,
    propertyId: str,
    propertyAlias: NotRequired[str],
    propertyNotificationState: NotRequired[PropertyNotificationStateType],  # (1)
    clientToken: NotRequired[str],
    propertyUnit: NotRequired[str],
```

1. See [:material-code-brackets: PropertyNotificationStateType](./literals.md#propertynotificationstatetype) 
## UpdateAssetRequestRequestTypeDef

```python
# UpdateAssetRequestRequestTypeDef definition

class UpdateAssetRequestRequestTypeDef(TypedDict):
    assetId: str,
    assetName: str,
    clientToken: NotRequired[str],
    assetDescription: NotRequired[str],
    assetExternalId: NotRequired[str],
```

## UpdateDashboardRequestRequestTypeDef

```python
# UpdateDashboardRequestRequestTypeDef definition

class UpdateDashboardRequestRequestTypeDef(TypedDict):
    dashboardId: str,
    dashboardName: str,
    dashboardDefinition: str,
    dashboardDescription: NotRequired[str],
    clientToken: NotRequired[str],
```

## UpdateGatewayCapabilityConfigurationRequestRequestTypeDef

```python
# UpdateGatewayCapabilityConfigurationRequestRequestTypeDef definition

class UpdateGatewayCapabilityConfigurationRequestRequestTypeDef(TypedDict):
    gatewayId: str,
    capabilityNamespace: str,
    capabilityConfiguration: str,
```

## UpdateGatewayRequestRequestTypeDef

```python
# UpdateGatewayRequestRequestTypeDef definition

class UpdateGatewayRequestRequestTypeDef(TypedDict):
    gatewayId: str,
    gatewayName: str,
```

## UpdateProjectRequestRequestTypeDef

```python
# UpdateProjectRequestRequestTypeDef definition

class UpdateProjectRequestRequestTypeDef(TypedDict):
    projectId: str,
    projectName: str,
    projectDescription: NotRequired[str],
    clientToken: NotRequired[str],
```

## ActionSummaryTypeDef

```python
# ActionSummaryTypeDef definition

class ActionSummaryTypeDef(TypedDict):
    actionId: NotRequired[str],
    actionDefinitionId: NotRequired[str],
    targetResource: NotRequired[TargetResourceTypeDef],  # (1)
```

1. See [:material-code-braces: TargetResourceTypeDef](./type_defs.md#targetresourcetypedef) 
## ExecuteActionRequestRequestTypeDef

```python
# ExecuteActionRequestRequestTypeDef definition

class ExecuteActionRequestRequestTypeDef(TypedDict):
    targetResource: TargetResourceTypeDef,  # (1)
    actionDefinitionId: str,
    actionPayload: ActionPayloadTypeDef,  # (2)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: TargetResourceTypeDef](./type_defs.md#targetresourcetypedef) 
2. See [:material-code-braces: ActionPayloadTypeDef](./type_defs.md#actionpayloadtypedef) 
## AggregatedValueTypeDef

```python
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
# AssetRelationshipSummaryTypeDef definition

class AssetRelationshipSummaryTypeDef(TypedDict):
    relationshipType: AssetRelationshipTypeType,  # (2)
    hierarchyInfo: NotRequired[AssetHierarchyInfoTypeDef],  # (1)
```

1. See [:material-code-braces: AssetHierarchyInfoTypeDef](./type_defs.md#assethierarchyinfotypedef) 
2. See [:material-code-brackets: AssetRelationshipTypeType](./literals.md#assetrelationshiptypetype) 
## AssetModelCompositeModelSummaryTypeDef

```python
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
# VariableValueOutputTypeDef definition

class VariableValueOutputTypeDef(TypedDict):
    propertyId: NotRequired[str],
    hierarchyId: NotRequired[str],
    propertyPath: NotRequired[List[AssetModelPropertyPathSegmentTypeDef]],  # (1)
```

1. See [:material-code-braces: AssetModelPropertyPathSegmentTypeDef](./type_defs.md#assetmodelpropertypathsegmenttypedef) 
## VariableValueTypeDef

```python
# VariableValueTypeDef definition

class VariableValueTypeDef(TypedDict):
    propertyId: NotRequired[str],
    hierarchyId: NotRequired[str],
    propertyPath: NotRequired[Sequence[AssetModelPropertyPathSegmentTypeDef]],  # (1)
```

1. See [:material-code-braces: AssetModelPropertyPathSegmentTypeDef](./type_defs.md#assetmodelpropertypathsegmenttypedef) 
## AssetPropertySummaryTypeDef

```python
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
# BatchPutAssetPropertyErrorTypeDef definition

class BatchPutAssetPropertyErrorTypeDef(TypedDict):
    errorCode: BatchPutAssetPropertyValueErrorCodeType,  # (1)
    errorMessage: str,
    timestamps: List[TimeInNanosTypeDef],  # (2)
```

1. See [:material-code-brackets: BatchPutAssetPropertyValueErrorCodeType](./literals.md#batchputassetpropertyvalueerrorcodetype) 
2. See [:material-code-braces: TimeInNanosTypeDef](./type_defs.md#timeinnanostypedef) 
## AssetPropertyValueTypeDef

```python
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
# InterpolatedAssetPropertyValueTypeDef definition

class InterpolatedAssetPropertyValueTypeDef(TypedDict):
    timestamp: TimeInNanosTypeDef,  # (1)
    value: VariantTypeDef,  # (2)
```

1. See [:material-code-braces: TimeInNanosTypeDef](./type_defs.md#timeinnanostypedef) 
2. See [:material-code-braces: VariantTypeDef](./type_defs.md#varianttypedef) 
## BatchAssociateProjectAssetsResponseTypeDef

```python
# BatchAssociateProjectAssetsResponseTypeDef definition

class BatchAssociateProjectAssetsResponseTypeDef(TypedDict):
    errors: List[AssetErrorDetailsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssetErrorDetailsTypeDef](./type_defs.md#asseterrordetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDisassociateProjectAssetsResponseTypeDef

```python
# BatchDisassociateProjectAssetsResponseTypeDef definition

class BatchDisassociateProjectAssetsResponseTypeDef(TypedDict):
    errors: List[AssetErrorDetailsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssetErrorDetailsTypeDef](./type_defs.md#asseterrordetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAccessPolicyResponseTypeDef

```python
# CreateAccessPolicyResponseTypeDef definition

class CreateAccessPolicyResponseTypeDef(TypedDict):
    accessPolicyId: str,
    accessPolicyArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBulkImportJobResponseTypeDef

```python
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
# CreateDashboardResponseTypeDef definition

class CreateDashboardResponseTypeDef(TypedDict):
    dashboardId: str,
    dashboardArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGatewayResponseTypeDef

```python
# CreateGatewayResponseTypeDef definition

class CreateGatewayResponseTypeDef(TypedDict):
    gatewayId: str,
    gatewayArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProjectResponseTypeDef

```python
# CreateProjectResponseTypeDef definition

class CreateProjectResponseTypeDef(TypedDict):
    projectId: str,
    projectArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeActionResponseTypeDef

```python
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
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExecuteActionResponseTypeDef

```python
# ExecuteActionResponseTypeDef definition

class ExecuteActionResponseTypeDef(TypedDict):
    actionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProjectAssetsResponseTypeDef

```python
# ListProjectAssetsResponseTypeDef definition

class ListProjectAssetsResponseTypeDef(TypedDict):
    assetIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
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
## UpdateGatewayCapabilityConfigurationResponseTypeDef

```python
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
## GetAssetPropertyAggregatesRequestRequestTypeDef

```python
# GetAssetPropertyAggregatesRequestRequestTypeDef definition

class GetAssetPropertyAggregatesRequestRequestTypeDef(TypedDict):
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
## GetAssetPropertyValueHistoryRequestRequestTypeDef

```python
# GetAssetPropertyValueHistoryRequestRequestTypeDef definition

class GetAssetPropertyValueHistoryRequestRequestTypeDef(TypedDict):
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
# BatchGetAssetPropertyAggregatesSkippedEntryTypeDef definition

class BatchGetAssetPropertyAggregatesSkippedEntryTypeDef(TypedDict):
    entryId: str,
    completionStatus: BatchEntryCompletionStatusType,  # (1)
    errorInfo: NotRequired[BatchGetAssetPropertyAggregatesErrorInfoTypeDef],  # (2)
```

1. See [:material-code-brackets: BatchEntryCompletionStatusType](./literals.md#batchentrycompletionstatustype) 
2. See [:material-code-braces: BatchGetAssetPropertyAggregatesErrorInfoTypeDef](./type_defs.md#batchgetassetpropertyaggregateserrorinfotypedef) 
## BatchGetAssetPropertyValueRequestRequestTypeDef

```python
# BatchGetAssetPropertyValueRequestRequestTypeDef definition

class BatchGetAssetPropertyValueRequestRequestTypeDef(TypedDict):
    entries: Sequence[BatchGetAssetPropertyValueEntryTypeDef],  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BatchGetAssetPropertyValueEntryTypeDef](./type_defs.md#batchgetassetpropertyvalueentrytypedef) 
## BatchGetAssetPropertyValueSkippedEntryTypeDef

```python
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
# ImageFileTypeDef definition

class ImageFileTypeDef(TypedDict):
    data: BlobTypeDef,
    type: ImageFileTypeType,  # (1)
```

1. See [:material-code-brackets: ImageFileTypeType](./literals.md#imagefiletypetype) 
## ColumnInfoTypeDef

```python
# ColumnInfoTypeDef definition

class ColumnInfoTypeDef(TypedDict):
    name: NotRequired[str],
    type: NotRequired[ColumnTypeTypeDef],  # (1)
```

1. See [:material-code-braces: ColumnTypeTypeDef](./type_defs.md#columntypetypedef) 
## CompositionDetailsTypeDef

```python
# CompositionDetailsTypeDef definition

class CompositionDetailsTypeDef(TypedDict):
    compositionRelationship: NotRequired[List[CompositionRelationshipItemTypeDef]],  # (1)
```

1. See [:material-code-braces: CompositionRelationshipItemTypeDef](./type_defs.md#compositionrelationshipitemtypedef) 
## ListCompositionRelationshipsResponseTypeDef

```python
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
# ConfigurationStatusTypeDef definition

class ConfigurationStatusTypeDef(TypedDict):
    state: ConfigurationStateType,  # (1)
    error: NotRequired[ConfigurationErrorDetailsTypeDef],  # (2)
```

1. See [:material-code-brackets: ConfigurationStateType](./literals.md#configurationstatetype) 
2. See [:material-code-braces: ConfigurationErrorDetailsTypeDef](./type_defs.md#configurationerrordetailstypedef) 
## FileFormatOutputTypeDef

```python
# FileFormatOutputTypeDef definition

class FileFormatOutputTypeDef(TypedDict):
    csv: NotRequired[CsvOutputTypeDef],  # (1)
    parquet: NotRequired[Dict[str, Any]],
```

1. See [:material-code-braces: CsvOutputTypeDef](./type_defs.md#csvoutputtypedef) 
## MultiLayerStorageTypeDef

```python
# MultiLayerStorageTypeDef definition

class MultiLayerStorageTypeDef(TypedDict):
    customerManagedS3Storage: CustomerManagedS3StorageTypeDef,  # (1)
```

1. See [:material-code-braces: CustomerManagedS3StorageTypeDef](./type_defs.md#customermanageds3storagetypedef) 
## ListDashboardsResponseTypeDef

```python
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
# RowPaginatorTypeDef definition

class RowPaginatorTypeDef(TypedDict):
    data: List[DatumPaginatorTypeDef],  # (1)
```

1. See [:material-code-braces: DatumPaginatorTypeDef](./type_defs.md#datumpaginatortypedef) 
## RowTypeDef

```python
# RowTypeDef definition

class RowTypeDef(TypedDict):
    data: List[DatumTypeDef],  # (1)
```

1. See [:material-code-braces: DatumTypeDef](./type_defs.md#datumtypedef) 
## DescribeAssetModelRequestAssetModelActiveWaitTypeDef

```python
# DescribeAssetModelRequestAssetModelActiveWaitTypeDef definition

class DescribeAssetModelRequestAssetModelActiveWaitTypeDef(TypedDict):
    assetModelId: str,
    excludeProperties: NotRequired[bool],
    assetModelVersion: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeAssetModelRequestAssetModelNotExistsWaitTypeDef

```python
# DescribeAssetModelRequestAssetModelNotExistsWaitTypeDef definition

class DescribeAssetModelRequestAssetModelNotExistsWaitTypeDef(TypedDict):
    assetModelId: str,
    excludeProperties: NotRequired[bool],
    assetModelVersion: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeAssetRequestAssetActiveWaitTypeDef

```python
# DescribeAssetRequestAssetActiveWaitTypeDef definition

class DescribeAssetRequestAssetActiveWaitTypeDef(TypedDict):
    assetId: str,
    excludeProperties: NotRequired[bool],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeAssetRequestAssetNotExistsWaitTypeDef

```python
# DescribeAssetRequestAssetNotExistsWaitTypeDef definition

class DescribeAssetRequestAssetNotExistsWaitTypeDef(TypedDict):
    assetId: str,
    excludeProperties: NotRequired[bool],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribePortalRequestPortalActiveWaitTypeDef

```python
# DescribePortalRequestPortalActiveWaitTypeDef definition

class DescribePortalRequestPortalActiveWaitTypeDef(TypedDict):
    portalId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribePortalRequestPortalNotExistsWaitTypeDef

```python
# DescribePortalRequestPortalNotExistsWaitTypeDef definition

class DescribePortalRequestPortalNotExistsWaitTypeDef(TypedDict):
    portalId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeLoggingOptionsResponseTypeDef

```python
# DescribeLoggingOptionsResponseTypeDef definition

class DescribeLoggingOptionsResponseTypeDef(TypedDict):
    loggingOptions: LoggingOptionsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoggingOptionsTypeDef](./type_defs.md#loggingoptionstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutLoggingOptionsRequestRequestTypeDef

```python
# PutLoggingOptionsRequestRequestTypeDef definition

class PutLoggingOptionsRequestRequestTypeDef(TypedDict):
    loggingOptions: LoggingOptionsTypeDef,  # (1)
```

1. See [:material-code-braces: LoggingOptionsTypeDef](./type_defs.md#loggingoptionstypedef) 
## ErrorDetailsTypeDef

```python
# ErrorDetailsTypeDef definition

class ErrorDetailsTypeDef(TypedDict):
    code: ErrorCodeType,  # (1)
    message: str,
    details: NotRequired[List[DetailedErrorTypeDef]],  # (2)
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
2. See [:material-code-braces: DetailedErrorTypeDef](./type_defs.md#detailederrortypedef) 
## ExecuteQueryRequestExecuteQueryPaginateTypeDef

```python
# ExecuteQueryRequestExecuteQueryPaginateTypeDef definition

class ExecuteQueryRequestExecuteQueryPaginateTypeDef(TypedDict):
    queryStatement: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef

```python
# GetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef definition

class GetAssetPropertyAggregatesRequestGetAssetPropertyAggregatesPaginateTypeDef(TypedDict):
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
## GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef

```python
# GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef definition

class GetAssetPropertyValueHistoryRequestGetAssetPropertyValueHistoryPaginateTypeDef(TypedDict):
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
## GetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef

```python
# GetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef definition

class GetInterpolatedAssetPropertyValuesRequestGetInterpolatedAssetPropertyValuesPaginateTypeDef(TypedDict):
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
## ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef

```python
# ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef definition

class ListAccessPoliciesRequestListAccessPoliciesPaginateTypeDef(TypedDict):
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
## ListActionsRequestListActionsPaginateTypeDef

```python
# ListActionsRequestListActionsPaginateTypeDef definition

class ListActionsRequestListActionsPaginateTypeDef(TypedDict):
    targetResourceType: TargetResourceTypeType,  # (1)
    targetResourceId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: TargetResourceTypeType](./literals.md#targetresourcetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssetModelCompositeModelsRequestListAssetModelCompositeModelsPaginateTypeDef

```python
# ListAssetModelCompositeModelsRequestListAssetModelCompositeModelsPaginateTypeDef definition

class ListAssetModelCompositeModelsRequestListAssetModelCompositeModelsPaginateTypeDef(TypedDict):
    assetModelId: str,
    assetModelVersion: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef

```python
# ListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef definition

class ListAssetModelPropertiesRequestListAssetModelPropertiesPaginateTypeDef(TypedDict):
    assetModelId: str,
    filter: NotRequired[ListAssetModelPropertiesFilterType],  # (1)
    assetModelVersion: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ListAssetModelPropertiesFilterType](./literals.md#listassetmodelpropertiesfiltertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssetModelsRequestListAssetModelsPaginateTypeDef

```python
# ListAssetModelsRequestListAssetModelsPaginateTypeDef definition

class ListAssetModelsRequestListAssetModelsPaginateTypeDef(TypedDict):
    assetModelTypes: NotRequired[Sequence[AssetModelTypeType]],  # (1)
    assetModelVersion: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: AssetModelTypeType](./literals.md#assetmodeltypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef

```python
# ListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef definition

class ListAssetPropertiesRequestListAssetPropertiesPaginateTypeDef(TypedDict):
    assetId: str,
    filter: NotRequired[ListAssetPropertiesFilterType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ListAssetPropertiesFilterType](./literals.md#listassetpropertiesfiltertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef

```python
# ListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef definition

class ListAssetRelationshipsRequestListAssetRelationshipsPaginateTypeDef(TypedDict):
    assetId: str,
    traversalType: TraversalTypeType,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: TraversalTypeType](./literals.md#traversaltypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssetsRequestListAssetsPaginateTypeDef

```python
# ListAssetsRequestListAssetsPaginateTypeDef definition

class ListAssetsRequestListAssetsPaginateTypeDef(TypedDict):
    assetModelId: NotRequired[str],
    filter: NotRequired[ListAssetsFilterType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ListAssetsFilterType](./literals.md#listassetsfiltertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef

```python
# ListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef definition

class ListAssociatedAssetsRequestListAssociatedAssetsPaginateTypeDef(TypedDict):
    assetId: str,
    hierarchyId: NotRequired[str],
    traversalDirection: NotRequired[TraversalDirectionType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: TraversalDirectionType](./literals.md#traversaldirectiontype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBulkImportJobsRequestListBulkImportJobsPaginateTypeDef

```python
# ListBulkImportJobsRequestListBulkImportJobsPaginateTypeDef definition

class ListBulkImportJobsRequestListBulkImportJobsPaginateTypeDef(TypedDict):
    filter: NotRequired[ListBulkImportJobsFilterType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ListBulkImportJobsFilterType](./literals.md#listbulkimportjobsfiltertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCompositionRelationshipsRequestListCompositionRelationshipsPaginateTypeDef

```python
# ListCompositionRelationshipsRequestListCompositionRelationshipsPaginateTypeDef definition

class ListCompositionRelationshipsRequestListCompositionRelationshipsPaginateTypeDef(TypedDict):
    assetModelId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDashboardsRequestListDashboardsPaginateTypeDef

```python
# ListDashboardsRequestListDashboardsPaginateTypeDef definition

class ListDashboardsRequestListDashboardsPaginateTypeDef(TypedDict):
    projectId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGatewaysRequestListGatewaysPaginateTypeDef

```python
# ListGatewaysRequestListGatewaysPaginateTypeDef definition

class ListGatewaysRequestListGatewaysPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPortalsRequestListPortalsPaginateTypeDef

```python
# ListPortalsRequestListPortalsPaginateTypeDef definition

class ListPortalsRequestListPortalsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProjectAssetsRequestListProjectAssetsPaginateTypeDef

```python
# ListProjectAssetsRequestListProjectAssetsPaginateTypeDef definition

class ListProjectAssetsRequestListProjectAssetsPaginateTypeDef(TypedDict):
    projectId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProjectsRequestListProjectsPaginateTypeDef

```python
# ListProjectsRequestListProjectsPaginateTypeDef definition

class ListProjectsRequestListProjectsPaginateTypeDef(TypedDict):
    portalId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTimeSeriesRequestListTimeSeriesPaginateTypeDef

```python
# ListTimeSeriesRequestListTimeSeriesPaginateTypeDef definition

class ListTimeSeriesRequestListTimeSeriesPaginateTypeDef(TypedDict):
    assetId: NotRequired[str],
    aliasPrefix: NotRequired[str],
    timeSeriesType: NotRequired[ListTimeSeriesTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ListTimeSeriesTypeType](./literals.md#listtimeseriestypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## MeasurementProcessingConfigTypeDef

```python
# MeasurementProcessingConfigTypeDef definition

class MeasurementProcessingConfigTypeDef(TypedDict):
    forwardingConfig: ForwardingConfigTypeDef,  # (1)
```

1. See [:material-code-braces: ForwardingConfigTypeDef](./type_defs.md#forwardingconfigtypedef) 
## TransformProcessingConfigTypeDef

```python
# TransformProcessingConfigTypeDef definition

class TransformProcessingConfigTypeDef(TypedDict):
    computeLocation: ComputeLocationType,  # (1)
    forwardingConfig: NotRequired[ForwardingConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ComputeLocationType](./literals.md#computelocationtype) 
2. See [:material-code-braces: ForwardingConfigTypeDef](./type_defs.md#forwardingconfigtypedef) 
## GatewayPlatformTypeDef

```python
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
# ListBulkImportJobsResponseTypeDef definition

class ListBulkImportJobsResponseTypeDef(TypedDict):
    jobSummaries: List[JobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: JobSummaryTypeDef](./type_defs.md#jobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProjectsResponseTypeDef

```python
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
# ListTimeSeriesResponseTypeDef definition

class ListTimeSeriesResponseTypeDef(TypedDict):
    TimeSeriesSummaries: List[TimeSeriesSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TimeSeriesSummaryTypeDef](./type_defs.md#timeseriessummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MetricWindowTypeDef

```python
# MetricWindowTypeDef definition

class MetricWindowTypeDef(TypedDict):
    tumbling: NotRequired[TumblingWindowTypeDef],  # (1)
```

1. See [:material-code-braces: TumblingWindowTypeDef](./type_defs.md#tumblingwindowtypedef) 
## PortalStatusTypeDef

```python
# PortalStatusTypeDef definition

class PortalStatusTypeDef(TypedDict):
    state: PortalStateType,  # (1)
    error: NotRequired[MonitorErrorDetailsTypeDef],  # (2)
```

1. See [:material-code-brackets: PortalStateType](./literals.md#portalstatetype) 
2. See [:material-code-braces: MonitorErrorDetailsTypeDef](./type_defs.md#monitorerrordetailstypedef) 
## ResourceTypeDef

```python
# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    portal: NotRequired[PortalResourceTypeDef],  # (1)
    project: NotRequired[ProjectResourceTypeDef],  # (2)
```

1. See [:material-code-braces: PortalResourceTypeDef](./type_defs.md#portalresourcetypedef) 
2. See [:material-code-braces: ProjectResourceTypeDef](./type_defs.md#projectresourcetypedef) 
## ListActionsResponseTypeDef

```python
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
# BatchGetAssetPropertyAggregatesSuccessEntryTypeDef definition

class BatchGetAssetPropertyAggregatesSuccessEntryTypeDef(TypedDict):
    entryId: str,
    aggregatedValues: List[AggregatedValueTypeDef],  # (1)
```

1. See [:material-code-braces: AggregatedValueTypeDef](./type_defs.md#aggregatedvaluetypedef) 
## GetAssetPropertyAggregatesResponseTypeDef

```python
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
# ExpressionVariableOutputTypeDef definition

class ExpressionVariableOutputTypeDef(TypedDict):
    name: str,
    value: VariableValueOutputTypeDef,  # (1)
```

1. See [:material-code-braces: VariableValueOutputTypeDef](./type_defs.md#variablevalueoutputtypedef) 
## ListAssetPropertiesResponseTypeDef

```python
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
# BatchPutAssetPropertyErrorEntryTypeDef definition

class BatchPutAssetPropertyErrorEntryTypeDef(TypedDict):
    entryId: str,
    errors: List[BatchPutAssetPropertyErrorTypeDef],  # (1)
```

1. See [:material-code-braces: BatchPutAssetPropertyErrorTypeDef](./type_defs.md#batchputassetpropertyerrortypedef) 
## BatchGetAssetPropertyValueHistorySuccessEntryTypeDef

```python
# BatchGetAssetPropertyValueHistorySuccessEntryTypeDef definition

class BatchGetAssetPropertyValueHistorySuccessEntryTypeDef(TypedDict):
    entryId: str,
    assetPropertyValueHistory: List[AssetPropertyValueTypeDef],  # (1)
```

1. See [:material-code-braces: AssetPropertyValueTypeDef](./type_defs.md#assetpropertyvaluetypedef) 
## BatchGetAssetPropertyValueSuccessEntryTypeDef

```python
# BatchGetAssetPropertyValueSuccessEntryTypeDef definition

class BatchGetAssetPropertyValueSuccessEntryTypeDef(TypedDict):
    entryId: str,
    assetPropertyValue: NotRequired[AssetPropertyValueTypeDef],  # (1)
```

1. See [:material-code-braces: AssetPropertyValueTypeDef](./type_defs.md#assetpropertyvaluetypedef) 
## GetAssetPropertyValueHistoryResponseTypeDef

```python
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
# GetAssetPropertyValueResponseTypeDef definition

class GetAssetPropertyValueResponseTypeDef(TypedDict):
    propertyValue: AssetPropertyValueTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssetPropertyValueTypeDef](./type_defs.md#assetpropertyvaluetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutAssetPropertyValueEntryTypeDef

```python
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
# GetInterpolatedAssetPropertyValuesResponseTypeDef definition

class GetInterpolatedAssetPropertyValuesResponseTypeDef(TypedDict):
    interpolatedAssetPropertyValues: List[InterpolatedAssetPropertyValueTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: InterpolatedAssetPropertyValueTypeDef](./type_defs.md#interpolatedassetpropertyvaluetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetAssetPropertyAggregatesRequestRequestTypeDef

```python
# BatchGetAssetPropertyAggregatesRequestRequestTypeDef definition

class BatchGetAssetPropertyAggregatesRequestRequestTypeDef(TypedDict):
    entries: Sequence[BatchGetAssetPropertyAggregatesEntryTypeDef],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: BatchGetAssetPropertyAggregatesEntryTypeDef](./type_defs.md#batchgetassetpropertyaggregatesentrytypedef) 
## BatchGetAssetPropertyValueHistoryRequestRequestTypeDef

```python
# BatchGetAssetPropertyValueHistoryRequestRequestTypeDef definition

class BatchGetAssetPropertyValueHistoryRequestRequestTypeDef(TypedDict):
    entries: Sequence[BatchGetAssetPropertyValueHistoryEntryTypeDef],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: BatchGetAssetPropertyValueHistoryEntryTypeDef](./type_defs.md#batchgetassetpropertyvaluehistoryentrytypedef) 
## CreatePortalRequestRequestTypeDef

```python
# CreatePortalRequestRequestTypeDef definition

class CreatePortalRequestRequestTypeDef(TypedDict):
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
```

1. See [:material-code-braces: ImageFileTypeDef](./type_defs.md#imagefiletypedef) 
2. See [:material-code-brackets: AuthModeType](./literals.md#authmodetype) 
3. See [:material-code-braces: AlarmsTypeDef](./type_defs.md#alarmstypedef) 
## ImageTypeDef

```python
# ImageTypeDef definition

class ImageTypeDef(TypedDict):
    id: NotRequired[str],
    file: NotRequired[ImageFileTypeDef],  # (1)
```

1. See [:material-code-braces: ImageFileTypeDef](./type_defs.md#imagefiletypedef) 
## DescribeDefaultEncryptionConfigurationResponseTypeDef

```python
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
# JobConfigurationOutputTypeDef definition

class JobConfigurationOutputTypeDef(TypedDict):
    fileFormat: FileFormatOutputTypeDef,  # (1)
```

1. See [:material-code-braces: FileFormatOutputTypeDef](./type_defs.md#fileformatoutputtypedef) 
## FileFormatTypeDef

```python
# FileFormatTypeDef definition

class FileFormatTypeDef(TypedDict):
    csv: NotRequired[CsvUnionTypeDef],  # (1)
    parquet: NotRequired[Mapping[str, Any]],
```

1. See [:material-code-braces: CsvTypeDef](./type_defs.md#csvtypedef) [:material-code-braces: CsvOutputTypeDef](./type_defs.md#csvoutputtypedef) 
## DescribeStorageConfigurationResponseTypeDef

```python
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
## PutStorageConfigurationRequestRequestTypeDef

```python
# PutStorageConfigurationRequestRequestTypeDef definition

class PutStorageConfigurationRequestRequestTypeDef(TypedDict):
    storageType: StorageTypeType,  # (1)
    multiLayerStorage: NotRequired[MultiLayerStorageTypeDef],  # (2)
    disassociatedDataStorage: NotRequired[DisassociatedDataStorageStateType],  # (3)
    retentionPeriod: NotRequired[RetentionPeriodTypeDef],  # (4)
    warmTier: NotRequired[WarmTierStateType],  # (5)
    warmTierRetentionPeriod: NotRequired[WarmTierRetentionPeriodTypeDef],  # (6)
```

1. See [:material-code-brackets: StorageTypeType](./literals.md#storagetypetype) 
2. See [:material-code-braces: MultiLayerStorageTypeDef](./type_defs.md#multilayerstoragetypedef) 
3. See [:material-code-brackets: DisassociatedDataStorageStateType](./literals.md#disassociateddatastoragestatetype) 
4. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
5. See [:material-code-brackets: WarmTierStateType](./literals.md#warmtierstatetype) 
6. See [:material-code-braces: WarmTierRetentionPeriodTypeDef](./type_defs.md#warmtierretentionperiodtypedef) 
## PutStorageConfigurationResponseTypeDef

```python
# PutStorageConfigurationResponseTypeDef definition

class PutStorageConfigurationResponseTypeDef(TypedDict):
    storageType: StorageTypeType,  # (1)
    multiLayerStorage: MultiLayerStorageTypeDef,  # (2)
    disassociatedDataStorage: DisassociatedDataStorageStateType,  # (3)
    retentionPeriod: RetentionPeriodTypeDef,  # (4)
    configurationStatus: ConfigurationStatusTypeDef,  # (5)
    warmTier: WarmTierStateType,  # (6)
    warmTierRetentionPeriod: WarmTierRetentionPeriodTypeDef,  # (7)
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
## AssetModelStatusTypeDef

```python
# AssetModelStatusTypeDef definition

class AssetModelStatusTypeDef(TypedDict):
    state: AssetModelStateType,  # (1)
    error: NotRequired[ErrorDetailsTypeDef],  # (2)
```

1. See [:material-code-brackets: AssetModelStateType](./literals.md#assetmodelstatetype) 
2. See [:material-code-braces: ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef) 
## AssetStatusTypeDef

```python
# AssetStatusTypeDef definition

class AssetStatusTypeDef(TypedDict):
    state: AssetStateType,  # (1)
    error: NotRequired[ErrorDetailsTypeDef],  # (2)
```

1. See [:material-code-brackets: AssetStateType](./literals.md#assetstatetype) 
2. See [:material-code-braces: ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef) 
## MeasurementTypeDef

```python
# MeasurementTypeDef definition

class MeasurementTypeDef(TypedDict):
    processingConfig: NotRequired[MeasurementProcessingConfigTypeDef],  # (1)
```

1. See [:material-code-braces: MeasurementProcessingConfigTypeDef](./type_defs.md#measurementprocessingconfigtypedef) 
## CreateGatewayRequestRequestTypeDef

```python
# CreateGatewayRequestRequestTypeDef definition

class CreateGatewayRequestRequestTypeDef(TypedDict):
    gatewayName: str,
    gatewayPlatform: GatewayPlatformTypeDef,  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: GatewayPlatformTypeDef](./type_defs.md#gatewayplatformtypedef) 
## DescribeGatewayResponseTypeDef

```python
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
## CreatePortalResponseTypeDef

```python
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
# DeletePortalResponseTypeDef definition

class DeletePortalResponseTypeDef(TypedDict):
    portalStatus: PortalStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PortalStatusTypeDef](./type_defs.md#portalstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePortalResponseTypeDef

```python
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
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: PortalStatusTypeDef](./type_defs.md#portalstatustypedef) 
2. See [:material-code-braces: ImageLocationTypeDef](./type_defs.md#imagelocationtypedef) 
3. See [:material-code-brackets: AuthModeType](./literals.md#authmodetype) 
4. See [:material-code-braces: AlarmsTypeDef](./type_defs.md#alarmstypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PortalSummaryTypeDef

```python
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
```

1. See [:material-code-braces: PortalStatusTypeDef](./type_defs.md#portalstatustypedef) 
## UpdatePortalResponseTypeDef

```python
# UpdatePortalResponseTypeDef definition

class UpdatePortalResponseTypeDef(TypedDict):
    portalStatus: PortalStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PortalStatusTypeDef](./type_defs.md#portalstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AccessPolicySummaryTypeDef

```python
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
## CreateAccessPolicyRequestRequestTypeDef

```python
# CreateAccessPolicyRequestRequestTypeDef definition

class CreateAccessPolicyRequestRequestTypeDef(TypedDict):
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
## UpdateAccessPolicyRequestRequestTypeDef

```python
# UpdateAccessPolicyRequestRequestTypeDef definition

class UpdateAccessPolicyRequestRequestTypeDef(TypedDict):
    accessPolicyId: str,
    accessPolicyIdentity: IdentityTypeDef,  # (1)
    accessPolicyResource: ResourceTypeDef,  # (2)
    accessPolicyPermission: PermissionType,  # (3)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
2. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
3. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
## BatchGetAssetPropertyAggregatesResponseTypeDef

```python
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
# ExpressionVariableTypeDef definition

class ExpressionVariableTypeDef(TypedDict):
    name: str,
    value: VariableValueUnionTypeDef,  # (1)
```

1. See [:material-code-braces: VariableValueTypeDef](./type_defs.md#variablevaluetypedef) [:material-code-braces: VariableValueOutputTypeDef](./type_defs.md#variablevalueoutputtypedef) 
## BatchPutAssetPropertyValueResponseTypeDef

```python
# BatchPutAssetPropertyValueResponseTypeDef definition

class BatchPutAssetPropertyValueResponseTypeDef(TypedDict):
    errorEntries: List[BatchPutAssetPropertyErrorEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchPutAssetPropertyErrorEntryTypeDef](./type_defs.md#batchputassetpropertyerrorentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetAssetPropertyValueHistoryResponseTypeDef

```python
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
## BatchPutAssetPropertyValueRequestRequestTypeDef

```python
# BatchPutAssetPropertyValueRequestRequestTypeDef definition

class BatchPutAssetPropertyValueRequestRequestTypeDef(TypedDict):
    entries: Sequence[PutAssetPropertyValueEntryTypeDef],  # (1)
```

1. See [:material-code-braces: PutAssetPropertyValueEntryTypeDef](./type_defs.md#putassetpropertyvalueentrytypedef) 
## UpdatePortalRequestRequestTypeDef

```python
# UpdatePortalRequestRequestTypeDef definition

class UpdatePortalRequestRequestTypeDef(TypedDict):
    portalId: str,
    portalName: str,
    portalContactEmail: str,
    roleArn: str,
    portalDescription: NotRequired[str],
    portalLogoImage: NotRequired[ImageTypeDef],  # (1)
    clientToken: NotRequired[str],
    notificationSenderEmail: NotRequired[str],
    alarms: NotRequired[AlarmsTypeDef],  # (2)
```

1. See [:material-code-braces: ImageTypeDef](./type_defs.md#imagetypedef) 
2. See [:material-code-braces: AlarmsTypeDef](./type_defs.md#alarmstypedef) 
## DescribeBulkImportJobResponseTypeDef

```python
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
# DeleteAssetModelCompositeModelResponseTypeDef definition

class DeleteAssetModelCompositeModelResponseTypeDef(TypedDict):
    assetModelStatus: AssetModelStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssetModelStatusTypeDef](./type_defs.md#assetmodelstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAssetModelResponseTypeDef

```python
# DeleteAssetModelResponseTypeDef definition

class DeleteAssetModelResponseTypeDef(TypedDict):
    assetModelStatus: AssetModelStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssetModelStatusTypeDef](./type_defs.md#assetmodelstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAssetModelCompositeModelResponseTypeDef

```python
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
# UpdateAssetModelResponseTypeDef definition

class UpdateAssetModelResponseTypeDef(TypedDict):
    assetModelStatus: AssetModelStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssetModelStatusTypeDef](./type_defs.md#assetmodelstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssetSummaryTypeDef

```python
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
# DeleteAssetResponseTypeDef definition

class DeleteAssetResponseTypeDef(TypedDict):
    assetStatus: AssetStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssetStatusTypeDef](./type_defs.md#assetstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAssetResponseTypeDef

```python
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
# UpdateAssetResponseTypeDef definition

class UpdateAssetResponseTypeDef(TypedDict):
    assetStatus: AssetStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssetStatusTypeDef](./type_defs.md#assetstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGatewaysResponseTypeDef

```python
# ListGatewaysResponseTypeDef definition

class ListGatewaysResponseTypeDef(TypedDict):
    gatewaySummaries: List[GatewaySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: GatewaySummaryTypeDef](./type_defs.md#gatewaysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPortalsResponseTypeDef

```python
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
# ListAccessPoliciesResponseTypeDef definition

class ListAccessPoliciesResponseTypeDef(TypedDict):
    accessPolicySummaries: List[AccessPolicySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AccessPolicySummaryTypeDef](./type_defs.md#accesspolicysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PropertyTypeOutputTypeDef

```python
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
## JobConfigurationTypeDef

```python
# JobConfigurationTypeDef definition

class JobConfigurationTypeDef(TypedDict):
    fileFormat: FileFormatUnionTypeDef,  # (1)
```

1. See [:material-code-braces: FileFormatTypeDef](./type_defs.md#fileformattypedef) [:material-code-braces: FileFormatOutputTypeDef](./type_defs.md#fileformatoutputtypedef) 
## ListAssetModelsResponseTypeDef

```python
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
# ListAssociatedAssetsResponseTypeDef definition

class ListAssociatedAssetsResponseTypeDef(TypedDict):
    assetSummaries: List[AssociatedAssetsSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AssociatedAssetsSummaryTypeDef](./type_defs.md#associatedassetssummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssetModelPropertyOutputTypeDef

```python
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
# TransformTypeDef definition

class TransformTypeDef(TypedDict):
    expression: str,
    variables: Sequence[ExpressionVariableUnionTypeDef],  # (1)
    processingConfig: NotRequired[TransformProcessingConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ExpressionVariableTypeDef](./type_defs.md#expressionvariabletypedef) [:material-code-braces: ExpressionVariableOutputTypeDef](./type_defs.md#expressionvariableoutputtypedef) 
2. See [:material-code-braces: TransformProcessingConfigTypeDef](./type_defs.md#transformprocessingconfigtypedef) 
## CreateBulkImportJobRequestRequestTypeDef

```python
# CreateBulkImportJobRequestRequestTypeDef definition

class CreateBulkImportJobRequestRequestTypeDef(TypedDict):
    jobName: str,
    jobRoleArn: str,
    files: Sequence[FileTypeDef],  # (1)
    errorReportLocation: ErrorReportLocationTypeDef,  # (2)
    jobConfiguration: JobConfigurationTypeDef,  # (3)
    adaptiveIngestion: NotRequired[bool],
    deleteFilesAfterImport: NotRequired[bool],
```

1. See [:material-code-braces: FileTypeDef](./type_defs.md#filetypedef) 
2. See [:material-code-braces: ErrorReportLocationTypeDef](./type_defs.md#errorreportlocationtypedef) 
3. See [:material-code-braces: JobConfigurationTypeDef](./type_defs.md#jobconfigurationtypedef) 
## AssetModelCompositeModelOutputTypeDef

```python
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
# CompositeModelPropertyTypeDef definition

class CompositeModelPropertyTypeDef(TypedDict):
    name: str,
    type: str,
    assetProperty: PropertyTypeDef,  # (1)
    id: NotRequired[str],
    externalId: NotRequired[str],
```

1. See [:material-code-braces: PropertyTypeDef](./type_defs.md#propertytypedef) 
## DescribeAssetModelResponseTypeDef

```python
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
## AssetModelPropertyDefinitionTypeDef

```python
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
## CreateAssetModelCompositeModelRequestRequestTypeDef

```python
# CreateAssetModelCompositeModelRequestRequestTypeDef definition

class CreateAssetModelCompositeModelRequestRequestTypeDef(TypedDict):
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
## UpdateAssetModelCompositeModelRequestRequestTypeDef

```python
# UpdateAssetModelCompositeModelRequestRequestTypeDef definition

class UpdateAssetModelCompositeModelRequestRequestTypeDef(TypedDict):
    assetModelId: str,
    assetModelCompositeModelId: str,
    assetModelCompositeModelName: str,
    assetModelCompositeModelExternalId: NotRequired[str],
    assetModelCompositeModelDescription: NotRequired[str],
    clientToken: NotRequired[str],
    assetModelCompositeModelProperties: NotRequired[Sequence[AssetModelPropertyTypeDef]],  # (1)
    ifMatch: NotRequired[str],
    ifNoneMatch: NotRequired[str],
    matchForVersionType: NotRequired[AssetModelVersionTypeType],  # (2)
```

1. See [:material-code-braces: AssetModelPropertyTypeDef](./type_defs.md#assetmodelpropertytypedef) 
2. See [:material-code-brackets: AssetModelVersionTypeType](./literals.md#assetmodelversiontypetype) 
## CreateAssetModelRequestRequestTypeDef

```python
# CreateAssetModelRequestRequestTypeDef definition

class CreateAssetModelRequestRequestTypeDef(TypedDict):
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
## UpdateAssetModelRequestRequestTypeDef

```python
# UpdateAssetModelRequestRequestTypeDef definition

class UpdateAssetModelRequestRequestTypeDef(TypedDict):
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
