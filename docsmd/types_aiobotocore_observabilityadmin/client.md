# CloudWatchObservabilityAdminServiceClient

> [Index](../README.md) > [CloudWatchObservabilityAdminService](./README.md) > CloudWatchObservabilityAdminServiceClient

!!! note ""

    Auto-generated documentation for [CloudWatchObservabilityAdminService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin.html#cloudwatchobservabilityadminservice)
    type annotations stubs module [types-aiobotocore-observabilityadmin](https://pypi.org/project/types-aiobotocore-observabilityadmin/).

## CloudWatchObservabilityAdminServiceClient

Type annotations and code completion for `#!python session.create_client("observabilityadmin")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin.html#CloudWatchObservabilityAdminService.Client)

```python
# CloudWatchObservabilityAdminServiceClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_observabilityadmin.client import CloudWatchObservabilityAdminServiceClient

session = get_session()
async with session.create_client("observabilityadmin") as client:
    client: CloudWatchObservabilityAdminServiceClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("observabilityadmin").exceptions` structure.

```python
# CloudWatchObservabilityAdminServiceClient.exceptions usage example

async with session.create_client("observabilityadmin") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.InternalServerException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# CloudWatchObservabilityAdminServiceClient usage type checking example

from types_aiobotocore_observabilityadmin.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("observabilityadmin").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("observabilityadmin").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/generate_presigned_url.html)

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


### get\_telemetry\_evaluation\_status

Returns the current onboarding status of the telemetry config feature,
including the status of the feature and reason the feature failed to start or
stop.

Type annotations and code completion for `#!python session.create_client("observabilityadmin").get_telemetry_evaluation_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/get_telemetry_evaluation_status.html)

```python
# get_telemetry_evaluation_status method definition

await def get_telemetry_evaluation_status(
    self,
) -> GetTelemetryEvaluationStatusOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTelemetryEvaluationStatusOutputTypeDef](./type_defs.md#gettelemetryevaluationstatusoutputtypedef) 

### get\_telemetry\_evaluation\_status\_for\_organization

This returns the onboarding status of the telemetry configuration feature for
the organization.

Type annotations and code completion for `#!python session.create_client("observabilityadmin").get_telemetry_evaluation_status_for_organization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/get_telemetry_evaluation_status_for_organization.html)

```python
# get_telemetry_evaluation_status_for_organization method definition

await def get_telemetry_evaluation_status_for_organization(
    self,
) -> GetTelemetryEvaluationStatusForOrganizationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTelemetryEvaluationStatusForOrganizationOutputTypeDef](./type_defs.md#gettelemetryevaluationstatusfororganizationoutputtypedef) 

### list\_resource\_telemetry

Returns a list of telemetry configurations for AWS resources supported by
telemetry config.

Type annotations and code completion for `#!python session.create_client("observabilityadmin").list_resource_telemetry` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/list_resource_telemetry.html)

```python
# list_resource_telemetry method definition

await def list_resource_telemetry(
    self,
    *,
    ResourceIdentifierPrefix: str = ...,
    ResourceTypes: Sequence[ResourceTypeType] = ...,  # (1)
    TelemetryConfigurationState: Mapping[TelemetryTypeType, TelemetryStateType] = ...,  # (2)
    ResourceTags: Mapping[str, str] = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListResourceTelemetryOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: TelemetryTypeType](./literals.md#telemetrytypetype) [:material-code-brackets: TelemetryStateType](./literals.md#telemetrystatetype) 
3. See [:material-code-braces: ListResourceTelemetryOutputTypeDef](./type_defs.md#listresourcetelemetryoutputtypedef) 


```python
# list_resource_telemetry method usage example with argument unpacking

kwargs: ListResourceTelemetryInputTypeDef = {  # (1)
    "ResourceIdentifierPrefix": ...,
}

parent.list_resource_telemetry(**kwargs)
```

1. See [:material-code-braces: ListResourceTelemetryInputTypeDef](./type_defs.md#listresourcetelemetryinputtypedef) 

### list\_resource\_telemetry\_for\_organization

Returns a list of telemetry configurations for AWS resources supported by
telemetry config in the organization.

Type annotations and code completion for `#!python session.create_client("observabilityadmin").list_resource_telemetry_for_organization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/list_resource_telemetry_for_organization.html)

```python
# list_resource_telemetry_for_organization method definition

await def list_resource_telemetry_for_organization(
    self,
    *,
    AccountIdentifiers: Sequence[str] = ...,
    ResourceIdentifierPrefix: str = ...,
    ResourceTypes: Sequence[ResourceTypeType] = ...,  # (1)
    TelemetryConfigurationState: Mapping[TelemetryTypeType, TelemetryStateType] = ...,  # (2)
    ResourceTags: Mapping[str, str] = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListResourceTelemetryForOrganizationOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: TelemetryTypeType](./literals.md#telemetrytypetype) [:material-code-brackets: TelemetryStateType](./literals.md#telemetrystatetype) 
3. See [:material-code-braces: ListResourceTelemetryForOrganizationOutputTypeDef](./type_defs.md#listresourcetelemetryfororganizationoutputtypedef) 


```python
# list_resource_telemetry_for_organization method usage example with argument unpacking

kwargs: ListResourceTelemetryForOrganizationInputTypeDef = {  # (1)
    "AccountIdentifiers": ...,
}

parent.list_resource_telemetry_for_organization(**kwargs)
```

1. See [:material-code-braces: ListResourceTelemetryForOrganizationInputTypeDef](./type_defs.md#listresourcetelemetryfororganizationinputtypedef) 

### start\_telemetry\_evaluation

This action begins onboarding onboarding the caller AWS account to the
telemetry config feature.

Type annotations and code completion for `#!python session.create_client("observabilityadmin").start_telemetry_evaluation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/start_telemetry_evaluation.html)

```python
# start_telemetry_evaluation method definition

await def start_telemetry_evaluation(
    self,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 

### start\_telemetry\_evaluation\_for\_organization

This actions begins onboarding the organization and all member accounts to the
telemetry config feature.

Type annotations and code completion for `#!python session.create_client("observabilityadmin").start_telemetry_evaluation_for_organization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/start_telemetry_evaluation_for_organization.html)

```python
# start_telemetry_evaluation_for_organization method definition

await def start_telemetry_evaluation_for_organization(
    self,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 

### stop\_telemetry\_evaluation

This action begins offboarding the caller AWS account from the telemetry config
feature.

Type annotations and code completion for `#!python session.create_client("observabilityadmin").stop_telemetry_evaluation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/stop_telemetry_evaluation.html)

```python
# stop_telemetry_evaluation method definition

await def stop_telemetry_evaluation(
    self,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 

### stop\_telemetry\_evaluation\_for\_organization

This action offboards the Organization of the caller AWS account from thef
telemetry config feature.

Type annotations and code completion for `#!python session.create_client("observabilityadmin").stop_telemetry_evaluation_for_organization` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/client/stop_telemetry_evaluation_for_organization.html)

```python
# stop_telemetry_evaluation_for_organization method definition

await def stop_telemetry_evaluation_for_organization(
    self,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("observabilityadmin").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin.html#CloudWatchObservabilityAdminService.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("observabilityadmin").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin.html#CloudWatchObservabilityAdminService.Client)

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




### get_paginator

Type annotations and code completion for `#!python session.create_client("observabilityadmin").get_paginator` method with overloads.

- `client.get_paginator("list_resource_telemetry_for_organization")` -> [ListResourceTelemetryForOrganizationPaginator](./paginators.md#listresourcetelemetryfororganizationpaginator)
- `client.get_paginator("list_resource_telemetry")` -> [ListResourceTelemetryPaginator](./paginators.md#listresourcetelemetrypaginator)



