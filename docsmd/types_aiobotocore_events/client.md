# EventBridgeClient

> [Index](../README.md) > [EventBridge](./README.md) > EventBridgeClient

!!! note ""

    Auto-generated documentation for [EventBridge](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
    type annotations stubs module [types-aiobotocore-events](https://pypi.org/project/types-aiobotocore-events/).

## EventBridgeClient

Type annotations and code completion for `#!python session.create_client("events")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client)

```python
EventBridgeClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_events.client import EventBridgeClient

session = get_session()
async with session.create_client("events") as client:
    client: EventBridgeClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("events").exceptions` structure.

```python
EventBridgeClient.exceptions usage example

async with session.create_client("events") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.ConcurrentModificationException,
        client.IllegalStatusException,
        client.InternalException,
        client.InvalidEventPatternException,
        client.InvalidStateException,
        client.LimitExceededException,
        client.ManagedRuleException,
        client.OperationDisabledException,
        client.PolicyLengthExceededException,
        client.ResourceAlreadyExistsException,
        client.ResourceNotFoundException,
    ) as e:
        print(e)
```

```python
EventBridgeClient usage type checking example

from types_aiobotocore_events.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### activate\_event\_source

Activates a partner event source that has been deactivated.

Type annotations and code completion for `#!python session.create_client("events").activate_event_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.activate_event_source)

```python
# activate_event_source method definition

await def activate_event_source(
    self,
    *,
    Name: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# activate_event_source method usage example with argument unpacking

kwargs: ActivateEventSourceRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.activate_event_source(**kwargs)
```

1. See [:material-code-braces: ActivateEventSourceRequestRequestTypeDef](./type_defs.md#activateeventsourcerequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("events").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### cancel\_replay

Cancels the specified replay.

Type annotations and code completion for `#!python session.create_client("events").cancel_replay` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.cancel_replay)

```python
# cancel_replay method definition

await def cancel_replay(
    self,
    *,
    ReplayName: str,
) -> CancelReplayResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelReplayResponseTypeDef](./type_defs.md#cancelreplayresponsetypedef) 


```python
# cancel_replay method usage example with argument unpacking

kwargs: CancelReplayRequestRequestTypeDef = {  # (1)
    "ReplayName": ...,
}

parent.cancel_replay(**kwargs)
```

1. See [:material-code-braces: CancelReplayRequestRequestTypeDef](./type_defs.md#cancelreplayrequestrequesttypedef) 

### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("events").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_api\_destination

Creates an API destination, which is an HTTP invocation endpoint configured as a
target for events.

Type annotations and code completion for `#!python session.create_client("events").create_api_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.create_api_destination)

```python
# create_api_destination method definition

await def create_api_destination(
    self,
    *,
    Name: str,
    ConnectionArn: str,
    InvocationEndpoint: str,
    HttpMethod: ApiDestinationHttpMethodType,  # (1)
    Description: str = ...,
    InvocationRateLimitPerSecond: int = ...,
) -> CreateApiDestinationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ApiDestinationHttpMethodType](./literals.md#apidestinationhttpmethodtype) 
2. See [:material-code-braces: CreateApiDestinationResponseTypeDef](./type_defs.md#createapidestinationresponsetypedef) 


```python
# create_api_destination method usage example with argument unpacking

kwargs: CreateApiDestinationRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "ConnectionArn": ...,
    "InvocationEndpoint": ...,
    "HttpMethod": ...,
}

parent.create_api_destination(**kwargs)
```

1. See [:material-code-braces: CreateApiDestinationRequestRequestTypeDef](./type_defs.md#createapidestinationrequestrequesttypedef) 

### create\_archive

Creates an archive of events with the specified settings.

Type annotations and code completion for `#!python session.create_client("events").create_archive` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.create_archive)

```python
# create_archive method definition

await def create_archive(
    self,
    *,
    ArchiveName: str,
    EventSourceArn: str,
    Description: str = ...,
    EventPattern: str = ...,
    RetentionDays: int = ...,
) -> CreateArchiveResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateArchiveResponseTypeDef](./type_defs.md#createarchiveresponsetypedef) 


```python
# create_archive method usage example with argument unpacking

kwargs: CreateArchiveRequestRequestTypeDef = {  # (1)
    "ArchiveName": ...,
    "EventSourceArn": ...,
}

parent.create_archive(**kwargs)
```

1. See [:material-code-braces: CreateArchiveRequestRequestTypeDef](./type_defs.md#createarchiverequestrequesttypedef) 

### create\_connection

Creates a connection.

Type annotations and code completion for `#!python session.create_client("events").create_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.create_connection)

```python
# create_connection method definition

await def create_connection(
    self,
    *,
    Name: str,
    AuthorizationType: ConnectionAuthorizationTypeType,  # (1)
    AuthParameters: CreateConnectionAuthRequestParametersTypeDef,  # (2)
    Description: str = ...,
) -> CreateConnectionResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ConnectionAuthorizationTypeType](./literals.md#connectionauthorizationtypetype) 
2. See [:material-code-braces: CreateConnectionAuthRequestParametersTypeDef](./type_defs.md#createconnectionauthrequestparameterstypedef) 
3. See [:material-code-braces: CreateConnectionResponseTypeDef](./type_defs.md#createconnectionresponsetypedef) 


```python
# create_connection method usage example with argument unpacking

kwargs: CreateConnectionRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "AuthorizationType": ...,
    "AuthParameters": ...,
}

parent.create_connection(**kwargs)
```

1. See [:material-code-braces: CreateConnectionRequestRequestTypeDef](./type_defs.md#createconnectionrequestrequesttypedef) 

### create\_endpoint

Creates a global endpoint.

Type annotations and code completion for `#!python session.create_client("events").create_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.create_endpoint)

```python
# create_endpoint method definition

await def create_endpoint(
    self,
    *,
    Name: str,
    RoutingConfig: RoutingConfigTypeDef,  # (1)
    EventBuses: Sequence[EndpointEventBusTypeDef],  # (2)
    Description: str = ...,
    ReplicationConfig: ReplicationConfigTypeDef = ...,  # (3)
    RoleArn: str = ...,
) -> CreateEndpointResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: RoutingConfigTypeDef](./type_defs.md#routingconfigtypedef) 
2. See [:material-code-braces: EndpointEventBusTypeDef](./type_defs.md#endpointeventbustypedef) 
3. See [:material-code-braces: ReplicationConfigTypeDef](./type_defs.md#replicationconfigtypedef) 
4. See [:material-code-braces: CreateEndpointResponseTypeDef](./type_defs.md#createendpointresponsetypedef) 


```python
# create_endpoint method usage example with argument unpacking

kwargs: CreateEndpointRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "RoutingConfig": ...,
    "EventBuses": ...,
}

parent.create_endpoint(**kwargs)
```

1. See [:material-code-braces: CreateEndpointRequestRequestTypeDef](./type_defs.md#createendpointrequestrequesttypedef) 

### create\_event\_bus

Creates a new event bus within your account.

Type annotations and code completion for `#!python session.create_client("events").create_event_bus` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.create_event_bus)

```python
# create_event_bus method definition

await def create_event_bus(
    self,
    *,
    Name: str,
    EventSourceName: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateEventBusResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateEventBusResponseTypeDef](./type_defs.md#createeventbusresponsetypedef) 


```python
# create_event_bus method usage example with argument unpacking

kwargs: CreateEventBusRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.create_event_bus(**kwargs)
```

1. See [:material-code-braces: CreateEventBusRequestRequestTypeDef](./type_defs.md#createeventbusrequestrequesttypedef) 

### create\_partner\_event\_source

Called by an SaaS partner to create a partner event source.

Type annotations and code completion for `#!python session.create_client("events").create_partner_event_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.create_partner_event_source)

```python
# create_partner_event_source method definition

await def create_partner_event_source(
    self,
    *,
    Name: str,
    Account: str,
) -> CreatePartnerEventSourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreatePartnerEventSourceResponseTypeDef](./type_defs.md#createpartnereventsourceresponsetypedef) 


```python
# create_partner_event_source method usage example with argument unpacking

kwargs: CreatePartnerEventSourceRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Account": ...,
}

parent.create_partner_event_source(**kwargs)
```

1. See [:material-code-braces: CreatePartnerEventSourceRequestRequestTypeDef](./type_defs.md#createpartnereventsourcerequestrequesttypedef) 

### deactivate\_event\_source

You can use this operation to temporarily stop receiving events from the
specified partner event source.

Type annotations and code completion for `#!python session.create_client("events").deactivate_event_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.deactivate_event_source)

```python
# deactivate_event_source method definition

await def deactivate_event_source(
    self,
    *,
    Name: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# deactivate_event_source method usage example with argument unpacking

kwargs: DeactivateEventSourceRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.deactivate_event_source(**kwargs)
```

1. See [:material-code-braces: DeactivateEventSourceRequestRequestTypeDef](./type_defs.md#deactivateeventsourcerequestrequesttypedef) 

### deauthorize\_connection

Removes all authorization parameters from the connection.

Type annotations and code completion for `#!python session.create_client("events").deauthorize_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.deauthorize_connection)

```python
# deauthorize_connection method definition

await def deauthorize_connection(
    self,
    *,
    Name: str,
) -> DeauthorizeConnectionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeauthorizeConnectionResponseTypeDef](./type_defs.md#deauthorizeconnectionresponsetypedef) 


```python
# deauthorize_connection method usage example with argument unpacking

kwargs: DeauthorizeConnectionRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.deauthorize_connection(**kwargs)
```

1. See [:material-code-braces: DeauthorizeConnectionRequestRequestTypeDef](./type_defs.md#deauthorizeconnectionrequestrequesttypedef) 

### delete\_api\_destination

Deletes the specified API destination.

Type annotations and code completion for `#!python session.create_client("events").delete_api_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.delete_api_destination)

```python
# delete_api_destination method definition

await def delete_api_destination(
    self,
    *,
    Name: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_api_destination method usage example with argument unpacking

kwargs: DeleteApiDestinationRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_api_destination(**kwargs)
```

1. See [:material-code-braces: DeleteApiDestinationRequestRequestTypeDef](./type_defs.md#deleteapidestinationrequestrequesttypedef) 

### delete\_archive

Deletes the specified archive.

Type annotations and code completion for `#!python session.create_client("events").delete_archive` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.delete_archive)

```python
# delete_archive method definition

await def delete_archive(
    self,
    *,
    ArchiveName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_archive method usage example with argument unpacking

kwargs: DeleteArchiveRequestRequestTypeDef = {  # (1)
    "ArchiveName": ...,
}

parent.delete_archive(**kwargs)
```

1. See [:material-code-braces: DeleteArchiveRequestRequestTypeDef](./type_defs.md#deletearchiverequestrequesttypedef) 

### delete\_connection

Deletes a connection.

Type annotations and code completion for `#!python session.create_client("events").delete_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.delete_connection)

```python
# delete_connection method definition

await def delete_connection(
    self,
    *,
    Name: str,
) -> DeleteConnectionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteConnectionResponseTypeDef](./type_defs.md#deleteconnectionresponsetypedef) 


```python
# delete_connection method usage example with argument unpacking

kwargs: DeleteConnectionRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_connection(**kwargs)
```

1. See [:material-code-braces: DeleteConnectionRequestRequestTypeDef](./type_defs.md#deleteconnectionrequestrequesttypedef) 

### delete\_endpoint

Delete an existing global endpoint.

Type annotations and code completion for `#!python session.create_client("events").delete_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.delete_endpoint)

```python
# delete_endpoint method definition

await def delete_endpoint(
    self,
    *,
    Name: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_endpoint method usage example with argument unpacking

kwargs: DeleteEndpointRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_endpoint(**kwargs)
```

1. See [:material-code-braces: DeleteEndpointRequestRequestTypeDef](./type_defs.md#deleteendpointrequestrequesttypedef) 

### delete\_event\_bus

Deletes the specified custom event bus or partner event bus.

Type annotations and code completion for `#!python session.create_client("events").delete_event_bus` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.delete_event_bus)

```python
# delete_event_bus method definition

await def delete_event_bus(
    self,
    *,
    Name: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_event_bus method usage example with argument unpacking

kwargs: DeleteEventBusRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_event_bus(**kwargs)
```

1. See [:material-code-braces: DeleteEventBusRequestRequestTypeDef](./type_defs.md#deleteeventbusrequestrequesttypedef) 

### delete\_partner\_event\_source

This operation is used by SaaS partners to delete a partner event source.

Type annotations and code completion for `#!python session.create_client("events").delete_partner_event_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.delete_partner_event_source)

```python
# delete_partner_event_source method definition

await def delete_partner_event_source(
    self,
    *,
    Name: str,
    Account: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_partner_event_source method usage example with argument unpacking

kwargs: DeletePartnerEventSourceRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "Account": ...,
}

parent.delete_partner_event_source(**kwargs)
```

1. See [:material-code-braces: DeletePartnerEventSourceRequestRequestTypeDef](./type_defs.md#deletepartnereventsourcerequestrequesttypedef) 

### delete\_rule

Deletes the specified rule.

Type annotations and code completion for `#!python session.create_client("events").delete_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.delete_rule)

```python
# delete_rule method definition

await def delete_rule(
    self,
    *,
    Name: str,
    EventBusName: str = ...,
    Force: bool = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_rule method usage example with argument unpacking

kwargs: DeleteRuleRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_rule(**kwargs)
```

1. See [:material-code-braces: DeleteRuleRequestRequestTypeDef](./type_defs.md#deleterulerequestrequesttypedef) 

### describe\_api\_destination

Retrieves details about an API destination.

Type annotations and code completion for `#!python session.create_client("events").describe_api_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.describe_api_destination)

```python
# describe_api_destination method definition

await def describe_api_destination(
    self,
    *,
    Name: str,
) -> DescribeApiDestinationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeApiDestinationResponseTypeDef](./type_defs.md#describeapidestinationresponsetypedef) 


```python
# describe_api_destination method usage example with argument unpacking

kwargs: DescribeApiDestinationRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.describe_api_destination(**kwargs)
```

1. See [:material-code-braces: DescribeApiDestinationRequestRequestTypeDef](./type_defs.md#describeapidestinationrequestrequesttypedef) 

### describe\_archive

Retrieves details about an archive.

Type annotations and code completion for `#!python session.create_client("events").describe_archive` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.describe_archive)

```python
# describe_archive method definition

await def describe_archive(
    self,
    *,
    ArchiveName: str,
) -> DescribeArchiveResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeArchiveResponseTypeDef](./type_defs.md#describearchiveresponsetypedef) 


```python
# describe_archive method usage example with argument unpacking

kwargs: DescribeArchiveRequestRequestTypeDef = {  # (1)
    "ArchiveName": ...,
}

parent.describe_archive(**kwargs)
```

1. See [:material-code-braces: DescribeArchiveRequestRequestTypeDef](./type_defs.md#describearchiverequestrequesttypedef) 

### describe\_connection

Retrieves details about a connection.

Type annotations and code completion for `#!python session.create_client("events").describe_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.describe_connection)

```python
# describe_connection method definition

await def describe_connection(
    self,
    *,
    Name: str,
) -> DescribeConnectionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeConnectionResponseTypeDef](./type_defs.md#describeconnectionresponsetypedef) 


```python
# describe_connection method usage example with argument unpacking

kwargs: DescribeConnectionRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.describe_connection(**kwargs)
```

1. See [:material-code-braces: DescribeConnectionRequestRequestTypeDef](./type_defs.md#describeconnectionrequestrequesttypedef) 

### describe\_endpoint

Get the information about an existing global endpoint.

Type annotations and code completion for `#!python session.create_client("events").describe_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.describe_endpoint)

```python
# describe_endpoint method definition

await def describe_endpoint(
    self,
    *,
    Name: str,
    HomeRegion: str = ...,
) -> DescribeEndpointResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEndpointResponseTypeDef](./type_defs.md#describeendpointresponsetypedef) 


```python
# describe_endpoint method usage example with argument unpacking

kwargs: DescribeEndpointRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.describe_endpoint(**kwargs)
```

1. See [:material-code-braces: DescribeEndpointRequestRequestTypeDef](./type_defs.md#describeendpointrequestrequesttypedef) 

### describe\_event\_bus

Displays details about an event bus in your account.

Type annotations and code completion for `#!python session.create_client("events").describe_event_bus` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.describe_event_bus)

```python
# describe_event_bus method definition

await def describe_event_bus(
    self,
    *,
    Name: str = ...,
) -> DescribeEventBusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEventBusResponseTypeDef](./type_defs.md#describeeventbusresponsetypedef) 


```python
# describe_event_bus method usage example with argument unpacking

kwargs: DescribeEventBusRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.describe_event_bus(**kwargs)
```

1. See [:material-code-braces: DescribeEventBusRequestRequestTypeDef](./type_defs.md#describeeventbusrequestrequesttypedef) 

### describe\_event\_source

This operation lists details about a partner event source that is shared with
your account.

Type annotations and code completion for `#!python session.create_client("events").describe_event_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.describe_event_source)

```python
# describe_event_source method definition

await def describe_event_source(
    self,
    *,
    Name: str,
) -> DescribeEventSourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEventSourceResponseTypeDef](./type_defs.md#describeeventsourceresponsetypedef) 


```python
# describe_event_source method usage example with argument unpacking

kwargs: DescribeEventSourceRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.describe_event_source(**kwargs)
```

1. See [:material-code-braces: DescribeEventSourceRequestRequestTypeDef](./type_defs.md#describeeventsourcerequestrequesttypedef) 

### describe\_partner\_event\_source

An SaaS partner can use this operation to list details about a partner event
source that they have created.

Type annotations and code completion for `#!python session.create_client("events").describe_partner_event_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.describe_partner_event_source)

```python
# describe_partner_event_source method definition

await def describe_partner_event_source(
    self,
    *,
    Name: str,
) -> DescribePartnerEventSourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribePartnerEventSourceResponseTypeDef](./type_defs.md#describepartnereventsourceresponsetypedef) 


```python
# describe_partner_event_source method usage example with argument unpacking

kwargs: DescribePartnerEventSourceRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.describe_partner_event_source(**kwargs)
```

1. See [:material-code-braces: DescribePartnerEventSourceRequestRequestTypeDef](./type_defs.md#describepartnereventsourcerequestrequesttypedef) 

### describe\_replay

Retrieves details about a replay.

Type annotations and code completion for `#!python session.create_client("events").describe_replay` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.describe_replay)

```python
# describe_replay method definition

await def describe_replay(
    self,
    *,
    ReplayName: str,
) -> DescribeReplayResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeReplayResponseTypeDef](./type_defs.md#describereplayresponsetypedef) 


```python
# describe_replay method usage example with argument unpacking

kwargs: DescribeReplayRequestRequestTypeDef = {  # (1)
    "ReplayName": ...,
}

parent.describe_replay(**kwargs)
```

1. See [:material-code-braces: DescribeReplayRequestRequestTypeDef](./type_defs.md#describereplayrequestrequesttypedef) 

### describe\_rule

Describes the specified rule.

Type annotations and code completion for `#!python session.create_client("events").describe_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.describe_rule)

```python
# describe_rule method definition

await def describe_rule(
    self,
    *,
    Name: str,
    EventBusName: str = ...,
) -> DescribeRuleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeRuleResponseTypeDef](./type_defs.md#describeruleresponsetypedef) 


```python
# describe_rule method usage example with argument unpacking

kwargs: DescribeRuleRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.describe_rule(**kwargs)
```

1. See [:material-code-braces: DescribeRuleRequestRequestTypeDef](./type_defs.md#describerulerequestrequesttypedef) 

### disable\_rule

Disables the specified rule.

Type annotations and code completion for `#!python session.create_client("events").disable_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.disable_rule)

```python
# disable_rule method definition

await def disable_rule(
    self,
    *,
    Name: str,
    EventBusName: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# disable_rule method usage example with argument unpacking

kwargs: DisableRuleRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.disable_rule(**kwargs)
```

1. See [:material-code-braces: DisableRuleRequestRequestTypeDef](./type_defs.md#disablerulerequestrequesttypedef) 

### enable\_rule

Enables the specified rule.

Type annotations and code completion for `#!python session.create_client("events").enable_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.enable_rule)

```python
# enable_rule method definition

await def enable_rule(
    self,
    *,
    Name: str,
    EventBusName: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# enable_rule method usage example with argument unpacking

kwargs: EnableRuleRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.enable_rule(**kwargs)
```

1. See [:material-code-braces: EnableRuleRequestRequestTypeDef](./type_defs.md#enablerulerequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("events").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.generate_presigned_url)

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


### list\_api\_destinations

Retrieves a list of API destination in the account in the current Region.

Type annotations and code completion for `#!python session.create_client("events").list_api_destinations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_api_destinations)

```python
# list_api_destinations method definition

await def list_api_destinations(
    self,
    *,
    NamePrefix: str = ...,
    ConnectionArn: str = ...,
    NextToken: str = ...,
    Limit: int = ...,
) -> ListApiDestinationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListApiDestinationsResponseTypeDef](./type_defs.md#listapidestinationsresponsetypedef) 


```python
# list_api_destinations method usage example with argument unpacking

kwargs: ListApiDestinationsRequestRequestTypeDef = {  # (1)
    "NamePrefix": ...,
}

parent.list_api_destinations(**kwargs)
```

1. See [:material-code-braces: ListApiDestinationsRequestRequestTypeDef](./type_defs.md#listapidestinationsrequestrequesttypedef) 

### list\_archives

Lists your archives.

Type annotations and code completion for `#!python session.create_client("events").list_archives` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_archives)

```python
# list_archives method definition

await def list_archives(
    self,
    *,
    NamePrefix: str = ...,
    EventSourceArn: str = ...,
    State: ArchiveStateType = ...,  # (1)
    NextToken: str = ...,
    Limit: int = ...,
) -> ListArchivesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ArchiveStateType](./literals.md#archivestatetype) 
2. See [:material-code-braces: ListArchivesResponseTypeDef](./type_defs.md#listarchivesresponsetypedef) 


```python
# list_archives method usage example with argument unpacking

kwargs: ListArchivesRequestRequestTypeDef = {  # (1)
    "NamePrefix": ...,
}

parent.list_archives(**kwargs)
```

1. See [:material-code-braces: ListArchivesRequestRequestTypeDef](./type_defs.md#listarchivesrequestrequesttypedef) 

### list\_connections

Retrieves a list of connections from the account.

Type annotations and code completion for `#!python session.create_client("events").list_connections` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_connections)

```python
# list_connections method definition

await def list_connections(
    self,
    *,
    NamePrefix: str = ...,
    ConnectionState: ConnectionStateType = ...,  # (1)
    NextToken: str = ...,
    Limit: int = ...,
) -> ListConnectionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ConnectionStateType](./literals.md#connectionstatetype) 
2. See [:material-code-braces: ListConnectionsResponseTypeDef](./type_defs.md#listconnectionsresponsetypedef) 


```python
# list_connections method usage example with argument unpacking

kwargs: ListConnectionsRequestRequestTypeDef = {  # (1)
    "NamePrefix": ...,
}

parent.list_connections(**kwargs)
```

1. See [:material-code-braces: ListConnectionsRequestRequestTypeDef](./type_defs.md#listconnectionsrequestrequesttypedef) 

### list\_endpoints

List the global endpoints associated with this account.

Type annotations and code completion for `#!python session.create_client("events").list_endpoints` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_endpoints)

```python
# list_endpoints method definition

await def list_endpoints(
    self,
    *,
    NamePrefix: str = ...,
    HomeRegion: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListEndpointsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEndpointsResponseTypeDef](./type_defs.md#listendpointsresponsetypedef) 


```python
# list_endpoints method usage example with argument unpacking

kwargs: ListEndpointsRequestRequestTypeDef = {  # (1)
    "NamePrefix": ...,
}

parent.list_endpoints(**kwargs)
```

1. See [:material-code-braces: ListEndpointsRequestRequestTypeDef](./type_defs.md#listendpointsrequestrequesttypedef) 

### list\_event\_buses

Lists all the event buses in your account, including the default event bus,
custom event buses, and partner event buses.

Type annotations and code completion for `#!python session.create_client("events").list_event_buses` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_event_buses)

```python
# list_event_buses method definition

await def list_event_buses(
    self,
    *,
    NamePrefix: str = ...,
    NextToken: str = ...,
    Limit: int = ...,
) -> ListEventBusesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEventBusesResponseTypeDef](./type_defs.md#listeventbusesresponsetypedef) 


```python
# list_event_buses method usage example with argument unpacking

kwargs: ListEventBusesRequestRequestTypeDef = {  # (1)
    "NamePrefix": ...,
}

parent.list_event_buses(**kwargs)
```

1. See [:material-code-braces: ListEventBusesRequestRequestTypeDef](./type_defs.md#listeventbusesrequestrequesttypedef) 

### list\_event\_sources

You can use this to see all the partner event sources that have been shared with
your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("events").list_event_sources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_event_sources)

```python
# list_event_sources method definition

await def list_event_sources(
    self,
    *,
    NamePrefix: str = ...,
    NextToken: str = ...,
    Limit: int = ...,
) -> ListEventSourcesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEventSourcesResponseTypeDef](./type_defs.md#listeventsourcesresponsetypedef) 


```python
# list_event_sources method usage example with argument unpacking

kwargs: ListEventSourcesRequestRequestTypeDef = {  # (1)
    "NamePrefix": ...,
}

parent.list_event_sources(**kwargs)
```

1. See [:material-code-braces: ListEventSourcesRequestRequestTypeDef](./type_defs.md#listeventsourcesrequestrequesttypedef) 

### list\_partner\_event\_source\_accounts

An SaaS partner can use this operation to display the Amazon Web Services
account ID that a particular partner event source name is associated with.

Type annotations and code completion for `#!python session.create_client("events").list_partner_event_source_accounts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_partner_event_source_accounts)

```python
# list_partner_event_source_accounts method definition

await def list_partner_event_source_accounts(
    self,
    *,
    EventSourceName: str,
    NextToken: str = ...,
    Limit: int = ...,
) -> ListPartnerEventSourceAccountsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPartnerEventSourceAccountsResponseTypeDef](./type_defs.md#listpartnereventsourceaccountsresponsetypedef) 


```python
# list_partner_event_source_accounts method usage example with argument unpacking

kwargs: ListPartnerEventSourceAccountsRequestRequestTypeDef = {  # (1)
    "EventSourceName": ...,
}

parent.list_partner_event_source_accounts(**kwargs)
```

1. See [:material-code-braces: ListPartnerEventSourceAccountsRequestRequestTypeDef](./type_defs.md#listpartnereventsourceaccountsrequestrequesttypedef) 

### list\_partner\_event\_sources

An SaaS partner can use this operation to list all the partner event source
names that they have created.

Type annotations and code completion for `#!python session.create_client("events").list_partner_event_sources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_partner_event_sources)

```python
# list_partner_event_sources method definition

await def list_partner_event_sources(
    self,
    *,
    NamePrefix: str,
    NextToken: str = ...,
    Limit: int = ...,
) -> ListPartnerEventSourcesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPartnerEventSourcesResponseTypeDef](./type_defs.md#listpartnereventsourcesresponsetypedef) 


```python
# list_partner_event_sources method usage example with argument unpacking

kwargs: ListPartnerEventSourcesRequestRequestTypeDef = {  # (1)
    "NamePrefix": ...,
}

parent.list_partner_event_sources(**kwargs)
```

1. See [:material-code-braces: ListPartnerEventSourcesRequestRequestTypeDef](./type_defs.md#listpartnereventsourcesrequestrequesttypedef) 

### list\_replays

Lists your replays.

Type annotations and code completion for `#!python session.create_client("events").list_replays` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_replays)

```python
# list_replays method definition

await def list_replays(
    self,
    *,
    NamePrefix: str = ...,
    State: ReplayStateType = ...,  # (1)
    EventSourceArn: str = ...,
    NextToken: str = ...,
    Limit: int = ...,
) -> ListReplaysResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ReplayStateType](./literals.md#replaystatetype) 
2. See [:material-code-braces: ListReplaysResponseTypeDef](./type_defs.md#listreplaysresponsetypedef) 


```python
# list_replays method usage example with argument unpacking

kwargs: ListReplaysRequestRequestTypeDef = {  # (1)
    "NamePrefix": ...,
}

parent.list_replays(**kwargs)
```

1. See [:material-code-braces: ListReplaysRequestRequestTypeDef](./type_defs.md#listreplaysrequestrequesttypedef) 

### list\_rule\_names\_by\_target

Lists the rules for the specified target.

Type annotations and code completion for `#!python session.create_client("events").list_rule_names_by_target` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_rule_names_by_target)

```python
# list_rule_names_by_target method definition

await def list_rule_names_by_target(
    self,
    *,
    TargetArn: str,
    EventBusName: str = ...,
    NextToken: str = ...,
    Limit: int = ...,
) -> ListRuleNamesByTargetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRuleNamesByTargetResponseTypeDef](./type_defs.md#listrulenamesbytargetresponsetypedef) 


```python
# list_rule_names_by_target method usage example with argument unpacking

kwargs: ListRuleNamesByTargetRequestRequestTypeDef = {  # (1)
    "TargetArn": ...,
}

parent.list_rule_names_by_target(**kwargs)
```

1. See [:material-code-braces: ListRuleNamesByTargetRequestRequestTypeDef](./type_defs.md#listrulenamesbytargetrequestrequesttypedef) 

### list\_rules

Lists your Amazon EventBridge rules.

Type annotations and code completion for `#!python session.create_client("events").list_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_rules)

```python
# list_rules method definition

await def list_rules(
    self,
    *,
    NamePrefix: str = ...,
    EventBusName: str = ...,
    NextToken: str = ...,
    Limit: int = ...,
) -> ListRulesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRulesResponseTypeDef](./type_defs.md#listrulesresponsetypedef) 


```python
# list_rules method usage example with argument unpacking

kwargs: ListRulesRequestRequestTypeDef = {  # (1)
    "NamePrefix": ...,
}

parent.list_rules(**kwargs)
```

1. See [:material-code-braces: ListRulesRequestRequestTypeDef](./type_defs.md#listrulesrequestrequesttypedef) 

### list\_tags\_for\_resource

Displays the tags associated with an EventBridge resource.

Type annotations and code completion for `#!python session.create_client("events").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceARN: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_targets\_by\_rule

Lists the targets assigned to the specified rule.

Type annotations and code completion for `#!python session.create_client("events").list_targets_by_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_targets_by_rule)

```python
# list_targets_by_rule method definition

await def list_targets_by_rule(
    self,
    *,
    Rule: str,
    EventBusName: str = ...,
    NextToken: str = ...,
    Limit: int = ...,
) -> ListTargetsByRuleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTargetsByRuleResponseTypeDef](./type_defs.md#listtargetsbyruleresponsetypedef) 


```python
# list_targets_by_rule method usage example with argument unpacking

kwargs: ListTargetsByRuleRequestRequestTypeDef = {  # (1)
    "Rule": ...,
}

parent.list_targets_by_rule(**kwargs)
```

1. See [:material-code-braces: ListTargetsByRuleRequestRequestTypeDef](./type_defs.md#listtargetsbyrulerequestrequesttypedef) 

### put\_events

Sends custom events to Amazon EventBridge so that they can be matched to rules.

Type annotations and code completion for `#!python session.create_client("events").put_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.put_events)

```python
# put_events method definition

await def put_events(
    self,
    *,
    Entries: Sequence[PutEventsRequestEntryTypeDef],  # (1)
    EndpointId: str = ...,
) -> PutEventsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PutEventsRequestEntryTypeDef](./type_defs.md#puteventsrequestentrytypedef) 
2. See [:material-code-braces: PutEventsResponseTypeDef](./type_defs.md#puteventsresponsetypedef) 


```python
# put_events method usage example with argument unpacking

kwargs: PutEventsRequestRequestTypeDef = {  # (1)
    "Entries": ...,
}

parent.put_events(**kwargs)
```

1. See [:material-code-braces: PutEventsRequestRequestTypeDef](./type_defs.md#puteventsrequestrequesttypedef) 

### put\_partner\_events

This is used by SaaS partners to write events to a customer's partner event bus.

Type annotations and code completion for `#!python session.create_client("events").put_partner_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.put_partner_events)

```python
# put_partner_events method definition

await def put_partner_events(
    self,
    *,
    Entries: Sequence[PutPartnerEventsRequestEntryTypeDef],  # (1)
) -> PutPartnerEventsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PutPartnerEventsRequestEntryTypeDef](./type_defs.md#putpartnereventsrequestentrytypedef) 
2. See [:material-code-braces: PutPartnerEventsResponseTypeDef](./type_defs.md#putpartnereventsresponsetypedef) 


```python
# put_partner_events method usage example with argument unpacking

kwargs: PutPartnerEventsRequestRequestTypeDef = {  # (1)
    "Entries": ...,
}

parent.put_partner_events(**kwargs)
```

1. See [:material-code-braces: PutPartnerEventsRequestRequestTypeDef](./type_defs.md#putpartnereventsrequestrequesttypedef) 

### put\_permission

Running `PutPermission` permits the specified Amazon Web Services account or
Amazon Web Services organization to put events to the specified *event bus*.

Type annotations and code completion for `#!python session.create_client("events").put_permission` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.put_permission)

```python
# put_permission method definition

await def put_permission(
    self,
    *,
    EventBusName: str = ...,
    Action: str = ...,
    Principal: str = ...,
    StatementId: str = ...,
    Condition: ConditionTypeDef = ...,  # (1)
    Policy: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_permission method usage example with argument unpacking

kwargs: PutPermissionRequestRequestTypeDef = {  # (1)
    "EventBusName": ...,
}

parent.put_permission(**kwargs)
```

1. See [:material-code-braces: PutPermissionRequestRequestTypeDef](./type_defs.md#putpermissionrequestrequesttypedef) 

### put\_rule

Creates or updates the specified rule.

Type annotations and code completion for `#!python session.create_client("events").put_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.put_rule)

```python
# put_rule method definition

await def put_rule(
    self,
    *,
    Name: str,
    ScheduleExpression: str = ...,
    EventPattern: str = ...,
    State: RuleStateType = ...,  # (1)
    Description: str = ...,
    RoleArn: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    EventBusName: str = ...,
) -> PutRuleResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: RuleStateType](./literals.md#rulestatetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: PutRuleResponseTypeDef](./type_defs.md#putruleresponsetypedef) 


```python
# put_rule method usage example with argument unpacking

kwargs: PutRuleRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.put_rule(**kwargs)
```

1. See [:material-code-braces: PutRuleRequestRequestTypeDef](./type_defs.md#putrulerequestrequesttypedef) 

### put\_targets

Adds the specified targets to the specified rule, or updates the targets if they
are already associated with the rule.

Type annotations and code completion for `#!python session.create_client("events").put_targets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.put_targets)

```python
# put_targets method definition

await def put_targets(
    self,
    *,
    Rule: str,
    Targets: Sequence[TargetTypeDef],  # (1)
    EventBusName: str = ...,
) -> PutTargetsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
2. See [:material-code-braces: PutTargetsResponseTypeDef](./type_defs.md#puttargetsresponsetypedef) 


```python
# put_targets method usage example with argument unpacking

kwargs: PutTargetsRequestRequestTypeDef = {  # (1)
    "Rule": ...,
    "Targets": ...,
}

parent.put_targets(**kwargs)
```

1. See [:material-code-braces: PutTargetsRequestRequestTypeDef](./type_defs.md#puttargetsrequestrequesttypedef) 

### remove\_permission

Revokes the permission of another Amazon Web Services account to be able to put
events to the specified event bus.

Type annotations and code completion for `#!python session.create_client("events").remove_permission` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.remove_permission)

```python
# remove_permission method definition

await def remove_permission(
    self,
    *,
    StatementId: str = ...,
    RemoveAllPermissions: bool = ...,
    EventBusName: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# remove_permission method usage example with argument unpacking

kwargs: RemovePermissionRequestRequestTypeDef = {  # (1)
    "StatementId": ...,
}

parent.remove_permission(**kwargs)
```

1. See [:material-code-braces: RemovePermissionRequestRequestTypeDef](./type_defs.md#removepermissionrequestrequesttypedef) 

### remove\_targets

Removes the specified targets from the specified rule.

Type annotations and code completion for `#!python session.create_client("events").remove_targets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.remove_targets)

```python
# remove_targets method definition

await def remove_targets(
    self,
    *,
    Rule: str,
    Ids: Sequence[str],
    EventBusName: str = ...,
    Force: bool = ...,
) -> RemoveTargetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RemoveTargetsResponseTypeDef](./type_defs.md#removetargetsresponsetypedef) 


```python
# remove_targets method usage example with argument unpacking

kwargs: RemoveTargetsRequestRequestTypeDef = {  # (1)
    "Rule": ...,
    "Ids": ...,
}

parent.remove_targets(**kwargs)
```

1. See [:material-code-braces: RemoveTargetsRequestRequestTypeDef](./type_defs.md#removetargetsrequestrequesttypedef) 

### start\_replay

Starts the specified replay.

Type annotations and code completion for `#!python session.create_client("events").start_replay` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.start_replay)

```python
# start_replay method definition

await def start_replay(
    self,
    *,
    ReplayName: str,
    EventSourceArn: str,
    EventStartTime: Union[datetime, str],
    EventEndTime: Union[datetime, str],
    Destination: ReplayDestinationTypeDef,  # (1)
    Description: str = ...,
) -> StartReplayResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ReplayDestinationTypeDef](./type_defs.md#replaydestinationtypedef) 
2. See [:material-code-braces: StartReplayResponseTypeDef](./type_defs.md#startreplayresponsetypedef) 


```python
# start_replay method usage example with argument unpacking

kwargs: StartReplayRequestRequestTypeDef = {  # (1)
    "ReplayName": ...,
    "EventSourceArn": ...,
    "EventStartTime": ...,
    "EventEndTime": ...,
    "Destination": ...,
}

parent.start_replay(**kwargs)
```

1. See [:material-code-braces: StartReplayRequestRequestTypeDef](./type_defs.md#startreplayrequestrequesttypedef) 

### tag\_resource

Assigns one or more tags (key-value pairs) to the specified EventBridge
resource.

Type annotations and code completion for `#!python session.create_client("events").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### test\_event\_pattern

Tests whether the specified event pattern matches the provided event.

Type annotations and code completion for `#!python session.create_client("events").test_event_pattern` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.test_event_pattern)

```python
# test_event_pattern method definition

await def test_event_pattern(
    self,
    *,
    EventPattern: str,
    Event: str,
) -> TestEventPatternResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: TestEventPatternResponseTypeDef](./type_defs.md#testeventpatternresponsetypedef) 


```python
# test_event_pattern method usage example with argument unpacking

kwargs: TestEventPatternRequestRequestTypeDef = {  # (1)
    "EventPattern": ...,
    "Event": ...,
}

parent.test_event_pattern(**kwargs)
```

1. See [:material-code-braces: TestEventPatternRequestRequestTypeDef](./type_defs.md#testeventpatternrequestrequesttypedef) 

### untag\_resource

Removes one or more tags from the specified EventBridge resource.

Type annotations and code completion for `#!python session.create_client("events").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceARN: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceARN": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_api\_destination

Updates an API destination.

Type annotations and code completion for `#!python session.create_client("events").update_api_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.update_api_destination)

```python
# update_api_destination method definition

await def update_api_destination(
    self,
    *,
    Name: str,
    Description: str = ...,
    ConnectionArn: str = ...,
    InvocationEndpoint: str = ...,
    HttpMethod: ApiDestinationHttpMethodType = ...,  # (1)
    InvocationRateLimitPerSecond: int = ...,
) -> UpdateApiDestinationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ApiDestinationHttpMethodType](./literals.md#apidestinationhttpmethodtype) 
2. See [:material-code-braces: UpdateApiDestinationResponseTypeDef](./type_defs.md#updateapidestinationresponsetypedef) 


```python
# update_api_destination method usage example with argument unpacking

kwargs: UpdateApiDestinationRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.update_api_destination(**kwargs)
```

1. See [:material-code-braces: UpdateApiDestinationRequestRequestTypeDef](./type_defs.md#updateapidestinationrequestrequesttypedef) 

### update\_archive

Updates the specified archive.

Type annotations and code completion for `#!python session.create_client("events").update_archive` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.update_archive)

```python
# update_archive method definition

await def update_archive(
    self,
    *,
    ArchiveName: str,
    Description: str = ...,
    EventPattern: str = ...,
    RetentionDays: int = ...,
) -> UpdateArchiveResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateArchiveResponseTypeDef](./type_defs.md#updatearchiveresponsetypedef) 


```python
# update_archive method usage example with argument unpacking

kwargs: UpdateArchiveRequestRequestTypeDef = {  # (1)
    "ArchiveName": ...,
}

parent.update_archive(**kwargs)
```

1. See [:material-code-braces: UpdateArchiveRequestRequestTypeDef](./type_defs.md#updatearchiverequestrequesttypedef) 

### update\_connection

Updates settings for a connection.

Type annotations and code completion for `#!python session.create_client("events").update_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.update_connection)

```python
# update_connection method definition

await def update_connection(
    self,
    *,
    Name: str,
    Description: str = ...,
    AuthorizationType: ConnectionAuthorizationTypeType = ...,  # (1)
    AuthParameters: UpdateConnectionAuthRequestParametersTypeDef = ...,  # (2)
) -> UpdateConnectionResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ConnectionAuthorizationTypeType](./literals.md#connectionauthorizationtypetype) 
2. See [:material-code-braces: UpdateConnectionAuthRequestParametersTypeDef](./type_defs.md#updateconnectionauthrequestparameterstypedef) 
3. See [:material-code-braces: UpdateConnectionResponseTypeDef](./type_defs.md#updateconnectionresponsetypedef) 


```python
# update_connection method usage example with argument unpacking

kwargs: UpdateConnectionRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.update_connection(**kwargs)
```

1. See [:material-code-braces: UpdateConnectionRequestRequestTypeDef](./type_defs.md#updateconnectionrequestrequesttypedef) 

### update\_endpoint

Update an existing endpoint.

Type annotations and code completion for `#!python session.create_client("events").update_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.update_endpoint)

```python
# update_endpoint method definition

await def update_endpoint(
    self,
    *,
    Name: str,
    Description: str = ...,
    RoutingConfig: RoutingConfigTypeDef = ...,  # (1)
    ReplicationConfig: ReplicationConfigTypeDef = ...,  # (2)
    EventBuses: Sequence[EndpointEventBusTypeDef] = ...,  # (3)
    RoleArn: str = ...,
) -> UpdateEndpointResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: RoutingConfigTypeDef](./type_defs.md#routingconfigtypedef) 
2. See [:material-code-braces: ReplicationConfigTypeDef](./type_defs.md#replicationconfigtypedef) 
3. See [:material-code-braces: EndpointEventBusTypeDef](./type_defs.md#endpointeventbustypedef) 
4. See [:material-code-braces: UpdateEndpointResponseTypeDef](./type_defs.md#updateendpointresponsetypedef) 


```python
# update_endpoint method usage example with argument unpacking

kwargs: UpdateEndpointRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.update_endpoint(**kwargs)
```

1. See [:material-code-braces: UpdateEndpointRequestRequestTypeDef](./type_defs.md#updateendpointrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("events").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> EventBridgeClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("events").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("events").get_paginator` method with overloads.

- `client.get_paginator("list_rule_names_by_target")` -> [ListRuleNamesByTargetPaginator](./paginators.md#listrulenamesbytargetpaginator)
- `client.get_paginator("list_rules")` -> [ListRulesPaginator](./paginators.md#listrulespaginator)
- `client.get_paginator("list_targets_by_rule")` -> [ListTargetsByRulePaginator](./paginators.md#listtargetsbyrulepaginator)



