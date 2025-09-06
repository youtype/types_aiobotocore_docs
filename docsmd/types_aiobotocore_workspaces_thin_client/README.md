# WorkSpacesThinClient module

> [Index](../README.md) > WorkSpacesThinClient


!!! note ""

    Auto-generated documentation for [WorkSpacesThinClient](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#workspacesthinclient)
    type annotations stubs module [types-aiobotocore-workspaces-thin-client](https://pypi.org/project/types-aiobotocore-workspaces-thin-client/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.24.2' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `WorkSpacesThinClient` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `WorkSpacesThinClient` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[workspaces-thin-client]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[workspaces-thin-client]'

# standalone installation
python -m pip install types-aiobotocore-workspaces-thin-client
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-workspaces-thin-client
```

## Usage

Code samples can be found in [Examples](./usage.md).

## WorkSpacesThinClientClient

Type annotations and code completion for  `#!python session.create_client("workspaces-thin-client")` as [WorkSpacesThinClientClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#WorkSpacesThinClient.Client)

```python
# WorkSpacesThinClientClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_workspaces_thin_client.client import WorkSpacesThinClientClient


session = get_session()
async with session.create_client("workspaces-thin-client") as client:
    client: WorkSpacesThinClientClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("workspaces-thin-client").get_paginator("...")`.

```python
# ListDevicesPaginator usage example

from types_aiobotocore_workspaces_thin_client.paginator import ListDevicesPaginator

def get_list_devices_paginator() -> ListDevicesPaginator:
    return client.get_paginator("list_devices"))
```

- [ListDevicesPaginator](./paginators.md#listdevicespaginator)
- [ListEnvironmentsPaginator](./paginators.md#listenvironmentspaginator)
- [ListSoftwareSetsPaginator](./paginators.md#listsoftwaresetspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ApplyTimeOfType usage example

from types_aiobotocore_workspaces_thin_client.literals import ApplyTimeOfType

def get_value() -> ApplyTimeOfType:
    return "DEVICE"
```

- [ApplyTimeOfType](./literals.md#applytimeoftype)
- [DayOfWeekType](./literals.md#dayofweektype)
- [DesktopTypeType](./literals.md#desktoptypetype)
- [DeviceSoftwareSetComplianceStatusType](./literals.md#devicesoftwaresetcompliancestatustype)
- [DeviceStatusType](./literals.md#devicestatustype)
- [EnvironmentSoftwareSetComplianceStatusType](./literals.md#environmentsoftwaresetcompliancestatustype)
- [ListDevicesPaginatorName](./literals.md#listdevicespaginatorname)
- [ListEnvironmentsPaginatorName](./literals.md#listenvironmentspaginatorname)
- [ListSoftwareSetsPaginatorName](./literals.md#listsoftwaresetspaginatorname)
- [MaintenanceWindowTypeType](./literals.md#maintenancewindowtypetype)
- [SoftwareSetUpdateModeType](./literals.md#softwaresetupdatemodetype)
- [SoftwareSetUpdateScheduleType](./literals.md#softwaresetupdatescheduletype)
- [SoftwareSetUpdateStatusType](./literals.md#softwaresetupdatestatustype)
- [SoftwareSetValidationStatusType](./literals.md#softwaresetvalidationstatustype)
- [TargetDeviceStatusType](./literals.md#targetdevicestatustype)
- [WorkSpacesThinClientServiceName](./literals.md#workspacesthinclientservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteDeviceRequestTypeDef](./type_defs.md#deletedevicerequesttypedef)
- [DeleteEnvironmentRequestTypeDef](./type_defs.md#deleteenvironmentrequesttypedef)
- [DeregisterDeviceRequestTypeDef](./type_defs.md#deregisterdevicerequesttypedef)
- [DeviceSummaryTypeDef](./type_defs.md#devicesummarytypedef)
- [DeviceTypeDef](./type_defs.md#devicetypedef)
- [MaintenanceWindowOutputTypeDef](./type_defs.md#maintenancewindowoutputtypedef)
- [GetDeviceRequestTypeDef](./type_defs.md#getdevicerequesttypedef)
- [GetEnvironmentRequestTypeDef](./type_defs.md#getenvironmentrequesttypedef)
- [GetSoftwareSetRequestTypeDef](./type_defs.md#getsoftwaresetrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListDevicesRequestTypeDef](./type_defs.md#listdevicesrequesttypedef)
- [ListEnvironmentsRequestTypeDef](./type_defs.md#listenvironmentsrequesttypedef)
- [ListSoftwareSetsRequestTypeDef](./type_defs.md#listsoftwaresetsrequesttypedef)
- [SoftwareSetSummaryTypeDef](./type_defs.md#softwaresetsummarytypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [MaintenanceWindowTypeDef](./type_defs.md#maintenancewindowtypedef)
- [SoftwareTypeDef](./type_defs.md#softwaretypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdateDeviceRequestTypeDef](./type_defs.md#updatedevicerequesttypedef)
- [UpdateSoftwareSetRequestTypeDef](./type_defs.md#updatesoftwaresetrequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ListDevicesResponseTypeDef](./type_defs.md#listdevicesresponsetypedef)
- [UpdateDeviceResponseTypeDef](./type_defs.md#updatedeviceresponsetypedef)
- [GetDeviceResponseTypeDef](./type_defs.md#getdeviceresponsetypedef)
- [EnvironmentSummaryTypeDef](./type_defs.md#environmentsummarytypedef)
- [EnvironmentTypeDef](./type_defs.md#environmenttypedef)
- [ListDevicesRequestPaginateTypeDef](./type_defs.md#listdevicesrequestpaginatetypedef)
- [ListEnvironmentsRequestPaginateTypeDef](./type_defs.md#listenvironmentsrequestpaginatetypedef)
- [ListSoftwareSetsRequestPaginateTypeDef](./type_defs.md#listsoftwaresetsrequestpaginatetypedef)
- [ListSoftwareSetsResponseTypeDef](./type_defs.md#listsoftwaresetsresponsetypedef)
- [MaintenanceWindowUnionTypeDef](./type_defs.md#maintenancewindowuniontypedef)
- [SoftwareSetTypeDef](./type_defs.md#softwaresettypedef)
- [CreateEnvironmentResponseTypeDef](./type_defs.md#createenvironmentresponsetypedef)
- [ListEnvironmentsResponseTypeDef](./type_defs.md#listenvironmentsresponsetypedef)
- [UpdateEnvironmentResponseTypeDef](./type_defs.md#updateenvironmentresponsetypedef)
- [GetEnvironmentResponseTypeDef](./type_defs.md#getenvironmentresponsetypedef)
- [CreateEnvironmentRequestTypeDef](./type_defs.md#createenvironmentrequesttypedef)
- [UpdateEnvironmentRequestTypeDef](./type_defs.md#updateenvironmentrequesttypedef)
- [GetSoftwareSetResponseTypeDef](./type_defs.md#getsoftwaresetresponsetypedef)

