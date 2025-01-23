# Paginators

> [Index](../README.md) > [CloudWatchObservabilityAdminService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CloudWatchObservabilityAdminService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin.html#cloudwatchobservabilityadminservice)
    type annotations stubs module [types-aiobotocore-observabilityadmin](https://pypi.org/project/types-aiobotocore-observabilityadmin/).

## ListResourceTelemetryForOrganizationPaginator

Type annotations and code completion for `#!python session.create_client("observabilityadmin").get_paginator("list_resource_telemetry_for_organization")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/paginator/ListResourceTelemetryForOrganization.html#CloudWatchObservabilityAdminService.Paginator.ListResourceTelemetryForOrganization)

```python
# ListResourceTelemetryForOrganizationPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_observabilityadmin.paginator import ListResourceTelemetryForOrganizationPaginator

session = get_session()
async with session.create_client("observabilityadmin") as client:  # (1)
    paginator: ListResourceTelemetryForOrganizationPaginator = client.get_paginator("list_resource_telemetry_for_organization")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourceTelemetryForOrganizationOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchObservabilityAdminServiceClient](./client.md)
2. paginator: [ListResourceTelemetryForOrganizationPaginator](./paginators.md#listresourcetelemetryfororganizationpaginator)
3. item: [:material-code-braces: ListResourceTelemetryForOrganizationOutputTypeDef](./type_defs.md#listresourcetelemetryfororganizationoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListResourceTelemetryForOrganizationPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AccountIdentifiers: Sequence[str] = ...,
    ResourceIdentifierPrefix: str = ...,
    ResourceTypes: Sequence[ResourceTypeType] = ...,  # (1)
    TelemetryConfigurationState: Mapping[TelemetryTypeType, TelemetryStateType] = ...,  # (2)
    ResourceTags: Mapping[str, str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListResourceTelemetryForOrganizationOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: TelemetryTypeType](./literals.md#telemetrytypetype) [:material-code-brackets: TelemetryStateType](./literals.md#telemetrystatetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListResourceTelemetryForOrganizationOutputTypeDef](./type_defs.md#listresourcetelemetryfororganizationoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListResourceTelemetryForOrganizationInputPaginateTypeDef = {  # (1)
    "AccountIdentifiers": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourceTelemetryForOrganizationInputPaginateTypeDef](./type_defs.md#listresourcetelemetryfororganizationinputpaginatetypedef) 
## ListResourceTelemetryPaginator

Type annotations and code completion for `#!python session.create_client("observabilityadmin").get_paginator("list_resource_telemetry")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/paginator/ListResourceTelemetry.html#CloudWatchObservabilityAdminService.Paginator.ListResourceTelemetry)

```python
# ListResourceTelemetryPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_observabilityadmin.paginator import ListResourceTelemetryPaginator

session = get_session()
async with session.create_client("observabilityadmin") as client:  # (1)
    paginator: ListResourceTelemetryPaginator = client.get_paginator("list_resource_telemetry")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourceTelemetryOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchObservabilityAdminServiceClient](./client.md)
2. paginator: [ListResourceTelemetryPaginator](./paginators.md#listresourcetelemetrypaginator)
3. item: [:material-code-braces: ListResourceTelemetryOutputTypeDef](./type_defs.md#listresourcetelemetryoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListResourceTelemetryPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceIdentifierPrefix: str = ...,
    ResourceTypes: Sequence[ResourceTypeType] = ...,  # (1)
    TelemetryConfigurationState: Mapping[TelemetryTypeType, TelemetryStateType] = ...,  # (2)
    ResourceTags: Mapping[str, str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListResourceTelemetryOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: TelemetryTypeType](./literals.md#telemetrytypetype) [:material-code-brackets: TelemetryStateType](./literals.md#telemetrystatetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListResourceTelemetryOutputTypeDef](./type_defs.md#listresourcetelemetryoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListResourceTelemetryInputPaginateTypeDef = {  # (1)
    "ResourceIdentifierPrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourceTelemetryInputPaginateTypeDef](./type_defs.md#listresourcetelemetryinputpaginatetypedef) 
