<a id="paginators-for-aiobotocore-elasticsearchservice-module"></a>

# Paginators for aiobotocore ElasticsearchService module

> [Index](..) > [ElasticsearchService](.) > Paginators

Auto-generated documentation for
[ElasticsearchService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService)
type annotations stubs module
[types-aiobotocore-es](https://pypi.org/project/types-aiobotocore-es/).

- [Paginators for aiobotocore ElasticsearchService module](#paginators-for-aiobotocore-elasticsearchservice-module)
  - [DescribeReservedElasticsearchInstanceOfferingsPaginator](#describereservedelasticsearchinstanceofferingspaginator)
  - [DescribeReservedElasticsearchInstancesPaginator](#describereservedelasticsearchinstancespaginator)
  - [GetUpgradeHistoryPaginator](#getupgradehistorypaginator)
  - [ListElasticsearchInstanceTypesPaginator](#listelasticsearchinstancetypespaginator)
  - [ListElasticsearchVersionsPaginator](#listelasticsearchversionspaginator)

<a id="describereservedelasticsearchinstanceofferingspaginator"></a>

## DescribeReservedElasticsearchInstanceOfferingsPaginator

Type annotations for
`session.create_client("es").get_paginator("describe_reserved_elasticsearch_instance_offerings")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_es.paginator import DescribeReservedElasticsearchInstanceOfferingsPaginator

session = get_session()
async with session.create_client("es") as client:
    client: ElasticsearchServiceClient
    paginator: DescribeReservedElasticsearchInstanceOfferingsPaginator = client.get_paginator("describe_reserved_elasticsearch_instance_offerings")
```

Boto3 documentation:
[ElasticsearchService.Paginator.DescribeReservedElasticsearchInstanceOfferings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.DescribeReservedElasticsearchInstanceOfferings)

Arguments for
`DescribeReservedElasticsearchInstanceOfferingsPaginator.paginate` method:

- `ReservedElasticsearchInstanceOfferingId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeReservedElasticsearchInstanceOfferingsPaginator.paginate` returns
`_PageIterator`\[[DescribeReservedElasticsearchInstanceOfferingsResponseTypeDef](./type_defs.md#describereservedelasticsearchinstanceofferingsresponsetypedef)\].

<a id="describereservedelasticsearchinstancespaginator"></a>

## DescribeReservedElasticsearchInstancesPaginator

Type annotations for
`session.create_client("es").get_paginator("describe_reserved_elasticsearch_instances")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_es.paginator import DescribeReservedElasticsearchInstancesPaginator

session = get_session()
async with session.create_client("es") as client:
    client: ElasticsearchServiceClient
    paginator: DescribeReservedElasticsearchInstancesPaginator = client.get_paginator("describe_reserved_elasticsearch_instances")
```

Boto3 documentation:
[ElasticsearchService.Paginator.DescribeReservedElasticsearchInstances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.DescribeReservedElasticsearchInstances)

Arguments for `DescribeReservedElasticsearchInstancesPaginator.paginate`
method:

- `ReservedElasticsearchInstanceId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeReservedElasticsearchInstancesPaginator.paginate` returns
`_PageIterator`\[[DescribeReservedElasticsearchInstancesResponseTypeDef](./type_defs.md#describereservedelasticsearchinstancesresponsetypedef)\].

<a id="getupgradehistorypaginator"></a>

## GetUpgradeHistoryPaginator

Type annotations for
`session.create_client("es").get_paginator("get_upgrade_history")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_es.paginator import GetUpgradeHistoryPaginator

session = get_session()
async with session.create_client("es") as client:
    client: ElasticsearchServiceClient
    paginator: GetUpgradeHistoryPaginator = client.get_paginator("get_upgrade_history")
```

Boto3 documentation:
[ElasticsearchService.Paginator.GetUpgradeHistory](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.GetUpgradeHistory)

Arguments for `GetUpgradeHistoryPaginator.paginate` method:

- `DomainName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetUpgradeHistoryPaginator.paginate` returns
`_PageIterator`\[[GetUpgradeHistoryResponseTypeDef](./type_defs.md#getupgradehistoryresponsetypedef)\].

<a id="listelasticsearchinstancetypespaginator"></a>

## ListElasticsearchInstanceTypesPaginator

Type annotations for
`session.create_client("es").get_paginator("list_elasticsearch_instance_types")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_es.paginator import ListElasticsearchInstanceTypesPaginator

session = get_session()
async with session.create_client("es") as client:
    client: ElasticsearchServiceClient
    paginator: ListElasticsearchInstanceTypesPaginator = client.get_paginator("list_elasticsearch_instance_types")
```

Boto3 documentation:
[ElasticsearchService.Paginator.ListElasticsearchInstanceTypes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.ListElasticsearchInstanceTypes)

Arguments for `ListElasticsearchInstanceTypesPaginator.paginate` method:

- `ElasticsearchVersion`: `str` *(required)*
- `DomainName`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListElasticsearchInstanceTypesPaginator.paginate` returns
`_PageIterator`\[[ListElasticsearchInstanceTypesResponseTypeDef](./type_defs.md#listelasticsearchinstancetypesresponsetypedef)\].

<a id="listelasticsearchversionspaginator"></a>

## ListElasticsearchVersionsPaginator

Type annotations for
`session.create_client("es").get_paginator("list_elasticsearch_versions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_es.paginator import ListElasticsearchVersionsPaginator

session = get_session()
async with session.create_client("es") as client:
    client: ElasticsearchServiceClient
    paginator: ListElasticsearchVersionsPaginator = client.get_paginator("list_elasticsearch_versions")
```

Boto3 documentation:
[ElasticsearchService.Paginator.ListElasticsearchVersions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#ElasticsearchService.Paginator.ListElasticsearchVersions)

Arguments for `ListElasticsearchVersionsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListElasticsearchVersionsPaginator.paginate` returns
`_PageIterator`\[[ListElasticsearchVersionsResponseTypeDef](./type_defs.md#listelasticsearchversionsresponsetypedef)\].
