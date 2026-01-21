# SnowDeviceManagement module

> [Index](../README.md) > SnowDeviceManagement


!!! note ""

    Auto-generated documentation for [SnowDeviceManagement](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#snowdevicemanagement)
    type annotations stubs module [types-aiobotocore-snow-device-management](https://pypi.org/project/types-aiobotocore-snow-device-management/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `SnowDeviceManagement` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `SnowDeviceManagement` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[snow-device-management]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[snow-device-management]'

# standalone installation
python -m pip install types-aiobotocore-snow-device-management
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-snow-device-management
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SnowDeviceManagementClient

Type annotations and code completion for  `#!python session.create_client("snow-device-management")` as [SnowDeviceManagementClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement.Client)

```python
# SnowDeviceManagementClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_snow_device_management.client import SnowDeviceManagementClient


session = get_session()
async with session.create_client("snow-device-management") as client:
    client: SnowDeviceManagementClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("snow-device-management").get_paginator("...")`.

```python
# ListDeviceResourcesPaginator usage example

from types_aiobotocore_snow_device_management.paginator import ListDeviceResourcesPaginator

def get_list_device_resources_paginator() -> ListDeviceResourcesPaginator:
    return client.get_paginator("list_device_resources"))
```

- [ListDeviceResourcesPaginator](./paginators.md#listdeviceresourcespaginator)
- [ListDevicesPaginator](./paginators.md#listdevicespaginator)
- [ListExecutionsPaginator](./paginators.md#listexecutionspaginator)
- [ListTasksPaginator](./paginators.md#listtaskspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AttachmentStatusType usage example

from types_aiobotocore_snow_device_management.literals import AttachmentStatusType

def get_value() -> AttachmentStatusType:
    return "ATTACHED"
```

- [AttachmentStatusType](./literals.md#attachmentstatustype)
- [ExecutionStateType](./literals.md#executionstatetype)
- [InstanceStateNameType](./literals.md#instancestatenametype)
- [IpAddressAssignmentType](./literals.md#ipaddressassignmenttype)
- [ListDeviceResourcesPaginatorName](./literals.md#listdeviceresourcespaginatorname)
- [ListDevicesPaginatorName](./literals.md#listdevicespaginatorname)
- [ListExecutionsPaginatorName](./literals.md#listexecutionspaginatorname)
- [ListTasksPaginatorName](./literals.md#listtaskspaginatorname)
- [PhysicalConnectorTypeType](./literals.md#physicalconnectortypetype)
- [TaskStateType](./literals.md#taskstatetype)
- [UnlockStateType](./literals.md#unlockstatetype)
- [SnowDeviceManagementServiceName](./literals.md#snowdevicemanagementservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [CancelTaskInputTypeDef](./type_defs.md#canceltaskinputtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CapacityTypeDef](./type_defs.md#capacitytypedef)
- [CommandTypeDef](./type_defs.md#commandtypedef)
- [CpuOptionsTypeDef](./type_defs.md#cpuoptionstypedef)
- [DescribeDeviceEc2InputTypeDef](./type_defs.md#describedeviceec2inputtypedef)
- [DescribeDeviceInputTypeDef](./type_defs.md#describedeviceinputtypedef)
- [PhysicalNetworkInterfaceTypeDef](./type_defs.md#physicalnetworkinterfacetypedef)
- [SoftwareInformationTypeDef](./type_defs.md#softwareinformationtypedef)
- [DescribeExecutionInputTypeDef](./type_defs.md#describeexecutioninputtypedef)
- [DescribeTaskInputTypeDef](./type_defs.md#describetaskinputtypedef)
- [DeviceSummaryTypeDef](./type_defs.md#devicesummarytypedef)
- [EbsInstanceBlockDeviceTypeDef](./type_defs.md#ebsinstanceblockdevicetypedef)
- [ExecutionSummaryTypeDef](./type_defs.md#executionsummarytypedef)
- [InstanceStateTypeDef](./type_defs.md#instancestatetypedef)
- [SecurityGroupIdentifierTypeDef](./type_defs.md#securitygroupidentifiertypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListDeviceResourcesInputTypeDef](./type_defs.md#listdeviceresourcesinputtypedef)
- [ResourceSummaryTypeDef](./type_defs.md#resourcesummarytypedef)
- [ListDevicesInputTypeDef](./type_defs.md#listdevicesinputtypedef)
- [ListExecutionsInputTypeDef](./type_defs.md#listexecutionsinputtypedef)
- [ListTagsForResourceInputTypeDef](./type_defs.md#listtagsforresourceinputtypedef)
- [ListTasksInputTypeDef](./type_defs.md#listtasksinputtypedef)
- [TaskSummaryTypeDef](./type_defs.md#tasksummarytypedef)
- [TagResourceInputTypeDef](./type_defs.md#tagresourceinputtypedef)
- [UntagResourceInputTypeDef](./type_defs.md#untagresourceinputtypedef)
- [CancelTaskOutputTypeDef](./type_defs.md#canceltaskoutputtypedef)
- [CreateTaskOutputTypeDef](./type_defs.md#createtaskoutputtypedef)
- [DescribeExecutionOutputTypeDef](./type_defs.md#describeexecutionoutputtypedef)
- [DescribeTaskOutputTypeDef](./type_defs.md#describetaskoutputtypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [CreateTaskInputTypeDef](./type_defs.md#createtaskinputtypedef)
- [DescribeDeviceOutputTypeDef](./type_defs.md#describedeviceoutputtypedef)
- [ListDevicesOutputTypeDef](./type_defs.md#listdevicesoutputtypedef)
- [InstanceBlockDeviceMappingTypeDef](./type_defs.md#instanceblockdevicemappingtypedef)
- [ListExecutionsOutputTypeDef](./type_defs.md#listexecutionsoutputtypedef)
- [ListDeviceResourcesInputPaginateTypeDef](./type_defs.md#listdeviceresourcesinputpaginatetypedef)
- [ListDevicesInputPaginateTypeDef](./type_defs.md#listdevicesinputpaginatetypedef)
- [ListExecutionsInputPaginateTypeDef](./type_defs.md#listexecutionsinputpaginatetypedef)
- [ListTasksInputPaginateTypeDef](./type_defs.md#listtasksinputpaginatetypedef)
- [ListDeviceResourcesOutputTypeDef](./type_defs.md#listdeviceresourcesoutputtypedef)
- [ListTasksOutputTypeDef](./type_defs.md#listtasksoutputtypedef)
- [InstanceTypeDef](./type_defs.md#instancetypedef)
- [InstanceSummaryTypeDef](./type_defs.md#instancesummarytypedef)
- [DescribeDeviceEc2OutputTypeDef](./type_defs.md#describedeviceec2outputtypedef)

