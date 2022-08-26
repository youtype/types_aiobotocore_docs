# Paginators

> [Index](../README.md) > [EFS](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [EFS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
    type annotations stubs module [types-aiobotocore-efs](https://pypi.org/project/types-aiobotocore-efs/).

## DescribeFileSystemsPaginator

Type annotations and code completion for `#!python session.create_client("efs").get_paginator("describe_file_systems")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeFileSystems)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_efs.paginator import DescribeFileSystemsPaginator

session = get_session()
async with session.create_client("efs") as client:  # (1)
    paginator: DescribeFileSystemsPaginator = client.get_paginator("describe_file_systems")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeFileSystemsResponseTypeDef
        print(item)  # (3)
```

1. client: [EFSClient](./client.md)
2. paginator: [DescribeFileSystemsPaginator](./paginators.md#describefilesystemspaginator)
3. item: [:material-code-braces: DescribeFileSystemsResponseTypeDef](./type_defs.md#describefilesystemsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeFileSystemsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    CreationToken: str = ...,
    FileSystemId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeFileSystemsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeFileSystemsResponseTypeDef](./type_defs.md#describefilesystemsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef = {  # (1)
    "CreationToken": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef](./type_defs.md#describefilesystemsrequestdescribefilesystemspaginatetypedef) 
## DescribeMountTargetsPaginator

Type annotations and code completion for `#!python session.create_client("efs").get_paginator("describe_mount_targets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeMountTargets)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_efs.paginator import DescribeMountTargetsPaginator

session = get_session()
async with session.create_client("efs") as client:  # (1)
    paginator: DescribeMountTargetsPaginator = client.get_paginator("describe_mount_targets")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeMountTargetsResponseTypeDef
        print(item)  # (3)
```

1. client: [EFSClient](./client.md)
2. paginator: [DescribeMountTargetsPaginator](./paginators.md#describemounttargetspaginator)
3. item: [:material-code-braces: DescribeMountTargetsResponseTypeDef](./type_defs.md#describemounttargetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeMountTargetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    FileSystemId: str = ...,
    MountTargetId: str = ...,
    AccessPointId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeMountTargetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeMountTargetsResponseTypeDef](./type_defs.md#describemounttargetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef = {  # (1)
    "FileSystemId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef](./type_defs.md#describemounttargetsrequestdescribemounttargetspaginatetypedef) 
## DescribeTagsPaginator

Type annotations and code completion for `#!python session.create_client("efs").get_paginator("describe_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeTags)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_efs.paginator import DescribeTagsPaginator

session = get_session()
async with session.create_client("efs") as client:  # (1)
    paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeTagsResponseTypeDef
        print(item)  # (3)
```

1. client: [EFSClient](./client.md)
2. paginator: [DescribeTagsPaginator](./paginators.md#describetagspaginator)
3. item: [:material-code-braces: DescribeTagsResponseTypeDef](./type_defs.md#describetagsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTagsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    FileSystemId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeTagsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeTagsResponseTypeDef](./type_defs.md#describetagsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeTagsRequestDescribeTagsPaginateTypeDef = {  # (1)
    "FileSystemId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTagsRequestDescribeTagsPaginateTypeDef](./type_defs.md#describetagsrequestdescribetagspaginatetypedef) 
