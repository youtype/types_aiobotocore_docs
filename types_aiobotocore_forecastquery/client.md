<a id="forecastqueryserviceclient-for-aiobotocore-forecastqueryservice-module"></a>

# ForecastQueryServiceClient for aiobotocore ForecastQueryService module

> [Index](..) > [ForecastQueryService](.) > ForecastQueryServiceClient

Auto-generated documentation for
[ForecastQueryService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService)
type annotations stubs module
[types-aiobotocore-forecastquery](https://pypi.org/project/types-aiobotocore-forecastquery/).

- [ForecastQueryServiceClient for aiobotocore ForecastQueryService module](#forecastqueryserviceclient-for-aiobotocore-forecastqueryservice-module)
  - [ForecastQueryServiceClient](#forecastqueryserviceclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [generate_presigned_url](#generate_presigned_url)
    - [query_forecast](#query_forecast)

<a id="forecastqueryserviceclient"></a>

## ForecastQueryServiceClient

Type annotations for `aiobotocore.create_client("forecastquery")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_forecastquery.client import ForecastQueryServiceClient

def get_forecastquery_client() -> ForecastQueryServiceClient:
    return Session().client("forecastquery")
```

Boto3 documentation:
[ForecastQueryService.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_forecastquery.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.InvalidInputException`
- `Exceptions.InvalidNextTokenException`
- `Exceptions.LimitExceededException`
- `Exceptions.ResourceInUseException`
- `Exceptions.ResourceNotFoundException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

ForecastQueryServiceClient exceptions.

Type annotations for `aiobotocore.create_client("forecastquery").exceptions`
method.

Boto3 documentation:
[ForecastQueryService.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `aiobotocore.create_client("forecastquery").can_paginate`
method.

Boto3 documentation:
[ForecastQueryService.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`aiobotocore.create_client("forecastquery").generate_presigned_url` method.

Boto3 documentation:
[ForecastQueryService.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="query_forecast"></a>

### query_forecast

Retrieves a forecast for a single item, filtered by the supplied criteria.

Type annotations for
`aiobotocore.create_client("forecastquery").query_forecast` method.

Boto3 documentation:
[ForecastQueryService.Client.query_forecast](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService.Client.query_forecast)

Asynchronous method. Use `await query_forecast(...)` for a synchronous call.

Arguments mapping described in
[QueryForecastRequestRequestTypeDef](./type_defs.md#queryforecastrequestrequesttypedef).

Keyword-only arguments:

- `ForecastArn`: `str` *(required)*
- `Filters`: `Mapping`\[`str`, `str`\] *(required)*
- `StartDate`: `str`
- `EndDate`: `str`
- `NextToken`: `str`

Returns a `Coroutine` for
[QueryForecastResponseTypeDef](./type_defs.md#queryforecastresponsetypedef).
