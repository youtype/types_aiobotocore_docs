# CloudWatchInternetMonitorClient

> [Index](../README.md) > [CloudWatchInternetMonitor](./README.md) > CloudWatchInternetMonitorClient

!!! note ""

    Auto-generated documentation for [CloudWatchInternetMonitor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor)
    type annotations stubs module [types-aiobotocore-internetmonitor](https://pypi.org/project/types-aiobotocore-internetmonitor/).

## CloudWatchInternetMonitorClient

Type annotations and code completion for `#!python session.create_client("internetmonitor")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client)

```python
CloudWatchInternetMonitorClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_internetmonitor.client import CloudWatchInternetMonitorClient

session = get_session()
async with session.create_client("internetmonitor") as client:
    client: CloudWatchInternetMonitorClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("internetmonitor").exceptions` structure.

```python
CloudWatchInternetMonitorClient.exceptions usage example

async with session.create_client("internetmonitor") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.BadRequestException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerErrorException,
        client.InternalServerException,
        client.LimitExceededException,
        client.NotFoundException,
        client.ResourceNotFoundException,
        client.ThrottlingException,
        client.TooManyRequestsException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
CloudWatchInternetMonitorClient usage type checking example

from types_aiobotocore_internetmonitor.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("internetmonitor").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("internetmonitor").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_monitor

Creates a monitor in Amazon CloudWatch Internet Monitor.

Type annotations and code completion for `#!python session.create_client("internetmonitor").create_monitor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.create_monitor)

```python
# create_monitor method definition

await def create_monitor(
    self,
    *,
    MonitorName: str,
    Resources: Sequence[str] = ...,
    ClientToken: str = ...,
    Tags: Mapping[str, str] = ...,
    MaxCityNetworksToMonitor: int = ...,
    InternetMeasurementsLogDelivery: InternetMeasurementsLogDeliveryTypeDef = ...,  # (1)
    TrafficPercentageToMonitor: int = ...,
    HealthEventsConfig: HealthEventsConfigTypeDef = ...,  # (2)
) -> CreateMonitorOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: InternetMeasurementsLogDeliveryTypeDef](./type_defs.md#internetmeasurementslogdeliverytypedef) 
2. See [:material-code-braces: HealthEventsConfigTypeDef](./type_defs.md#healtheventsconfigtypedef) 
3. See [:material-code-braces: CreateMonitorOutputTypeDef](./type_defs.md#createmonitoroutputtypedef) 


```python
# create_monitor method usage example with argument unpacking

kwargs: CreateMonitorInputRequestTypeDef = {  # (1)
    "MonitorName": ...,
}

parent.create_monitor(**kwargs)
```

1. See [:material-code-braces: CreateMonitorInputRequestTypeDef](./type_defs.md#createmonitorinputrequesttypedef) 

### delete\_monitor

Deletes a monitor in Amazon CloudWatch Internet Monitor.

Type annotations and code completion for `#!python session.create_client("internetmonitor").delete_monitor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.delete_monitor)

```python
# delete_monitor method definition

await def delete_monitor(
    self,
    *,
    MonitorName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_monitor method usage example with argument unpacking

kwargs: DeleteMonitorInputRequestTypeDef = {  # (1)
    "MonitorName": ...,
}

parent.delete_monitor(**kwargs)
```

1. See [:material-code-braces: DeleteMonitorInputRequestTypeDef](./type_defs.md#deletemonitorinputrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("internetmonitor").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.generate_presigned_url)

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


### get\_health\_event

Gets information the Amazon CloudWatch Internet Monitor has created and stored
about a health event for a specified monitor.

Type annotations and code completion for `#!python session.create_client("internetmonitor").get_health_event` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.get_health_event)

```python
# get_health_event method definition

await def get_health_event(
    self,
    *,
    MonitorName: str,
    EventId: str,
) -> GetHealthEventOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetHealthEventOutputTypeDef](./type_defs.md#gethealtheventoutputtypedef) 


```python
# get_health_event method usage example with argument unpacking

kwargs: GetHealthEventInputRequestTypeDef = {  # (1)
    "MonitorName": ...,
    "EventId": ...,
}

parent.get_health_event(**kwargs)
```

1. See [:material-code-braces: GetHealthEventInputRequestTypeDef](./type_defs.md#gethealtheventinputrequesttypedef) 

### get\_monitor

Gets information about a monitor in Amazon CloudWatch Internet Monitor based on
a monitor name.

Type annotations and code completion for `#!python session.create_client("internetmonitor").get_monitor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.get_monitor)

```python
# get_monitor method definition

await def get_monitor(
    self,
    *,
    MonitorName: str,
) -> GetMonitorOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMonitorOutputTypeDef](./type_defs.md#getmonitoroutputtypedef) 


```python
# get_monitor method usage example with argument unpacking

kwargs: GetMonitorInputRequestTypeDef = {  # (1)
    "MonitorName": ...,
}

parent.get_monitor(**kwargs)
```

1. See [:material-code-braces: GetMonitorInputRequestTypeDef](./type_defs.md#getmonitorinputrequesttypedef) 

### list\_health\_events

Lists all health events for a monitor in Amazon CloudWatch Internet Monitor.

Type annotations and code completion for `#!python session.create_client("internetmonitor").list_health_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.list_health_events)

```python
# list_health_events method definition

await def list_health_events(
    self,
    *,
    MonitorName: str,
    StartTime: Union[datetime, str] = ...,
    EndTime: Union[datetime, str] = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
    EventStatus: HealthEventStatusType = ...,  # (1)
) -> ListHealthEventsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: HealthEventStatusType](./literals.md#healtheventstatustype) 
2. See [:material-code-braces: ListHealthEventsOutputTypeDef](./type_defs.md#listhealtheventsoutputtypedef) 


```python
# list_health_events method usage example with argument unpacking

kwargs: ListHealthEventsInputRequestTypeDef = {  # (1)
    "MonitorName": ...,
}

parent.list_health_events(**kwargs)
```

1. See [:material-code-braces: ListHealthEventsInputRequestTypeDef](./type_defs.md#listhealtheventsinputrequesttypedef) 

### list\_monitors

Lists all of your monitors for Amazon CloudWatch Internet Monitor and their
statuses, along with the Amazon Resource Name (ARN) and name of each monitor.

Type annotations and code completion for `#!python session.create_client("internetmonitor").list_monitors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.list_monitors)

```python
# list_monitors method definition

await def list_monitors(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    MonitorStatus: str = ...,
) -> ListMonitorsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMonitorsOutputTypeDef](./type_defs.md#listmonitorsoutputtypedef) 


```python
# list_monitors method usage example with argument unpacking

kwargs: ListMonitorsInputRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_monitors(**kwargs)
```

1. See [:material-code-braces: ListMonitorsInputRequestTypeDef](./type_defs.md#listmonitorsinputrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags for a resource.

Type annotations and code completion for `#!python session.create_client("internetmonitor").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceInputRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef) 

### tag\_resource

Adds a tag to a resource.

Type annotations and code completion for `#!python session.create_client("internetmonitor").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceInputRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef) 

### untag\_resource

Removes a tag from a resource.

Type annotations and code completion for `#!python session.create_client("internetmonitor").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceInputRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef) 

### update\_monitor

Updates a monitor.

Type annotations and code completion for `#!python session.create_client("internetmonitor").update_monitor` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.update_monitor)

```python
# update_monitor method definition

await def update_monitor(
    self,
    *,
    MonitorName: str,
    ResourcesToAdd: Sequence[str] = ...,
    ResourcesToRemove: Sequence[str] = ...,
    Status: MonitorConfigStateType = ...,  # (1)
    ClientToken: str = ...,
    MaxCityNetworksToMonitor: int = ...,
    InternetMeasurementsLogDelivery: InternetMeasurementsLogDeliveryTypeDef = ...,  # (2)
    TrafficPercentageToMonitor: int = ...,
    HealthEventsConfig: HealthEventsConfigTypeDef = ...,  # (3)
) -> UpdateMonitorOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: MonitorConfigStateType](./literals.md#monitorconfigstatetype) 
2. See [:material-code-braces: InternetMeasurementsLogDeliveryTypeDef](./type_defs.md#internetmeasurementslogdeliverytypedef) 
3. See [:material-code-braces: HealthEventsConfigTypeDef](./type_defs.md#healtheventsconfigtypedef) 
4. See [:material-code-braces: UpdateMonitorOutputTypeDef](./type_defs.md#updatemonitoroutputtypedef) 


```python
# update_monitor method usage example with argument unpacking

kwargs: UpdateMonitorInputRequestTypeDef = {  # (1)
    "MonitorName": ...,
}

parent.update_monitor(**kwargs)
```

1. See [:material-code-braces: UpdateMonitorInputRequestTypeDef](./type_defs.md#updatemonitorinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("internetmonitor").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> CloudWatchInternetMonitorClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("internetmonitor").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#CloudWatchInternetMonitor.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("internetmonitor").get_paginator` method with overloads.

- `client.get_paginator("list_health_events")` -> [ListHealthEventsPaginator](./paginators.md#listhealtheventspaginator)
- `client.get_paginator("list_monitors")` -> [ListMonitorsPaginator](./paginators.md#listmonitorspaginator)



