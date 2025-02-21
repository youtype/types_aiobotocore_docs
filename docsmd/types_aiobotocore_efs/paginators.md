# Paginators

> [Index](../README.md) > [EFS](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [EFS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#efs)
    type annotations stubs module [types-aiobotocore-efs](https://pypi.org/project/types-aiobotocore-efs/).

## DescribeAccessPointsPaginator

Type annotations and code completion for `#!python session.create_client("efs").get_paginator("describe_access_points")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/paginator/DescribeAccessPoints.html#EFS.Paginator.DescribeAccessPoints)

```python
# DescribeAccessPointsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_efs.paginator import DescribeAccessPointsPaginator

session = get_session()
async with session.create_client("efs") as client:  # (1)
    paginator: DescribeAccessPointsPaginator = client.get_paginator("describe_access_points")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAccessPointsResponseTypeDef
        print(item)  # (3)
```

1. client: [EFSClient](./client.md)
2. paginator: [DescribeAccessPointsPaginator](./paginators.md#describeaccesspointspaginator)
3. item: [:material-code-braces: DescribeAccessPointsResponseTypeDef](./type_defs.md#describeaccesspointsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeAccessPointsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AccessPointId: str = ...,
    FileSystemId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeAccessPointsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeAccessPointsResponseTypeDef](./type_defs.md#describeaccesspointsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeAccessPointsRequestPaginateTypeDef = {  # (1)
    "AccessPointId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAccessPointsRequestPaginateTypeDef](./type_defs.md#describeaccesspointsrequestpaginatetypedef) 
## DescribeFileSystemsPaginator

Type annotations and code completion for `#!python session.create_client("efs").get_paginator("describe_file_systems")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/paginator/DescribeFileSystems.html#EFS.Paginator.DescribeFileSystems)

```python
# DescribeFileSystemsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    CreationToken: str = ...,
    FileSystemId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeFileSystemsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeFileSystemsResponseTypeDef](./type_defs.md#describefilesystemsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeFileSystemsRequestPaginateTypeDef = {  # (1)
    "CreationToken": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeFileSystemsRequestPaginateTypeDef](./type_defs.md#describefilesystemsrequestpaginatetypedef) 
## DescribeMountTargetsPaginator

Type annotations and code completion for `#!python session.create_client("efs").get_paginator("describe_mount_targets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/paginator/DescribeMountTargets.html#EFS.Paginator.DescribeMountTargets)

```python
# DescribeMountTargetsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    FileSystemId: str = ...,
    MountTargetId: str = ...,
    AccessPointId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeMountTargetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeMountTargetsResponseTypeDef](./type_defs.md#describemounttargetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeMountTargetsRequestPaginateTypeDef = {  # (1)
    "FileSystemId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeMountTargetsRequestPaginateTypeDef](./type_defs.md#describemounttargetsrequestpaginatetypedef) 
## DescribeReplicationConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("efs").get_paginator("describe_replication_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/paginator/DescribeReplicationConfigurations.html#EFS.Paginator.DescribeReplicationConfigurations)

```python
# DescribeReplicationConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_efs.paginator import DescribeReplicationConfigurationsPaginator

session = get_session()
async with session.create_client("efs") as client:  # (1)
    paginator: DescribeReplicationConfigurationsPaginator = client.get_paginator("describe_replication_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeReplicationConfigurationsResponseTypeDef
        print(item)  # (3)
```

1. client: [EFSClient](./client.md)
2. paginator: [DescribeReplicationConfigurationsPaginator](./paginators.md#describereplicationconfigurationspaginator)
3. item: [:material-code-braces: DescribeReplicationConfigurationsResponseTypeDef](./type_defs.md#describereplicationconfigurationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeReplicationConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FileSystemId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeReplicationConfigurationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeReplicationConfigurationsResponseTypeDef](./type_defs.md#describereplicationconfigurationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeReplicationConfigurationsRequestPaginateTypeDef = {  # (1)
    "FileSystemId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReplicationConfigurationsRequestPaginateTypeDef](./type_defs.md#describereplicationconfigurationsrequestpaginatetypedef) 
## DescribeTagsPaginator

Type annotations and code completion for `#!python session.create_client("efs").get_paginator("describe_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs/paginator/DescribeTags.html#EFS.Paginator.DescribeTags)

```python
# DescribeTagsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    FileSystemId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeTagsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeTagsResponseTypeDef](./type_defs.md#describetagsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeTagsRequestPaginateTypeDef = {  # (1)
    "FileSystemId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTagsRequestPaginateTypeDef](./type_defs.md#describetagsrequestpaginatetypedef) 
