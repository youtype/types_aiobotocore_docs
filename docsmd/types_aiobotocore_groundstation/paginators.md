# Paginators

> [Index](../README.md) > [GroundStation](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [GroundStation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#groundstation)
    type annotations stubs module [types-aiobotocore-groundstation](https://pypi.org/project/types-aiobotocore-groundstation/).

## ListConfigsPaginator

Type annotations and code completion for `#!python session.create_client("groundstation").get_paginator("list_configs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation/paginator/ListConfigs.html#GroundStation.Paginator.ListConfigs)

```python
# ListConfigsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_groundstation.paginator import ListConfigsPaginator

session = get_session()
async with session.create_client("groundstation") as client:  # (1)
    paginator: ListConfigsPaginator = client.get_paginator("list_configs")  # (2)
    async for item in paginator.paginate(...):
        item: ListConfigsResponseTypeDef
        print(item)  # (3)
```

1. client: [GroundStationClient](./client.md)
2. paginator: [ListConfigsPaginator](./paginators.md#listconfigspaginator)
3. item: `AioPageIterator[ListConfigsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListConfigsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListConfigsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListConfigsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListConfigsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConfigsRequestPaginateTypeDef](./type_defs.md#listconfigsrequestpaginatetypedef)
## ListContactsPaginator

Type annotations and code completion for `#!python session.create_client("groundstation").get_paginator("list_contacts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation/paginator/ListContacts.html#GroundStation.Paginator.ListContacts)

```python
# ListContactsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_groundstation.paginator import ListContactsPaginator

session = get_session()
async with session.create_client("groundstation") as client:  # (1)
    paginator: ListContactsPaginator = client.get_paginator("list_contacts")  # (2)
    async for item in paginator.paginate(...):
        item: ListContactsResponseTypeDef
        print(item)  # (3)
```

1. client: [GroundStationClient](./client.md)
2. paginator: [ListContactsPaginator](./paginators.md#listcontactspaginator)
3. item: `AioPageIterator[ListContactsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListContactsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    statusList: Sequence[ContactStatusType],  # (1)
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    groundStation: str = ...,
    satelliteArn: str = ...,
    missionProfileArn: str = ...,
    ephemeris: EphemerisFilterTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListContactsResponseTypeDef]:  # (4)
    ...
```

1. See `Sequence[ContactStatusType]`
2. See [:material-code-braces: EphemerisFilterTypeDef](./type_defs.md#ephemerisfiltertypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListContactsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListContactsRequestPaginateTypeDef = {  # (1)
    "statusList": ...,
    "startTime": ...,
    "endTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListContactsRequestPaginateTypeDef](./type_defs.md#listcontactsrequestpaginatetypedef)
## ListDataflowEndpointGroupsPaginator

Type annotations and code completion for `#!python session.create_client("groundstation").get_paginator("list_dataflow_endpoint_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation/paginator/ListDataflowEndpointGroups.html#GroundStation.Paginator.ListDataflowEndpointGroups)

```python
# ListDataflowEndpointGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_groundstation.paginator import ListDataflowEndpointGroupsPaginator

session = get_session()
async with session.create_client("groundstation") as client:  # (1)
    paginator: ListDataflowEndpointGroupsPaginator = client.get_paginator("list_dataflow_endpoint_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListDataflowEndpointGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [GroundStationClient](./client.md)
2. paginator: [ListDataflowEndpointGroupsPaginator](./paginators.md#listdataflowendpointgroupspaginator)
3. item: `AioPageIterator[ListDataflowEndpointGroupsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDataflowEndpointGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDataflowEndpointGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDataflowEndpointGroupsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDataflowEndpointGroupsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDataflowEndpointGroupsRequestPaginateTypeDef](./type_defs.md#listdataflowendpointgroupsrequestpaginatetypedef)
## ListEphemeridesPaginator

Type annotations and code completion for `#!python session.create_client("groundstation").get_paginator("list_ephemerides")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation/paginator/ListEphemerides.html#GroundStation.Paginator.ListEphemerides)

```python
# ListEphemeridesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_groundstation.paginator import ListEphemeridesPaginator

session = get_session()
async with session.create_client("groundstation") as client:  # (1)
    paginator: ListEphemeridesPaginator = client.get_paginator("list_ephemerides")  # (2)
    async for item in paginator.paginate(...):
        item: ListEphemeridesResponseTypeDef
        print(item)  # (3)
```

1. client: [GroundStationClient](./client.md)
2. paginator: [ListEphemeridesPaginator](./paginators.md#listephemeridespaginator)
3. item: `AioPageIterator[ListEphemeridesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListEphemeridesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    startTime: TimestampTypeDef,
    endTime: TimestampTypeDef,
    satelliteId: str = ...,
    ephemerisType: EphemerisTypeType = ...,  # (1)
    statusList: Sequence[EphemerisStatusType] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListEphemeridesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: EphemerisTypeType](./literals.md#ephemeristypetype)
2. See `Sequence[EphemerisStatusType]`
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListEphemeridesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListEphemeridesRequestPaginateTypeDef = {  # (1)
    "startTime": ...,
    "endTime": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEphemeridesRequestPaginateTypeDef](./type_defs.md#listephemeridesrequestpaginatetypedef)
## ListGroundStationsPaginator

Type annotations and code completion for `#!python session.create_client("groundstation").get_paginator("list_ground_stations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation/paginator/ListGroundStations.html#GroundStation.Paginator.ListGroundStations)

```python
# ListGroundStationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_groundstation.paginator import ListGroundStationsPaginator

session = get_session()
async with session.create_client("groundstation") as client:  # (1)
    paginator: ListGroundStationsPaginator = client.get_paginator("list_ground_stations")  # (2)
    async for item in paginator.paginate(...):
        item: ListGroundStationsResponseTypeDef
        print(item)  # (3)
```

1. client: [GroundStationClient](./client.md)
2. paginator: [ListGroundStationsPaginator](./paginators.md#listgroundstationspaginator)
3. item: `AioPageIterator[ListGroundStationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListGroundStationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    satelliteId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListGroundStationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListGroundStationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListGroundStationsRequestPaginateTypeDef = {  # (1)
    "satelliteId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGroundStationsRequestPaginateTypeDef](./type_defs.md#listgroundstationsrequestpaginatetypedef)
## ListMissionProfilesPaginator

Type annotations and code completion for `#!python session.create_client("groundstation").get_paginator("list_mission_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation/paginator/ListMissionProfiles.html#GroundStation.Paginator.ListMissionProfiles)

```python
# ListMissionProfilesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_groundstation.paginator import ListMissionProfilesPaginator

session = get_session()
async with session.create_client("groundstation") as client:  # (1)
    paginator: ListMissionProfilesPaginator = client.get_paginator("list_mission_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: ListMissionProfilesResponseTypeDef
        print(item)  # (3)
```

1. client: [GroundStationClient](./client.md)
2. paginator: [ListMissionProfilesPaginator](./paginators.md#listmissionprofilespaginator)
3. item: `AioPageIterator[ListMissionProfilesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListMissionProfilesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListMissionProfilesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListMissionProfilesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListMissionProfilesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMissionProfilesRequestPaginateTypeDef](./type_defs.md#listmissionprofilesrequestpaginatetypedef)
## ListSatellitesPaginator

Type annotations and code completion for `#!python session.create_client("groundstation").get_paginator("list_satellites")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation/paginator/ListSatellites.html#GroundStation.Paginator.ListSatellites)

```python
# ListSatellitesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_groundstation.paginator import ListSatellitesPaginator

session = get_session()
async with session.create_client("groundstation") as client:  # (1)
    paginator: ListSatellitesPaginator = client.get_paginator("list_satellites")  # (2)
    async for item in paginator.paginate(...):
        item: ListSatellitesResponseTypeDef
        print(item)  # (3)
```

1. client: [GroundStationClient](./client.md)
2. paginator: [ListSatellitesPaginator](./paginators.md#listsatellitespaginator)
3. item: `AioPageIterator[ListSatellitesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSatellitesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListSatellitesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListSatellitesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSatellitesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSatellitesRequestPaginateTypeDef](./type_defs.md#listsatellitesrequestpaginatetypedef)
