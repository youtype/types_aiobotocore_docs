# MigrationHubConfigClient

> [Index](../README.md) > [MigrationHubConfig](./README.md) > MigrationHubConfigClient

!!! note ""

    Auto-generated documentation for [MigrationHubConfig](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig)
    type annotations stubs module [types-aiobotocore-migrationhub-config](https://pypi.org/project/types-aiobotocore-migrationhub-config/).

## MigrationHubConfigClient

Type annotations and code completion for `#!python session.create_client("migrationhub-config")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig.Client)

```python title="Usage example"
from aiobotocore.session import get_session
from types_aiobotocore_migrationhub_config.client import MigrationHubConfigClient

session = get_session()
async with session.create_client("migrationhub-config") as client:
    client: MigrationHubConfigClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("migrationhub-config").exceptions` structure.

```python title="Usage example"
async with session.create_client("migrationhub-config") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.DryRunOperation,
        client.InternalServerError,
        client.InvalidInputException,
        client.ServiceUnavailableException,
        client.ThrottlingException,
    ) as e:
        print(e)
```

```python title="Type checking example"
from types_aiobotocore_migrationhub_config.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("migrationhub-config").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig.Client.can_paginate)

```python title="Method definition"
def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### create\_home\_region\_control

This API sets up the home region for the calling account only.

Type annotations and code completion for `#!python session.create_client("migrationhub-config").create_home_region_control` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig.Client.create_home_region_control)

```python title="Method definition"
await def create_home_region_control(
    self,
    *,
    HomeRegion: str,
    Target: TargetTypeDef,  # (1)
    DryRun: bool = ...,
) -> CreateHomeRegionControlResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
2. See [:material-code-braces: CreateHomeRegionControlResultTypeDef](./type_defs.md#createhomeregioncontrolresulttypedef) 


```python title="Usage example with kwargs"
kwargs: CreateHomeRegionControlRequestRequestTypeDef = {  # (1)
    "HomeRegion": ...,
    "Target": ...,
}

parent.create_home_region_control(**kwargs)
```

1. See [:material-code-braces: CreateHomeRegionControlRequestRequestTypeDef](./type_defs.md#createhomeregioncontrolrequestrequesttypedef) 

### describe\_home\_region\_controls

This API permits filtering on the `ControlId` and `HomeRegion` fields.

Type annotations and code completion for `#!python session.create_client("migrationhub-config").describe_home_region_controls` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig.Client.describe_home_region_controls)

```python title="Method definition"
await def describe_home_region_controls(
    self,
    *,
    ControlId: str = ...,
    HomeRegion: str = ...,
    Target: TargetTypeDef = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeHomeRegionControlsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
2. See [:material-code-braces: DescribeHomeRegionControlsResultTypeDef](./type_defs.md#describehomeregioncontrolsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeHomeRegionControlsRequestRequestTypeDef = {  # (1)
    "ControlId": ...,
}

parent.describe_home_region_controls(**kwargs)
```

1. See [:material-code-braces: DescribeHomeRegionControlsRequestRequestTypeDef](./type_defs.md#describehomeregioncontrolsrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("migrationhub-config").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig.Client.generate_presigned_url)

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


### get\_home\_region

Returns the calling account’s home region, if configured.

Type annotations and code completion for `#!python session.create_client("migrationhub-config").get_home_region` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig.Client.get_home_region)

```python title="Method definition"
await def get_home_region(
    self,
) -> GetHomeRegionResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetHomeRegionResultTypeDef](./type_defs.md#gethomeregionresulttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("migrationhub-config").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig.Client.__aenter__)

```python title="Method definition"
await def __aenter__(
    self,
) -> MigrationHubConfigClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("migrationhub-config").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig.Client.__aexit__)

```python title="Method definition"
await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```





