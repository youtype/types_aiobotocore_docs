# Paginators

> [Index](../README.md) > [GreengrassV2](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [GreengrassV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#greengrassv2)
    type annotations stubs module [types-aiobotocore-greengrassv2](https://pypi.org/project/types-aiobotocore-greengrassv2/).

## ListClientDevicesAssociatedWithCoreDevicePaginator

Type annotations and code completion for `#!python session.create_client("greengrassv2").get_paginator("list_client_devices_associated_with_core_device")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2/paginator/ListClientDevicesAssociatedWithCoreDevice.html#GreengrassV2.Paginator.ListClientDevicesAssociatedWithCoreDevice)

```python
# ListClientDevicesAssociatedWithCoreDevicePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_greengrassv2.paginator import ListClientDevicesAssociatedWithCoreDevicePaginator

session = get_session()
async with session.create_client("greengrassv2") as client:  # (1)
    paginator: ListClientDevicesAssociatedWithCoreDevicePaginator = client.get_paginator("list_client_devices_associated_with_core_device")  # (2)
    async for item in paginator.paginate(...):
        item: ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassV2Client](./client.md)
2. paginator: [ListClientDevicesAssociatedWithCoreDevicePaginator](./paginators.md#listclientdevicesassociatedwithcoredevicepaginator)
3. item: [:material-code-braces: ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef](./type_defs.md#listclientdevicesassociatedwithcoredeviceresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListClientDevicesAssociatedWithCoreDevicePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    coreDeviceThingName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef](./type_defs.md#listclientdevicesassociatedwithcoredeviceresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListClientDevicesAssociatedWithCoreDeviceRequestPaginateTypeDef = {  # (1)
    "coreDeviceThingName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListClientDevicesAssociatedWithCoreDeviceRequestPaginateTypeDef](./type_defs.md#listclientdevicesassociatedwithcoredevicerequestpaginatetypedef) 
## ListComponentVersionsPaginator

Type annotations and code completion for `#!python session.create_client("greengrassv2").get_paginator("list_component_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2/paginator/ListComponentVersions.html#GreengrassV2.Paginator.ListComponentVersions)

```python
# ListComponentVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_greengrassv2.paginator import ListComponentVersionsPaginator

session = get_session()
async with session.create_client("greengrassv2") as client:  # (1)
    paginator: ListComponentVersionsPaginator = client.get_paginator("list_component_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListComponentVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassV2Client](./client.md)
2. paginator: [ListComponentVersionsPaginator](./paginators.md#listcomponentversionspaginator)
3. item: [:material-code-braces: ListComponentVersionsResponseTypeDef](./type_defs.md#listcomponentversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListComponentVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    arn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListComponentVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListComponentVersionsResponseTypeDef](./type_defs.md#listcomponentversionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListComponentVersionsRequestPaginateTypeDef = {  # (1)
    "arn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListComponentVersionsRequestPaginateTypeDef](./type_defs.md#listcomponentversionsrequestpaginatetypedef) 
## ListComponentsPaginator

Type annotations and code completion for `#!python session.create_client("greengrassv2").get_paginator("list_components")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2/paginator/ListComponents.html#GreengrassV2.Paginator.ListComponents)

```python
# ListComponentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_greengrassv2.paginator import ListComponentsPaginator

session = get_session()
async with session.create_client("greengrassv2") as client:  # (1)
    paginator: ListComponentsPaginator = client.get_paginator("list_components")  # (2)
    async for item in paginator.paginate(...):
        item: ListComponentsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassV2Client](./client.md)
2. paginator: [ListComponentsPaginator](./paginators.md#listcomponentspaginator)
3. item: [:material-code-braces: ListComponentsResponseTypeDef](./type_defs.md#listcomponentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListComponentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    scope: ComponentVisibilityScopeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListComponentsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ComponentVisibilityScopeType](./literals.md#componentvisibilityscopetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListComponentsResponseTypeDef](./type_defs.md#listcomponentsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListComponentsRequestPaginateTypeDef = {  # (1)
    "scope": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListComponentsRequestPaginateTypeDef](./type_defs.md#listcomponentsrequestpaginatetypedef) 
## ListCoreDevicesPaginator

Type annotations and code completion for `#!python session.create_client("greengrassv2").get_paginator("list_core_devices")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2/paginator/ListCoreDevices.html#GreengrassV2.Paginator.ListCoreDevices)

```python
# ListCoreDevicesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_greengrassv2.paginator import ListCoreDevicesPaginator

session = get_session()
async with session.create_client("greengrassv2") as client:  # (1)
    paginator: ListCoreDevicesPaginator = client.get_paginator("list_core_devices")  # (2)
    async for item in paginator.paginate(...):
        item: ListCoreDevicesResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassV2Client](./client.md)
2. paginator: [ListCoreDevicesPaginator](./paginators.md#listcoredevicespaginator)
3. item: [:material-code-braces: ListCoreDevicesResponseTypeDef](./type_defs.md#listcoredevicesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCoreDevicesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    thingGroupArn: str = ...,
    status: CoreDeviceStatusType = ...,  # (1)
    runtime: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListCoreDevicesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: CoreDeviceStatusType](./literals.md#coredevicestatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListCoreDevicesResponseTypeDef](./type_defs.md#listcoredevicesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCoreDevicesRequestPaginateTypeDef = {  # (1)
    "thingGroupArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCoreDevicesRequestPaginateTypeDef](./type_defs.md#listcoredevicesrequestpaginatetypedef) 
## ListDeploymentsPaginator

Type annotations and code completion for `#!python session.create_client("greengrassv2").get_paginator("list_deployments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2/paginator/ListDeployments.html#GreengrassV2.Paginator.ListDeployments)

```python
# ListDeploymentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_greengrassv2.paginator import ListDeploymentsPaginator

session = get_session()
async with session.create_client("greengrassv2") as client:  # (1)
    paginator: ListDeploymentsPaginator = client.get_paginator("list_deployments")  # (2)
    async for item in paginator.paginate(...):
        item: ListDeploymentsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassV2Client](./client.md)
2. paginator: [ListDeploymentsPaginator](./paginators.md#listdeploymentspaginator)
3. item: [:material-code-braces: ListDeploymentsResponseTypeDef](./type_defs.md#listdeploymentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDeploymentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    targetArn: str = ...,
    historyFilter: DeploymentHistoryFilterType = ...,  # (1)
    parentTargetArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListDeploymentsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: DeploymentHistoryFilterType](./literals.md#deploymenthistoryfiltertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDeploymentsResponseTypeDef](./type_defs.md#listdeploymentsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDeploymentsRequestPaginateTypeDef = {  # (1)
    "targetArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeploymentsRequestPaginateTypeDef](./type_defs.md#listdeploymentsrequestpaginatetypedef) 
## ListEffectiveDeploymentsPaginator

Type annotations and code completion for `#!python session.create_client("greengrassv2").get_paginator("list_effective_deployments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2/paginator/ListEffectiveDeployments.html#GreengrassV2.Paginator.ListEffectiveDeployments)

```python
# ListEffectiveDeploymentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_greengrassv2.paginator import ListEffectiveDeploymentsPaginator

session = get_session()
async with session.create_client("greengrassv2") as client:  # (1)
    paginator: ListEffectiveDeploymentsPaginator = client.get_paginator("list_effective_deployments")  # (2)
    async for item in paginator.paginate(...):
        item: ListEffectiveDeploymentsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassV2Client](./client.md)
2. paginator: [ListEffectiveDeploymentsPaginator](./paginators.md#listeffectivedeploymentspaginator)
3. item: [:material-code-braces: ListEffectiveDeploymentsResponseTypeDef](./type_defs.md#listeffectivedeploymentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEffectiveDeploymentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    coreDeviceThingName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListEffectiveDeploymentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEffectiveDeploymentsResponseTypeDef](./type_defs.md#listeffectivedeploymentsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEffectiveDeploymentsRequestPaginateTypeDef = {  # (1)
    "coreDeviceThingName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEffectiveDeploymentsRequestPaginateTypeDef](./type_defs.md#listeffectivedeploymentsrequestpaginatetypedef) 
## ListInstalledComponentsPaginator

Type annotations and code completion for `#!python session.create_client("greengrassv2").get_paginator("list_installed_components")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2/paginator/ListInstalledComponents.html#GreengrassV2.Paginator.ListInstalledComponents)

```python
# ListInstalledComponentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_greengrassv2.paginator import ListInstalledComponentsPaginator

session = get_session()
async with session.create_client("greengrassv2") as client:  # (1)
    paginator: ListInstalledComponentsPaginator = client.get_paginator("list_installed_components")  # (2)
    async for item in paginator.paginate(...):
        item: ListInstalledComponentsResponseTypeDef
        print(item)  # (3)
```

1. client: [GreengrassV2Client](./client.md)
2. paginator: [ListInstalledComponentsPaginator](./paginators.md#listinstalledcomponentspaginator)
3. item: [:material-code-braces: ListInstalledComponentsResponseTypeDef](./type_defs.md#listinstalledcomponentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListInstalledComponentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    coreDeviceThingName: str,
    topologyFilter: InstalledComponentTopologyFilterType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListInstalledComponentsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: InstalledComponentTopologyFilterType](./literals.md#installedcomponenttopologyfiltertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListInstalledComponentsResponseTypeDef](./type_defs.md#listinstalledcomponentsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListInstalledComponentsRequestPaginateTypeDef = {  # (1)
    "coreDeviceThingName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInstalledComponentsRequestPaginateTypeDef](./type_defs.md#listinstalledcomponentsrequestpaginatetypedef) 
