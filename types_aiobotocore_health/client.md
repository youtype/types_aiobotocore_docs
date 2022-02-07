<a id="healthclient-for-aiobotocore-health-module"></a>

# HealthClient for aiobotocore Health module

> [Index](..) > [Health](.) > HealthClient

Auto-generated documentation for
[Health](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health)
type annotations stubs module
[types-aiobotocore-health](https://pypi.org/project/types-aiobotocore-health/).

- [HealthClient for aiobotocore Health module](#healthclient-for-aiobotocore-health-module)
  - [HealthClient](#healthclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [describe_affected_accounts_for_organization](#describe_affected_accounts_for_organization)
    - [describe_affected_entities](#describe_affected_entities)
    - [describe_affected_entities_for_organization](#describe_affected_entities_for_organization)
    - [describe_entity_aggregates](#describe_entity_aggregates)
    - [describe_event_aggregates](#describe_event_aggregates)
    - [describe_event_details](#describe_event_details)
    - [describe_event_details_for_organization](#describe_event_details_for_organization)
    - [describe_event_types](#describe_event_types)
    - [describe_events](#describe_events)
    - [describe_events_for_organization](#describe_events_for_organization)
    - [describe_health_service_status_for_organization](#describe_health_service_status_for_organization)
    - [disable_health_service_access_for_organization](#disable_health_service_access_for_organization)
    - [enable_health_service_access_for_organization](#enable_health_service_access_for_organization)
    - [generate_presigned_url](#generate_presigned_url)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="healthclient"></a>

## HealthClient

Type annotations for `session.create_client("health")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_health.client import HealthClient

session = get_session()
async with session.create_client("health") as client:
    client: HealthClient
```

Boto3 documentation:
[Health.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_health.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.ConcurrentModificationException`
- `Exceptions.InvalidPaginationToken`
- `Exceptions.UnsupportedLocale`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

HealthClient exceptions.

Type annotations for `session.create_client("health").exceptions` method.

Boto3 documentation:
[Health.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("health").can_paginate` method.

Boto3 documentation:
[Health.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="describe_affected_accounts_for_organization"></a>

### describe_affected_accounts_for_organization

Returns a list of accounts in the organization from Organizations that are
affected by the provided event.

Type annotations for
`session.create_client("health").describe_affected_accounts_for_organization`
method.

Boto3 documentation:
[Health.Client.describe_affected_accounts_for_organization](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.describe_affected_accounts_for_organization)

Asynchronous method. Use
`await describe_affected_accounts_for_organization(...)` for a synchronous
call.

Arguments mapping described in
[DescribeAffectedAccountsForOrganizationRequestRequestTypeDef](./type_defs.md#describeaffectedaccountsfororganizationrequestrequesttypedef).

Keyword-only arguments:

- `eventArn`: `str` *(required)*
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[DescribeAffectedAccountsForOrganizationResponseTypeDef](./type_defs.md#describeaffectedaccountsfororganizationresponsetypedef).

<a id="describe_affected_entities"></a>

### describe_affected_entities

Returns a list of entities that have been affected by the specified events,
based on the specified filter criteria.

Type annotations for
`session.create_client("health").describe_affected_entities` method.

Boto3 documentation:
[Health.Client.describe_affected_entities](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.describe_affected_entities)

Asynchronous method. Use `await describe_affected_entities(...)` for a
synchronous call.

Arguments mapping described in
[DescribeAffectedEntitiesRequestRequestTypeDef](./type_defs.md#describeaffectedentitiesrequestrequesttypedef).

Keyword-only arguments:

- `filter`: [EntityFilterTypeDef](./type_defs.md#entityfiltertypedef)
  *(required)*
- `locale`: `str`
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[DescribeAffectedEntitiesResponseTypeDef](./type_defs.md#describeaffectedentitiesresponsetypedef).

<a id="describe_affected_entities_for_organization"></a>

### describe_affected_entities_for_organization

Returns a list of entities that have been affected by one or more events for
one or more accounts in your organization in Organizations, based on the filter
criteria.

Type annotations for
`session.create_client("health").describe_affected_entities_for_organization`
method.

Boto3 documentation:
[Health.Client.describe_affected_entities_for_organization](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.describe_affected_entities_for_organization)

Asynchronous method. Use
`await describe_affected_entities_for_organization(...)` for a synchronous
call.

Arguments mapping described in
[DescribeAffectedEntitiesForOrganizationRequestRequestTypeDef](./type_defs.md#describeaffectedentitiesfororganizationrequestrequesttypedef).

Keyword-only arguments:

- `organizationEntityFilters`:
  `Sequence`\[[EventAccountFilterTypeDef](./type_defs.md#eventaccountfiltertypedef)\]
  *(required)*
- `locale`: `str`
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[DescribeAffectedEntitiesForOrganizationResponseTypeDef](./type_defs.md#describeaffectedentitiesfororganizationresponsetypedef).

<a id="describe_entity_aggregates"></a>

### describe_entity_aggregates

Returns the number of entities that are affected by each of the specified
events.

Type annotations for
`session.create_client("health").describe_entity_aggregates` method.

Boto3 documentation:
[Health.Client.describe_entity_aggregates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.describe_entity_aggregates)

Asynchronous method. Use `await describe_entity_aggregates(...)` for a
synchronous call.

Arguments mapping described in
[DescribeEntityAggregatesRequestRequestTypeDef](./type_defs.md#describeentityaggregatesrequestrequesttypedef).

Keyword-only arguments:

- `eventArns`: `Sequence`\[`str`\]

Returns a `Coroutine` for
[DescribeEntityAggregatesResponseTypeDef](./type_defs.md#describeentityaggregatesresponsetypedef).

<a id="describe_event_aggregates"></a>

### describe_event_aggregates

Returns the number of events of each event type (issue, scheduled change, and
account notification).

Type annotations for
`session.create_client("health").describe_event_aggregates` method.

Boto3 documentation:
[Health.Client.describe_event_aggregates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.describe_event_aggregates)

Asynchronous method. Use `await describe_event_aggregates(...)` for a
synchronous call.

Arguments mapping described in
[DescribeEventAggregatesRequestRequestTypeDef](./type_defs.md#describeeventaggregatesrequestrequesttypedef).

Keyword-only arguments:

- `aggregateField`: `Literal['eventTypeCategory']` (see
  [eventAggregateFieldType](./literals.md#eventaggregatefieldtype))
  *(required)*
- `filter`: [EventFilterTypeDef](./type_defs.md#eventfiltertypedef)
- `maxResults`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[DescribeEventAggregatesResponseTypeDef](./type_defs.md#describeeventaggregatesresponsetypedef).

<a id="describe_event_details"></a>

### describe_event_details

Returns detailed information about one or more specified events.

Type annotations for `session.create_client("health").describe_event_details`
method.

Boto3 documentation:
[Health.Client.describe_event_details](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.describe_event_details)

Asynchronous method. Use `await describe_event_details(...)` for a synchronous
call.

Arguments mapping described in
[DescribeEventDetailsRequestRequestTypeDef](./type_defs.md#describeeventdetailsrequestrequesttypedef).

Keyword-only arguments:

- `eventArns`: `Sequence`\[`str`\] *(required)*
- `locale`: `str`

Returns a `Coroutine` for
[DescribeEventDetailsResponseTypeDef](./type_defs.md#describeeventdetailsresponsetypedef).

<a id="describe_event_details_for_organization"></a>

### describe_event_details_for_organization

Returns detailed information about one or more specified events for one or more
Amazon Web Services accounts in your organization.

Type annotations for
`session.create_client("health").describe_event_details_for_organization`
method.

Boto3 documentation:
[Health.Client.describe_event_details_for_organization](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.describe_event_details_for_organization)

Asynchronous method. Use `await describe_event_details_for_organization(...)`
for a synchronous call.

Arguments mapping described in
[DescribeEventDetailsForOrganizationRequestRequestTypeDef](./type_defs.md#describeeventdetailsfororganizationrequestrequesttypedef).

Keyword-only arguments:

- `organizationEventDetailFilters`:
  `Sequence`\[[EventAccountFilterTypeDef](./type_defs.md#eventaccountfiltertypedef)\]
  *(required)*
- `locale`: `str`

Returns a `Coroutine` for
[DescribeEventDetailsForOrganizationResponseTypeDef](./type_defs.md#describeeventdetailsfororganizationresponsetypedef).

<a id="describe_event_types"></a>

### describe_event_types

Returns the event types that meet the specified filter criteria.

Type annotations for `session.create_client("health").describe_event_types`
method.

Boto3 documentation:
[Health.Client.describe_event_types](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.describe_event_types)

Asynchronous method. Use `await describe_event_types(...)` for a synchronous
call.

Arguments mapping described in
[DescribeEventTypesRequestRequestTypeDef](./type_defs.md#describeeventtypesrequestrequesttypedef).

Keyword-only arguments:

- `filter`: [EventTypeFilterTypeDef](./type_defs.md#eventtypefiltertypedef)
- `locale`: `str`
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[DescribeEventTypesResponseTypeDef](./type_defs.md#describeeventtypesresponsetypedef).

<a id="describe_events"></a>

### describe_events

Returns information about events that meet the specified filter criteria.

Type annotations for `session.create_client("health").describe_events` method.

Boto3 documentation:
[Health.Client.describe_events](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.describe_events)

Asynchronous method. Use `await describe_events(...)` for a synchronous call.

Arguments mapping described in
[DescribeEventsRequestRequestTypeDef](./type_defs.md#describeeventsrequestrequesttypedef).

Keyword-only arguments:

- `filter`: [EventFilterTypeDef](./type_defs.md#eventfiltertypedef)
- `nextToken`: `str`
- `maxResults`: `int`
- `locale`: `str`

Returns a `Coroutine` for
[DescribeEventsResponseTypeDef](./type_defs.md#describeeventsresponsetypedef).

<a id="describe_events_for_organization"></a>

### describe_events_for_organization

Returns information about events across your organization in Organizations.

Type annotations for
`session.create_client("health").describe_events_for_organization` method.

Boto3 documentation:
[Health.Client.describe_events_for_organization](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.describe_events_for_organization)

Asynchronous method. Use `await describe_events_for_organization(...)` for a
synchronous call.

Arguments mapping described in
[DescribeEventsForOrganizationRequestRequestTypeDef](./type_defs.md#describeeventsfororganizationrequestrequesttypedef).

Keyword-only arguments:

- `filter`:
  [OrganizationEventFilterTypeDef](./type_defs.md#organizationeventfiltertypedef)
- `nextToken`: `str`
- `maxResults`: `int`
- `locale`: `str`

Returns a `Coroutine` for
[DescribeEventsForOrganizationResponseTypeDef](./type_defs.md#describeeventsfororganizationresponsetypedef).

<a id="describe_health_service_status_for_organization"></a>

### describe_health_service_status_for_organization

This operation provides status information on enabling or disabling Health to
work with your organization.

Type annotations for
`session.create_client("health").describe_health_service_status_for_organization`
method.

Boto3 documentation:
[Health.Client.describe_health_service_status_for_organization](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.describe_health_service_status_for_organization)

Asynchronous method. Use
`await describe_health_service_status_for_organization(...)` for a synchronous
call.

Returns a `Coroutine` for
[DescribeHealthServiceStatusForOrganizationResponseTypeDef](./type_defs.md#describehealthservicestatusfororganizationresponsetypedef).

<a id="disable_health_service_access_for_organization"></a>

### disable_health_service_access_for_organization

Disables Health from working with Organizations.

Type annotations for
`session.create_client("health").disable_health_service_access_for_organization`
method.

Boto3 documentation:
[Health.Client.disable_health_service_access_for_organization](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.disable_health_service_access_for_organization)

Asynchronous method. Use
`await disable_health_service_access_for_organization(...)` for a synchronous
call.

<a id="enable_health_service_access_for_organization"></a>

### enable_health_service_access_for_organization

Enables Health to work with Organizations.

Type annotations for
`session.create_client("health").enable_health_service_access_for_organization`
method.

Boto3 documentation:
[Health.Client.enable_health_service_access_for_organization](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.enable_health_service_access_for_organization)

Asynchronous method. Use
`await enable_health_service_access_for_organization(...)` for a synchronous
call.

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("health").generate_presigned_url`
method.

Boto3 documentation:
[Health.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("health").__aenter__` method.

Boto3 documentation:
[Health.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [HealthClient](#healthclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("health").__aexit__` method.

Boto3 documentation:
[Health.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#Health.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("health").get_paginator` method
with overloads.

- `client.get_paginator("describe_affected_accounts_for_organization")` ->
  [DescribeAffectedAccountsForOrganizationPaginator](./paginators.md#describeaffectedaccountsfororganizationpaginator)
- `client.get_paginator("describe_affected_entities")` ->
  [DescribeAffectedEntitiesPaginator](./paginators.md#describeaffectedentitiespaginator)
- `client.get_paginator("describe_affected_entities_for_organization")` ->
  [DescribeAffectedEntitiesForOrganizationPaginator](./paginators.md#describeaffectedentitiesfororganizationpaginator)
- `client.get_paginator("describe_event_aggregates")` ->
  [DescribeEventAggregatesPaginator](./paginators.md#describeeventaggregatespaginator)
- `client.get_paginator("describe_event_types")` ->
  [DescribeEventTypesPaginator](./paginators.md#describeeventtypespaginator)
- `client.get_paginator("describe_events")` ->
  [DescribeEventsPaginator](./paginators.md#describeeventspaginator)
- `client.get_paginator("describe_events_for_organization")` ->
  [DescribeEventsForOrganizationPaginator](./paginators.md#describeeventsfororganizationpaginator)
