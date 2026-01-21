# Paginators

> [Index](../README.md) > [SSMIncidents](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [SSMIncidents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#ssmincidents)
    type annotations stubs module [types-aiobotocore-ssm-incidents](https://pypi.org/project/types-aiobotocore-ssm-incidents/).

## GetResourcePoliciesPaginator

Type annotations and code completion for `#!python session.create_client("ssm-incidents").get_paginator("get_resource_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents/paginator/GetResourcePolicies.html#SSMIncidents.Paginator.GetResourcePolicies)

```python
# GetResourcePoliciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ssm_incidents.paginator import GetResourcePoliciesPaginator

session = get_session()
async with session.create_client("ssm-incidents") as client:  # (1)
    paginator: GetResourcePoliciesPaginator = client.get_paginator("get_resource_policies")  # (2)
    async for item in paginator.paginate(...):
        item: GetResourcePoliciesOutputTypeDef
        print(item)  # (3)
```

1. client: [SSMIncidentsClient](./client.md)
2. paginator: [GetResourcePoliciesPaginator](./paginators.md#getresourcepoliciespaginator)
3. item: `AioPageIterator[GetResourcePoliciesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python GetResourcePoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    resourceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetResourcePoliciesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetResourcePoliciesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetResourcePoliciesInputPaginateTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetResourcePoliciesInputPaginateTypeDef](./type_defs.md#getresourcepoliciesinputpaginatetypedef)
## ListIncidentFindingsPaginator

Type annotations and code completion for `#!python session.create_client("ssm-incidents").get_paginator("list_incident_findings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents/paginator/ListIncidentFindings.html#SSMIncidents.Paginator.ListIncidentFindings)

```python
# ListIncidentFindingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ssm_incidents.paginator import ListIncidentFindingsPaginator

session = get_session()
async with session.create_client("ssm-incidents") as client:  # (1)
    paginator: ListIncidentFindingsPaginator = client.get_paginator("list_incident_findings")  # (2)
    async for item in paginator.paginate(...):
        item: ListIncidentFindingsOutputTypeDef
        print(item)  # (3)
```

1. client: [SSMIncidentsClient](./client.md)
2. paginator: [ListIncidentFindingsPaginator](./paginators.md#listincidentfindingspaginator)
3. item: `AioPageIterator[ListIncidentFindingsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListIncidentFindingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    incidentRecordArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListIncidentFindingsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListIncidentFindingsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListIncidentFindingsInputPaginateTypeDef = {  # (1)
    "incidentRecordArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIncidentFindingsInputPaginateTypeDef](./type_defs.md#listincidentfindingsinputpaginatetypedef)
## ListIncidentRecordsPaginator

Type annotations and code completion for `#!python session.create_client("ssm-incidents").get_paginator("list_incident_records")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents/paginator/ListIncidentRecords.html#SSMIncidents.Paginator.ListIncidentRecords)

```python
# ListIncidentRecordsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ssm_incidents.paginator import ListIncidentRecordsPaginator

session = get_session()
async with session.create_client("ssm-incidents") as client:  # (1)
    paginator: ListIncidentRecordsPaginator = client.get_paginator("list_incident_records")  # (2)
    async for item in paginator.paginate(...):
        item: ListIncidentRecordsOutputTypeDef
        print(item)  # (3)
```

1. client: [SSMIncidentsClient](./client.md)
2. paginator: [ListIncidentRecordsPaginator](./paginators.md#listincidentrecordspaginator)
3. item: `AioPageIterator[ListIncidentRecordsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListIncidentRecordsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListIncidentRecordsOutputTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListIncidentRecordsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListIncidentRecordsInputPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIncidentRecordsInputPaginateTypeDef](./type_defs.md#listincidentrecordsinputpaginatetypedef)
## ListRelatedItemsPaginator

Type annotations and code completion for `#!python session.create_client("ssm-incidents").get_paginator("list_related_items")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents/paginator/ListRelatedItems.html#SSMIncidents.Paginator.ListRelatedItems)

```python
# ListRelatedItemsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ssm_incidents.paginator import ListRelatedItemsPaginator

session = get_session()
async with session.create_client("ssm-incidents") as client:  # (1)
    paginator: ListRelatedItemsPaginator = client.get_paginator("list_related_items")  # (2)
    async for item in paginator.paginate(...):
        item: ListRelatedItemsOutputTypeDef
        print(item)  # (3)
```

1. client: [SSMIncidentsClient](./client.md)
2. paginator: [ListRelatedItemsPaginator](./paginators.md#listrelateditemspaginator)
3. item: `AioPageIterator[ListRelatedItemsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRelatedItemsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    incidentRecordArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListRelatedItemsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListRelatedItemsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRelatedItemsInputPaginateTypeDef = {  # (1)
    "incidentRecordArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRelatedItemsInputPaginateTypeDef](./type_defs.md#listrelateditemsinputpaginatetypedef)
## ListReplicationSetsPaginator

Type annotations and code completion for `#!python session.create_client("ssm-incidents").get_paginator("list_replication_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents/paginator/ListReplicationSets.html#SSMIncidents.Paginator.ListReplicationSets)

```python
# ListReplicationSetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ssm_incidents.paginator import ListReplicationSetsPaginator

session = get_session()
async with session.create_client("ssm-incidents") as client:  # (1)
    paginator: ListReplicationSetsPaginator = client.get_paginator("list_replication_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListReplicationSetsOutputTypeDef
        print(item)  # (3)
```

1. client: [SSMIncidentsClient](./client.md)
2. paginator: [ListReplicationSetsPaginator](./paginators.md#listreplicationsetspaginator)
3. item: `AioPageIterator[ListReplicationSetsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListReplicationSetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListReplicationSetsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListReplicationSetsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListReplicationSetsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListReplicationSetsInputPaginateTypeDef](./type_defs.md#listreplicationsetsinputpaginatetypedef)
## ListResponsePlansPaginator

Type annotations and code completion for `#!python session.create_client("ssm-incidents").get_paginator("list_response_plans")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents/paginator/ListResponsePlans.html#SSMIncidents.Paginator.ListResponsePlans)

```python
# ListResponsePlansPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ssm_incidents.paginator import ListResponsePlansPaginator

session = get_session()
async with session.create_client("ssm-incidents") as client:  # (1)
    paginator: ListResponsePlansPaginator = client.get_paginator("list_response_plans")  # (2)
    async for item in paginator.paginate(...):
        item: ListResponsePlansOutputTypeDef
        print(item)  # (3)
```

1. client: [SSMIncidentsClient](./client.md)
2. paginator: [ListResponsePlansPaginator](./paginators.md#listresponseplanspaginator)
3. item: `AioPageIterator[ListResponsePlansOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListResponsePlansPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListResponsePlansOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListResponsePlansOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListResponsePlansInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResponsePlansInputPaginateTypeDef](./type_defs.md#listresponseplansinputpaginatetypedef)
## ListTimelineEventsPaginator

Type annotations and code completion for `#!python session.create_client("ssm-incidents").get_paginator("list_timeline_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents/paginator/ListTimelineEvents.html#SSMIncidents.Paginator.ListTimelineEvents)

```python
# ListTimelineEventsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ssm_incidents.paginator import ListTimelineEventsPaginator

session = get_session()
async with session.create_client("ssm-incidents") as client:  # (1)
    paginator: ListTimelineEventsPaginator = client.get_paginator("list_timeline_events")  # (2)
    async for item in paginator.paginate(...):
        item: ListTimelineEventsOutputTypeDef
        print(item)  # (3)
```

1. client: [SSMIncidentsClient](./client.md)
2. paginator: [ListTimelineEventsPaginator](./paginators.md#listtimelineeventspaginator)
3. item: `AioPageIterator[ListTimelineEventsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTimelineEventsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    incidentRecordArn: str,
    filters: Sequence[FilterTypeDef] = ...,  # (1)
    sortBy: TimelineEventSortType = ...,  # (2)
    sortOrder: SortOrderType = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[ListTimelineEventsOutputTypeDef]:  # (5)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-brackets: TimelineEventSortType](./literals.md#timelineeventsorttype)
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype)
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[ListTimelineEventsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTimelineEventsInputPaginateTypeDef = {  # (1)
    "incidentRecordArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTimelineEventsInputPaginateTypeDef](./type_defs.md#listtimelineeventsinputpaginatetypedef)
