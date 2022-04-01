# Paginators

> [Index](../README.md) > [CloudHSMV2](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CloudHSMV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2)
    type annotations stubs module [types-aiobotocore-cloudhsmv2](https://pypi.org/project/types-aiobotocore-cloudhsmv2/).

## DescribeBackupsPaginator

Type annotations and code completion for `#!python session.create_client("cloudhsmv2").get_paginator("describe_backups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Paginator.DescribeBackups)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_cloudhsmv2.paginator import DescribeBackupsPaginator

session = get_session()
async with session.create_client("cloudhsmv2") as client:
    client: CloudHSMV2Client
    paginator: DescribeBackupsPaginator = client.get_paginator("describe_backups")
```


### paginate

Type annotations and code completion for `#!python DescribeBackupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Mapping[str, Sequence[str]] = ...,
    SortAscending: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeBackupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeBackupsResponseTypeDef](./type_defs.md#describebackupsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeBackupsRequestDescribeBackupsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeBackupsRequestDescribeBackupsPaginateTypeDef](./type_defs.md#describebackupsrequestdescribebackupspaginatetypedef) 
## DescribeClustersPaginator

Type annotations and code completion for `#!python session.create_client("cloudhsmv2").get_paginator("describe_clusters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Paginator.DescribeClusters)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_cloudhsmv2.paginator import DescribeClustersPaginator

session = get_session()
async with session.create_client("cloudhsmv2") as client:
    client: CloudHSMV2Client
    paginator: DescribeClustersPaginator = client.get_paginator("describe_clusters")
```


### paginate

Type annotations and code completion for `#!python DescribeClustersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Mapping[str, Sequence[str]] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeClustersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeClustersResponseTypeDef](./type_defs.md#describeclustersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeClustersRequestDescribeClustersPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClustersRequestDescribeClustersPaginateTypeDef](./type_defs.md#describeclustersrequestdescribeclusterspaginatetypedef) 
## ListTagsPaginator

Type annotations and code completion for `#!python session.create_client("cloudhsmv2").get_paginator("list_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Paginator.ListTags)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_cloudhsmv2.paginator import ListTagsPaginator

session = get_session()
async with session.create_client("cloudhsmv2") as client:
    client: CloudHSMV2Client
    paginator: ListTagsPaginator = client.get_paginator("list_tags")
```


### paginate

Type annotations and code completion for `#!python ListTagsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ResourceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTagsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTagsResponseTypeDef](./type_defs.md#listtagsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTagsRequestListTagsPaginateTypeDef = {  # (1)
    "ResourceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsRequestListTagsPaginateTypeDef](./type_defs.md#listtagsrequestlisttagspaginatetypedef) 
