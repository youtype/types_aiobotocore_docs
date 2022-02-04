<a id="migrationhubconfigclient-for-aiobotocore-migrationhubconfig-module"></a>

# MigrationHubConfigClient for aiobotocore MigrationHubConfig module

> [Index](..) > [MigrationHubConfig](.) > MigrationHubConfigClient

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

<a id="migrationhubconfigclient"></a>

## MigrationHubConfigClient

Type annotations for `aiobotocore.create_client("migrationhub-config")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_migrationhub_config.client import MigrationHubConfigClient

def get_migrationhub-config_client() -> MigrationHubConfigClient:
    return Session().client("migrationhub-config")
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

Type annotations for
`aiobotocore.create_client("migrationhub-config").exceptions` method.

Boto3 documentation:
[MigrationHubConfig.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for
`aiobotocore.create_client("migrationhub-config").can_paginate` method.

Boto3 documentation:
[MigrationHubConfig.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="create_home_region_control"></a>

### create_home_region_control

This API sets up the home region for the calling account only.

Type annotations for
`aiobotocore.create_client("migrationhub-config").create_home_region_control`
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

<a id="describe_home_region_controls"></a>

### describe_home_region_controls

This API permits filtering on the `ControlId` and `HomeRegion` fields.

Type annotations for
`aiobotocore.create_client("migrationhub-config").describe_home_region_controls`
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

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`aiobotocore.create_client("migrationhub-config").generate_presigned_url`
method.

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

<a id="get_home_region"></a>

### get_home_region

Returns the calling account’s home region, if configured.

Type annotations for
`aiobotocore.create_client("migrationhub-config").get_home_region` method.

Boto3 documentation:
[MigrationHubConfig.Client.get_home_region](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig.Client.get_home_region)

Asynchronous method. Use `await get_home_region(...)` for a synchronous call.

Returns a `Coroutine` for
[GetHomeRegionResultTypeDef](./type_defs.md#gethomeregionresulttypedef).
