# Paginators

> [Index](../README.md) > [IoT1ClickDevicesService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [IoT1ClickDevicesService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
    type annotations stubs module [types-aiobotocore-iot1click-devices](https://pypi.org/project/types-aiobotocore-iot1click-devices/).

## ListDeviceEventsPaginator

Type annotations and code completion for `#!python session.create_client("iot1click-devices").get_paginator("list_device_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Paginator.ListDeviceEvents)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_iot1click_devices.paginator import ListDeviceEventsPaginator

session = get_session()
async with session.create_client("iot1click-devices") as client:
    client: IoT1ClickDevicesServiceClient
    paginator: ListDeviceEventsPaginator = client.get_paginator("list_device_events")
```


### paginate

Type annotations and code completion for `#!python ListDeviceEventsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DeviceId: str,
    FromTimeStamp: Union[datetime, str],
    ToTimeStamp: Union[datetime, str],
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDeviceEventsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDeviceEventsResponseTypeDef](./type_defs.md#listdeviceeventsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDeviceEventsRequestListDeviceEventsPaginateTypeDef = {  # (1)
    "DeviceId": ...,
    "FromTimeStamp": ...,
    "ToTimeStamp": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeviceEventsRequestListDeviceEventsPaginateTypeDef](./type_defs.md#listdeviceeventsrequestlistdeviceeventspaginatetypedef) 
## ListDevicesPaginator

Type annotations and code completion for `#!python session.create_client("iot1click-devices").get_paginator("list_devices")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Paginator.ListDevices)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_iot1click_devices.paginator import ListDevicesPaginator

session = get_session()
async with session.create_client("iot1click-devices") as client:
    client: IoT1ClickDevicesServiceClient
    paginator: ListDevicesPaginator = client.get_paginator("list_devices")
```


### paginate

Type annotations and code completion for `#!python ListDevicesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DeviceType: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDevicesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDevicesResponseTypeDef](./type_defs.md#listdevicesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDevicesRequestListDevicesPaginateTypeDef = {  # (1)
    "DeviceType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDevicesRequestListDevicesPaginateTypeDef](./type_defs.md#listdevicesrequestlistdevicespaginatetypedef) 
