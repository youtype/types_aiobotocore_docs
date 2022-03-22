<a id="migrationhubconfigclient-for-aiobotocore-migrationhubconfig-module"></a>

# MigrationHubConfigClient for aiobotocore MigrationHubConfig module

> [Index](../README.md) > [MigrationHubConfig](./README.md) >
> MigrationHubConfigClient

Auto-generated documentation for
[MigrationHubConfig](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
type annotations stubs module
[types-aiobotocore-migrationhub-config](https://pypi.org/project/types-aiobotocore-migrationhub-config/).

- [MigrationHubConfigClient for aiobotocore MigrationHubConfig module](#migrationhubconfigclient-for-aiobotocore-migrationhubconfig-module)
  - [MigrationHubConfigClient](#migrationhubconfigclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_home_region_control](#create_home_region_control)
    - [describe_home_region_controls](#describe_home_region_controls)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_home_region](#get_home_region)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)

<a id="migrationhubconfigclient"></a>

## MigrationHubConfigClient

Type annotations for `session.create_client("migrationhub-config")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_migrationhub_config.client import MigrationHubConfigClient

session = get_session()
async with session.create_client("migrationhub-config") as client:
    client: MigrationHubConfigClient
```

Boto3 documentation:
[MigrationHubConfig.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_migrationhub_config.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessDeniedException`
- `Exceptions.ClientError`
- `Exceptions.DryRunOperation`
- `Exceptions.InternalServerError`
- `Exceptions.InvalidInputException`
- `Exceptions.ServiceUnavailableException`
- `Exceptions.ThrottlingException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

MigrationHubConfigClient exceptions.

Type annotations for `session.create_client("migrationhub-config").exceptions`
method.

Boto3 documentation:
[MigrationHubConfig.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for
`session.create_client("migrationhub-config").can_paginate` method.

Boto3 documentation:
[MigrationHubConfig.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create\_home\_region\_control"></a>

### create_home_region_control

This API sets up the home region for the calling account only.

Type annotations for
`session.create_client("migrationhub-config").create_home_region_control`
method.

Boto3 documentation:
[MigrationHubConfig.Client.create_home_region_control](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig.Client.create_home_region_control)

Asynchronous method. Use `await create_home_region_control(...)` for a
synchronous call.

Arguments mapping described in
[CreateHomeRegionControlRequestRequestTypeDef](./type_defs.md#createhomeregioncontrolrequestrequesttypedef).

Keyword-only arguments:

- `HomeRegion`: `str` *(required)*
- `Target`: [TargetTypeDef](./type_defs.md#targettypedef) *(required)*
- `DryRun`: `bool`

Returns a `Coroutine` for
[CreateHomeRegionControlResultTypeDef](./type_defs.md#createhomeregioncontrolresulttypedef).

<a id="describe\_home\_region\_controls"></a>

### describe_home_region_controls

This API permits filtering on the `ControlId` and `HomeRegion` fields.

Type annotations for
`session.create_client("migrationhub-config").describe_home_region_controls`
method.

Boto3 documentation:
[MigrationHubConfig.Client.describe_home_region_controls](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig.Client.describe_home_region_controls)

Asynchronous method. Use `await describe_home_region_controls(...)` for a
synchronous call.

Arguments mapping described in
[DescribeHomeRegionControlsRequestRequestTypeDef](./type_defs.md#describehomeregioncontrolsrequestrequesttypedef).

Keyword-only arguments:

- `ControlId`: `str`
- `HomeRegion`: `str`
- `Target`: [TargetTypeDef](./type_defs.md#targettypedef)
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[DescribeHomeRegionControlsResultTypeDef](./type_defs.md#describehomeregioncontrolsresulttypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("migrationhub-config").generate_presigned_url` method.

Boto3 documentation:
[MigrationHubConfig.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get\_home\_region"></a>

### get_home_region

Returns the calling account’s home region, if configured.

Type annotations for
`session.create_client("migrationhub-config").get_home_region` method.

Boto3 documentation:
[MigrationHubConfig.Client.get_home_region](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig.Client.get_home_region)

Asynchronous method. Use `await get_home_region(...)` for a synchronous call.

Returns a `Coroutine` for
[GetHomeRegionResultTypeDef](./type_defs.md#gethomeregionresulttypedef).

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("migrationhub-config").__aenter__`
method.

Boto3 documentation:
[MigrationHubConfig.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for
[MigrationHubConfigClient](#migrationhubconfigclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("migrationhub-config").__aexit__`
method.

Boto3 documentation:
[MigrationHubConfig.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.
