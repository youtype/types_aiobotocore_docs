# NetworkFlowMonitorClient

> [Index](../README.md) > [NetworkFlowMonitor](./README.md) > NetworkFlowMonitorClient

!!! note ""

    Auto-generated documentation for [NetworkFlowMonitor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor.html#networkflowmonitor)
    type annotations stubs module [types-aiobotocore-networkflowmonitor](https://pypi.org/project/types-aiobotocore-networkflowmonitor/).

## NetworkFlowMonitorClient

Type annotations and code completion for `#!python session.create_client("networkflowmonitor")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor.html#NetworkFlowMonitor.Client)

```python
# NetworkFlowMonitorClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_networkflowmonitor.client import NetworkFlowMonitorClient

session = get_session()
async with session.create_client("networkflowmonitor") as client:
    client: NetworkFlowMonitorClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("networkflowmonitor").exceptions` structure.

```python
# NetworkFlowMonitorClient.exceptions usage example

async with session.create_client("networkflowmonitor") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# NetworkFlowMonitorClient usage type checking example

from types_aiobotocore_networkflowmonitor.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("networkflowmonitor").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("networkflowmonitor").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### close



Type annotations and code completion for `#!python session.create_client("networkflowmonitor").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_monitor

Create a monitor for specific network flows between local and remote resources,
so that you can monitor network performance for one or several of your
workloads.

Type annotations and code completion for `#!python session.create_client("networkflowmonitor").create_monitor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor/client/create_monitor.html)

```python
# create_monitor method definition

await def create_monitor(
    self,
    *,
    monitorName: str,
    localResources: Sequence[MonitorLocalResourceTypeDef],  # (1)
    scopeArn: str,
    remoteResources: Sequence[MonitorRemoteResourceTypeDef] = ...,  # (2)
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateMonitorOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: MonitorLocalResourceTypeDef](./type_defs.md#monitorlocalresourcetypedef) 
2. See [:material-code-braces: MonitorRemoteResourceTypeDef](./type_defs.md#monitorremoteresourcetypedef) 
3. See [:material-code-braces: CreateMonitorOutputTypeDef](./type_defs.md#createmonitoroutputtypedef) 


```python
# create_monitor method usage example with argument unpacking

kwargs: CreateMonitorInputRequestTypeDef = {  # (1)
    "monitorName": ...,
    "localResources": ...,
    "scopeArn": ...,
}

parent.create_monitor(**kwargs)
```

1. See [:material-code-braces: CreateMonitorInputRequestTypeDef](./type_defs.md#createmonitorinputrequesttypedef) 

### create\_scope

Create a scope of resources that you want to be available for Network Flow
Monitor to generate metrics for, when you have active agents on those resources
sending metrics reports to the Network Flow Monitor backend.

Type annotations and code completion for `#!python session.create_client("networkflowmonitor").create_scope` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor/client/create_scope.html)

```python
# create_scope method definition

await def create_scope(
    self,
    *,
    targets: Sequence[TargetResourceTypeDef],  # (1)
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateScopeOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TargetResourceTypeDef](./type_defs.md#targetresourcetypedef) 
2. See [:material-code-braces: CreateScopeOutputTypeDef](./type_defs.md#createscopeoutputtypedef) 


```python
# create_scope method usage example with argument unpacking

kwargs: CreateScopeInputRequestTypeDef = {  # (1)
    "targets": ...,
}

parent.create_scope(**kwargs)
```

1. See [:material-code-braces: CreateScopeInputRequestTypeDef](./type_defs.md#createscopeinputrequesttypedef) 

### delete\_monitor

Deletes a monitor in Network Flow Monitor.

Type annotations and code completion for `#!python session.create_client("networkflowmonitor").delete_monitor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor/client/delete_monitor.html)

```python
# delete_monitor method definition

await def delete_monitor(
    self,
    *,
    monitorName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_monitor method usage example with argument unpacking

kwargs: DeleteMonitorInputRequestTypeDef = {  # (1)
    "monitorName": ...,
}

parent.delete_monitor(**kwargs)
```

1. See [:material-code-braces: DeleteMonitorInputRequestTypeDef](./type_defs.md#deletemonitorinputrequesttypedef) 

### delete\_scope

Deletes a scope that has been defined.

Type annotations and code completion for `#!python session.create_client("networkflowmonitor").delete_scope` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor/client/delete_scope.html)

```python
# delete_scope method definition

await def delete_scope(
    self,
    *,
    scopeId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_scope method usage example with argument unpacking

kwargs: DeleteScopeInputRequestTypeDef = {  # (1)
    "scopeId": ...,
}

parent.delete_scope(**kwargs)
```

1. See [:material-code-braces: DeleteScopeInputRequestTypeDef](./type_defs.md#deletescopeinputrequesttypedef) 

### get\_monitor

Gets information about a monitor in Network Flow Monitor based on a monitor
name.

Type annotations and code completion for `#!python session.create_client("networkflowmonitor").get_monitor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor/client/get_monitor.html)

```python
# get_monitor method definition

await def get_monitor(
    self,
    *,
    monitorName: str,
) -> GetMonitorOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMonitorOutputTypeDef](./type_defs.md#getmonitoroutputtypedef) 


```python
# get_monitor method usage example with argument unpacking

kwargs: GetMonitorInputRequestTypeDef = {  # (1)
    "monitorName": ...,
}

parent.get_monitor(**kwargs)
```

1. See [:material-code-braces: GetMonitorInputRequestTypeDef](./type_defs.md#getmonitorinputrequesttypedef) 

### get\_query\_results\_monitor\_top\_contributors

Return the data for a query with the Network Flow Monitor query interface.

Type annotations and code completion for `#!python session.create_client("networkflowmonitor").get_query_results_monitor_top_contributors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor/client/get_query_results_monitor_top_contributors.html)

```python
# get_query_results_monitor_top_contributors method definition

await def get_query_results_monitor_top_contributors(
    self,
    *,
    monitorName: str,
    queryId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> GetQueryResultsMonitorTopContributorsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetQueryResultsMonitorTopContributorsOutputTypeDef](./type_defs.md#getqueryresultsmonitortopcontributorsoutputtypedef) 


```python
# get_query_results_monitor_top_contributors method usage example with argument unpacking

kwargs: GetQueryResultsMonitorTopContributorsInputRequestTypeDef = {  # (1)
    "monitorName": ...,
    "queryId": ...,
}

parent.get_query_results_monitor_top_contributors(**kwargs)
```

1. See [:material-code-braces: GetQueryResultsMonitorTopContributorsInputRequestTypeDef](./type_defs.md#getqueryresultsmonitortopcontributorsinputrequesttypedef) 

### get\_query\_results\_workload\_insights\_top\_contributors

Return the data for a query with the Network Flow Monitor query interface.

Type annotations and code completion for `#!python session.create_client("networkflowmonitor").get_query_results_workload_insights_top_contributors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor/client/get_query_results_workload_insights_top_contributors.html)

```python
# get_query_results_workload_insights_top_contributors method definition

await def get_query_results_workload_insights_top_contributors(
    self,
    *,
    scopeId: str,
    queryId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> GetQueryResultsWorkloadInsightsTopContributorsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetQueryResultsWorkloadInsightsTopContributorsOutputTypeDef](./type_defs.md#getqueryresultsworkloadinsightstopcontributorsoutputtypedef) 


```python
# get_query_results_workload_insights_top_contributors method usage example with argument unpacking

kwargs: GetQueryResultsWorkloadInsightsTopContributorsInputRequestTypeDef = {  # (1)
    "scopeId": ...,
    "queryId": ...,
}

parent.get_query_results_workload_insights_top_contributors(**kwargs)
```

1. See [:material-code-braces: GetQueryResultsWorkloadInsightsTopContributorsInputRequestTypeDef](./type_defs.md#getqueryresultsworkloadinsightstopcontributorsinputrequesttypedef) 

### get\_query\_results\_workload\_insights\_top\_contributors\_data

Return the data for a query with the Network Flow Monitor query interface.

Type annotations and code completion for `#!python session.create_client("networkflowmonitor").get_query_results_workload_insights_top_contributors_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor/client/get_query_results_workload_insights_top_contributors_data.html)

```python
# get_query_results_workload_insights_top_contributors_data method definition

await def get_query_results_workload_insights_top_contributors_data(
    self,
    *,
    scopeId: str,
    queryId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> GetQueryResultsWorkloadInsightsTopContributorsDataOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetQueryResultsWorkloadInsightsTopContributorsDataOutputTypeDef](./type_defs.md#getqueryresultsworkloadinsightstopcontributorsdataoutputtypedef) 


```python
# get_query_results_workload_insights_top_contributors_data method usage example with argument unpacking

kwargs: GetQueryResultsWorkloadInsightsTopContributorsDataInputRequestTypeDef = {  # (1)
    "scopeId": ...,
    "queryId": ...,
}

parent.get_query_results_workload_insights_top_contributors_data(**kwargs)
```

1. See [:material-code-braces: GetQueryResultsWorkloadInsightsTopContributorsDataInputRequestTypeDef](./type_defs.md#getqueryresultsworkloadinsightstopcontributorsdatainputrequesttypedef) 

### get\_query\_status\_monitor\_top\_contributors

Returns the current status of a query for the Network Flow Monitor query
interface, for a specified query ID and monitor.

Type annotations and code completion for `#!python session.create_client("networkflowmonitor").get_query_status_monitor_top_contributors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor/client/get_query_status_monitor_top_contributors.html)

```python
# get_query_status_monitor_top_contributors method definition

await def get_query_status_monitor_top_contributors(
    self,
    *,
    monitorName: str,
    queryId: str,
) -> GetQueryStatusMonitorTopContributorsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetQueryStatusMonitorTopContributorsOutputTypeDef](./type_defs.md#getquerystatusmonitortopcontributorsoutputtypedef) 


```python
# get_query_status_monitor_top_contributors method usage example with argument unpacking

kwargs: GetQueryStatusMonitorTopContributorsInputRequestTypeDef = {  # (1)
    "monitorName": ...,
    "queryId": ...,
}

parent.get_query_status_monitor_top_contributors(**kwargs)
```

1. See [:material-code-braces: GetQueryStatusMonitorTopContributorsInputRequestTypeDef](./type_defs.md#getquerystatusmonitortopcontributorsinputrequesttypedef) 

### get\_query\_status\_workload\_insights\_top\_contributors

Return the data for a query with the Network Flow Monitor query interface.

Type annotations and code completion for `#!python session.create_client("networkflowmonitor").get_query_status_workload_insights_top_contributors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor/client/get_query_status_workload_insights_top_contributors.html)

```python
# get_query_status_workload_insights_top_contributors method definition

await def get_query_status_workload_insights_top_contributors(
    self,
    *,
    scopeId: str,
    queryId: str,
) -> GetQueryStatusWorkloadInsightsTopContributorsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetQueryStatusWorkloadInsightsTopContributorsOutputTypeDef](./type_defs.md#getquerystatusworkloadinsightstopcontributorsoutputtypedef) 


```python
# get_query_status_workload_insights_top_contributors method usage example with argument unpacking

kwargs: GetQueryStatusWorkloadInsightsTopContributorsInputRequestTypeDef = {  # (1)
    "scopeId": ...,
    "queryId": ...,
}

parent.get_query_status_workload_insights_top_contributors(**kwargs)
```

1. See [:material-code-braces: GetQueryStatusWorkloadInsightsTopContributorsInputRequestTypeDef](./type_defs.md#getquerystatusworkloadinsightstopcontributorsinputrequesttypedef) 

### get\_query\_status\_workload\_insights\_top\_contributors\_data

Returns the current status of a query for the Network Flow Monitor query
interface, for a specified query ID and monitor.

Type annotations and code completion for `#!python session.create_client("networkflowmonitor").get_query_status_workload_insights_top_contributors_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor/client/get_query_status_workload_insights_top_contributors_data.html)

```python
# get_query_status_workload_insights_top_contributors_data method definition

await def get_query_status_workload_insights_top_contributors_data(
    self,
    *,
    scopeId: str,
    queryId: str,
) -> GetQueryStatusWorkloadInsightsTopContributorsDataOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetQueryStatusWorkloadInsightsTopContributorsDataOutputTypeDef](./type_defs.md#getquerystatusworkloadinsightstopcontributorsdataoutputtypedef) 


```python
# get_query_status_workload_insights_top_contributors_data method usage example with argument unpacking

kwargs: GetQueryStatusWorkloadInsightsTopContributorsDataInputRequestTypeDef = {  # (1)
    "scopeId": ...,
    "queryId": ...,
}

parent.get_query_status_workload_insights_top_contributors_data(**kwargs)
```

1. See [:material-code-braces: GetQueryStatusWorkloadInsightsTopContributorsDataInputRequestTypeDef](./type_defs.md#getquerystatusworkloadinsightstopcontributorsdatainputrequesttypedef) 

### get\_scope

Gets information about a scope, including the name, status, tags, and target
details.

Type annotations and code completion for `#!python session.create_client("networkflowmonitor").get_scope` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor/client/get_scope.html)

```python
# get_scope method definition

await def get_scope(
    self,
    *,
    scopeId: str,
) -> GetScopeOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetScopeOutputTypeDef](./type_defs.md#getscopeoutputtypedef) 


```python
# get_scope method usage example with argument unpacking

kwargs: GetScopeInputRequestTypeDef = {  # (1)
    "scopeId": ...,
}

parent.get_scope(**kwargs)
```

1. See [:material-code-braces: GetScopeInputRequestTypeDef](./type_defs.md#getscopeinputrequesttypedef) 

### list\_monitors

List all monitors in an account.

Type annotations and code completion for `#!python session.create_client("networkflowmonitor").list_monitors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor/client/list_monitors.html)

```python
# list_monitors method definition

await def list_monitors(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
    monitorStatus: MonitorStatusType = ...,  # (1)
) -> ListMonitorsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: MonitorStatusType](./literals.md#monitorstatustype) 
2. See [:material-code-braces: ListMonitorsOutputTypeDef](./type_defs.md#listmonitorsoutputtypedef) 


```python
# list_monitors method usage example with argument unpacking

kwargs: ListMonitorsInputRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_monitors(**kwargs)
```

1. See [:material-code-braces: ListMonitorsInputRequestTypeDef](./type_defs.md#listmonitorsinputrequesttypedef) 

### list\_scopes

List all the scopes for an account.

Type annotations and code completion for `#!python session.create_client("networkflowmonitor").list_scopes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor/client/list_scopes.html)

```python
# list_scopes method definition

await def list_scopes(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListScopesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListScopesOutputTypeDef](./type_defs.md#listscopesoutputtypedef) 


```python
# list_scopes method usage example with argument unpacking

kwargs: ListScopesInputRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_scopes(**kwargs)
```

1. See [:material-code-braces: ListScopesInputRequestTypeDef](./type_defs.md#listscopesinputrequesttypedef) 

### list\_tags\_for\_resource

Returns all the tags for a resource.

Type annotations and code completion for `#!python session.create_client("networkflowmonitor").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef) 

### start\_query\_monitor\_top\_contributors

Start a query to return the data with the Network Flow Monitor query interface.

Type annotations and code completion for `#!python session.create_client("networkflowmonitor").start_query_monitor_top_contributors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor/client/start_query_monitor_top_contributors.html)

```python
# start_query_monitor_top_contributors method definition

await def start_query_monitor_top_contributors(
    self,
    *,
    monitorName: str,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    metricName: MonitorMetricType,  # (1)
    destinationCategory: DestinationCategoryType,  # (2)
    limit: int = ...,
) -> StartQueryMonitorTopContributorsOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: MonitorMetricType](./literals.md#monitormetrictype) 
2. See [:material-code-brackets: DestinationCategoryType](./literals.md#destinationcategorytype) 
3. See [:material-code-braces: StartQueryMonitorTopContributorsOutputTypeDef](./type_defs.md#startquerymonitortopcontributorsoutputtypedef) 


```python
# start_query_monitor_top_contributors method usage example with argument unpacking

kwargs: StartQueryMonitorTopContributorsInputRequestTypeDef = {  # (1)
    "monitorName": ...,
    "startTime": ...,
    "endTime": ...,
    "metricName": ...,
    "destinationCategory": ...,
}

parent.start_query_monitor_top_contributors(**kwargs)
```

1. See [:material-code-braces: StartQueryMonitorTopContributorsInputRequestTypeDef](./type_defs.md#startquerymonitortopcontributorsinputrequesttypedef) 

### start\_query\_workload\_insights\_top\_contributors

Start a query to return the data with the Network Flow Monitor query interface.

Type annotations and code completion for `#!python session.create_client("networkflowmonitor").start_query_workload_insights_top_contributors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor/client/start_query_workload_insights_top_contributors.html)

```python
# start_query_workload_insights_top_contributors method definition

await def start_query_workload_insights_top_contributors(
    self,
    *,
    scopeId: str,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    metricName: WorkloadInsightsMetricType,  # (1)
    destinationCategory: DestinationCategoryType,  # (2)
    limit: int = ...,
) -> StartQueryWorkloadInsightsTopContributorsOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: WorkloadInsightsMetricType](./literals.md#workloadinsightsmetrictype) 
2. See [:material-code-brackets: DestinationCategoryType](./literals.md#destinationcategorytype) 
3. See [:material-code-braces: StartQueryWorkloadInsightsTopContributorsOutputTypeDef](./type_defs.md#startqueryworkloadinsightstopcontributorsoutputtypedef) 


```python
# start_query_workload_insights_top_contributors method usage example with argument unpacking

kwargs: StartQueryWorkloadInsightsTopContributorsInputRequestTypeDef = {  # (1)
    "scopeId": ...,
    "startTime": ...,
    "endTime": ...,
    "metricName": ...,
    "destinationCategory": ...,
}

parent.start_query_workload_insights_top_contributors(**kwargs)
```

1. See [:material-code-braces: StartQueryWorkloadInsightsTopContributorsInputRequestTypeDef](./type_defs.md#startqueryworkloadinsightstopcontributorsinputrequesttypedef) 

### start\_query\_workload\_insights\_top\_contributors\_data

Return the data for a query with the Network Flow Monitor query interface.

Type annotations and code completion for `#!python session.create_client("networkflowmonitor").start_query_workload_insights_top_contributors_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor/client/start_query_workload_insights_top_contributors_data.html)

```python
# start_query_workload_insights_top_contributors_data method definition

await def start_query_workload_insights_top_contributors_data(
    self,
    *,
    scopeId: str,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    metricName: WorkloadInsightsMetricType,  # (1)
    destinationCategory: DestinationCategoryType,  # (2)
) -> StartQueryWorkloadInsightsTopContributorsDataOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: WorkloadInsightsMetricType](./literals.md#workloadinsightsmetrictype) 
2. See [:material-code-brackets: DestinationCategoryType](./literals.md#destinationcategorytype) 
3. See [:material-code-braces: StartQueryWorkloadInsightsTopContributorsDataOutputTypeDef](./type_defs.md#startqueryworkloadinsightstopcontributorsdataoutputtypedef) 


```python
# start_query_workload_insights_top_contributors_data method usage example with argument unpacking

kwargs: StartQueryWorkloadInsightsTopContributorsDataInputRequestTypeDef = {  # (1)
    "scopeId": ...,
    "startTime": ...,
    "endTime": ...,
    "metricName": ...,
    "destinationCategory": ...,
}

parent.start_query_workload_insights_top_contributors_data(**kwargs)
```

1. See [:material-code-braces: StartQueryWorkloadInsightsTopContributorsDataInputRequestTypeDef](./type_defs.md#startqueryworkloadinsightstopcontributorsdatainputrequesttypedef) 

### stop\_query\_monitor\_top\_contributors

Stop a query with the Network Flow Monitor query interface.

Type annotations and code completion for `#!python session.create_client("networkflowmonitor").stop_query_monitor_top_contributors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor/client/stop_query_monitor_top_contributors.html)

```python
# stop_query_monitor_top_contributors method definition

await def stop_query_monitor_top_contributors(
    self,
    *,
    monitorName: str,
    queryId: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_query_monitor_top_contributors method usage example with argument unpacking

kwargs: StopQueryMonitorTopContributorsInputRequestTypeDef = {  # (1)
    "monitorName": ...,
    "queryId": ...,
}

parent.stop_query_monitor_top_contributors(**kwargs)
```

1. See [:material-code-braces: StopQueryMonitorTopContributorsInputRequestTypeDef](./type_defs.md#stopquerymonitortopcontributorsinputrequesttypedef) 

### stop\_query\_workload\_insights\_top\_contributors

Stop a query with the Network Flow Monitor query interface.

Type annotations and code completion for `#!python session.create_client("networkflowmonitor").stop_query_workload_insights_top_contributors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor/client/stop_query_workload_insights_top_contributors.html)

```python
# stop_query_workload_insights_top_contributors method definition

await def stop_query_workload_insights_top_contributors(
    self,
    *,
    scopeId: str,
    queryId: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_query_workload_insights_top_contributors method usage example with argument unpacking

kwargs: StopQueryWorkloadInsightsTopContributorsInputRequestTypeDef = {  # (1)
    "scopeId": ...,
    "queryId": ...,
}

parent.stop_query_workload_insights_top_contributors(**kwargs)
```

1. See [:material-code-braces: StopQueryWorkloadInsightsTopContributorsInputRequestTypeDef](./type_defs.md#stopqueryworkloadinsightstopcontributorsinputrequesttypedef) 

### stop\_query\_workload\_insights\_top\_contributors\_data

Return the data for a query with the Network Flow Monitor query interface.

Type annotations and code completion for `#!python session.create_client("networkflowmonitor").stop_query_workload_insights_top_contributors_data` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor/client/stop_query_workload_insights_top_contributors_data.html)

```python
# stop_query_workload_insights_top_contributors_data method definition

await def stop_query_workload_insights_top_contributors_data(
    self,
    *,
    scopeId: str,
    queryId: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_query_workload_insights_top_contributors_data method usage example with argument unpacking

kwargs: StopQueryWorkloadInsightsTopContributorsDataInputRequestTypeDef = {  # (1)
    "scopeId": ...,
    "queryId": ...,
}

parent.stop_query_workload_insights_top_contributors_data(**kwargs)
```

1. See [:material-code-braces: StopQueryWorkloadInsightsTopContributorsDataInputRequestTypeDef](./type_defs.md#stopqueryworkloadinsightstopcontributorsdatainputrequesttypedef) 

### tag\_resource

Adds a tag to a resource.

Type annotations and code completion for `#!python session.create_client("networkflowmonitor").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef) 

### untag\_resource

Removes a tag from a resource.

Type annotations and code completion for `#!python session.create_client("networkflowmonitor").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceInputRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef) 

### update\_monitor

Update a monitor to add or remove local or remote resources.

Type annotations and code completion for `#!python session.create_client("networkflowmonitor").update_monitor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor/client/update_monitor.html)

```python
# update_monitor method definition

await def update_monitor(
    self,
    *,
    monitorName: str,
    localResourcesToAdd: Sequence[MonitorLocalResourceTypeDef] = ...,  # (1)
    localResourcesToRemove: Sequence[MonitorLocalResourceTypeDef] = ...,  # (1)
    remoteResourcesToAdd: Sequence[MonitorRemoteResourceTypeDef] = ...,  # (3)
    remoteResourcesToRemove: Sequence[MonitorRemoteResourceTypeDef] = ...,  # (3)
    clientToken: str = ...,
) -> UpdateMonitorOutputTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: MonitorLocalResourceTypeDef](./type_defs.md#monitorlocalresourcetypedef) 
2. See [:material-code-braces: MonitorLocalResourceTypeDef](./type_defs.md#monitorlocalresourcetypedef) 
3. See [:material-code-braces: MonitorRemoteResourceTypeDef](./type_defs.md#monitorremoteresourcetypedef) 
4. See [:material-code-braces: MonitorRemoteResourceTypeDef](./type_defs.md#monitorremoteresourcetypedef) 
5. See [:material-code-braces: UpdateMonitorOutputTypeDef](./type_defs.md#updatemonitoroutputtypedef) 


```python
# update_monitor method usage example with argument unpacking

kwargs: UpdateMonitorInputRequestTypeDef = {  # (1)
    "monitorName": ...,
}

parent.update_monitor(**kwargs)
```

1. See [:material-code-braces: UpdateMonitorInputRequestTypeDef](./type_defs.md#updatemonitorinputrequesttypedef) 

### update\_scope

Update a scope to add or remove resources that you want to be available for
Network Flow Monitor to generate metrics for, when you have active agents on
those resources sending metrics reports to the Network Flow Monitor backend.

Type annotations and code completion for `#!python session.create_client("networkflowmonitor").update_scope` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor/client/update_scope.html)

```python
# update_scope method definition

await def update_scope(
    self,
    *,
    scopeId: str,
    resourcesToAdd: Sequence[TargetResourceTypeDef] = ...,  # (1)
    resourcesToDelete: Sequence[TargetResourceTypeDef] = ...,  # (1)
) -> UpdateScopeOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TargetResourceTypeDef](./type_defs.md#targetresourcetypedef) 
2. See [:material-code-braces: TargetResourceTypeDef](./type_defs.md#targetresourcetypedef) 
3. See [:material-code-braces: UpdateScopeOutputTypeDef](./type_defs.md#updatescopeoutputtypedef) 


```python
# update_scope method usage example with argument unpacking

kwargs: UpdateScopeInputRequestTypeDef = {  # (1)
    "scopeId": ...,
}

parent.update_scope(**kwargs)
```

1. See [:material-code-braces: UpdateScopeInputRequestTypeDef](./type_defs.md#updatescopeinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("networkflowmonitor").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor.html#NetworkFlowMonitor.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "NetworkFlowMonitorClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("networkflowmonitor").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor.html#NetworkFlowMonitor.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("networkflowmonitor").get_paginator` method with overloads.

- `client.get_paginator("get_query_results_monitor_top_contributors")` -> [GetQueryResultsMonitorTopContributorsPaginator](./paginators.md#getqueryresultsmonitortopcontributorspaginator)
- `client.get_paginator("get_query_results_workload_insights_top_contributors_data")` -> [GetQueryResultsWorkloadInsightsTopContributorsDataPaginator](./paginators.md#getqueryresultsworkloadinsightstopcontributorsdatapaginator)
- `client.get_paginator("get_query_results_workload_insights_top_contributors")` -> [GetQueryResultsWorkloadInsightsTopContributorsPaginator](./paginators.md#getqueryresultsworkloadinsightstopcontributorspaginator)
- `client.get_paginator("list_monitors")` -> [ListMonitorsPaginator](./paginators.md#listmonitorspaginator)
- `client.get_paginator("list_scopes")` -> [ListScopesPaginator](./paginators.md#listscopespaginator)



