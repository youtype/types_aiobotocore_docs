<a id="typed-dictionaries-for-aiobotocore-cloudtrail-module"></a>

# Typed dictionaries for aiobotocore CloudTrail module

> [Index](../README.md) > [CloudTrail](./README.md) > Typed dictionaries

Auto-generated documentation for
[CloudTrail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail)
type annotations stubs module
[types-aiobotocore-cloudtrail](https://pypi.org/project/types-aiobotocore-cloudtrail/).

- [Typed dictionaries for aiobotocore CloudTrail module](#typed-dictionaries-for-aiobotocore-cloudtrail-module)
  - [AddTagsRequestRequestTypeDef](#addtagsrequestrequesttypedef)
  - [AdvancedEventSelectorTypeDef](#advancedeventselectortypedef)
  - [AdvancedFieldSelectorTypeDef](#advancedfieldselectortypedef)
  - [CancelQueryRequestRequestTypeDef](#cancelqueryrequestrequesttypedef)
  - [CancelQueryResponseTypeDef](#cancelqueryresponsetypedef)
  - [CreateEventDataStoreRequestRequestTypeDef](#createeventdatastorerequestrequesttypedef)
  - [CreateEventDataStoreResponseTypeDef](#createeventdatastoreresponsetypedef)
  - [CreateTrailRequestRequestTypeDef](#createtrailrequestrequesttypedef)
  - [CreateTrailResponseTypeDef](#createtrailresponsetypedef)
  - [DataResourceTypeDef](#dataresourcetypedef)
  - [DeleteEventDataStoreRequestRequestTypeDef](#deleteeventdatastorerequestrequesttypedef)
  - [DeleteTrailRequestRequestTypeDef](#deletetrailrequestrequesttypedef)
  - [DescribeQueryRequestRequestTypeDef](#describequeryrequestrequesttypedef)
  - [DescribeQueryResponseTypeDef](#describequeryresponsetypedef)
  - [DescribeTrailsRequestRequestTypeDef](#describetrailsrequestrequesttypedef)
  - [DescribeTrailsResponseTypeDef](#describetrailsresponsetypedef)
  - [EventDataStoreTypeDef](#eventdatastoretypedef)
  - [EventSelectorTypeDef](#eventselectortypedef)
  - [EventTypeDef](#eventtypedef)
  - [GetEventDataStoreRequestRequestTypeDef](#geteventdatastorerequestrequesttypedef)
  - [GetEventDataStoreResponseTypeDef](#geteventdatastoreresponsetypedef)
  - [GetEventSelectorsRequestRequestTypeDef](#geteventselectorsrequestrequesttypedef)
  - [GetEventSelectorsResponseTypeDef](#geteventselectorsresponsetypedef)
  - [GetInsightSelectorsRequestRequestTypeDef](#getinsightselectorsrequestrequesttypedef)
  - [GetInsightSelectorsResponseTypeDef](#getinsightselectorsresponsetypedef)
  - [GetQueryResultsRequestRequestTypeDef](#getqueryresultsrequestrequesttypedef)
  - [GetQueryResultsResponseTypeDef](#getqueryresultsresponsetypedef)
  - [GetTrailRequestRequestTypeDef](#gettrailrequestrequesttypedef)
  - [GetTrailResponseTypeDef](#gettrailresponsetypedef)
  - [GetTrailStatusRequestRequestTypeDef](#gettrailstatusrequestrequesttypedef)
  - [GetTrailStatusResponseTypeDef](#gettrailstatusresponsetypedef)
  - [InsightSelectorTypeDef](#insightselectortypedef)
  - [ListEventDataStoresRequestRequestTypeDef](#listeventdatastoresrequestrequesttypedef)
  - [ListEventDataStoresResponseTypeDef](#listeventdatastoresresponsetypedef)
  - [ListPublicKeysRequestRequestTypeDef](#listpublickeysrequestrequesttypedef)
  - [ListPublicKeysResponseTypeDef](#listpublickeysresponsetypedef)
  - [ListQueriesRequestRequestTypeDef](#listqueriesrequestrequesttypedef)
  - [ListQueriesResponseTypeDef](#listqueriesresponsetypedef)
  - [ListTagsRequestRequestTypeDef](#listtagsrequestrequesttypedef)
  - [ListTagsResponseTypeDef](#listtagsresponsetypedef)
  - [ListTrailsRequestRequestTypeDef](#listtrailsrequestrequesttypedef)
  - [ListTrailsResponseTypeDef](#listtrailsresponsetypedef)
  - [LookupAttributeTypeDef](#lookupattributetypedef)
  - [LookupEventsRequestRequestTypeDef](#lookupeventsrequestrequesttypedef)
  - [LookupEventsResponseTypeDef](#lookupeventsresponsetypedef)
  - [PaginatorConfigTypeDef](#paginatorconfigtypedef)
  - [PublicKeyTypeDef](#publickeytypedef)
  - [PutEventSelectorsRequestRequestTypeDef](#puteventselectorsrequestrequesttypedef)
  - [PutEventSelectorsResponseTypeDef](#puteventselectorsresponsetypedef)
  - [PutInsightSelectorsRequestRequestTypeDef](#putinsightselectorsrequestrequesttypedef)
  - [PutInsightSelectorsResponseTypeDef](#putinsightselectorsresponsetypedef)
  - [QueryStatisticsForDescribeQueryTypeDef](#querystatisticsfordescribequerytypedef)
  - [QueryStatisticsTypeDef](#querystatisticstypedef)
  - [QueryTypeDef](#querytypedef)
  - [RemoveTagsRequestRequestTypeDef](#removetagsrequestrequesttypedef)
  - [ResourceTagTypeDef](#resourcetagtypedef)
  - [ResourceTypeDef](#resourcetypedef)
  - [ResponseMetadataTypeDef](#responsemetadatatypedef)
  - [RestoreEventDataStoreRequestRequestTypeDef](#restoreeventdatastorerequestrequesttypedef)
  - [RestoreEventDataStoreResponseTypeDef](#restoreeventdatastoreresponsetypedef)
  - [StartLoggingRequestRequestTypeDef](#startloggingrequestrequesttypedef)
  - [StartQueryRequestRequestTypeDef](#startqueryrequestrequesttypedef)
  - [StartQueryResponseTypeDef](#startqueryresponsetypedef)
  - [StopLoggingRequestRequestTypeDef](#stoploggingrequestrequesttypedef)
  - [TagTypeDef](#tagtypedef)
  - [TrailInfoTypeDef](#trailinfotypedef)
  - [TrailTypeDef](#trailtypedef)
  - [UpdateEventDataStoreRequestRequestTypeDef](#updateeventdatastorerequestrequesttypedef)
  - [UpdateEventDataStoreResponseTypeDef](#updateeventdatastoreresponsetypedef)
  - [UpdateTrailRequestRequestTypeDef](#updatetrailrequestrequesttypedef)
  - [UpdateTrailResponseTypeDef](#updatetrailresponsetypedef)

<a id="addtagsrequestrequesttypedef"></a>

## AddTagsRequestRequestTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import AddTagsRequestRequestTypeDef
```

Required fields:

- `ResourceId`: `str`
- `TagsList`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

<a id="advancedeventselectortypedef"></a>

## AdvancedEventSelectorTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import AdvancedEventSelectorTypeDef
```

Required fields:

- `FieldSelectors`:
  `Sequence`\[[AdvancedFieldSelectorTypeDef](./type_defs.md#advancedfieldselectortypedef)\]

Optional fields:

- `Name`: `str`

<a id="advancedfieldselectortypedef"></a>

## AdvancedFieldSelectorTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import AdvancedFieldSelectorTypeDef
```

Required fields:

- `Field`: `str`

Optional fields:

- `Equals`: `Sequence`\[`str`\]
- `StartsWith`: `Sequence`\[`str`\]
- `EndsWith`: `Sequence`\[`str`\]
- `NotEquals`: `Sequence`\[`str`\]
- `NotStartsWith`: `Sequence`\[`str`\]
- `NotEndsWith`: `Sequence`\[`str`\]

<a id="cancelqueryrequestrequesttypedef"></a>

## CancelQueryRequestRequestTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import CancelQueryRequestRequestTypeDef
```

Required fields:

- `EventDataStore`: `str`
- `QueryId`: `str`

<a id="cancelqueryresponsetypedef"></a>

## CancelQueryResponseTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import CancelQueryResponseTypeDef
```

Required fields:

- `QueryId`: `str`
- `QueryStatus`: [QueryStatusType](./literals.md#querystatustype)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createeventdatastorerequestrequesttypedef"></a>

## CreateEventDataStoreRequestRequestTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import CreateEventDataStoreRequestRequestTypeDef
```

Required fields:

- `Name`: `str`

Optional fields:

- `AdvancedEventSelectors`:
  `Sequence`\[[AdvancedEventSelectorTypeDef](./type_defs.md#advancedeventselectortypedef)\]
- `MultiRegionEnabled`: `bool`
- `OrganizationEnabled`: `bool`
- `RetentionPeriod`: `int`
- `TerminationProtectionEnabled`: `bool`
- `TagsList`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

<a id="createeventdatastoreresponsetypedef"></a>

## CreateEventDataStoreResponseTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import CreateEventDataStoreResponseTypeDef
```

Required fields:

- `EventDataStoreArn`: `str`
- `Name`: `str`
- `Status`: [EventDataStoreStatusType](./literals.md#eventdatastorestatustype)
- `AdvancedEventSelectors`:
  `List`\[[AdvancedEventSelectorTypeDef](./type_defs.md#advancedeventselectortypedef)\]
- `MultiRegionEnabled`: `bool`
- `OrganizationEnabled`: `bool`
- `RetentionPeriod`: `int`
- `TerminationProtectionEnabled`: `bool`
- `TagsList`: `List`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `CreatedTimestamp`: `datetime`
- `UpdatedTimestamp`: `datetime`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createtrailrequestrequesttypedef"></a>

## CreateTrailRequestRequestTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import CreateTrailRequestRequestTypeDef
```

Required fields:

- `Name`: `str`
- `S3BucketName`: `str`

Optional fields:

- `S3KeyPrefix`: `str`
- `SnsTopicName`: `str`
- `IncludeGlobalServiceEvents`: `bool`
- `IsMultiRegionTrail`: `bool`
- `EnableLogFileValidation`: `bool`
- `CloudWatchLogsLogGroupArn`: `str`
- `CloudWatchLogsRoleArn`: `str`
- `KmsKeyId`: `str`
- `IsOrganizationTrail`: `bool`
- `TagsList`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

<a id="createtrailresponsetypedef"></a>

## CreateTrailResponseTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import CreateTrailResponseTypeDef
```

Required fields:

- `Name`: `str`
- `S3BucketName`: `str`
- `S3KeyPrefix`: `str`
- `SnsTopicName`: `str`
- `SnsTopicARN`: `str`
- `IncludeGlobalServiceEvents`: `bool`
- `IsMultiRegionTrail`: `bool`
- `TrailARN`: `str`
- `LogFileValidationEnabled`: `bool`
- `CloudWatchLogsLogGroupArn`: `str`
- `CloudWatchLogsRoleArn`: `str`
- `KmsKeyId`: `str`
- `IsOrganizationTrail`: `bool`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="dataresourcetypedef"></a>

## DataResourceTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import DataResourceTypeDef
```

Optional fields:

- `Type`: `str`
- `Values`: `List`\[`str`\]

<a id="deleteeventdatastorerequestrequesttypedef"></a>

## DeleteEventDataStoreRequestRequestTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import DeleteEventDataStoreRequestRequestTypeDef
```

Required fields:

- `EventDataStore`: `str`

<a id="deletetrailrequestrequesttypedef"></a>

## DeleteTrailRequestRequestTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import DeleteTrailRequestRequestTypeDef
```

Required fields:

- `Name`: `str`

<a id="describequeryrequestrequesttypedef"></a>

## DescribeQueryRequestRequestTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import DescribeQueryRequestRequestTypeDef
```

Required fields:

- `EventDataStore`: `str`
- `QueryId`: `str`

<a id="describequeryresponsetypedef"></a>

## DescribeQueryResponseTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import DescribeQueryResponseTypeDef
```

Required fields:

- `QueryId`: `str`
- `QueryString`: `str`
- `QueryStatus`: [QueryStatusType](./literals.md#querystatustype)
- `QueryStatistics`:
  [QueryStatisticsForDescribeQueryTypeDef](./type_defs.md#querystatisticsfordescribequerytypedef)
- `ErrorMessage`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describetrailsrequestrequesttypedef"></a>

## DescribeTrailsRequestRequestTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import DescribeTrailsRequestRequestTypeDef
```

Optional fields:

- `trailNameList`: `Sequence`\[`str`\]
- `includeShadowTrails`: `bool`

<a id="describetrailsresponsetypedef"></a>

## DescribeTrailsResponseTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import DescribeTrailsResponseTypeDef
```

Required fields:

- `trailList`: `List`\[[TrailTypeDef](./type_defs.md#trailtypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="eventdatastoretypedef"></a>

## EventDataStoreTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import EventDataStoreTypeDef
```

Optional fields:

- `EventDataStoreArn`: `str`
- `Name`: `str`
- `TerminationProtectionEnabled`: `bool`
- `Status`: [EventDataStoreStatusType](./literals.md#eventdatastorestatustype)
- `AdvancedEventSelectors`:
  `List`\[[AdvancedEventSelectorTypeDef](./type_defs.md#advancedeventselectortypedef)\]
- `MultiRegionEnabled`: `bool`
- `OrganizationEnabled`: `bool`
- `RetentionPeriod`: `int`
- `CreatedTimestamp`: `datetime`
- `UpdatedTimestamp`: `datetime`

<a id="eventselectortypedef"></a>

## EventSelectorTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import EventSelectorTypeDef
```

Optional fields:

- `ReadWriteType`: [ReadWriteTypeType](./literals.md#readwritetypetype)
- `IncludeManagementEvents`: `bool`
- `DataResources`:
  `List`\[[DataResourceTypeDef](./type_defs.md#dataresourcetypedef)\]
- `ExcludeManagementEventSources`: `List`\[`str`\]

<a id="eventtypedef"></a>

## EventTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import EventTypeDef
```

Optional fields:

- `EventId`: `str`
- `EventName`: `str`
- `ReadOnly`: `str`
- `AccessKeyId`: `str`
- `EventTime`: `datetime`
- `EventSource`: `str`
- `Username`: `str`
- `Resources`: `List`\[[ResourceTypeDef](./type_defs.md#resourcetypedef)\]
- `CloudTrailEvent`: `str`

<a id="geteventdatastorerequestrequesttypedef"></a>

## GetEventDataStoreRequestRequestTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import GetEventDataStoreRequestRequestTypeDef
```

Required fields:

- `EventDataStore`: `str`

<a id="geteventdatastoreresponsetypedef"></a>

## GetEventDataStoreResponseTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import GetEventDataStoreResponseTypeDef
```

Required fields:

- `EventDataStoreArn`: `str`
- `Name`: `str`
- `Status`: [EventDataStoreStatusType](./literals.md#eventdatastorestatustype)
- `AdvancedEventSelectors`:
  `List`\[[AdvancedEventSelectorTypeDef](./type_defs.md#advancedeventselectortypedef)\]
- `MultiRegionEnabled`: `bool`
- `OrganizationEnabled`: `bool`
- `RetentionPeriod`: `int`
- `TerminationProtectionEnabled`: `bool`
- `CreatedTimestamp`: `datetime`
- `UpdatedTimestamp`: `datetime`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="geteventselectorsrequestrequesttypedef"></a>

## GetEventSelectorsRequestRequestTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import GetEventSelectorsRequestRequestTypeDef
```

Required fields:

- `TrailName`: `str`

<a id="geteventselectorsresponsetypedef"></a>

## GetEventSelectorsResponseTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import GetEventSelectorsResponseTypeDef
```

Required fields:

- `TrailARN`: `str`
- `EventSelectors`:
  `List`\[[EventSelectorTypeDef](./type_defs.md#eventselectortypedef)\]
- `AdvancedEventSelectors`:
  `List`\[[AdvancedEventSelectorTypeDef](./type_defs.md#advancedeventselectortypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getinsightselectorsrequestrequesttypedef"></a>

## GetInsightSelectorsRequestRequestTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import GetInsightSelectorsRequestRequestTypeDef
```

Required fields:

- `TrailName`: `str`

<a id="getinsightselectorsresponsetypedef"></a>

## GetInsightSelectorsResponseTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import GetInsightSelectorsResponseTypeDef
```

Required fields:

- `TrailARN`: `str`
- `InsightSelectors`:
  `List`\[[InsightSelectorTypeDef](./type_defs.md#insightselectortypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getqueryresultsrequestrequesttypedef"></a>

## GetQueryResultsRequestRequestTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import GetQueryResultsRequestRequestTypeDef
```

Required fields:

- `EventDataStore`: `str`
- `QueryId`: `str`

Optional fields:

- `NextToken`: `str`
- `MaxQueryResults`: `int`

<a id="getqueryresultsresponsetypedef"></a>

## GetQueryResultsResponseTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import GetQueryResultsResponseTypeDef
```

Required fields:

- `QueryStatus`: [QueryStatusType](./literals.md#querystatustype)
- `QueryStatistics`:
  [QueryStatisticsTypeDef](./type_defs.md#querystatisticstypedef)
- `QueryResultRows`: `List`\[`List`\[`Dict`\[`str`, `str`\]\]\]
- `NextToken`: `str`
- `ErrorMessage`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="gettrailrequestrequesttypedef"></a>

## GetTrailRequestRequestTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import GetTrailRequestRequestTypeDef
```

Required fields:

- `Name`: `str`

<a id="gettrailresponsetypedef"></a>

## GetTrailResponseTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import GetTrailResponseTypeDef
```

Required fields:

- `Trail`: [TrailTypeDef](./type_defs.md#trailtypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="gettrailstatusrequestrequesttypedef"></a>

## GetTrailStatusRequestRequestTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import GetTrailStatusRequestRequestTypeDef
```

Required fields:

- `Name`: `str`

<a id="gettrailstatusresponsetypedef"></a>

## GetTrailStatusResponseTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import GetTrailStatusResponseTypeDef
```

Required fields:

- `IsLogging`: `bool`
- `LatestDeliveryError`: `str`
- `LatestNotificationError`: `str`
- `LatestDeliveryTime`: `datetime`
- `LatestNotificationTime`: `datetime`
- `StartLoggingTime`: `datetime`
- `StopLoggingTime`: `datetime`
- `LatestCloudWatchLogsDeliveryError`: `str`
- `LatestCloudWatchLogsDeliveryTime`: `datetime`
- `LatestDigestDeliveryTime`: `datetime`
- `LatestDigestDeliveryError`: `str`
- `LatestDeliveryAttemptTime`: `str`
- `LatestNotificationAttemptTime`: `str`
- `LatestNotificationAttemptSucceeded`: `str`
- `LatestDeliveryAttemptSucceeded`: `str`
- `TimeLoggingStarted`: `str`
- `TimeLoggingStopped`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="insightselectortypedef"></a>

## InsightSelectorTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import InsightSelectorTypeDef
```

Optional fields:

- `InsightType`: [InsightTypeType](./literals.md#insighttypetype)

<a id="listeventdatastoresrequestrequesttypedef"></a>

## ListEventDataStoresRequestRequestTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import ListEventDataStoresRequestRequestTypeDef
```

Optional fields:

- `NextToken`: `str`
- `MaxResults`: `int`

<a id="listeventdatastoresresponsetypedef"></a>

## ListEventDataStoresResponseTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import ListEventDataStoresResponseTypeDef
```

Required fields:

- `EventDataStores`:
  `List`\[[EventDataStoreTypeDef](./type_defs.md#eventdatastoretypedef)\]
- `NextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listpublickeysrequestrequesttypedef"></a>

## ListPublicKeysRequestRequestTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import ListPublicKeysRequestRequestTypeDef
```

Optional fields:

- `StartTime`: `Union`\[`datetime`, `str`\]
- `EndTime`: `Union`\[`datetime`, `str`\]
- `NextToken`: `str`

<a id="listpublickeysresponsetypedef"></a>

## ListPublicKeysResponseTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import ListPublicKeysResponseTypeDef
```

Required fields:

- `PublicKeyList`:
  `List`\[[PublicKeyTypeDef](./type_defs.md#publickeytypedef)\]
- `NextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listqueriesrequestrequesttypedef"></a>

## ListQueriesRequestRequestTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import ListQueriesRequestRequestTypeDef
```

Required fields:

- `EventDataStore`: `str`

Optional fields:

- `NextToken`: `str`
- `MaxResults`: `int`
- `StartTime`: `Union`\[`datetime`, `str`\]
- `EndTime`: `Union`\[`datetime`, `str`\]
- `QueryStatus`: [QueryStatusType](./literals.md#querystatustype)

<a id="listqueriesresponsetypedef"></a>

## ListQueriesResponseTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import ListQueriesResponseTypeDef
```

Required fields:

- `Queries`: `List`\[[QueryTypeDef](./type_defs.md#querytypedef)\]
- `NextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listtagsrequestrequesttypedef"></a>

## ListTagsRequestRequestTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import ListTagsRequestRequestTypeDef
```

Required fields:

- `ResourceIdList`: `Sequence`\[`str`\]

Optional fields:

- `NextToken`: `str`

<a id="listtagsresponsetypedef"></a>

## ListTagsResponseTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import ListTagsResponseTypeDef
```

Required fields:

- `ResourceTagList`:
  `List`\[[ResourceTagTypeDef](./type_defs.md#resourcetagtypedef)\]
- `NextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listtrailsrequestrequesttypedef"></a>

## ListTrailsRequestRequestTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import ListTrailsRequestRequestTypeDef
```

Optional fields:

- `NextToken`: `str`

<a id="listtrailsresponsetypedef"></a>

## ListTrailsResponseTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import ListTrailsResponseTypeDef
```

Required fields:

- `Trails`: `List`\[[TrailInfoTypeDef](./type_defs.md#trailinfotypedef)\]
- `NextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="lookupattributetypedef"></a>

## LookupAttributeTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import LookupAttributeTypeDef
```

Required fields:

- `AttributeKey`:
  [LookupAttributeKeyType](./literals.md#lookupattributekeytype)
- `AttributeValue`: `str`

<a id="lookupeventsrequestrequesttypedef"></a>

## LookupEventsRequestRequestTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import LookupEventsRequestRequestTypeDef
```

Optional fields:

- `LookupAttributes`:
  `Sequence`\[[LookupAttributeTypeDef](./type_defs.md#lookupattributetypedef)\]
- `StartTime`: `Union`\[`datetime`, `str`\]
- `EndTime`: `Union`\[`datetime`, `str`\]
- `EventCategory`: `Literal['insight']` (see
  [EventCategoryType](./literals.md#eventcategorytype))
- `MaxResults`: `int`
- `NextToken`: `str`

<a id="lookupeventsresponsetypedef"></a>

## LookupEventsResponseTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import LookupEventsResponseTypeDef
```

Required fields:

- `Events`: `List`\[[EventTypeDef](./type_defs.md#eventtypedef)\]
- `NextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="paginatorconfigtypedef"></a>

## PaginatorConfigTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import PaginatorConfigTypeDef
```

Optional fields:

- `MaxItems`: `int`
- `PageSize`: `int`
- `StartingToken`: `str`

<a id="publickeytypedef"></a>

## PublicKeyTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import PublicKeyTypeDef
```

Optional fields:

- `Value`: `bytes`
- `ValidityStartTime`: `datetime`
- `ValidityEndTime`: `datetime`
- `Fingerprint`: `str`

<a id="puteventselectorsrequestrequesttypedef"></a>

## PutEventSelectorsRequestRequestTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import PutEventSelectorsRequestRequestTypeDef
```

Required fields:

- `TrailName`: `str`

Optional fields:

- `EventSelectors`:
  `Sequence`\[[EventSelectorTypeDef](./type_defs.md#eventselectortypedef)\]
- `AdvancedEventSelectors`:
  `Sequence`\[[AdvancedEventSelectorTypeDef](./type_defs.md#advancedeventselectortypedef)\]

<a id="puteventselectorsresponsetypedef"></a>

## PutEventSelectorsResponseTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import PutEventSelectorsResponseTypeDef
```

Required fields:

- `TrailARN`: `str`
- `EventSelectors`:
  `List`\[[EventSelectorTypeDef](./type_defs.md#eventselectortypedef)\]
- `AdvancedEventSelectors`:
  `List`\[[AdvancedEventSelectorTypeDef](./type_defs.md#advancedeventselectortypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="putinsightselectorsrequestrequesttypedef"></a>

## PutInsightSelectorsRequestRequestTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import PutInsightSelectorsRequestRequestTypeDef
```

Required fields:

- `TrailName`: `str`
- `InsightSelectors`:
  `Sequence`\[[InsightSelectorTypeDef](./type_defs.md#insightselectortypedef)\]

<a id="putinsightselectorsresponsetypedef"></a>

## PutInsightSelectorsResponseTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import PutInsightSelectorsResponseTypeDef
```

Required fields:

- `TrailARN`: `str`
- `InsightSelectors`:
  `List`\[[InsightSelectorTypeDef](./type_defs.md#insightselectortypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="querystatisticsfordescribequerytypedef"></a>

## QueryStatisticsForDescribeQueryTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import QueryStatisticsForDescribeQueryTypeDef
```

Optional fields:

- `EventsMatched`: `int`
- `EventsScanned`: `int`
- `BytesScanned`: `int`
- `ExecutionTimeInMillis`: `int`
- `CreationTime`: `datetime`

<a id="querystatisticstypedef"></a>

## QueryStatisticsTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import QueryStatisticsTypeDef
```

Optional fields:

- `ResultsCount`: `int`
- `TotalResultsCount`: `int`
- `BytesScanned`: `int`

<a id="querytypedef"></a>

## QueryTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import QueryTypeDef
```

Optional fields:

- `QueryId`: `str`
- `QueryStatus`: [QueryStatusType](./literals.md#querystatustype)
- `CreationTime`: `datetime`

<a id="removetagsrequestrequesttypedef"></a>

## RemoveTagsRequestRequestTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import RemoveTagsRequestRequestTypeDef
```

Required fields:

- `ResourceId`: `str`
- `TagsList`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

<a id="resourcetagtypedef"></a>

## ResourceTagTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import ResourceTagTypeDef
```

Optional fields:

- `ResourceId`: `str`
- `TagsList`: `List`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

<a id="resourcetypedef"></a>

## ResourceTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import ResourceTypeDef
```

Optional fields:

- `ResourceType`: `str`
- `ResourceName`: `str`

<a id="responsemetadatatypedef"></a>

## ResponseMetadataTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import ResponseMetadataTypeDef
```

Required fields:

- `RequestId`: `str`
- `HostId`: `str`
- `HTTPStatusCode`: `int`
- `HTTPHeaders`: `Dict`\[`str`, `str`\]
- `RetryAttempts`: `int`

<a id="restoreeventdatastorerequestrequesttypedef"></a>

## RestoreEventDataStoreRequestRequestTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import RestoreEventDataStoreRequestRequestTypeDef
```

Required fields:

- `EventDataStore`: `str`

<a id="restoreeventdatastoreresponsetypedef"></a>

## RestoreEventDataStoreResponseTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import RestoreEventDataStoreResponseTypeDef
```

Required fields:

- `EventDataStoreArn`: `str`
- `Name`: `str`
- `Status`: [EventDataStoreStatusType](./literals.md#eventdatastorestatustype)
- `AdvancedEventSelectors`:
  `List`\[[AdvancedEventSelectorTypeDef](./type_defs.md#advancedeventselectortypedef)\]
- `MultiRegionEnabled`: `bool`
- `OrganizationEnabled`: `bool`
- `RetentionPeriod`: `int`
- `TerminationProtectionEnabled`: `bool`
- `CreatedTimestamp`: `datetime`
- `UpdatedTimestamp`: `datetime`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="startloggingrequestrequesttypedef"></a>

## StartLoggingRequestRequestTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import StartLoggingRequestRequestTypeDef
```

Required fields:

- `Name`: `str`

<a id="startqueryrequestrequesttypedef"></a>

## StartQueryRequestRequestTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import StartQueryRequestRequestTypeDef
```

Required fields:

- `QueryStatement`: `str`

<a id="startqueryresponsetypedef"></a>

## StartQueryResponseTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import StartQueryResponseTypeDef
```

Required fields:

- `QueryId`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="stoploggingrequestrequesttypedef"></a>

## StopLoggingRequestRequestTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import StopLoggingRequestRequestTypeDef
```

Required fields:

- `Name`: `str`

<a id="tagtypedef"></a>

## TagTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import TagTypeDef
```

Required fields:

- `Key`: `str`

Optional fields:

- `Value`: `str`

<a id="trailinfotypedef"></a>

## TrailInfoTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import TrailInfoTypeDef
```

Optional fields:

- `TrailARN`: `str`
- `Name`: `str`
- `HomeRegion`: `str`

<a id="trailtypedef"></a>

## TrailTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import TrailTypeDef
```

Optional fields:

- `Name`: `str`
- `S3BucketName`: `str`
- `S3KeyPrefix`: `str`
- `SnsTopicName`: `str`
- `SnsTopicARN`: `str`
- `IncludeGlobalServiceEvents`: `bool`
- `IsMultiRegionTrail`: `bool`
- `HomeRegion`: `str`
- `TrailARN`: `str`
- `LogFileValidationEnabled`: `bool`
- `CloudWatchLogsLogGroupArn`: `str`
- `CloudWatchLogsRoleArn`: `str`
- `KmsKeyId`: `str`
- `HasCustomEventSelectors`: `bool`
- `HasInsightSelectors`: `bool`
- `IsOrganizationTrail`: `bool`

<a id="updateeventdatastorerequestrequesttypedef"></a>

## UpdateEventDataStoreRequestRequestTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import UpdateEventDataStoreRequestRequestTypeDef
```

Required fields:

- `EventDataStore`: `str`

Optional fields:

- `Name`: `str`
- `AdvancedEventSelectors`:
  `Sequence`\[[AdvancedEventSelectorTypeDef](./type_defs.md#advancedeventselectortypedef)\]
- `MultiRegionEnabled`: `bool`
- `OrganizationEnabled`: `bool`
- `RetentionPeriod`: `int`
- `TerminationProtectionEnabled`: `bool`

<a id="updateeventdatastoreresponsetypedef"></a>

## UpdateEventDataStoreResponseTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import UpdateEventDataStoreResponseTypeDef
```

Required fields:

- `EventDataStoreArn`: `str`
- `Name`: `str`
- `Status`: [EventDataStoreStatusType](./literals.md#eventdatastorestatustype)
- `AdvancedEventSelectors`:
  `List`\[[AdvancedEventSelectorTypeDef](./type_defs.md#advancedeventselectortypedef)\]
- `MultiRegionEnabled`: `bool`
- `OrganizationEnabled`: `bool`
- `RetentionPeriod`: `int`
- `TerminationProtectionEnabled`: `bool`
- `CreatedTimestamp`: `datetime`
- `UpdatedTimestamp`: `datetime`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="updatetrailrequestrequesttypedef"></a>

## UpdateTrailRequestRequestTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import UpdateTrailRequestRequestTypeDef
```

Required fields:

- `Name`: `str`

Optional fields:

- `S3BucketName`: `str`
- `S3KeyPrefix`: `str`
- `SnsTopicName`: `str`
- `IncludeGlobalServiceEvents`: `bool`
- `IsMultiRegionTrail`: `bool`
- `EnableLogFileValidation`: `bool`
- `CloudWatchLogsLogGroupArn`: `str`
- `CloudWatchLogsRoleArn`: `str`
- `KmsKeyId`: `str`
- `IsOrganizationTrail`: `bool`

<a id="updatetrailresponsetypedef"></a>

## UpdateTrailResponseTypeDef

```python
from types_aiobotocore_cloudtrail.type_defs import UpdateTrailResponseTypeDef
```

Required fields:

- `Name`: `str`
- `S3BucketName`: `str`
- `S3KeyPrefix`: `str`
- `SnsTopicName`: `str`
- `SnsTopicARN`: `str`
- `IncludeGlobalServiceEvents`: `bool`
- `IsMultiRegionTrail`: `bool`
- `TrailARN`: `str`
- `LogFileValidationEnabled`: `bool`
- `CloudWatchLogsLogGroupArn`: `str`
- `CloudWatchLogsRoleArn`: `str`
- `KmsKeyId`: `str`
- `IsOrganizationTrail`: `bool`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
