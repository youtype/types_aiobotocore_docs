# ForecastQueryServiceClient

> [Index](../README.md) > [ForecastQueryService](./README.md) > ForecastQueryServiceClient

!!! note ""

    Auto-generated documentation for [ForecastQueryService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService)
    type annotations stubs module [types-aiobotocore-forecastquery](https://pypi.org/project/types-aiobotocore-forecastquery/).

## ForecastQueryServiceClient

Type annotations and code completion for `#!python session.create_client("forecastquery")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService.Client)

```python title="Usage example"
from aiobotocore.session import get_session
from types_aiobotocore_forecastquery.client import ForecastQueryServiceClient

session = get_session()
async with session.create_client("forecastquery") as client:
    client: ForecastQueryServiceClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("forecastquery").exceptions` structure.

```python title="Usage example"
async with session.create_client("forecastquery") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.InvalidInputException,
        client.InvalidNextTokenException,
        client.LimitExceededException,
        client.ResourceInUseException,
        client.ResourceNotFoundException,
    ) as e:
        print(e)
```

```python title="Type checking example"
from types_aiobotocore_forecastquery.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("forecastquery").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService.Client.can_paginate)

```python title="Method definition"
def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("forecastquery").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService.Client.close)

```python title="Method definition"
await def close(
    self,
) -> None:
    ...
```


### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("forecastquery").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService.Client.generate_presigned_url)

```python title="Method definition"
await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### query\_forecast

Retrieves a forecast for a single item, filtered by the supplied criteria.

Type annotations and code completion for `#!python session.create_client("forecastquery").query_forecast` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService.Client.query_forecast)

```python title="Method definition"
await def query_forecast(
    self,
    *,
    ForecastArn: str,
    Filters: Mapping[str, str],
    StartDate: str = ...,
    EndDate: str = ...,
    NextToken: str = ...,
) -> QueryForecastResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: QueryForecastResponseTypeDef](./type_defs.md#queryforecastresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: QueryForecastRequestRequestTypeDef = {  # (1)
    "ForecastArn": ...,
    "Filters": ...,
}

parent.query_forecast(**kwargs)
```

1. See [:material-code-braces: QueryForecastRequestRequestTypeDef](./type_defs.md#queryforecastrequestrequesttypedef) 

### query\_what\_if\_forecast

Retrieves a what-if forecast.

Type annotations and code completion for `#!python session.create_client("forecastquery").query_what_if_forecast` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService.Client.query_what_if_forecast)

```python title="Method definition"
await def query_what_if_forecast(
    self,
    *,
    WhatIfForecastArn: str,
    Filters: Mapping[str, str],
    StartDate: str = ...,
    EndDate: str = ...,
    NextToken: str = ...,
) -> QueryWhatIfForecastResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: QueryWhatIfForecastResponseTypeDef](./type_defs.md#querywhatifforecastresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: QueryWhatIfForecastRequestRequestTypeDef = {  # (1)
    "WhatIfForecastArn": ...,
    "Filters": ...,
}

parent.query_what_if_forecast(**kwargs)
```

1. See [:material-code-braces: QueryWhatIfForecastRequestRequestTypeDef](./type_defs.md#querywhatifforecastrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("forecastquery").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService.Client.__aenter__)

```python title="Method definition"
await def __aenter__(
    self,
) -> ForecastQueryServiceClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("forecastquery").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService.Client.__aexit__)

```python title="Method definition"
await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```





