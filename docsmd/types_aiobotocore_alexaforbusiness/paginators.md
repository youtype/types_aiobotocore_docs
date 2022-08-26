# Paginators

> [Index](../README.md) > [AlexaForBusiness](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [AlexaForBusiness](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness)
    type annotations stubs module [types-aiobotocore-alexaforbusiness](https://pypi.org/project/types-aiobotocore-alexaforbusiness/).

## ListBusinessReportSchedulesPaginator

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").get_paginator("list_business_report_schedules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Paginator.ListBusinessReportSchedules)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_alexaforbusiness.paginator import ListBusinessReportSchedulesPaginator

session = get_session()
async with session.create_client("alexaforbusiness") as client:  # (1)
    paginator: ListBusinessReportSchedulesPaginator = client.get_paginator("list_business_report_schedules")  # (2)
    async for item in paginator.paginate(...):
        item: ListBusinessReportSchedulesResponseTypeDef
        print(item)  # (3)
```

1. client: [AlexaForBusinessClient](./client.md)
2. paginator: [ListBusinessReportSchedulesPaginator](./paginators.md#listbusinessreportschedulespaginator)
3. item: [:material-code-braces: ListBusinessReportSchedulesResponseTypeDef](./type_defs.md#listbusinessreportschedulesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListBusinessReportSchedulesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListBusinessReportSchedulesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListBusinessReportSchedulesResponseTypeDef](./type_defs.md#listbusinessreportschedulesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListBusinessReportSchedulesRequestListBusinessReportSchedulesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBusinessReportSchedulesRequestListBusinessReportSchedulesPaginateTypeDef](./type_defs.md#listbusinessreportschedulesrequestlistbusinessreportschedulespaginatetypedef) 
## ListConferenceProvidersPaginator

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").get_paginator("list_conference_providers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Paginator.ListConferenceProviders)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_alexaforbusiness.paginator import ListConferenceProvidersPaginator

session = get_session()
async with session.create_client("alexaforbusiness") as client:  # (1)
    paginator: ListConferenceProvidersPaginator = client.get_paginator("list_conference_providers")  # (2)
    async for item in paginator.paginate(...):
        item: ListConferenceProvidersResponseTypeDef
        print(item)  # (3)
```

1. client: [AlexaForBusinessClient](./client.md)
2. paginator: [ListConferenceProvidersPaginator](./paginators.md#listconferenceproviderspaginator)
3. item: [:material-code-braces: ListConferenceProvidersResponseTypeDef](./type_defs.md#listconferenceprovidersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListConferenceProvidersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListConferenceProvidersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListConferenceProvidersResponseTypeDef](./type_defs.md#listconferenceprovidersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListConferenceProvidersRequestListConferenceProvidersPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConferenceProvidersRequestListConferenceProvidersPaginateTypeDef](./type_defs.md#listconferenceprovidersrequestlistconferenceproviderspaginatetypedef) 
## ListDeviceEventsPaginator

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").get_paginator("list_device_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Paginator.ListDeviceEvents)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_alexaforbusiness.paginator import ListDeviceEventsPaginator

session = get_session()
async with session.create_client("alexaforbusiness") as client:  # (1)
    paginator: ListDeviceEventsPaginator = client.get_paginator("list_device_events")  # (2)
    async for item in paginator.paginate(...):
        item: ListDeviceEventsResponseTypeDef
        print(item)  # (3)
```

1. client: [AlexaForBusinessClient](./client.md)
2. paginator: [ListDeviceEventsPaginator](./paginators.md#listdeviceeventspaginator)
3. item: [:material-code-braces: ListDeviceEventsResponseTypeDef](./type_defs.md#listdeviceeventsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDeviceEventsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DeviceArn: str,
    EventType: DeviceEventTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListDeviceEventsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: DeviceEventTypeType](./literals.md#deviceeventtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDeviceEventsResponseTypeDef](./type_defs.md#listdeviceeventsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDeviceEventsRequestListDeviceEventsPaginateTypeDef = {  # (1)
    "DeviceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeviceEventsRequestListDeviceEventsPaginateTypeDef](./type_defs.md#listdeviceeventsrequestlistdeviceeventspaginatetypedef) 
## ListSkillsPaginator

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").get_paginator("list_skills")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Paginator.ListSkills)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_alexaforbusiness.paginator import ListSkillsPaginator

session = get_session()
async with session.create_client("alexaforbusiness") as client:  # (1)
    paginator: ListSkillsPaginator = client.get_paginator("list_skills")  # (2)
    async for item in paginator.paginate(...):
        item: ListSkillsResponseTypeDef
        print(item)  # (3)
```

1. client: [AlexaForBusinessClient](./client.md)
2. paginator: [ListSkillsPaginator](./paginators.md#listskillspaginator)
3. item: [:material-code-braces: ListSkillsResponseTypeDef](./type_defs.md#listskillsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSkillsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    SkillGroupArn: str = ...,
    EnablementType: EnablementTypeFilterType = ...,  # (1)
    SkillType: SkillTypeFilterType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListSkillsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: EnablementTypeFilterType](./literals.md#enablementtypefiltertype) 
2. See [:material-code-brackets: SkillTypeFilterType](./literals.md#skilltypefiltertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListSkillsResponseTypeDef](./type_defs.md#listskillsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSkillsRequestListSkillsPaginateTypeDef = {  # (1)
    "SkillGroupArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSkillsRequestListSkillsPaginateTypeDef](./type_defs.md#listskillsrequestlistskillspaginatetypedef) 
## ListSkillsStoreCategoriesPaginator

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").get_paginator("list_skills_store_categories")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Paginator.ListSkillsStoreCategories)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_alexaforbusiness.paginator import ListSkillsStoreCategoriesPaginator

session = get_session()
async with session.create_client("alexaforbusiness") as client:  # (1)
    paginator: ListSkillsStoreCategoriesPaginator = client.get_paginator("list_skills_store_categories")  # (2)
    async for item in paginator.paginate(...):
        item: ListSkillsStoreCategoriesResponseTypeDef
        print(item)  # (3)
```

1. client: [AlexaForBusinessClient](./client.md)
2. paginator: [ListSkillsStoreCategoriesPaginator](./paginators.md#listskillsstorecategoriespaginator)
3. item: [:material-code-braces: ListSkillsStoreCategoriesResponseTypeDef](./type_defs.md#listskillsstorecategoriesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSkillsStoreCategoriesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSkillsStoreCategoriesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSkillsStoreCategoriesResponseTypeDef](./type_defs.md#listskillsstorecategoriesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSkillsStoreCategoriesRequestListSkillsStoreCategoriesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSkillsStoreCategoriesRequestListSkillsStoreCategoriesPaginateTypeDef](./type_defs.md#listskillsstorecategoriesrequestlistskillsstorecategoriespaginatetypedef) 
## ListSkillsStoreSkillsByCategoryPaginator

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").get_paginator("list_skills_store_skills_by_category")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Paginator.ListSkillsStoreSkillsByCategory)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_alexaforbusiness.paginator import ListSkillsStoreSkillsByCategoryPaginator

session = get_session()
async with session.create_client("alexaforbusiness") as client:  # (1)
    paginator: ListSkillsStoreSkillsByCategoryPaginator = client.get_paginator("list_skills_store_skills_by_category")  # (2)
    async for item in paginator.paginate(...):
        item: ListSkillsStoreSkillsByCategoryResponseTypeDef
        print(item)  # (3)
```

1. client: [AlexaForBusinessClient](./client.md)
2. paginator: [ListSkillsStoreSkillsByCategoryPaginator](./paginators.md#listskillsstoreskillsbycategorypaginator)
3. item: [:material-code-braces: ListSkillsStoreSkillsByCategoryResponseTypeDef](./type_defs.md#listskillsstoreskillsbycategoryresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSkillsStoreSkillsByCategoryPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    CategoryId: int,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSkillsStoreSkillsByCategoryResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSkillsStoreSkillsByCategoryResponseTypeDef](./type_defs.md#listskillsstoreskillsbycategoryresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSkillsStoreSkillsByCategoryRequestListSkillsStoreSkillsByCategoryPaginateTypeDef = {  # (1)
    "CategoryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSkillsStoreSkillsByCategoryRequestListSkillsStoreSkillsByCategoryPaginateTypeDef](./type_defs.md#listskillsstoreskillsbycategoryrequestlistskillsstoreskillsbycategorypaginatetypedef) 
## ListSmartHomeAppliancesPaginator

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").get_paginator("list_smart_home_appliances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Paginator.ListSmartHomeAppliances)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_alexaforbusiness.paginator import ListSmartHomeAppliancesPaginator

session = get_session()
async with session.create_client("alexaforbusiness") as client:  # (1)
    paginator: ListSmartHomeAppliancesPaginator = client.get_paginator("list_smart_home_appliances")  # (2)
    async for item in paginator.paginate(...):
        item: ListSmartHomeAppliancesResponseTypeDef
        print(item)  # (3)
```

1. client: [AlexaForBusinessClient](./client.md)
2. paginator: [ListSmartHomeAppliancesPaginator](./paginators.md#listsmarthomeappliancespaginator)
3. item: [:material-code-braces: ListSmartHomeAppliancesResponseTypeDef](./type_defs.md#listsmarthomeappliancesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSmartHomeAppliancesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    RoomArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSmartHomeAppliancesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSmartHomeAppliancesResponseTypeDef](./type_defs.md#listsmarthomeappliancesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListSmartHomeAppliancesRequestListSmartHomeAppliancesPaginateTypeDef = {  # (1)
    "RoomArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSmartHomeAppliancesRequestListSmartHomeAppliancesPaginateTypeDef](./type_defs.md#listsmarthomeappliancesrequestlistsmarthomeappliancespaginatetypedef) 
## ListTagsPaginator

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").get_paginator("list_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Paginator.ListTags)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_alexaforbusiness.paginator import ListTagsPaginator

session = get_session()
async with session.create_client("alexaforbusiness") as client:  # (1)
    paginator: ListTagsPaginator = client.get_paginator("list_tags")  # (2)
    async for item in paginator.paginate(...):
        item: ListTagsResponseTypeDef
        print(item)  # (3)
```

1. client: [AlexaForBusinessClient](./client.md)
2. paginator: [ListTagsPaginator](./paginators.md#listtagspaginator)
3. item: [:material-code-braces: ListTagsResponseTypeDef](./type_defs.md#listtagsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTagsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Arn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTagsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTagsResponseTypeDef](./type_defs.md#listtagsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTagsRequestListTagsPaginateTypeDef = {  # (1)
    "Arn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsRequestListTagsPaginateTypeDef](./type_defs.md#listtagsrequestlisttagspaginatetypedef) 
## SearchDevicesPaginator

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").get_paginator("search_devices")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Paginator.SearchDevices)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_alexaforbusiness.paginator import SearchDevicesPaginator

session = get_session()
async with session.create_client("alexaforbusiness") as client:  # (1)
    paginator: SearchDevicesPaginator = client.get_paginator("search_devices")  # (2)
    async for item in paginator.paginate(...):
        item: SearchDevicesResponseTypeDef
        print(item)  # (3)
```

1. client: [AlexaForBusinessClient](./client.md)
2. paginator: [SearchDevicesPaginator](./paginators.md#searchdevicespaginator)
3. item: [:material-code-braces: SearchDevicesResponseTypeDef](./type_defs.md#searchdevicesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SearchDevicesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    SortCriteria: Sequence[SortTypeDef] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[SearchDevicesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: SearchDevicesResponseTypeDef](./type_defs.md#searchdevicesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: SearchDevicesRequestSearchDevicesPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchDevicesRequestSearchDevicesPaginateTypeDef](./type_defs.md#searchdevicesrequestsearchdevicespaginatetypedef) 
## SearchProfilesPaginator

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").get_paginator("search_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Paginator.SearchProfiles)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_alexaforbusiness.paginator import SearchProfilesPaginator

session = get_session()
async with session.create_client("alexaforbusiness") as client:  # (1)
    paginator: SearchProfilesPaginator = client.get_paginator("search_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: SearchProfilesResponseTypeDef
        print(item)  # (3)
```

1. client: [AlexaForBusinessClient](./client.md)
2. paginator: [SearchProfilesPaginator](./paginators.md#searchprofilespaginator)
3. item: [:material-code-braces: SearchProfilesResponseTypeDef](./type_defs.md#searchprofilesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SearchProfilesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    SortCriteria: Sequence[SortTypeDef] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[SearchProfilesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: SearchProfilesResponseTypeDef](./type_defs.md#searchprofilesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: SearchProfilesRequestSearchProfilesPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchProfilesRequestSearchProfilesPaginateTypeDef](./type_defs.md#searchprofilesrequestsearchprofilespaginatetypedef) 
## SearchRoomsPaginator

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").get_paginator("search_rooms")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Paginator.SearchRooms)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_alexaforbusiness.paginator import SearchRoomsPaginator

session = get_session()
async with session.create_client("alexaforbusiness") as client:  # (1)
    paginator: SearchRoomsPaginator = client.get_paginator("search_rooms")  # (2)
    async for item in paginator.paginate(...):
        item: SearchRoomsResponseTypeDef
        print(item)  # (3)
```

1. client: [AlexaForBusinessClient](./client.md)
2. paginator: [SearchRoomsPaginator](./paginators.md#searchroomspaginator)
3. item: [:material-code-braces: SearchRoomsResponseTypeDef](./type_defs.md#searchroomsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SearchRoomsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    SortCriteria: Sequence[SortTypeDef] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[SearchRoomsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: SearchRoomsResponseTypeDef](./type_defs.md#searchroomsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: SearchRoomsRequestSearchRoomsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchRoomsRequestSearchRoomsPaginateTypeDef](./type_defs.md#searchroomsrequestsearchroomspaginatetypedef) 
## SearchSkillGroupsPaginator

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").get_paginator("search_skill_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Paginator.SearchSkillGroups)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_alexaforbusiness.paginator import SearchSkillGroupsPaginator

session = get_session()
async with session.create_client("alexaforbusiness") as client:  # (1)
    paginator: SearchSkillGroupsPaginator = client.get_paginator("search_skill_groups")  # (2)
    async for item in paginator.paginate(...):
        item: SearchSkillGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [AlexaForBusinessClient](./client.md)
2. paginator: [SearchSkillGroupsPaginator](./paginators.md#searchskillgroupspaginator)
3. item: [:material-code-braces: SearchSkillGroupsResponseTypeDef](./type_defs.md#searchskillgroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SearchSkillGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    SortCriteria: Sequence[SortTypeDef] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[SearchSkillGroupsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: SearchSkillGroupsResponseTypeDef](./type_defs.md#searchskillgroupsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: SearchSkillGroupsRequestSearchSkillGroupsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchSkillGroupsRequestSearchSkillGroupsPaginateTypeDef](./type_defs.md#searchskillgroupsrequestsearchskillgroupspaginatetypedef) 
## SearchUsersPaginator

Type annotations and code completion for `#!python session.create_client("alexaforbusiness").get_paginator("search_users")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/alexaforbusiness.html#AlexaForBusiness.Paginator.SearchUsers)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_alexaforbusiness.paginator import SearchUsersPaginator

session = get_session()
async with session.create_client("alexaforbusiness") as client:  # (1)
    paginator: SearchUsersPaginator = client.get_paginator("search_users")  # (2)
    async for item in paginator.paginate(...):
        item: SearchUsersResponseTypeDef
        print(item)  # (3)
```

1. client: [AlexaForBusinessClient](./client.md)
2. paginator: [SearchUsersPaginator](./paginators.md#searchuserspaginator)
3. item: [:material-code-braces: SearchUsersResponseTypeDef](./type_defs.md#searchusersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SearchUsersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    SortCriteria: Sequence[SortTypeDef] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[SearchUsersResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: SearchUsersResponseTypeDef](./type_defs.md#searchusersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: SearchUsersRequestSearchUsersPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchUsersRequestSearchUsersPaginateTypeDef](./type_defs.md#searchusersrequestsearchuserspaginatetypedef) 
