# Type definitions

> [Index](../README.md) > [CloudTrail](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CloudTrail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
    type annotations stubs module [types-aiobotocore-cloudtrail](https://pypi.org/project/types-aiobotocore-cloudtrail/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: NotRequired[str],
```

## AdvancedFieldSelectorTypeDef

```python
# AdvancedFieldSelectorTypeDef definition

class AdvancedFieldSelectorTypeDef(TypedDict):
    Field: str,
    Equals: NotRequired[Sequence[str]],
    StartsWith: NotRequired[Sequence[str]],
    EndsWith: NotRequired[Sequence[str]],
    NotEquals: NotRequired[Sequence[str]],
    NotStartsWith: NotRequired[Sequence[str]],
    NotEndsWith: NotRequired[Sequence[str]],
```

## CancelQueryRequestRequestTypeDef

```python
# CancelQueryRequestRequestTypeDef definition

class CancelQueryRequestRequestTypeDef(TypedDict):
    QueryId: str,
    EventDataStore: NotRequired[str],
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

## ChannelTypeDef

```python
# ChannelTypeDef definition

class ChannelTypeDef(TypedDict):
    ChannelArn: NotRequired[str],
    Name: NotRequired[str],
```

## DestinationTypeDef

```python
# DestinationTypeDef definition

class DestinationTypeDef(TypedDict):
    Type: DestinationTypeType,  # (1)
    Location: str,
```

1. See [:material-code-brackets: DestinationTypeType](./literals.md#destinationtypetype) 
## DataResourceTypeDef

```python
# DataResourceTypeDef definition

class DataResourceTypeDef(TypedDict):
    Type: NotRequired[str],
    Values: NotRequired[List[str]],
```

## DeleteChannelRequestRequestTypeDef

```python
# DeleteChannelRequestRequestTypeDef definition

class DeleteChannelRequestRequestTypeDef(TypedDict):
    Channel: str,
```

## DeleteEventDataStoreRequestRequestTypeDef

```python
# DeleteEventDataStoreRequestRequestTypeDef definition

class DeleteEventDataStoreRequestRequestTypeDef(TypedDict):
    EventDataStore: str,
```

## DeleteResourcePolicyRequestRequestTypeDef

```python
# DeleteResourcePolicyRequestRequestTypeDef definition

class DeleteResourcePolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## DeleteTrailRequestRequestTypeDef

```python
# DeleteTrailRequestRequestTypeDef definition

class DeleteTrailRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeregisterOrganizationDelegatedAdminRequestRequestTypeDef

```python
# DeregisterOrganizationDelegatedAdminRequestRequestTypeDef definition

class DeregisterOrganizationDelegatedAdminRequestRequestTypeDef(TypedDict):
    DelegatedAdminAccountId: str,
```

## DescribeQueryRequestRequestTypeDef

```python
# DescribeQueryRequestRequestTypeDef definition

class DescribeQueryRequestRequestTypeDef(TypedDict):
    EventDataStore: NotRequired[str],
    QueryId: NotRequired[str],
    QueryAlias: NotRequired[str],
```

## QueryStatisticsForDescribeQueryTypeDef

```python
# QueryStatisticsForDescribeQueryTypeDef definition

class QueryStatisticsForDescribeQueryTypeDef(TypedDict):
    EventsMatched: NotRequired[int],
    EventsScanned: NotRequired[int],
    BytesScanned: NotRequired[int],
    ExecutionTimeInMillis: NotRequired[int],
    CreationTime: NotRequired[datetime],
```

## DescribeTrailsRequestRequestTypeDef

```python
# DescribeTrailsRequestRequestTypeDef definition

class DescribeTrailsRequestRequestTypeDef(TypedDict):
    trailNameList: NotRequired[Sequence[str]],
    includeShadowTrails: NotRequired[bool],
```

## TrailTypeDef

```python
# TrailTypeDef definition

class TrailTypeDef(TypedDict):
    Name: NotRequired[str],
    S3BucketName: NotRequired[str],
    S3KeyPrefix: NotRequired[str],
    SnsTopicName: NotRequired[str],
    SnsTopicARN: NotRequired[str],
    IncludeGlobalServiceEvents: NotRequired[bool],
    IsMultiRegionTrail: NotRequired[bool],
    HomeRegion: NotRequired[str],
    TrailARN: NotRequired[str],
    LogFileValidationEnabled: NotRequired[bool],
    CloudWatchLogsLogGroupArn: NotRequired[str],
    CloudWatchLogsRoleArn: NotRequired[str],
    KmsKeyId: NotRequired[str],
    HasCustomEventSelectors: NotRequired[bool],
    HasInsightSelectors: NotRequired[bool],
    IsOrganizationTrail: NotRequired[bool],
```

## ResourceTypeDef

```python
# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    ResourceType: NotRequired[str],
    ResourceName: NotRequired[str],
```

## GetChannelRequestRequestTypeDef

```python
# GetChannelRequestRequestTypeDef definition

class GetChannelRequestRequestTypeDef(TypedDict):
    Channel: str,
```

## IngestionStatusTypeDef

```python
# IngestionStatusTypeDef definition

class IngestionStatusTypeDef(TypedDict):
    LatestIngestionSuccessTime: NotRequired[datetime],
    LatestIngestionSuccessEventID: NotRequired[str],
    LatestIngestionErrorCode: NotRequired[str],
    LatestIngestionAttemptTime: NotRequired[datetime],
    LatestIngestionAttemptEventID: NotRequired[str],
```

## GetEventDataStoreRequestRequestTypeDef

```python
# GetEventDataStoreRequestRequestTypeDef definition

class GetEventDataStoreRequestRequestTypeDef(TypedDict):
    EventDataStore: str,
```

## GetEventSelectorsRequestRequestTypeDef

```python
# GetEventSelectorsRequestRequestTypeDef definition

class GetEventSelectorsRequestRequestTypeDef(TypedDict):
    TrailName: str,
```

## GetImportRequestRequestTypeDef

```python
# GetImportRequestRequestTypeDef definition

class GetImportRequestRequestTypeDef(TypedDict):
    ImportId: str,
```

## ImportStatisticsTypeDef

```python
# ImportStatisticsTypeDef definition

class ImportStatisticsTypeDef(TypedDict):
    PrefixesFound: NotRequired[int],
    PrefixesCompleted: NotRequired[int],
    FilesCompleted: NotRequired[int],
    EventsCompleted: NotRequired[int],
    FailedEntries: NotRequired[int],
```

## GetInsightSelectorsRequestRequestTypeDef

```python
# GetInsightSelectorsRequestRequestTypeDef definition

class GetInsightSelectorsRequestRequestTypeDef(TypedDict):
    TrailName: str,
```

## InsightSelectorTypeDef

```python
# InsightSelectorTypeDef definition

class InsightSelectorTypeDef(TypedDict):
    InsightType: NotRequired[InsightTypeType],  # (1)
```

1. See [:material-code-brackets: InsightTypeType](./literals.md#insighttypetype) 
## GetQueryResultsRequestRequestTypeDef

```python
# GetQueryResultsRequestRequestTypeDef definition

class GetQueryResultsRequestRequestTypeDef(TypedDict):
    QueryId: str,
    EventDataStore: NotRequired[str],
    NextToken: NotRequired[str],
    MaxQueryResults: NotRequired[int],
```

## QueryStatisticsTypeDef

```python
# QueryStatisticsTypeDef definition

class QueryStatisticsTypeDef(TypedDict):
    ResultsCount: NotRequired[int],
    TotalResultsCount: NotRequired[int],
    BytesScanned: NotRequired[int],
```

## GetResourcePolicyRequestRequestTypeDef

```python
# GetResourcePolicyRequestRequestTypeDef definition

class GetResourcePolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## GetTrailRequestRequestTypeDef

```python
# GetTrailRequestRequestTypeDef definition

class GetTrailRequestRequestTypeDef(TypedDict):
    Name: str,
```

## GetTrailStatusRequestRequestTypeDef

```python
# GetTrailStatusRequestRequestTypeDef definition

class GetTrailStatusRequestRequestTypeDef(TypedDict):
    Name: str,
```

## ImportFailureListItemTypeDef

```python
# ImportFailureListItemTypeDef definition

class ImportFailureListItemTypeDef(TypedDict):
    Location: NotRequired[str],
    Status: NotRequired[ImportFailureStatusType],  # (1)
    ErrorType: NotRequired[str],
    ErrorMessage: NotRequired[str],
    LastUpdatedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ImportFailureStatusType](./literals.md#importfailurestatustype) 
## S3ImportSourceTypeDef

```python
# S3ImportSourceTypeDef definition

class S3ImportSourceTypeDef(TypedDict):
    S3LocationUri: str,
    S3BucketRegion: str,
    S3BucketAccessRoleArn: str,
```

## ImportsListItemTypeDef

```python
# ImportsListItemTypeDef definition

class ImportsListItemTypeDef(TypedDict):
    ImportId: NotRequired[str],
    ImportStatus: NotRequired[ImportStatusType],  # (1)
    Destinations: NotRequired[List[str]],
    CreatedTimestamp: NotRequired[datetime],
    UpdatedTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: ImportStatusType](./literals.md#importstatustype) 
## ListChannelsRequestRequestTypeDef

```python
# ListChannelsRequestRequestTypeDef definition

class ListChannelsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListEventDataStoresRequestRequestTypeDef

```python
# ListEventDataStoresRequestRequestTypeDef definition

class ListEventDataStoresRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListImportFailuresRequestRequestTypeDef

```python
# ListImportFailuresRequestRequestTypeDef definition

class ListImportFailuresRequestRequestTypeDef(TypedDict):
    ImportId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListImportsRequestRequestTypeDef

```python
# ListImportsRequestRequestTypeDef definition

class ListImportsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    Destination: NotRequired[str],
    ImportStatus: NotRequired[ImportStatusType],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ImportStatusType](./literals.md#importstatustype) 
## PublicKeyTypeDef

```python
# PublicKeyTypeDef definition

class PublicKeyTypeDef(TypedDict):
    Value: NotRequired[bytes],
    ValidityStartTime: NotRequired[datetime],
    ValidityEndTime: NotRequired[datetime],
    Fingerprint: NotRequired[str],
```

## QueryTypeDef

```python
# QueryTypeDef definition

class QueryTypeDef(TypedDict):
    QueryId: NotRequired[str],
    QueryStatus: NotRequired[QueryStatusType],  # (1)
    CreationTime: NotRequired[datetime],
```

1. See [:material-code-brackets: QueryStatusType](./literals.md#querystatustype) 
## ListTagsRequestRequestTypeDef

```python
# ListTagsRequestRequestTypeDef definition

class ListTagsRequestRequestTypeDef(TypedDict):
    ResourceIdList: Sequence[str],
    NextToken: NotRequired[str],
```

## ListTrailsRequestRequestTypeDef

```python
# ListTrailsRequestRequestTypeDef definition

class ListTrailsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
```

## TrailInfoTypeDef

```python
# TrailInfoTypeDef definition

class TrailInfoTypeDef(TypedDict):
    TrailARN: NotRequired[str],
    Name: NotRequired[str],
    HomeRegion: NotRequired[str],
```

## LookupAttributeTypeDef

```python
# LookupAttributeTypeDef definition

class LookupAttributeTypeDef(TypedDict):
    AttributeKey: LookupAttributeKeyType,  # (1)
    AttributeValue: str,
```

1. See [:material-code-brackets: LookupAttributeKeyType](./literals.md#lookupattributekeytype) 
## PutResourcePolicyRequestRequestTypeDef

```python
# PutResourcePolicyRequestRequestTypeDef definition

class PutResourcePolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    ResourcePolicy: str,
```

## RegisterOrganizationDelegatedAdminRequestRequestTypeDef

```python
# RegisterOrganizationDelegatedAdminRequestRequestTypeDef definition

class RegisterOrganizationDelegatedAdminRequestRequestTypeDef(TypedDict):
    MemberAccountId: str,
```

## RestoreEventDataStoreRequestRequestTypeDef

```python
# RestoreEventDataStoreRequestRequestTypeDef definition

class RestoreEventDataStoreRequestRequestTypeDef(TypedDict):
    EventDataStore: str,
```

## StartEventDataStoreIngestionRequestRequestTypeDef

```python
# StartEventDataStoreIngestionRequestRequestTypeDef definition

class StartEventDataStoreIngestionRequestRequestTypeDef(TypedDict):
    EventDataStore: str,
```

## StartLoggingRequestRequestTypeDef

```python
# StartLoggingRequestRequestTypeDef definition

class StartLoggingRequestRequestTypeDef(TypedDict):
    Name: str,
```

## StartQueryRequestRequestTypeDef

```python
# StartQueryRequestRequestTypeDef definition

class StartQueryRequestRequestTypeDef(TypedDict):
    QueryStatement: NotRequired[str],
    DeliveryS3Uri: NotRequired[str],
    QueryAlias: NotRequired[str],
    QueryParameters: NotRequired[Sequence[str]],
```

## StopEventDataStoreIngestionRequestRequestTypeDef

```python
# StopEventDataStoreIngestionRequestRequestTypeDef definition

class StopEventDataStoreIngestionRequestRequestTypeDef(TypedDict):
    EventDataStore: str,
```

## StopImportRequestRequestTypeDef

```python
# StopImportRequestRequestTypeDef definition

class StopImportRequestRequestTypeDef(TypedDict):
    ImportId: str,
```

## StopLoggingRequestRequestTypeDef

```python
# StopLoggingRequestRequestTypeDef definition

class StopLoggingRequestRequestTypeDef(TypedDict):
    Name: str,
```

## UpdateTrailRequestRequestTypeDef

```python
# UpdateTrailRequestRequestTypeDef definition

class UpdateTrailRequestRequestTypeDef(TypedDict):
    Name: str,
    S3BucketName: NotRequired[str],
    S3KeyPrefix: NotRequired[str],
    SnsTopicName: NotRequired[str],
    IncludeGlobalServiceEvents: NotRequired[bool],
    IsMultiRegionTrail: NotRequired[bool],
    EnableLogFileValidation: NotRequired[bool],
    CloudWatchLogsLogGroupArn: NotRequired[str],
    CloudWatchLogsRoleArn: NotRequired[str],
    KmsKeyId: NotRequired[str],
    IsOrganizationTrail: NotRequired[bool],
```

## AddTagsRequestRequestTypeDef

```python
# AddTagsRequestRequestTypeDef definition

class AddTagsRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    TagsList: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateTrailRequestRequestTypeDef

```python
# CreateTrailRequestRequestTypeDef definition

class CreateTrailRequestRequestTypeDef(TypedDict):
    Name: str,
    S3BucketName: str,
    S3KeyPrefix: NotRequired[str],
    SnsTopicName: NotRequired[str],
    IncludeGlobalServiceEvents: NotRequired[bool],
    IsMultiRegionTrail: NotRequired[bool],
    EnableLogFileValidation: NotRequired[bool],
    CloudWatchLogsLogGroupArn: NotRequired[str],
    CloudWatchLogsRoleArn: NotRequired[str],
    KmsKeyId: NotRequired[str],
    IsOrganizationTrail: NotRequired[bool],
    TagsList: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## RemoveTagsRequestRequestTypeDef

```python
# RemoveTagsRequestRequestTypeDef definition

class RemoveTagsRequestRequestTypeDef(TypedDict):
    ResourceId: str,
    TagsList: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ResourceTagTypeDef

```python
# ResourceTagTypeDef definition

class ResourceTagTypeDef(TypedDict):
    ResourceId: NotRequired[str],
    TagsList: NotRequired[List[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## AdvancedEventSelectorTypeDef

```python
# AdvancedEventSelectorTypeDef definition

class AdvancedEventSelectorTypeDef(TypedDict):
    FieldSelectors: Sequence[AdvancedFieldSelectorTypeDef],  # (1)
    Name: NotRequired[str],
```

1. See [:material-code-braces: AdvancedFieldSelectorTypeDef](./type_defs.md#advancedfieldselectortypedef) 
## CancelQueryResponseTypeDef

```python
# CancelQueryResponseTypeDef definition

class CancelQueryResponseTypeDef(TypedDict):
    QueryId: str,
    QueryStatus: QueryStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: QueryStatusType](./literals.md#querystatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTrailResponseTypeDef

```python
# CreateTrailResponseTypeDef definition

class CreateTrailResponseTypeDef(TypedDict):
    Name: str,
    S3BucketName: str,
    S3KeyPrefix: str,
    SnsTopicName: str,
    SnsTopicARN: str,
    IncludeGlobalServiceEvents: bool,
    IsMultiRegionTrail: bool,
    TrailARN: str,
    LogFileValidationEnabled: bool,
    CloudWatchLogsLogGroupArn: str,
    CloudWatchLogsRoleArn: str,
    KmsKeyId: str,
    IsOrganizationTrail: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourcePolicyResponseTypeDef

```python
# GetResourcePolicyResponseTypeDef definition

class GetResourcePolicyResponseTypeDef(TypedDict):
    ResourceArn: str,
    ResourcePolicy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTrailStatusResponseTypeDef

```python
# GetTrailStatusResponseTypeDef definition

class GetTrailStatusResponseTypeDef(TypedDict):
    IsLogging: bool,
    LatestDeliveryError: str,
    LatestNotificationError: str,
    LatestDeliveryTime: datetime,
    LatestNotificationTime: datetime,
    StartLoggingTime: datetime,
    StopLoggingTime: datetime,
    LatestCloudWatchLogsDeliveryError: str,
    LatestCloudWatchLogsDeliveryTime: datetime,
    LatestDigestDeliveryTime: datetime,
    LatestDigestDeliveryError: str,
    LatestDeliveryAttemptTime: str,
    LatestNotificationAttemptTime: str,
    LatestNotificationAttemptSucceeded: str,
    LatestDeliveryAttemptSucceeded: str,
    TimeLoggingStarted: str,
    TimeLoggingStopped: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutResourcePolicyResponseTypeDef

```python
# PutResourcePolicyResponseTypeDef definition

class PutResourcePolicyResponseTypeDef(TypedDict):
    ResourceArn: str,
    ResourcePolicy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartQueryResponseTypeDef

```python
# StartQueryResponseTypeDef definition

class StartQueryResponseTypeDef(TypedDict):
    QueryId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTrailResponseTypeDef

```python
# UpdateTrailResponseTypeDef definition

class UpdateTrailResponseTypeDef(TypedDict):
    Name: str,
    S3BucketName: str,
    S3KeyPrefix: str,
    SnsTopicName: str,
    SnsTopicARN: str,
    IncludeGlobalServiceEvents: bool,
    IsMultiRegionTrail: bool,
    TrailARN: str,
    LogFileValidationEnabled: bool,
    CloudWatchLogsLogGroupArn: str,
    CloudWatchLogsRoleArn: str,
    KmsKeyId: str,
    IsOrganizationTrail: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListChannelsResponseTypeDef

```python
# ListChannelsResponseTypeDef definition

class ListChannelsResponseTypeDef(TypedDict):
    Channels: List[ChannelTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelTypeDef](./type_defs.md#channeltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateChannelRequestRequestTypeDef

```python
# CreateChannelRequestRequestTypeDef definition

class CreateChannelRequestRequestTypeDef(TypedDict):
    Name: str,
    Source: str,
    Destinations: Sequence[DestinationTypeDef],  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateChannelResponseTypeDef

```python
# CreateChannelResponseTypeDef definition

class CreateChannelResponseTypeDef(TypedDict):
    ChannelArn: str,
    Name: str,
    Source: str,
    Destinations: List[DestinationTypeDef],  # (1)
    Tags: List[TagTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateChannelRequestRequestTypeDef

```python
# UpdateChannelRequestRequestTypeDef definition

class UpdateChannelRequestRequestTypeDef(TypedDict):
    Channel: str,
    Destinations: NotRequired[Sequence[DestinationTypeDef]],  # (1)
    Name: NotRequired[str],
```

1. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
## UpdateChannelResponseTypeDef

```python
# UpdateChannelResponseTypeDef definition

class UpdateChannelResponseTypeDef(TypedDict):
    ChannelArn: str,
    Name: str,
    Source: str,
    Destinations: List[DestinationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EventSelectorTypeDef

```python
# EventSelectorTypeDef definition

class EventSelectorTypeDef(TypedDict):
    ReadWriteType: NotRequired[ReadWriteTypeType],  # (1)
    IncludeManagementEvents: NotRequired[bool],
    DataResources: NotRequired[List[DataResourceTypeDef]],  # (2)
    ExcludeManagementEventSources: NotRequired[List[str]],
```

1. See [:material-code-brackets: ReadWriteTypeType](./literals.md#readwritetypetype) 
2. See [:material-code-braces: DataResourceTypeDef](./type_defs.md#dataresourcetypedef) 
## DescribeQueryResponseTypeDef

```python
# DescribeQueryResponseTypeDef definition

class DescribeQueryResponseTypeDef(TypedDict):
    QueryId: str,
    QueryString: str,
    QueryStatus: QueryStatusType,  # (1)
    QueryStatistics: QueryStatisticsForDescribeQueryTypeDef,  # (2)
    ErrorMessage: str,
    DeliveryS3Uri: str,
    DeliveryStatus: DeliveryStatusType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: QueryStatusType](./literals.md#querystatustype) 
2. See [:material-code-braces: QueryStatisticsForDescribeQueryTypeDef](./type_defs.md#querystatisticsfordescribequerytypedef) 
3. See [:material-code-brackets: DeliveryStatusType](./literals.md#deliverystatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTrailsResponseTypeDef

```python
# DescribeTrailsResponseTypeDef definition

class DescribeTrailsResponseTypeDef(TypedDict):
    trailList: List[TrailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrailTypeDef](./type_defs.md#trailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTrailResponseTypeDef

```python
# GetTrailResponseTypeDef definition

class GetTrailResponseTypeDef(TypedDict):
    Trail: TrailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrailTypeDef](./type_defs.md#trailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EventTypeDef

```python
# EventTypeDef definition

class EventTypeDef(TypedDict):
    EventId: NotRequired[str],
    EventName: NotRequired[str],
    ReadOnly: NotRequired[str],
    AccessKeyId: NotRequired[str],
    EventTime: NotRequired[datetime],
    EventSource: NotRequired[str],
    Username: NotRequired[str],
    Resources: NotRequired[List[ResourceTypeDef]],  # (1)
    CloudTrailEvent: NotRequired[str],
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
## GetInsightSelectorsResponseTypeDef

```python
# GetInsightSelectorsResponseTypeDef definition

class GetInsightSelectorsResponseTypeDef(TypedDict):
    TrailARN: str,
    InsightSelectors: List[InsightSelectorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InsightSelectorTypeDef](./type_defs.md#insightselectortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutInsightSelectorsRequestRequestTypeDef

```python
# PutInsightSelectorsRequestRequestTypeDef definition

class PutInsightSelectorsRequestRequestTypeDef(TypedDict):
    TrailName: str,
    InsightSelectors: Sequence[InsightSelectorTypeDef],  # (1)
```

1. See [:material-code-braces: InsightSelectorTypeDef](./type_defs.md#insightselectortypedef) 
## PutInsightSelectorsResponseTypeDef

```python
# PutInsightSelectorsResponseTypeDef definition

class PutInsightSelectorsResponseTypeDef(TypedDict):
    TrailARN: str,
    InsightSelectors: List[InsightSelectorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InsightSelectorTypeDef](./type_defs.md#insightselectortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetQueryResultsResponseTypeDef

```python
# GetQueryResultsResponseTypeDef definition

class GetQueryResultsResponseTypeDef(TypedDict):
    QueryStatus: QueryStatusType,  # (1)
    QueryStatistics: QueryStatisticsTypeDef,  # (2)
    QueryResultRows: List[List[Dict[str, str]]],
    NextToken: str,
    ErrorMessage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: QueryStatusType](./literals.md#querystatustype) 
2. See [:material-code-braces: QueryStatisticsTypeDef](./type_defs.md#querystatisticstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListImportFailuresResponseTypeDef

```python
# ListImportFailuresResponseTypeDef definition

class ListImportFailuresResponseTypeDef(TypedDict):
    Failures: List[ImportFailureListItemTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImportFailureListItemTypeDef](./type_defs.md#importfailurelistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportSourceTypeDef

```python
# ImportSourceTypeDef definition

class ImportSourceTypeDef(TypedDict):
    S3: S3ImportSourceTypeDef,  # (1)
```

1. See [:material-code-braces: S3ImportSourceTypeDef](./type_defs.md#s3importsourcetypedef) 
## ListImportsResponseTypeDef

```python
# ListImportsResponseTypeDef definition

class ListImportsResponseTypeDef(TypedDict):
    Imports: List[ImportsListItemTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImportsListItemTypeDef](./type_defs.md#importslistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListImportFailuresRequestListImportFailuresPaginateTypeDef

```python
# ListImportFailuresRequestListImportFailuresPaginateTypeDef definition

class ListImportFailuresRequestListImportFailuresPaginateTypeDef(TypedDict):
    ImportId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListImportsRequestListImportsPaginateTypeDef

```python
# ListImportsRequestListImportsPaginateTypeDef definition

class ListImportsRequestListImportsPaginateTypeDef(TypedDict):
    Destination: NotRequired[str],
    ImportStatus: NotRequired[ImportStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ImportStatusType](./literals.md#importstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsRequestListTagsPaginateTypeDef

```python
# ListTagsRequestListTagsPaginateTypeDef definition

class ListTagsRequestListTagsPaginateTypeDef(TypedDict):
    ResourceIdList: Sequence[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTrailsRequestListTrailsPaginateTypeDef

```python
# ListTrailsRequestListTrailsPaginateTypeDef definition

class ListTrailsRequestListTrailsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPublicKeysRequestListPublicKeysPaginateTypeDef

```python
# ListPublicKeysRequestListPublicKeysPaginateTypeDef definition

class ListPublicKeysRequestListPublicKeysPaginateTypeDef(TypedDict):
    StartTime: NotRequired[Union[datetime, str]],
    EndTime: NotRequired[Union[datetime, str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPublicKeysRequestRequestTypeDef

```python
# ListPublicKeysRequestRequestTypeDef definition

class ListPublicKeysRequestRequestTypeDef(TypedDict):
    StartTime: NotRequired[Union[datetime, str]],
    EndTime: NotRequired[Union[datetime, str]],
    NextToken: NotRequired[str],
```

## ListQueriesRequestRequestTypeDef

```python
# ListQueriesRequestRequestTypeDef definition

class ListQueriesRequestRequestTypeDef(TypedDict):
    EventDataStore: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    StartTime: NotRequired[Union[datetime, str]],
    EndTime: NotRequired[Union[datetime, str]],
    QueryStatus: NotRequired[QueryStatusType],  # (1)
```

1. See [:material-code-brackets: QueryStatusType](./literals.md#querystatustype) 
## ListPublicKeysResponseTypeDef

```python
# ListPublicKeysResponseTypeDef definition

class ListPublicKeysResponseTypeDef(TypedDict):
    PublicKeyList: List[PublicKeyTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PublicKeyTypeDef](./type_defs.md#publickeytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListQueriesResponseTypeDef

```python
# ListQueriesResponseTypeDef definition

class ListQueriesResponseTypeDef(TypedDict):
    Queries: List[QueryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QueryTypeDef](./type_defs.md#querytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTrailsResponseTypeDef

```python
# ListTrailsResponseTypeDef definition

class ListTrailsResponseTypeDef(TypedDict):
    Trails: List[TrailInfoTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrailInfoTypeDef](./type_defs.md#trailinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LookupEventsRequestLookupEventsPaginateTypeDef

```python
# LookupEventsRequestLookupEventsPaginateTypeDef definition

class LookupEventsRequestLookupEventsPaginateTypeDef(TypedDict):
    LookupAttributes: NotRequired[Sequence[LookupAttributeTypeDef]],  # (1)
    StartTime: NotRequired[Union[datetime, str]],
    EndTime: NotRequired[Union[datetime, str]],
    EventCategory: NotRequired[EventCategoryType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: LookupAttributeTypeDef](./type_defs.md#lookupattributetypedef) 
2. See [:material-code-brackets: EventCategoryType](./literals.md#eventcategorytype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## LookupEventsRequestRequestTypeDef

```python
# LookupEventsRequestRequestTypeDef definition

class LookupEventsRequestRequestTypeDef(TypedDict):
    LookupAttributes: NotRequired[Sequence[LookupAttributeTypeDef]],  # (1)
    StartTime: NotRequired[Union[datetime, str]],
    EndTime: NotRequired[Union[datetime, str]],
    EventCategory: NotRequired[EventCategoryType],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: LookupAttributeTypeDef](./type_defs.md#lookupattributetypedef) 
2. See [:material-code-brackets: EventCategoryType](./literals.md#eventcategorytype) 
## ListTagsResponseTypeDef

```python
# ListTagsResponseTypeDef definition

class ListTagsResponseTypeDef(TypedDict):
    ResourceTagList: List[ResourceTagTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEventDataStoreRequestRequestTypeDef

```python
# CreateEventDataStoreRequestRequestTypeDef definition

class CreateEventDataStoreRequestRequestTypeDef(TypedDict):
    Name: str,
    AdvancedEventSelectors: NotRequired[Sequence[AdvancedEventSelectorTypeDef]],  # (1)
    MultiRegionEnabled: NotRequired[bool],
    OrganizationEnabled: NotRequired[bool],
    RetentionPeriod: NotRequired[int],
    TerminationProtectionEnabled: NotRequired[bool],
    TagsList: NotRequired[Sequence[TagTypeDef]],  # (2)
    KmsKeyId: NotRequired[str],
    StartIngestion: NotRequired[bool],
```

1. See [:material-code-braces: AdvancedEventSelectorTypeDef](./type_defs.md#advancedeventselectortypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateEventDataStoreResponseTypeDef

```python
# CreateEventDataStoreResponseTypeDef definition

class CreateEventDataStoreResponseTypeDef(TypedDict):
    EventDataStoreArn: str,
    Name: str,
    Status: EventDataStoreStatusType,  # (1)
    AdvancedEventSelectors: List[AdvancedEventSelectorTypeDef],  # (2)
    MultiRegionEnabled: bool,
    OrganizationEnabled: bool,
    RetentionPeriod: int,
    TerminationProtectionEnabled: bool,
    TagsList: List[TagTypeDef],  # (3)
    CreatedTimestamp: datetime,
    UpdatedTimestamp: datetime,
    KmsKeyId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: EventDataStoreStatusType](./literals.md#eventdatastorestatustype) 
2. See [:material-code-braces: AdvancedEventSelectorTypeDef](./type_defs.md#advancedeventselectortypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EventDataStoreTypeDef

```python
# EventDataStoreTypeDef definition

class EventDataStoreTypeDef(TypedDict):
    EventDataStoreArn: NotRequired[str],
    Name: NotRequired[str],
    TerminationProtectionEnabled: NotRequired[bool],
    Status: NotRequired[EventDataStoreStatusType],  # (1)
    AdvancedEventSelectors: NotRequired[List[AdvancedEventSelectorTypeDef]],  # (2)
    MultiRegionEnabled: NotRequired[bool],
    OrganizationEnabled: NotRequired[bool],
    RetentionPeriod: NotRequired[int],
    CreatedTimestamp: NotRequired[datetime],
    UpdatedTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: EventDataStoreStatusType](./literals.md#eventdatastorestatustype) 
2. See [:material-code-braces: AdvancedEventSelectorTypeDef](./type_defs.md#advancedeventselectortypedef) 
## GetEventDataStoreResponseTypeDef

```python
# GetEventDataStoreResponseTypeDef definition

class GetEventDataStoreResponseTypeDef(TypedDict):
    EventDataStoreArn: str,
    Name: str,
    Status: EventDataStoreStatusType,  # (1)
    AdvancedEventSelectors: List[AdvancedEventSelectorTypeDef],  # (2)
    MultiRegionEnabled: bool,
    OrganizationEnabled: bool,
    RetentionPeriod: int,
    TerminationProtectionEnabled: bool,
    CreatedTimestamp: datetime,
    UpdatedTimestamp: datetime,
    KmsKeyId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: EventDataStoreStatusType](./literals.md#eventdatastorestatustype) 
2. See [:material-code-braces: AdvancedEventSelectorTypeDef](./type_defs.md#advancedeventselectortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreEventDataStoreResponseTypeDef

```python
# RestoreEventDataStoreResponseTypeDef definition

class RestoreEventDataStoreResponseTypeDef(TypedDict):
    EventDataStoreArn: str,
    Name: str,
    Status: EventDataStoreStatusType,  # (1)
    AdvancedEventSelectors: List[AdvancedEventSelectorTypeDef],  # (2)
    MultiRegionEnabled: bool,
    OrganizationEnabled: bool,
    RetentionPeriod: int,
    TerminationProtectionEnabled: bool,
    CreatedTimestamp: datetime,
    UpdatedTimestamp: datetime,
    KmsKeyId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: EventDataStoreStatusType](./literals.md#eventdatastorestatustype) 
2. See [:material-code-braces: AdvancedEventSelectorTypeDef](./type_defs.md#advancedeventselectortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SourceConfigTypeDef

```python
# SourceConfigTypeDef definition

class SourceConfigTypeDef(TypedDict):
    ApplyToAllRegions: NotRequired[bool],
    AdvancedEventSelectors: NotRequired[List[AdvancedEventSelectorTypeDef]],  # (1)
```

1. See [:material-code-braces: AdvancedEventSelectorTypeDef](./type_defs.md#advancedeventselectortypedef) 
## UpdateEventDataStoreRequestRequestTypeDef

```python
# UpdateEventDataStoreRequestRequestTypeDef definition

class UpdateEventDataStoreRequestRequestTypeDef(TypedDict):
    EventDataStore: str,
    Name: NotRequired[str],
    AdvancedEventSelectors: NotRequired[Sequence[AdvancedEventSelectorTypeDef]],  # (1)
    MultiRegionEnabled: NotRequired[bool],
    OrganizationEnabled: NotRequired[bool],
    RetentionPeriod: NotRequired[int],
    TerminationProtectionEnabled: NotRequired[bool],
    KmsKeyId: NotRequired[str],
```

1. See [:material-code-braces: AdvancedEventSelectorTypeDef](./type_defs.md#advancedeventselectortypedef) 
## UpdateEventDataStoreResponseTypeDef

```python
# UpdateEventDataStoreResponseTypeDef definition

class UpdateEventDataStoreResponseTypeDef(TypedDict):
    EventDataStoreArn: str,
    Name: str,
    Status: EventDataStoreStatusType,  # (1)
    AdvancedEventSelectors: List[AdvancedEventSelectorTypeDef],  # (2)
    MultiRegionEnabled: bool,
    OrganizationEnabled: bool,
    RetentionPeriod: int,
    TerminationProtectionEnabled: bool,
    CreatedTimestamp: datetime,
    UpdatedTimestamp: datetime,
    KmsKeyId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: EventDataStoreStatusType](./literals.md#eventdatastorestatustype) 
2. See [:material-code-braces: AdvancedEventSelectorTypeDef](./type_defs.md#advancedeventselectortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEventSelectorsResponseTypeDef

```python
# GetEventSelectorsResponseTypeDef definition

class GetEventSelectorsResponseTypeDef(TypedDict):
    TrailARN: str,
    EventSelectors: List[EventSelectorTypeDef],  # (1)
    AdvancedEventSelectors: List[AdvancedEventSelectorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: EventSelectorTypeDef](./type_defs.md#eventselectortypedef) 
2. See [:material-code-braces: AdvancedEventSelectorTypeDef](./type_defs.md#advancedeventselectortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutEventSelectorsRequestRequestTypeDef

```python
# PutEventSelectorsRequestRequestTypeDef definition

class PutEventSelectorsRequestRequestTypeDef(TypedDict):
    TrailName: str,
    EventSelectors: NotRequired[Sequence[EventSelectorTypeDef]],  # (1)
    AdvancedEventSelectors: NotRequired[Sequence[AdvancedEventSelectorTypeDef]],  # (2)
```

1. See [:material-code-braces: EventSelectorTypeDef](./type_defs.md#eventselectortypedef) 
2. See [:material-code-braces: AdvancedEventSelectorTypeDef](./type_defs.md#advancedeventselectortypedef) 
## PutEventSelectorsResponseTypeDef

```python
# PutEventSelectorsResponseTypeDef definition

class PutEventSelectorsResponseTypeDef(TypedDict):
    TrailARN: str,
    EventSelectors: List[EventSelectorTypeDef],  # (1)
    AdvancedEventSelectors: List[AdvancedEventSelectorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: EventSelectorTypeDef](./type_defs.md#eventselectortypedef) 
2. See [:material-code-braces: AdvancedEventSelectorTypeDef](./type_defs.md#advancedeventselectortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LookupEventsResponseTypeDef

```python
# LookupEventsResponseTypeDef definition

class LookupEventsResponseTypeDef(TypedDict):
    Events: List[EventTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetImportResponseTypeDef

```python
# GetImportResponseTypeDef definition

class GetImportResponseTypeDef(TypedDict):
    ImportId: str,
    Destinations: List[str],
    ImportSource: ImportSourceTypeDef,  # (1)
    StartEventTime: datetime,
    EndEventTime: datetime,
    ImportStatus: ImportStatusType,  # (2)
    CreatedTimestamp: datetime,
    UpdatedTimestamp: datetime,
    ImportStatistics: ImportStatisticsTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ImportSourceTypeDef](./type_defs.md#importsourcetypedef) 
2. See [:material-code-brackets: ImportStatusType](./literals.md#importstatustype) 
3. See [:material-code-braces: ImportStatisticsTypeDef](./type_defs.md#importstatisticstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartImportRequestRequestTypeDef

```python
# StartImportRequestRequestTypeDef definition

class StartImportRequestRequestTypeDef(TypedDict):
    Destinations: NotRequired[Sequence[str]],
    ImportSource: NotRequired[ImportSourceTypeDef],  # (1)
    StartEventTime: NotRequired[Union[datetime, str]],
    EndEventTime: NotRequired[Union[datetime, str]],
    ImportId: NotRequired[str],
```

1. See [:material-code-braces: ImportSourceTypeDef](./type_defs.md#importsourcetypedef) 
## StartImportResponseTypeDef

```python
# StartImportResponseTypeDef definition

class StartImportResponseTypeDef(TypedDict):
    ImportId: str,
    Destinations: List[str],
    ImportSource: ImportSourceTypeDef,  # (1)
    StartEventTime: datetime,
    EndEventTime: datetime,
    ImportStatus: ImportStatusType,  # (2)
    CreatedTimestamp: datetime,
    UpdatedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ImportSourceTypeDef](./type_defs.md#importsourcetypedef) 
2. See [:material-code-brackets: ImportStatusType](./literals.md#importstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopImportResponseTypeDef

```python
# StopImportResponseTypeDef definition

class StopImportResponseTypeDef(TypedDict):
    ImportId: str,
    ImportSource: ImportSourceTypeDef,  # (1)
    Destinations: List[str],
    ImportStatus: ImportStatusType,  # (2)
    CreatedTimestamp: datetime,
    UpdatedTimestamp: datetime,
    StartEventTime: datetime,
    EndEventTime: datetime,
    ImportStatistics: ImportStatisticsTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ImportSourceTypeDef](./type_defs.md#importsourcetypedef) 
2. See [:material-code-brackets: ImportStatusType](./literals.md#importstatustype) 
3. See [:material-code-braces: ImportStatisticsTypeDef](./type_defs.md#importstatisticstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEventDataStoresResponseTypeDef

```python
# ListEventDataStoresResponseTypeDef definition

class ListEventDataStoresResponseTypeDef(TypedDict):
    EventDataStores: List[EventDataStoreTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventDataStoreTypeDef](./type_defs.md#eventdatastoretypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetChannelResponseTypeDef

```python
# GetChannelResponseTypeDef definition

class GetChannelResponseTypeDef(TypedDict):
    ChannelArn: str,
    Name: str,
    Source: str,
    SourceConfig: SourceConfigTypeDef,  # (1)
    Destinations: List[DestinationTypeDef],  # (2)
    IngestionStatus: IngestionStatusTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: SourceConfigTypeDef](./type_defs.md#sourceconfigtypedef) 
2. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
3. See [:material-code-braces: IngestionStatusTypeDef](./type_defs.md#ingestionstatustypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
