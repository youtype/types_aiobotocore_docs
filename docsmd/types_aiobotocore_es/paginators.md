# Paginators

> [Index](../README.md) > [ElasticsearchService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ElasticsearchService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#elasticsearchservice)
    type annotations stubs module [types-aiobotocore-es](https://pypi.org/project/types-aiobotocore-es/).

## DescribeReservedElasticsearchInstanceOfferingsPaginator

Type annotations and code completion for `#!python session.create_client("es").get_paginator("describe_reserved_elasticsearch_instance_offerings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es/paginator/DescribeReservedElasticsearchInstanceOfferings.html#ElasticsearchService.Paginator.DescribeReservedElasticsearchInstanceOfferings)

```python
# DescribeReservedElasticsearchInstanceOfferingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_es.paginator import DescribeReservedElasticsearchInstanceOfferingsPaginator

session = get_session()
async with session.create_client("es") as client:  # (1)
    paginator: DescribeReservedElasticsearchInstanceOfferingsPaginator = client.get_paginator("describe_reserved_elasticsearch_instance_offerings")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef
        print(item)  # (3)
```

1. client: [ElasticsearchServiceClient](./client.md)
2. paginator: [DescribeReservedElasticsearchInstanceOfferingsPaginator](./paginators.md#describereservedelasticsearchinstanceofferingspaginator)
3. item: `AioPageIterator[DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeReservedElasticsearchInstanceOfferingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ReservedElasticsearchInstanceOfferingId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeReservedElasticsearchInstanceOfferingsRequestPaginateTypeDef = {  # (1)
    "ReservedElasticsearchInstanceOfferingId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReservedElasticsearchInstanceOfferingsRequestPaginateTypeDef](./type_defs.md#describereservedelasticsearchinstanceofferingsrequestpaginatetypedef)
## DescribeReservedElasticsearchInstancesPaginator

Type annotations and code completion for `#!python session.create_client("es").get_paginator("describe_reserved_elasticsearch_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es/paginator/DescribeReservedElasticsearchInstances.html#ElasticsearchService.Paginator.DescribeReservedElasticsearchInstances)

```python
# DescribeReservedElasticsearchInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_es.paginator import DescribeReservedElasticsearchInstancesPaginator

session = get_session()
async with session.create_client("es") as client:  # (1)
    paginator: DescribeReservedElasticsearchInstancesPaginator = client.get_paginator("describe_reserved_elasticsearch_instances")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeReservedElasticsearchInstancesResponseTypeDef
        print(item)  # (3)
```

1. client: [ElasticsearchServiceClient](./client.md)
2. paginator: [DescribeReservedElasticsearchInstancesPaginator](./paginators.md#describereservedelasticsearchinstancespaginator)
3. item: `AioPageIterator[DescribeReservedElasticsearchInstancesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeReservedElasticsearchInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ReservedElasticsearchInstanceId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeReservedElasticsearchInstancesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeReservedElasticsearchInstancesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeReservedElasticsearchInstancesRequestPaginateTypeDef = {  # (1)
    "ReservedElasticsearchInstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReservedElasticsearchInstancesRequestPaginateTypeDef](./type_defs.md#describereservedelasticsearchinstancesrequestpaginatetypedef)
## GetUpgradeHistoryPaginator

Type annotations and code completion for `#!python session.create_client("es").get_paginator("get_upgrade_history")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es/paginator/GetUpgradeHistory.html#ElasticsearchService.Paginator.GetUpgradeHistory)

```python
# GetUpgradeHistoryPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_es.paginator import GetUpgradeHistoryPaginator

session = get_session()
async with session.create_client("es") as client:  # (1)
    paginator: GetUpgradeHistoryPaginator = client.get_paginator("get_upgrade_history")  # (2)
    async for item in paginator.paginate(...):
        item: GetUpgradeHistoryResponseTypeDef
        print(item)  # (3)
```

1. client: [ElasticsearchServiceClient](./client.md)
2. paginator: [GetUpgradeHistoryPaginator](./paginators.md#getupgradehistorypaginator)
3. item: `AioPageIterator[GetUpgradeHistoryResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetUpgradeHistoryPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DomainName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetUpgradeHistoryResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetUpgradeHistoryResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetUpgradeHistoryRequestPaginateTypeDef = {  # (1)
    "DomainName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetUpgradeHistoryRequestPaginateTypeDef](./type_defs.md#getupgradehistoryrequestpaginatetypedef)
## ListElasticsearchInstanceTypesPaginator

Type annotations and code completion for `#!python session.create_client("es").get_paginator("list_elasticsearch_instance_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es/paginator/ListElasticsearchInstanceTypes.html#ElasticsearchService.Paginator.ListElasticsearchInstanceTypes)

```python
# ListElasticsearchInstanceTypesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_es.paginator import ListElasticsearchInstanceTypesPaginator

session = get_session()
async with session.create_client("es") as client:  # (1)
    paginator: ListElasticsearchInstanceTypesPaginator = client.get_paginator("list_elasticsearch_instance_types")  # (2)
    async for item in paginator.paginate(...):
        item: ListElasticsearchInstanceTypesResponseTypeDef
        print(item)  # (3)
```

1. client: [ElasticsearchServiceClient](./client.md)
2. paginator: [ListElasticsearchInstanceTypesPaginator](./paginators.md#listelasticsearchinstancetypespaginator)
3. item: `AioPageIterator[ListElasticsearchInstanceTypesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListElasticsearchInstanceTypesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ElasticsearchVersion: str,
    DomainName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListElasticsearchInstanceTypesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListElasticsearchInstanceTypesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListElasticsearchInstanceTypesRequestPaginateTypeDef = {  # (1)
    "ElasticsearchVersion": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListElasticsearchInstanceTypesRequestPaginateTypeDef](./type_defs.md#listelasticsearchinstancetypesrequestpaginatetypedef)
## ListElasticsearchVersionsPaginator

Type annotations and code completion for `#!python session.create_client("es").get_paginator("list_elasticsearch_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es/paginator/ListElasticsearchVersions.html#ElasticsearchService.Paginator.ListElasticsearchVersions)

```python
# ListElasticsearchVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_es.paginator import ListElasticsearchVersionsPaginator

session = get_session()
async with session.create_client("es") as client:  # (1)
    paginator: ListElasticsearchVersionsPaginator = client.get_paginator("list_elasticsearch_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListElasticsearchVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [ElasticsearchServiceClient](./client.md)
2. paginator: [ListElasticsearchVersionsPaginator](./paginators.md#listelasticsearchversionspaginator)
3. item: `AioPageIterator[ListElasticsearchVersionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListElasticsearchVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListElasticsearchVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListElasticsearchVersionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListElasticsearchVersionsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListElasticsearchVersionsRequestPaginateTypeDef](./type_defs.md#listelasticsearchversionsrequestpaginatetypedef)
