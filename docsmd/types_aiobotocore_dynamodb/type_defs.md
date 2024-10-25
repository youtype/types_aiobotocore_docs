# Type definitions

> [Index](../README.md) > [DynamoDB](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [DynamoDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
    type annotations stubs module [types-aiobotocore-dynamodb](https://pypi.org/project/types-aiobotocore-dynamodb/).

## TableAttributeValueTypeDef

```python
# TableAttributeValueTypeDef definition

TableAttributeValueTypeDef = Union[
    bytes,
    bytearray,
    str,
    int,
    Decimal,
    bool,
    Set[int],
    Set[Decimal],
    Set[str],
    Set[bytes],
    Set[bytearray],
    Sequence[Any],
    Mapping[str, Any],
    None,
]
```


## ConditionBaseImportTypeDef

```python
# ConditionBaseImportTypeDef definition

ConditionBaseImportTypeDef = Union[
    str,
    ConditionBase,
]
```


## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## UniversalAttributeValueTypeDef

```python
# UniversalAttributeValueTypeDef definition

UniversalAttributeValueTypeDef = Union[
    AttributeValueTypeDef,  # (1)
    bytes,
    bytearray,
    str,
    int,
    Decimal,
    bool,
    Set[int],
    Set[Decimal],
    Set[str],
    Set[bytes],
    Set[bytearray],
    Sequence[Any],
    Mapping[str, Any],
    None,
]
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 

## CsvOptionsUnionTypeDef

```python
# CsvOptionsUnionTypeDef definition

CsvOptionsUnionTypeDef = Union[
    CsvOptionsTypeDef,  # (1)
    CsvOptionsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CsvOptionsTypeDef](./type_defs.md#csvoptionstypedef) 
2. See [:material-code-braces: CsvOptionsOutputTypeDef](./type_defs.md#csvoptionsoutputtypedef) 

## ProjectionUnionTypeDef

```python
# ProjectionUnionTypeDef definition

ProjectionUnionTypeDef = Union[
    ProjectionTypeDef,  # (1)
    ProjectionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ProjectionTypeDef](./type_defs.md#projectiontypedef) 
2. See [:material-code-braces: ProjectionOutputTypeDef](./type_defs.md#projectionoutputtypedef) 

## DeleteRequestServiceResourceUnionTypeDef

```python
# DeleteRequestServiceResourceUnionTypeDef definition

DeleteRequestServiceResourceUnionTypeDef = Union[
    DeleteRequestServiceResourceTypeDef,  # (1)
    DeleteRequestServiceResourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DeleteRequestServiceResourceTypeDef](./type_defs.md#deleterequestserviceresourcetypedef) 
2. See [:material-code-braces: DeleteRequestServiceResourceOutputTypeDef](./type_defs.md#deleterequestserviceresourceoutputtypedef) 

## KeysAndAttributesServiceResourceUnionTypeDef

```python
# KeysAndAttributesServiceResourceUnionTypeDef definition

KeysAndAttributesServiceResourceUnionTypeDef = Union[
    KeysAndAttributesServiceResourceTypeDef,  # (1)
    KeysAndAttributesServiceResourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: KeysAndAttributesServiceResourceTypeDef](./type_defs.md#keysandattributesserviceresourcetypedef) 
2. See [:material-code-braces: KeysAndAttributesServiceResourceOutputTypeDef](./type_defs.md#keysandattributesserviceresourceoutputtypedef) 

## PutRequestServiceResourceUnionTypeDef

```python
# PutRequestServiceResourceUnionTypeDef definition

PutRequestServiceResourceUnionTypeDef = Union[
    PutRequestServiceResourceTypeDef,  # (1)
    PutRequestServiceResourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PutRequestServiceResourceTypeDef](./type_defs.md#putrequestserviceresourcetypedef) 
2. See [:material-code-braces: PutRequestServiceResourceOutputTypeDef](./type_defs.md#putrequestserviceresourceoutputtypedef) 

## GlobalSecondaryIndexUnionTypeDef

```python
# GlobalSecondaryIndexUnionTypeDef definition

GlobalSecondaryIndexUnionTypeDef = Union[
    GlobalSecondaryIndexTypeDef,  # (1)
    GlobalSecondaryIndexOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: GlobalSecondaryIndexTypeDef](./type_defs.md#globalsecondaryindextypedef) 
2. See [:material-code-braces: GlobalSecondaryIndexOutputTypeDef](./type_defs.md#globalsecondaryindexoutputtypedef) 

## DeleteRequestUnionTypeDef

```python
# DeleteRequestUnionTypeDef definition

DeleteRequestUnionTypeDef = Union[
    DeleteRequestTypeDef,  # (1)
    DeleteRequestOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DeleteRequestTypeDef](./type_defs.md#deleterequesttypedef) 
2. See [:material-code-braces: DeleteRequestOutputTypeDef](./type_defs.md#deleterequestoutputtypedef) 

## KeysAndAttributesUnionTypeDef

```python
# KeysAndAttributesUnionTypeDef definition

KeysAndAttributesUnionTypeDef = Union[
    KeysAndAttributesTypeDef,  # (1)
    KeysAndAttributesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: KeysAndAttributesTypeDef](./type_defs.md#keysandattributestypedef) 
2. See [:material-code-braces: KeysAndAttributesOutputTypeDef](./type_defs.md#keysandattributesoutputtypedef) 

## PutRequestUnionTypeDef

```python
# PutRequestUnionTypeDef definition

PutRequestUnionTypeDef = Union[
    PutRequestTypeDef,  # (1)
    PutRequestOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PutRequestTypeDef](./type_defs.md#putrequesttypedef) 
2. See [:material-code-braces: PutRequestOutputTypeDef](./type_defs.md#putrequestoutputtypedef) 

## WriteRequestServiceResourceUnionTypeDef

```python
# WriteRequestServiceResourceUnionTypeDef definition

WriteRequestServiceResourceUnionTypeDef = Union[
    WriteRequestServiceResourceTypeDef,  # (1)
    WriteRequestServiceResourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: WriteRequestServiceResourceTypeDef](./type_defs.md#writerequestserviceresourcetypedef) 
2. See [:material-code-braces: WriteRequestServiceResourceOutputTypeDef](./type_defs.md#writerequestserviceresourceoutputtypedef) 

## WriteRequestUnionTypeDef

```python
# WriteRequestUnionTypeDef definition

WriteRequestUnionTypeDef = Union[
    WriteRequestTypeDef,  # (1)
    WriteRequestOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: WriteRequestTypeDef](./type_defs.md#writerequesttypedef) 
2. See [:material-code-braces: WriteRequestOutputTypeDef](./type_defs.md#writerequestoutputtypedef) 



## ArchivalSummaryTypeDef

```python
# ArchivalSummaryTypeDef definition

class ArchivalSummaryTypeDef(TypedDict):
    ArchivalDateTime: NotRequired[datetime],
    ArchivalReason: NotRequired[str],
    ArchivalBackupArn: NotRequired[str],
```

## AttributeDefinitionTypeDef

```python
# AttributeDefinitionTypeDef definition

class AttributeDefinitionTypeDef(TypedDict):
    AttributeName: str,
    AttributeType: ScalarAttributeTypeType,  # (1)
```

1. See [:material-code-brackets: ScalarAttributeTypeType](./literals.md#scalarattributetypetype) 
## AttributeValueTypeDef

```python
# AttributeValueTypeDef definition

class AttributeValueTypeDef(TypedDict):
    S: NotRequired[str],
    N: NotRequired[str],
    B: NotRequired[bytes],
    SS: NotRequired[Sequence[str]],
    NS: NotRequired[Sequence[str]],
    BS: NotRequired[Sequence[bytes]],
    M: NotRequired[Mapping[str, Any]],
    L: NotRequired[Sequence[Any]],
    NULL: NotRequired[bool],
    BOOL: NotRequired[bool],
```

## AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef

```python
# AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef definition

class AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef(TypedDict):
    TargetValue: float,
    DisableScaleIn: NotRequired[bool],
    ScaleInCooldown: NotRequired[int],
    ScaleOutCooldown: NotRequired[int],
```

## AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef

```python
# AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef definition

class AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef(TypedDict):
    TargetValue: float,
    DisableScaleIn: NotRequired[bool],
    ScaleInCooldown: NotRequired[int],
    ScaleOutCooldown: NotRequired[int],
```

## BackupDetailsTypeDef

```python
# BackupDetailsTypeDef definition

class BackupDetailsTypeDef(TypedDict):
    BackupArn: str,
    BackupName: str,
    BackupStatus: BackupStatusType,  # (1)
    BackupType: BackupTypeType,  # (2)
    BackupCreationDateTime: datetime,
    BackupSizeBytes: NotRequired[int],
    BackupExpiryDateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: BackupStatusType](./literals.md#backupstatustype) 
2. See [:material-code-brackets: BackupTypeType](./literals.md#backuptypetype) 
## BackupSummaryTypeDef

```python
# BackupSummaryTypeDef definition

class BackupSummaryTypeDef(TypedDict):
    TableName: NotRequired[str],
    TableId: NotRequired[str],
    TableArn: NotRequired[str],
    BackupArn: NotRequired[str],
    BackupName: NotRequired[str],
    BackupCreationDateTime: NotRequired[datetime],
    BackupExpiryDateTime: NotRequired[datetime],
    BackupStatus: NotRequired[BackupStatusType],  # (1)
    BackupType: NotRequired[BackupTypeType],  # (2)
    BackupSizeBytes: NotRequired[int],
```

1. See [:material-code-brackets: BackupStatusType](./literals.md#backupstatustype) 
2. See [:material-code-brackets: BackupTypeType](./literals.md#backuptypetype) 
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

## BillingModeSummaryTypeDef

```python
# BillingModeSummaryTypeDef definition

class BillingModeSummaryTypeDef(TypedDict):
    BillingMode: NotRequired[BillingModeType],  # (1)
    LastUpdateToPayPerRequestDateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
## CapacityTypeDef

```python
# CapacityTypeDef definition

class CapacityTypeDef(TypedDict):
    ReadCapacityUnits: NotRequired[float],
    WriteCapacityUnits: NotRequired[float],
    CapacityUnits: NotRequired[float],
```

## PointInTimeRecoveryDescriptionTypeDef

```python
# PointInTimeRecoveryDescriptionTypeDef definition

class PointInTimeRecoveryDescriptionTypeDef(TypedDict):
    PointInTimeRecoveryStatus: NotRequired[PointInTimeRecoveryStatusType],  # (1)
    EarliestRestorableDateTime: NotRequired[datetime],
    LatestRestorableDateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: PointInTimeRecoveryStatusType](./literals.md#pointintimerecoverystatustype) 
## ContributorInsightsSummaryTypeDef

```python
# ContributorInsightsSummaryTypeDef definition

class ContributorInsightsSummaryTypeDef(TypedDict):
    TableName: NotRequired[str],
    IndexName: NotRequired[str],
    ContributorInsightsStatus: NotRequired[ContributorInsightsStatusType],  # (1)
```

1. See [:material-code-brackets: ContributorInsightsStatusType](./literals.md#contributorinsightsstatustype) 
## CreateBackupInputRequestTypeDef

```python
# CreateBackupInputRequestTypeDef definition

class CreateBackupInputRequestTypeDef(TypedDict):
    TableName: str,
    BackupName: str,
```

## KeySchemaElementTypeDef

```python
# KeySchemaElementTypeDef definition

class KeySchemaElementTypeDef(TypedDict):
    AttributeName: str,
    KeyType: KeyTypeType,  # (1)
```

1. See [:material-code-brackets: KeyTypeType](./literals.md#keytypetype) 
## OnDemandThroughputTypeDef

```python
# OnDemandThroughputTypeDef definition

class OnDemandThroughputTypeDef(TypedDict):
    MaxReadRequestUnits: NotRequired[int],
    MaxWriteRequestUnits: NotRequired[int],
```

## ProvisionedThroughputTypeDef

```python
# ProvisionedThroughputTypeDef definition

class ProvisionedThroughputTypeDef(TypedDict):
    ReadCapacityUnits: int,
    WriteCapacityUnits: int,
```

## ReplicaTypeDef

```python
# ReplicaTypeDef definition

class ReplicaTypeDef(TypedDict):
    RegionName: NotRequired[str],
```

## CreateReplicaActionTypeDef

```python
# CreateReplicaActionTypeDef definition

class CreateReplicaActionTypeDef(TypedDict):
    RegionName: str,
```

## OnDemandThroughputOverrideTypeDef

```python
# OnDemandThroughputOverrideTypeDef definition

class OnDemandThroughputOverrideTypeDef(TypedDict):
    MaxReadRequestUnits: NotRequired[int],
```

## ProvisionedThroughputOverrideTypeDef

```python
# ProvisionedThroughputOverrideTypeDef definition

class ProvisionedThroughputOverrideTypeDef(TypedDict):
    ReadCapacityUnits: NotRequired[int],
```

## SSESpecificationTypeDef

```python
# SSESpecificationTypeDef definition

class SSESpecificationTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    SSEType: NotRequired[SSETypeType],  # (1)
    KMSMasterKeyId: NotRequired[str],
```

1. See [:material-code-brackets: SSETypeType](./literals.md#ssetypetype) 
## StreamSpecificationTypeDef

```python
# StreamSpecificationTypeDef definition

class StreamSpecificationTypeDef(TypedDict):
    StreamEnabled: bool,
    StreamViewType: NotRequired[StreamViewTypeType],  # (1)
```

1. See [:material-code-brackets: StreamViewTypeType](./literals.md#streamviewtypetype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## CsvOptionsOutputTypeDef

```python
# CsvOptionsOutputTypeDef definition

class CsvOptionsOutputTypeDef(TypedDict):
    Delimiter: NotRequired[str],
    HeaderList: NotRequired[List[str]],
```

## CsvOptionsTypeDef

```python
# CsvOptionsTypeDef definition

class CsvOptionsTypeDef(TypedDict):
    Delimiter: NotRequired[str],
    HeaderList: NotRequired[Sequence[str]],
```

## DeleteBackupInputRequestTypeDef

```python
# DeleteBackupInputRequestTypeDef definition

class DeleteBackupInputRequestTypeDef(TypedDict):
    BackupArn: str,
```

## DeleteGlobalSecondaryIndexActionTypeDef

```python
# DeleteGlobalSecondaryIndexActionTypeDef definition

class DeleteGlobalSecondaryIndexActionTypeDef(TypedDict):
    IndexName: str,
```

## DeleteReplicaActionTypeDef

```python
# DeleteReplicaActionTypeDef definition

class DeleteReplicaActionTypeDef(TypedDict):
    RegionName: str,
```

## DeleteReplicationGroupMemberActionTypeDef

```python
# DeleteReplicationGroupMemberActionTypeDef definition

class DeleteReplicationGroupMemberActionTypeDef(TypedDict):
    RegionName: str,
```

## DeleteResourcePolicyInputRequestTypeDef

```python
# DeleteResourcePolicyInputRequestTypeDef definition

class DeleteResourcePolicyInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    ExpectedRevisionId: NotRequired[str],
```

## DeleteTableInputRequestTypeDef

```python
# DeleteTableInputRequestTypeDef definition

class DeleteTableInputRequestTypeDef(TypedDict):
    TableName: str,
```

## DescribeBackupInputRequestTypeDef

```python
# DescribeBackupInputRequestTypeDef definition

class DescribeBackupInputRequestTypeDef(TypedDict):
    BackupArn: str,
```

## DescribeContinuousBackupsInputRequestTypeDef

```python
# DescribeContinuousBackupsInputRequestTypeDef definition

class DescribeContinuousBackupsInputRequestTypeDef(TypedDict):
    TableName: str,
```

## DescribeContributorInsightsInputRequestTypeDef

```python
# DescribeContributorInsightsInputRequestTypeDef definition

class DescribeContributorInsightsInputRequestTypeDef(TypedDict):
    TableName: str,
    IndexName: NotRequired[str],
```

## FailureExceptionTypeDef

```python
# FailureExceptionTypeDef definition

class FailureExceptionTypeDef(TypedDict):
    ExceptionName: NotRequired[str],
    ExceptionDescription: NotRequired[str],
```

## EndpointTypeDef

```python
# EndpointTypeDef definition

class EndpointTypeDef(TypedDict):
    Address: str,
    CachePeriodInMinutes: int,
```

## DescribeExportInputRequestTypeDef

```python
# DescribeExportInputRequestTypeDef definition

class DescribeExportInputRequestTypeDef(TypedDict):
    ExportArn: str,
```

## DescribeGlobalTableInputRequestTypeDef

```python
# DescribeGlobalTableInputRequestTypeDef definition

class DescribeGlobalTableInputRequestTypeDef(TypedDict):
    GlobalTableName: str,
```

## DescribeGlobalTableSettingsInputRequestTypeDef

```python
# DescribeGlobalTableSettingsInputRequestTypeDef definition

class DescribeGlobalTableSettingsInputRequestTypeDef(TypedDict):
    GlobalTableName: str,
```

## DescribeImportInputRequestTypeDef

```python
# DescribeImportInputRequestTypeDef definition

class DescribeImportInputRequestTypeDef(TypedDict):
    ImportArn: str,
```

## DescribeKinesisStreamingDestinationInputRequestTypeDef

```python
# DescribeKinesisStreamingDestinationInputRequestTypeDef definition

class DescribeKinesisStreamingDestinationInputRequestTypeDef(TypedDict):
    TableName: str,
```

## KinesisDataStreamDestinationTypeDef

```python
# KinesisDataStreamDestinationTypeDef definition

class KinesisDataStreamDestinationTypeDef(TypedDict):
    StreamArn: NotRequired[str],
    DestinationStatus: NotRequired[DestinationStatusType],  # (1)
    DestinationStatusDescription: NotRequired[str],
    ApproximateCreationDateTimePrecision: NotRequired[ApproximateCreationDateTimePrecisionType],  # (2)
```

1. See [:material-code-brackets: DestinationStatusType](./literals.md#destinationstatustype) 
2. See [:material-code-brackets: ApproximateCreationDateTimePrecisionType](./literals.md#approximatecreationdatetimeprecisiontype) 
## DescribeTableInputRequestTypeDef

```python
# DescribeTableInputRequestTypeDef definition

class DescribeTableInputRequestTypeDef(TypedDict):
    TableName: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeTableReplicaAutoScalingInputRequestTypeDef

```python
# DescribeTableReplicaAutoScalingInputRequestTypeDef definition

class DescribeTableReplicaAutoScalingInputRequestTypeDef(TypedDict):
    TableName: str,
```

## DescribeTimeToLiveInputRequestTypeDef

```python
# DescribeTimeToLiveInputRequestTypeDef definition

class DescribeTimeToLiveInputRequestTypeDef(TypedDict):
    TableName: str,
```

## TimeToLiveDescriptionTypeDef

```python
# TimeToLiveDescriptionTypeDef definition

class TimeToLiveDescriptionTypeDef(TypedDict):
    TimeToLiveStatus: NotRequired[TimeToLiveStatusType],  # (1)
    AttributeName: NotRequired[str],
```

1. See [:material-code-brackets: TimeToLiveStatusType](./literals.md#timetolivestatustype) 
## EnableKinesisStreamingConfigurationTypeDef

```python
# EnableKinesisStreamingConfigurationTypeDef definition

class EnableKinesisStreamingConfigurationTypeDef(TypedDict):
    ApproximateCreationDateTimePrecision: NotRequired[ApproximateCreationDateTimePrecisionType],  # (1)
```

1. See [:material-code-brackets: ApproximateCreationDateTimePrecisionType](./literals.md#approximatecreationdatetimeprecisiontype) 
## IncrementalExportSpecificationOutputTypeDef

```python
# IncrementalExportSpecificationOutputTypeDef definition

class IncrementalExportSpecificationOutputTypeDef(TypedDict):
    ExportFromTime: NotRequired[datetime],
    ExportToTime: NotRequired[datetime],
    ExportViewType: NotRequired[ExportViewTypeType],  # (1)
```

1. See [:material-code-brackets: ExportViewTypeType](./literals.md#exportviewtypetype) 
## ExportSummaryTypeDef

```python
# ExportSummaryTypeDef definition

class ExportSummaryTypeDef(TypedDict):
    ExportArn: NotRequired[str],
    ExportStatus: NotRequired[ExportStatusType],  # (1)
    ExportType: NotRequired[ExportTypeType],  # (2)
```

1. See [:material-code-brackets: ExportStatusType](./literals.md#exportstatustype) 
2. See [:material-code-brackets: ExportTypeType](./literals.md#exporttypetype) 
## GetResourcePolicyInputRequestTypeDef

```python
# GetResourcePolicyInputRequestTypeDef definition

class GetResourcePolicyInputRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ProjectionOutputTypeDef

```python
# ProjectionOutputTypeDef definition

class ProjectionOutputTypeDef(TypedDict):
    ProjectionType: NotRequired[ProjectionTypeType],  # (1)
    NonKeyAttributes: NotRequired[List[str]],
```

1. See [:material-code-brackets: ProjectionTypeType](./literals.md#projectiontypetype) 
## ProvisionedThroughputDescriptionTypeDef

```python
# ProvisionedThroughputDescriptionTypeDef definition

class ProvisionedThroughputDescriptionTypeDef(TypedDict):
    LastIncreaseDateTime: NotRequired[datetime],
    LastDecreaseDateTime: NotRequired[datetime],
    NumberOfDecreasesToday: NotRequired[int],
    ReadCapacityUnits: NotRequired[int],
    WriteCapacityUnits: NotRequired[int],
```

## ProjectionTypeDef

```python
# ProjectionTypeDef definition

class ProjectionTypeDef(TypedDict):
    ProjectionType: NotRequired[ProjectionTypeType],  # (1)
    NonKeyAttributes: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: ProjectionTypeType](./literals.md#projectiontypetype) 
## S3BucketSourceTypeDef

```python
# S3BucketSourceTypeDef definition

class S3BucketSourceTypeDef(TypedDict):
    S3Bucket: str,
    S3BucketOwner: NotRequired[str],
    S3KeyPrefix: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListContributorInsightsInputRequestTypeDef

```python
# ListContributorInsightsInputRequestTypeDef definition

class ListContributorInsightsInputRequestTypeDef(TypedDict):
    TableName: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListExportsInputRequestTypeDef

```python
# ListExportsInputRequestTypeDef definition

class ListExportsInputRequestTypeDef(TypedDict):
    TableArn: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListGlobalTablesInputRequestTypeDef

```python
# ListGlobalTablesInputRequestTypeDef definition

class ListGlobalTablesInputRequestTypeDef(TypedDict):
    ExclusiveStartGlobalTableName: NotRequired[str],
    Limit: NotRequired[int],
    RegionName: NotRequired[str],
```

## ListImportsInputRequestTypeDef

```python
# ListImportsInputRequestTypeDef definition

class ListImportsInputRequestTypeDef(TypedDict):
    TableArn: NotRequired[str],
    PageSize: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTablesInputRequestTypeDef

```python
# ListTablesInputRequestTypeDef definition

class ListTablesInputRequestTypeDef(TypedDict):
    ExclusiveStartTableName: NotRequired[str],
    Limit: NotRequired[int],
```

## ListTagsOfResourceInputRequestTypeDef

```python
# ListTagsOfResourceInputRequestTypeDef definition

class ListTagsOfResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    NextToken: NotRequired[str],
```

## PointInTimeRecoverySpecificationTypeDef

```python
# PointInTimeRecoverySpecificationTypeDef definition

class PointInTimeRecoverySpecificationTypeDef(TypedDict):
    PointInTimeRecoveryEnabled: bool,
```

## PutResourcePolicyInputRequestTypeDef

```python
# PutResourcePolicyInputRequestTypeDef definition

class PutResourcePolicyInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    Policy: str,
    ExpectedRevisionId: NotRequired[str],
    ConfirmRemoveSelfResourceAccess: NotRequired[bool],
```

## TableClassSummaryTypeDef

```python
# TableClassSummaryTypeDef definition

class TableClassSummaryTypeDef(TypedDict):
    TableClass: NotRequired[TableClassType],  # (1)
    LastUpdateDateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: TableClassType](./literals.md#tableclasstype) 
## RestoreSummaryTypeDef

```python
# RestoreSummaryTypeDef definition

class RestoreSummaryTypeDef(TypedDict):
    RestoreDateTime: datetime,
    RestoreInProgress: bool,
    SourceBackupArn: NotRequired[str],
    SourceTableArn: NotRequired[str],
```

## SSEDescriptionTypeDef

```python
# SSEDescriptionTypeDef definition

class SSEDescriptionTypeDef(TypedDict):
    Status: NotRequired[SSEStatusType],  # (1)
    SSEType: NotRequired[SSETypeType],  # (2)
    KMSMasterKeyArn: NotRequired[str],
    InaccessibleEncryptionDateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: SSEStatusType](./literals.md#ssestatustype) 
2. See [:material-code-brackets: SSETypeType](./literals.md#ssetypetype) 
## TableBatchWriterRequestTypeDef

```python
# TableBatchWriterRequestTypeDef definition

class TableBatchWriterRequestTypeDef(TypedDict):
    overwrite_by_pkeys: NotRequired[List[str]],
```

## TimeToLiveSpecificationTypeDef

```python
# TimeToLiveSpecificationTypeDef definition

class TimeToLiveSpecificationTypeDef(TypedDict):
    Enabled: bool,
    AttributeName: str,
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateContributorInsightsInputRequestTypeDef

```python
# UpdateContributorInsightsInputRequestTypeDef definition

class UpdateContributorInsightsInputRequestTypeDef(TypedDict):
    TableName: str,
    ContributorInsightsAction: ContributorInsightsActionType,  # (1)
    IndexName: NotRequired[str],
```

1. See [:material-code-brackets: ContributorInsightsActionType](./literals.md#contributorinsightsactiontype) 
## UpdateKinesisStreamingConfigurationTypeDef

```python
# UpdateKinesisStreamingConfigurationTypeDef definition

class UpdateKinesisStreamingConfigurationTypeDef(TypedDict):
    ApproximateCreationDateTimePrecision: NotRequired[ApproximateCreationDateTimePrecisionType],  # (1)
```

1. See [:material-code-brackets: ApproximateCreationDateTimePrecisionType](./literals.md#approximatecreationdatetimeprecisiontype) 
## BatchStatementErrorTypeDef

```python
# BatchStatementErrorTypeDef definition

class BatchStatementErrorTypeDef(TypedDict):
    Code: NotRequired[BatchStatementErrorCodeEnumType],  # (1)
    Message: NotRequired[str],
    Item: NotRequired[Dict[str, AttributeValueTypeDef]],  # (2)
```

1. See [:material-code-brackets: BatchStatementErrorCodeEnumType](./literals.md#batchstatementerrorcodeenumtype) 
2. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
## DeleteRequestOutputTypeDef

```python
# DeleteRequestOutputTypeDef definition

class DeleteRequestOutputTypeDef(TypedDict):
    Key: Dict[str, AttributeValueTypeDef],  # (1)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
## ItemCollectionMetricsTypeDef

```python
# ItemCollectionMetricsTypeDef definition

class ItemCollectionMetricsTypeDef(TypedDict):
    ItemCollectionKey: NotRequired[Dict[str, AttributeValueTypeDef]],  # (1)
    SizeEstimateRangeGB: NotRequired[List[float]],
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
## ItemResponseTypeDef

```python
# ItemResponseTypeDef definition

class ItemResponseTypeDef(TypedDict):
    Item: NotRequired[Dict[str, AttributeValueTypeDef]],  # (1)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
## KeysAndAttributesOutputTypeDef

```python
# KeysAndAttributesOutputTypeDef definition

class KeysAndAttributesOutputTypeDef(TypedDict):
    Keys: List[Dict[str, AttributeValueTypeDef]],  # (1)
    AttributesToGet: NotRequired[List[str]],
    ConsistentRead: NotRequired[bool],
    ProjectionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
## PutRequestOutputTypeDef

```python
# PutRequestOutputTypeDef definition

class PutRequestOutputTypeDef(TypedDict):
    Item: Dict[str, AttributeValueTypeDef],  # (1)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
## AttributeValueUpdateTableTypeDef

```python
# AttributeValueUpdateTableTypeDef definition

class AttributeValueUpdateTableTypeDef(TypedDict):
    Value: NotRequired[TableAttributeValueTypeDef],
    Action: NotRequired[AttributeActionType],  # (1)
```

1. See [:material-code-brackets: AttributeActionType](./literals.md#attributeactiontype) 
## ConditionTableTypeDef

```python
# ConditionTableTypeDef definition

class ConditionTableTypeDef(TypedDict):
    ComparisonOperator: ComparisonOperatorType,  # (1)
    AttributeValueList: NotRequired[Sequence[TableAttributeValueTypeDef]],
```

1. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
## DeleteRequestServiceResourceOutputTypeDef

```python
# DeleteRequestServiceResourceOutputTypeDef definition

class DeleteRequestServiceResourceOutputTypeDef(TypedDict):
    Key: Dict[str, TableAttributeValueTypeDef],
```

## DeleteRequestServiceResourceTypeDef

```python
# DeleteRequestServiceResourceTypeDef definition

class DeleteRequestServiceResourceTypeDef(TypedDict):
    Key: Mapping[str, TableAttributeValueTypeDef],
```

## ExpectedAttributeValueTableTypeDef

```python
# ExpectedAttributeValueTableTypeDef definition

class ExpectedAttributeValueTableTypeDef(TypedDict):
    Value: NotRequired[TableAttributeValueTypeDef],
    Exists: NotRequired[bool],
    ComparisonOperator: NotRequired[ComparisonOperatorType],  # (1)
    AttributeValueList: NotRequired[Sequence[TableAttributeValueTypeDef]],
```

1. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
## GetItemInputTableGetItemTypeDef

```python
# GetItemInputTableGetItemTypeDef definition

class GetItemInputTableGetItemTypeDef(TypedDict):
    Key: Mapping[str, TableAttributeValueTypeDef],
    AttributesToGet: NotRequired[Sequence[str]],
    ConsistentRead: NotRequired[bool],
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (1)
    ProjectionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
## ItemCollectionMetricsServiceResourceTypeDef

```python
# ItemCollectionMetricsServiceResourceTypeDef definition

class ItemCollectionMetricsServiceResourceTypeDef(TypedDict):
    ItemCollectionKey: NotRequired[Dict[str, TableAttributeValueTypeDef]],
    SizeEstimateRangeGB: NotRequired[List[float]],
```

## ItemCollectionMetricsTableTypeDef

```python
# ItemCollectionMetricsTableTypeDef definition

class ItemCollectionMetricsTableTypeDef(TypedDict):
    ItemCollectionKey: NotRequired[Dict[str, TableAttributeValueTypeDef]],
    SizeEstimateRangeGB: NotRequired[List[float]],
```

## KeysAndAttributesServiceResourceOutputTypeDef

```python
# KeysAndAttributesServiceResourceOutputTypeDef definition

class KeysAndAttributesServiceResourceOutputTypeDef(TypedDict):
    Keys: List[Dict[str, TableAttributeValueTypeDef]],
    AttributesToGet: NotRequired[List[str]],
    ConsistentRead: NotRequired[bool],
    ProjectionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Dict[str, str]],
```

## KeysAndAttributesServiceResourceTypeDef

```python
# KeysAndAttributesServiceResourceTypeDef definition

class KeysAndAttributesServiceResourceTypeDef(TypedDict):
    Keys: Sequence[Mapping[str, TableAttributeValueTypeDef]],
    AttributesToGet: NotRequired[Sequence[str]],
    ConsistentRead: NotRequired[bool],
    ProjectionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
```

## PutRequestServiceResourceOutputTypeDef

```python
# PutRequestServiceResourceOutputTypeDef definition

class PutRequestServiceResourceOutputTypeDef(TypedDict):
    Item: Dict[str, TableAttributeValueTypeDef],
```

## PutRequestServiceResourceTypeDef

```python
# PutRequestServiceResourceTypeDef definition

class PutRequestServiceResourceTypeDef(TypedDict):
    Item: Mapping[str, TableAttributeValueTypeDef],
```

## AutoScalingPolicyDescriptionTypeDef

```python
# AutoScalingPolicyDescriptionTypeDef definition

class AutoScalingPolicyDescriptionTypeDef(TypedDict):
    PolicyName: NotRequired[str],
    TargetTrackingScalingPolicyConfiguration: NotRequired[AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef],  # (1)
```

1. See [:material-code-braces: AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef](./type_defs.md#autoscalingtargettrackingscalingpolicyconfigurationdescriptiontypedef) 
## AutoScalingPolicyUpdateTypeDef

```python
# AutoScalingPolicyUpdateTypeDef definition

class AutoScalingPolicyUpdateTypeDef(TypedDict):
    TargetTrackingScalingPolicyConfiguration: AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,  # (1)
    PolicyName: NotRequired[str],
```

1. See [:material-code-braces: AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef](./type_defs.md#autoscalingtargettrackingscalingpolicyconfigurationupdatetypedef) 
## CreateBackupOutputTypeDef

```python
# CreateBackupOutputTypeDef definition

class CreateBackupOutputTypeDef(TypedDict):
    BackupDetails: BackupDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackupDetailsTypeDef](./type_defs.md#backupdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteResourcePolicyOutputTypeDef

```python
# DeleteResourcePolicyOutputTypeDef definition

class DeleteResourcePolicyOutputTypeDef(TypedDict):
    RevisionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLimitsOutputTypeDef

```python
# DescribeLimitsOutputTypeDef definition

class DescribeLimitsOutputTypeDef(TypedDict):
    AccountMaxReadCapacityUnits: int,
    AccountMaxWriteCapacityUnits: int,
    TableMaxReadCapacityUnits: int,
    TableMaxWriteCapacityUnits: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourcePolicyOutputTypeDef

```python
# GetResourcePolicyOutputTypeDef definition

class GetResourcePolicyOutputTypeDef(TypedDict):
    Policy: str,
    RevisionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBackupsOutputTypeDef

```python
# ListBackupsOutputTypeDef definition

class ListBackupsOutputTypeDef(TypedDict):
    BackupSummaries: List[BackupSummaryTypeDef],  # (1)
    LastEvaluatedBackupArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackupSummaryTypeDef](./type_defs.md#backupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTablesOutputTypeDef

```python
# ListTablesOutputTypeDef definition

class ListTablesOutputTypeDef(TypedDict):
    TableNames: List[str],
    LastEvaluatedTableName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutResourcePolicyOutputTypeDef

```python
# PutResourcePolicyOutputTypeDef definition

class PutResourcePolicyOutputTypeDef(TypedDict):
    RevisionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateContributorInsightsOutputTypeDef

```python
# UpdateContributorInsightsOutputTypeDef definition

class UpdateContributorInsightsOutputTypeDef(TypedDict):
    TableName: str,
    IndexName: str,
    ContributorInsightsStatus: ContributorInsightsStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ContributorInsightsStatusType](./literals.md#contributorinsightsstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConsumedCapacityTypeDef

```python
# ConsumedCapacityTypeDef definition

class ConsumedCapacityTypeDef(TypedDict):
    TableName: NotRequired[str],
    CapacityUnits: NotRequired[float],
    ReadCapacityUnits: NotRequired[float],
    WriteCapacityUnits: NotRequired[float],
    Table: NotRequired[CapacityTypeDef],  # (1)
    LocalSecondaryIndexes: NotRequired[Dict[str, CapacityTypeDef]],  # (2)
    GlobalSecondaryIndexes: NotRequired[Dict[str, CapacityTypeDef]],  # (2)
```

1. See [:material-code-braces: CapacityTypeDef](./type_defs.md#capacitytypedef) 
2. See [:material-code-braces: CapacityTypeDef](./type_defs.md#capacitytypedef) 
3. See [:material-code-braces: CapacityTypeDef](./type_defs.md#capacitytypedef) 
## ContinuousBackupsDescriptionTypeDef

```python
# ContinuousBackupsDescriptionTypeDef definition

class ContinuousBackupsDescriptionTypeDef(TypedDict):
    ContinuousBackupsStatus: ContinuousBackupsStatusType,  # (1)
    PointInTimeRecoveryDescription: NotRequired[PointInTimeRecoveryDescriptionTypeDef],  # (2)
```

1. See [:material-code-brackets: ContinuousBackupsStatusType](./literals.md#continuousbackupsstatustype) 
2. See [:material-code-braces: PointInTimeRecoveryDescriptionTypeDef](./type_defs.md#pointintimerecoverydescriptiontypedef) 
## ListContributorInsightsOutputTypeDef

```python
# ListContributorInsightsOutputTypeDef definition

class ListContributorInsightsOutputTypeDef(TypedDict):
    ContributorInsightsSummaries: List[ContributorInsightsSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ContributorInsightsSummaryTypeDef](./type_defs.md#contributorinsightssummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SourceTableDetailsTypeDef

```python
# SourceTableDetailsTypeDef definition

class SourceTableDetailsTypeDef(TypedDict):
    TableName: str,
    TableId: str,
    KeySchema: List[KeySchemaElementTypeDef],  # (1)
    TableCreationDateTime: datetime,
    ProvisionedThroughput: ProvisionedThroughputTypeDef,  # (2)
    TableArn: NotRequired[str],
    TableSizeBytes: NotRequired[int],
    OnDemandThroughput: NotRequired[OnDemandThroughputTypeDef],  # (3)
    ItemCount: NotRequired[int],
    BillingMode: NotRequired[BillingModeType],  # (4)
```

1. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
2. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
3. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
4. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
## UpdateGlobalSecondaryIndexActionTypeDef

```python
# UpdateGlobalSecondaryIndexActionTypeDef definition

class UpdateGlobalSecondaryIndexActionTypeDef(TypedDict):
    IndexName: str,
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (1)
    OnDemandThroughput: NotRequired[OnDemandThroughputTypeDef],  # (2)
```

1. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
2. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
## CreateGlobalTableInputRequestTypeDef

```python
# CreateGlobalTableInputRequestTypeDef definition

class CreateGlobalTableInputRequestTypeDef(TypedDict):
    GlobalTableName: str,
    ReplicationGroup: Sequence[ReplicaTypeDef],  # (1)
```

1. See [:material-code-braces: ReplicaTypeDef](./type_defs.md#replicatypedef) 
## GlobalTableTypeDef

```python
# GlobalTableTypeDef definition

class GlobalTableTypeDef(TypedDict):
    GlobalTableName: NotRequired[str],
    ReplicationGroup: NotRequired[List[ReplicaTypeDef]],  # (1)
```

1. See [:material-code-braces: ReplicaTypeDef](./type_defs.md#replicatypedef) 
## ReplicaGlobalSecondaryIndexDescriptionTypeDef

```python
# ReplicaGlobalSecondaryIndexDescriptionTypeDef definition

class ReplicaGlobalSecondaryIndexDescriptionTypeDef(TypedDict):
    IndexName: NotRequired[str],
    ProvisionedThroughputOverride: NotRequired[ProvisionedThroughputOverrideTypeDef],  # (1)
    OnDemandThroughputOverride: NotRequired[OnDemandThroughputOverrideTypeDef],  # (2)
```

1. See [:material-code-braces: ProvisionedThroughputOverrideTypeDef](./type_defs.md#provisionedthroughputoverridetypedef) 
2. See [:material-code-braces: OnDemandThroughputOverrideTypeDef](./type_defs.md#ondemandthroughputoverridetypedef) 
## ReplicaGlobalSecondaryIndexTypeDef

```python
# ReplicaGlobalSecondaryIndexTypeDef definition

class ReplicaGlobalSecondaryIndexTypeDef(TypedDict):
    IndexName: str,
    ProvisionedThroughputOverride: NotRequired[ProvisionedThroughputOverrideTypeDef],  # (1)
    OnDemandThroughputOverride: NotRequired[OnDemandThroughputOverrideTypeDef],  # (2)
```

1. See [:material-code-braces: ProvisionedThroughputOverrideTypeDef](./type_defs.md#provisionedthroughputoverridetypedef) 
2. See [:material-code-braces: OnDemandThroughputOverrideTypeDef](./type_defs.md#ondemandthroughputoverridetypedef) 
## ListTagsOfResourceOutputTypeDef

```python
# ListTagsOfResourceOutputTypeDef definition

class ListTagsOfResourceOutputTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## InputFormatOptionsOutputTypeDef

```python
# InputFormatOptionsOutputTypeDef definition

class InputFormatOptionsOutputTypeDef(TypedDict):
    Csv: NotRequired[CsvOptionsOutputTypeDef],  # (1)
```

1. See [:material-code-braces: CsvOptionsOutputTypeDef](./type_defs.md#csvoptionsoutputtypedef) 
## ReplicaUpdateTypeDef

```python
# ReplicaUpdateTypeDef definition

class ReplicaUpdateTypeDef(TypedDict):
    Create: NotRequired[CreateReplicaActionTypeDef],  # (1)
    Delete: NotRequired[DeleteReplicaActionTypeDef],  # (2)
```

1. See [:material-code-braces: CreateReplicaActionTypeDef](./type_defs.md#createreplicaactiontypedef) 
2. See [:material-code-braces: DeleteReplicaActionTypeDef](./type_defs.md#deletereplicaactiontypedef) 
## DescribeContributorInsightsOutputTypeDef

```python
# DescribeContributorInsightsOutputTypeDef definition

class DescribeContributorInsightsOutputTypeDef(TypedDict):
    TableName: str,
    IndexName: str,
    ContributorInsightsRuleList: List[str],
    ContributorInsightsStatus: ContributorInsightsStatusType,  # (1)
    LastUpdateDateTime: datetime,
    FailureException: FailureExceptionTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ContributorInsightsStatusType](./literals.md#contributorinsightsstatustype) 
2. See [:material-code-braces: FailureExceptionTypeDef](./type_defs.md#failureexceptiontypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEndpointsResponseTypeDef

```python
# DescribeEndpointsResponseTypeDef definition

class DescribeEndpointsResponseTypeDef(TypedDict):
    Endpoints: List[EndpointTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeKinesisStreamingDestinationOutputTypeDef

```python
# DescribeKinesisStreamingDestinationOutputTypeDef definition

class DescribeKinesisStreamingDestinationOutputTypeDef(TypedDict):
    TableName: str,
    KinesisDataStreamDestinations: List[KinesisDataStreamDestinationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KinesisDataStreamDestinationTypeDef](./type_defs.md#kinesisdatastreamdestinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTableInputTableExistsWaitTypeDef

```python
# DescribeTableInputTableExistsWaitTypeDef definition

class DescribeTableInputTableExistsWaitTypeDef(TypedDict):
    TableName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeTableInputTableNotExistsWaitTypeDef

```python
# DescribeTableInputTableNotExistsWaitTypeDef definition

class DescribeTableInputTableNotExistsWaitTypeDef(TypedDict):
    TableName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeTimeToLiveOutputTypeDef

```python
# DescribeTimeToLiveOutputTypeDef definition

class DescribeTimeToLiveOutputTypeDef(TypedDict):
    TimeToLiveDescription: TimeToLiveDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TimeToLiveDescriptionTypeDef](./type_defs.md#timetolivedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## KinesisStreamingDestinationInputRequestTypeDef

```python
# KinesisStreamingDestinationInputRequestTypeDef definition

class KinesisStreamingDestinationInputRequestTypeDef(TypedDict):
    TableName: str,
    StreamArn: str,
    EnableKinesisStreamingConfiguration: NotRequired[EnableKinesisStreamingConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: EnableKinesisStreamingConfigurationTypeDef](./type_defs.md#enablekinesisstreamingconfigurationtypedef) 
## KinesisStreamingDestinationOutputTypeDef

```python
# KinesisStreamingDestinationOutputTypeDef definition

class KinesisStreamingDestinationOutputTypeDef(TypedDict):
    TableName: str,
    StreamArn: str,
    DestinationStatus: DestinationStatusType,  # (1)
    EnableKinesisStreamingConfiguration: EnableKinesisStreamingConfigurationTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: DestinationStatusType](./literals.md#destinationstatustype) 
2. See [:material-code-braces: EnableKinesisStreamingConfigurationTypeDef](./type_defs.md#enablekinesisstreamingconfigurationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportDescriptionTypeDef

```python
# ExportDescriptionTypeDef definition

class ExportDescriptionTypeDef(TypedDict):
    ExportArn: NotRequired[str],
    ExportStatus: NotRequired[ExportStatusType],  # (1)
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    ExportManifest: NotRequired[str],
    TableArn: NotRequired[str],
    TableId: NotRequired[str],
    ExportTime: NotRequired[datetime],
    ClientToken: NotRequired[str],
    S3Bucket: NotRequired[str],
    S3BucketOwner: NotRequired[str],
    S3Prefix: NotRequired[str],
    S3SseAlgorithm: NotRequired[S3SseAlgorithmType],  # (2)
    S3SseKmsKeyId: NotRequired[str],
    FailureCode: NotRequired[str],
    FailureMessage: NotRequired[str],
    ExportFormat: NotRequired[ExportFormatType],  # (3)
    BilledSizeBytes: NotRequired[int],
    ItemCount: NotRequired[int],
    ExportType: NotRequired[ExportTypeType],  # (4)
    IncrementalExportSpecification: NotRequired[IncrementalExportSpecificationOutputTypeDef],  # (5)
```

1. See [:material-code-brackets: ExportStatusType](./literals.md#exportstatustype) 
2. See [:material-code-brackets: S3SseAlgorithmType](./literals.md#s3ssealgorithmtype) 
3. See [:material-code-brackets: ExportFormatType](./literals.md#exportformattype) 
4. See [:material-code-brackets: ExportTypeType](./literals.md#exporttypetype) 
5. See [:material-code-braces: IncrementalExportSpecificationOutputTypeDef](./type_defs.md#incrementalexportspecificationoutputtypedef) 
## ListExportsOutputTypeDef

```python
# ListExportsOutputTypeDef definition

class ListExportsOutputTypeDef(TypedDict):
    ExportSummaries: List[ExportSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ExportSummaryTypeDef](./type_defs.md#exportsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IncrementalExportSpecificationTypeDef

```python
# IncrementalExportSpecificationTypeDef definition

class IncrementalExportSpecificationTypeDef(TypedDict):
    ExportFromTime: NotRequired[TimestampTypeDef],
    ExportToTime: NotRequired[TimestampTypeDef],
    ExportViewType: NotRequired[ExportViewTypeType],  # (1)
```

1. See [:material-code-brackets: ExportViewTypeType](./literals.md#exportviewtypetype) 
## ListBackupsInputRequestTypeDef

```python
# ListBackupsInputRequestTypeDef definition

class ListBackupsInputRequestTypeDef(TypedDict):
    TableName: NotRequired[str],
    Limit: NotRequired[int],
    TimeRangeLowerBound: NotRequired[TimestampTypeDef],
    TimeRangeUpperBound: NotRequired[TimestampTypeDef],
    ExclusiveStartBackupArn: NotRequired[str],
    BackupType: NotRequired[BackupTypeFilterType],  # (1)
```

1. See [:material-code-brackets: BackupTypeFilterType](./literals.md#backuptypefiltertype) 
## GlobalSecondaryIndexInfoTypeDef

```python
# GlobalSecondaryIndexInfoTypeDef definition

class GlobalSecondaryIndexInfoTypeDef(TypedDict):
    IndexName: NotRequired[str],
    KeySchema: NotRequired[List[KeySchemaElementTypeDef]],  # (1)
    Projection: NotRequired[ProjectionOutputTypeDef],  # (2)
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (3)
    OnDemandThroughput: NotRequired[OnDemandThroughputTypeDef],  # (4)
```

1. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
2. See [:material-code-braces: ProjectionOutputTypeDef](./type_defs.md#projectionoutputtypedef) 
3. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
4. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
## GlobalSecondaryIndexOutputTypeDef

```python
# GlobalSecondaryIndexOutputTypeDef definition

class GlobalSecondaryIndexOutputTypeDef(TypedDict):
    IndexName: str,
    KeySchema: List[KeySchemaElementTypeDef],  # (1)
    Projection: ProjectionOutputTypeDef,  # (2)
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (3)
    OnDemandThroughput: NotRequired[OnDemandThroughputTypeDef],  # (4)
```

1. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
2. See [:material-code-braces: ProjectionOutputTypeDef](./type_defs.md#projectionoutputtypedef) 
3. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
4. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
## LocalSecondaryIndexDescriptionTypeDef

```python
# LocalSecondaryIndexDescriptionTypeDef definition

class LocalSecondaryIndexDescriptionTypeDef(TypedDict):
    IndexName: NotRequired[str],
    KeySchema: NotRequired[List[KeySchemaElementTypeDef]],  # (1)
    Projection: NotRequired[ProjectionOutputTypeDef],  # (2)
    IndexSizeBytes: NotRequired[int],
    ItemCount: NotRequired[int],
    IndexArn: NotRequired[str],
```

1. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
2. See [:material-code-braces: ProjectionOutputTypeDef](./type_defs.md#projectionoutputtypedef) 
## LocalSecondaryIndexInfoTypeDef

```python
# LocalSecondaryIndexInfoTypeDef definition

class LocalSecondaryIndexInfoTypeDef(TypedDict):
    IndexName: NotRequired[str],
    KeySchema: NotRequired[List[KeySchemaElementTypeDef]],  # (1)
    Projection: NotRequired[ProjectionOutputTypeDef],  # (2)
```

1. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
2. See [:material-code-braces: ProjectionOutputTypeDef](./type_defs.md#projectionoutputtypedef) 
## GlobalSecondaryIndexDescriptionTypeDef

```python
# GlobalSecondaryIndexDescriptionTypeDef definition

class GlobalSecondaryIndexDescriptionTypeDef(TypedDict):
    IndexName: NotRequired[str],
    KeySchema: NotRequired[List[KeySchemaElementTypeDef]],  # (1)
    Projection: NotRequired[ProjectionOutputTypeDef],  # (2)
    IndexStatus: NotRequired[IndexStatusType],  # (3)
    Backfilling: NotRequired[bool],
    ProvisionedThroughput: NotRequired[ProvisionedThroughputDescriptionTypeDef],  # (4)
    IndexSizeBytes: NotRequired[int],
    ItemCount: NotRequired[int],
    IndexArn: NotRequired[str],
    OnDemandThroughput: NotRequired[OnDemandThroughputTypeDef],  # (5)
```

1. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
2. See [:material-code-braces: ProjectionOutputTypeDef](./type_defs.md#projectionoutputtypedef) 
3. See [:material-code-brackets: IndexStatusType](./literals.md#indexstatustype) 
4. See [:material-code-braces: ProvisionedThroughputDescriptionTypeDef](./type_defs.md#provisionedthroughputdescriptiontypedef) 
5. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
## GlobalSecondaryIndexTypeDef

```python
# GlobalSecondaryIndexTypeDef definition

class GlobalSecondaryIndexTypeDef(TypedDict):
    IndexName: str,
    KeySchema: Sequence[KeySchemaElementTypeDef],  # (1)
    Projection: ProjectionTypeDef,  # (2)
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (3)
    OnDemandThroughput: NotRequired[OnDemandThroughputTypeDef],  # (4)
```

1. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
2. See [:material-code-braces: ProjectionTypeDef](./type_defs.md#projectiontypedef) 
3. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
4. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
## ImportSummaryTypeDef

```python
# ImportSummaryTypeDef definition

class ImportSummaryTypeDef(TypedDict):
    ImportArn: NotRequired[str],
    ImportStatus: NotRequired[ImportStatusType],  # (1)
    TableArn: NotRequired[str],
    S3BucketSource: NotRequired[S3BucketSourceTypeDef],  # (2)
    CloudWatchLogGroupArn: NotRequired[str],
    InputFormat: NotRequired[InputFormatType],  # (3)
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ImportStatusType](./literals.md#importstatustype) 
2. See [:material-code-braces: S3BucketSourceTypeDef](./type_defs.md#s3bucketsourcetypedef) 
3. See [:material-code-brackets: InputFormatType](./literals.md#inputformattype) 
## ListBackupsInputListBackupsPaginateTypeDef

```python
# ListBackupsInputListBackupsPaginateTypeDef definition

class ListBackupsInputListBackupsPaginateTypeDef(TypedDict):
    TableName: NotRequired[str],
    TimeRangeLowerBound: NotRequired[TimestampTypeDef],
    TimeRangeUpperBound: NotRequired[TimestampTypeDef],
    BackupType: NotRequired[BackupTypeFilterType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: BackupTypeFilterType](./literals.md#backuptypefiltertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTablesInputListTablesPaginateTypeDef

```python
# ListTablesInputListTablesPaginateTypeDef definition

class ListTablesInputListTablesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef

```python
# ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef definition

class ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef(TypedDict):
    ResourceArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## UpdateContinuousBackupsInputRequestTypeDef

```python
# UpdateContinuousBackupsInputRequestTypeDef definition

class UpdateContinuousBackupsInputRequestTypeDef(TypedDict):
    TableName: str,
    PointInTimeRecoverySpecification: PointInTimeRecoverySpecificationTypeDef,  # (1)
```

1. See [:material-code-braces: PointInTimeRecoverySpecificationTypeDef](./type_defs.md#pointintimerecoveryspecificationtypedef) 
## UpdateTimeToLiveInputRequestTypeDef

```python
# UpdateTimeToLiveInputRequestTypeDef definition

class UpdateTimeToLiveInputRequestTypeDef(TypedDict):
    TableName: str,
    TimeToLiveSpecification: TimeToLiveSpecificationTypeDef,  # (1)
```

1. See [:material-code-braces: TimeToLiveSpecificationTypeDef](./type_defs.md#timetolivespecificationtypedef) 
## UpdateTimeToLiveOutputTypeDef

```python
# UpdateTimeToLiveOutputTypeDef definition

class UpdateTimeToLiveOutputTypeDef(TypedDict):
    TimeToLiveSpecification: TimeToLiveSpecificationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TimeToLiveSpecificationTypeDef](./type_defs.md#timetolivespecificationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateKinesisStreamingDestinationInputRequestTypeDef

```python
# UpdateKinesisStreamingDestinationInputRequestTypeDef definition

class UpdateKinesisStreamingDestinationInputRequestTypeDef(TypedDict):
    TableName: str,
    StreamArn: str,
    UpdateKinesisStreamingConfiguration: NotRequired[UpdateKinesisStreamingConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: UpdateKinesisStreamingConfigurationTypeDef](./type_defs.md#updatekinesisstreamingconfigurationtypedef) 
## UpdateKinesisStreamingDestinationOutputTypeDef

```python
# UpdateKinesisStreamingDestinationOutputTypeDef definition

class UpdateKinesisStreamingDestinationOutputTypeDef(TypedDict):
    TableName: str,
    StreamArn: str,
    DestinationStatus: DestinationStatusType,  # (1)
    UpdateKinesisStreamingConfiguration: UpdateKinesisStreamingConfigurationTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: DestinationStatusType](./literals.md#destinationstatustype) 
2. See [:material-code-braces: UpdateKinesisStreamingConfigurationTypeDef](./type_defs.md#updatekinesisstreamingconfigurationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchStatementResponseTypeDef

```python
# BatchStatementResponseTypeDef definition

class BatchStatementResponseTypeDef(TypedDict):
    Error: NotRequired[BatchStatementErrorTypeDef],  # (1)
    TableName: NotRequired[str],
    Item: NotRequired[Dict[str, AttributeValueTypeDef]],  # (2)
```

1. See [:material-code-braces: BatchStatementErrorTypeDef](./type_defs.md#batchstatementerrortypedef) 
2. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
## WriteRequestOutputTypeDef

```python
# WriteRequestOutputTypeDef definition

class WriteRequestOutputTypeDef(TypedDict):
    PutRequest: NotRequired[PutRequestOutputTypeDef],  # (1)
    DeleteRequest: NotRequired[DeleteRequestOutputTypeDef],  # (2)
```

1. See [:material-code-braces: PutRequestOutputTypeDef](./type_defs.md#putrequestoutputtypedef) 
2. See [:material-code-braces: DeleteRequestOutputTypeDef](./type_defs.md#deleterequestoutputtypedef) 
## AttributeValueUpdateTypeDef

```python
# AttributeValueUpdateTypeDef definition

class AttributeValueUpdateTypeDef(TypedDict):
    Value: NotRequired[UniversalAttributeValueTypeDef],  # (1)
    Action: NotRequired[AttributeActionType],  # (2)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-brackets: AttributeActionType](./literals.md#attributeactiontype) 
## BatchStatementRequestTypeDef

```python
# BatchStatementRequestTypeDef definition

class BatchStatementRequestTypeDef(TypedDict):
    Statement: str,
    Parameters: NotRequired[Sequence[UniversalAttributeValueTypeDef]],  # (1)
    ConsistentRead: NotRequired[bool],
    ReturnValuesOnConditionCheckFailure: NotRequired[ReturnValuesOnConditionCheckFailureType],  # (2)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
## ConditionCheckTypeDef

```python
# ConditionCheckTypeDef definition

class ConditionCheckTypeDef(TypedDict):
    Key: Mapping[str, UniversalAttributeValueTypeDef],  # (1)
    TableName: str,
    ConditionExpression: str,
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, UniversalAttributeValueTypeDef]],  # (1)
    ReturnValuesOnConditionCheckFailure: NotRequired[ReturnValuesOnConditionCheckFailureType],  # (3)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
3. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
## ConditionTypeDef

```python
# ConditionTypeDef definition

class ConditionTypeDef(TypedDict):
    ComparisonOperator: ComparisonOperatorType,  # (2)
    AttributeValueList: NotRequired[Sequence[UniversalAttributeValueTypeDef]],  # (1)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
## DeleteRequestTypeDef

```python
# DeleteRequestTypeDef definition

class DeleteRequestTypeDef(TypedDict):
    Key: Mapping[str, UniversalAttributeValueTypeDef],  # (1)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
## DeleteTypeDef

```python
# DeleteTypeDef definition

class DeleteTypeDef(TypedDict):
    Key: Mapping[str, UniversalAttributeValueTypeDef],  # (1)
    TableName: str,
    ConditionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, UniversalAttributeValueTypeDef]],  # (1)
    ReturnValuesOnConditionCheckFailure: NotRequired[ReturnValuesOnConditionCheckFailureType],  # (3)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
3. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
## ExecuteStatementInputRequestTypeDef

```python
# ExecuteStatementInputRequestTypeDef definition

class ExecuteStatementInputRequestTypeDef(TypedDict):
    Statement: str,
    Parameters: NotRequired[Sequence[UniversalAttributeValueTypeDef]],  # (1)
    ConsistentRead: NotRequired[bool],
    NextToken: NotRequired[str],
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (2)
    Limit: NotRequired[int],
    ReturnValuesOnConditionCheckFailure: NotRequired[ReturnValuesOnConditionCheckFailureType],  # (3)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
3. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
## ExpectedAttributeValueTypeDef

```python
# ExpectedAttributeValueTypeDef definition

class ExpectedAttributeValueTypeDef(TypedDict):
    Value: NotRequired[UniversalAttributeValueTypeDef],  # (1)
    Exists: NotRequired[bool],
    ComparisonOperator: NotRequired[ComparisonOperatorType],  # (2)
    AttributeValueList: NotRequired[Sequence[UniversalAttributeValueTypeDef]],  # (3)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
3. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
## GetItemInputRequestTypeDef

```python
# GetItemInputRequestTypeDef definition

class GetItemInputRequestTypeDef(TypedDict):
    TableName: str,
    Key: Mapping[str, UniversalAttributeValueTypeDef],  # (1)
    AttributesToGet: NotRequired[Sequence[str]],
    ConsistentRead: NotRequired[bool],
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (2)
    ProjectionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
## GetTypeDef

```python
# GetTypeDef definition

class GetTypeDef(TypedDict):
    Key: Mapping[str, UniversalAttributeValueTypeDef],  # (1)
    TableName: str,
    ProjectionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
## KeysAndAttributesTypeDef

```python
# KeysAndAttributesTypeDef definition

class KeysAndAttributesTypeDef(TypedDict):
    Keys: Sequence[Mapping[str, UniversalAttributeValueTypeDef]],  # (1)
    AttributesToGet: NotRequired[Sequence[str]],
    ConsistentRead: NotRequired[bool],
    ProjectionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
## ParameterizedStatementTypeDef

```python
# ParameterizedStatementTypeDef definition

class ParameterizedStatementTypeDef(TypedDict):
    Statement: str,
    Parameters: NotRequired[Sequence[UniversalAttributeValueTypeDef]],  # (1)
    ReturnValuesOnConditionCheckFailure: NotRequired[ReturnValuesOnConditionCheckFailureType],  # (2)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
## PutRequestTypeDef

```python
# PutRequestTypeDef definition

class PutRequestTypeDef(TypedDict):
    Item: Mapping[str, UniversalAttributeValueTypeDef],  # (1)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
## PutTypeDef

```python
# PutTypeDef definition

class PutTypeDef(TypedDict):
    Item: Mapping[str, UniversalAttributeValueTypeDef],  # (1)
    TableName: str,
    ConditionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, UniversalAttributeValueTypeDef]],  # (1)
    ReturnValuesOnConditionCheckFailure: NotRequired[ReturnValuesOnConditionCheckFailureType],  # (3)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
3. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
## UpdateTypeDef

```python
# UpdateTypeDef definition

class UpdateTypeDef(TypedDict):
    Key: Mapping[str, UniversalAttributeValueTypeDef],  # (1)
    UpdateExpression: str,
    TableName: str,
    ConditionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, UniversalAttributeValueTypeDef]],  # (1)
    ReturnValuesOnConditionCheckFailure: NotRequired[ReturnValuesOnConditionCheckFailureType],  # (3)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
3. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
## QueryInputTableQueryTypeDef

```python
# QueryInputTableQueryTypeDef definition

class QueryInputTableQueryTypeDef(TypedDict):
    IndexName: NotRequired[str],
    Select: NotRequired[SelectType],  # (1)
    AttributesToGet: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
    ConsistentRead: NotRequired[bool],
    KeyConditions: NotRequired[Mapping[str, ConditionTableTypeDef]],  # (2)
    QueryFilter: NotRequired[Mapping[str, ConditionTableTypeDef]],  # (2)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (4)
    ScanIndexForward: NotRequired[bool],
    ExclusiveStartKey: NotRequired[Mapping[str, TableAttributeValueTypeDef]],
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (5)
    ProjectionExpression: NotRequired[str],
    FilterExpression: NotRequired[ConditionBaseImportTypeDef],
    KeyConditionExpression: NotRequired[ConditionBaseImportTypeDef],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, TableAttributeValueTypeDef]],
```

1. See [:material-code-brackets: SelectType](./literals.md#selecttype) 
2. See [:material-code-braces: ConditionTableTypeDef](./type_defs.md#conditiontabletypedef) 
3. See [:material-code-braces: ConditionTableTypeDef](./type_defs.md#conditiontabletypedef) 
4. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
5. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
## ScanInputTableScanTypeDef

```python
# ScanInputTableScanTypeDef definition

class ScanInputTableScanTypeDef(TypedDict):
    IndexName: NotRequired[str],
    AttributesToGet: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
    Select: NotRequired[SelectType],  # (1)
    ScanFilter: NotRequired[Mapping[str, ConditionTableTypeDef]],  # (2)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (3)
    ExclusiveStartKey: NotRequired[Mapping[str, TableAttributeValueTypeDef]],
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (4)
    TotalSegments: NotRequired[int],
    Segment: NotRequired[int],
    ProjectionExpression: NotRequired[str],
    FilterExpression: NotRequired[ConditionBaseImportTypeDef],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, TableAttributeValueTypeDef]],
    ConsistentRead: NotRequired[bool],
```

1. See [:material-code-brackets: SelectType](./literals.md#selecttype) 
2. See [:material-code-braces: ConditionTableTypeDef](./type_defs.md#conditiontabletypedef) 
3. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
4. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
## DeleteItemInputTableDeleteItemTypeDef

```python
# DeleteItemInputTableDeleteItemTypeDef definition

class DeleteItemInputTableDeleteItemTypeDef(TypedDict):
    Key: Mapping[str, TableAttributeValueTypeDef],
    Expected: NotRequired[Mapping[str, ExpectedAttributeValueTableTypeDef]],  # (1)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (2)
    ReturnValues: NotRequired[ReturnValueType],  # (3)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (4)
    ReturnItemCollectionMetrics: NotRequired[ReturnItemCollectionMetricsType],  # (5)
    ConditionExpression: NotRequired[ConditionBaseImportTypeDef],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, TableAttributeValueTypeDef]],
    ReturnValuesOnConditionCheckFailure: NotRequired[ReturnValuesOnConditionCheckFailureType],  # (6)
```

1. See [:material-code-braces: ExpectedAttributeValueTableTypeDef](./type_defs.md#expectedattributevaluetabletypedef) 
2. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
3. See [:material-code-brackets: ReturnValueType](./literals.md#returnvaluetype) 
4. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
5. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
6. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
## PutItemInputTablePutItemTypeDef

```python
# PutItemInputTablePutItemTypeDef definition

class PutItemInputTablePutItemTypeDef(TypedDict):
    Item: Mapping[str, TableAttributeValueTypeDef],
    Expected: NotRequired[Mapping[str, ExpectedAttributeValueTableTypeDef]],  # (1)
    ReturnValues: NotRequired[ReturnValueType],  # (2)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (3)
    ReturnItemCollectionMetrics: NotRequired[ReturnItemCollectionMetricsType],  # (4)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (5)
    ConditionExpression: NotRequired[ConditionBaseImportTypeDef],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, TableAttributeValueTypeDef]],
    ReturnValuesOnConditionCheckFailure: NotRequired[ReturnValuesOnConditionCheckFailureType],  # (6)
```

1. See [:material-code-braces: ExpectedAttributeValueTableTypeDef](./type_defs.md#expectedattributevaluetabletypedef) 
2. See [:material-code-brackets: ReturnValueType](./literals.md#returnvaluetype) 
3. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
4. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
5. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
6. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
## UpdateItemInputTableUpdateItemTypeDef

```python
# UpdateItemInputTableUpdateItemTypeDef definition

class UpdateItemInputTableUpdateItemTypeDef(TypedDict):
    Key: Mapping[str, TableAttributeValueTypeDef],
    AttributeUpdates: NotRequired[Mapping[str, AttributeValueUpdateTableTypeDef]],  # (1)
    Expected: NotRequired[Mapping[str, ExpectedAttributeValueTableTypeDef]],  # (2)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (3)
    ReturnValues: NotRequired[ReturnValueType],  # (4)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (5)
    ReturnItemCollectionMetrics: NotRequired[ReturnItemCollectionMetricsType],  # (6)
    UpdateExpression: NotRequired[str],
    ConditionExpression: NotRequired[ConditionBaseImportTypeDef],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, TableAttributeValueTypeDef]],
    ReturnValuesOnConditionCheckFailure: NotRequired[ReturnValuesOnConditionCheckFailureType],  # (7)
```

1. See [:material-code-braces: AttributeValueUpdateTableTypeDef](./type_defs.md#attributevalueupdatetabletypedef) 
2. See [:material-code-braces: ExpectedAttributeValueTableTypeDef](./type_defs.md#expectedattributevaluetabletypedef) 
3. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
4. See [:material-code-brackets: ReturnValueType](./literals.md#returnvaluetype) 
5. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
6. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
7. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
## WriteRequestServiceResourceOutputTypeDef

```python
# WriteRequestServiceResourceOutputTypeDef definition

class WriteRequestServiceResourceOutputTypeDef(TypedDict):
    PutRequest: NotRequired[PutRequestServiceResourceOutputTypeDef],  # (1)
    DeleteRequest: NotRequired[DeleteRequestServiceResourceOutputTypeDef],  # (2)
```

1. See [:material-code-braces: PutRequestServiceResourceOutputTypeDef](./type_defs.md#putrequestserviceresourceoutputtypedef) 
2. See [:material-code-braces: DeleteRequestServiceResourceOutputTypeDef](./type_defs.md#deleterequestserviceresourceoutputtypedef) 
## AutoScalingSettingsDescriptionTypeDef

```python
# AutoScalingSettingsDescriptionTypeDef definition

class AutoScalingSettingsDescriptionTypeDef(TypedDict):
    MinimumUnits: NotRequired[int],
    MaximumUnits: NotRequired[int],
    AutoScalingDisabled: NotRequired[bool],
    AutoScalingRoleArn: NotRequired[str],
    ScalingPolicies: NotRequired[List[AutoScalingPolicyDescriptionTypeDef]],  # (1)
```

1. See [:material-code-braces: AutoScalingPolicyDescriptionTypeDef](./type_defs.md#autoscalingpolicydescriptiontypedef) 
## AutoScalingSettingsUpdateTypeDef

```python
# AutoScalingSettingsUpdateTypeDef definition

class AutoScalingSettingsUpdateTypeDef(TypedDict):
    MinimumUnits: NotRequired[int],
    MaximumUnits: NotRequired[int],
    AutoScalingDisabled: NotRequired[bool],
    AutoScalingRoleArn: NotRequired[str],
    ScalingPolicyUpdate: NotRequired[AutoScalingPolicyUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: AutoScalingPolicyUpdateTypeDef](./type_defs.md#autoscalingpolicyupdatetypedef) 
## BatchGetItemOutputServiceResourceTypeDef

```python
# BatchGetItemOutputServiceResourceTypeDef definition

class BatchGetItemOutputServiceResourceTypeDef(TypedDict):
    Responses: Dict[str, List[Dict[str, TableAttributeValueTypeDef]]],
    UnprocessedKeys: Dict[str, KeysAndAttributesServiceResourceOutputTypeDef],  # (1)
    ConsumedCapacity: List[ConsumedCapacityTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: KeysAndAttributesServiceResourceOutputTypeDef](./type_defs.md#keysandattributesserviceresourceoutputtypedef) 
2. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetItemOutputTypeDef

```python
# BatchGetItemOutputTypeDef definition

class BatchGetItemOutputTypeDef(TypedDict):
    Responses: Dict[str, List[Dict[str, AttributeValueTypeDef]]],  # (1)
    UnprocessedKeys: Dict[str, KeysAndAttributesOutputTypeDef],  # (2)
    ConsumedCapacity: List[ConsumedCapacityTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: KeysAndAttributesOutputTypeDef](./type_defs.md#keysandattributesoutputtypedef) 
3. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteItemOutputTableTypeDef

```python
# DeleteItemOutputTableTypeDef definition

class DeleteItemOutputTableTypeDef(TypedDict):
    Attributes: Dict[str, TableAttributeValueTypeDef],
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (1)
    ItemCollectionMetrics: ItemCollectionMetricsTableTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
2. See [:material-code-braces: ItemCollectionMetricsTableTypeDef](./type_defs.md#itemcollectionmetricstabletypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteItemOutputTypeDef

```python
# DeleteItemOutputTypeDef definition

class DeleteItemOutputTypeDef(TypedDict):
    Attributes: Dict[str, AttributeValueTypeDef],  # (1)
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (2)
    ItemCollectionMetrics: ItemCollectionMetricsTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
3. See [:material-code-braces: ItemCollectionMetricsTypeDef](./type_defs.md#itemcollectionmetricstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExecuteStatementOutputTypeDef

```python
# ExecuteStatementOutputTypeDef definition

class ExecuteStatementOutputTypeDef(TypedDict):
    Items: List[Dict[str, AttributeValueTypeDef]],  # (1)
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (2)
    LastEvaluatedKey: Dict[str, AttributeValueTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
3. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExecuteTransactionOutputTypeDef

```python
# ExecuteTransactionOutputTypeDef definition

class ExecuteTransactionOutputTypeDef(TypedDict):
    Responses: List[ItemResponseTypeDef],  # (1)
    ConsumedCapacity: List[ConsumedCapacityTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ItemResponseTypeDef](./type_defs.md#itemresponsetypedef) 
2. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetItemOutputTableTypeDef

```python
# GetItemOutputTableTypeDef definition

class GetItemOutputTableTypeDef(TypedDict):
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    Item: NotRequired[Dict[str, TableAttributeValueTypeDef]],
```

1. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetItemOutputTypeDef

```python
# GetItemOutputTypeDef definition

class GetItemOutputTypeDef(TypedDict):
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    Item: NotRequired[Dict[str, AttributeValueTypeDef]],  # (1)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutItemOutputTableTypeDef

```python
# PutItemOutputTableTypeDef definition

class PutItemOutputTableTypeDef(TypedDict):
    Attributes: Dict[str, TableAttributeValueTypeDef],
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (1)
    ItemCollectionMetrics: ItemCollectionMetricsTableTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
2. See [:material-code-braces: ItemCollectionMetricsTableTypeDef](./type_defs.md#itemcollectionmetricstabletypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutItemOutputTypeDef

```python
# PutItemOutputTypeDef definition

class PutItemOutputTypeDef(TypedDict):
    Attributes: Dict[str, AttributeValueTypeDef],  # (1)
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (2)
    ItemCollectionMetrics: ItemCollectionMetricsTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
3. See [:material-code-braces: ItemCollectionMetricsTypeDef](./type_defs.md#itemcollectionmetricstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## QueryOutputTableTypeDef

```python
# QueryOutputTableTypeDef definition

class QueryOutputTableTypeDef(TypedDict):
    Items: List[Dict[str, TableAttributeValueTypeDef]],
    Count: int,
    ScannedCount: int,
    LastEvaluatedKey: Dict[str, TableAttributeValueTypeDef],
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## QueryOutputTypeDef

```python
# QueryOutputTypeDef definition

class QueryOutputTypeDef(TypedDict):
    Items: List[Dict[str, AttributeValueTypeDef]],  # (1)
    Count: int,
    ScannedCount: int,
    LastEvaluatedKey: Dict[str, AttributeValueTypeDef],  # (2)
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
3. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ScanOutputTableTypeDef

```python
# ScanOutputTableTypeDef definition

class ScanOutputTableTypeDef(TypedDict):
    Items: List[Dict[str, TableAttributeValueTypeDef]],
    Count: int,
    ScannedCount: int,
    LastEvaluatedKey: Dict[str, TableAttributeValueTypeDef],
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ScanOutputTypeDef

```python
# ScanOutputTypeDef definition

class ScanOutputTypeDef(TypedDict):
    Items: List[Dict[str, AttributeValueTypeDef]],  # (1)
    Count: int,
    ScannedCount: int,
    LastEvaluatedKey: Dict[str, AttributeValueTypeDef],  # (2)
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
3. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TransactGetItemsOutputTypeDef

```python
# TransactGetItemsOutputTypeDef definition

class TransactGetItemsOutputTypeDef(TypedDict):
    ConsumedCapacity: List[ConsumedCapacityTypeDef],  # (1)
    Responses: List[ItemResponseTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
2. See [:material-code-braces: ItemResponseTypeDef](./type_defs.md#itemresponsetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TransactWriteItemsOutputTypeDef

```python
# TransactWriteItemsOutputTypeDef definition

class TransactWriteItemsOutputTypeDef(TypedDict):
    ConsumedCapacity: List[ConsumedCapacityTypeDef],  # (1)
    ItemCollectionMetrics: Dict[str, List[ItemCollectionMetricsTypeDef]],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
2. See [:material-code-braces: ItemCollectionMetricsTypeDef](./type_defs.md#itemcollectionmetricstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateItemOutputTableTypeDef

```python
# UpdateItemOutputTableTypeDef definition

class UpdateItemOutputTableTypeDef(TypedDict):
    Attributes: Dict[str, TableAttributeValueTypeDef],
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (1)
    ItemCollectionMetrics: ItemCollectionMetricsTableTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
2. See [:material-code-braces: ItemCollectionMetricsTableTypeDef](./type_defs.md#itemcollectionmetricstabletypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateItemOutputTypeDef

```python
# UpdateItemOutputTypeDef definition

class UpdateItemOutputTypeDef(TypedDict):
    Attributes: Dict[str, AttributeValueTypeDef],  # (1)
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (2)
    ItemCollectionMetrics: ItemCollectionMetricsTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
3. See [:material-code-braces: ItemCollectionMetricsTypeDef](./type_defs.md#itemcollectionmetricstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeContinuousBackupsOutputTypeDef

```python
# DescribeContinuousBackupsOutputTypeDef definition

class DescribeContinuousBackupsOutputTypeDef(TypedDict):
    ContinuousBackupsDescription: ContinuousBackupsDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContinuousBackupsDescriptionTypeDef](./type_defs.md#continuousbackupsdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateContinuousBackupsOutputTypeDef

```python
# UpdateContinuousBackupsOutputTypeDef definition

class UpdateContinuousBackupsOutputTypeDef(TypedDict):
    ContinuousBackupsDescription: ContinuousBackupsDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContinuousBackupsDescriptionTypeDef](./type_defs.md#continuousbackupsdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGlobalTablesOutputTypeDef

```python
# ListGlobalTablesOutputTypeDef definition

class ListGlobalTablesOutputTypeDef(TypedDict):
    GlobalTables: List[GlobalTableTypeDef],  # (1)
    LastEvaluatedGlobalTableName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GlobalTableTypeDef](./type_defs.md#globaltabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReplicaDescriptionTypeDef

```python
# ReplicaDescriptionTypeDef definition

class ReplicaDescriptionTypeDef(TypedDict):
    RegionName: NotRequired[str],
    ReplicaStatus: NotRequired[ReplicaStatusType],  # (1)
    ReplicaStatusDescription: NotRequired[str],
    ReplicaStatusPercentProgress: NotRequired[str],
    KMSMasterKeyId: NotRequired[str],
    ProvisionedThroughputOverride: NotRequired[ProvisionedThroughputOverrideTypeDef],  # (2)
    OnDemandThroughputOverride: NotRequired[OnDemandThroughputOverrideTypeDef],  # (3)
    GlobalSecondaryIndexes: NotRequired[List[ReplicaGlobalSecondaryIndexDescriptionTypeDef]],  # (4)
    ReplicaInaccessibleDateTime: NotRequired[datetime],
    ReplicaTableClassSummary: NotRequired[TableClassSummaryTypeDef],  # (5)
```

1. See [:material-code-brackets: ReplicaStatusType](./literals.md#replicastatustype) 
2. See [:material-code-braces: ProvisionedThroughputOverrideTypeDef](./type_defs.md#provisionedthroughputoverridetypedef) 
3. See [:material-code-braces: OnDemandThroughputOverrideTypeDef](./type_defs.md#ondemandthroughputoverridetypedef) 
4. See [:material-code-braces: ReplicaGlobalSecondaryIndexDescriptionTypeDef](./type_defs.md#replicaglobalsecondaryindexdescriptiontypedef) 
5. See [:material-code-braces: TableClassSummaryTypeDef](./type_defs.md#tableclasssummarytypedef) 
## CreateReplicationGroupMemberActionTypeDef

```python
# CreateReplicationGroupMemberActionTypeDef definition

class CreateReplicationGroupMemberActionTypeDef(TypedDict):
    RegionName: str,
    KMSMasterKeyId: NotRequired[str],
    ProvisionedThroughputOverride: NotRequired[ProvisionedThroughputOverrideTypeDef],  # (1)
    OnDemandThroughputOverride: NotRequired[OnDemandThroughputOverrideTypeDef],  # (2)
    GlobalSecondaryIndexes: NotRequired[Sequence[ReplicaGlobalSecondaryIndexTypeDef]],  # (3)
    TableClassOverride: NotRequired[TableClassType],  # (4)
```

1. See [:material-code-braces: ProvisionedThroughputOverrideTypeDef](./type_defs.md#provisionedthroughputoverridetypedef) 
2. See [:material-code-braces: OnDemandThroughputOverrideTypeDef](./type_defs.md#ondemandthroughputoverridetypedef) 
3. See [:material-code-braces: ReplicaGlobalSecondaryIndexTypeDef](./type_defs.md#replicaglobalsecondaryindextypedef) 
4. See [:material-code-brackets: TableClassType](./literals.md#tableclasstype) 
## UpdateReplicationGroupMemberActionTypeDef

```python
# UpdateReplicationGroupMemberActionTypeDef definition

class UpdateReplicationGroupMemberActionTypeDef(TypedDict):
    RegionName: str,
    KMSMasterKeyId: NotRequired[str],
    ProvisionedThroughputOverride: NotRequired[ProvisionedThroughputOverrideTypeDef],  # (1)
    OnDemandThroughputOverride: NotRequired[OnDemandThroughputOverrideTypeDef],  # (2)
    GlobalSecondaryIndexes: NotRequired[Sequence[ReplicaGlobalSecondaryIndexTypeDef]],  # (3)
    TableClassOverride: NotRequired[TableClassType],  # (4)
```

1. See [:material-code-braces: ProvisionedThroughputOverrideTypeDef](./type_defs.md#provisionedthroughputoverridetypedef) 
2. See [:material-code-braces: OnDemandThroughputOverrideTypeDef](./type_defs.md#ondemandthroughputoverridetypedef) 
3. See [:material-code-braces: ReplicaGlobalSecondaryIndexTypeDef](./type_defs.md#replicaglobalsecondaryindextypedef) 
4. See [:material-code-brackets: TableClassType](./literals.md#tableclasstype) 
## InputFormatOptionsTypeDef

```python
# InputFormatOptionsTypeDef definition

class InputFormatOptionsTypeDef(TypedDict):
    Csv: NotRequired[CsvOptionsUnionTypeDef],  # (1)
```

1. See [:material-code-braces: CsvOptionsTypeDef](./type_defs.md#csvoptionstypedef) [:material-code-braces: CsvOptionsOutputTypeDef](./type_defs.md#csvoptionsoutputtypedef) 
## UpdateGlobalTableInputRequestTypeDef

```python
# UpdateGlobalTableInputRequestTypeDef definition

class UpdateGlobalTableInputRequestTypeDef(TypedDict):
    GlobalTableName: str,
    ReplicaUpdates: Sequence[ReplicaUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: ReplicaUpdateTypeDef](./type_defs.md#replicaupdatetypedef) 
## DescribeExportOutputTypeDef

```python
# DescribeExportOutputTypeDef definition

class DescribeExportOutputTypeDef(TypedDict):
    ExportDescription: ExportDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExportDescriptionTypeDef](./type_defs.md#exportdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportTableToPointInTimeOutputTypeDef

```python
# ExportTableToPointInTimeOutputTypeDef definition

class ExportTableToPointInTimeOutputTypeDef(TypedDict):
    ExportDescription: ExportDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExportDescriptionTypeDef](./type_defs.md#exportdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportTableToPointInTimeInputRequestTypeDef

```python
# ExportTableToPointInTimeInputRequestTypeDef definition

class ExportTableToPointInTimeInputRequestTypeDef(TypedDict):
    TableArn: str,
    S3Bucket: str,
    ExportTime: NotRequired[TimestampTypeDef],
    ClientToken: NotRequired[str],
    S3BucketOwner: NotRequired[str],
    S3Prefix: NotRequired[str],
    S3SseAlgorithm: NotRequired[S3SseAlgorithmType],  # (1)
    S3SseKmsKeyId: NotRequired[str],
    ExportFormat: NotRequired[ExportFormatType],  # (2)
    ExportType: NotRequired[ExportTypeType],  # (3)
    IncrementalExportSpecification: NotRequired[IncrementalExportSpecificationTypeDef],  # (4)
```

1. See [:material-code-brackets: S3SseAlgorithmType](./literals.md#s3ssealgorithmtype) 
2. See [:material-code-brackets: ExportFormatType](./literals.md#exportformattype) 
3. See [:material-code-brackets: ExportTypeType](./literals.md#exporttypetype) 
4. See [:material-code-braces: IncrementalExportSpecificationTypeDef](./type_defs.md#incrementalexportspecificationtypedef) 
## TableCreationParametersOutputTypeDef

```python
# TableCreationParametersOutputTypeDef definition

class TableCreationParametersOutputTypeDef(TypedDict):
    TableName: str,
    AttributeDefinitions: List[AttributeDefinitionTypeDef],  # (1)
    KeySchema: List[KeySchemaElementTypeDef],  # (2)
    BillingMode: NotRequired[BillingModeType],  # (3)
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (4)
    OnDemandThroughput: NotRequired[OnDemandThroughputTypeDef],  # (5)
    SSESpecification: NotRequired[SSESpecificationTypeDef],  # (6)
    GlobalSecondaryIndexes: NotRequired[List[GlobalSecondaryIndexOutputTypeDef]],  # (7)
```

1. See [:material-code-braces: AttributeDefinitionTypeDef](./type_defs.md#attributedefinitiontypedef) 
2. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
3. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
4. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
5. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
6. See [:material-code-braces: SSESpecificationTypeDef](./type_defs.md#ssespecificationtypedef) 
7. See [:material-code-braces: GlobalSecondaryIndexOutputTypeDef](./type_defs.md#globalsecondaryindexoutputtypedef) 
## SourceTableFeatureDetailsTypeDef

```python
# SourceTableFeatureDetailsTypeDef definition

class SourceTableFeatureDetailsTypeDef(TypedDict):
    LocalSecondaryIndexes: NotRequired[List[LocalSecondaryIndexInfoTypeDef]],  # (1)
    GlobalSecondaryIndexes: NotRequired[List[GlobalSecondaryIndexInfoTypeDef]],  # (2)
    StreamDescription: NotRequired[StreamSpecificationTypeDef],  # (3)
    TimeToLiveDescription: NotRequired[TimeToLiveDescriptionTypeDef],  # (4)
    SSEDescription: NotRequired[SSEDescriptionTypeDef],  # (5)
```

1. See [:material-code-braces: LocalSecondaryIndexInfoTypeDef](./type_defs.md#localsecondaryindexinfotypedef) 
2. See [:material-code-braces: GlobalSecondaryIndexInfoTypeDef](./type_defs.md#globalsecondaryindexinfotypedef) 
3. See [:material-code-braces: StreamSpecificationTypeDef](./type_defs.md#streamspecificationtypedef) 
4. See [:material-code-braces: TimeToLiveDescriptionTypeDef](./type_defs.md#timetolivedescriptiontypedef) 
5. See [:material-code-braces: SSEDescriptionTypeDef](./type_defs.md#ssedescriptiontypedef) 
## CreateGlobalSecondaryIndexActionTypeDef

```python
# CreateGlobalSecondaryIndexActionTypeDef definition

class CreateGlobalSecondaryIndexActionTypeDef(TypedDict):
    IndexName: str,
    KeySchema: Sequence[KeySchemaElementTypeDef],  # (1)
    Projection: ProjectionUnionTypeDef,  # (2)
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (3)
    OnDemandThroughput: NotRequired[OnDemandThroughputTypeDef],  # (4)
```

1. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
2. See [:material-code-braces: ProjectionTypeDef](./type_defs.md#projectiontypedef) [:material-code-braces: ProjectionOutputTypeDef](./type_defs.md#projectionoutputtypedef) 
3. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
4. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
## LocalSecondaryIndexTypeDef

```python
# LocalSecondaryIndexTypeDef definition

class LocalSecondaryIndexTypeDef(TypedDict):
    IndexName: str,
    KeySchema: Sequence[KeySchemaElementTypeDef],  # (1)
    Projection: ProjectionUnionTypeDef,  # (2)
```

1. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
2. See [:material-code-braces: ProjectionTypeDef](./type_defs.md#projectiontypedef) [:material-code-braces: ProjectionOutputTypeDef](./type_defs.md#projectionoutputtypedef) 
## ListImportsOutputTypeDef

```python
# ListImportsOutputTypeDef definition

class ListImportsOutputTypeDef(TypedDict):
    ImportSummaryList: List[ImportSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ImportSummaryTypeDef](./type_defs.md#importsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchExecuteStatementOutputTypeDef

```python
# BatchExecuteStatementOutputTypeDef definition

class BatchExecuteStatementOutputTypeDef(TypedDict):
    Responses: List[BatchStatementResponseTypeDef],  # (1)
    ConsumedCapacity: List[ConsumedCapacityTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchStatementResponseTypeDef](./type_defs.md#batchstatementresponsetypedef) 
2. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchWriteItemOutputTypeDef

```python
# BatchWriteItemOutputTypeDef definition

class BatchWriteItemOutputTypeDef(TypedDict):
    UnprocessedItems: Dict[str, List[WriteRequestOutputTypeDef]],  # (1)
    ItemCollectionMetrics: Dict[str, List[ItemCollectionMetricsTypeDef]],  # (2)
    ConsumedCapacity: List[ConsumedCapacityTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: WriteRequestOutputTypeDef](./type_defs.md#writerequestoutputtypedef) 
2. See [:material-code-braces: ItemCollectionMetricsTypeDef](./type_defs.md#itemcollectionmetricstypedef) 
3. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchExecuteStatementInputRequestTypeDef

```python
# BatchExecuteStatementInputRequestTypeDef definition

class BatchExecuteStatementInputRequestTypeDef(TypedDict):
    Statements: Sequence[BatchStatementRequestTypeDef],  # (1)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (2)
```

1. See [:material-code-braces: BatchStatementRequestTypeDef](./type_defs.md#batchstatementrequesttypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
## QueryInputQueryPaginateTypeDef

```python
# QueryInputQueryPaginateTypeDef definition

class QueryInputQueryPaginateTypeDef(TypedDict):
    TableName: str,
    IndexName: NotRequired[str],
    Select: NotRequired[SelectType],  # (1)
    AttributesToGet: NotRequired[Sequence[str]],
    ConsistentRead: NotRequired[bool],
    KeyConditions: NotRequired[Mapping[str, ConditionTypeDef]],  # (2)
    QueryFilter: NotRequired[Mapping[str, ConditionTypeDef]],  # (2)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (4)
    ScanIndexForward: NotRequired[bool],
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (5)
    ProjectionExpression: NotRequired[str],
    FilterExpression: NotRequired[str],
    KeyConditionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, UniversalAttributeValueTypeDef]],  # (6)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (7)
```

1. See [:material-code-brackets: SelectType](./literals.md#selecttype) 
2. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
3. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
4. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
5. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
6. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
7. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## QueryInputRequestTypeDef

```python
# QueryInputRequestTypeDef definition

class QueryInputRequestTypeDef(TypedDict):
    TableName: str,
    IndexName: NotRequired[str],
    Select: NotRequired[SelectType],  # (1)
    AttributesToGet: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
    ConsistentRead: NotRequired[bool],
    KeyConditions: NotRequired[Mapping[str, ConditionTypeDef]],  # (2)
    QueryFilter: NotRequired[Mapping[str, ConditionTypeDef]],  # (2)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (4)
    ScanIndexForward: NotRequired[bool],
    ExclusiveStartKey: NotRequired[Mapping[str, UniversalAttributeValueTypeDef]],  # (5)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (6)
    ProjectionExpression: NotRequired[str],
    FilterExpression: NotRequired[str],
    KeyConditionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, UniversalAttributeValueTypeDef]],  # (5)
```

1. See [:material-code-brackets: SelectType](./literals.md#selecttype) 
2. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
3. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
4. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
5. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
6. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
7. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
## ScanInputRequestTypeDef

```python
# ScanInputRequestTypeDef definition

class ScanInputRequestTypeDef(TypedDict):
    TableName: str,
    IndexName: NotRequired[str],
    AttributesToGet: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
    Select: NotRequired[SelectType],  # (1)
    ScanFilter: NotRequired[Mapping[str, ConditionTypeDef]],  # (2)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (3)
    ExclusiveStartKey: NotRequired[Mapping[str, UniversalAttributeValueTypeDef]],  # (4)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (5)
    TotalSegments: NotRequired[int],
    Segment: NotRequired[int],
    ProjectionExpression: NotRequired[str],
    FilterExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, UniversalAttributeValueTypeDef]],  # (4)
    ConsistentRead: NotRequired[bool],
```

1. See [:material-code-brackets: SelectType](./literals.md#selecttype) 
2. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
3. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
4. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
5. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
6. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
## ScanInputScanPaginateTypeDef

```python
# ScanInputScanPaginateTypeDef definition

class ScanInputScanPaginateTypeDef(TypedDict):
    TableName: str,
    IndexName: NotRequired[str],
    AttributesToGet: NotRequired[Sequence[str]],
    Select: NotRequired[SelectType],  # (1)
    ScanFilter: NotRequired[Mapping[str, ConditionTypeDef]],  # (2)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (3)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (4)
    TotalSegments: NotRequired[int],
    Segment: NotRequired[int],
    ProjectionExpression: NotRequired[str],
    FilterExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, UniversalAttributeValueTypeDef]],  # (5)
    ConsistentRead: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (6)
```

1. See [:material-code-brackets: SelectType](./literals.md#selecttype) 
2. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
3. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
4. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
5. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
6. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DeleteItemInputRequestTypeDef

```python
# DeleteItemInputRequestTypeDef definition

class DeleteItemInputRequestTypeDef(TypedDict):
    TableName: str,
    Key: Mapping[str, UniversalAttributeValueTypeDef],  # (1)
    Expected: NotRequired[Mapping[str, ExpectedAttributeValueTypeDef]],  # (2)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (3)
    ReturnValues: NotRequired[ReturnValueType],  # (4)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (5)
    ReturnItemCollectionMetrics: NotRequired[ReturnItemCollectionMetricsType],  # (6)
    ConditionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, UniversalAttributeValueTypeDef]],  # (1)
    ReturnValuesOnConditionCheckFailure: NotRequired[ReturnValuesOnConditionCheckFailureType],  # (8)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: ExpectedAttributeValueTypeDef](./type_defs.md#expectedattributevaluetypedef) 
3. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
4. See [:material-code-brackets: ReturnValueType](./literals.md#returnvaluetype) 
5. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
6. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
7. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
8. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
## PutItemInputRequestTypeDef

```python
# PutItemInputRequestTypeDef definition

class PutItemInputRequestTypeDef(TypedDict):
    TableName: str,
    Item: Mapping[str, UniversalAttributeValueTypeDef],  # (1)
    Expected: NotRequired[Mapping[str, ExpectedAttributeValueTypeDef]],  # (2)
    ReturnValues: NotRequired[ReturnValueType],  # (3)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (4)
    ReturnItemCollectionMetrics: NotRequired[ReturnItemCollectionMetricsType],  # (5)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (6)
    ConditionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, UniversalAttributeValueTypeDef]],  # (1)
    ReturnValuesOnConditionCheckFailure: NotRequired[ReturnValuesOnConditionCheckFailureType],  # (8)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: ExpectedAttributeValueTypeDef](./type_defs.md#expectedattributevaluetypedef) 
3. See [:material-code-brackets: ReturnValueType](./literals.md#returnvaluetype) 
4. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
5. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
6. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
7. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
8. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
## UpdateItemInputRequestTypeDef

```python
# UpdateItemInputRequestTypeDef definition

class UpdateItemInputRequestTypeDef(TypedDict):
    TableName: str,
    Key: Mapping[str, UniversalAttributeValueTypeDef],  # (1)
    AttributeUpdates: NotRequired[Mapping[str, AttributeValueUpdateTypeDef]],  # (2)
    Expected: NotRequired[Mapping[str, ExpectedAttributeValueTypeDef]],  # (3)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (4)
    ReturnValues: NotRequired[ReturnValueType],  # (5)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (6)
    ReturnItemCollectionMetrics: NotRequired[ReturnItemCollectionMetricsType],  # (7)
    UpdateExpression: NotRequired[str],
    ConditionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, UniversalAttributeValueTypeDef]],  # (1)
    ReturnValuesOnConditionCheckFailure: NotRequired[ReturnValuesOnConditionCheckFailureType],  # (9)
```

1. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
2. See [:material-code-braces: AttributeValueUpdateTypeDef](./type_defs.md#attributevalueupdatetypedef) 
3. See [:material-code-braces: ExpectedAttributeValueTypeDef](./type_defs.md#expectedattributevaluetypedef) 
4. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
5. See [:material-code-brackets: ReturnValueType](./literals.md#returnvaluetype) 
6. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
7. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
8. See [:material-code-braces: AttributeValueTypeDef](./type_defs.md#attributevaluetypedef) 
9. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
## TransactGetItemTypeDef

```python
# TransactGetItemTypeDef definition

class TransactGetItemTypeDef(TypedDict):
    Get: GetTypeDef,  # (1)
```

1. See [:material-code-braces: GetTypeDef](./type_defs.md#gettypedef) 
## ExecuteTransactionInputRequestTypeDef

```python
# ExecuteTransactionInputRequestTypeDef definition

class ExecuteTransactionInputRequestTypeDef(TypedDict):
    TransactStatements: Sequence[ParameterizedStatementTypeDef],  # (1)
    ClientRequestToken: NotRequired[str],
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (2)
```

1. See [:material-code-braces: ParameterizedStatementTypeDef](./type_defs.md#parameterizedstatementtypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
## TransactWriteItemTypeDef

```python
# TransactWriteItemTypeDef definition

class TransactWriteItemTypeDef(TypedDict):
    ConditionCheck: NotRequired[ConditionCheckTypeDef],  # (1)
    Put: NotRequired[PutTypeDef],  # (2)
    Delete: NotRequired[DeleteTypeDef],  # (3)
    Update: NotRequired[UpdateTypeDef],  # (4)
```

1. See [:material-code-braces: ConditionCheckTypeDef](./type_defs.md#conditionchecktypedef) 
2. See [:material-code-braces: PutTypeDef](./type_defs.md#puttypedef) 
3. See [:material-code-braces: DeleteTypeDef](./type_defs.md#deletetypedef) 
4. See [:material-code-braces: UpdateTypeDef](./type_defs.md#updatetypedef) 
## BatchGetItemInputServiceResourceBatchGetItemTypeDef

```python
# BatchGetItemInputServiceResourceBatchGetItemTypeDef definition

class BatchGetItemInputServiceResourceBatchGetItemTypeDef(TypedDict):
    RequestItems: Mapping[str, KeysAndAttributesServiceResourceUnionTypeDef],  # (1)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (2)
```

1. See [:material-code-braces: KeysAndAttributesServiceResourceTypeDef](./type_defs.md#keysandattributesserviceresourcetypedef) [:material-code-braces: KeysAndAttributesServiceResourceOutputTypeDef](./type_defs.md#keysandattributesserviceresourceoutputtypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
## BatchWriteItemOutputServiceResourceTypeDef

```python
# BatchWriteItemOutputServiceResourceTypeDef definition

class BatchWriteItemOutputServiceResourceTypeDef(TypedDict):
    UnprocessedItems: Dict[str, List[WriteRequestServiceResourceOutputTypeDef]],  # (1)
    ItemCollectionMetrics: Dict[str, List[ItemCollectionMetricsServiceResourceTypeDef]],  # (2)
    ConsumedCapacity: List[ConsumedCapacityTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: WriteRequestServiceResourceOutputTypeDef](./type_defs.md#writerequestserviceresourceoutputtypedef) 
2. See [:material-code-braces: ItemCollectionMetricsServiceResourceTypeDef](./type_defs.md#itemcollectionmetricsserviceresourcetypedef) 
3. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WriteRequestServiceResourceTypeDef

```python
# WriteRequestServiceResourceTypeDef definition

class WriteRequestServiceResourceTypeDef(TypedDict):
    PutRequest: NotRequired[PutRequestServiceResourceUnionTypeDef],  # (1)
    DeleteRequest: NotRequired[DeleteRequestServiceResourceUnionTypeDef],  # (2)
```

1. See [:material-code-braces: PutRequestServiceResourceTypeDef](./type_defs.md#putrequestserviceresourcetypedef) [:material-code-braces: PutRequestServiceResourceOutputTypeDef](./type_defs.md#putrequestserviceresourceoutputtypedef) 
2. See [:material-code-braces: DeleteRequestServiceResourceTypeDef](./type_defs.md#deleterequestserviceresourcetypedef) [:material-code-braces: DeleteRequestServiceResourceOutputTypeDef](./type_defs.md#deleterequestserviceresourceoutputtypedef) 
## ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef

```python
# ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef definition

class ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef(TypedDict):
    IndexName: NotRequired[str],
    IndexStatus: NotRequired[IndexStatusType],  # (1)
    ProvisionedReadCapacityAutoScalingSettings: NotRequired[AutoScalingSettingsDescriptionTypeDef],  # (2)
    ProvisionedWriteCapacityAutoScalingSettings: NotRequired[AutoScalingSettingsDescriptionTypeDef],  # (2)
```

1. See [:material-code-brackets: IndexStatusType](./literals.md#indexstatustype) 
2. See [:material-code-braces: AutoScalingSettingsDescriptionTypeDef](./type_defs.md#autoscalingsettingsdescriptiontypedef) 
3. See [:material-code-braces: AutoScalingSettingsDescriptionTypeDef](./type_defs.md#autoscalingsettingsdescriptiontypedef) 
## ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef

```python
# ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef definition

class ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef(TypedDict):
    IndexName: str,
    IndexStatus: NotRequired[IndexStatusType],  # (1)
    ProvisionedReadCapacityUnits: NotRequired[int],
    ProvisionedReadCapacityAutoScalingSettings: NotRequired[AutoScalingSettingsDescriptionTypeDef],  # (2)
    ProvisionedWriteCapacityUnits: NotRequired[int],
    ProvisionedWriteCapacityAutoScalingSettings: NotRequired[AutoScalingSettingsDescriptionTypeDef],  # (2)
```

1. See [:material-code-brackets: IndexStatusType](./literals.md#indexstatustype) 
2. See [:material-code-braces: AutoScalingSettingsDescriptionTypeDef](./type_defs.md#autoscalingsettingsdescriptiontypedef) 
3. See [:material-code-braces: AutoScalingSettingsDescriptionTypeDef](./type_defs.md#autoscalingsettingsdescriptiontypedef) 
## GlobalSecondaryIndexAutoScalingUpdateTypeDef

```python
# GlobalSecondaryIndexAutoScalingUpdateTypeDef definition

class GlobalSecondaryIndexAutoScalingUpdateTypeDef(TypedDict):
    IndexName: NotRequired[str],
    ProvisionedWriteCapacityAutoScalingUpdate: NotRequired[AutoScalingSettingsUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: AutoScalingSettingsUpdateTypeDef](./type_defs.md#autoscalingsettingsupdatetypedef) 
## GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef

```python
# GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef definition

class GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef(TypedDict):
    IndexName: str,
    ProvisionedWriteCapacityUnits: NotRequired[int],
    ProvisionedWriteCapacityAutoScalingSettingsUpdate: NotRequired[AutoScalingSettingsUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: AutoScalingSettingsUpdateTypeDef](./type_defs.md#autoscalingsettingsupdatetypedef) 
## ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef

```python
# ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef definition

class ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef(TypedDict):
    IndexName: NotRequired[str],
    ProvisionedReadCapacityAutoScalingUpdate: NotRequired[AutoScalingSettingsUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: AutoScalingSettingsUpdateTypeDef](./type_defs.md#autoscalingsettingsupdatetypedef) 
## ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef

```python
# ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef definition

class ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef(TypedDict):
    IndexName: str,
    ProvisionedReadCapacityUnits: NotRequired[int],
    ProvisionedReadCapacityAutoScalingSettingsUpdate: NotRequired[AutoScalingSettingsUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: AutoScalingSettingsUpdateTypeDef](./type_defs.md#autoscalingsettingsupdatetypedef) 
## GlobalTableDescriptionTypeDef

```python
# GlobalTableDescriptionTypeDef definition

class GlobalTableDescriptionTypeDef(TypedDict):
    ReplicationGroup: NotRequired[List[ReplicaDescriptionTypeDef]],  # (1)
    GlobalTableArn: NotRequired[str],
    CreationDateTime: NotRequired[datetime],
    GlobalTableStatus: NotRequired[GlobalTableStatusType],  # (2)
    GlobalTableName: NotRequired[str],
```

1. See [:material-code-braces: ReplicaDescriptionTypeDef](./type_defs.md#replicadescriptiontypedef) 
2. See [:material-code-brackets: GlobalTableStatusType](./literals.md#globaltablestatustype) 
## TableDescriptionTypeDef

```python
# TableDescriptionTypeDef definition

class TableDescriptionTypeDef(TypedDict):
    AttributeDefinitions: NotRequired[List[AttributeDefinitionTypeDef]],  # (1)
    TableName: NotRequired[str],
    KeySchema: NotRequired[List[KeySchemaElementTypeDef]],  # (2)
    TableStatus: NotRequired[TableStatusType],  # (3)
    CreationDateTime: NotRequired[datetime],
    ProvisionedThroughput: NotRequired[ProvisionedThroughputDescriptionTypeDef],  # (4)
    TableSizeBytes: NotRequired[int],
    ItemCount: NotRequired[int],
    TableArn: NotRequired[str],
    TableId: NotRequired[str],
    BillingModeSummary: NotRequired[BillingModeSummaryTypeDef],  # (5)
    LocalSecondaryIndexes: NotRequired[List[LocalSecondaryIndexDescriptionTypeDef]],  # (6)
    GlobalSecondaryIndexes: NotRequired[List[GlobalSecondaryIndexDescriptionTypeDef]],  # (7)
    StreamSpecification: NotRequired[StreamSpecificationTypeDef],  # (8)
    LatestStreamLabel: NotRequired[str],
    LatestStreamArn: NotRequired[str],
    GlobalTableVersion: NotRequired[str],
    Replicas: NotRequired[List[ReplicaDescriptionTypeDef]],  # (9)
    RestoreSummary: NotRequired[RestoreSummaryTypeDef],  # (10)
    SSEDescription: NotRequired[SSEDescriptionTypeDef],  # (11)
    ArchivalSummary: NotRequired[ArchivalSummaryTypeDef],  # (12)
    TableClassSummary: NotRequired[TableClassSummaryTypeDef],  # (13)
    DeletionProtectionEnabled: NotRequired[bool],
    OnDemandThroughput: NotRequired[OnDemandThroughputTypeDef],  # (14)
```

1. See [:material-code-braces: AttributeDefinitionTypeDef](./type_defs.md#attributedefinitiontypedef) 
2. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
3. See [:material-code-brackets: TableStatusType](./literals.md#tablestatustype) 
4. See [:material-code-braces: ProvisionedThroughputDescriptionTypeDef](./type_defs.md#provisionedthroughputdescriptiontypedef) 
5. See [:material-code-braces: BillingModeSummaryTypeDef](./type_defs.md#billingmodesummarytypedef) 
6. See [:material-code-braces: LocalSecondaryIndexDescriptionTypeDef](./type_defs.md#localsecondaryindexdescriptiontypedef) 
7. See [:material-code-braces: GlobalSecondaryIndexDescriptionTypeDef](./type_defs.md#globalsecondaryindexdescriptiontypedef) 
8. See [:material-code-braces: StreamSpecificationTypeDef](./type_defs.md#streamspecificationtypedef) 
9. See [:material-code-braces: ReplicaDescriptionTypeDef](./type_defs.md#replicadescriptiontypedef) 
10. See [:material-code-braces: RestoreSummaryTypeDef](./type_defs.md#restoresummarytypedef) 
11. See [:material-code-braces: SSEDescriptionTypeDef](./type_defs.md#ssedescriptiontypedef) 
12. See [:material-code-braces: ArchivalSummaryTypeDef](./type_defs.md#archivalsummarytypedef) 
13. See [:material-code-braces: TableClassSummaryTypeDef](./type_defs.md#tableclasssummarytypedef) 
14. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
## ReplicationGroupUpdateTypeDef

```python
# ReplicationGroupUpdateTypeDef definition

class ReplicationGroupUpdateTypeDef(TypedDict):
    Create: NotRequired[CreateReplicationGroupMemberActionTypeDef],  # (1)
    Update: NotRequired[UpdateReplicationGroupMemberActionTypeDef],  # (2)
    Delete: NotRequired[DeleteReplicationGroupMemberActionTypeDef],  # (3)
```

1. See [:material-code-braces: CreateReplicationGroupMemberActionTypeDef](./type_defs.md#createreplicationgroupmemberactiontypedef) 
2. See [:material-code-braces: UpdateReplicationGroupMemberActionTypeDef](./type_defs.md#updatereplicationgroupmemberactiontypedef) 
3. See [:material-code-braces: DeleteReplicationGroupMemberActionTypeDef](./type_defs.md#deletereplicationgroupmemberactiontypedef) 
## ImportTableDescriptionTypeDef

```python
# ImportTableDescriptionTypeDef definition

class ImportTableDescriptionTypeDef(TypedDict):
    ImportArn: NotRequired[str],
    ImportStatus: NotRequired[ImportStatusType],  # (1)
    TableArn: NotRequired[str],
    TableId: NotRequired[str],
    ClientToken: NotRequired[str],
    S3BucketSource: NotRequired[S3BucketSourceTypeDef],  # (2)
    ErrorCount: NotRequired[int],
    CloudWatchLogGroupArn: NotRequired[str],
    InputFormat: NotRequired[InputFormatType],  # (3)
    InputFormatOptions: NotRequired[InputFormatOptionsOutputTypeDef],  # (4)
    InputCompressionType: NotRequired[InputCompressionTypeType],  # (5)
    TableCreationParameters: NotRequired[TableCreationParametersOutputTypeDef],  # (6)
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    ProcessedSizeBytes: NotRequired[int],
    ProcessedItemCount: NotRequired[int],
    ImportedItemCount: NotRequired[int],
    FailureCode: NotRequired[str],
    FailureMessage: NotRequired[str],
```

1. See [:material-code-brackets: ImportStatusType](./literals.md#importstatustype) 
2. See [:material-code-braces: S3BucketSourceTypeDef](./type_defs.md#s3bucketsourcetypedef) 
3. See [:material-code-brackets: InputFormatType](./literals.md#inputformattype) 
4. See [:material-code-braces: InputFormatOptionsOutputTypeDef](./type_defs.md#inputformatoptionsoutputtypedef) 
5. See [:material-code-brackets: InputCompressionTypeType](./literals.md#inputcompressiontypetype) 
6. See [:material-code-braces: TableCreationParametersOutputTypeDef](./type_defs.md#tablecreationparametersoutputtypedef) 
## BackupDescriptionTypeDef

```python
# BackupDescriptionTypeDef definition

class BackupDescriptionTypeDef(TypedDict):
    BackupDetails: NotRequired[BackupDetailsTypeDef],  # (1)
    SourceTableDetails: NotRequired[SourceTableDetailsTypeDef],  # (2)
    SourceTableFeatureDetails: NotRequired[SourceTableFeatureDetailsTypeDef],  # (3)
```

1. See [:material-code-braces: BackupDetailsTypeDef](./type_defs.md#backupdetailstypedef) 
2. See [:material-code-braces: SourceTableDetailsTypeDef](./type_defs.md#sourcetabledetailstypedef) 
3. See [:material-code-braces: SourceTableFeatureDetailsTypeDef](./type_defs.md#sourcetablefeaturedetailstypedef) 
## TableCreationParametersTypeDef

```python
# TableCreationParametersTypeDef definition

class TableCreationParametersTypeDef(TypedDict):
    TableName: str,
    AttributeDefinitions: Sequence[AttributeDefinitionTypeDef],  # (1)
    KeySchema: Sequence[KeySchemaElementTypeDef],  # (2)
    BillingMode: NotRequired[BillingModeType],  # (3)
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (4)
    OnDemandThroughput: NotRequired[OnDemandThroughputTypeDef],  # (5)
    SSESpecification: NotRequired[SSESpecificationTypeDef],  # (6)
    GlobalSecondaryIndexes: NotRequired[Sequence[GlobalSecondaryIndexUnionTypeDef]],  # (7)
```

1. See [:material-code-braces: AttributeDefinitionTypeDef](./type_defs.md#attributedefinitiontypedef) 
2. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
3. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
4. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
5. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
6. See [:material-code-braces: SSESpecificationTypeDef](./type_defs.md#ssespecificationtypedef) 
7. See [:material-code-braces: GlobalSecondaryIndexTypeDef](./type_defs.md#globalsecondaryindextypedef) [:material-code-braces: GlobalSecondaryIndexOutputTypeDef](./type_defs.md#globalsecondaryindexoutputtypedef) 
## GlobalSecondaryIndexUpdateTypeDef

```python
# GlobalSecondaryIndexUpdateTypeDef definition

class GlobalSecondaryIndexUpdateTypeDef(TypedDict):
    Update: NotRequired[UpdateGlobalSecondaryIndexActionTypeDef],  # (1)
    Create: NotRequired[CreateGlobalSecondaryIndexActionTypeDef],  # (2)
    Delete: NotRequired[DeleteGlobalSecondaryIndexActionTypeDef],  # (3)
```

1. See [:material-code-braces: UpdateGlobalSecondaryIndexActionTypeDef](./type_defs.md#updateglobalsecondaryindexactiontypedef) 
2. See [:material-code-braces: CreateGlobalSecondaryIndexActionTypeDef](./type_defs.md#createglobalsecondaryindexactiontypedef) 
3. See [:material-code-braces: DeleteGlobalSecondaryIndexActionTypeDef](./type_defs.md#deleteglobalsecondaryindexactiontypedef) 
## CreateTableInputRequestTypeDef

```python
# CreateTableInputRequestTypeDef definition

class CreateTableInputRequestTypeDef(TypedDict):
    AttributeDefinitions: Sequence[AttributeDefinitionTypeDef],  # (1)
    TableName: str,
    KeySchema: Sequence[KeySchemaElementTypeDef],  # (2)
    LocalSecondaryIndexes: NotRequired[Sequence[LocalSecondaryIndexTypeDef]],  # (3)
    GlobalSecondaryIndexes: NotRequired[Sequence[GlobalSecondaryIndexUnionTypeDef]],  # (4)
    BillingMode: NotRequired[BillingModeType],  # (5)
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (6)
    StreamSpecification: NotRequired[StreamSpecificationTypeDef],  # (7)
    SSESpecification: NotRequired[SSESpecificationTypeDef],  # (8)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (9)
    TableClass: NotRequired[TableClassType],  # (10)
    DeletionProtectionEnabled: NotRequired[bool],
    ResourcePolicy: NotRequired[str],
    OnDemandThroughput: NotRequired[OnDemandThroughputTypeDef],  # (11)
```

1. See [:material-code-braces: AttributeDefinitionTypeDef](./type_defs.md#attributedefinitiontypedef) 
2. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
3. See [:material-code-braces: LocalSecondaryIndexTypeDef](./type_defs.md#localsecondaryindextypedef) 
4. See [:material-code-braces: GlobalSecondaryIndexTypeDef](./type_defs.md#globalsecondaryindextypedef) [:material-code-braces: GlobalSecondaryIndexOutputTypeDef](./type_defs.md#globalsecondaryindexoutputtypedef) 
5. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
6. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
7. See [:material-code-braces: StreamSpecificationTypeDef](./type_defs.md#streamspecificationtypedef) 
8. See [:material-code-braces: SSESpecificationTypeDef](./type_defs.md#ssespecificationtypedef) 
9. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
10. See [:material-code-brackets: TableClassType](./literals.md#tableclasstype) 
11. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
## CreateTableInputServiceResourceCreateTableTypeDef

```python
# CreateTableInputServiceResourceCreateTableTypeDef definition

class CreateTableInputServiceResourceCreateTableTypeDef(TypedDict):
    AttributeDefinitions: Sequence[AttributeDefinitionTypeDef],  # (1)
    TableName: str,
    KeySchema: Sequence[KeySchemaElementTypeDef],  # (2)
    LocalSecondaryIndexes: NotRequired[Sequence[LocalSecondaryIndexTypeDef]],  # (3)
    GlobalSecondaryIndexes: NotRequired[Sequence[GlobalSecondaryIndexTypeDef]],  # (4)
    BillingMode: NotRequired[BillingModeType],  # (5)
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (6)
    StreamSpecification: NotRequired[StreamSpecificationTypeDef],  # (7)
    SSESpecification: NotRequired[SSESpecificationTypeDef],  # (8)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (9)
    TableClass: NotRequired[TableClassType],  # (10)
    DeletionProtectionEnabled: NotRequired[bool],
    ResourcePolicy: NotRequired[str],
    OnDemandThroughput: NotRequired[OnDemandThroughputTypeDef],  # (11)
```

1. See [:material-code-braces: AttributeDefinitionTypeDef](./type_defs.md#attributedefinitiontypedef) 
2. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
3. See [:material-code-braces: LocalSecondaryIndexTypeDef](./type_defs.md#localsecondaryindextypedef) 
4. See [:material-code-braces: GlobalSecondaryIndexTypeDef](./type_defs.md#globalsecondaryindextypedef) 
5. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
6. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
7. See [:material-code-braces: StreamSpecificationTypeDef](./type_defs.md#streamspecificationtypedef) 
8. See [:material-code-braces: SSESpecificationTypeDef](./type_defs.md#ssespecificationtypedef) 
9. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
10. See [:material-code-brackets: TableClassType](./literals.md#tableclasstype) 
11. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
## RestoreTableFromBackupInputRequestTypeDef

```python
# RestoreTableFromBackupInputRequestTypeDef definition

class RestoreTableFromBackupInputRequestTypeDef(TypedDict):
    TargetTableName: str,
    BackupArn: str,
    BillingModeOverride: NotRequired[BillingModeType],  # (1)
    GlobalSecondaryIndexOverride: NotRequired[Sequence[GlobalSecondaryIndexTypeDef]],  # (2)
    LocalSecondaryIndexOverride: NotRequired[Sequence[LocalSecondaryIndexTypeDef]],  # (3)
    ProvisionedThroughputOverride: NotRequired[ProvisionedThroughputTypeDef],  # (4)
    OnDemandThroughputOverride: NotRequired[OnDemandThroughputTypeDef],  # (5)
    SSESpecificationOverride: NotRequired[SSESpecificationTypeDef],  # (6)
```

1. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
2. See [:material-code-braces: GlobalSecondaryIndexTypeDef](./type_defs.md#globalsecondaryindextypedef) 
3. See [:material-code-braces: LocalSecondaryIndexTypeDef](./type_defs.md#localsecondaryindextypedef) 
4. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
5. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
6. See [:material-code-braces: SSESpecificationTypeDef](./type_defs.md#ssespecificationtypedef) 
## RestoreTableToPointInTimeInputRequestTypeDef

```python
# RestoreTableToPointInTimeInputRequestTypeDef definition

class RestoreTableToPointInTimeInputRequestTypeDef(TypedDict):
    TargetTableName: str,
    SourceTableArn: NotRequired[str],
    SourceTableName: NotRequired[str],
    UseLatestRestorableTime: NotRequired[bool],
    RestoreDateTime: NotRequired[TimestampTypeDef],
    BillingModeOverride: NotRequired[BillingModeType],  # (1)
    GlobalSecondaryIndexOverride: NotRequired[Sequence[GlobalSecondaryIndexTypeDef]],  # (2)
    LocalSecondaryIndexOverride: NotRequired[Sequence[LocalSecondaryIndexTypeDef]],  # (3)
    ProvisionedThroughputOverride: NotRequired[ProvisionedThroughputTypeDef],  # (4)
    OnDemandThroughputOverride: NotRequired[OnDemandThroughputTypeDef],  # (5)
    SSESpecificationOverride: NotRequired[SSESpecificationTypeDef],  # (6)
```

1. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
2. See [:material-code-braces: GlobalSecondaryIndexTypeDef](./type_defs.md#globalsecondaryindextypedef) 
3. See [:material-code-braces: LocalSecondaryIndexTypeDef](./type_defs.md#localsecondaryindextypedef) 
4. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
5. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
6. See [:material-code-braces: SSESpecificationTypeDef](./type_defs.md#ssespecificationtypedef) 
## TransactGetItemsInputRequestTypeDef

```python
# TransactGetItemsInputRequestTypeDef definition

class TransactGetItemsInputRequestTypeDef(TypedDict):
    TransactItems: Sequence[TransactGetItemTypeDef],  # (1)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (2)
```

1. See [:material-code-braces: TransactGetItemTypeDef](./type_defs.md#transactgetitemtypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
## BatchGetItemInputRequestTypeDef

```python
# BatchGetItemInputRequestTypeDef definition

class BatchGetItemInputRequestTypeDef(TypedDict):
    RequestItems: Mapping[str, KeysAndAttributesUnionTypeDef],  # (1)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (2)
```

1. See [:material-code-braces: KeysAndAttributesTypeDef](./type_defs.md#keysandattributestypedef) [:material-code-braces: KeysAndAttributesOutputTypeDef](./type_defs.md#keysandattributesoutputtypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
## WriteRequestTypeDef

```python
# WriteRequestTypeDef definition

class WriteRequestTypeDef(TypedDict):
    PutRequest: NotRequired[PutRequestUnionTypeDef],  # (1)
    DeleteRequest: NotRequired[DeleteRequestUnionTypeDef],  # (2)
```

1. See [:material-code-braces: PutRequestTypeDef](./type_defs.md#putrequesttypedef) [:material-code-braces: PutRequestOutputTypeDef](./type_defs.md#putrequestoutputtypedef) 
2. See [:material-code-braces: DeleteRequestTypeDef](./type_defs.md#deleterequesttypedef) [:material-code-braces: DeleteRequestOutputTypeDef](./type_defs.md#deleterequestoutputtypedef) 
## TransactWriteItemsInputRequestTypeDef

```python
# TransactWriteItemsInputRequestTypeDef definition

class TransactWriteItemsInputRequestTypeDef(TypedDict):
    TransactItems: Sequence[TransactWriteItemTypeDef],  # (1)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (2)
    ReturnItemCollectionMetrics: NotRequired[ReturnItemCollectionMetricsType],  # (3)
    ClientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: TransactWriteItemTypeDef](./type_defs.md#transactwriteitemtypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
3. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
## ReplicaAutoScalingDescriptionTypeDef

```python
# ReplicaAutoScalingDescriptionTypeDef definition

class ReplicaAutoScalingDescriptionTypeDef(TypedDict):
    RegionName: NotRequired[str],
    GlobalSecondaryIndexes: NotRequired[List[ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef]],  # (1)
    ReplicaProvisionedReadCapacityAutoScalingSettings: NotRequired[AutoScalingSettingsDescriptionTypeDef],  # (2)
    ReplicaProvisionedWriteCapacityAutoScalingSettings: NotRequired[AutoScalingSettingsDescriptionTypeDef],  # (2)
    ReplicaStatus: NotRequired[ReplicaStatusType],  # (4)
```

1. See [:material-code-braces: ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef](./type_defs.md#replicaglobalsecondaryindexautoscalingdescriptiontypedef) 
2. See [:material-code-braces: AutoScalingSettingsDescriptionTypeDef](./type_defs.md#autoscalingsettingsdescriptiontypedef) 
3. See [:material-code-braces: AutoScalingSettingsDescriptionTypeDef](./type_defs.md#autoscalingsettingsdescriptiontypedef) 
4. See [:material-code-brackets: ReplicaStatusType](./literals.md#replicastatustype) 
## ReplicaSettingsDescriptionTypeDef

```python
# ReplicaSettingsDescriptionTypeDef definition

class ReplicaSettingsDescriptionTypeDef(TypedDict):
    RegionName: str,
    ReplicaStatus: NotRequired[ReplicaStatusType],  # (1)
    ReplicaBillingModeSummary: NotRequired[BillingModeSummaryTypeDef],  # (2)
    ReplicaProvisionedReadCapacityUnits: NotRequired[int],
    ReplicaProvisionedReadCapacityAutoScalingSettings: NotRequired[AutoScalingSettingsDescriptionTypeDef],  # (3)
    ReplicaProvisionedWriteCapacityUnits: NotRequired[int],
    ReplicaProvisionedWriteCapacityAutoScalingSettings: NotRequired[AutoScalingSettingsDescriptionTypeDef],  # (3)
    ReplicaGlobalSecondaryIndexSettings: NotRequired[List[ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef]],  # (5)
    ReplicaTableClassSummary: NotRequired[TableClassSummaryTypeDef],  # (6)
```

1. See [:material-code-brackets: ReplicaStatusType](./literals.md#replicastatustype) 
2. See [:material-code-braces: BillingModeSummaryTypeDef](./type_defs.md#billingmodesummarytypedef) 
3. See [:material-code-braces: AutoScalingSettingsDescriptionTypeDef](./type_defs.md#autoscalingsettingsdescriptiontypedef) 
4. See [:material-code-braces: AutoScalingSettingsDescriptionTypeDef](./type_defs.md#autoscalingsettingsdescriptiontypedef) 
5. See [:material-code-braces: ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef](./type_defs.md#replicaglobalsecondaryindexsettingsdescriptiontypedef) 
6. See [:material-code-braces: TableClassSummaryTypeDef](./type_defs.md#tableclasssummarytypedef) 
## ReplicaAutoScalingUpdateTypeDef

```python
# ReplicaAutoScalingUpdateTypeDef definition

class ReplicaAutoScalingUpdateTypeDef(TypedDict):
    RegionName: str,
    ReplicaGlobalSecondaryIndexUpdates: NotRequired[Sequence[ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef]],  # (1)
    ReplicaProvisionedReadCapacityAutoScalingUpdate: NotRequired[AutoScalingSettingsUpdateTypeDef],  # (2)
```

1. See [:material-code-braces: ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef](./type_defs.md#replicaglobalsecondaryindexautoscalingupdatetypedef) 
2. See [:material-code-braces: AutoScalingSettingsUpdateTypeDef](./type_defs.md#autoscalingsettingsupdatetypedef) 
## ReplicaSettingsUpdateTypeDef

```python
# ReplicaSettingsUpdateTypeDef definition

class ReplicaSettingsUpdateTypeDef(TypedDict):
    RegionName: str,
    ReplicaProvisionedReadCapacityUnits: NotRequired[int],
    ReplicaProvisionedReadCapacityAutoScalingSettingsUpdate: NotRequired[AutoScalingSettingsUpdateTypeDef],  # (1)
    ReplicaGlobalSecondaryIndexSettingsUpdate: NotRequired[Sequence[ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef]],  # (2)
    ReplicaTableClass: NotRequired[TableClassType],  # (3)
```

1. See [:material-code-braces: AutoScalingSettingsUpdateTypeDef](./type_defs.md#autoscalingsettingsupdatetypedef) 
2. See [:material-code-braces: ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef](./type_defs.md#replicaglobalsecondaryindexsettingsupdatetypedef) 
3. See [:material-code-brackets: TableClassType](./literals.md#tableclasstype) 
## CreateGlobalTableOutputTypeDef

```python
# CreateGlobalTableOutputTypeDef definition

class CreateGlobalTableOutputTypeDef(TypedDict):
    GlobalTableDescription: GlobalTableDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GlobalTableDescriptionTypeDef](./type_defs.md#globaltabledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeGlobalTableOutputTypeDef

```python
# DescribeGlobalTableOutputTypeDef definition

class DescribeGlobalTableOutputTypeDef(TypedDict):
    GlobalTableDescription: GlobalTableDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GlobalTableDescriptionTypeDef](./type_defs.md#globaltabledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGlobalTableOutputTypeDef

```python
# UpdateGlobalTableOutputTypeDef definition

class UpdateGlobalTableOutputTypeDef(TypedDict):
    GlobalTableDescription: GlobalTableDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GlobalTableDescriptionTypeDef](./type_defs.md#globaltabledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTableOutputTypeDef

```python
# CreateTableOutputTypeDef definition

class CreateTableOutputTypeDef(TypedDict):
    TableDescription: TableDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableDescriptionTypeDef](./type_defs.md#tabledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteTableOutputTypeDef

```python
# DeleteTableOutputTypeDef definition

class DeleteTableOutputTypeDef(TypedDict):
    TableDescription: TableDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableDescriptionTypeDef](./type_defs.md#tabledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTableOutputTypeDef

```python
# DescribeTableOutputTypeDef definition

class DescribeTableOutputTypeDef(TypedDict):
    Table: TableDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableDescriptionTypeDef](./type_defs.md#tabledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreTableFromBackupOutputTypeDef

```python
# RestoreTableFromBackupOutputTypeDef definition

class RestoreTableFromBackupOutputTypeDef(TypedDict):
    TableDescription: TableDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableDescriptionTypeDef](./type_defs.md#tabledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreTableToPointInTimeOutputTypeDef

```python
# RestoreTableToPointInTimeOutputTypeDef definition

class RestoreTableToPointInTimeOutputTypeDef(TypedDict):
    TableDescription: TableDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableDescriptionTypeDef](./type_defs.md#tabledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTableOutputTypeDef

```python
# UpdateTableOutputTypeDef definition

class UpdateTableOutputTypeDef(TypedDict):
    TableDescription: TableDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableDescriptionTypeDef](./type_defs.md#tabledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeImportOutputTypeDef

```python
# DescribeImportOutputTypeDef definition

class DescribeImportOutputTypeDef(TypedDict):
    ImportTableDescription: ImportTableDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImportTableDescriptionTypeDef](./type_defs.md#importtabledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportTableOutputTypeDef

```python
# ImportTableOutputTypeDef definition

class ImportTableOutputTypeDef(TypedDict):
    ImportTableDescription: ImportTableDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImportTableDescriptionTypeDef](./type_defs.md#importtabledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteBackupOutputTypeDef

```python
# DeleteBackupOutputTypeDef definition

class DeleteBackupOutputTypeDef(TypedDict):
    BackupDescription: BackupDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackupDescriptionTypeDef](./type_defs.md#backupdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeBackupOutputTypeDef

```python
# DescribeBackupOutputTypeDef definition

class DescribeBackupOutputTypeDef(TypedDict):
    BackupDescription: BackupDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackupDescriptionTypeDef](./type_defs.md#backupdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportTableInputRequestTypeDef

```python
# ImportTableInputRequestTypeDef definition

class ImportTableInputRequestTypeDef(TypedDict):
    S3BucketSource: S3BucketSourceTypeDef,  # (1)
    InputFormat: InputFormatType,  # (2)
    TableCreationParameters: TableCreationParametersTypeDef,  # (3)
    ClientToken: NotRequired[str],
    InputFormatOptions: NotRequired[InputFormatOptionsTypeDef],  # (4)
    InputCompressionType: NotRequired[InputCompressionTypeType],  # (5)
```

1. See [:material-code-braces: S3BucketSourceTypeDef](./type_defs.md#s3bucketsourcetypedef) 
2. See [:material-code-brackets: InputFormatType](./literals.md#inputformattype) 
3. See [:material-code-braces: TableCreationParametersTypeDef](./type_defs.md#tablecreationparameterstypedef) 
4. See [:material-code-braces: InputFormatOptionsTypeDef](./type_defs.md#inputformatoptionstypedef) 
5. See [:material-code-brackets: InputCompressionTypeType](./literals.md#inputcompressiontypetype) 
## UpdateTableInputRequestTypeDef

```python
# UpdateTableInputRequestTypeDef definition

class UpdateTableInputRequestTypeDef(TypedDict):
    TableName: str,
    AttributeDefinitions: NotRequired[Sequence[AttributeDefinitionTypeDef]],  # (1)
    BillingMode: NotRequired[BillingModeType],  # (2)
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (3)
    GlobalSecondaryIndexUpdates: NotRequired[Sequence[GlobalSecondaryIndexUpdateTypeDef]],  # (4)
    StreamSpecification: NotRequired[StreamSpecificationTypeDef],  # (5)
    SSESpecification: NotRequired[SSESpecificationTypeDef],  # (6)
    ReplicaUpdates: NotRequired[Sequence[ReplicationGroupUpdateTypeDef]],  # (7)
    TableClass: NotRequired[TableClassType],  # (8)
    DeletionProtectionEnabled: NotRequired[bool],
    OnDemandThroughput: NotRequired[OnDemandThroughputTypeDef],  # (9)
```

1. See [:material-code-braces: AttributeDefinitionTypeDef](./type_defs.md#attributedefinitiontypedef) 
2. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
3. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
4. See [:material-code-braces: GlobalSecondaryIndexUpdateTypeDef](./type_defs.md#globalsecondaryindexupdatetypedef) 
5. See [:material-code-braces: StreamSpecificationTypeDef](./type_defs.md#streamspecificationtypedef) 
6. See [:material-code-braces: SSESpecificationTypeDef](./type_defs.md#ssespecificationtypedef) 
7. See [:material-code-braces: ReplicationGroupUpdateTypeDef](./type_defs.md#replicationgroupupdatetypedef) 
8. See [:material-code-brackets: TableClassType](./literals.md#tableclasstype) 
9. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
## UpdateTableInputTableUpdateTypeDef

```python
# UpdateTableInputTableUpdateTypeDef definition

class UpdateTableInputTableUpdateTypeDef(TypedDict):
    AttributeDefinitions: NotRequired[Sequence[AttributeDefinitionTypeDef]],  # (1)
    BillingMode: NotRequired[BillingModeType],  # (2)
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (3)
    GlobalSecondaryIndexUpdates: NotRequired[Sequence[GlobalSecondaryIndexUpdateTypeDef]],  # (4)
    StreamSpecification: NotRequired[StreamSpecificationTypeDef],  # (5)
    SSESpecification: NotRequired[SSESpecificationTypeDef],  # (6)
    ReplicaUpdates: NotRequired[Sequence[ReplicationGroupUpdateTypeDef]],  # (7)
    TableClass: NotRequired[TableClassType],  # (8)
    DeletionProtectionEnabled: NotRequired[bool],
    OnDemandThroughput: NotRequired[OnDemandThroughputTypeDef],  # (9)
```

1. See [:material-code-braces: AttributeDefinitionTypeDef](./type_defs.md#attributedefinitiontypedef) 
2. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
3. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
4. See [:material-code-braces: GlobalSecondaryIndexUpdateTypeDef](./type_defs.md#globalsecondaryindexupdatetypedef) 
5. See [:material-code-braces: StreamSpecificationTypeDef](./type_defs.md#streamspecificationtypedef) 
6. See [:material-code-braces: SSESpecificationTypeDef](./type_defs.md#ssespecificationtypedef) 
7. See [:material-code-braces: ReplicationGroupUpdateTypeDef](./type_defs.md#replicationgroupupdatetypedef) 
8. See [:material-code-brackets: TableClassType](./literals.md#tableclasstype) 
9. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
## BatchWriteItemInputServiceResourceBatchWriteItemTypeDef

```python
# BatchWriteItemInputServiceResourceBatchWriteItemTypeDef definition

class BatchWriteItemInputServiceResourceBatchWriteItemTypeDef(TypedDict):
    RequestItems: Mapping[str, Sequence[WriteRequestServiceResourceUnionTypeDef]],  # (1)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (2)
    ReturnItemCollectionMetrics: NotRequired[ReturnItemCollectionMetricsType],  # (3)
```

1. See [:material-code-braces: WriteRequestServiceResourceTypeDef](./type_defs.md#writerequestserviceresourcetypedef) [:material-code-braces: WriteRequestServiceResourceOutputTypeDef](./type_defs.md#writerequestserviceresourceoutputtypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
3. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
## TableAutoScalingDescriptionTypeDef

```python
# TableAutoScalingDescriptionTypeDef definition

class TableAutoScalingDescriptionTypeDef(TypedDict):
    TableName: NotRequired[str],
    TableStatus: NotRequired[TableStatusType],  # (1)
    Replicas: NotRequired[List[ReplicaAutoScalingDescriptionTypeDef]],  # (2)
```

1. See [:material-code-brackets: TableStatusType](./literals.md#tablestatustype) 
2. See [:material-code-braces: ReplicaAutoScalingDescriptionTypeDef](./type_defs.md#replicaautoscalingdescriptiontypedef) 
## DescribeGlobalTableSettingsOutputTypeDef

```python
# DescribeGlobalTableSettingsOutputTypeDef definition

class DescribeGlobalTableSettingsOutputTypeDef(TypedDict):
    GlobalTableName: str,
    ReplicaSettings: List[ReplicaSettingsDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicaSettingsDescriptionTypeDef](./type_defs.md#replicasettingsdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGlobalTableSettingsOutputTypeDef

```python
# UpdateGlobalTableSettingsOutputTypeDef definition

class UpdateGlobalTableSettingsOutputTypeDef(TypedDict):
    GlobalTableName: str,
    ReplicaSettings: List[ReplicaSettingsDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicaSettingsDescriptionTypeDef](./type_defs.md#replicasettingsdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTableReplicaAutoScalingInputRequestTypeDef

```python
# UpdateTableReplicaAutoScalingInputRequestTypeDef definition

class UpdateTableReplicaAutoScalingInputRequestTypeDef(TypedDict):
    TableName: str,
    GlobalSecondaryIndexUpdates: NotRequired[Sequence[GlobalSecondaryIndexAutoScalingUpdateTypeDef]],  # (1)
    ProvisionedWriteCapacityAutoScalingUpdate: NotRequired[AutoScalingSettingsUpdateTypeDef],  # (2)
    ReplicaUpdates: NotRequired[Sequence[ReplicaAutoScalingUpdateTypeDef]],  # (3)
```

1. See [:material-code-braces: GlobalSecondaryIndexAutoScalingUpdateTypeDef](./type_defs.md#globalsecondaryindexautoscalingupdatetypedef) 
2. See [:material-code-braces: AutoScalingSettingsUpdateTypeDef](./type_defs.md#autoscalingsettingsupdatetypedef) 
3. See [:material-code-braces: ReplicaAutoScalingUpdateTypeDef](./type_defs.md#replicaautoscalingupdatetypedef) 
## UpdateGlobalTableSettingsInputRequestTypeDef

```python
# UpdateGlobalTableSettingsInputRequestTypeDef definition

class UpdateGlobalTableSettingsInputRequestTypeDef(TypedDict):
    GlobalTableName: str,
    GlobalTableBillingMode: NotRequired[BillingModeType],  # (1)
    GlobalTableProvisionedWriteCapacityUnits: NotRequired[int],
    GlobalTableProvisionedWriteCapacityAutoScalingSettingsUpdate: NotRequired[AutoScalingSettingsUpdateTypeDef],  # (2)
    GlobalTableGlobalSecondaryIndexSettingsUpdate: NotRequired[Sequence[GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef]],  # (3)
    ReplicaSettingsUpdate: NotRequired[Sequence[ReplicaSettingsUpdateTypeDef]],  # (4)
```

1. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
2. See [:material-code-braces: AutoScalingSettingsUpdateTypeDef](./type_defs.md#autoscalingsettingsupdatetypedef) 
3. See [:material-code-braces: GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef](./type_defs.md#globaltableglobalsecondaryindexsettingsupdatetypedef) 
4. See [:material-code-braces: ReplicaSettingsUpdateTypeDef](./type_defs.md#replicasettingsupdatetypedef) 
## BatchWriteItemInputRequestTypeDef

```python
# BatchWriteItemInputRequestTypeDef definition

class BatchWriteItemInputRequestTypeDef(TypedDict):
    RequestItems: Mapping[str, Sequence[WriteRequestUnionTypeDef]],  # (1)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (2)
    ReturnItemCollectionMetrics: NotRequired[ReturnItemCollectionMetricsType],  # (3)
```

1. See [:material-code-braces: WriteRequestTypeDef](./type_defs.md#writerequesttypedef) [:material-code-braces: WriteRequestOutputTypeDef](./type_defs.md#writerequestoutputtypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
3. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
## DescribeTableReplicaAutoScalingOutputTypeDef

```python
# DescribeTableReplicaAutoScalingOutputTypeDef definition

class DescribeTableReplicaAutoScalingOutputTypeDef(TypedDict):
    TableAutoScalingDescription: TableAutoScalingDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableAutoScalingDescriptionTypeDef](./type_defs.md#tableautoscalingdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTableReplicaAutoScalingOutputTypeDef

```python
# UpdateTableReplicaAutoScalingOutputTypeDef definition

class UpdateTableReplicaAutoScalingOutputTypeDef(TypedDict):
    TableAutoScalingDescription: TableAutoScalingDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableAutoScalingDescriptionTypeDef](./type_defs.md#tableautoscalingdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
