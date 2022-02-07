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
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)

<a id="forecastqueryserviceclient"></a>

## ForecastQueryServiceClient

Type annotations for `session.create_client("forecastquery")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_forecastquery.client import ForecastQueryServiceClient

session = get_session()
async with session.create_client("forecastquery") as client:
    client: ForecastQueryServiceClient
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

Type annotations for `session.create_client("forecastquery").exceptions`
method.

Boto3 documentation:
[ForecastQueryService.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("forecastquery").can_paginate`
method.

Boto3 documentation:
[ForecastQueryService.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("forecastquery").generate_presigned_url` method.

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

Type annotations for `session.create_client("forecastquery").query_forecast`
method.

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

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("forecastquery").__aenter__`
method.

Boto3 documentation:
[ForecastQueryService.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for
[ForecastQueryServiceClient](#forecastqueryserviceclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("forecastquery").__aexit__` method.

Boto3 documentation:
[ForecastQueryService.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.
