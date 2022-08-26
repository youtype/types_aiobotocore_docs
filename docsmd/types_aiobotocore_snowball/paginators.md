# Paginators

> [Index](../README.md) > [Snowball](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Snowball](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball)
    type annotations stubs module [types-aiobotocore-snowball](https://pypi.org/project/types-aiobotocore-snowball/).

## DescribeAddressesPaginator

Type annotations and code completion for `#!python session.create_client("snowball").get_paginator("describe_addresses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.DescribeAddresses)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeAddressesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeAddressesResultTypeDef](./type_defs.md#describeaddressesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeAddressesRequestDescribeAddressesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAddressesRequestDescribeAddressesPaginateTypeDef](./type_defs.md#describeaddressesrequestdescribeaddressespaginatetypedef) 
## ListClusterJobsPaginator

Type annotations and code completion for `#!python session.create_client("snowball").get_paginator("list_cluster_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusterJobs)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    ClusterId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListClusterJobsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListClusterJobsResultTypeDef](./type_defs.md#listclusterjobsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListClusterJobsRequestListClusterJobsPaginateTypeDef = {  # (1)
    "ClusterId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListClusterJobsRequestListClusterJobsPaginateTypeDef](./type_defs.md#listclusterjobsrequestlistclusterjobspaginatetypedef) 
## ListClustersPaginator

Type annotations and code completion for `#!python session.create_client("snowball").get_paginator("list_clusters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListClusters)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListClustersResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListClustersResultTypeDef](./type_defs.md#listclustersresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListClustersRequestListClustersPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListClustersRequestListClustersPaginateTypeDef](./type_defs.md#listclustersrequestlistclusterspaginatetypedef) 
## ListCompatibleImagesPaginator

Type annotations and code completion for `#!python session.create_client("snowball").get_paginator("list_compatible_images")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListCompatibleImages)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListCompatibleImagesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCompatibleImagesResultTypeDef](./type_defs.md#listcompatibleimagesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCompatibleImagesRequestListCompatibleImagesPaginateTypeDef](./type_defs.md#listcompatibleimagesrequestlistcompatibleimagespaginatetypedef) 
## ListJobsPaginator

Type annotations and code completion for `#!python session.create_client("snowball").get_paginator("list_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#Snowball.Paginator.ListJobs)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListJobsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListJobsResultTypeDef](./type_defs.md#listjobsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListJobsRequestListJobsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobsRequestListJobsPaginateTypeDef](./type_defs.md#listjobsrequestlistjobspaginatetypedef) 
