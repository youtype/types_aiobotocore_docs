<a id="eventbridgeclient-for-aiobotocore-eventbridge-module"></a>

# EventBridgeClient for aiobotocore EventBridge module

> [Index](../README.md) > [EventBridge](./README.md) > EventBridgeClient

Auto-generated documentation for
[EventBridge](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
type annotations stubs module
[types-aiobotocore-events](https://pypi.org/project/types-aiobotocore-events/).

- [EventBridgeClient for aiobotocore EventBridge module](#eventbridgeclient-for-aiobotocore-eventbridge-module)
  - [EventBridgeClient](#eventbridgeclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [activate_event_source](#activate_event_source)
    - [can_paginate](#can_paginate)
    - [cancel_replay](#cancel_replay)
    - [create_api_destination](#create_api_destination)
    - [create_archive](#create_archive)
    - [create_connection](#create_connection)
    - [create_event_bus](#create_event_bus)
    - [create_partner_event_source](#create_partner_event_source)
    - [deactivate_event_source](#deactivate_event_source)
    - [deauthorize_connection](#deauthorize_connection)
    - [delete_api_destination](#delete_api_destination)
    - [delete_archive](#delete_archive)
    - [delete_connection](#delete_connection)
    - [delete_event_bus](#delete_event_bus)
    - [delete_partner_event_source](#delete_partner_event_source)
    - [delete_rule](#delete_rule)
    - [describe_api_destination](#describe_api_destination)
    - [describe_archive](#describe_archive)
    - [describe_connection](#describe_connection)
    - [describe_event_bus](#describe_event_bus)
    - [describe_event_source](#describe_event_source)
    - [describe_partner_event_source](#describe_partner_event_source)
    - [describe_replay](#describe_replay)
    - [describe_rule](#describe_rule)
    - [disable_rule](#disable_rule)
    - [enable_rule](#enable_rule)
    - [generate_presigned_url](#generate_presigned_url)
    - [list_api_destinations](#list_api_destinations)
    - [list_archives](#list_archives)
    - [list_connections](#list_connections)
    - [list_event_buses](#list_event_buses)
    - [list_event_sources](#list_event_sources)
    - [list_partner_event_source_accounts](#list_partner_event_source_accounts)
    - [list_partner_event_sources](#list_partner_event_sources)
    - [list_replays](#list_replays)
    - [list_rule_names_by_target](#list_rule_names_by_target)
    - [list_rules](#list_rules)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [list_targets_by_rule](#list_targets_by_rule)
    - [put_events](#put_events)
    - [put_partner_events](#put_partner_events)
    - [put_permission](#put_permission)
    - [put_rule](#put_rule)
    - [put_targets](#put_targets)
    - [remove_permission](#remove_permission)
    - [remove_targets](#remove_targets)
    - [start_replay](#start_replay)
    - [tag_resource](#tag_resource)
    - [test_event_pattern](#test_event_pattern)
    - [untag_resource](#untag_resource)
    - [update_api_destination](#update_api_destination)
    - [update_archive](#update_archive)
    - [update_connection](#update_connection)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="eventbridgeclient"></a>

## EventBridgeClient

Type annotations for `session.create_client("events")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_events.client import EventBridgeClient

session = get_session()
async with session.create_client("events") as client:
    client: EventBridgeClient
```

Boto3 documentation:
[EventBridge.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_events.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.ConcurrentModificationException`
- `Exceptions.IllegalStatusException`
- `Exceptions.InternalException`
- `Exceptions.InvalidEventPatternException`
- `Exceptions.InvalidStateException`
- `Exceptions.LimitExceededException`
- `Exceptions.ManagedRuleException`
- `Exceptions.OperationDisabledException`
- `Exceptions.PolicyLengthExceededException`
- `Exceptions.ResourceAlreadyExistsException`
- `Exceptions.ResourceNotFoundException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

EventBridgeClient exceptions.

Type annotations for `session.create_client("events").exceptions` method.

Boto3 documentation:
[EventBridge.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="activate\_event\_source"></a>

### activate_event_source

Activates a partner event source that has been deactivated.

Type annotations for `session.create_client("events").activate_event_source`
method.

Boto3 documentation:
[EventBridge.Client.activate_event_source](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.activate_event_source)

Asynchronous method. Use `await activate_event_source(...)` for a synchronous
call.

Arguments mapping described in
[ActivateEventSourceRequestRequestTypeDef](./type_defs.md#activateeventsourcerequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("events").can_paginate` method.

Boto3 documentation:
[EventBridge.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="cancel\_replay"></a>

### cancel_replay

Cancels the specified replay.

Type annotations for `session.create_client("events").cancel_replay` method.

Boto3 documentation:
[EventBridge.Client.cancel_replay](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.cancel_replay)

Asynchronous method. Use `await cancel_replay(...)` for a synchronous call.

Arguments mapping described in
[CancelReplayRequestRequestTypeDef](./type_defs.md#cancelreplayrequestrequesttypedef).

Keyword-only arguments:

- `ReplayName`: `str` *(required)*

Returns a `Coroutine` for
[CancelReplayResponseTypeDef](./type_defs.md#cancelreplayresponsetypedef).

<a id="create\_api\_destination"></a>

### create_api_destination

Creates an API destination, which is an HTTP invocation endpoint configured as
a target for events.

Type annotations for `session.create_client("events").create_api_destination`
method.

Boto3 documentation:
[EventBridge.Client.create_api_destination](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.create_api_destination)

Asynchronous method. Use `await create_api_destination(...)` for a synchronous
call.

Arguments mapping described in
[CreateApiDestinationRequestRequestTypeDef](./type_defs.md#createapidestinationrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `ConnectionArn`: `str` *(required)*
- `InvocationEndpoint`: `str` *(required)*
- `HttpMethod`:
  [ApiDestinationHttpMethodType](./literals.md#apidestinationhttpmethodtype)
  *(required)*
- `Description`: `str`
- `InvocationRateLimitPerSecond`: `int`

Returns a `Coroutine` for
[CreateApiDestinationResponseTypeDef](./type_defs.md#createapidestinationresponsetypedef).

<a id="create\_archive"></a>

### create_archive

Creates an archive of events with the specified settings.

Type annotations for `session.create_client("events").create_archive` method.

Boto3 documentation:
[EventBridge.Client.create_archive](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.create_archive)

Asynchronous method. Use `await create_archive(...)` for a synchronous call.

Arguments mapping described in
[CreateArchiveRequestRequestTypeDef](./type_defs.md#createarchiverequestrequesttypedef).

Keyword-only arguments:

- `ArchiveName`: `str` *(required)*
- `EventSourceArn`: `str` *(required)*
- `Description`: `str`
- `EventPattern`: `str`
- `RetentionDays`: `int`

Returns a `Coroutine` for
[CreateArchiveResponseTypeDef](./type_defs.md#createarchiveresponsetypedef).

<a id="create\_connection"></a>

### create_connection

Creates a connection.

Type annotations for `session.create_client("events").create_connection`
method.

Boto3 documentation:
[EventBridge.Client.create_connection](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.create_connection)

Asynchronous method. Use `await create_connection(...)` for a synchronous call.

Arguments mapping described in
[CreateConnectionRequestRequestTypeDef](./type_defs.md#createconnectionrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `AuthorizationType`:
  [ConnectionAuthorizationTypeType](./literals.md#connectionauthorizationtypetype)
  *(required)*
- `AuthParameters`:
  [CreateConnectionAuthRequestParametersTypeDef](./type_defs.md#createconnectionauthrequestparameterstypedef)
  *(required)*
- `Description`: `str`

Returns a `Coroutine` for
[CreateConnectionResponseTypeDef](./type_defs.md#createconnectionresponsetypedef).

<a id="create\_event\_bus"></a>

### create_event_bus

Creates a new event bus within your account.

Type annotations for `session.create_client("events").create_event_bus` method.

Boto3 documentation:
[EventBridge.Client.create_event_bus](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.create_event_bus)

Asynchronous method. Use `await create_event_bus(...)` for a synchronous call.

Arguments mapping described in
[CreateEventBusRequestRequestTypeDef](./type_defs.md#createeventbusrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `EventSourceName`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateEventBusResponseTypeDef](./type_defs.md#createeventbusresponsetypedef).

<a id="create\_partner\_event\_source"></a>

### create_partner_event_source

Called by an SaaS partner to create a partner event source.

Type annotations for
`session.create_client("events").create_partner_event_source` method.

Boto3 documentation:
[EventBridge.Client.create_partner_event_source](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.create_partner_event_source)

Asynchronous method. Use `await create_partner_event_source(...)` for a
synchronous call.

Arguments mapping described in
[CreatePartnerEventSourceRequestRequestTypeDef](./type_defs.md#createpartnereventsourcerequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `Account`: `str` *(required)*

Returns a `Coroutine` for
[CreatePartnerEventSourceResponseTypeDef](./type_defs.md#createpartnereventsourceresponsetypedef).

<a id="deactivate\_event\_source"></a>

### deactivate_event_source

You can use this operation to temporarily stop receiving events from the
specified partner event source.

Type annotations for `session.create_client("events").deactivate_event_source`
method.

Boto3 documentation:
[EventBridge.Client.deactivate_event_source](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.deactivate_event_source)

Asynchronous method. Use `await deactivate_event_source(...)` for a synchronous
call.

Arguments mapping described in
[DeactivateEventSourceRequestRequestTypeDef](./type_defs.md#deactivateeventsourcerequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

<a id="deauthorize\_connection"></a>

### deauthorize_connection

Removes all authorization parameters from the connection.

Type annotations for `session.create_client("events").deauthorize_connection`
method.

Boto3 documentation:
[EventBridge.Client.deauthorize_connection](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.deauthorize_connection)

Asynchronous method. Use `await deauthorize_connection(...)` for a synchronous
call.

Arguments mapping described in
[DeauthorizeConnectionRequestRequestTypeDef](./type_defs.md#deauthorizeconnectionrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for
[DeauthorizeConnectionResponseTypeDef](./type_defs.md#deauthorizeconnectionresponsetypedef).

<a id="delete\_api\_destination"></a>

### delete_api_destination

Deletes the specified API destination.

Type annotations for `session.create_client("events").delete_api_destination`
method.

Boto3 documentation:
[EventBridge.Client.delete_api_destination](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.delete_api_destination)

Asynchronous method. Use `await delete_api_destination(...)` for a synchronous
call.

Arguments mapping described in
[DeleteApiDestinationRequestRequestTypeDef](./type_defs.md#deleteapidestinationrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_archive"></a>

### delete_archive

Deletes the specified archive.

Type annotations for `session.create_client("events").delete_archive` method.

Boto3 documentation:
[EventBridge.Client.delete_archive](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.delete_archive)

Asynchronous method. Use `await delete_archive(...)` for a synchronous call.

Arguments mapping described in
[DeleteArchiveRequestRequestTypeDef](./type_defs.md#deletearchiverequestrequesttypedef).

Keyword-only arguments:

- `ArchiveName`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_connection"></a>

### delete_connection

Deletes a connection.

Type annotations for `session.create_client("events").delete_connection`
method.

Boto3 documentation:
[EventBridge.Client.delete_connection](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.delete_connection)

Asynchronous method. Use `await delete_connection(...)` for a synchronous call.

Arguments mapping described in
[DeleteConnectionRequestRequestTypeDef](./type_defs.md#deleteconnectionrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for
[DeleteConnectionResponseTypeDef](./type_defs.md#deleteconnectionresponsetypedef).

<a id="delete\_event\_bus"></a>

### delete_event_bus

Deletes the specified custom event bus or partner event bus.

Type annotations for `session.create_client("events").delete_event_bus` method.

Boto3 documentation:
[EventBridge.Client.delete_event_bus](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.delete_event_bus)

Asynchronous method. Use `await delete_event_bus(...)` for a synchronous call.

Arguments mapping described in
[DeleteEventBusRequestRequestTypeDef](./type_defs.md#deleteeventbusrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

<a id="delete\_partner\_event\_source"></a>

### delete_partner_event_source

This operation is used by SaaS partners to delete a partner event source.

Type annotations for
`session.create_client("events").delete_partner_event_source` method.

Boto3 documentation:
[EventBridge.Client.delete_partner_event_source](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.delete_partner_event_source)

Asynchronous method. Use `await delete_partner_event_source(...)` for a
synchronous call.

Arguments mapping described in
[DeletePartnerEventSourceRequestRequestTypeDef](./type_defs.md#deletepartnereventsourcerequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `Account`: `str` *(required)*

<a id="delete\_rule"></a>

### delete_rule

Deletes the specified rule.

Type annotations for `session.create_client("events").delete_rule` method.

Boto3 documentation:
[EventBridge.Client.delete_rule](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.delete_rule)

Asynchronous method. Use `await delete_rule(...)` for a synchronous call.

Arguments mapping described in
[DeleteRuleRequestRequestTypeDef](./type_defs.md#deleterulerequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `EventBusName`: `str`
- `Force`: `bool`

<a id="describe\_api\_destination"></a>

### describe_api_destination

Retrieves details about an API destination.

Type annotations for `session.create_client("events").describe_api_destination`
method.

Boto3 documentation:
[EventBridge.Client.describe_api_destination](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.describe_api_destination)

Asynchronous method. Use `await describe_api_destination(...)` for a
synchronous call.

Arguments mapping described in
[DescribeApiDestinationRequestRequestTypeDef](./type_defs.md#describeapidestinationrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for
[DescribeApiDestinationResponseTypeDef](./type_defs.md#describeapidestinationresponsetypedef).

<a id="describe\_archive"></a>

### describe_archive

Retrieves details about an archive.

Type annotations for `session.create_client("events").describe_archive` method.

Boto3 documentation:
[EventBridge.Client.describe_archive](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.describe_archive)

Asynchronous method. Use `await describe_archive(...)` for a synchronous call.

Arguments mapping described in
[DescribeArchiveRequestRequestTypeDef](./type_defs.md#describearchiverequestrequesttypedef).

Keyword-only arguments:

- `ArchiveName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeArchiveResponseTypeDef](./type_defs.md#describearchiveresponsetypedef).

<a id="describe\_connection"></a>

### describe_connection

Retrieves details about a connection.

Type annotations for `session.create_client("events").describe_connection`
method.

Boto3 documentation:
[EventBridge.Client.describe_connection](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.describe_connection)

Asynchronous method. Use `await describe_connection(...)` for a synchronous
call.

Arguments mapping described in
[DescribeConnectionRequestRequestTypeDef](./type_defs.md#describeconnectionrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for
[DescribeConnectionResponseTypeDef](./type_defs.md#describeconnectionresponsetypedef).

<a id="describe\_event\_bus"></a>

### describe_event_bus

Displays details about an event bus in your account.

Type annotations for `session.create_client("events").describe_event_bus`
method.

Boto3 documentation:
[EventBridge.Client.describe_event_bus](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.describe_event_bus)

Asynchronous method. Use `await describe_event_bus(...)` for a synchronous
call.

Arguments mapping described in
[DescribeEventBusRequestRequestTypeDef](./type_defs.md#describeeventbusrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str`

Returns a `Coroutine` for
[DescribeEventBusResponseTypeDef](./type_defs.md#describeeventbusresponsetypedef).

<a id="describe\_event\_source"></a>

### describe_event_source

This operation lists details about a partner event source that is shared with
your account.

Type annotations for `session.create_client("events").describe_event_source`
method.

Boto3 documentation:
[EventBridge.Client.describe_event_source](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.describe_event_source)

Asynchronous method. Use `await describe_event_source(...)` for a synchronous
call.

Arguments mapping described in
[DescribeEventSourceRequestRequestTypeDef](./type_defs.md#describeeventsourcerequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for
[DescribeEventSourceResponseTypeDef](./type_defs.md#describeeventsourceresponsetypedef).

<a id="describe\_partner\_event\_source"></a>

### describe_partner_event_source

An SaaS partner can use this operation to list details about a partner event
source that they have created.

Type annotations for
`session.create_client("events").describe_partner_event_source` method.

Boto3 documentation:
[EventBridge.Client.describe_partner_event_source](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.describe_partner_event_source)

Asynchronous method. Use `await describe_partner_event_source(...)` for a
synchronous call.

Arguments mapping described in
[DescribePartnerEventSourceRequestRequestTypeDef](./type_defs.md#describepartnereventsourcerequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for
[DescribePartnerEventSourceResponseTypeDef](./type_defs.md#describepartnereventsourceresponsetypedef).

<a id="describe\_replay"></a>

### describe_replay

Retrieves details about a replay.

Type annotations for `session.create_client("events").describe_replay` method.

Boto3 documentation:
[EventBridge.Client.describe_replay](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.describe_replay)

Asynchronous method. Use `await describe_replay(...)` for a synchronous call.

Arguments mapping described in
[DescribeReplayRequestRequestTypeDef](./type_defs.md#describereplayrequestrequesttypedef).

Keyword-only arguments:

- `ReplayName`: `str` *(required)*

Returns a `Coroutine` for
[DescribeReplayResponseTypeDef](./type_defs.md#describereplayresponsetypedef).

<a id="describe\_rule"></a>

### describe_rule

Describes the specified rule.

Type annotations for `session.create_client("events").describe_rule` method.

Boto3 documentation:
[EventBridge.Client.describe_rule](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.describe_rule)

Asynchronous method. Use `await describe_rule(...)` for a synchronous call.

Arguments mapping described in
[DescribeRuleRequestRequestTypeDef](./type_defs.md#describerulerequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `EventBusName`: `str`

Returns a `Coroutine` for
[DescribeRuleResponseTypeDef](./type_defs.md#describeruleresponsetypedef).

<a id="disable\_rule"></a>

### disable_rule

Disables the specified rule.

Type annotations for `session.create_client("events").disable_rule` method.

Boto3 documentation:
[EventBridge.Client.disable_rule](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.disable_rule)

Asynchronous method. Use `await disable_rule(...)` for a synchronous call.

Arguments mapping described in
[DisableRuleRequestRequestTypeDef](./type_defs.md#disablerulerequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `EventBusName`: `str`

<a id="enable\_rule"></a>

### enable_rule

Enables the specified rule.

Type annotations for `session.create_client("events").enable_rule` method.

Boto3 documentation:
[EventBridge.Client.enable_rule](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.enable_rule)

Asynchronous method. Use `await enable_rule(...)` for a synchronous call.

Arguments mapping described in
[EnableRuleRequestRequestTypeDef](./type_defs.md#enablerulerequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `EventBusName`: `str`

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("events").generate_presigned_url`
method.

Boto3 documentation:
[EventBridge.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="list\_api\_destinations"></a>

### list_api_destinations

Retrieves a list of API destination in the account in the current Region.

Type annotations for `session.create_client("events").list_api_destinations`
method.

Boto3 documentation:
[EventBridge.Client.list_api_destinations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_api_destinations)

Asynchronous method. Use `await list_api_destinations(...)` for a synchronous
call.

Arguments mapping described in
[ListApiDestinationsRequestRequestTypeDef](./type_defs.md#listapidestinationsrequestrequesttypedef).

Keyword-only arguments:

- `NamePrefix`: `str`
- `ConnectionArn`: `str`
- `NextToken`: `str`
- `Limit`: `int`

Returns a `Coroutine` for
[ListApiDestinationsResponseTypeDef](./type_defs.md#listapidestinationsresponsetypedef).

<a id="list\_archives"></a>

### list_archives

Lists your archives.

Type annotations for `session.create_client("events").list_archives` method.

Boto3 documentation:
[EventBridge.Client.list_archives](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_archives)

Asynchronous method. Use `await list_archives(...)` for a synchronous call.

Arguments mapping described in
[ListArchivesRequestRequestTypeDef](./type_defs.md#listarchivesrequestrequesttypedef).

Keyword-only arguments:

- `NamePrefix`: `str`
- `EventSourceArn`: `str`
- `State`: [ArchiveStateType](./literals.md#archivestatetype)
- `NextToken`: `str`
- `Limit`: `int`

Returns a `Coroutine` for
[ListArchivesResponseTypeDef](./type_defs.md#listarchivesresponsetypedef).

<a id="list\_connections"></a>

### list_connections

Retrieves a list of connections from the account.

Type annotations for `session.create_client("events").list_connections` method.

Boto3 documentation:
[EventBridge.Client.list_connections](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_connections)

Asynchronous method. Use `await list_connections(...)` for a synchronous call.

Arguments mapping described in
[ListConnectionsRequestRequestTypeDef](./type_defs.md#listconnectionsrequestrequesttypedef).

Keyword-only arguments:

- `NamePrefix`: `str`
- `ConnectionState`: [ConnectionStateType](./literals.md#connectionstatetype)
- `NextToken`: `str`
- `Limit`: `int`

Returns a `Coroutine` for
[ListConnectionsResponseTypeDef](./type_defs.md#listconnectionsresponsetypedef).

<a id="list\_event\_buses"></a>

### list_event_buses

Lists all the event buses in your account, including the default event bus,
custom event buses, and partner event buses.

Type annotations for `session.create_client("events").list_event_buses` method.

Boto3 documentation:
[EventBridge.Client.list_event_buses](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_event_buses)

Asynchronous method. Use `await list_event_buses(...)` for a synchronous call.

Arguments mapping described in
[ListEventBusesRequestRequestTypeDef](./type_defs.md#listeventbusesrequestrequesttypedef).

Keyword-only arguments:

- `NamePrefix`: `str`
- `NextToken`: `str`
- `Limit`: `int`

Returns a `Coroutine` for
[ListEventBusesResponseTypeDef](./type_defs.md#listeventbusesresponsetypedef).

<a id="list\_event\_sources"></a>

### list_event_sources

You can use this to see all the partner event sources that have been shared
with your Amazon Web Services account.

Type annotations for `session.create_client("events").list_event_sources`
method.

Boto3 documentation:
[EventBridge.Client.list_event_sources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_event_sources)

Asynchronous method. Use `await list_event_sources(...)` for a synchronous
call.

Arguments mapping described in
[ListEventSourcesRequestRequestTypeDef](./type_defs.md#listeventsourcesrequestrequesttypedef).

Keyword-only arguments:

- `NamePrefix`: `str`
- `NextToken`: `str`
- `Limit`: `int`

Returns a `Coroutine` for
[ListEventSourcesResponseTypeDef](./type_defs.md#listeventsourcesresponsetypedef).

<a id="list\_partner\_event\_source\_accounts"></a>

### list_partner_event_source_accounts

An SaaS partner can use this operation to display the Amazon Web Services
account ID that a particular partner event source name is associated with.

Type annotations for
`session.create_client("events").list_partner_event_source_accounts` method.

Boto3 documentation:
[EventBridge.Client.list_partner_event_source_accounts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_partner_event_source_accounts)

Asynchronous method. Use `await list_partner_event_source_accounts(...)` for a
synchronous call.

Arguments mapping described in
[ListPartnerEventSourceAccountsRequestRequestTypeDef](./type_defs.md#listpartnereventsourceaccountsrequestrequesttypedef).

Keyword-only arguments:

- `EventSourceName`: `str` *(required)*
- `NextToken`: `str`
- `Limit`: `int`

Returns a `Coroutine` for
[ListPartnerEventSourceAccountsResponseTypeDef](./type_defs.md#listpartnereventsourceaccountsresponsetypedef).

<a id="list\_partner\_event\_sources"></a>

### list_partner_event_sources

An SaaS partner can use this operation to list all the partner event source
names that they have created.

Type annotations for
`session.create_client("events").list_partner_event_sources` method.

Boto3 documentation:
[EventBridge.Client.list_partner_event_sources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_partner_event_sources)

Asynchronous method. Use `await list_partner_event_sources(...)` for a
synchronous call.

Arguments mapping described in
[ListPartnerEventSourcesRequestRequestTypeDef](./type_defs.md#listpartnereventsourcesrequestrequesttypedef).

Keyword-only arguments:

- `NamePrefix`: `str` *(required)*
- `NextToken`: `str`
- `Limit`: `int`

Returns a `Coroutine` for
[ListPartnerEventSourcesResponseTypeDef](./type_defs.md#listpartnereventsourcesresponsetypedef).

<a id="list\_replays"></a>

### list_replays

Lists your replays.

Type annotations for `session.create_client("events").list_replays` method.

Boto3 documentation:
[EventBridge.Client.list_replays](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_replays)

Asynchronous method. Use `await list_replays(...)` for a synchronous call.

Arguments mapping described in
[ListReplaysRequestRequestTypeDef](./type_defs.md#listreplaysrequestrequesttypedef).

Keyword-only arguments:

- `NamePrefix`: `str`
- `State`: [ReplayStateType](./literals.md#replaystatetype)
- `EventSourceArn`: `str`
- `NextToken`: `str`
- `Limit`: `int`

Returns a `Coroutine` for
[ListReplaysResponseTypeDef](./type_defs.md#listreplaysresponsetypedef).

<a id="list\_rule\_names\_by\_target"></a>

### list_rule_names_by_target

Lists the rules for the specified target.

Type annotations for
`session.create_client("events").list_rule_names_by_target` method.

Boto3 documentation:
[EventBridge.Client.list_rule_names_by_target](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_rule_names_by_target)

Asynchronous method. Use `await list_rule_names_by_target(...)` for a
synchronous call.

Arguments mapping described in
[ListRuleNamesByTargetRequestRequestTypeDef](./type_defs.md#listrulenamesbytargetrequestrequesttypedef).

Keyword-only arguments:

- `TargetArn`: `str` *(required)*
- `EventBusName`: `str`
- `NextToken`: `str`
- `Limit`: `int`

Returns a `Coroutine` for
[ListRuleNamesByTargetResponseTypeDef](./type_defs.md#listrulenamesbytargetresponsetypedef).

<a id="list\_rules"></a>

### list_rules

Lists your Amazon EventBridge rules.

Type annotations for `session.create_client("events").list_rules` method.

Boto3 documentation:
[EventBridge.Client.list_rules](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_rules)

Asynchronous method. Use `await list_rules(...)` for a synchronous call.

Arguments mapping described in
[ListRulesRequestRequestTypeDef](./type_defs.md#listrulesrequestrequesttypedef).

Keyword-only arguments:

- `NamePrefix`: `str`
- `EventBusName`: `str`
- `NextToken`: `str`
- `Limit`: `int`

Returns a `Coroutine` for
[ListRulesResponseTypeDef](./type_defs.md#listrulesresponsetypedef).

<a id="list\_tags\_for\_resource"></a>

### list_tags_for_resource

Displays the tags associated with an EventBridge resource.

Type annotations for `session.create_client("events").list_tags_for_resource`
method.

Boto3 documentation:
[EventBridge.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceARN`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="list\_targets\_by\_rule"></a>

### list_targets_by_rule

Lists the targets assigned to the specified rule.

Type annotations for `session.create_client("events").list_targets_by_rule`
method.

Boto3 documentation:
[EventBridge.Client.list_targets_by_rule](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_targets_by_rule)

Asynchronous method. Use `await list_targets_by_rule(...)` for a synchronous
call.

Arguments mapping described in
[ListTargetsByRuleRequestRequestTypeDef](./type_defs.md#listtargetsbyrulerequestrequesttypedef).

Keyword-only arguments:

- `Rule`: `str` *(required)*
- `EventBusName`: `str`
- `NextToken`: `str`
- `Limit`: `int`

Returns a `Coroutine` for
[ListTargetsByRuleResponseTypeDef](./type_defs.md#listtargetsbyruleresponsetypedef).

<a id="put\_events"></a>

### put_events

Sends custom events to Amazon EventBridge so that they can be matched to rules.

Type annotations for `session.create_client("events").put_events` method.

Boto3 documentation:
[EventBridge.Client.put_events](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.put_events)

Asynchronous method. Use `await put_events(...)` for a synchronous call.

Arguments mapping described in
[PutEventsRequestRequestTypeDef](./type_defs.md#puteventsrequestrequesttypedef).

Keyword-only arguments:

- `Entries`:
  `Sequence`\[[PutEventsRequestEntryTypeDef](./type_defs.md#puteventsrequestentrytypedef)\]
  *(required)*

Returns a `Coroutine` for
[PutEventsResponseTypeDef](./type_defs.md#puteventsresponsetypedef).

<a id="put\_partner\_events"></a>

### put_partner_events

This is used by SaaS partners to write events to a customer's partner event
bus.

Type annotations for `session.create_client("events").put_partner_events`
method.

Boto3 documentation:
[EventBridge.Client.put_partner_events](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.put_partner_events)

Asynchronous method. Use `await put_partner_events(...)` for a synchronous
call.

Arguments mapping described in
[PutPartnerEventsRequestRequestTypeDef](./type_defs.md#putpartnereventsrequestrequesttypedef).

Keyword-only arguments:

- `Entries`:
  `Sequence`\[[PutPartnerEventsRequestEntryTypeDef](./type_defs.md#putpartnereventsrequestentrytypedef)\]
  *(required)*

Returns a `Coroutine` for
[PutPartnerEventsResponseTypeDef](./type_defs.md#putpartnereventsresponsetypedef).

<a id="put\_permission"></a>

### put_permission

Running `PutPermission` permits the specified Amazon Web Services account or
Amazon Web Services organization to put events to the specified *event bus*.

Type annotations for `session.create_client("events").put_permission` method.

Boto3 documentation:
[EventBridge.Client.put_permission](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.put_permission)

Asynchronous method. Use `await put_permission(...)` for a synchronous call.

Arguments mapping described in
[PutPermissionRequestRequestTypeDef](./type_defs.md#putpermissionrequestrequesttypedef).

Keyword-only arguments:

- `EventBusName`: `str`
- `Action`: `str`
- `Principal`: `str`
- `StatementId`: `str`
- `Condition`: [ConditionTypeDef](./type_defs.md#conditiontypedef)
- `Policy`: `str`

<a id="put\_rule"></a>

### put_rule

Creates or updates the specified rule.

Type annotations for `session.create_client("events").put_rule` method.

Boto3 documentation:
[EventBridge.Client.put_rule](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.put_rule)

Asynchronous method. Use `await put_rule(...)` for a synchronous call.

Arguments mapping described in
[PutRuleRequestRequestTypeDef](./type_defs.md#putrulerequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `ScheduleExpression`: `str`
- `EventPattern`: `str`
- `State`: [RuleStateType](./literals.md#rulestatetype)
- `Description`: `str`
- `RoleArn`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `EventBusName`: `str`

Returns a `Coroutine` for
[PutRuleResponseTypeDef](./type_defs.md#putruleresponsetypedef).

<a id="put\_targets"></a>

### put_targets

Adds the specified targets to the specified rule, or updates the targets if
they are already associated with the rule.

Type annotations for `session.create_client("events").put_targets` method.

Boto3 documentation:
[EventBridge.Client.put_targets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.put_targets)

Asynchronous method. Use `await put_targets(...)` for a synchronous call.

Arguments mapping described in
[PutTargetsRequestRequestTypeDef](./type_defs.md#puttargetsrequestrequesttypedef).

Keyword-only arguments:

- `Rule`: `str` *(required)*
- `Targets`: `Sequence`\[[TargetTypeDef](./type_defs.md#targettypedef)\]
  *(required)*
- `EventBusName`: `str`

Returns a `Coroutine` for
[PutTargetsResponseTypeDef](./type_defs.md#puttargetsresponsetypedef).

<a id="remove\_permission"></a>

### remove_permission

Revokes the permission of another Amazon Web Services account to be able to put
events to the specified event bus.

Type annotations for `session.create_client("events").remove_permission`
method.

Boto3 documentation:
[EventBridge.Client.remove_permission](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.remove_permission)

Asynchronous method. Use `await remove_permission(...)` for a synchronous call.

Arguments mapping described in
[RemovePermissionRequestRequestTypeDef](./type_defs.md#removepermissionrequestrequesttypedef).

Keyword-only arguments:

- `StatementId`: `str`
- `RemoveAllPermissions`: `bool`
- `EventBusName`: `str`

<a id="remove\_targets"></a>

### remove_targets

Removes the specified targets from the specified rule.

Type annotations for `session.create_client("events").remove_targets` method.

Boto3 documentation:
[EventBridge.Client.remove_targets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.remove_targets)

Asynchronous method. Use `await remove_targets(...)` for a synchronous call.

Arguments mapping described in
[RemoveTargetsRequestRequestTypeDef](./type_defs.md#removetargetsrequestrequesttypedef).

Keyword-only arguments:

- `Rule`: `str` *(required)*
- `Ids`: `Sequence`\[`str`\] *(required)*
- `EventBusName`: `str`
- `Force`: `bool`

Returns a `Coroutine` for
[RemoveTargetsResponseTypeDef](./type_defs.md#removetargetsresponsetypedef).

<a id="start\_replay"></a>

### start_replay

Starts the specified replay.

Type annotations for `session.create_client("events").start_replay` method.

Boto3 documentation:
[EventBridge.Client.start_replay](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.start_replay)

Asynchronous method. Use `await start_replay(...)` for a synchronous call.

Arguments mapping described in
[StartReplayRequestRequestTypeDef](./type_defs.md#startreplayrequestrequesttypedef).

Keyword-only arguments:

- `ReplayName`: `str` *(required)*
- `EventSourceArn`: `str` *(required)*
- `EventStartTime`: `Union`\[`datetime`, `str`\] *(required)*
- `EventEndTime`: `Union`\[`datetime`, `str`\] *(required)*
- `Destination`:
  [ReplayDestinationTypeDef](./type_defs.md#replaydestinationtypedef)
  *(required)*
- `Description`: `str`

Returns a `Coroutine` for
[StartReplayResponseTypeDef](./type_defs.md#startreplayresponsetypedef).

<a id="tag\_resource"></a>

### tag_resource

Assigns one or more tags (key-value pairs) to the specified EventBridge
resource.

Type annotations for `session.create_client("events").tag_resource` method.

Boto3 documentation:
[EventBridge.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceARN`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="test\_event\_pattern"></a>

### test_event_pattern

Tests whether the specified event pattern matches the provided event.

Type annotations for `session.create_client("events").test_event_pattern`
method.

Boto3 documentation:
[EventBridge.Client.test_event_pattern](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.test_event_pattern)

Asynchronous method. Use `await test_event_pattern(...)` for a synchronous
call.

Arguments mapping described in
[TestEventPatternRequestRequestTypeDef](./type_defs.md#testeventpatternrequestrequesttypedef).

Keyword-only arguments:

- `EventPattern`: `str` *(required)*
- `Event`: `str` *(required)*

Returns a `Coroutine` for
[TestEventPatternResponseTypeDef](./type_defs.md#testeventpatternresponsetypedef).

<a id="untag\_resource"></a>

### untag_resource

Removes one or more tags from the specified EventBridge resource.

Type annotations for `session.create_client("events").untag_resource` method.

Boto3 documentation:
[EventBridge.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceARN`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_api\_destination"></a>

### update_api_destination

Updates an API destination.

Type annotations for `session.create_client("events").update_api_destination`
method.

Boto3 documentation:
[EventBridge.Client.update_api_destination](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.update_api_destination)

Asynchronous method. Use `await update_api_destination(...)` for a synchronous
call.

Arguments mapping described in
[UpdateApiDestinationRequestRequestTypeDef](./type_defs.md#updateapidestinationrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `Description`: `str`
- `ConnectionArn`: `str`
- `InvocationEndpoint`: `str`
- `HttpMethod`:
  [ApiDestinationHttpMethodType](./literals.md#apidestinationhttpmethodtype)
- `InvocationRateLimitPerSecond`: `int`

Returns a `Coroutine` for
[UpdateApiDestinationResponseTypeDef](./type_defs.md#updateapidestinationresponsetypedef).

<a id="update\_archive"></a>

### update_archive

Updates the specified archive.

Type annotations for `session.create_client("events").update_archive` method.

Boto3 documentation:
[EventBridge.Client.update_archive](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.update_archive)

Asynchronous method. Use `await update_archive(...)` for a synchronous call.

Arguments mapping described in
[UpdateArchiveRequestRequestTypeDef](./type_defs.md#updatearchiverequestrequesttypedef).

Keyword-only arguments:

- `ArchiveName`: `str` *(required)*
- `Description`: `str`
- `EventPattern`: `str`
- `RetentionDays`: `int`

Returns a `Coroutine` for
[UpdateArchiveResponseTypeDef](./type_defs.md#updatearchiveresponsetypedef).

<a id="update\_connection"></a>

### update_connection

Updates settings for a connection.

Type annotations for `session.create_client("events").update_connection`
method.

Boto3 documentation:
[EventBridge.Client.update_connection](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.update_connection)

Asynchronous method. Use `await update_connection(...)` for a synchronous call.

Arguments mapping described in
[UpdateConnectionRequestRequestTypeDef](./type_defs.md#updateconnectionrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `Description`: `str`
- `AuthorizationType`:
  [ConnectionAuthorizationTypeType](./literals.md#connectionauthorizationtypetype)
- `AuthParameters`:
  [UpdateConnectionAuthRequestParametersTypeDef](./type_defs.md#updateconnectionauthrequestparameterstypedef)

Returns a `Coroutine` for
[UpdateConnectionResponseTypeDef](./type_defs.md#updateconnectionresponsetypedef).

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("events").__aenter__` method.

Boto3 documentation:
[EventBridge.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [EventBridgeClient](#eventbridgeclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("events").__aexit__` method.

Boto3 documentation:
[EventBridge.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("events").get_paginator` method
with overloads.

- `client.get_paginator("list_rule_names_by_target")` ->
  [ListRuleNamesByTargetPaginator](./paginators.md#listrulenamesbytargetpaginator)
- `client.get_paginator("list_rules")` ->
  [ListRulesPaginator](./paginators.md#listrulespaginator)
- `client.get_paginator("list_targets_by_rule")` ->
  [ListTargetsByRulePaginator](./paginators.md#listtargetsbyrulepaginator)
