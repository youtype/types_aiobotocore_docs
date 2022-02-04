<a id="paginators-for-aiobotocore-greengrassv2-module"></a>

# Paginators for aiobotocore GreengrassV2 module

> [Index](..) > [GreengrassV2](.) > Paginators

Auto-generated documentation for
[GreengrassV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2)
type annotations stubs module
[types-aiobotocore-greengrassv2](https://pypi.org/project/types-aiobotocore-greengrassv2/).

- [Paginators for aiobotocore GreengrassV2 module](#paginators-for-aiobotocore-greengrassv2-module)
  - [ListClientDevicesAssociatedWithCoreDevicePaginator](#listclientdevicesassociatedwithcoredevicepaginator)
  - [ListComponentVersionsPaginator](#listcomponentversionspaginator)
  - [ListComponentsPaginator](#listcomponentspaginator)
  - [ListCoreDevicesPaginator](#listcoredevicespaginator)
  - [ListDeploymentsPaginator](#listdeploymentspaginator)
  - [ListEffectiveDeploymentsPaginator](#listeffectivedeploymentspaginator)
  - [ListInstalledComponentsPaginator](#listinstalledcomponentspaginator)

<a id="listclientdevicesassociatedwithcoredevicepaginator"></a>

## ListClientDevicesAssociatedWithCoreDevicePaginator

Type annotations for
`aiobotocore.create_client("greengrassv2").get_paginator("list_client_devices_associated_with_core_device")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_greengrassv2.paginator import ListClientDevicesAssociatedWithCoreDevicePaginator

def get_list_client_devices_associated_with_core_device_paginator() -> ListClientDevicesAssociatedWithCoreDevicePaginator:
    return Session().create_client("greengrassv2").get_paginator("list_client_devices_associated_with_core_device")
```

Boto3 documentation:
[GreengrassV2.Paginator.ListClientDevicesAssociatedWithCoreDevice](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListClientDevicesAssociatedWithCoreDevice)

Arguments for `ListClientDevicesAssociatedWithCoreDevicePaginator.paginate`
method:

- `coreDeviceThingName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListClientDevicesAssociatedWithCoreDevicePaginator.paginate` returns
`_PageIterator`\[[ListClientDevicesAssociatedWithCoreDeviceResponseTypeDef](./type_defs.md#listclientdevicesassociatedwithcoredeviceresponsetypedef)\].

<a id="listcomponentversionspaginator"></a>

## ListComponentVersionsPaginator

Type annotations for
`aiobotocore.create_client("greengrassv2").get_paginator("list_component_versions")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_greengrassv2.paginator import ListComponentVersionsPaginator

def get_list_component_versions_paginator() -> ListComponentVersionsPaginator:
    return Session().create_client("greengrassv2").get_paginator("list_component_versions")
```

Boto3 documentation:
[GreengrassV2.Paginator.ListComponentVersions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListComponentVersions)

Arguments for `ListComponentVersionsPaginator.paginate` method:

- `arn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListComponentVersionsPaginator.paginate` returns
`_PageIterator`\[[ListComponentVersionsResponseTypeDef](./type_defs.md#listcomponentversionsresponsetypedef)\].

<a id="listcomponentspaginator"></a>

## ListComponentsPaginator

Type annotations for
`aiobotocore.create_client("greengrassv2").get_paginator("list_components")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_greengrassv2.paginator import ListComponentsPaginator

def get_list_components_paginator() -> ListComponentsPaginator:
    return Session().create_client("greengrassv2").get_paginator("list_components")
```

Boto3 documentation:
[GreengrassV2.Paginator.ListComponents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListComponents)

Arguments for `ListComponentsPaginator.paginate` method:

- `scope`:
  [ComponentVisibilityScopeType](./literals.md#componentvisibilityscopetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListComponentsPaginator.paginate` returns
`_PageIterator`\[[ListComponentsResponseTypeDef](./type_defs.md#listcomponentsresponsetypedef)\].

<a id="listcoredevicespaginator"></a>

## ListCoreDevicesPaginator

Type annotations for
`aiobotocore.create_client("greengrassv2").get_paginator("list_core_devices")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_greengrassv2.paginator import ListCoreDevicesPaginator

def get_list_core_devices_paginator() -> ListCoreDevicesPaginator:
    return Session().create_client("greengrassv2").get_paginator("list_core_devices")
```

Boto3 documentation:
[GreengrassV2.Paginator.ListCoreDevices](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListCoreDevices)

Arguments for `ListCoreDevicesPaginator.paginate` method:

- `thingGroupArn`: `str`
- `status`: [CoreDeviceStatusType](./literals.md#coredevicestatustype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListCoreDevicesPaginator.paginate` returns
`_PageIterator`\[[ListCoreDevicesResponseTypeDef](./type_defs.md#listcoredevicesresponsetypedef)\].

<a id="listdeploymentspaginator"></a>

## ListDeploymentsPaginator

Type annotations for
`aiobotocore.create_client("greengrassv2").get_paginator("list_deployments")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_greengrassv2.paginator import ListDeploymentsPaginator

def get_list_deployments_paginator() -> ListDeploymentsPaginator:
    return Session().create_client("greengrassv2").get_paginator("list_deployments")
```

Boto3 documentation:
[GreengrassV2.Paginator.ListDeployments](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListDeployments)

Arguments for `ListDeploymentsPaginator.paginate` method:

- `targetArn`: `str`
- `historyFilter`:
  [DeploymentHistoryFilterType](./literals.md#deploymenthistoryfiltertype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDeploymentsPaginator.paginate` returns
`_PageIterator`\[[ListDeploymentsResponseTypeDef](./type_defs.md#listdeploymentsresponsetypedef)\].

<a id="listeffectivedeploymentspaginator"></a>

## ListEffectiveDeploymentsPaginator

Type annotations for
`aiobotocore.create_client("greengrassv2").get_paginator("list_effective_deployments")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_greengrassv2.paginator import ListEffectiveDeploymentsPaginator

def get_list_effective_deployments_paginator() -> ListEffectiveDeploymentsPaginator:
    return Session().create_client("greengrassv2").get_paginator("list_effective_deployments")
```

Boto3 documentation:
[GreengrassV2.Paginator.ListEffectiveDeployments](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListEffectiveDeployments)

Arguments for `ListEffectiveDeploymentsPaginator.paginate` method:

- `coreDeviceThingName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListEffectiveDeploymentsPaginator.paginate` returns
`_PageIterator`\[[ListEffectiveDeploymentsResponseTypeDef](./type_defs.md#listeffectivedeploymentsresponsetypedef)\].

<a id="listinstalledcomponentspaginator"></a>

## ListInstalledComponentsPaginator

Type annotations for
`aiobotocore.create_client("greengrassv2").get_paginator("list_installed_components")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_greengrassv2.paginator import ListInstalledComponentsPaginator

def get_list_installed_components_paginator() -> ListInstalledComponentsPaginator:
    return Session().create_client("greengrassv2").get_paginator("list_installed_components")
```

Boto3 documentation:
[GreengrassV2.Paginator.ListInstalledComponents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#GreengrassV2.Paginator.ListInstalledComponents)

Arguments for `ListInstalledComponentsPaginator.paginate` method:

- `coreDeviceThingName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListInstalledComponentsPaginator.paginate` returns
`_PageIterator`\[[ListInstalledComponentsResponseTypeDef](./type_defs.md#listinstalledcomponentsresponsetypedef)\].
