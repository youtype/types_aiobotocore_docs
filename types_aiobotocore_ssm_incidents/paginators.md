<a id="paginators-for-aiobotocore-ssmincidents-module"></a>

# Paginators for aiobotocore SSMIncidents module

> [Index](..) > [SSMIncidents](.) > Paginators

Auto-generated documentation for
[SSMIncidents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents)
type annotations stubs module
[types-aiobotocore-ssm-incidents](https://pypi.org/project/types-aiobotocore-ssm-incidents/).

- [Paginators for aiobotocore SSMIncidents module](#paginators-for-aiobotocore-ssmincidents-module)
  - [GetResourcePoliciesPaginator](#getresourcepoliciespaginator)
  - [ListIncidentRecordsPaginator](#listincidentrecordspaginator)
  - [ListRelatedItemsPaginator](#listrelateditemspaginator)
  - [ListReplicationSetsPaginator](#listreplicationsetspaginator)
  - [ListResponsePlansPaginator](#listresponseplanspaginator)
  - [ListTimelineEventsPaginator](#listtimelineeventspaginator)

<a id="getresourcepoliciespaginator"></a>

## GetResourcePoliciesPaginator

Type annotations for
`aiobotocore.create_client("ssm-incidents").get_paginator("get_resource_policies")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_ssm_incidents.paginator import GetResourcePoliciesPaginator

def get_get_resource_policies_paginator() -> GetResourcePoliciesPaginator:
    return Session().create_client("ssm-incidents").get_paginator("get_resource_policies")
```

Boto3 documentation:
[SSMIncidents.Paginator.GetResourcePolicies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.GetResourcePolicies)

Arguments for `GetResourcePoliciesPaginator.paginate` method:

- `resourceArn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetResourcePoliciesPaginator.paginate` returns
`_PageIterator`\[[GetResourcePoliciesOutputTypeDef](./type_defs.md#getresourcepoliciesoutputtypedef)\].

<a id="listincidentrecordspaginator"></a>

## ListIncidentRecordsPaginator

Type annotations for
`aiobotocore.create_client("ssm-incidents").get_paginator("list_incident_records")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_ssm_incidents.paginator import ListIncidentRecordsPaginator

def get_list_incident_records_paginator() -> ListIncidentRecordsPaginator:
    return Session().create_client("ssm-incidents").get_paginator("list_incident_records")
```

Boto3 documentation:
[SSMIncidents.Paginator.ListIncidentRecords](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListIncidentRecords)

Arguments for `ListIncidentRecordsPaginator.paginate` method:

- `filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListIncidentRecordsPaginator.paginate` returns
`_PageIterator`\[[ListIncidentRecordsOutputTypeDef](./type_defs.md#listincidentrecordsoutputtypedef)\].

<a id="listrelateditemspaginator"></a>

## ListRelatedItemsPaginator

Type annotations for
`aiobotocore.create_client("ssm-incidents").get_paginator("list_related_items")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_ssm_incidents.paginator import ListRelatedItemsPaginator

def get_list_related_items_paginator() -> ListRelatedItemsPaginator:
    return Session().create_client("ssm-incidents").get_paginator("list_related_items")
```

Boto3 documentation:
[SSMIncidents.Paginator.ListRelatedItems](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListRelatedItems)

Arguments for `ListRelatedItemsPaginator.paginate` method:

- `incidentRecordArn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRelatedItemsPaginator.paginate` returns
`_PageIterator`\[[ListRelatedItemsOutputTypeDef](./type_defs.md#listrelateditemsoutputtypedef)\].

<a id="listreplicationsetspaginator"></a>

## ListReplicationSetsPaginator

Type annotations for
`aiobotocore.create_client("ssm-incidents").get_paginator("list_replication_sets")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_ssm_incidents.paginator import ListReplicationSetsPaginator

def get_list_replication_sets_paginator() -> ListReplicationSetsPaginator:
    return Session().create_client("ssm-incidents").get_paginator("list_replication_sets")
```

Boto3 documentation:
[SSMIncidents.Paginator.ListReplicationSets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListReplicationSets)

Arguments for `ListReplicationSetsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListReplicationSetsPaginator.paginate` returns
`_PageIterator`\[[ListReplicationSetsOutputTypeDef](./type_defs.md#listreplicationsetsoutputtypedef)\].

<a id="listresponseplanspaginator"></a>

## ListResponsePlansPaginator

Type annotations for
`aiobotocore.create_client("ssm-incidents").get_paginator("list_response_plans")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_ssm_incidents.paginator import ListResponsePlansPaginator

def get_list_response_plans_paginator() -> ListResponsePlansPaginator:
    return Session().create_client("ssm-incidents").get_paginator("list_response_plans")
```

Boto3 documentation:
[SSMIncidents.Paginator.ListResponsePlans](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListResponsePlans)

Arguments for `ListResponsePlansPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListResponsePlansPaginator.paginate` returns
`_PageIterator`\[[ListResponsePlansOutputTypeDef](./type_defs.md#listresponseplansoutputtypedef)\].

<a id="listtimelineeventspaginator"></a>

## ListTimelineEventsPaginator

Type annotations for
`aiobotocore.create_client("ssm-incidents").get_paginator("list_timeline_events")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_ssm_incidents.paginator import ListTimelineEventsPaginator

def get_list_timeline_events_paginator() -> ListTimelineEventsPaginator:
    return Session().create_client("ssm-incidents").get_paginator("list_timeline_events")
```

Boto3 documentation:
[SSMIncidents.Paginator.ListTimelineEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#SSMIncidents.Paginator.ListTimelineEvents)

Arguments for `ListTimelineEventsPaginator.paginate` method:

- `incidentRecordArn`: `str` *(required)*
- `filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `sortBy`: `Literal['EVENT_TIME']` (see
  [TimelineEventSortType](./literals.md#timelineeventsorttype))
- `sortOrder`: [SortOrderType](./literals.md#sortordertype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTimelineEventsPaginator.paginate` returns
`_PageIterator`\[[ListTimelineEventsOutputTypeDef](./type_defs.md#listtimelineeventsoutputtypedef)\].
