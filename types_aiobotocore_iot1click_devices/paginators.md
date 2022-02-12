<a id="paginators-for-aiobotocore-iot1clickdevicesservice-module"></a>

# Paginators for aiobotocore IoT1ClickDevicesService module

> [Index](..) > [IoT1ClickDevicesService](.) > Paginators

Auto-generated documentation for
[IoT1ClickDevicesService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
type annotations stubs module
[types-aiobotocore-iot1click-devices](https://pypi.org/project/types-aiobotocore-iot1click-devices/).

- [Paginators for aiobotocore IoT1ClickDevicesService module](#paginators-for-aiobotocore-iot1clickdevicesservice-module)
  - [ListDeviceEventsPaginator](#listdeviceeventspaginator)
  - [ListDevicesPaginator](#listdevicespaginator)

<a id="listdeviceeventspaginator"></a>

## ListDeviceEventsPaginator

Type annotations for
`session.create_client("iot1click-devices").get_paginator("list_device_events")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot1click_devices.paginator import ListDeviceEventsPaginator

session = get_session()
async with session.create_client("iot1click-devices") as client:
    client: IoT1ClickDevicesServiceClient
    paginator: ListDeviceEventsPaginator = client.get_paginator("list_device_events")
```

Boto3 documentation:
[IoT1ClickDevicesService.Paginator.ListDeviceEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Paginator.ListDeviceEvents)

Arguments for `ListDeviceEventsPaginator.paginate` method:

- `DeviceId`: `str` *(required)*
- `FromTimeStamp`: `Union`\[`datetime`, `str`\] *(required)*
- `ToTimeStamp`: `Union`\[`datetime`, `str`\] *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDeviceEventsPaginator.paginate` returns
`AsyncIterable`\[[ListDeviceEventsResponseTypeDef](./type_defs.md#listdeviceeventsresponsetypedef)\].

<a id="listdevicespaginator"></a>

## ListDevicesPaginator

Type annotations for
`session.create_client("iot1click-devices").get_paginator("list_devices")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot1click_devices.paginator import ListDevicesPaginator

session = get_session()
async with session.create_client("iot1click-devices") as client:
    client: IoT1ClickDevicesServiceClient
    paginator: ListDevicesPaginator = client.get_paginator("list_devices")
```

Boto3 documentation:
[IoT1ClickDevicesService.Paginator.ListDevices](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Paginator.ListDevices)

Arguments for `ListDevicesPaginator.paginate` method:

- `DeviceType`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDevicesPaginator.paginate` returns
`AsyncIterable`\[[ListDevicesResponseTypeDef](./type_defs.md#listdevicesresponsetypedef)\].
