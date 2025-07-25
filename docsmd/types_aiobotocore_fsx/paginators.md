# Paginators

> [Index](../README.md) > [FSx](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [FSx](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#fsx)
    type annotations stubs module [types-aiobotocore-fsx](https://pypi.org/project/types-aiobotocore-fsx/).

## DescribeBackupsPaginator

Type annotations and code completion for `#!python session.create_client("fsx").get_paginator("describe_backups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx/paginator/DescribeBackups.html#FSx.Paginator.DescribeBackups)

```python
# DescribeBackupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_fsx.paginator import DescribeBackupsPaginator

session = get_session()
async with session.create_client("fsx") as client:  # (1)
    paginator: DescribeBackupsPaginator = client.get_paginator("describe_backups")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeBackupsResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [FSxClient](./client.md)
2. paginator: [DescribeBackupsPaginator](./paginators.md#describebackupspaginator)
3. item: `AioPageIterator[DescribeBackupsResponsePaginatorTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeBackupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    BackupIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeBackupsResponsePaginatorTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeBackupsResponsePaginatorTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeBackupsRequestPaginateTypeDef = {  # (1)
    "BackupIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeBackupsRequestPaginateTypeDef](./type_defs.md#describebackupsrequestpaginatetypedef)
## DescribeFileSystemsPaginator

Type annotations and code completion for `#!python session.create_client("fsx").get_paginator("describe_file_systems")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx/paginator/DescribeFileSystems.html#FSx.Paginator.DescribeFileSystems)

```python
# DescribeFileSystemsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_fsx.paginator import DescribeFileSystemsPaginator

session = get_session()
async with session.create_client("fsx") as client:  # (1)
    paginator: DescribeFileSystemsPaginator = client.get_paginator("describe_file_systems")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeFileSystemsResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [FSxClient](./client.md)
2. paginator: [DescribeFileSystemsPaginator](./paginators.md#describefilesystemspaginator)
3. item: `AioPageIterator[DescribeFileSystemsResponsePaginatorTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeFileSystemsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FileSystemIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeFileSystemsResponsePaginatorTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeFileSystemsResponsePaginatorTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeFileSystemsRequestPaginateTypeDef = {  # (1)
    "FileSystemIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeFileSystemsRequestPaginateTypeDef](./type_defs.md#describefilesystemsrequestpaginatetypedef)
## DescribeS3AccessPointAttachmentsPaginator

Type annotations and code completion for `#!python session.create_client("fsx").get_paginator("describe_s3_access_point_attachments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx/paginator/DescribeS3AccessPointAttachments.html#FSx.Paginator.DescribeS3AccessPointAttachments)

```python
# DescribeS3AccessPointAttachmentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_fsx.paginator import DescribeS3AccessPointAttachmentsPaginator

session = get_session()
async with session.create_client("fsx") as client:  # (1)
    paginator: DescribeS3AccessPointAttachmentsPaginator = client.get_paginator("describe_s3_access_point_attachments")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeS3AccessPointAttachmentsResponseTypeDef
        print(item)  # (3)
```

1. client: [FSxClient](./client.md)
2. paginator: [DescribeS3AccessPointAttachmentsPaginator](./paginators.md#describes3accesspointattachmentspaginator)
3. item: `AioPageIterator[DescribeS3AccessPointAttachmentsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeS3AccessPointAttachmentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Names: Sequence[str] = ...,
    Filters: Sequence[S3AccessPointAttachmentsFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeS3AccessPointAttachmentsResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[S3AccessPointAttachmentsFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeS3AccessPointAttachmentsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeS3AccessPointAttachmentsRequestPaginateTypeDef = {  # (1)
    "Names": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeS3AccessPointAttachmentsRequestPaginateTypeDef](./type_defs.md#describes3accesspointattachmentsrequestpaginatetypedef)
## DescribeSnapshotsPaginator

Type annotations and code completion for `#!python session.create_client("fsx").get_paginator("describe_snapshots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx/paginator/DescribeSnapshots.html#FSx.Paginator.DescribeSnapshots)

```python
# DescribeSnapshotsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_fsx.paginator import DescribeSnapshotsPaginator

session = get_session()
async with session.create_client("fsx") as client:  # (1)
    paginator: DescribeSnapshotsPaginator = client.get_paginator("describe_snapshots")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSnapshotsResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [FSxClient](./client.md)
2. paginator: [DescribeSnapshotsPaginator](./paginators.md#describesnapshotspaginator)
3. item: `AioPageIterator[DescribeSnapshotsResponsePaginatorTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeSnapshotsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SnapshotIds: Sequence[str] = ...,
    Filters: Sequence[SnapshotFilterTypeDef] = ...,  # (1)
    IncludeShared: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeSnapshotsResponsePaginatorTypeDef]:  # (3)
    ...
```

1. See `Sequence[SnapshotFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeSnapshotsResponsePaginatorTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSnapshotsRequestPaginateTypeDef = {  # (1)
    "SnapshotIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSnapshotsRequestPaginateTypeDef](./type_defs.md#describesnapshotsrequestpaginatetypedef)
## DescribeStorageVirtualMachinesPaginator

Type annotations and code completion for `#!python session.create_client("fsx").get_paginator("describe_storage_virtual_machines")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx/paginator/DescribeStorageVirtualMachines.html#FSx.Paginator.DescribeStorageVirtualMachines)

```python
# DescribeStorageVirtualMachinesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_fsx.paginator import DescribeStorageVirtualMachinesPaginator

session = get_session()
async with session.create_client("fsx") as client:  # (1)
    paginator: DescribeStorageVirtualMachinesPaginator = client.get_paginator("describe_storage_virtual_machines")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeStorageVirtualMachinesResponseTypeDef
        print(item)  # (3)
```

1. client: [FSxClient](./client.md)
2. paginator: [DescribeStorageVirtualMachinesPaginator](./paginators.md#describestoragevirtualmachinespaginator)
3. item: `AioPageIterator[DescribeStorageVirtualMachinesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeStorageVirtualMachinesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    StorageVirtualMachineIds: Sequence[str] = ...,
    Filters: Sequence[StorageVirtualMachineFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeStorageVirtualMachinesResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[StorageVirtualMachineFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeStorageVirtualMachinesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeStorageVirtualMachinesRequestPaginateTypeDef = {  # (1)
    "StorageVirtualMachineIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeStorageVirtualMachinesRequestPaginateTypeDef](./type_defs.md#describestoragevirtualmachinesrequestpaginatetypedef)
## DescribeVolumesPaginator

Type annotations and code completion for `#!python session.create_client("fsx").get_paginator("describe_volumes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx/paginator/DescribeVolumes.html#FSx.Paginator.DescribeVolumes)

```python
# DescribeVolumesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_fsx.paginator import DescribeVolumesPaginator

session = get_session()
async with session.create_client("fsx") as client:  # (1)
    paginator: DescribeVolumesPaginator = client.get_paginator("describe_volumes")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeVolumesResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [FSxClient](./client.md)
2. paginator: [DescribeVolumesPaginator](./paginators.md#describevolumespaginator)
3. item: `AioPageIterator[DescribeVolumesResponsePaginatorTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeVolumesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    VolumeIds: Sequence[str] = ...,
    Filters: Sequence[VolumeFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeVolumesResponsePaginatorTypeDef]:  # (3)
    ...
```

1. See `Sequence[VolumeFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeVolumesResponsePaginatorTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeVolumesRequestPaginateTypeDef = {  # (1)
    "VolumeIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVolumesRequestPaginateTypeDef](./type_defs.md#describevolumesrequestpaginatetypedef)
## ListTagsForResourcePaginator

Type annotations and code completion for `#!python session.create_client("fsx").get_paginator("list_tags_for_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx/paginator/ListTagsForResource.html#FSx.Paginator.ListTagsForResource)

```python
# ListTagsForResourcePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_fsx.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("fsx") as client:  # (1)
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")  # (2)
    async for item in paginator.paginate(...):
        item: ListTagsForResourceResponseTypeDef
        print(item)  # (3)
```

1. client: [FSxClient](./client.md)
2. paginator: [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
3. item: `AioPageIterator[ListTagsForResourceResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTagsForResourcePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceARN: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTagsForResourceResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTagsForResourceResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTagsForResourceRequestPaginateTypeDef = {  # (1)
    "ResourceARN": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestPaginateTypeDef](./type_defs.md#listtagsforresourcerequestpaginatetypedef)
