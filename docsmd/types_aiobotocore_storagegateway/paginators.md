# Paginators

> [Index](../README.md) > [StorageGateway](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [StorageGateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#storagegateway)
    type annotations stubs module [types-aiobotocore-storagegateway](https://pypi.org/project/types-aiobotocore-storagegateway/).

## DescribeTapeArchivesPaginator

Type annotations and code completion for `#!python session.create_client("storagegateway").get_paginator("describe_tape_archives")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway/paginator/DescribeTapeArchives.html#StorageGateway.Paginator.DescribeTapeArchives)

```python
# DescribeTapeArchivesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_storagegateway.paginator import DescribeTapeArchivesPaginator

session = get_session()
async with session.create_client("storagegateway") as client:  # (1)
    paginator: DescribeTapeArchivesPaginator = client.get_paginator("describe_tape_archives")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeTapeArchivesOutputTypeDef
        print(item)  # (3)
```

1. client: [StorageGatewayClient](./client.md)
2. paginator: [DescribeTapeArchivesPaginator](./paginators.md#describetapearchivespaginator)
3. item: [:material-code-braces: DescribeTapeArchivesOutputTypeDef](./type_defs.md#describetapearchivesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTapeArchivesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TapeARNs: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeTapeArchivesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeTapeArchivesOutputTypeDef](./type_defs.md#describetapearchivesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeTapeArchivesInputPaginateTypeDef = {  # (1)
    "TapeARNs": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTapeArchivesInputPaginateTypeDef](./type_defs.md#describetapearchivesinputpaginatetypedef) 
## DescribeTapeRecoveryPointsPaginator

Type annotations and code completion for `#!python session.create_client("storagegateway").get_paginator("describe_tape_recovery_points")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway/paginator/DescribeTapeRecoveryPoints.html#StorageGateway.Paginator.DescribeTapeRecoveryPoints)

```python
# DescribeTapeRecoveryPointsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_storagegateway.paginator import DescribeTapeRecoveryPointsPaginator

session = get_session()
async with session.create_client("storagegateway") as client:  # (1)
    paginator: DescribeTapeRecoveryPointsPaginator = client.get_paginator("describe_tape_recovery_points")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeTapeRecoveryPointsOutputTypeDef
        print(item)  # (3)
```

1. client: [StorageGatewayClient](./client.md)
2. paginator: [DescribeTapeRecoveryPointsPaginator](./paginators.md#describetaperecoverypointspaginator)
3. item: [:material-code-braces: DescribeTapeRecoveryPointsOutputTypeDef](./type_defs.md#describetaperecoverypointsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTapeRecoveryPointsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    GatewayARN: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeTapeRecoveryPointsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeTapeRecoveryPointsOutputTypeDef](./type_defs.md#describetaperecoverypointsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeTapeRecoveryPointsInputPaginateTypeDef = {  # (1)
    "GatewayARN": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTapeRecoveryPointsInputPaginateTypeDef](./type_defs.md#describetaperecoverypointsinputpaginatetypedef) 
## DescribeTapesPaginator

Type annotations and code completion for `#!python session.create_client("storagegateway").get_paginator("describe_tapes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway/paginator/DescribeTapes.html#StorageGateway.Paginator.DescribeTapes)

```python
# DescribeTapesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_storagegateway.paginator import DescribeTapesPaginator

session = get_session()
async with session.create_client("storagegateway") as client:  # (1)
    paginator: DescribeTapesPaginator = client.get_paginator("describe_tapes")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeTapesOutputTypeDef
        print(item)  # (3)
```

1. client: [StorageGatewayClient](./client.md)
2. paginator: [DescribeTapesPaginator](./paginators.md#describetapespaginator)
3. item: [:material-code-braces: DescribeTapesOutputTypeDef](./type_defs.md#describetapesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTapesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    GatewayARN: str,
    TapeARNs: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeTapesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeTapesOutputTypeDef](./type_defs.md#describetapesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeTapesInputPaginateTypeDef = {  # (1)
    "GatewayARN": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTapesInputPaginateTypeDef](./type_defs.md#describetapesinputpaginatetypedef) 
## DescribeVTLDevicesPaginator

Type annotations and code completion for `#!python session.create_client("storagegateway").get_paginator("describe_vtl_devices")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway/paginator/DescribeVTLDevices.html#StorageGateway.Paginator.DescribeVTLDevices)

```python
# DescribeVTLDevicesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_storagegateway.paginator import DescribeVTLDevicesPaginator

session = get_session()
async with session.create_client("storagegateway") as client:  # (1)
    paginator: DescribeVTLDevicesPaginator = client.get_paginator("describe_vtl_devices")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeVTLDevicesOutputTypeDef
        print(item)  # (3)
```

1. client: [StorageGatewayClient](./client.md)
2. paginator: [DescribeVTLDevicesPaginator](./paginators.md#describevtldevicespaginator)
3. item: [:material-code-braces: DescribeVTLDevicesOutputTypeDef](./type_defs.md#describevtldevicesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python DescribeVTLDevicesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    GatewayARN: str,
    VTLDeviceARNs: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeVTLDevicesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeVTLDevicesOutputTypeDef](./type_defs.md#describevtldevicesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeVTLDevicesInputPaginateTypeDef = {  # (1)
    "GatewayARN": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVTLDevicesInputPaginateTypeDef](./type_defs.md#describevtldevicesinputpaginatetypedef) 
## ListFileSharesPaginator

Type annotations and code completion for `#!python session.create_client("storagegateway").get_paginator("list_file_shares")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway/paginator/ListFileShares.html#StorageGateway.Paginator.ListFileShares)

```python
# ListFileSharesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_storagegateway.paginator import ListFileSharesPaginator

session = get_session()
async with session.create_client("storagegateway") as client:  # (1)
    paginator: ListFileSharesPaginator = client.get_paginator("list_file_shares")  # (2)
    async for item in paginator.paginate(...):
        item: ListFileSharesOutputTypeDef
        print(item)  # (3)
```

1. client: [StorageGatewayClient](./client.md)
2. paginator: [ListFileSharesPaginator](./paginators.md#listfilesharespaginator)
3. item: [:material-code-braces: ListFileSharesOutputTypeDef](./type_defs.md#listfilesharesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListFileSharesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    GatewayARN: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListFileSharesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFileSharesOutputTypeDef](./type_defs.md#listfilesharesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFileSharesInputPaginateTypeDef = {  # (1)
    "GatewayARN": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFileSharesInputPaginateTypeDef](./type_defs.md#listfilesharesinputpaginatetypedef) 
## ListFileSystemAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("storagegateway").get_paginator("list_file_system_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway/paginator/ListFileSystemAssociations.html#StorageGateway.Paginator.ListFileSystemAssociations)

```python
# ListFileSystemAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_storagegateway.paginator import ListFileSystemAssociationsPaginator

session = get_session()
async with session.create_client("storagegateway") as client:  # (1)
    paginator: ListFileSystemAssociationsPaginator = client.get_paginator("list_file_system_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListFileSystemAssociationsOutputTypeDef
        print(item)  # (3)
```

1. client: [StorageGatewayClient](./client.md)
2. paginator: [ListFileSystemAssociationsPaginator](./paginators.md#listfilesystemassociationspaginator)
3. item: [:material-code-braces: ListFileSystemAssociationsOutputTypeDef](./type_defs.md#listfilesystemassociationsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListFileSystemAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    GatewayARN: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListFileSystemAssociationsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFileSystemAssociationsOutputTypeDef](./type_defs.md#listfilesystemassociationsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFileSystemAssociationsInputPaginateTypeDef = {  # (1)
    "GatewayARN": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFileSystemAssociationsInputPaginateTypeDef](./type_defs.md#listfilesystemassociationsinputpaginatetypedef) 
## ListGatewaysPaginator

Type annotations and code completion for `#!python session.create_client("storagegateway").get_paginator("list_gateways")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway/paginator/ListGateways.html#StorageGateway.Paginator.ListGateways)

```python
# ListGatewaysPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_storagegateway.paginator import ListGatewaysPaginator

session = get_session()
async with session.create_client("storagegateway") as client:  # (1)
    paginator: ListGatewaysPaginator = client.get_paginator("list_gateways")  # (2)
    async for item in paginator.paginate(...):
        item: ListGatewaysOutputTypeDef
        print(item)  # (3)
```

1. client: [StorageGatewayClient](./client.md)
2. paginator: [ListGatewaysPaginator](./paginators.md#listgatewayspaginator)
3. item: [:material-code-braces: ListGatewaysOutputTypeDef](./type_defs.md#listgatewaysoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListGatewaysPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListGatewaysOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGatewaysOutputTypeDef](./type_defs.md#listgatewaysoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListGatewaysInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGatewaysInputPaginateTypeDef](./type_defs.md#listgatewaysinputpaginatetypedef) 
## ListTagsForResourcePaginator

Type annotations and code completion for `#!python session.create_client("storagegateway").get_paginator("list_tags_for_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway/paginator/ListTagsForResource.html#StorageGateway.Paginator.ListTagsForResource)

```python
# ListTagsForResourcePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_storagegateway.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("storagegateway") as client:  # (1)
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")  # (2)
    async for item in paginator.paginate(...):
        item: ListTagsForResourceOutputTypeDef
        print(item)  # (3)
```

1. client: [StorageGatewayClient](./client.md)
2. paginator: [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
3. item: [:material-code-braces: ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListTagsForResourcePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceARN: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTagsForResourceOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTagsForResourceInputPaginateTypeDef = {  # (1)
    "ResourceARN": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceInputPaginateTypeDef](./type_defs.md#listtagsforresourceinputpaginatetypedef) 
## ListTapePoolsPaginator

Type annotations and code completion for `#!python session.create_client("storagegateway").get_paginator("list_tape_pools")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway/paginator/ListTapePools.html#StorageGateway.Paginator.ListTapePools)

```python
# ListTapePoolsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_storagegateway.paginator import ListTapePoolsPaginator

session = get_session()
async with session.create_client("storagegateway") as client:  # (1)
    paginator: ListTapePoolsPaginator = client.get_paginator("list_tape_pools")  # (2)
    async for item in paginator.paginate(...):
        item: ListTapePoolsOutputTypeDef
        print(item)  # (3)
```

1. client: [StorageGatewayClient](./client.md)
2. paginator: [ListTapePoolsPaginator](./paginators.md#listtapepoolspaginator)
3. item: [:material-code-braces: ListTapePoolsOutputTypeDef](./type_defs.md#listtapepoolsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListTapePoolsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PoolARNs: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTapePoolsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTapePoolsOutputTypeDef](./type_defs.md#listtapepoolsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTapePoolsInputPaginateTypeDef = {  # (1)
    "PoolARNs": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTapePoolsInputPaginateTypeDef](./type_defs.md#listtapepoolsinputpaginatetypedef) 
## ListTapesPaginator

Type annotations and code completion for `#!python session.create_client("storagegateway").get_paginator("list_tapes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway/paginator/ListTapes.html#StorageGateway.Paginator.ListTapes)

```python
# ListTapesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_storagegateway.paginator import ListTapesPaginator

session = get_session()
async with session.create_client("storagegateway") as client:  # (1)
    paginator: ListTapesPaginator = client.get_paginator("list_tapes")  # (2)
    async for item in paginator.paginate(...):
        item: ListTapesOutputTypeDef
        print(item)  # (3)
```

1. client: [StorageGatewayClient](./client.md)
2. paginator: [ListTapesPaginator](./paginators.md#listtapespaginator)
3. item: [:material-code-braces: ListTapesOutputTypeDef](./type_defs.md#listtapesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListTapesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TapeARNs: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTapesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTapesOutputTypeDef](./type_defs.md#listtapesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTapesInputPaginateTypeDef = {  # (1)
    "TapeARNs": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTapesInputPaginateTypeDef](./type_defs.md#listtapesinputpaginatetypedef) 
## ListVolumesPaginator

Type annotations and code completion for `#!python session.create_client("storagegateway").get_paginator("list_volumes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway/paginator/ListVolumes.html#StorageGateway.Paginator.ListVolumes)

```python
# ListVolumesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_storagegateway.paginator import ListVolumesPaginator

session = get_session()
async with session.create_client("storagegateway") as client:  # (1)
    paginator: ListVolumesPaginator = client.get_paginator("list_volumes")  # (2)
    async for item in paginator.paginate(...):
        item: ListVolumesOutputTypeDef
        print(item)  # (3)
```

1. client: [StorageGatewayClient](./client.md)
2. paginator: [ListVolumesPaginator](./paginators.md#listvolumespaginator)
3. item: [:material-code-braces: ListVolumesOutputTypeDef](./type_defs.md#listvolumesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListVolumesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    GatewayARN: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListVolumesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListVolumesOutputTypeDef](./type_defs.md#listvolumesoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListVolumesInputPaginateTypeDef = {  # (1)
    "GatewayARN": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListVolumesInputPaginateTypeDef](./type_defs.md#listvolumesinputpaginatetypedef) 
