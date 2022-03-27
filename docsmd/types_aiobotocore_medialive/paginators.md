# Paginators

> [Index](../README.md) > [MediaLive](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MediaLive](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
    type annotations stubs module [types-aiobotocore-medialive](https://pypi.org/project/types-aiobotocore-medialive/).

## DescribeSchedulePaginator

Type annotations and code completion for `#!python session.create_client("medialive").get_paginator("describe_schedule")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.DescribeSchedule)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import DescribeSchedulePaginator

session = get_session()
async with session.create_client("medialive") as client:
    client: MediaLiveClient
    paginator: DescribeSchedulePaginator = client.get_paginator("describe_schedule")
```


### paginate

Type annotations and code completion for `#!python DescribeSchedulePaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ChannelId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeScheduleResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeScheduleResponseTypeDef](./type_defs.md#describescheduleresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeScheduleRequestDescribeSchedulePaginateTypeDef = {  # (1)
    "ChannelId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeScheduleRequestDescribeSchedulePaginateTypeDef](./type_defs.md#describeschedulerequestdescribeschedulepaginatetypedef) 
## ListChannelsPaginator

Type annotations and code completion for `#!python session.create_client("medialive").get_paginator("list_channels")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListChannels)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListChannelsPaginator

session = get_session()
async with session.create_client("medialive") as client:
    client: MediaLiveClient
    paginator: ListChannelsPaginator = client.get_paginator("list_channels")
```


### paginate

Type annotations and code completion for `#!python ListChannelsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListChannelsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListChannelsRequestListChannelsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListChannelsRequestListChannelsPaginateTypeDef](./type_defs.md#listchannelsrequestlistchannelspaginatetypedef) 
## ListInputDeviceTransfersPaginator

Type annotations and code completion for `#!python session.create_client("medialive").get_paginator("list_input_device_transfers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDeviceTransfers)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListInputDeviceTransfersPaginator

session = get_session()
async with session.create_client("medialive") as client:
    client: MediaLiveClient
    paginator: ListInputDeviceTransfersPaginator = client.get_paginator("list_input_device_transfers")
```


### paginate

Type annotations and code completion for `#!python ListInputDeviceTransfersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TransferType: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListInputDeviceTransfersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListInputDeviceTransfersResponseTypeDef](./type_defs.md#listinputdevicetransfersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef = {  # (1)
    "TransferType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInputDeviceTransfersRequestListInputDeviceTransfersPaginateTypeDef](./type_defs.md#listinputdevicetransfersrequestlistinputdevicetransferspaginatetypedef) 
## ListInputDevicesPaginator

Type annotations and code completion for `#!python session.create_client("medialive").get_paginator("list_input_devices")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputDevices)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListInputDevicesPaginator

session = get_session()
async with session.create_client("medialive") as client:
    client: MediaLiveClient
    paginator: ListInputDevicesPaginator = client.get_paginator("list_input_devices")
```


### paginate

Type annotations and code completion for `#!python ListInputDevicesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListInputDevicesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListInputDevicesResponseTypeDef](./type_defs.md#listinputdevicesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListInputDevicesRequestListInputDevicesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInputDevicesRequestListInputDevicesPaginateTypeDef](./type_defs.md#listinputdevicesrequestlistinputdevicespaginatetypedef) 
## ListInputSecurityGroupsPaginator

Type annotations and code completion for `#!python session.create_client("medialive").get_paginator("list_input_security_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputSecurityGroups)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListInputSecurityGroupsPaginator

session = get_session()
async with session.create_client("medialive") as client:
    client: MediaLiveClient
    paginator: ListInputSecurityGroupsPaginator = client.get_paginator("list_input_security_groups")
```


### paginate

Type annotations and code completion for `#!python ListInputSecurityGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListInputSecurityGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListInputSecurityGroupsResponseTypeDef](./type_defs.md#listinputsecuritygroupsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInputSecurityGroupsRequestListInputSecurityGroupsPaginateTypeDef](./type_defs.md#listinputsecuritygroupsrequestlistinputsecuritygroupspaginatetypedef) 
## ListInputsPaginator

Type annotations and code completion for `#!python session.create_client("medialive").get_paginator("list_inputs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListInputs)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListInputsPaginator

session = get_session()
async with session.create_client("medialive") as client:
    client: MediaLiveClient
    paginator: ListInputsPaginator = client.get_paginator("list_inputs")
```


### paginate

Type annotations and code completion for `#!python ListInputsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListInputsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListInputsResponseTypeDef](./type_defs.md#listinputsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListInputsRequestListInputsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInputsRequestListInputsPaginateTypeDef](./type_defs.md#listinputsrequestlistinputspaginatetypedef) 
## ListMultiplexProgramsPaginator

Type annotations and code completion for `#!python session.create_client("medialive").get_paginator("list_multiplex_programs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexPrograms)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListMultiplexProgramsPaginator

session = get_session()
async with session.create_client("medialive") as client:
    client: MediaLiveClient
    paginator: ListMultiplexProgramsPaginator = client.get_paginator("list_multiplex_programs")
```


### paginate

Type annotations and code completion for `#!python ListMultiplexProgramsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    MultiplexId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListMultiplexProgramsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMultiplexProgramsResponseTypeDef](./type_defs.md#listmultiplexprogramsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef = {  # (1)
    "MultiplexId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMultiplexProgramsRequestListMultiplexProgramsPaginateTypeDef](./type_defs.md#listmultiplexprogramsrequestlistmultiplexprogramspaginatetypedef) 
## ListMultiplexesPaginator

Type annotations and code completion for `#!python session.create_client("medialive").get_paginator("list_multiplexes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListMultiplexes)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListMultiplexesPaginator

session = get_session()
async with session.create_client("medialive") as client:
    client: MediaLiveClient
    paginator: ListMultiplexesPaginator = client.get_paginator("list_multiplexes")
```


### paginate

Type annotations and code completion for `#!python ListMultiplexesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListMultiplexesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMultiplexesResponseTypeDef](./type_defs.md#listmultiplexesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListMultiplexesRequestListMultiplexesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMultiplexesRequestListMultiplexesPaginateTypeDef](./type_defs.md#listmultiplexesrequestlistmultiplexespaginatetypedef) 
## ListOfferingsPaginator

Type annotations and code completion for `#!python session.create_client("medialive").get_paginator("list_offerings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListOfferings)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListOfferingsPaginator

session = get_session()
async with session.create_client("medialive") as client:
    client: MediaLiveClient
    paginator: ListOfferingsPaginator = client.get_paginator("list_offerings")
```


### paginate

Type annotations and code completion for `#!python ListOfferingsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ChannelClass: str = ...,
    ChannelConfiguration: str = ...,
    Codec: str = ...,
    Duration: str = ...,
    MaximumBitrate: str = ...,
    MaximumFramerate: str = ...,
    Resolution: str = ...,
    ResourceType: str = ...,
    SpecialFeature: str = ...,
    VideoQuality: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListOfferingsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListOfferingsResponseTypeDef](./type_defs.md#listofferingsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListOfferingsRequestListOfferingsPaginateTypeDef = {  # (1)
    "ChannelClass": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOfferingsRequestListOfferingsPaginateTypeDef](./type_defs.md#listofferingsrequestlistofferingspaginatetypedef) 
## ListReservationsPaginator

Type annotations and code completion for `#!python session.create_client("medialive").get_paginator("list_reservations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Paginator.ListReservations)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_medialive.paginator import ListReservationsPaginator

session = get_session()
async with session.create_client("medialive") as client:
    client: MediaLiveClient
    paginator: ListReservationsPaginator = client.get_paginator("list_reservations")
```


### paginate

Type annotations and code completion for `#!python ListReservationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ChannelClass: str = ...,
    Codec: str = ...,
    MaximumBitrate: str = ...,
    MaximumFramerate: str = ...,
    Resolution: str = ...,
    ResourceType: str = ...,
    SpecialFeature: str = ...,
    VideoQuality: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListReservationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListReservationsResponseTypeDef](./type_defs.md#listreservationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListReservationsRequestListReservationsPaginateTypeDef = {  # (1)
    "ChannelClass": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListReservationsRequestListReservationsPaginateTypeDef](./type_defs.md#listreservationsrequestlistreservationspaginatetypedef) 
