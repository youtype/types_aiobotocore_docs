# Paginators

> [Index](../README.md) > [ManagedintegrationsforIoTDeviceManagement](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ManagedintegrationsforIoTDeviceManagement](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-managed-integrations.html#managedintegrationsforiotdevicemanagement)
    type annotations stubs module [types-aiobotocore-iot-managed-integrations](https://pypi.org/project/types-aiobotocore-iot-managed-integrations/).

## ListCredentialLockersPaginator

Type annotations and code completion for `#!python session.create_client("iot-managed-integrations").get_paginator("list_credential_lockers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-managed-integrations/paginator/ListCredentialLockers.html#ManagedintegrationsforIoTDeviceManagement.Paginator.ListCredentialLockers)

```python
# ListCredentialLockersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot_managed_integrations.paginator import ListCredentialLockersPaginator

session = get_session()
async with session.create_client("iot-managed-integrations") as client:  # (1)
    paginator: ListCredentialLockersPaginator = client.get_paginator("list_credential_lockers")  # (2)
    async for item in paginator.paginate(...):
        item: ListCredentialLockersResponseTypeDef
        print(item)  # (3)
```

1. client: [ManagedintegrationsforIoTDeviceManagementClient](./client.md)
2. paginator: [ListCredentialLockersPaginator](./paginators.md#listcredentiallockerspaginator)
3. item: `AioPageIterator[ListCredentialLockersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCredentialLockersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListCredentialLockersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListCredentialLockersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCredentialLockersRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCredentialLockersRequestPaginateTypeDef](./type_defs.md#listcredentiallockersrequestpaginatetypedef)
## ListDestinationsPaginator

Type annotations and code completion for `#!python session.create_client("iot-managed-integrations").get_paginator("list_destinations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-managed-integrations/paginator/ListDestinations.html#ManagedintegrationsforIoTDeviceManagement.Paginator.ListDestinations)

```python
# ListDestinationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot_managed_integrations.paginator import ListDestinationsPaginator

session = get_session()
async with session.create_client("iot-managed-integrations") as client:  # (1)
    paginator: ListDestinationsPaginator = client.get_paginator("list_destinations")  # (2)
    async for item in paginator.paginate(...):
        item: ListDestinationsResponseTypeDef
        print(item)  # (3)
```

1. client: [ManagedintegrationsforIoTDeviceManagementClient](./client.md)
2. paginator: [ListDestinationsPaginator](./paginators.md#listdestinationspaginator)
3. item: `AioPageIterator[ListDestinationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDestinationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDestinationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDestinationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDestinationsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDestinationsRequestPaginateTypeDef](./type_defs.md#listdestinationsrequestpaginatetypedef)
## ListEventLogConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("iot-managed-integrations").get_paginator("list_event_log_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-managed-integrations/paginator/ListEventLogConfigurations.html#ManagedintegrationsforIoTDeviceManagement.Paginator.ListEventLogConfigurations)

```python
# ListEventLogConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot_managed_integrations.paginator import ListEventLogConfigurationsPaginator

session = get_session()
async with session.create_client("iot-managed-integrations") as client:  # (1)
    paginator: ListEventLogConfigurationsPaginator = client.get_paginator("list_event_log_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListEventLogConfigurationsResponseTypeDef
        print(item)  # (3)
```

1. client: [ManagedintegrationsforIoTDeviceManagementClient](./client.md)
2. paginator: [ListEventLogConfigurationsPaginator](./paginators.md#listeventlogconfigurationspaginator)
3. item: `AioPageIterator[ListEventLogConfigurationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListEventLogConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListEventLogConfigurationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListEventLogConfigurationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListEventLogConfigurationsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEventLogConfigurationsRequestPaginateTypeDef](./type_defs.md#listeventlogconfigurationsrequestpaginatetypedef)
## ListManagedThingSchemasPaginator

Type annotations and code completion for `#!python session.create_client("iot-managed-integrations").get_paginator("list_managed_thing_schemas")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-managed-integrations/paginator/ListManagedThingSchemas.html#ManagedintegrationsforIoTDeviceManagement.Paginator.ListManagedThingSchemas)

```python
# ListManagedThingSchemasPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot_managed_integrations.paginator import ListManagedThingSchemasPaginator

session = get_session()
async with session.create_client("iot-managed-integrations") as client:  # (1)
    paginator: ListManagedThingSchemasPaginator = client.get_paginator("list_managed_thing_schemas")  # (2)
    async for item in paginator.paginate(...):
        item: ListManagedThingSchemasResponseTypeDef
        print(item)  # (3)
```

1. client: [ManagedintegrationsforIoTDeviceManagementClient](./client.md)
2. paginator: [ListManagedThingSchemasPaginator](./paginators.md#listmanagedthingschemaspaginator)
3. item: `AioPageIterator[ListManagedThingSchemasResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListManagedThingSchemasPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Identifier: str,
    EndpointIdFilter: str = ...,
    CapabilityIdFilter: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListManagedThingSchemasResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListManagedThingSchemasResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListManagedThingSchemasRequestPaginateTypeDef = {  # (1)
    "Identifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListManagedThingSchemasRequestPaginateTypeDef](./type_defs.md#listmanagedthingschemasrequestpaginatetypedef)
## ListManagedThingsPaginator

Type annotations and code completion for `#!python session.create_client("iot-managed-integrations").get_paginator("list_managed_things")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-managed-integrations/paginator/ListManagedThings.html#ManagedintegrationsforIoTDeviceManagement.Paginator.ListManagedThings)

```python
# ListManagedThingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot_managed_integrations.paginator import ListManagedThingsPaginator

session = get_session()
async with session.create_client("iot-managed-integrations") as client:  # (1)
    paginator: ListManagedThingsPaginator = client.get_paginator("list_managed_things")  # (2)
    async for item in paginator.paginate(...):
        item: ListManagedThingsResponseTypeDef
        print(item)  # (3)
```

1. client: [ManagedintegrationsforIoTDeviceManagementClient](./client.md)
2. paginator: [ListManagedThingsPaginator](./paginators.md#listmanagedthingspaginator)
3. item: `AioPageIterator[ListManagedThingsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListManagedThingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OwnerFilter: str = ...,
    CredentialLockerFilter: str = ...,
    RoleFilter: RoleType = ...,  # (1)
    ParentControllerIdentifierFilter: str = ...,
    ConnectorPolicyIdFilter: str = ...,
    SerialNumberFilter: str = ...,
    ProvisioningStatusFilter: ProvisioningStatusType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListManagedThingsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: RoleType](./literals.md#roletype)
2. See [:material-code-brackets: ProvisioningStatusType](./literals.md#provisioningstatustype)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListManagedThingsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListManagedThingsRequestPaginateTypeDef = {  # (1)
    "OwnerFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListManagedThingsRequestPaginateTypeDef](./type_defs.md#listmanagedthingsrequestpaginatetypedef)
## ListNotificationConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("iot-managed-integrations").get_paginator("list_notification_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-managed-integrations/paginator/ListNotificationConfigurations.html#ManagedintegrationsforIoTDeviceManagement.Paginator.ListNotificationConfigurations)

```python
# ListNotificationConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot_managed_integrations.paginator import ListNotificationConfigurationsPaginator

session = get_session()
async with session.create_client("iot-managed-integrations") as client:  # (1)
    paginator: ListNotificationConfigurationsPaginator = client.get_paginator("list_notification_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListNotificationConfigurationsResponseTypeDef
        print(item)  # (3)
```

1. client: [ManagedintegrationsforIoTDeviceManagementClient](./client.md)
2. paginator: [ListNotificationConfigurationsPaginator](./paginators.md#listnotificationconfigurationspaginator)
3. item: `AioPageIterator[ListNotificationConfigurationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListNotificationConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListNotificationConfigurationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListNotificationConfigurationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListNotificationConfigurationsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListNotificationConfigurationsRequestPaginateTypeDef](./type_defs.md#listnotificationconfigurationsrequestpaginatetypedef)
## ListOtaTaskConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("iot-managed-integrations").get_paginator("list_ota_task_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-managed-integrations/paginator/ListOtaTaskConfigurations.html#ManagedintegrationsforIoTDeviceManagement.Paginator.ListOtaTaskConfigurations)

```python
# ListOtaTaskConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot_managed_integrations.paginator import ListOtaTaskConfigurationsPaginator

session = get_session()
async with session.create_client("iot-managed-integrations") as client:  # (1)
    paginator: ListOtaTaskConfigurationsPaginator = client.get_paginator("list_ota_task_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListOtaTaskConfigurationsResponseTypeDef
        print(item)  # (3)
```

1. client: [ManagedintegrationsforIoTDeviceManagementClient](./client.md)
2. paginator: [ListOtaTaskConfigurationsPaginator](./paginators.md#listotataskconfigurationspaginator)
3. item: `AioPageIterator[ListOtaTaskConfigurationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListOtaTaskConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListOtaTaskConfigurationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListOtaTaskConfigurationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListOtaTaskConfigurationsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOtaTaskConfigurationsRequestPaginateTypeDef](./type_defs.md#listotataskconfigurationsrequestpaginatetypedef)
## ListOtaTaskExecutionsPaginator

Type annotations and code completion for `#!python session.create_client("iot-managed-integrations").get_paginator("list_ota_task_executions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-managed-integrations/paginator/ListOtaTaskExecutions.html#ManagedintegrationsforIoTDeviceManagement.Paginator.ListOtaTaskExecutions)

```python
# ListOtaTaskExecutionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot_managed_integrations.paginator import ListOtaTaskExecutionsPaginator

session = get_session()
async with session.create_client("iot-managed-integrations") as client:  # (1)
    paginator: ListOtaTaskExecutionsPaginator = client.get_paginator("list_ota_task_executions")  # (2)
    async for item in paginator.paginate(...):
        item: ListOtaTaskExecutionsResponseTypeDef
        print(item)  # (3)
```

1. client: [ManagedintegrationsforIoTDeviceManagementClient](./client.md)
2. paginator: [ListOtaTaskExecutionsPaginator](./paginators.md#listotataskexecutionspaginator)
3. item: `AioPageIterator[ListOtaTaskExecutionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListOtaTaskExecutionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Identifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListOtaTaskExecutionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListOtaTaskExecutionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListOtaTaskExecutionsRequestPaginateTypeDef = {  # (1)
    "Identifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOtaTaskExecutionsRequestPaginateTypeDef](./type_defs.md#listotataskexecutionsrequestpaginatetypedef)
## ListOtaTasksPaginator

Type annotations and code completion for `#!python session.create_client("iot-managed-integrations").get_paginator("list_ota_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-managed-integrations/paginator/ListOtaTasks.html#ManagedintegrationsforIoTDeviceManagement.Paginator.ListOtaTasks)

```python
# ListOtaTasksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot_managed_integrations.paginator import ListOtaTasksPaginator

session = get_session()
async with session.create_client("iot-managed-integrations") as client:  # (1)
    paginator: ListOtaTasksPaginator = client.get_paginator("list_ota_tasks")  # (2)
    async for item in paginator.paginate(...):
        item: ListOtaTasksResponseTypeDef
        print(item)  # (3)
```

1. client: [ManagedintegrationsforIoTDeviceManagementClient](./client.md)
2. paginator: [ListOtaTasksPaginator](./paginators.md#listotataskspaginator)
3. item: `AioPageIterator[ListOtaTasksResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListOtaTasksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListOtaTasksResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListOtaTasksResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListOtaTasksRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOtaTasksRequestPaginateTypeDef](./type_defs.md#listotatasksrequestpaginatetypedef)
## ListProvisioningProfilesPaginator

Type annotations and code completion for `#!python session.create_client("iot-managed-integrations").get_paginator("list_provisioning_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-managed-integrations/paginator/ListProvisioningProfiles.html#ManagedintegrationsforIoTDeviceManagement.Paginator.ListProvisioningProfiles)

```python
# ListProvisioningProfilesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot_managed_integrations.paginator import ListProvisioningProfilesPaginator

session = get_session()
async with session.create_client("iot-managed-integrations") as client:  # (1)
    paginator: ListProvisioningProfilesPaginator = client.get_paginator("list_provisioning_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: ListProvisioningProfilesResponseTypeDef
        print(item)  # (3)
```

1. client: [ManagedintegrationsforIoTDeviceManagementClient](./client.md)
2. paginator: [ListProvisioningProfilesPaginator](./paginators.md#listprovisioningprofilespaginator)
3. item: `AioPageIterator[ListProvisioningProfilesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListProvisioningProfilesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListProvisioningProfilesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListProvisioningProfilesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListProvisioningProfilesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProvisioningProfilesRequestPaginateTypeDef](./type_defs.md#listprovisioningprofilesrequestpaginatetypedef)
## ListSchemaVersionsPaginator

Type annotations and code completion for `#!python session.create_client("iot-managed-integrations").get_paginator("list_schema_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-managed-integrations/paginator/ListSchemaVersions.html#ManagedintegrationsforIoTDeviceManagement.Paginator.ListSchemaVersions)

```python
# ListSchemaVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot_managed_integrations.paginator import ListSchemaVersionsPaginator

session = get_session()
async with session.create_client("iot-managed-integrations") as client:  # (1)
    paginator: ListSchemaVersionsPaginator = client.get_paginator("list_schema_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListSchemaVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [ManagedintegrationsforIoTDeviceManagementClient](./client.md)
2. paginator: [ListSchemaVersionsPaginator](./paginators.md#listschemaversionspaginator)
3. item: `AioPageIterator[ListSchemaVersionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSchemaVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Type: SchemaVersionTypeType,  # (1)
    SchemaId: str = ...,
    Namespace: str = ...,
    Visibility: SchemaVersionVisibilityType = ...,  # (2)
    SemanticVersion: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListSchemaVersionsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: SchemaVersionTypeType](./literals.md#schemaversiontypetype)
2. See [:material-code-brackets: SchemaVersionVisibilityType](./literals.md#schemaversionvisibilitytype)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListSchemaVersionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSchemaVersionsRequestPaginateTypeDef = {  # (1)
    "Type": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSchemaVersionsRequestPaginateTypeDef](./type_defs.md#listschemaversionsrequestpaginatetypedef)
