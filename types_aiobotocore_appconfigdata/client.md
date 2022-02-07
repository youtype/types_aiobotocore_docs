<a id="appconfigdataclient-for-aiobotocore-appconfigdata-module"></a>

# AppConfigDataClient for aiobotocore AppConfigData module

> [Index](..) > [AppConfigData](.) > AppConfigDataClient

Auto-generated documentation for
[AppConfigData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData)
type annotations stubs module
[types-aiobotocore-appconfigdata](https://pypi.org/project/types-aiobotocore-appconfigdata/).

- [AppConfigDataClient for aiobotocore AppConfigData module](#appconfigdataclient-for-aiobotocore-appconfigdata-module)
  - [AppConfigDataClient](#appconfigdataclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_latest_configuration](#get_latest_configuration)
    - [start_configuration_session](#start_configuration_session)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)

<a id="appconfigdataclient"></a>

## AppConfigDataClient

Type annotations for `session.create_client("appconfigdata")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_appconfigdata.client import AppConfigDataClient

session = get_session()
async with session.create_client("appconfigdata") as client:
    client: AppConfigDataClient
```

Boto3 documentation:
[AppConfigData.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_appconfigdata.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```

Exceptions:

- `Exceptions.BadRequestException`
- `Exceptions.ClientError`
- `Exceptions.InternalServerException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ThrottlingException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

AppConfigDataClient exceptions.

Type annotations for `session.create_client("appconfigdata").exceptions`
method.

Boto3 documentation:
[AppConfigData.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("appconfigdata").can_paginate`
method.

Boto3 documentation:
[AppConfigData.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("appconfigdata").generate_presigned_url` method.

Boto3 documentation:
[AppConfigData.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_latest_configuration"></a>

### get_latest_configuration

Retrieves the latest deployed configuration.

Type annotations for
`session.create_client("appconfigdata").get_latest_configuration` method.

Boto3 documentation:
[AppConfigData.Client.get_latest_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData.Client.get_latest_configuration)

Asynchronous method. Use `await get_latest_configuration(...)` for a
synchronous call.

Arguments mapping described in
[GetLatestConfigurationRequestRequestTypeDef](./type_defs.md#getlatestconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `ConfigurationToken`: `str` *(required)*

Returns a `Coroutine` for
[GetLatestConfigurationResponseTypeDef](./type_defs.md#getlatestconfigurationresponsetypedef).

<a id="start_configuration_session"></a>

### start_configuration_session

Starts a configuration session used to retrieve a deployed configuration.

Type annotations for
`session.create_client("appconfigdata").start_configuration_session` method.

Boto3 documentation:
[AppConfigData.Client.start_configuration_session](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData.Client.start_configuration_session)

Asynchronous method. Use `await start_configuration_session(...)` for a
synchronous call.

Arguments mapping described in
[StartConfigurationSessionRequestRequestTypeDef](./type_defs.md#startconfigurationsessionrequestrequesttypedef).

Keyword-only arguments:

- `ApplicationIdentifier`: `str` *(required)*
- `ConfigurationProfileIdentifier`: `str` *(required)*
- `EnvironmentIdentifier`: `str` *(required)*
- `RequiredMinimumPollIntervalInSeconds`: `int`

Returns a `Coroutine` for
[StartConfigurationSessionResponseTypeDef](./type_defs.md#startconfigurationsessionresponsetypedef).

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("appconfigdata").__aenter__`
method.

Boto3 documentation:
[AppConfigData.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [AppConfigDataClient](#appconfigdataclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("appconfigdata").__aexit__` method.

Boto3 documentation:
[AppConfigData.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.
