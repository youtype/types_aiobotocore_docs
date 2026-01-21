# Paginators

> [Index](../README.md) > [Outposts](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Outposts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#outposts)
    type annotations stubs module [types-aiobotocore-outposts](https://pypi.org/project/types-aiobotocore-outposts/).

## GetOutpostBillingInformationPaginator

Type annotations and code completion for `#!python session.create_client("outposts").get_paginator("get_outpost_billing_information")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts/paginator/GetOutpostBillingInformation.html#Outposts.Paginator.GetOutpostBillingInformation)

```python
# GetOutpostBillingInformationPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_outposts.paginator import GetOutpostBillingInformationPaginator

session = get_session()
async with session.create_client("outposts") as client:  # (1)
    paginator: GetOutpostBillingInformationPaginator = client.get_paginator("get_outpost_billing_information")  # (2)
    async for item in paginator.paginate(...):
        item: GetOutpostBillingInformationOutputTypeDef
        print(item)  # (3)
```

1. client: [OutpostsClient](./client.md)
2. paginator: [GetOutpostBillingInformationPaginator](./paginators.md#getoutpostbillinginformationpaginator)
3. item: `AioPageIterator[GetOutpostBillingInformationOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python GetOutpostBillingInformationPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OutpostIdentifier: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetOutpostBillingInformationOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetOutpostBillingInformationOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetOutpostBillingInformationInputPaginateTypeDef = {  # (1)
    "OutpostIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetOutpostBillingInformationInputPaginateTypeDef](./type_defs.md#getoutpostbillinginformationinputpaginatetypedef)
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
3. item: `AioPageIterator[GetOutpostInstanceTypesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python GetOutpostInstanceTypesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OutpostId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetOutpostInstanceTypesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetOutpostInstanceTypesOutputTypeDef]`


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
3. item: `AioPageIterator[GetOutpostSupportedInstanceTypesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python GetOutpostSupportedInstanceTypesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OutpostIdentifier: str,
    OrderId: str = ...,
    AssetId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetOutpostSupportedInstanceTypesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetOutpostSupportedInstanceTypesOutputTypeDef]`


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
3. item: `AioPageIterator[ListAssetInstancesOutputTypeDef]`


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
) -> aiobotocore.paginate.AioPageIterator[ListAssetInstancesOutputTypeDef]:  # (3)
    ...
```

1. See `Sequence[AWSServiceNameType]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListAssetInstancesOutputTypeDef]`


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
3. item: `AioPageIterator[ListAssetsOutputTypeDef]`


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
) -> aiobotocore.paginate.AioPageIterator[ListAssetsOutputTypeDef]:  # (3)
    ...
```

1. See `Sequence[AssetStateType]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListAssetsOutputTypeDef]`


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
3. item: `AioPageIterator[ListBlockingInstancesForCapacityTaskOutputTypeDef]`


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
) -> aiobotocore.paginate.AioPageIterator[ListBlockingInstancesForCapacityTaskOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListBlockingInstancesForCapacityTaskOutputTypeDef]`


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
3. item: `AioPageIterator[ListCapacityTasksOutputTypeDef]`


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
) -> aiobotocore.paginate.AioPageIterator[ListCapacityTasksOutputTypeDef]:  # (3)
    ...
```

1. See `Sequence[CapacityTaskStatusType]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListCapacityTasksOutputTypeDef]`


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
3. item: `AioPageIterator[ListCatalogItemsOutputTypeDef]`


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
) -> aiobotocore.paginate.AioPageIterator[ListCatalogItemsOutputTypeDef]:  # (4)
    ...
```

1. See `Sequence[CatalogItemClassType]`
2. See `Sequence[SupportedStorageEnumType]`
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListCatalogItemsOutputTypeDef]`


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
3. item: `AioPageIterator[ListOrdersOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListOrdersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OutpostIdentifierFilter: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListOrdersOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListOrdersOutputTypeDef]`


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
3. item: `AioPageIterator[ListOutpostsOutputTypeDef]`


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
) -> aiobotocore.paginate.AioPageIterator[ListOutpostsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListOutpostsOutputTypeDef]`


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
3. item: `AioPageIterator[ListSitesOutputTypeDef]`


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
) -> aiobotocore.paginate.AioPageIterator[ListSitesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListSitesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSitesInputPaginateTypeDef = {  # (1)
    "OperatingAddressCountryCodeFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSitesInputPaginateTypeDef](./type_defs.md#listsitesinputpaginatetypedef)
