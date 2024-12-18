# UserNotificationsClient

> [Index](../README.md) > [UserNotifications](./README.md) > UserNotificationsClient

!!! note ""

    Auto-generated documentation for [UserNotifications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications.html#usernotifications)
    type annotations stubs module [types-aiobotocore-notifications](https://pypi.org/project/types-aiobotocore-notifications/).

## UserNotificationsClient

Type annotations and code completion for `#!python session.create_client("notifications")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications.html#UserNotifications.Client)

```python
# UserNotificationsClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_notifications.client import UserNotificationsClient

session = get_session()
async with session.create_client("notifications") as client:
    client: UserNotificationsClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("notifications").exceptions` structure.

```python
# UserNotificationsClient.exceptions usage example

async with session.create_client("notifications") as client:
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
# UserNotificationsClient usage type checking example

from types_aiobotocore_notifications.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("notifications").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("notifications").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/client/generate_presigned_url.html)

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



Type annotations and code completion for `#!python session.create_client("notifications").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### associate\_channel

Associates a delivery <a
href="https://docs.aws.amazon.com/notifications/latest/userguide/managing-delivery-channels.html">Channel</a>
with a particular NotificationConfiguration.

Type annotations and code completion for `#!python session.create_client("notifications").associate_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/client/associate_channel.html)

```python
# associate_channel method definition

await def associate_channel(
    self,
    *,
    arn: str,
    notificationConfigurationArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# associate_channel method usage example with argument unpacking

kwargs: AssociateChannelRequestRequestTypeDef = {  # (1)
    "arn": ...,
    "notificationConfigurationArn": ...,
}

parent.associate_channel(**kwargs)
```

1. See [:material-code-braces: AssociateChannelRequestRequestTypeDef](./type_defs.md#associatechannelrequestrequesttypedef) 

### create\_event\_rule

Creates an <a
href="https://docs.aws.amazon.com/notifications/latest/userguide/glossary.html">EventRule</a>
that is associated with a specified Notification Configuration.

Type annotations and code completion for `#!python session.create_client("notifications").create_event_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/client/create_event_rule.html)

```python
# create_event_rule method definition

await def create_event_rule(
    self,
    *,
    notificationConfigurationArn: str,
    source: str,
    eventType: str,
    regions: Sequence[str],
    eventPattern: str = ...,
) -> CreateEventRuleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateEventRuleResponseTypeDef](./type_defs.md#createeventruleresponsetypedef) 


```python
# create_event_rule method usage example with argument unpacking

kwargs: CreateEventRuleRequestRequestTypeDef = {  # (1)
    "notificationConfigurationArn": ...,
    "source": ...,
    "eventType": ...,
    "regions": ...,
}

parent.create_event_rule(**kwargs)
```

1. See [:material-code-braces: CreateEventRuleRequestRequestTypeDef](./type_defs.md#createeventrulerequestrequesttypedef) 

### create\_notification\_configuration

Creates a new NotificationConfiguration.

Type annotations and code completion for `#!python session.create_client("notifications").create_notification_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/client/create_notification_configuration.html)

```python
# create_notification_configuration method definition

await def create_notification_configuration(
    self,
    *,
    name: str,
    description: str,
    aggregationDuration: AggregationDurationType = ...,  # (1)
    tags: Mapping[str, str] = ...,
) -> CreateNotificationConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AggregationDurationType](./literals.md#aggregationdurationtype) 
2. See [:material-code-braces: CreateNotificationConfigurationResponseTypeDef](./type_defs.md#createnotificationconfigurationresponsetypedef) 


```python
# create_notification_configuration method usage example with argument unpacking

kwargs: CreateNotificationConfigurationRequestRequestTypeDef = {  # (1)
    "name": ...,
    "description": ...,
}

parent.create_notification_configuration(**kwargs)
```

1. See [:material-code-braces: CreateNotificationConfigurationRequestRequestTypeDef](./type_defs.md#createnotificationconfigurationrequestrequesttypedef) 

### delete\_event\_rule

Deletes an EventRule.

Type annotations and code completion for `#!python session.create_client("notifications").delete_event_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/client/delete_event_rule.html)

```python
# delete_event_rule method definition

await def delete_event_rule(
    self,
    *,
    arn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_event_rule method usage example with argument unpacking

kwargs: DeleteEventRuleRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.delete_event_rule(**kwargs)
```

1. See [:material-code-braces: DeleteEventRuleRequestRequestTypeDef](./type_defs.md#deleteeventrulerequestrequesttypedef) 

### delete\_notification\_configuration

Deletes a NotificationConfiguration.

Type annotations and code completion for `#!python session.create_client("notifications").delete_notification_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/client/delete_notification_configuration.html)

```python
# delete_notification_configuration method definition

await def delete_notification_configuration(
    self,
    *,
    arn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_notification_configuration method usage example with argument unpacking

kwargs: DeleteNotificationConfigurationRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.delete_notification_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteNotificationConfigurationRequestRequestTypeDef](./type_defs.md#deletenotificationconfigurationrequestrequesttypedef) 

### deregister\_notification\_hub

Deregisters a NotificationHub in the specified Region.

Type annotations and code completion for `#!python session.create_client("notifications").deregister_notification_hub` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/client/deregister_notification_hub.html)

```python
# deregister_notification_hub method definition

await def deregister_notification_hub(
    self,
    *,
    notificationHubRegion: str,
) -> DeregisterNotificationHubResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeregisterNotificationHubResponseTypeDef](./type_defs.md#deregisternotificationhubresponsetypedef) 


```python
# deregister_notification_hub method usage example with argument unpacking

kwargs: DeregisterNotificationHubRequestRequestTypeDef = {  # (1)
    "notificationHubRegion": ...,
}

parent.deregister_notification_hub(**kwargs)
```

1. See [:material-code-braces: DeregisterNotificationHubRequestRequestTypeDef](./type_defs.md#deregisternotificationhubrequestrequesttypedef) 

### disassociate\_channel

Disassociates a Channel from a specified NotificationConfiguration.

Type annotations and code completion for `#!python session.create_client("notifications").disassociate_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/client/disassociate_channel.html)

```python
# disassociate_channel method definition

await def disassociate_channel(
    self,
    *,
    arn: str,
    notificationConfigurationArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_channel method usage example with argument unpacking

kwargs: DisassociateChannelRequestRequestTypeDef = {  # (1)
    "arn": ...,
    "notificationConfigurationArn": ...,
}

parent.disassociate_channel(**kwargs)
```

1. See [:material-code-braces: DisassociateChannelRequestRequestTypeDef](./type_defs.md#disassociatechannelrequestrequesttypedef) 

### get\_event\_rule

Returns a specified EventRule.

Type annotations and code completion for `#!python session.create_client("notifications").get_event_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/client/get_event_rule.html)

```python
# get_event_rule method definition

await def get_event_rule(
    self,
    *,
    arn: str,
) -> GetEventRuleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEventRuleResponseTypeDef](./type_defs.md#geteventruleresponsetypedef) 


```python
# get_event_rule method usage example with argument unpacking

kwargs: GetEventRuleRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_event_rule(**kwargs)
```

1. See [:material-code-braces: GetEventRuleRequestRequestTypeDef](./type_defs.md#geteventrulerequestrequesttypedef) 

### get\_notification\_configuration

Returns a specified NotificationConfiguration.

Type annotations and code completion for `#!python session.create_client("notifications").get_notification_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/client/get_notification_configuration.html)

```python
# get_notification_configuration method definition

await def get_notification_configuration(
    self,
    *,
    arn: str,
) -> GetNotificationConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetNotificationConfigurationResponseTypeDef](./type_defs.md#getnotificationconfigurationresponsetypedef) 


```python
# get_notification_configuration method usage example with argument unpacking

kwargs: GetNotificationConfigurationRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_notification_configuration(**kwargs)
```

1. See [:material-code-braces: GetNotificationConfigurationRequestRequestTypeDef](./type_defs.md#getnotificationconfigurationrequestrequesttypedef) 

### get\_notification\_event

Returns a specified NotificationEvent.

Type annotations and code completion for `#!python session.create_client("notifications").get_notification_event` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/client/get_notification_event.html)

```python
# get_notification_event method definition

await def get_notification_event(
    self,
    *,
    arn: str,
    locale: LocaleCodeType = ...,  # (1)
) -> GetNotificationEventResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LocaleCodeType](./literals.md#localecodetype) 
2. See [:material-code-braces: GetNotificationEventResponseTypeDef](./type_defs.md#getnotificationeventresponsetypedef) 


```python
# get_notification_event method usage example with argument unpacking

kwargs: GetNotificationEventRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_notification_event(**kwargs)
```

1. See [:material-code-braces: GetNotificationEventRequestRequestTypeDef](./type_defs.md#getnotificationeventrequestrequesttypedef) 

### list\_channels

Returns a list of Channels for a NotificationConfiguration.

Type annotations and code completion for `#!python session.create_client("notifications").list_channels` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/client/list_channels.html)

```python
# list_channels method definition

await def list_channels(
    self,
    *,
    notificationConfigurationArn: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListChannelsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef) 


```python
# list_channels method usage example with argument unpacking

kwargs: ListChannelsRequestRequestTypeDef = {  # (1)
    "notificationConfigurationArn": ...,
}

parent.list_channels(**kwargs)
```

1. See [:material-code-braces: ListChannelsRequestRequestTypeDef](./type_defs.md#listchannelsrequestrequesttypedef) 

### list\_event\_rules

Returns a list of EventRules according to specified filters, in reverse
chronological order (newest first).

Type annotations and code completion for `#!python session.create_client("notifications").list_event_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/client/list_event_rules.html)

```python
# list_event_rules method definition

await def list_event_rules(
    self,
    *,
    notificationConfigurationArn: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListEventRulesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEventRulesResponseTypeDef](./type_defs.md#listeventrulesresponsetypedef) 


```python
# list_event_rules method usage example with argument unpacking

kwargs: ListEventRulesRequestRequestTypeDef = {  # (1)
    "notificationConfigurationArn": ...,
}

parent.list_event_rules(**kwargs)
```

1. See [:material-code-braces: ListEventRulesRequestRequestTypeDef](./type_defs.md#listeventrulesrequestrequesttypedef) 

### list\_notification\_configurations

Returns a list of abbreviated NotificationConfigurations according to specified
filters, in reverse chronological order (newest first).

Type annotations and code completion for `#!python session.create_client("notifications").list_notification_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/client/list_notification_configurations.html)

```python
# list_notification_configurations method definition

await def list_notification_configurations(
    self,
    *,
    eventRuleSource: str = ...,
    channelArn: str = ...,
    status: NotificationConfigurationStatusType = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListNotificationConfigurationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: NotificationConfigurationStatusType](./literals.md#notificationconfigurationstatustype) 
2. See [:material-code-braces: ListNotificationConfigurationsResponseTypeDef](./type_defs.md#listnotificationconfigurationsresponsetypedef) 


```python
# list_notification_configurations method usage example with argument unpacking

kwargs: ListNotificationConfigurationsRequestRequestTypeDef = {  # (1)
    "eventRuleSource": ...,
}

parent.list_notification_configurations(**kwargs)
```

1. See [:material-code-braces: ListNotificationConfigurationsRequestRequestTypeDef](./type_defs.md#listnotificationconfigurationsrequestrequesttypedef) 

### list\_notification\_events

Returns a list of NotificationEvents according to specified filters, in reverse
chronological order (newest first).

Type annotations and code completion for `#!python session.create_client("notifications").list_notification_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/client/list_notification_events.html)

```python
# list_notification_events method definition

await def list_notification_events(
    self,
    *,
    startTime: TimestampTypeDef = ...,
    endTime: TimestampTypeDef = ...,
    locale: LocaleCodeType = ...,  # (1)
    source: str = ...,
    includeChildEvents: bool = ...,
    aggregateNotificationEventArn: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListNotificationEventsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LocaleCodeType](./literals.md#localecodetype) 
2. See [:material-code-braces: ListNotificationEventsResponseTypeDef](./type_defs.md#listnotificationeventsresponsetypedef) 


```python
# list_notification_events method usage example with argument unpacking

kwargs: ListNotificationEventsRequestRequestTypeDef = {  # (1)
    "startTime": ...,
}

parent.list_notification_events(**kwargs)
```

1. See [:material-code-braces: ListNotificationEventsRequestRequestTypeDef](./type_defs.md#listnotificationeventsrequestrequesttypedef) 

### list\_notification\_hubs

Returns a list of NotificationHubs.

Type annotations and code completion for `#!python session.create_client("notifications").list_notification_hubs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/client/list_notification_hubs.html)

```python
# list_notification_hubs method definition

await def list_notification_hubs(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListNotificationHubsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListNotificationHubsResponseTypeDef](./type_defs.md#listnotificationhubsresponsetypedef) 


```python
# list_notification_hubs method usage example with argument unpacking

kwargs: ListNotificationHubsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_notification_hubs(**kwargs)
```

1. See [:material-code-braces: ListNotificationHubsRequestRequestTypeDef](./type_defs.md#listnotificationhubsrequestrequesttypedef) 

### list\_tags\_for\_resource

Returns a list of tags for a specified Amazon Resource Name (ARN).

Type annotations and code completion for `#!python session.create_client("notifications").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    arn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### register\_notification\_hub

Registers a NotificationHub in the specified Region.

Type annotations and code completion for `#!python session.create_client("notifications").register_notification_hub` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/client/register_notification_hub.html)

```python
# register_notification_hub method definition

await def register_notification_hub(
    self,
    *,
    notificationHubRegion: str,
) -> RegisterNotificationHubResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RegisterNotificationHubResponseTypeDef](./type_defs.md#registernotificationhubresponsetypedef) 


```python
# register_notification_hub method usage example with argument unpacking

kwargs: RegisterNotificationHubRequestRequestTypeDef = {  # (1)
    "notificationHubRegion": ...,
}

parent.register_notification_hub(**kwargs)
```

1. See [:material-code-braces: RegisterNotificationHubRequestRequestTypeDef](./type_defs.md#registernotificationhubrequestrequesttypedef) 

### tag\_resource

Tags the resource with a tag key and value.

Type annotations and code completion for `#!python session.create_client("notifications").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    arn: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "arn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Untags a resource with a specified Amazon Resource Name (ARN).

Type annotations and code completion for `#!python session.create_client("notifications").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    arn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "arn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_event\_rule

Updates an existing EventRule.

Type annotations and code completion for `#!python session.create_client("notifications").update_event_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/client/update_event_rule.html)

```python
# update_event_rule method definition

await def update_event_rule(
    self,
    *,
    arn: str,
    eventPattern: str = ...,
    regions: Sequence[str] = ...,
) -> UpdateEventRuleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateEventRuleResponseTypeDef](./type_defs.md#updateeventruleresponsetypedef) 


```python
# update_event_rule method usage example with argument unpacking

kwargs: UpdateEventRuleRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.update_event_rule(**kwargs)
```

1. See [:material-code-braces: UpdateEventRuleRequestRequestTypeDef](./type_defs.md#updateeventrulerequestrequesttypedef) 

### update\_notification\_configuration

Updates a NotificationConfiguration.

Type annotations and code completion for `#!python session.create_client("notifications").update_notification_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications/client/update_notification_configuration.html)

```python
# update_notification_configuration method definition

await def update_notification_configuration(
    self,
    *,
    arn: str,
    name: str = ...,
    description: str = ...,
    aggregationDuration: AggregationDurationType = ...,  # (1)
) -> UpdateNotificationConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AggregationDurationType](./literals.md#aggregationdurationtype) 
2. See [:material-code-braces: UpdateNotificationConfigurationResponseTypeDef](./type_defs.md#updatenotificationconfigurationresponsetypedef) 


```python
# update_notification_configuration method usage example with argument unpacking

kwargs: UpdateNotificationConfigurationRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.update_notification_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateNotificationConfigurationRequestRequestTypeDef](./type_defs.md#updatenotificationconfigurationrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("notifications").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications.html#UserNotifications.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "UserNotificationsClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("notifications").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications.html#UserNotifications.Client)

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

Type annotations and code completion for `#!python session.create_client("notifications").get_paginator` method with overloads.

- `client.get_paginator("list_channels")` -> [ListChannelsPaginator](./paginators.md#listchannelspaginator)
- `client.get_paginator("list_event_rules")` -> [ListEventRulesPaginator](./paginators.md#listeventrulespaginator)
- `client.get_paginator("list_notification_configurations")` -> [ListNotificationConfigurationsPaginator](./paginators.md#listnotificationconfigurationspaginator)
- `client.get_paginator("list_notification_events")` -> [ListNotificationEventsPaginator](./paginators.md#listnotificationeventspaginator)
- `client.get_paginator("list_notification_hubs")` -> [ListNotificationHubsPaginator](./paginators.md#listnotificationhubspaginator)



