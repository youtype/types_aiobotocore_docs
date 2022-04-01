# Paginators

> [Index](../README.md) > [ElasticsearchService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ElasticsearchService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService)
    type annotations stubs module [types-aiobotocore-es](https://pypi.org/project/types-aiobotocore-es/).

## DescribeReservedElasticsearchInstanceOfferingsPaginator

Type annotations and code completion for `#!python session.create_client("es").get_paginator("describe_reserved_elasticsearch_instance_offerings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.DescribeReservedElasticsearchInstanceOfferings)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_es.paginator import DescribeReservedElasticsearchInstanceOfferingsPaginator

session = get_session()
async with session.create_client("es") as client:
    client: ElasticsearchServiceClient
    paginator: DescribeReservedElasticsearchInstanceOfferingsPaginator = client.get_paginator("describe_reserved_elasticsearch_instance_offerings")
```


### paginate

Type annotations and code completion for `#!python DescribeReservedElasticsearchInstanceOfferingsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ReservedElasticsearchInstanceOfferingId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef](./type_defs.md#describereservedelasticsearchinstanceofferingsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef = {  # (1)
    "ReservedElasticsearchInstanceOfferingId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReservedElasticsearchInstanceOfferingsRequestDescribeReservedElasticsearchInstanceOfferingsPaginateTypeDef](./type_defs.md#describereservedelasticsearchinstanceofferingsrequestdescribereservedelasticsearchinstanceofferingspaginatetypedef) 
## DescribeReservedElasticsearchInstancesPaginator

Type annotations and code completion for `#!python session.create_client("es").get_paginator("describe_reserved_elasticsearch_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.DescribeReservedElasticsearchInstances)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_es.paginator import DescribeReservedElasticsearchInstancesPaginator

session = get_session()
async with session.create_client("es") as client:
    client: ElasticsearchServiceClient
    paginator: DescribeReservedElasticsearchInstancesPaginator = client.get_paginator("describe_reserved_elasticsearch_instances")
```


### paginate

Type annotations and code completion for `#!python DescribeReservedElasticsearchInstancesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ReservedElasticsearchInstanceId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeReservedElasticsearchInstancesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeReservedElasticsearchInstancesResponseTypeDef](./type_defs.md#describereservedelasticsearchinstancesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef = {  # (1)
    "ReservedElasticsearchInstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReservedElasticsearchInstancesRequestDescribeReservedElasticsearchInstancesPaginateTypeDef](./type_defs.md#describereservedelasticsearchinstancesrequestdescribereservedelasticsearchinstancespaginatetypedef) 
## GetUpgradeHistoryPaginator

Type annotations and code completion for `#!python session.create_client("es").get_paginator("get_upgrade_history")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.GetUpgradeHistory)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_es.paginator import GetUpgradeHistoryPaginator

session = get_session()
async with session.create_client("es") as client:
    client: ElasticsearchServiceClient
    paginator: GetUpgradeHistoryPaginator = client.get_paginator("get_upgrade_history")
```


### paginate

Type annotations and code completion for `#!python GetUpgradeHistoryPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DomainName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetUpgradeHistoryResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetUpgradeHistoryResponseTypeDef](./type_defs.md#getupgradehistoryresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef = {  # (1)
    "DomainName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetUpgradeHistoryRequestGetUpgradeHistoryPaginateTypeDef](./type_defs.md#getupgradehistoryrequestgetupgradehistorypaginatetypedef) 
## ListElasticsearchInstanceTypesPaginator

Type annotations and code completion for `#!python session.create_client("es").get_paginator("list_elasticsearch_instance_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.ListElasticsearchInstanceTypes)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_es.paginator import ListElasticsearchInstanceTypesPaginator

session = get_session()
async with session.create_client("es") as client:
    client: ElasticsearchServiceClient
    paginator: ListElasticsearchInstanceTypesPaginator = client.get_paginator("list_elasticsearch_instance_types")
```


### paginate

Type annotations and code completion for `#!python ListElasticsearchInstanceTypesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ElasticsearchVersion: str,
    DomainName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListElasticsearchInstanceTypesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListElasticsearchInstanceTypesResponseTypeDef](./type_defs.md#listelasticsearchinstancetypesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef = {  # (1)
    "ElasticsearchVersion": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListElasticsearchInstanceTypesRequestListElasticsearchInstanceTypesPaginateTypeDef](./type_defs.md#listelasticsearchinstancetypesrequestlistelasticsearchinstancetypespaginatetypedef) 
## ListElasticsearchVersionsPaginator

Type annotations and code completion for `#!python session.create_client("es").get_paginator("list_elasticsearch_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.ListElasticsearchVersions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_es.paginator import ListElasticsearchVersionsPaginator

session = get_session()
async with session.create_client("es") as client:
    client: ElasticsearchServiceClient
    paginator: ListElasticsearchVersionsPaginator = client.get_paginator("list_elasticsearch_versions")
```


### paginate

Type annotations and code completion for `#!python ListElasticsearchVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListElasticsearchVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListElasticsearchVersionsResponseTypeDef](./type_defs.md#listelasticsearchversionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListElasticsearchVersionsRequestListElasticsearchVersionsPaginateTypeDef](./type_defs.md#listelasticsearchversionsrequestlistelasticsearchversionspaginatetypedef) 
