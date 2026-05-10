# Paginators

> [Index](../README.md) > [CloudWatchObservabilityAdminService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CloudWatchObservabilityAdminService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin.html#cloudwatchobservabilityadminservice)
    type annotations stubs module [types-aiobotocore-observabilityadmin](https://pypi.org/project/types-aiobotocore-observabilityadmin/).

## ListCentralizationRulesForOrganizationPaginator

Type annotations and code completion for `#!python session.create_client("observabilityadmin").get_paginator("list_centralization_rules_for_organization")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/paginator/ListCentralizationRulesForOrganization.html#CloudWatchObservabilityAdminService.Paginator.ListCentralizationRulesForOrganization)

```python
# ListCentralizationRulesForOrganizationPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_observabilityadmin.paginator import ListCentralizationRulesForOrganizationPaginator

session = get_session()
async with session.create_client("observabilityadmin") as client:  # (1)
    paginator: ListCentralizationRulesForOrganizationPaginator = client.get_paginator("list_centralization_rules_for_organization")  # (2)
    async for item in paginator.paginate(...):
        item: ListCentralizationRulesForOrganizationOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchObservabilityAdminServiceClient](./client.md)
2. paginator: [ListCentralizationRulesForOrganizationPaginator](./paginators.md#listcentralizationrulesfororganizationpaginator)
3. item: `AioPageIterator[ListCentralizationRulesForOrganizationOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCentralizationRulesForOrganizationPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    RuleNamePrefix: str = ...,
    AllRegions: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListCentralizationRulesForOrganizationOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListCentralizationRulesForOrganizationOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCentralizationRulesForOrganizationInputPaginateTypeDef = {  # (1)
    "RuleNamePrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCentralizationRulesForOrganizationInputPaginateTypeDef](./type_defs.md#listcentralizationrulesfororganizationinputpaginatetypedef)
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
3. item: `AioPageIterator[ListResourceTelemetryForOrganizationOutputTypeDef]`


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
) -> aiobotocore.paginate.AioPageIterator[ListResourceTelemetryForOrganizationOutputTypeDef]:  # (4)
    ...
```

1. See `Sequence[ResourceTypeType]`
2. See `Mapping[TelemetryTypeType, TelemetryStateType]`
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListResourceTelemetryForOrganizationOutputTypeDef]`


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
3. item: `AioPageIterator[ListResourceTelemetryOutputTypeDef]`


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
) -> aiobotocore.paginate.AioPageIterator[ListResourceTelemetryOutputTypeDef]:  # (4)
    ...
```

1. See `Sequence[ResourceTypeType]`
2. See `Mapping[TelemetryTypeType, TelemetryStateType]`
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListResourceTelemetryOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListResourceTelemetryInputPaginateTypeDef = {  # (1)
    "ResourceIdentifierPrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourceTelemetryInputPaginateTypeDef](./type_defs.md#listresourcetelemetryinputpaginatetypedef)
## ListS3TableIntegrationsPaginator

Type annotations and code completion for `#!python session.create_client("observabilityadmin").get_paginator("list_s3_table_integrations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/paginator/ListS3TableIntegrations.html#CloudWatchObservabilityAdminService.Paginator.ListS3TableIntegrations)

```python
# ListS3TableIntegrationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_observabilityadmin.paginator import ListS3TableIntegrationsPaginator

session = get_session()
async with session.create_client("observabilityadmin") as client:  # (1)
    paginator: ListS3TableIntegrationsPaginator = client.get_paginator("list_s3_table_integrations")  # (2)
    async for item in paginator.paginate(...):
        item: ListS3TableIntegrationsOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchObservabilityAdminServiceClient](./client.md)
2. paginator: [ListS3TableIntegrationsPaginator](./paginators.md#lists3tableintegrationspaginator)
3. item: `AioPageIterator[ListS3TableIntegrationsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListS3TableIntegrationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListS3TableIntegrationsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListS3TableIntegrationsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListS3TableIntegrationsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListS3TableIntegrationsInputPaginateTypeDef](./type_defs.md#lists3tableintegrationsinputpaginatetypedef)
## ListTelemetryPipelinesPaginator

Type annotations and code completion for `#!python session.create_client("observabilityadmin").get_paginator("list_telemetry_pipelines")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/paginator/ListTelemetryPipelines.html#CloudWatchObservabilityAdminService.Paginator.ListTelemetryPipelines)

```python
# ListTelemetryPipelinesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_observabilityadmin.paginator import ListTelemetryPipelinesPaginator

session = get_session()
async with session.create_client("observabilityadmin") as client:  # (1)
    paginator: ListTelemetryPipelinesPaginator = client.get_paginator("list_telemetry_pipelines")  # (2)
    async for item in paginator.paginate(...):
        item: ListTelemetryPipelinesOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchObservabilityAdminServiceClient](./client.md)
2. paginator: [ListTelemetryPipelinesPaginator](./paginators.md#listtelemetrypipelinespaginator)
3. item: `AioPageIterator[ListTelemetryPipelinesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTelemetryPipelinesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTelemetryPipelinesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTelemetryPipelinesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTelemetryPipelinesInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTelemetryPipelinesInputPaginateTypeDef](./type_defs.md#listtelemetrypipelinesinputpaginatetypedef)
## ListTelemetryRulesForOrganizationPaginator

Type annotations and code completion for `#!python session.create_client("observabilityadmin").get_paginator("list_telemetry_rules_for_organization")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/paginator/ListTelemetryRulesForOrganization.html#CloudWatchObservabilityAdminService.Paginator.ListTelemetryRulesForOrganization)

```python
# ListTelemetryRulesForOrganizationPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_observabilityadmin.paginator import ListTelemetryRulesForOrganizationPaginator

session = get_session()
async with session.create_client("observabilityadmin") as client:  # (1)
    paginator: ListTelemetryRulesForOrganizationPaginator = client.get_paginator("list_telemetry_rules_for_organization")  # (2)
    async for item in paginator.paginate(...):
        item: ListTelemetryRulesForOrganizationOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchObservabilityAdminServiceClient](./client.md)
2. paginator: [ListTelemetryRulesForOrganizationPaginator](./paginators.md#listtelemetryrulesfororganizationpaginator)
3. item: `AioPageIterator[ListTelemetryRulesForOrganizationOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTelemetryRulesForOrganizationPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    RuleNamePrefix: str = ...,
    SourceAccountIds: Sequence[str] = ...,
    SourceOrganizationUnitIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTelemetryRulesForOrganizationOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTelemetryRulesForOrganizationOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTelemetryRulesForOrganizationInputPaginateTypeDef = {  # (1)
    "RuleNamePrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTelemetryRulesForOrganizationInputPaginateTypeDef](./type_defs.md#listtelemetryrulesfororganizationinputpaginatetypedef)
## ListTelemetryRulesPaginator

Type annotations and code completion for `#!python session.create_client("observabilityadmin").get_paginator("list_telemetry_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin/paginator/ListTelemetryRules.html#CloudWatchObservabilityAdminService.Paginator.ListTelemetryRules)

```python
# ListTelemetryRulesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_observabilityadmin.paginator import ListTelemetryRulesPaginator

session = get_session()
async with session.create_client("observabilityadmin") as client:  # (1)
    paginator: ListTelemetryRulesPaginator = client.get_paginator("list_telemetry_rules")  # (2)
    async for item in paginator.paginate(...):
        item: ListTelemetryRulesOutputTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchObservabilityAdminServiceClient](./client.md)
2. paginator: [ListTelemetryRulesPaginator](./paginators.md#listtelemetryrulespaginator)
3. item: `AioPageIterator[ListTelemetryRulesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTelemetryRulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    RuleNamePrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTelemetryRulesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTelemetryRulesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTelemetryRulesInputPaginateTypeDef = {  # (1)
    "RuleNamePrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTelemetryRulesInputPaginateTypeDef](./type_defs.md#listtelemetryrulesinputpaginatetypedef)
