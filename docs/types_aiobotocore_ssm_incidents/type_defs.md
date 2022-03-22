<a id="typed-dictionaries-for-aiobotocore-ssmincidents-module"></a>

# Typed dictionaries for aiobotocore SSMIncidents module

> [Index](../README.md) > [SSMIncidents](./README.md) > Typed dictionaries

Auto-generated documentation for
[SSMIncidents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
type annotations stubs module
[types-aiobotocore-ssm-incidents](https://pypi.org/project/types-aiobotocore-ssm-incidents/).

- [Typed dictionaries for aiobotocore SSMIncidents module](#typed-dictionaries-for-aiobotocore-ssmincidents-module)
  - [ActionTypeDef](#actiontypedef)
  - [AddRegionActionTypeDef](#addregionactiontypedef)
  - [AttributeValueListTypeDef](#attributevaluelisttypedef)
  - [AutomationExecutionTypeDef](#automationexecutiontypedef)
  - [ChatChannelTypeDef](#chatchanneltypedef)
  - [ConditionTypeDef](#conditiontypedef)
  - [CreateReplicationSetInputRequestTypeDef](#createreplicationsetinputrequesttypedef)
  - [CreateReplicationSetOutputTypeDef](#createreplicationsetoutputtypedef)
  - [CreateResponsePlanInputRequestTypeDef](#createresponseplaninputrequesttypedef)
  - [CreateResponsePlanOutputTypeDef](#createresponseplanoutputtypedef)
  - [CreateTimelineEventInputRequestTypeDef](#createtimelineeventinputrequesttypedef)
  - [CreateTimelineEventOutputTypeDef](#createtimelineeventoutputtypedef)
  - [DeleteIncidentRecordInputRequestTypeDef](#deleteincidentrecordinputrequesttypedef)
  - [DeleteRegionActionTypeDef](#deleteregionactiontypedef)
  - [DeleteReplicationSetInputRequestTypeDef](#deletereplicationsetinputrequesttypedef)
  - [DeleteResourcePolicyInputRequestTypeDef](#deleteresourcepolicyinputrequesttypedef)
  - [DeleteResponsePlanInputRequestTypeDef](#deleteresponseplaninputrequesttypedef)
  - [DeleteTimelineEventInputRequestTypeDef](#deletetimelineeventinputrequesttypedef)
  - [EventSummaryTypeDef](#eventsummarytypedef)
  - [FilterTypeDef](#filtertypedef)
  - [GetIncidentRecordInputRequestTypeDef](#getincidentrecordinputrequesttypedef)
  - [GetIncidentRecordOutputTypeDef](#getincidentrecordoutputtypedef)
  - [GetReplicationSetInputRequestTypeDef](#getreplicationsetinputrequesttypedef)
  - [GetReplicationSetOutputTypeDef](#getreplicationsetoutputtypedef)
  - [GetResourcePoliciesInputRequestTypeDef](#getresourcepoliciesinputrequesttypedef)
  - [GetResourcePoliciesOutputTypeDef](#getresourcepoliciesoutputtypedef)
  - [GetResponsePlanInputRequestTypeDef](#getresponseplaninputrequesttypedef)
  - [GetResponsePlanOutputTypeDef](#getresponseplanoutputtypedef)
  - [GetTimelineEventInputRequestTypeDef](#gettimelineeventinputrequesttypedef)
  - [GetTimelineEventOutputTypeDef](#gettimelineeventoutputtypedef)
  - [IncidentRecordSourceTypeDef](#incidentrecordsourcetypedef)
  - [IncidentRecordSummaryTypeDef](#incidentrecordsummarytypedef)
  - [IncidentRecordTypeDef](#incidentrecordtypedef)
  - [IncidentTemplateTypeDef](#incidenttemplatetypedef)
  - [ItemIdentifierTypeDef](#itemidentifiertypedef)
  - [ItemValueTypeDef](#itemvaluetypedef)
  - [ListIncidentRecordsInputRequestTypeDef](#listincidentrecordsinputrequesttypedef)
  - [ListIncidentRecordsOutputTypeDef](#listincidentrecordsoutputtypedef)
  - [ListRelatedItemsInputRequestTypeDef](#listrelateditemsinputrequesttypedef)
  - [ListRelatedItemsOutputTypeDef](#listrelateditemsoutputtypedef)
  - [ListReplicationSetsInputRequestTypeDef](#listreplicationsetsinputrequesttypedef)
  - [ListReplicationSetsOutputTypeDef](#listreplicationsetsoutputtypedef)
  - [ListResponsePlansInputRequestTypeDef](#listresponseplansinputrequesttypedef)
  - [ListResponsePlansOutputTypeDef](#listresponseplansoutputtypedef)
  - [ListTagsForResourceRequestRequestTypeDef](#listtagsforresourcerequestrequesttypedef)
  - [ListTagsForResourceResponseTypeDef](#listtagsforresourceresponsetypedef)
  - [ListTimelineEventsInputRequestTypeDef](#listtimelineeventsinputrequesttypedef)
  - [ListTimelineEventsOutputTypeDef](#listtimelineeventsoutputtypedef)
  - [NotificationTargetItemTypeDef](#notificationtargetitemtypedef)
  - [PaginatorConfigTypeDef](#paginatorconfigtypedef)
  - [PutResourcePolicyInputRequestTypeDef](#putresourcepolicyinputrequesttypedef)
  - [PutResourcePolicyOutputTypeDef](#putresourcepolicyoutputtypedef)
  - [RegionInfoTypeDef](#regioninfotypedef)
  - [RegionMapInputValueTypeDef](#regionmapinputvaluetypedef)
  - [RelatedItemTypeDef](#relateditemtypedef)
  - [RelatedItemsUpdateTypeDef](#relateditemsupdatetypedef)
  - [ReplicationSetTypeDef](#replicationsettypedef)
  - [ResourcePolicyTypeDef](#resourcepolicytypedef)
  - [ResponseMetadataTypeDef](#responsemetadatatypedef)
  - [ResponsePlanSummaryTypeDef](#responseplansummarytypedef)
  - [SsmAutomationTypeDef](#ssmautomationtypedef)
  - [StartIncidentInputRequestTypeDef](#startincidentinputrequesttypedef)
  - [StartIncidentOutputTypeDef](#startincidentoutputtypedef)
  - [TagResourceRequestRequestTypeDef](#tagresourcerequestrequesttypedef)
  - [TimelineEventTypeDef](#timelineeventtypedef)
  - [TriggerDetailsTypeDef](#triggerdetailstypedef)
  - [UntagResourceRequestRequestTypeDef](#untagresourcerequestrequesttypedef)
  - [UpdateDeletionProtectionInputRequestTypeDef](#updatedeletionprotectioninputrequesttypedef)
  - [UpdateIncidentRecordInputRequestTypeDef](#updateincidentrecordinputrequesttypedef)
  - [UpdateRelatedItemsInputRequestTypeDef](#updaterelateditemsinputrequesttypedef)
  - [UpdateReplicationSetActionTypeDef](#updatereplicationsetactiontypedef)
  - [UpdateReplicationSetInputRequestTypeDef](#updatereplicationsetinputrequesttypedef)
  - [UpdateResponsePlanInputRequestTypeDef](#updateresponseplaninputrequesttypedef)
  - [UpdateTimelineEventInputRequestTypeDef](#updatetimelineeventinputrequesttypedef)
  - [WaiterConfigTypeDef](#waiterconfigtypedef)

<a id="actiontypedef"></a>

## ActionTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import ActionTypeDef
```

Optional fields:

- `ssmAutomation`: [SsmAutomationTypeDef](./type_defs.md#ssmautomationtypedef)

<a id="addregionactiontypedef"></a>

## AddRegionActionTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import AddRegionActionTypeDef
```

Required fields:

- `regionName`: `str`

Optional fields:

- `sseKmsKeyId`: `str`

<a id="attributevaluelisttypedef"></a>

## AttributeValueListTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import AttributeValueListTypeDef
```

Optional fields:

- `integerValues`: `Sequence`\[`int`\]
- `stringValues`: `Sequence`\[`str`\]

<a id="automationexecutiontypedef"></a>

## AutomationExecutionTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import AutomationExecutionTypeDef
```

Optional fields:

- `ssmExecutionArn`: `str`

<a id="chatchanneltypedef"></a>

## ChatChannelTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import ChatChannelTypeDef
```

Optional fields:

- `chatbotSns`: `Sequence`\[`str`\]
- `empty`: `Mapping`\[`str`, `Any`\]

<a id="conditiontypedef"></a>

## ConditionTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import ConditionTypeDef
```

Optional fields:

- `after`: `Union`\[`datetime`, `str`\]
- `before`: `Union`\[`datetime`, `str`\]
- `equals`:
  [AttributeValueListTypeDef](./type_defs.md#attributevaluelisttypedef)

<a id="createreplicationsetinputrequesttypedef"></a>

## CreateReplicationSetInputRequestTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import CreateReplicationSetInputRequestTypeDef
```

Required fields:

- `regions`: `Mapping`\[`str`,
  [RegionMapInputValueTypeDef](./type_defs.md#regionmapinputvaluetypedef)\]

Optional fields:

- `clientToken`: `str`

<a id="createreplicationsetoutputtypedef"></a>

## CreateReplicationSetOutputTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import CreateReplicationSetOutputTypeDef
```

Required fields:

- `arn`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createresponseplaninputrequesttypedef"></a>

## CreateResponsePlanInputRequestTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import CreateResponsePlanInputRequestTypeDef
```

Required fields:

- `incidentTemplate`:
  [IncidentTemplateTypeDef](./type_defs.md#incidenttemplatetypedef)
- `name`: `str`

Optional fields:

- `actions`: `Sequence`\[[ActionTypeDef](./type_defs.md#actiontypedef)\]
- `chatChannel`: [ChatChannelTypeDef](./type_defs.md#chatchanneltypedef)
- `clientToken`: `str`
- `displayName`: `str`
- `engagements`: `Sequence`\[`str`\]
- `tags`: `Mapping`\[`str`, `str`\]

<a id="createresponseplanoutputtypedef"></a>

## CreateResponsePlanOutputTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import CreateResponsePlanOutputTypeDef
```

Required fields:

- `arn`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createtimelineeventinputrequesttypedef"></a>

## CreateTimelineEventInputRequestTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import CreateTimelineEventInputRequestTypeDef
```

Required fields:

- `eventData`: `str`
- `eventTime`: `Union`\[`datetime`, `str`\]
- `eventType`: `str`
- `incidentRecordArn`: `str`

Optional fields:

- `clientToken`: `str`

<a id="createtimelineeventoutputtypedef"></a>

## CreateTimelineEventOutputTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import CreateTimelineEventOutputTypeDef
```

Required fields:

- `eventId`: `str`
- `incidentRecordArn`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="deleteincidentrecordinputrequesttypedef"></a>

## DeleteIncidentRecordInputRequestTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import DeleteIncidentRecordInputRequestTypeDef
```

Required fields:

- `arn`: `str`

<a id="deleteregionactiontypedef"></a>

## DeleteRegionActionTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import DeleteRegionActionTypeDef
```

Required fields:

- `regionName`: `str`

<a id="deletereplicationsetinputrequesttypedef"></a>

## DeleteReplicationSetInputRequestTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import DeleteReplicationSetInputRequestTypeDef
```

Required fields:

- `arn`: `str`

<a id="deleteresourcepolicyinputrequesttypedef"></a>

## DeleteResourcePolicyInputRequestTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import DeleteResourcePolicyInputRequestTypeDef
```

Required fields:

- `policyId`: `str`
- `resourceArn`: `str`

<a id="deleteresponseplaninputrequesttypedef"></a>

## DeleteResponsePlanInputRequestTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import DeleteResponsePlanInputRequestTypeDef
```

Required fields:

- `arn`: `str`

<a id="deletetimelineeventinputrequesttypedef"></a>

## DeleteTimelineEventInputRequestTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import DeleteTimelineEventInputRequestTypeDef
```

Required fields:

- `eventId`: `str`
- `incidentRecordArn`: `str`

<a id="eventsummarytypedef"></a>

## EventSummaryTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import EventSummaryTypeDef
```

Required fields:

- `eventId`: `str`
- `eventTime`: `datetime`
- `eventType`: `str`
- `eventUpdatedTime`: `datetime`
- `incidentRecordArn`: `str`

<a id="filtertypedef"></a>

## FilterTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import FilterTypeDef
```

Required fields:

- `condition`: [ConditionTypeDef](./type_defs.md#conditiontypedef)
- `key`: `str`

<a id="getincidentrecordinputrequesttypedef"></a>

## GetIncidentRecordInputRequestTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import GetIncidentRecordInputRequestTypeDef
```

Required fields:

- `arn`: `str`

<a id="getincidentrecordoutputtypedef"></a>

## GetIncidentRecordOutputTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import GetIncidentRecordOutputTypeDef
```

Required fields:

- `incidentRecord`:
  [IncidentRecordTypeDef](./type_defs.md#incidentrecordtypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getreplicationsetinputrequesttypedef"></a>

## GetReplicationSetInputRequestTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import GetReplicationSetInputRequestTypeDef
```

Required fields:

- `arn`: `str`

<a id="getreplicationsetoutputtypedef"></a>

## GetReplicationSetOutputTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import GetReplicationSetOutputTypeDef
```

Required fields:

- `replicationSet`:
  [ReplicationSetTypeDef](./type_defs.md#replicationsettypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getresourcepoliciesinputrequesttypedef"></a>

## GetResourcePoliciesInputRequestTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import GetResourcePoliciesInputRequestTypeDef
```

Required fields:

- `resourceArn`: `str`

Optional fields:

- `maxResults`: `int`
- `nextToken`: `str`

<a id="getresourcepoliciesoutputtypedef"></a>

## GetResourcePoliciesOutputTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import GetResourcePoliciesOutputTypeDef
```

Required fields:

- `nextToken`: `str`
- `resourcePolicies`:
  `List`\[[ResourcePolicyTypeDef](./type_defs.md#resourcepolicytypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getresponseplaninputrequesttypedef"></a>

## GetResponsePlanInputRequestTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import GetResponsePlanInputRequestTypeDef
```

Required fields:

- `arn`: `str`

<a id="getresponseplanoutputtypedef"></a>

## GetResponsePlanOutputTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import GetResponsePlanOutputTypeDef
```

Required fields:

- `actions`: `List`\[[ActionTypeDef](./type_defs.md#actiontypedef)\]
- `arn`: `str`
- `chatChannel`: [ChatChannelTypeDef](./type_defs.md#chatchanneltypedef)
- `displayName`: `str`
- `engagements`: `List`\[`str`\]
- `incidentTemplate`:
  [IncidentTemplateTypeDef](./type_defs.md#incidenttemplatetypedef)
- `name`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="gettimelineeventinputrequesttypedef"></a>

## GetTimelineEventInputRequestTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import GetTimelineEventInputRequestTypeDef
```

Required fields:

- `eventId`: `str`
- `incidentRecordArn`: `str`

<a id="gettimelineeventoutputtypedef"></a>

## GetTimelineEventOutputTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import GetTimelineEventOutputTypeDef
```

Required fields:

- `event`: [TimelineEventTypeDef](./type_defs.md#timelineeventtypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="incidentrecordsourcetypedef"></a>

## IncidentRecordSourceTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import IncidentRecordSourceTypeDef
```

Required fields:

- `createdBy`: `str`
- `source`: `str`

Optional fields:

- `invokedBy`: `str`
- `resourceArn`: `str`

<a id="incidentrecordsummarytypedef"></a>

## IncidentRecordSummaryTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import IncidentRecordSummaryTypeDef
```

Required fields:

- `arn`: `str`
- `creationTime`: `datetime`
- `impact`: `int`
- `incidentRecordSource`:
  [IncidentRecordSourceTypeDef](./type_defs.md#incidentrecordsourcetypedef)
- `status`: [IncidentRecordStatusType](./literals.md#incidentrecordstatustype)
- `title`: `str`

Optional fields:

- `resolvedTime`: `datetime`

<a id="incidentrecordtypedef"></a>

## IncidentRecordTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import IncidentRecordTypeDef
```

Required fields:

- `arn`: `str`
- `creationTime`: `datetime`
- `dedupeString`: `str`
- `impact`: `int`
- `incidentRecordSource`:
  [IncidentRecordSourceTypeDef](./type_defs.md#incidentrecordsourcetypedef)
- `lastModifiedBy`: `str`
- `lastModifiedTime`: `datetime`
- `status`: [IncidentRecordStatusType](./literals.md#incidentrecordstatustype)
- `title`: `str`

Optional fields:

- `automationExecutions`:
  `List`\[[AutomationExecutionTypeDef](./type_defs.md#automationexecutiontypedef)\]
- `chatChannel`: [ChatChannelTypeDef](./type_defs.md#chatchanneltypedef)
- `notificationTargets`:
  `List`\[[NotificationTargetItemTypeDef](./type_defs.md#notificationtargetitemtypedef)\]
- `resolvedTime`: `datetime`
- `summary`: `str`

<a id="incidenttemplatetypedef"></a>

## IncidentTemplateTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import IncidentTemplateTypeDef
```

Required fields:

- `impact`: `int`
- `title`: `str`

Optional fields:

- `dedupeString`: `str`
- `notificationTargets`:
  `Sequence`\[[NotificationTargetItemTypeDef](./type_defs.md#notificationtargetitemtypedef)\]
- `summary`: `str`

<a id="itemidentifiertypedef"></a>

## ItemIdentifierTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import ItemIdentifierTypeDef
```

Required fields:

- `type`: [ItemTypeType](./literals.md#itemtypetype)
- `value`: [ItemValueTypeDef](./type_defs.md#itemvaluetypedef)

<a id="itemvaluetypedef"></a>

## ItemValueTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import ItemValueTypeDef
```

Optional fields:

- `arn`: `str`
- `metricDefinition`: `str`
- `url`: `str`

<a id="listincidentrecordsinputrequesttypedef"></a>

## ListIncidentRecordsInputRequestTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import ListIncidentRecordsInputRequestTypeDef
```

Optional fields:

- `filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `maxResults`: `int`
- `nextToken`: `str`

<a id="listincidentrecordsoutputtypedef"></a>

## ListIncidentRecordsOutputTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import ListIncidentRecordsOutputTypeDef
```

Required fields:

- `incidentRecordSummaries`:
  `List`\[[IncidentRecordSummaryTypeDef](./type_defs.md#incidentrecordsummarytypedef)\]
- `nextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listrelateditemsinputrequesttypedef"></a>

## ListRelatedItemsInputRequestTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import ListRelatedItemsInputRequestTypeDef
```

Required fields:

- `incidentRecordArn`: `str`

Optional fields:

- `maxResults`: `int`
- `nextToken`: `str`

<a id="listrelateditemsoutputtypedef"></a>

## ListRelatedItemsOutputTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import ListRelatedItemsOutputTypeDef
```

Required fields:

- `nextToken`: `str`
- `relatedItems`:
  `List`\[[RelatedItemTypeDef](./type_defs.md#relateditemtypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listreplicationsetsinputrequesttypedef"></a>

## ListReplicationSetsInputRequestTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import ListReplicationSetsInputRequestTypeDef
```

Optional fields:

- `maxResults`: `int`
- `nextToken`: `str`

<a id="listreplicationsetsoutputtypedef"></a>

## ListReplicationSetsOutputTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import ListReplicationSetsOutputTypeDef
```

Required fields:

- `nextToken`: `str`
- `replicationSetArns`: `List`\[`str`\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listresponseplansinputrequesttypedef"></a>

## ListResponsePlansInputRequestTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import ListResponsePlansInputRequestTypeDef
```

Optional fields:

- `maxResults`: `int`
- `nextToken`: `str`

<a id="listresponseplansoutputtypedef"></a>

## ListResponsePlansOutputTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import ListResponsePlansOutputTypeDef
```

Required fields:

- `nextToken`: `str`
- `responsePlanSummaries`:
  `List`\[[ResponsePlanSummaryTypeDef](./type_defs.md#responseplansummarytypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listtagsforresourcerequestrequesttypedef"></a>

## ListTagsForResourceRequestRequestTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import ListTagsForResourceRequestRequestTypeDef
```

Required fields:

- `resourceArn`: `str`

<a id="listtagsforresourceresponsetypedef"></a>

## ListTagsForResourceResponseTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import ListTagsForResourceResponseTypeDef
```

Required fields:

- `tags`: `Dict`\[`str`, `str`\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listtimelineeventsinputrequesttypedef"></a>

## ListTimelineEventsInputRequestTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import ListTimelineEventsInputRequestTypeDef
```

Required fields:

- `incidentRecordArn`: `str`

Optional fields:

- `filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `maxResults`: `int`
- `nextToken`: `str`
- `sortBy`: `Literal['EVENT_TIME']` (see
  [TimelineEventSortType](./literals.md#timelineeventsorttype))
- `sortOrder`: [SortOrderType](./literals.md#sortordertype)

<a id="listtimelineeventsoutputtypedef"></a>

## ListTimelineEventsOutputTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import ListTimelineEventsOutputTypeDef
```

Required fields:

- `eventSummaries`:
  `List`\[[EventSummaryTypeDef](./type_defs.md#eventsummarytypedef)\]
- `nextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="notificationtargetitemtypedef"></a>

## NotificationTargetItemTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import NotificationTargetItemTypeDef
```

Optional fields:

- `snsTopicArn`: `str`

<a id="paginatorconfigtypedef"></a>

## PaginatorConfigTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import PaginatorConfigTypeDef
```

Optional fields:

- `MaxItems`: `int`
- `PageSize`: `int`
- `StartingToken`: `str`

<a id="putresourcepolicyinputrequesttypedef"></a>

## PutResourcePolicyInputRequestTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import PutResourcePolicyInputRequestTypeDef
```

Required fields:

- `policy`: `str`
- `resourceArn`: `str`

<a id="putresourcepolicyoutputtypedef"></a>

## PutResourcePolicyOutputTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import PutResourcePolicyOutputTypeDef
```

Required fields:

- `policyId`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="regioninfotypedef"></a>

## RegionInfoTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import RegionInfoTypeDef
```

Required fields:

- `status`: [RegionStatusType](./literals.md#regionstatustype)
- `statusUpdateDateTime`: `datetime`

Optional fields:

- `sseKmsKeyId`: `str`
- `statusMessage`: `str`

<a id="regionmapinputvaluetypedef"></a>

## RegionMapInputValueTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import RegionMapInputValueTypeDef
```

Optional fields:

- `sseKmsKeyId`: `str`

<a id="relateditemtypedef"></a>

## RelatedItemTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import RelatedItemTypeDef
```

Required fields:

- `identifier`: [ItemIdentifierTypeDef](./type_defs.md#itemidentifiertypedef)

Optional fields:

- `title`: `str`

<a id="relateditemsupdatetypedef"></a>

## RelatedItemsUpdateTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import RelatedItemsUpdateTypeDef
```

Optional fields:

- `itemToAdd`: [RelatedItemTypeDef](./type_defs.md#relateditemtypedef)
- `itemToRemove`: [ItemIdentifierTypeDef](./type_defs.md#itemidentifiertypedef)

<a id="replicationsettypedef"></a>

## ReplicationSetTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import ReplicationSetTypeDef
```

Required fields:

- `createdBy`: `str`
- `createdTime`: `datetime`
- `deletionProtected`: `bool`
- `lastModifiedBy`: `str`
- `lastModifiedTime`: `datetime`
- `regionMap`: `Dict`\[`str`,
  [RegionInfoTypeDef](./type_defs.md#regioninfotypedef)\]
- `status`: [ReplicationSetStatusType](./literals.md#replicationsetstatustype)

Optional fields:

- `arn`: `str`

<a id="resourcepolicytypedef"></a>

## ResourcePolicyTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import ResourcePolicyTypeDef
```

Required fields:

- `policyDocument`: `str`
- `policyId`: `str`
- `ramResourceShareRegion`: `str`

<a id="responsemetadatatypedef"></a>

## ResponseMetadataTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import ResponseMetadataTypeDef
```

Required fields:

- `RequestId`: `str`
- `HostId`: `str`
- `HTTPStatusCode`: `int`
- `HTTPHeaders`: `Dict`\[`str`, `str`\]
- `RetryAttempts`: `int`

<a id="responseplansummarytypedef"></a>

## ResponsePlanSummaryTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import ResponsePlanSummaryTypeDef
```

Required fields:

- `arn`: `str`
- `name`: `str`

Optional fields:

- `displayName`: `str`

<a id="ssmautomationtypedef"></a>

## SsmAutomationTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import SsmAutomationTypeDef
```

Required fields:

- `documentName`: `str`
- `roleArn`: `str`

Optional fields:

- `documentVersion`: `str`
- `parameters`: `Mapping`\[`str`, `Sequence`\[`str`\]\]
- `targetAccount`: [SsmTargetAccountType](./literals.md#ssmtargetaccounttype)

<a id="startincidentinputrequesttypedef"></a>

## StartIncidentInputRequestTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import StartIncidentInputRequestTypeDef
```

Required fields:

- `responsePlanArn`: `str`

Optional fields:

- `clientToken`: `str`
- `impact`: `int`
- `relatedItems`:
  `Sequence`\[[RelatedItemTypeDef](./type_defs.md#relateditemtypedef)\]
- `title`: `str`
- `triggerDetails`:
  [TriggerDetailsTypeDef](./type_defs.md#triggerdetailstypedef)

<a id="startincidentoutputtypedef"></a>

## StartIncidentOutputTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import StartIncidentOutputTypeDef
```

Required fields:

- `incidentRecordArn`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="tagresourcerequestrequesttypedef"></a>

## TagResourceRequestRequestTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import TagResourceRequestRequestTypeDef
```

Required fields:

- `resourceArn`: `str`
- `tags`: `Mapping`\[`str`, `str`\]

<a id="timelineeventtypedef"></a>

## TimelineEventTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import TimelineEventTypeDef
```

Required fields:

- `eventData`: `str`
- `eventId`: `str`
- `eventTime`: `datetime`
- `eventType`: `str`
- `eventUpdatedTime`: `datetime`
- `incidentRecordArn`: `str`

<a id="triggerdetailstypedef"></a>

## TriggerDetailsTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import TriggerDetailsTypeDef
```

Required fields:

- `source`: `str`
- `timestamp`: `Union`\[`datetime`, `str`\]

Optional fields:

- `rawData`: `str`
- `triggerArn`: `str`

<a id="untagresourcerequestrequesttypedef"></a>

## UntagResourceRequestRequestTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import UntagResourceRequestRequestTypeDef
```

Required fields:

- `resourceArn`: `str`
- `tagKeys`: `Sequence`\[`str`\]

<a id="updatedeletionprotectioninputrequesttypedef"></a>

## UpdateDeletionProtectionInputRequestTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import UpdateDeletionProtectionInputRequestTypeDef
```

Required fields:

- `arn`: `str`
- `deletionProtected`: `bool`

Optional fields:

- `clientToken`: `str`

<a id="updateincidentrecordinputrequesttypedef"></a>

## UpdateIncidentRecordInputRequestTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import UpdateIncidentRecordInputRequestTypeDef
```

Required fields:

- `arn`: `str`

Optional fields:

- `chatChannel`: [ChatChannelTypeDef](./type_defs.md#chatchanneltypedef)
- `clientToken`: `str`
- `impact`: `int`
- `notificationTargets`:
  `Sequence`\[[NotificationTargetItemTypeDef](./type_defs.md#notificationtargetitemtypedef)\]
- `status`: [IncidentRecordStatusType](./literals.md#incidentrecordstatustype)
- `summary`: `str`
- `title`: `str`

<a id="updaterelateditemsinputrequesttypedef"></a>

## UpdateRelatedItemsInputRequestTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import UpdateRelatedItemsInputRequestTypeDef
```

Required fields:

- `incidentRecordArn`: `str`
- `relatedItemsUpdate`:
  [RelatedItemsUpdateTypeDef](./type_defs.md#relateditemsupdatetypedef)

Optional fields:

- `clientToken`: `str`

<a id="updatereplicationsetactiontypedef"></a>

## UpdateReplicationSetActionTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import UpdateReplicationSetActionTypeDef
```

Optional fields:

- `addRegionAction`:
  [AddRegionActionTypeDef](./type_defs.md#addregionactiontypedef)
- `deleteRegionAction`:
  [DeleteRegionActionTypeDef](./type_defs.md#deleteregionactiontypedef)

<a id="updatereplicationsetinputrequesttypedef"></a>

## UpdateReplicationSetInputRequestTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import UpdateReplicationSetInputRequestTypeDef
```

Required fields:

- `actions`:
  `Sequence`\[[UpdateReplicationSetActionTypeDef](./type_defs.md#updatereplicationsetactiontypedef)\]
- `arn`: `str`

Optional fields:

- `clientToken`: `str`

<a id="updateresponseplaninputrequesttypedef"></a>

## UpdateResponsePlanInputRequestTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import UpdateResponsePlanInputRequestTypeDef
```

Required fields:

- `arn`: `str`

Optional fields:

- `actions`: `Sequence`\[[ActionTypeDef](./type_defs.md#actiontypedef)\]
- `chatChannel`: [ChatChannelTypeDef](./type_defs.md#chatchanneltypedef)
- `clientToken`: `str`
- `displayName`: `str`
- `engagements`: `Sequence`\[`str`\]
- `incidentTemplateDedupeString`: `str`
- `incidentTemplateImpact`: `int`
- `incidentTemplateNotificationTargets`:
  `Sequence`\[[NotificationTargetItemTypeDef](./type_defs.md#notificationtargetitemtypedef)\]
- `incidentTemplateSummary`: `str`
- `incidentTemplateTitle`: `str`

<a id="updatetimelineeventinputrequesttypedef"></a>

## UpdateTimelineEventInputRequestTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import UpdateTimelineEventInputRequestTypeDef
```

Required fields:

- `eventId`: `str`
- `incidentRecordArn`: `str`

Optional fields:

- `clientToken`: `str`
- `eventData`: `str`
- `eventTime`: `Union`\[`datetime`, `str`\]
- `eventType`: `str`

<a id="waiterconfigtypedef"></a>

## WaiterConfigTypeDef

```python
from types_aiobotocore_ssm_incidents.type_defs import WaiterConfigTypeDef
```

Optional fields:

- `Delay`: `int`
- `MaxAttempts`: `int`
