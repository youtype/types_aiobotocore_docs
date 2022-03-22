<a id="piclient-for-aiobotocore-pi-module"></a>

# PIClient for aiobotocore PI module

> [Index](../README.md) > [PI](./README.md) > PIClient

Auto-generated documentation for
[PI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
type annotations stubs module
[types-aiobotocore-pi](https://pypi.org/project/types-aiobotocore-pi/).

- [PIClient for aiobotocore PI module](#piclient-for-aiobotocore-pi-module)
  - [PIClient](#piclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [describe_dimension_keys](#describe_dimension_keys)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_dimension_key_details](#get_dimension_key_details)
    - [get_resource_metadata](#get_resource_metadata)
    - [get_resource_metrics](#get_resource_metrics)
    - [list_available_resource_dimensions](#list_available_resource_dimensions)
    - [list_available_resource_metrics](#list_available_resource_metrics)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)

<a id="piclient"></a>

## PIClient

Type annotations for `session.create_client("pi")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_pi.client import PIClient

session = get_session()
async with session.create_client("pi") as client:
    client: PIClient
```

Boto3 documentation:
[PI.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_pi.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.InternalServiceError`
- `Exceptions.InvalidArgumentException`
- `Exceptions.NotAuthorizedException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

PIClient exceptions.

Type annotations for `session.create_client("pi").exceptions` method.

Boto3 documentation:
[PI.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("pi").can_paginate` method.

Boto3 documentation:
[PI.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="describe\_dimension\_keys"></a>

### describe_dimension_keys

For a specific time period, retrieve the top `N` dimension keys for a metric.

Type annotations for `session.create_client("pi").describe_dimension_keys`
method.

Boto3 documentation:
[PI.Client.describe_dimension_keys](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.describe_dimension_keys)

Asynchronous method. Use `await describe_dimension_keys(...)` for a synchronous
call.

Arguments mapping described in
[DescribeDimensionKeysRequestRequestTypeDef](./type_defs.md#describedimensionkeysrequestrequesttypedef).

Keyword-only arguments:

- `ServiceType`: [ServiceTypeType](./literals.md#servicetypetype) *(required)*
- `Identifier`: `str` *(required)*
- `StartTime`: `Union`\[`datetime`, `str`\] *(required)*
- `EndTime`: `Union`\[`datetime`, `str`\] *(required)*
- `Metric`: `str` *(required)*
- `GroupBy`: [DimensionGroupTypeDef](./type_defs.md#dimensiongrouptypedef)
  *(required)*
- `PeriodInSeconds`: `int`
- `AdditionalMetrics`: `Sequence`\[`str`\]
- `PartitionBy`: [DimensionGroupTypeDef](./type_defs.md#dimensiongrouptypedef)
- `Filter`: `Mapping`\[`str`, `str`\]
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[DescribeDimensionKeysResponseTypeDef](./type_defs.md#describedimensionkeysresponsetypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("pi").generate_presigned_url`
method.

Boto3 documentation:
[PI.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get\_dimension\_key\_details"></a>

### get_dimension_key_details

Get the attributes of the specified dimension group for a DB instance or data
source.

Type annotations for `session.create_client("pi").get_dimension_key_details`
method.

Boto3 documentation:
[PI.Client.get_dimension_key_details](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.get_dimension_key_details)

Asynchronous method. Use `await get_dimension_key_details(...)` for a
synchronous call.

Arguments mapping described in
[GetDimensionKeyDetailsRequestRequestTypeDef](./type_defs.md#getdimensionkeydetailsrequestrequesttypedef).

Keyword-only arguments:

- `ServiceType`: [ServiceTypeType](./literals.md#servicetypetype) *(required)*
- `Identifier`: `str` *(required)*
- `Group`: `str` *(required)*
- `GroupIdentifier`: `str` *(required)*
- `RequestedDimensions`: `Sequence`\[`str`\]

Returns a `Coroutine` for
[GetDimensionKeyDetailsResponseTypeDef](./type_defs.md#getdimensionkeydetailsresponsetypedef).

<a id="get\_resource\_metadata"></a>

### get_resource_metadata

Retrieve the metadata for different features.

Type annotations for `session.create_client("pi").get_resource_metadata`
method.

Boto3 documentation:
[PI.Client.get_resource_metadata](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.get_resource_metadata)

Asynchronous method. Use `await get_resource_metadata(...)` for a synchronous
call.

Arguments mapping described in
[GetResourceMetadataRequestRequestTypeDef](./type_defs.md#getresourcemetadatarequestrequesttypedef).

Keyword-only arguments:

- `ServiceType`: [ServiceTypeType](./literals.md#servicetypetype) *(required)*
- `Identifier`: `str` *(required)*

Returns a `Coroutine` for
[GetResourceMetadataResponseTypeDef](./type_defs.md#getresourcemetadataresponsetypedef).

<a id="get\_resource\_metrics"></a>

### get_resource_metrics

Retrieve Performance Insights metrics for a set of data sources, over a time
period.

Type annotations for `session.create_client("pi").get_resource_metrics` method.

Boto3 documentation:
[PI.Client.get_resource_metrics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.get_resource_metrics)

Asynchronous method. Use `await get_resource_metrics(...)` for a synchronous
call.

Arguments mapping described in
[GetResourceMetricsRequestRequestTypeDef](./type_defs.md#getresourcemetricsrequestrequesttypedef).

Keyword-only arguments:

- `ServiceType`: [ServiceTypeType](./literals.md#servicetypetype) *(required)*
- `Identifier`: `str` *(required)*
- `MetricQueries`:
  `Sequence`\[[MetricQueryTypeDef](./type_defs.md#metricquerytypedef)\]
  *(required)*
- `StartTime`: `Union`\[`datetime`, `str`\] *(required)*
- `EndTime`: `Union`\[`datetime`, `str`\] *(required)*
- `PeriodInSeconds`: `int`
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[GetResourceMetricsResponseTypeDef](./type_defs.md#getresourcemetricsresponsetypedef).

<a id="list\_available\_resource\_dimensions"></a>

### list_available_resource_dimensions

Retrieve the dimensions that can be queried for each specified metric type on a
specified DB instance.

Type annotations for
`session.create_client("pi").list_available_resource_dimensions` method.

Boto3 documentation:
[PI.Client.list_available_resource_dimensions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.list_available_resource_dimensions)

Asynchronous method. Use `await list_available_resource_dimensions(...)` for a
synchronous call.

Arguments mapping described in
[ListAvailableResourceDimensionsRequestRequestTypeDef](./type_defs.md#listavailableresourcedimensionsrequestrequesttypedef).

Keyword-only arguments:

- `ServiceType`: [ServiceTypeType](./literals.md#servicetypetype) *(required)*
- `Identifier`: `str` *(required)*
- `Metrics`: `Sequence`\[`str`\] *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListAvailableResourceDimensionsResponseTypeDef](./type_defs.md#listavailableresourcedimensionsresponsetypedef).

<a id="list\_available\_resource\_metrics"></a>

### list_available_resource_metrics

Retrieve metrics of the specified types that can be queried for a specified DB
instance.

Type annotations for
`session.create_client("pi").list_available_resource_metrics` method.

Boto3 documentation:
[PI.Client.list_available_resource_metrics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.list_available_resource_metrics)

Asynchronous method. Use `await list_available_resource_metrics(...)` for a
synchronous call.

Arguments mapping described in
[ListAvailableResourceMetricsRequestRequestTypeDef](./type_defs.md#listavailableresourcemetricsrequestrequesttypedef).

Keyword-only arguments:

- `ServiceType`: [ServiceTypeType](./literals.md#servicetypetype) *(required)*
- `Identifier`: `str` *(required)*
- `MetricTypes`: `Sequence`\[`str`\] *(required)*
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListAvailableResourceMetricsResponseTypeDef](./type_defs.md#listavailableresourcemetricsresponsetypedef).

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("pi").__aenter__` method.

Boto3 documentation:
[PI.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [PIClient](#piclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("pi").__aexit__` method.

Boto3 documentation:
[PI.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.
