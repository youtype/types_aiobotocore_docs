# SSMIncidents module

> [Index](../README.md) > SSMIncidents


!!! note ""

    Auto-generated documentation for [SSMIncidents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#ssmincidents)
    type annotations stubs module [types-aiobotocore-ssm-incidents](https://pypi.org/project/types-aiobotocore-ssm-incidents/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `SSMIncidents` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `SSMIncidents` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[ssm-incidents]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[ssm-incidents]'

# standalone installation
python -m pip install types-aiobotocore-ssm-incidents
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-ssm-incidents
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SSMIncidentsClient

Type annotations and code completion for  `#!python session.create_client("ssm-incidents")` as [SSMIncidentsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Client)

```python
# SSMIncidentsClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_ssm_incidents.client import SSMIncidentsClient


session = get_session()
async with session.create_client("ssm-incidents") as client:
    client: SSMIncidentsClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("ssm-incidents").get_paginator("...")`.

```python
# GetResourcePoliciesPaginator usage example

from types_aiobotocore_ssm_incidents.paginator import GetResourcePoliciesPaginator

def get_get_resource_policies_paginator() -> GetResourcePoliciesPaginator:
    return client.get_paginator("get_resource_policies"))
```

- [GetResourcePoliciesPaginator](./paginators.md#getresourcepoliciespaginator)
- [ListIncidentFindingsPaginator](./paginators.md#listincidentfindingspaginator)
- [ListIncidentRecordsPaginator](./paginators.md#listincidentrecordspaginator)
- [ListRelatedItemsPaginator](./paginators.md#listrelateditemspaginator)
- [ListReplicationSetsPaginator](./paginators.md#listreplicationsetspaginator)
- [ListResponsePlansPaginator](./paginators.md#listresponseplanspaginator)
- [ListTimelineEventsPaginator](./paginators.md#listtimelineeventspaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("ssm-incidents").get_waiter("...")`.

```python
# WaitForReplicationSetActiveWaiter usage example

from types_aiobotocore_ssm_incidents.waiter import WaitForReplicationSetActiveWaiter

def get_wait_for_replication_set_active_waiter() -> WaitForReplicationSetActiveWaiter:
    return Session().client("ssm-incidents").get_waiter("wait_for_replication_set_active")
```

- [WaitForReplicationSetActiveWaiter](./waiters.md#waitforreplicationsetactivewaiter)
- [WaitForReplicationSetDeletedWaiter](./waiters.md#waitforreplicationsetdeletedwaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# GetResourcePoliciesPaginatorName usage example

from types_aiobotocore_ssm_incidents.literals import GetResourcePoliciesPaginatorName

def get_value() -> GetResourcePoliciesPaginatorName:
    return "get_resource_policies"
```

- [GetResourcePoliciesPaginatorName](./literals.md#getresourcepoliciespaginatorname)
- [IncidentRecordStatusType](./literals.md#incidentrecordstatustype)
- [ItemTypeType](./literals.md#itemtypetype)
- [ListIncidentFindingsPaginatorName](./literals.md#listincidentfindingspaginatorname)
- [ListIncidentRecordsPaginatorName](./literals.md#listincidentrecordspaginatorname)
- [ListRelatedItemsPaginatorName](./literals.md#listrelateditemspaginatorname)
- [ListReplicationSetsPaginatorName](./literals.md#listreplicationsetspaginatorname)
- [ListResponsePlansPaginatorName](./literals.md#listresponseplanspaginatorname)
- [ListTimelineEventsPaginatorName](./literals.md#listtimelineeventspaginatorname)
- [RegionStatusType](./literals.md#regionstatustype)
- [ReplicationSetStatusType](./literals.md#replicationsetstatustype)
- [SortOrderType](./literals.md#sortordertype)
- [SsmTargetAccountType](./literals.md#ssmtargetaccounttype)
- [TimelineEventSortType](./literals.md#timelineeventsorttype)
- [VariableTypeType](./literals.md#variabletypetype)
- [WaitForReplicationSetActiveWaiterName](./literals.md#waitforreplicationsetactivewaitername)
- [WaitForReplicationSetDeletedWaiterName](./literals.md#waitforreplicationsetdeletedwaitername)
- [SSMIncidentsServiceName](./literals.md#ssmincidentsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AddRegionActionTypeDef](./type_defs.md#addregionactiontypedef)
- [AttributeValueListTypeDef](./type_defs.md#attributevaluelisttypedef)
- [AutomationExecutionTypeDef](./type_defs.md#automationexecutiontypedef)
- [BatchGetIncidentFindingsErrorTypeDef](./type_defs.md#batchgetincidentfindingserrortypedef)
- [BatchGetIncidentFindingsInputRequestTypeDef](./type_defs.md#batchgetincidentfindingsinputrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ChatChannelOutputTypeDef](./type_defs.md#chatchanneloutputtypedef)
- [ChatChannelTypeDef](./type_defs.md#chatchanneltypedef)
- [CloudFormationStackUpdateTypeDef](./type_defs.md#cloudformationstackupdatetypedef)
- [CodeDeployDeploymentTypeDef](./type_defs.md#codedeploydeploymenttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [RegionMapInputValueTypeDef](./type_defs.md#regionmapinputvaluetypedef)
- [EventReferenceTypeDef](./type_defs.md#eventreferencetypedef)
- [DeleteIncidentRecordInputRequestTypeDef](./type_defs.md#deleteincidentrecordinputrequesttypedef)
- [DeleteRegionActionTypeDef](./type_defs.md#deleteregionactiontypedef)
- [DeleteReplicationSetInputRequestTypeDef](./type_defs.md#deletereplicationsetinputrequesttypedef)
- [DeleteResourcePolicyInputRequestTypeDef](./type_defs.md#deleteresourcepolicyinputrequesttypedef)
- [DeleteResponsePlanInputRequestTypeDef](./type_defs.md#deleteresponseplaninputrequesttypedef)
- [DeleteTimelineEventInputRequestTypeDef](./type_defs.md#deletetimelineeventinputrequesttypedef)
- [DynamicSsmParameterValueTypeDef](./type_defs.md#dynamicssmparametervaluetypedef)
- [FindingSummaryTypeDef](./type_defs.md#findingsummarytypedef)
- [GetIncidentRecordInputRequestTypeDef](./type_defs.md#getincidentrecordinputrequesttypedef)
- [GetReplicationSetInputRequestTypeDef](./type_defs.md#getreplicationsetinputrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [GetResourcePoliciesInputRequestTypeDef](./type_defs.md#getresourcepoliciesinputrequesttypedef)
- [ResourcePolicyTypeDef](./type_defs.md#resourcepolicytypedef)
- [GetResponsePlanInputRequestTypeDef](./type_defs.md#getresponseplaninputrequesttypedef)
- [GetTimelineEventInputRequestTypeDef](./type_defs.md#gettimelineeventinputrequesttypedef)
- [IncidentRecordSourceTypeDef](./type_defs.md#incidentrecordsourcetypedef)
- [NotificationTargetItemTypeDef](./type_defs.md#notificationtargetitemtypedef)
- [PagerDutyIncidentDetailTypeDef](./type_defs.md#pagerdutyincidentdetailtypedef)
- [ListIncidentFindingsInputRequestTypeDef](./type_defs.md#listincidentfindingsinputrequesttypedef)
- [ListRelatedItemsInputRequestTypeDef](./type_defs.md#listrelateditemsinputrequesttypedef)
- [ListReplicationSetsInputRequestTypeDef](./type_defs.md#listreplicationsetsinputrequesttypedef)
- [ListResponsePlansInputRequestTypeDef](./type_defs.md#listresponseplansinputrequesttypedef)
- [ResponsePlanSummaryTypeDef](./type_defs.md#responseplansummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [PagerDutyIncidentConfigurationTypeDef](./type_defs.md#pagerdutyincidentconfigurationtypedef)
- [PutResourcePolicyInputRequestTypeDef](./type_defs.md#putresourcepolicyinputrequesttypedef)
- [RegionInfoTypeDef](./type_defs.md#regioninfotypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateDeletionProtectionInputRequestTypeDef](./type_defs.md#updatedeletionprotectioninputrequesttypedef)
- [CreateReplicationSetOutputTypeDef](./type_defs.md#createreplicationsetoutputtypedef)
- [CreateResponsePlanOutputTypeDef](./type_defs.md#createresponseplanoutputtypedef)
- [CreateTimelineEventOutputTypeDef](./type_defs.md#createtimelineeventoutputtypedef)
- [ListReplicationSetsOutputTypeDef](./type_defs.md#listreplicationsetsoutputtypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [PutResourcePolicyOutputTypeDef](./type_defs.md#putresourcepolicyoutputtypedef)
- [StartIncidentOutputTypeDef](./type_defs.md#startincidentoutputtypedef)
- [FindingDetailsTypeDef](./type_defs.md#findingdetailstypedef)
- [ConditionTypeDef](./type_defs.md#conditiontypedef)
- [TriggerDetailsTypeDef](./type_defs.md#triggerdetailstypedef)
- [CreateReplicationSetInputRequestTypeDef](./type_defs.md#createreplicationsetinputrequesttypedef)
- [CreateTimelineEventInputRequestTypeDef](./type_defs.md#createtimelineeventinputrequesttypedef)
- [EventSummaryTypeDef](./type_defs.md#eventsummarytypedef)
- [TimelineEventTypeDef](./type_defs.md#timelineeventtypedef)
- [UpdateTimelineEventInputRequestTypeDef](./type_defs.md#updatetimelineeventinputrequesttypedef)
- [UpdateReplicationSetActionTypeDef](./type_defs.md#updatereplicationsetactiontypedef)
- [SsmAutomationOutputTypeDef](./type_defs.md#ssmautomationoutputtypedef)
- [SsmAutomationTypeDef](./type_defs.md#ssmautomationtypedef)
- [ListIncidentFindingsOutputTypeDef](./type_defs.md#listincidentfindingsoutputtypedef)
- [GetReplicationSetInputWaitTypeDef](./type_defs.md#getreplicationsetinputwaittypedef)
- [GetResourcePoliciesInputPaginateTypeDef](./type_defs.md#getresourcepoliciesinputpaginatetypedef)
- [ListIncidentFindingsInputPaginateTypeDef](./type_defs.md#listincidentfindingsinputpaginatetypedef)
- [ListRelatedItemsInputPaginateTypeDef](./type_defs.md#listrelateditemsinputpaginatetypedef)
- [ListReplicationSetsInputPaginateTypeDef](./type_defs.md#listreplicationsetsinputpaginatetypedef)
- [ListResponsePlansInputPaginateTypeDef](./type_defs.md#listresponseplansinputpaginatetypedef)
- [GetResourcePoliciesOutputTypeDef](./type_defs.md#getresourcepoliciesoutputtypedef)
- [IncidentRecordSummaryTypeDef](./type_defs.md#incidentrecordsummarytypedef)
- [IncidentRecordTypeDef](./type_defs.md#incidentrecordtypedef)
- [IncidentTemplateOutputTypeDef](./type_defs.md#incidenttemplateoutputtypedef)
- [IncidentTemplateTypeDef](./type_defs.md#incidenttemplatetypedef)
- [UpdateIncidentRecordInputRequestTypeDef](./type_defs.md#updateincidentrecordinputrequesttypedef)
- [ItemValueTypeDef](./type_defs.md#itemvaluetypedef)
- [ListResponsePlansOutputTypeDef](./type_defs.md#listresponseplansoutputtypedef)
- [PagerDutyConfigurationTypeDef](./type_defs.md#pagerdutyconfigurationtypedef)
- [ReplicationSetTypeDef](./type_defs.md#replicationsettypedef)
- [FindingTypeDef](./type_defs.md#findingtypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [ListTimelineEventsOutputTypeDef](./type_defs.md#listtimelineeventsoutputtypedef)
- [GetTimelineEventOutputTypeDef](./type_defs.md#gettimelineeventoutputtypedef)
- [UpdateReplicationSetInputRequestTypeDef](./type_defs.md#updatereplicationsetinputrequesttypedef)
- [ActionOutputTypeDef](./type_defs.md#actionoutputtypedef)
- [SsmAutomationUnionTypeDef](./type_defs.md#ssmautomationuniontypedef)
- [ListIncidentRecordsOutputTypeDef](./type_defs.md#listincidentrecordsoutputtypedef)
- [GetIncidentRecordOutputTypeDef](./type_defs.md#getincidentrecordoutputtypedef)
- [ItemIdentifierTypeDef](./type_defs.md#itemidentifiertypedef)
- [IntegrationTypeDef](./type_defs.md#integrationtypedef)
- [GetReplicationSetOutputTypeDef](./type_defs.md#getreplicationsetoutputtypedef)
- [BatchGetIncidentFindingsOutputTypeDef](./type_defs.md#batchgetincidentfindingsoutputtypedef)
- [ListIncidentRecordsInputPaginateTypeDef](./type_defs.md#listincidentrecordsinputpaginatetypedef)
- [ListIncidentRecordsInputRequestTypeDef](./type_defs.md#listincidentrecordsinputrequesttypedef)
- [ListTimelineEventsInputPaginateTypeDef](./type_defs.md#listtimelineeventsinputpaginatetypedef)
- [ListTimelineEventsInputRequestTypeDef](./type_defs.md#listtimelineeventsinputrequesttypedef)
- [ActionTypeDef](./type_defs.md#actiontypedef)
- [RelatedItemTypeDef](./type_defs.md#relateditemtypedef)
- [GetResponsePlanOutputTypeDef](./type_defs.md#getresponseplanoutputtypedef)
- [ActionUnionTypeDef](./type_defs.md#actionuniontypedef)
- [UpdateResponsePlanInputRequestTypeDef](./type_defs.md#updateresponseplaninputrequesttypedef)
- [ListRelatedItemsOutputTypeDef](./type_defs.md#listrelateditemsoutputtypedef)
- [RelatedItemsUpdateTypeDef](./type_defs.md#relateditemsupdatetypedef)
- [StartIncidentInputRequestTypeDef](./type_defs.md#startincidentinputrequesttypedef)
- [CreateResponsePlanInputRequestTypeDef](./type_defs.md#createresponseplaninputrequesttypedef)
- [UpdateRelatedItemsInputRequestTypeDef](./type_defs.md#updaterelateditemsinputrequesttypedef)

