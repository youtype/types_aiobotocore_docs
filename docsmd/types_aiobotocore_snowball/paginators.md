# Paginators

> [Index](../README.md) > [Snowball](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Snowball](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#snowball)
    type annotations stubs module [types-aiobotocore-snowball](https://pypi.org/project/types-aiobotocore-snowball/).

## DescribeAddressesPaginator

Type annotations and code completion for `#!python session.create_client("snowball").get_paginator("describe_addresses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball/paginator/DescribeAddresses.html#Snowball.Paginator.DescribeAddresses)

```python
# DescribeAddressesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_snowball.paginator import DescribeAddressesPaginator

session = get_session()
async with session.create_client("snowball") as client:  # (1)
    paginator: DescribeAddressesPaginator = client.get_paginator("describe_addresses")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAddressesResultTypeDef
        print(item)  # (3)
```

1. client: [SnowballClient](./client.md)
2. paginator: [DescribeAddressesPaginator](./paginators.md#describeaddressespaginator)
3. item: [:material-code-braces: DescribeAddressesResultTypeDef](./type_defs.md#describeaddressesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeAddressesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeAddressesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeAddressesResultTypeDef](./type_defs.md#describeaddressesresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeAddressesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAddressesRequestPaginateTypeDef](./type_defs.md#describeaddressesrequestpaginatetypedef) 
## ListClusterJobsPaginator

Type annotations and code completion for `#!python session.create_client("snowball").get_paginator("list_cluster_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball/paginator/ListClusterJobs.html#Snowball.Paginator.ListClusterJobs)

```python
# ListClusterJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_snowball.paginator import ListClusterJobsPaginator

session = get_session()
async with session.create_client("snowball") as client:  # (1)
    paginator: ListClusterJobsPaginator = client.get_paginator("list_cluster_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListClusterJobsResultTypeDef
        print(item)  # (3)
```

1. client: [SnowballClient](./client.md)
2. paginator: [ListClusterJobsPaginator](./paginators.md#listclusterjobspaginator)
3. item: [:material-code-braces: ListClusterJobsResultTypeDef](./type_defs.md#listclusterjobsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListClusterJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListClusterJobsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListClusterJobsResultTypeDef](./type_defs.md#listclusterjobsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListClusterJobsRequestPaginateTypeDef = {  # (1)
    "ClusterId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListClusterJobsRequestPaginateTypeDef](./type_defs.md#listclusterjobsrequestpaginatetypedef) 
## ListClustersPaginator

Type annotations and code completion for `#!python session.create_client("snowball").get_paginator("list_clusters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball/paginator/ListClusters.html#Snowball.Paginator.ListClusters)

```python
# ListClustersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_snowball.paginator import ListClustersPaginator

session = get_session()
async with session.create_client("snowball") as client:  # (1)
    paginator: ListClustersPaginator = client.get_paginator("list_clusters")  # (2)
    async for item in paginator.paginate(...):
        item: ListClustersResultTypeDef
        print(item)  # (3)
```

1. client: [SnowballClient](./client.md)
2. paginator: [ListClustersPaginator](./paginators.md#listclusterspaginator)
3. item: [:material-code-braces: ListClustersResultTypeDef](./type_defs.md#listclustersresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListClustersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListClustersResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListClustersResultTypeDef](./type_defs.md#listclustersresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListClustersRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListClustersRequestPaginateTypeDef](./type_defs.md#listclustersrequestpaginatetypedef) 
## ListCompatibleImagesPaginator

Type annotations and code completion for `#!python session.create_client("snowball").get_paginator("list_compatible_images")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball/paginator/ListCompatibleImages.html#Snowball.Paginator.ListCompatibleImages)

```python
# ListCompatibleImagesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_snowball.paginator import ListCompatibleImagesPaginator

session = get_session()
async with session.create_client("snowball") as client:  # (1)
    paginator: ListCompatibleImagesPaginator = client.get_paginator("list_compatible_images")  # (2)
    async for item in paginator.paginate(...):
        item: ListCompatibleImagesResultTypeDef
        print(item)  # (3)
```

1. client: [SnowballClient](./client.md)
2. paginator: [ListCompatibleImagesPaginator](./paginators.md#listcompatibleimagespaginator)
3. item: [:material-code-braces: ListCompatibleImagesResultTypeDef](./type_defs.md#listcompatibleimagesresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListCompatibleImagesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListCompatibleImagesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCompatibleImagesResultTypeDef](./type_defs.md#listcompatibleimagesresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCompatibleImagesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCompatibleImagesRequestPaginateTypeDef](./type_defs.md#listcompatibleimagesrequestpaginatetypedef) 
## ListJobsPaginator

Type annotations and code completion for `#!python session.create_client("snowball").get_paginator("list_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball/paginator/ListJobs.html#Snowball.Paginator.ListJobs)

```python
# ListJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_snowball.paginator import ListJobsPaginator

session = get_session()
async with session.create_client("snowball") as client:  # (1)
    paginator: ListJobsPaginator = client.get_paginator("list_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListJobsResultTypeDef
        print(item)  # (3)
```

1. client: [SnowballClient](./client.md)
2. paginator: [ListJobsPaginator](./paginators.md#listjobspaginator)
3. item: [:material-code-braces: ListJobsResultTypeDef](./type_defs.md#listjobsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListJobsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListJobsResultTypeDef](./type_defs.md#listjobsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListJobsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobsRequestPaginateTypeDef](./type_defs.md#listjobsrequestpaginatetypedef) 
## ListLongTermPricingPaginator

Type annotations and code completion for `#!python session.create_client("snowball").get_paginator("list_long_term_pricing")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball/paginator/ListLongTermPricing.html#Snowball.Paginator.ListLongTermPricing)

```python
# ListLongTermPricingPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_snowball.paginator import ListLongTermPricingPaginator

session = get_session()
async with session.create_client("snowball") as client:  # (1)
    paginator: ListLongTermPricingPaginator = client.get_paginator("list_long_term_pricing")  # (2)
    async for item in paginator.paginate(...):
        item: ListLongTermPricingResultTypeDef
        print(item)  # (3)
```

1. client: [SnowballClient](./client.md)
2. paginator: [ListLongTermPricingPaginator](./paginators.md#listlongtermpricingpaginator)
3. item: [:material-code-braces: ListLongTermPricingResultTypeDef](./type_defs.md#listlongtermpricingresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListLongTermPricingPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListLongTermPricingResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListLongTermPricingResultTypeDef](./type_defs.md#listlongtermpricingresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListLongTermPricingRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLongTermPricingRequestPaginateTypeDef](./type_defs.md#listlongtermpricingrequestpaginatetypedef) 
