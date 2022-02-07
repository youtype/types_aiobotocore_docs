<a id="paginators-for-aiobotocore-medialive-module"></a>

# Paginators for aiobotocore MediaLive module

> [Index](..) > [MediaLive](.) > Paginators

Auto-generated documentation for
[MediaLive](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
type annotations stubs module
[types-aiobotocore-medialive](https://pypi.org/project/types-aiobotocore-medialive/).

- [Paginators for aiobotocore MediaLive module](#paginators-for-aiobotocore-medialive-module)
  - [DescribeSchedulePaginator](#describeschedulepaginator)
  - [ListChannelsPaginator](#listchannelspaginator)
  - [ListInputDeviceTransfersPaginator](#listinputdevicetransferspaginator)
  - [ListInputDevicesPaginator](#listinputdevicespaginator)
  - [ListInputSecurityGroupsPaginator](#listinputsecuritygroupspaginator)
  - [ListInputsPaginator](#listinputspaginator)
  - [ListMultiplexProgramsPaginator](#listmultiplexprogramspaginator)
  - [ListMultiplexesPaginator](#listmultiplexespaginator)
  - [ListOfferingsPaginator](#listofferingspaginator)
  - [ListReservationsPaginator](#listreservationspaginator)

<a id="describeschedulepaginator"></a>

## DescribeSchedulePaginator

Type annotations for
`session.create_client("medialive").get_paginator("describe_schedule")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import DescribeSchedulePaginator

session = get_session()
async with session.create_client("medialive") as client:
    client: MediaLiveClient
    paginator: DescribeSchedulePaginator = client.get_paginator("describe_schedule")
```

Boto3 documentation:
[MediaLive.Paginator.DescribeSchedule](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.DescribeSchedule)

Arguments for `DescribeSchedulePaginator.paginate` method:

- `ChannelId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeSchedulePaginator.paginate` returns
`_PageIterator`\[[DescribeScheduleResponseTypeDef](./type_defs.md#describescheduleresponsetypedef)\].

<a id="listchannelspaginator"></a>

## ListChannelsPaginator

Type annotations for
`session.create_client("medialive").get_paginator("list_channels")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListChannelsPaginator

session = get_session()
async with session.create_client("medialive") as client:
    client: MediaLiveClient
    paginator: ListChannelsPaginator = client.get_paginator("list_channels")
```

Boto3 documentation:
[MediaLive.Paginator.ListChannels](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListChannels)

Arguments for `ListChannelsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListChannelsPaginator.paginate` returns
`_PageIterator`\[[ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef)\].

<a id="listinputdevicetransferspaginator"></a>

## ListInputDeviceTransfersPaginator

Type annotations for
`session.create_client("medialive").get_paginator("list_input_device_transfers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListInputDeviceTransfersPaginator

session = get_session()
async with session.create_client("medialive") as client:
    client: MediaLiveClient
    paginator: ListInputDeviceTransfersPaginator = client.get_paginator("list_input_device_transfers")
```

Boto3 documentation:
[MediaLive.Paginator.ListInputDeviceTransfers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDeviceTransfers)

Arguments for `ListInputDeviceTransfersPaginator.paginate` method:

- `TransferType`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListInputDeviceTransfersPaginator.paginate` returns
`_PageIterator`\[[ListInputDeviceTransfersResponseTypeDef](./type_defs.md#listinputdevicetransfersresponsetypedef)\].

<a id="listinputdevicespaginator"></a>

## ListInputDevicesPaginator

Type annotations for
`session.create_client("medialive").get_paginator("list_input_devices")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListInputDevicesPaginator

session = get_session()
async with session.create_client("medialive") as client:
    client: MediaLiveClient
    paginator: ListInputDevicesPaginator = client.get_paginator("list_input_devices")
```

Boto3 documentation:
[MediaLive.Paginator.ListInputDevices](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDevices)

Arguments for `ListInputDevicesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListInputDevicesPaginator.paginate` returns
`_PageIterator`\[[ListInputDevicesResponseTypeDef](./type_defs.md#listinputdevicesresponsetypedef)\].

<a id="listinputsecuritygroupspaginator"></a>

## ListInputSecurityGroupsPaginator

Type annotations for
`session.create_client("medialive").get_paginator("list_input_security_groups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListInputSecurityGroupsPaginator

session = get_session()
async with session.create_client("medialive") as client:
    client: MediaLiveClient
    paginator: ListInputSecurityGroupsPaginator = client.get_paginator("list_input_security_groups")
```

Boto3 documentation:
[MediaLive.Paginator.ListInputSecurityGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputSecurityGroups)

Arguments for `ListInputSecurityGroupsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListInputSecurityGroupsPaginator.paginate` returns
`_PageIterator`\[[ListInputSecurityGroupsResponseTypeDef](./type_defs.md#listinputsecuritygroupsresponsetypedef)\].

<a id="listinputspaginator"></a>

## ListInputsPaginator

Type annotations for
`session.create_client("medialive").get_paginator("list_inputs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListInputsPaginator

session = get_session()
async with session.create_client("medialive") as client:
    client: MediaLiveClient
    paginator: ListInputsPaginator = client.get_paginator("list_inputs")
```

Boto3 documentation:
[MediaLive.Paginator.ListInputs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputs)

Arguments for `ListInputsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListInputsPaginator.paginate` returns
`_PageIterator`\[[ListInputsResponseTypeDef](./type_defs.md#listinputsresponsetypedef)\].

<a id="listmultiplexprogramspaginator"></a>

## ListMultiplexProgramsPaginator

Type annotations for
`session.create_client("medialive").get_paginator("list_multiplex_programs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListMultiplexProgramsPaginator

session = get_session()
async with session.create_client("medialive") as client:
    client: MediaLiveClient
    paginator: ListMultiplexProgramsPaginator = client.get_paginator("list_multiplex_programs")
```

Boto3 documentation:
[MediaLive.Paginator.ListMultiplexPrograms](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexPrograms)

Arguments for `ListMultiplexProgramsPaginator.paginate` method:

- `MultiplexId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListMultiplexProgramsPaginator.paginate` returns
`_PageIterator`\[[ListMultiplexProgramsResponseTypeDef](./type_defs.md#listmultiplexprogramsresponsetypedef)\].

<a id="listmultiplexespaginator"></a>

## ListMultiplexesPaginator

Type annotations for
`session.create_client("medialive").get_paginator("list_multiplexes")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListMultiplexesPaginator

session = get_session()
async with session.create_client("medialive") as client:
    client: MediaLiveClient
    paginator: ListMultiplexesPaginator = client.get_paginator("list_multiplexes")
```

Boto3 documentation:
[MediaLive.Paginator.ListMultiplexes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexes)

Arguments for `ListMultiplexesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListMultiplexesPaginator.paginate` returns
`_PageIterator`\[[ListMultiplexesResponseTypeDef](./type_defs.md#listmultiplexesresponsetypedef)\].

<a id="listofferingspaginator"></a>

## ListOfferingsPaginator

Type annotations for
`session.create_client("medialive").get_paginator("list_offerings")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListOfferingsPaginator

session = get_session()
async with session.create_client("medialive") as client:
    client: MediaLiveClient
    paginator: ListOfferingsPaginator = client.get_paginator("list_offerings")
```

Boto3 documentation:
[MediaLive.Paginator.ListOfferings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListOfferings)

Arguments for `ListOfferingsPaginator.paginate` method:

- `ChannelClass`: `str`
- `ChannelConfiguration`: `str`
- `Codec`: `str`
- `Duration`: `str`
- `MaximumBitrate`: `str`
- `MaximumFramerate`: `str`
- `Resolution`: `str`
- `ResourceType`: `str`
- `SpecialFeature`: `str`
- `VideoQuality`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListOfferingsPaginator.paginate` returns
`_PageIterator`\[[ListOfferingsResponseTypeDef](./type_defs.md#listofferingsresponsetypedef)\].

<a id="listreservationspaginator"></a>

## ListReservationsPaginator

Type annotations for
`session.create_client("medialive").get_paginator("list_reservations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListReservationsPaginator

session = get_session()
async with session.create_client("medialive") as client:
    client: MediaLiveClient
    paginator: ListReservationsPaginator = client.get_paginator("list_reservations")
```

Boto3 documentation:
[MediaLive.Paginator.ListReservations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListReservations)

Arguments for `ListReservationsPaginator.paginate` method:

- `ChannelClass`: `str`
- `Codec`: `str`
- `MaximumBitrate`: `str`
- `MaximumFramerate`: `str`
- `Resolution`: `str`
- `ResourceType`: `str`
- `SpecialFeature`: `str`
- `VideoQuality`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListReservationsPaginator.paginate` returns
`_PageIterator`\[[ListReservationsResponseTypeDef](./type_defs.md#listreservationsresponsetypedef)\].
