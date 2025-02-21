# MigrationHubConfigClient

> [Index](../README.md) > [MigrationHubConfig](./README.md) > MigrationHubConfigClient

!!! note ""

    Auto-generated documentation for [MigrationHubConfig](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#migrationhubconfig)
    type annotations stubs module [types-aiobotocore-migrationhub-config](https://pypi.org/project/types-aiobotocore-migrationhub-config/).

## MigrationHubConfigClient

Type annotations and code completion for `#!python session.create_client("migrationhub-config")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig.Client)

```python
# MigrationHubConfigClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_migrationhub_config.client import MigrationHubConfigClient

session = get_session()
async with session.create_client("migrationhub-config") as client:
    client: MigrationHubConfigClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("migrationhub-config").exceptions` structure.

```python
# MigrationHubConfigClient.exceptions usage example

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

```python
# MigrationHubConfigClient usage type checking example

from types_aiobotocore_migrationhub_config.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("migrationhub-config").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("migrationhub-config").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### create\_home\_region\_control

This API sets up the home region for the calling account only.

Type annotations and code completion for `#!python session.create_client("migrationhub-config").create_home_region_control` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config/client/create_home_region_control.html)

```python
# create_home_region_control method definition

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


```python
# create_home_region_control method usage example with argument unpacking

kwargs: CreateHomeRegionControlRequestTypeDef = {  # (1)
    "HomeRegion": ...,
    "Target": ...,
}

parent.create_home_region_control(**kwargs)
```

1. See [:material-code-braces: CreateHomeRegionControlRequestTypeDef](./type_defs.md#createhomeregioncontrolrequesttypedef) 

### delete\_home\_region\_control

This operation deletes the home region configuration for the calling account.

Type annotations and code completion for `#!python session.create_client("migrationhub-config").delete_home_region_control` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config/client/delete_home_region_control.html)

```python
# delete_home_region_control method definition

await def delete_home_region_control(
    self,
    *,
    ControlId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_home_region_control method usage example with argument unpacking

kwargs: DeleteHomeRegionControlRequestTypeDef = {  # (1)
    "ControlId": ...,
}

parent.delete_home_region_control(**kwargs)
```

1. See [:material-code-braces: DeleteHomeRegionControlRequestTypeDef](./type_defs.md#deletehomeregioncontrolrequesttypedef) 

### describe\_home\_region\_controls

This API permits filtering on the <code>ControlId</code> and
<code>HomeRegion</code> fields.

Type annotations and code completion for `#!python session.create_client("migrationhub-config").describe_home_region_controls` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config/client/describe_home_region_controls.html)

```python
# describe_home_region_controls method definition

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


```python
# describe_home_region_controls method usage example with argument unpacking

kwargs: DescribeHomeRegionControlsRequestTypeDef = {  # (1)
    "ControlId": ...,
}

parent.describe_home_region_controls(**kwargs)
```

1. See [:material-code-braces: DescribeHomeRegionControlsRequestTypeDef](./type_defs.md#describehomeregioncontrolsrequesttypedef) 

### get\_home\_region

Returns the calling account's home region, if configured.

Type annotations and code completion for `#!python session.create_client("migrationhub-config").get_home_region` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config/client/get_home_region.html)

```python
# get_home_region method definition

await def get_home_region(
    self,
) -> GetHomeRegionResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetHomeRegionResultTypeDef](./type_defs.md#gethomeregionresulttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("migrationhub-config").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("migrationhub-config").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```





