<a id="piclient-for-aiobotocore-pi-module"></a>

# PIClient for aiobotocore PI module

> [Index](..) > [PI](.) > PIClient

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
    - [get_resource_metrics](#get_resource_metrics)

<a id="piclient"></a>

## PIClient

Type annotations for `aiobotocore.create_client("pi")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_pi.client import PIClient

def get_pi_client() -> PIClient:
    return Session().client("pi")
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

Type annotations for `aiobotocore.create_client("pi").exceptions` method.

Boto3 documentation:
[PI.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `aiobotocore.create_client("pi").can_paginate` method.

Boto3 documentation:
[PI.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="describe_dimension_keys"></a>

### describe_dimension_keys

For a specific time period, retrieve the top `N` dimension keys for a metric.

Type annotations for `aiobotocore.create_client("pi").describe_dimension_keys`
method.

Boto3 documentation:
[PI.Client.describe_dimension_keys](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.describe_dimension_keys)

Asynchronous method. Use `await describe_dimension_keys(...)` for a synchronous
call.

Arguments mapping described in
[DescribeDimensionKeysRequestRequestTypeDef](./type_defs.md#describedimensionkeysrequestrequesttypedef).

Keyword-only arguments:

- `ServiceType`: `Literal['RDS']` (see
  [ServiceTypeType](./literals.md#servicetypetype)) *(required)*
- `Identifier`: `str` *(required)*
- `StartTime`: `Union`\[`datetime`, `str`\] *(required)*
- `EndTime`: `Union`\[`datetime`, `str`\] *(required)*
- `Metric`: `str` *(required)*
- `GroupBy`: [DimensionGroupTypeDef](./type_defs.md#dimensiongrouptypedef)
  *(required)*
- `PeriodInSeconds`: `int`
- `PartitionBy`: [DimensionGroupTypeDef](./type_defs.md#dimensiongrouptypedef)
- `Filter`: `Mapping`\[`str`, `str`\]
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[DescribeDimensionKeysResponseTypeDef](./type_defs.md#describedimensionkeysresponsetypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `aiobotocore.create_client("pi").generate_presigned_url`
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

<a id="get_dimension_key_details"></a>

### get_dimension_key_details

Get the attributes of the specified dimension group for a DB instance or data
source.

Type annotations for
`aiobotocore.create_client("pi").get_dimension_key_details` method.

Boto3 documentation:
[PI.Client.get_dimension_key_details](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.get_dimension_key_details)

Asynchronous method. Use `await get_dimension_key_details(...)` for a
synchronous call.

Arguments mapping described in
[GetDimensionKeyDetailsRequestRequestTypeDef](./type_defs.md#getdimensionkeydetailsrequestrequesttypedef).

Keyword-only arguments:

- `ServiceType`: `Literal['RDS']` (see
  [ServiceTypeType](./literals.md#servicetypetype)) *(required)*
- `Identifier`: `str` *(required)*
- `Group`: `str` *(required)*
- `GroupIdentifier`: `str` *(required)*
- `RequestedDimensions`: `Sequence`\[`str`\]

Returns a `Coroutine` for
[GetDimensionKeyDetailsResponseTypeDef](./type_defs.md#getdimensionkeydetailsresponsetypedef).

<a id="get_resource_metrics"></a>

### get_resource_metrics

Retrieve Performance Insights metrics for a set of data sources, over a time
period.

Type annotations for `aiobotocore.create_client("pi").get_resource_metrics`
method.

Boto3 documentation:
[PI.Client.get_resource_metrics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client.get_resource_metrics)

Asynchronous method. Use `await get_resource_metrics(...)` for a synchronous
call.

Arguments mapping described in
[GetResourceMetricsRequestRequestTypeDef](./type_defs.md#getresourcemetricsrequestrequesttypedef).

Keyword-only arguments:

- `ServiceType`: `Literal['RDS']` (see
  [ServiceTypeType](./literals.md#servicetypetype)) *(required)*
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
