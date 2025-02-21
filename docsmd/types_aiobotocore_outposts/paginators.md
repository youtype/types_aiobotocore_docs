# Paginators

> [Index](../README.md) > [Outposts](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Outposts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#outposts)
    type annotations stubs module [types-aiobotocore-outposts](https://pypi.org/project/types-aiobotocore-outposts/).

## GetOutpostInstanceTypesPaginator

Type annotations and code completion for `#!python session.create_client("outposts").get_paginator("get_outpost_instance_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts/paginator/GetOutpostInstanceTypes.html#Outposts.Paginator.GetOutpostInstanceTypes)

```python
# GetOutpostInstanceTypesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_outposts.paginator import GetOutpostInstanceTypesPaginator

session = get_session()
async with session.create_client("outposts") as client:  # (1)
    paginator: GetOutpostInstanceTypesPaginator = client.get_paginator("get_outpost_instance_types")  # (2)
    async for item in paginator.paginate(...):
        item: GetOutpostInstanceTypesOutputTypeDef
        print(item)  # (3)
```

1. client: [OutpostsClient](./client.md)
2. paginator: [GetOutpostInstanceTypesPaginator](./paginators.md#getoutpostinstancetypespaginator)
3. item: [:material-code-braces: GetOutpostInstanceTypesOutputTypeDef](./type_defs.md#getoutpostinstancetypesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python GetOutpostInstanceTypesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OutpostId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetOutpostInstanceTypesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetOutpostInstanceTypesOutputTypeDef](./type_defs.md#getoutpostinstancetypesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetOutpostInstanceTypesInputPaginateTypeDef = {  # (1)
    "OutpostId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetOutpostInstanceTypesInputPaginateTypeDef](./type_defs.md#getoutpostinstancetypesinputpaginatetypedef) 
## GetOutpostSupportedInstanceTypesPaginator

Type annotations and code completion for `#!python session.create_client("outposts").get_paginator("get_outpost_supported_instance_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts/paginator/GetOutpostSupportedInstanceTypes.html#Outposts.Paginator.GetOutpostSupportedInstanceTypes)

```python
# GetOutpostSupportedInstanceTypesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_outposts.paginator import GetOutpostSupportedInstanceTypesPaginator

session = get_session()
async with session.create_client("outposts") as client:  # (1)
    paginator: GetOutpostSupportedInstanceTypesPaginator = client.get_paginator("get_outpost_supported_instance_types")  # (2)
    async for item in paginator.paginate(...):
        item: GetOutpostSupportedInstanceTypesOutputTypeDef
        print(item)  # (3)
```

1. client: [OutpostsClient](./client.md)
2. paginator: [GetOutpostSupportedInstanceTypesPaginator](./paginators.md#getoutpostsupportedinstancetypespaginator)
3. item: [:material-code-braces: GetOutpostSupportedInstanceTypesOutputTypeDef](./type_defs.md#getoutpostsupportedinstancetypesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python GetOutpostSupportedInstanceTypesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OutpostIdentifier: str,
    OrderId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetOutpostSupportedInstanceTypesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetOutpostSupportedInstanceTypesOutputTypeDef](./type_defs.md#getoutpostsupportedinstancetypesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetOutpostSupportedInstanceTypesInputPaginateTypeDef = {  # (1)
    "OutpostIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetOutpostSupportedInstanceTypesInputPaginateTypeDef](./type_defs.md#getoutpostsupportedinstancetypesinputpaginatetypedef) 
## ListAssetInstancesPaginator

Type annotations and code completion for `#!python session.create_client("outposts").get_paginator("list_asset_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts/paginator/ListAssetInstances.html#Outposts.Paginator.ListAssetInstances)

```python
# ListAssetInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_outposts.paginator import ListAssetInstancesPaginator

session = get_session()
async with session.create_client("outposts") as client:  # (1)
    paginator: ListAssetInstancesPaginator = client.get_paginator("list_asset_instances")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssetInstancesOutputTypeDef
        print(item)  # (3)
```

1. client: [OutpostsClient](./client.md)
2. paginator: [ListAssetInstancesPaginator](./paginators.md#listassetinstancespaginator)
3. item: [:material-code-braces: ListAssetInstancesOutputTypeDef](./type_defs.md#listassetinstancesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListAssetInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OutpostIdentifier: str,
    AssetIdFilter: Sequence[str] = ...,
    InstanceTypeFilter: Sequence[str] = ...,
    AccountIdFilter: Sequence[str] = ...,
    AwsServiceFilter: Sequence[AWSServiceNameType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListAssetInstancesOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: AWSServiceNameType](./literals.md#awsservicenametype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAssetInstancesOutputTypeDef](./type_defs.md#listassetinstancesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAssetInstancesInputPaginateTypeDef = {  # (1)
    "OutpostIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssetInstancesInputPaginateTypeDef](./type_defs.md#listassetinstancesinputpaginatetypedef) 
## ListAssetsPaginator

Type annotations and code completion for `#!python session.create_client("outposts").get_paginator("list_assets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts/paginator/ListAssets.html#Outposts.Paginator.ListAssets)

```python
# ListAssetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_outposts.paginator import ListAssetsPaginator

session = get_session()
async with session.create_client("outposts") as client:  # (1)
    paginator: ListAssetsPaginator = client.get_paginator("list_assets")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssetsOutputTypeDef
        print(item)  # (3)
```

1. client: [OutpostsClient](./client.md)
2. paginator: [ListAssetsPaginator](./paginators.md#listassetspaginator)
3. item: [:material-code-braces: ListAssetsOutputTypeDef](./type_defs.md#listassetsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListAssetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OutpostIdentifier: str,
    HostIdFilter: Sequence[str] = ...,
    StatusFilter: Sequence[AssetStateType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListAssetsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: AssetStateType](./literals.md#assetstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAssetsOutputTypeDef](./type_defs.md#listassetsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAssetsInputPaginateTypeDef = {  # (1)
    "OutpostIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssetsInputPaginateTypeDef](./type_defs.md#listassetsinputpaginatetypedef) 
## ListBlockingInstancesForCapacityTaskPaginator

Type annotations and code completion for `#!python session.create_client("outposts").get_paginator("list_blocking_instances_for_capacity_task")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts/paginator/ListBlockingInstancesForCapacityTask.html#Outposts.Paginator.ListBlockingInstancesForCapacityTask)

```python
# ListBlockingInstancesForCapacityTaskPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_outposts.paginator import ListBlockingInstancesForCapacityTaskPaginator

session = get_session()
async with session.create_client("outposts") as client:  # (1)
    paginator: ListBlockingInstancesForCapacityTaskPaginator = client.get_paginator("list_blocking_instances_for_capacity_task")  # (2)
    async for item in paginator.paginate(...):
        item: ListBlockingInstancesForCapacityTaskOutputTypeDef
        print(item)  # (3)
```

1. client: [OutpostsClient](./client.md)
2. paginator: [ListBlockingInstancesForCapacityTaskPaginator](./paginators.md#listblockinginstancesforcapacitytaskpaginator)
3. item: [:material-code-braces: ListBlockingInstancesForCapacityTaskOutputTypeDef](./type_defs.md#listblockinginstancesforcapacitytaskoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListBlockingInstancesForCapacityTaskPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OutpostIdentifier: str,
    CapacityTaskId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListBlockingInstancesForCapacityTaskOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListBlockingInstancesForCapacityTaskOutputTypeDef](./type_defs.md#listblockinginstancesforcapacitytaskoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListBlockingInstancesForCapacityTaskInputPaginateTypeDef = {  # (1)
    "OutpostIdentifier": ...,
    "CapacityTaskId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBlockingInstancesForCapacityTaskInputPaginateTypeDef](./type_defs.md#listblockinginstancesforcapacitytaskinputpaginatetypedef) 
## ListCapacityTasksPaginator

Type annotations and code completion for `#!python session.create_client("outposts").get_paginator("list_capacity_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts/paginator/ListCapacityTasks.html#Outposts.Paginator.ListCapacityTasks)

```python
# ListCapacityTasksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_outposts.paginator import ListCapacityTasksPaginator

session = get_session()
async with session.create_client("outposts") as client:  # (1)
    paginator: ListCapacityTasksPaginator = client.get_paginator("list_capacity_tasks")  # (2)
    async for item in paginator.paginate(...):
        item: ListCapacityTasksOutputTypeDef
        print(item)  # (3)
```

1. client: [OutpostsClient](./client.md)
2. paginator: [ListCapacityTasksPaginator](./paginators.md#listcapacitytaskspaginator)
3. item: [:material-code-braces: ListCapacityTasksOutputTypeDef](./type_defs.md#listcapacitytasksoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListCapacityTasksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OutpostIdentifierFilter: str = ...,
    CapacityTaskStatusFilter: Sequence[CapacityTaskStatusType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListCapacityTasksOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: CapacityTaskStatusType](./literals.md#capacitytaskstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListCapacityTasksOutputTypeDef](./type_defs.md#listcapacitytasksoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCapacityTasksInputPaginateTypeDef = {  # (1)
    "OutpostIdentifierFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCapacityTasksInputPaginateTypeDef](./type_defs.md#listcapacitytasksinputpaginatetypedef) 
## ListCatalogItemsPaginator

Type annotations and code completion for `#!python session.create_client("outposts").get_paginator("list_catalog_items")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts/paginator/ListCatalogItems.html#Outposts.Paginator.ListCatalogItems)

```python
# ListCatalogItemsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_outposts.paginator import ListCatalogItemsPaginator

session = get_session()
async with session.create_client("outposts") as client:  # (1)
    paginator: ListCatalogItemsPaginator = client.get_paginator("list_catalog_items")  # (2)
    async for item in paginator.paginate(...):
        item: ListCatalogItemsOutputTypeDef
        print(item)  # (3)
```

1. client: [OutpostsClient](./client.md)
2. paginator: [ListCatalogItemsPaginator](./paginators.md#listcatalogitemspaginator)
3. item: [:material-code-braces: ListCatalogItemsOutputTypeDef](./type_defs.md#listcatalogitemsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListCatalogItemsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ItemClassFilter: Sequence[CatalogItemClassType] = ...,  # (1)
    SupportedStorageFilter: Sequence[SupportedStorageEnumType] = ...,  # (2)
    EC2FamilyFilter: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListCatalogItemsOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: CatalogItemClassType](./literals.md#catalogitemclasstype) 
2. See [:material-code-brackets: SupportedStorageEnumType](./literals.md#supportedstorageenumtype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListCatalogItemsOutputTypeDef](./type_defs.md#listcatalogitemsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCatalogItemsInputPaginateTypeDef = {  # (1)
    "ItemClassFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCatalogItemsInputPaginateTypeDef](./type_defs.md#listcatalogitemsinputpaginatetypedef) 
## ListOrdersPaginator

Type annotations and code completion for `#!python session.create_client("outposts").get_paginator("list_orders")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts/paginator/ListOrders.html#Outposts.Paginator.ListOrders)

```python
# ListOrdersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_outposts.paginator import ListOrdersPaginator

session = get_session()
async with session.create_client("outposts") as client:  # (1)
    paginator: ListOrdersPaginator = client.get_paginator("list_orders")  # (2)
    async for item in paginator.paginate(...):
        item: ListOrdersOutputTypeDef
        print(item)  # (3)
```

1. client: [OutpostsClient](./client.md)
2. paginator: [ListOrdersPaginator](./paginators.md#listorderspaginator)
3. item: [:material-code-braces: ListOrdersOutputTypeDef](./type_defs.md#listordersoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListOrdersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OutpostIdentifierFilter: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListOrdersOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListOrdersOutputTypeDef](./type_defs.md#listordersoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListOrdersInputPaginateTypeDef = {  # (1)
    "OutpostIdentifierFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOrdersInputPaginateTypeDef](./type_defs.md#listordersinputpaginatetypedef) 
## ListOutpostsPaginator

Type annotations and code completion for `#!python session.create_client("outposts").get_paginator("list_outposts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts/paginator/ListOutposts.html#Outposts.Paginator.ListOutposts)

```python
# ListOutpostsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_outposts.paginator import ListOutpostsPaginator

session = get_session()
async with session.create_client("outposts") as client:  # (1)
    paginator: ListOutpostsPaginator = client.get_paginator("list_outposts")  # (2)
    async for item in paginator.paginate(...):
        item: ListOutpostsOutputTypeDef
        print(item)  # (3)
```

1. client: [OutpostsClient](./client.md)
2. paginator: [ListOutpostsPaginator](./paginators.md#listoutpostspaginator)
3. item: [:material-code-braces: ListOutpostsOutputTypeDef](./type_defs.md#listoutpostsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListOutpostsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    LifeCycleStatusFilter: Sequence[str] = ...,
    AvailabilityZoneFilter: Sequence[str] = ...,
    AvailabilityZoneIdFilter: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListOutpostsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListOutpostsOutputTypeDef](./type_defs.md#listoutpostsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListOutpostsInputPaginateTypeDef = {  # (1)
    "LifeCycleStatusFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOutpostsInputPaginateTypeDef](./type_defs.md#listoutpostsinputpaginatetypedef) 
## ListSitesPaginator

Type annotations and code completion for `#!python session.create_client("outposts").get_paginator("list_sites")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts/paginator/ListSites.html#Outposts.Paginator.ListSites)

```python
# ListSitesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_outposts.paginator import ListSitesPaginator

session = get_session()
async with session.create_client("outposts") as client:  # (1)
    paginator: ListSitesPaginator = client.get_paginator("list_sites")  # (2)
    async for item in paginator.paginate(...):
        item: ListSitesOutputTypeDef
        print(item)  # (3)
```

1. client: [OutpostsClient](./client.md)
2. paginator: [ListSitesPaginator](./paginators.md#listsitespaginator)
3. item: [:material-code-braces: ListSitesOutputTypeDef](./type_defs.md#listsitesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListSitesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OperatingAddressCountryCodeFilter: Sequence[str] = ...,
    OperatingAddressStateOrRegionFilter: Sequence[str] = ...,
    OperatingAddressCityFilter: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSitesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSitesOutputTypeDef](./type_defs.md#listsitesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSitesInputPaginateTypeDef = {  # (1)
    "OperatingAddressCountryCodeFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSitesInputPaginateTypeDef](./type_defs.md#listsitesinputpaginatetypedef) 
