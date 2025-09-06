# AppConfigDataClient

> [Index](../README.md) > [AppConfigData](./README.md) > AppConfigDataClient

!!! note ""

    Auto-generated documentation for [AppConfigData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#appconfigdata)
    type annotations stubs module [types-aiobotocore-appconfigdata](https://pypi.org/project/types-aiobotocore-appconfigdata/).

## AppConfigDataClient

Type annotations and code completion for `#!python session.create_client("appconfigdata")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData.Client)

```python
# AppConfigDataClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_appconfigdata.client import AppConfigDataClient

session = get_session()
async with session.create_client("appconfigdata") as client:
    client: AppConfigDataClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("appconfigdata").exceptions` structure.

```python
# AppConfigDataClient.exceptions usage example

async with session.create_client("appconfigdata") as client:
    try:
        do_something(client)
    except (
            client.BadRequestException,
        client.ClientError,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ThrottlingException,
    ) as e:
        print(e)
```

```python
# AppConfigDataClient usage type checking example

from types_aiobotocore_appconfigdata.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("appconfigdata").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("appconfigdata").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata/client/generate_presigned_url.html)

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


### get\_latest\_configuration

Retrieves the latest deployed configuration.

Type annotations and code completion for `#!python session.create_client("appconfigdata").get_latest_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata/client/get_latest_configuration.html)

```python
# get_latest_configuration method definition

await def get_latest_configuration(
    self,
    *,
    ConfigurationToken: str,
) -> GetLatestConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLatestConfigurationResponseTypeDef](./type_defs.md#getlatestconfigurationresponsetypedef)


```python
# get_latest_configuration method usage example with argument unpacking

kwargs: GetLatestConfigurationRequestTypeDef = {  # (1)
    "ConfigurationToken": ...,
}

parent.get_latest_configuration(**kwargs)
```

1. See [:material-code-braces: GetLatestConfigurationRequestTypeDef](./type_defs.md#getlatestconfigurationrequesttypedef)

### start\_configuration\_session

Starts a configuration session used to retrieve a deployed configuration.

Type annotations and code completion for `#!python session.create_client("appconfigdata").start_configuration_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata/client/start_configuration_session.html)

```python
# start_configuration_session method definition

await def start_configuration_session(
    self,
    *,
    ApplicationIdentifier: str,
    EnvironmentIdentifier: str,
    ConfigurationProfileIdentifier: str,
    RequiredMinimumPollIntervalInSeconds: int = ...,
) -> StartConfigurationSessionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartConfigurationSessionResponseTypeDef](./type_defs.md#startconfigurationsessionresponsetypedef)


```python
# start_configuration_session method usage example with argument unpacking

kwargs: StartConfigurationSessionRequestTypeDef = {  # (1)
    "ApplicationIdentifier": ...,
    "EnvironmentIdentifier": ...,
    "ConfigurationProfileIdentifier": ...,
}

parent.start_configuration_session(**kwargs)
```

1. See [:material-code-braces: StartConfigurationSessionRequestTypeDef](./type_defs.md#startconfigurationsessionrequesttypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("appconfigdata").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("appconfigdata").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Type[BaseException] | None,
    exc_val: BaseException | None,
    exc_tb: types.TracebackType | None,
) -> None:
    ...
```





