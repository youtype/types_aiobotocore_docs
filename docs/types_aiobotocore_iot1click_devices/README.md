<a id="type-annotations-for-aiobotocore-iot1clickdevicesservice-module"></a>

# Type annotations for aiobotocore IoT1ClickDevicesService module

> [Index](../README.md) > IoT1ClickDevicesService

Auto-generated documentation for
[IoT1ClickDevicesService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
type annotations stubs module
[types-aiobotocore-iot1click-devices](https://pypi.org/project/types-aiobotocore-iot1click-devices/).

- [Type annotations for aiobotocore IoT1ClickDevicesService module](#type-annotations-for-aiobotocore-iot1clickdevicesservice-module)
  - [How to install](#how-to-install)
    - [VSCode extension](#vscode-extension)
    - [From PyPI with pip](#from-pypi-with-pip)
  - [How to uninstall](#how-to-uninstall)
  - [Usage](#usage)
  - [IoT1ClickDevicesServiceClient](#iot1clickdevicesserviceclient)
    - [Methods](#methods)
    - [Exceptions](#exceptions)
  - [Paginators](#paginators)
  - [Literals](#literals)
  - [Typed dictionaries](#typed-dictionaries)

<a id="how-to-install"></a>

## How to install

<a id="vscode-extension"></a>

### VSCode extension

Add
[AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `IoT1ClickDevicesService`.

<a id="from-pypi-with-pip"></a>

### From PyPI with pip

Install `types-aiobotocore` for `IoT1ClickDevicesService` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[iot1click-devices]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[iot1click-devices]'


# standalone installation
python -m pip install types-aiobotocore-iot1click-devices
```

<a id="how-to-uninstall"></a>

## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-iot1click-devices
```

<a id="usage"></a>

## Usage

Code samples can be found [here](./usage.md).

<a id="iot1clickdevicesserviceclient"></a>

## IoT1ClickDevicesServiceClient

Type annotations for `session.create_client("iot1click-devices")` as
[IoT1ClickDevicesServiceClient](./client.md)

Can be used directly:

```python
from types_aiobotocore_iot1click_devices.client import IoT1ClickDevicesServiceClient
```

<a id="methods"></a>

### Methods

- [__aenter__](./client.md#__aenter__)
- [__aexit__](./client.md#__aexit__)
- [can_paginate](./client.md#can_paginate)
- [claim_devices_by_claim_code](./client.md#claim_devices_by_claim_code)
- [describe_device](./client.md#describe_device)
- [exceptions](./client.md#exceptions)
- [finalize_device_claim](./client.md#finalize_device_claim)
- [generate_presigned_url](./client.md#generate_presigned_url)
- [get_device_methods](./client.md#get_device_methods)
- [get_paginator](./client.md#get_paginator)
- [initiate_device_claim](./client.md#initiate_device_claim)
- [invoke_device_method](./client.md#invoke_device_method)
- [list_device_events](./client.md#list_device_events)
- [list_devices](./client.md#list_devices)
- [list_tags_for_resource](./client.md#list_tags_for_resource)
- [tag_resource](./client.md#tag_resource)
- [unclaim_device](./client.md#unclaim_device)
- [untag_resource](./client.md#untag_resource)
- [update_device_state](./client.md#update_device_state)

<a id="exceptions"></a>

### Exceptions

IoT1ClickDevicesServiceClient [exceptions](./client.md#exceptions)

- ClientError
- ForbiddenException
- InternalFailureException
- InvalidRequestException
- PreconditionFailedException
- RangeNotSatisfiableException
- ResourceConflictException
- ResourceNotFoundException

<a id="paginators"></a>

## Paginators

Type annotations for [paginators](./paginators.md) from
`boto3.client("iot1click-devices").get_paginator("...")`.

Can be used directly:

```python
from types_aiobotocore_iot1click_devices.paginator import ListDeviceEventsPaginator, ...
```

- [ListDeviceEventsPaginator](./paginators.md#listdeviceeventspaginator)
- [ListDevicesPaginator](./paginators.md#listdevicespaginator)

<a id="literals"></a>

## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

Can be used directly:

```python
from types_aiobotocore_iot1click_devices.literals import ListDeviceEventsPaginatorName, ...
```

- [ListDeviceEventsPaginatorName](./literals.md#listdeviceeventspaginatorname)
- [ListDevicesPaginatorName](./literals.md#listdevicespaginatorname)
- [IoT1ClickDevicesServiceServiceName](./literals.md#iot1clickdevicesserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)

<a id="typed-dictionaries"></a>

## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and
schema.

Can be used directly:

```python
from types_aiobotocore_iot1click_devices.type_defs import ClaimDevicesByClaimCodeRequestRequestTypeDef, ...
```

- [ClaimDevicesByClaimCodeRequestRequestTypeDef](./type_defs.md#claimdevicesbyclaimcoderequestrequesttypedef)
- [ClaimDevicesByClaimCodeResponseTypeDef](./type_defs.md#claimdevicesbyclaimcoderesponsetypedef)
- [DescribeDeviceRequestRequestTypeDef](./type_defs.md#describedevicerequestrequesttypedef)
- [DescribeDeviceResponseTypeDef](./type_defs.md#describedeviceresponsetypedef)
- [DeviceDescriptionTypeDef](./type_defs.md#devicedescriptiontypedef)
- [DeviceEventTypeDef](./type_defs.md#deviceeventtypedef)
- [DeviceMethodTypeDef](./type_defs.md#devicemethodtypedef)
- [DeviceTypeDef](./type_defs.md#devicetypedef)
- [FinalizeDeviceClaimRequestRequestTypeDef](./type_defs.md#finalizedeviceclaimrequestrequesttypedef)
- [FinalizeDeviceClaimResponseTypeDef](./type_defs.md#finalizedeviceclaimresponsetypedef)
- [GetDeviceMethodsRequestRequestTypeDef](./type_defs.md#getdevicemethodsrequestrequesttypedef)
- [GetDeviceMethodsResponseTypeDef](./type_defs.md#getdevicemethodsresponsetypedef)
- [InitiateDeviceClaimRequestRequestTypeDef](./type_defs.md#initiatedeviceclaimrequestrequesttypedef)
- [InitiateDeviceClaimResponseTypeDef](./type_defs.md#initiatedeviceclaimresponsetypedef)
- [InvokeDeviceMethodRequestRequestTypeDef](./type_defs.md#invokedevicemethodrequestrequesttypedef)
- [InvokeDeviceMethodResponseTypeDef](./type_defs.md#invokedevicemethodresponsetypedef)
- [ListDeviceEventsRequestRequestTypeDef](./type_defs.md#listdeviceeventsrequestrequesttypedef)
- [ListDeviceEventsResponseTypeDef](./type_defs.md#listdeviceeventsresponsetypedef)
- [ListDevicesRequestRequestTypeDef](./type_defs.md#listdevicesrequestrequesttypedef)
- [ListDevicesResponseTypeDef](./type_defs.md#listdevicesresponsetypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UnclaimDeviceRequestRequestTypeDef](./type_defs.md#unclaimdevicerequestrequesttypedef)
- [UnclaimDeviceResponseTypeDef](./type_defs.md#unclaimdeviceresponsetypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateDeviceStateRequestRequestTypeDef](./type_defs.md#updatedevicestaterequestrequesttypedef)