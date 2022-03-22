<a id="paginators-for-aiobotocore-storagegateway-module"></a>

# Paginators for aiobotocore StorageGateway module

> [Index](../README.md) > [StorageGateway](./README.md) > Paginators

Auto-generated documentation for
[StorageGateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway)
type annotations stubs module
[types-aiobotocore-storagegateway](https://pypi.org/project/types-aiobotocore-storagegateway/).

- [Paginators for aiobotocore StorageGateway module](#paginators-for-aiobotocore-storagegateway-module)
  - [DescribeTapeArchivesPaginator](#describetapearchivespaginator)
  - [DescribeTapeRecoveryPointsPaginator](#describetaperecoverypointspaginator)
  - [DescribeTapesPaginator](#describetapespaginator)
  - [DescribeVTLDevicesPaginator](#describevtldevicespaginator)
  - [ListFileSharesPaginator](#listfilesharespaginator)
  - [ListFileSystemAssociationsPaginator](#listfilesystemassociationspaginator)
  - [ListGatewaysPaginator](#listgatewayspaginator)
  - [ListTagsForResourcePaginator](#listtagsforresourcepaginator)
  - [ListTapePoolsPaginator](#listtapepoolspaginator)
  - [ListTapesPaginator](#listtapespaginator)
  - [ListVolumesPaginator](#listvolumespaginator)

<a id="describetapearchivespaginator"></a>

## DescribeTapeArchivesPaginator

Type annotations for
`session.create_client("storagegateway").get_paginator("describe_tape_archives")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_storagegateway.paginator import DescribeTapeArchivesPaginator

session = get_session()
async with session.create_client("storagegateway") as client:
    client: StorageGatewayClient
    paginator: DescribeTapeArchivesPaginator = client.get_paginator("describe_tape_archives")
```

Boto3 documentation:
[StorageGateway.Paginator.DescribeTapeArchives](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapeArchives)

Arguments for `DescribeTapeArchivesPaginator.paginate` method:

- `TapeARNs`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeTapeArchivesPaginator.paginate` returns
`AsyncIterator`\[[DescribeTapeArchivesOutputTypeDef](./type_defs.md#describetapearchivesoutputtypedef)\].

<a id="describetaperecoverypointspaginator"></a>

## DescribeTapeRecoveryPointsPaginator

Type annotations for
`session.create_client("storagegateway").get_paginator("describe_tape_recovery_points")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_storagegateway.paginator import DescribeTapeRecoveryPointsPaginator

session = get_session()
async with session.create_client("storagegateway") as client:
    client: StorageGatewayClient
    paginator: DescribeTapeRecoveryPointsPaginator = client.get_paginator("describe_tape_recovery_points")
```

Boto3 documentation:
[StorageGateway.Paginator.DescribeTapeRecoveryPoints](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapeRecoveryPoints)

Arguments for `DescribeTapeRecoveryPointsPaginator.paginate` method:

- `GatewayARN`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeTapeRecoveryPointsPaginator.paginate` returns
`AsyncIterator`\[[DescribeTapeRecoveryPointsOutputTypeDef](./type_defs.md#describetaperecoverypointsoutputtypedef)\].

<a id="describetapespaginator"></a>

## DescribeTapesPaginator

Type annotations for
`session.create_client("storagegateway").get_paginator("describe_tapes")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_storagegateway.paginator import DescribeTapesPaginator

session = get_session()
async with session.create_client("storagegateway") as client:
    client: StorageGatewayClient
    paginator: DescribeTapesPaginator = client.get_paginator("describe_tapes")
```

Boto3 documentation:
[StorageGateway.Paginator.DescribeTapes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeTapes)

Arguments for `DescribeTapesPaginator.paginate` method:

- `GatewayARN`: `str` *(required)*
- `TapeARNs`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeTapesPaginator.paginate` returns
`AsyncIterator`\[[DescribeTapesOutputTypeDef](./type_defs.md#describetapesoutputtypedef)\].

<a id="describevtldevicespaginator"></a>

## DescribeVTLDevicesPaginator

Type annotations for
`session.create_client("storagegateway").get_paginator("describe_vtl_devices")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_storagegateway.paginator import DescribeVTLDevicesPaginator

session = get_session()
async with session.create_client("storagegateway") as client:
    client: StorageGatewayClient
    paginator: DescribeVTLDevicesPaginator = client.get_paginator("describe_vtl_devices")
```

Boto3 documentation:
[StorageGateway.Paginator.DescribeVTLDevices](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.DescribeVTLDevices)

Arguments for `DescribeVTLDevicesPaginator.paginate` method:

- `GatewayARN`: `str` *(required)*
- `VTLDeviceARNs`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeVTLDevicesPaginator.paginate` returns
`AsyncIterator`\[[DescribeVTLDevicesOutputTypeDef](./type_defs.md#describevtldevicesoutputtypedef)\].

<a id="listfilesharespaginator"></a>

## ListFileSharesPaginator

Type annotations for
`session.create_client("storagegateway").get_paginator("list_file_shares")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_storagegateway.paginator import ListFileSharesPaginator

session = get_session()
async with session.create_client("storagegateway") as client:
    client: StorageGatewayClient
    paginator: ListFileSharesPaginator = client.get_paginator("list_file_shares")
```

Boto3 documentation:
[StorageGateway.Paginator.ListFileShares](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListFileShares)

Arguments for `ListFileSharesPaginator.paginate` method:

- `GatewayARN`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListFileSharesPaginator.paginate` returns
`AsyncIterator`\[[ListFileSharesOutputTypeDef](./type_defs.md#listfilesharesoutputtypedef)\].

<a id="listfilesystemassociationspaginator"></a>

## ListFileSystemAssociationsPaginator

Type annotations for
`session.create_client("storagegateway").get_paginator("list_file_system_associations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_storagegateway.paginator import ListFileSystemAssociationsPaginator

session = get_session()
async with session.create_client("storagegateway") as client:
    client: StorageGatewayClient
    paginator: ListFileSystemAssociationsPaginator = client.get_paginator("list_file_system_associations")
```

Boto3 documentation:
[StorageGateway.Paginator.ListFileSystemAssociations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListFileSystemAssociations)

Arguments for `ListFileSystemAssociationsPaginator.paginate` method:

- `GatewayARN`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListFileSystemAssociationsPaginator.paginate` returns
`AsyncIterator`\[[ListFileSystemAssociationsOutputTypeDef](./type_defs.md#listfilesystemassociationsoutputtypedef)\].

<a id="listgatewayspaginator"></a>

## ListGatewaysPaginator

Type annotations for
`session.create_client("storagegateway").get_paginator("list_gateways")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_storagegateway.paginator import ListGatewaysPaginator

session = get_session()
async with session.create_client("storagegateway") as client:
    client: StorageGatewayClient
    paginator: ListGatewaysPaginator = client.get_paginator("list_gateways")
```

Boto3 documentation:
[StorageGateway.Paginator.ListGateways](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListGateways)

Arguments for `ListGatewaysPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListGatewaysPaginator.paginate` returns
`AsyncIterator`\[[ListGatewaysOutputTypeDef](./type_defs.md#listgatewaysoutputtypedef)\].

<a id="listtagsforresourcepaginator"></a>

## ListTagsForResourcePaginator

Type annotations for
`session.create_client("storagegateway").get_paginator("list_tags_for_resource")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_storagegateway.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("storagegateway") as client:
    client: StorageGatewayClient
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
```

Boto3 documentation:
[StorageGateway.Paginator.ListTagsForResource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTagsForResource)

Arguments for `ListTagsForResourcePaginator.paginate` method:

- `ResourceARN`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTagsForResourcePaginator.paginate` returns
`AsyncIterator`\[[ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)\].

<a id="listtapepoolspaginator"></a>

## ListTapePoolsPaginator

Type annotations for
`session.create_client("storagegateway").get_paginator("list_tape_pools")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_storagegateway.paginator import ListTapePoolsPaginator

session = get_session()
async with session.create_client("storagegateway") as client:
    client: StorageGatewayClient
    paginator: ListTapePoolsPaginator = client.get_paginator("list_tape_pools")
```

Boto3 documentation:
[StorageGateway.Paginator.ListTapePools](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTapePools)

Arguments for `ListTapePoolsPaginator.paginate` method:

- `PoolARNs`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTapePoolsPaginator.paginate` returns
`AsyncIterator`\[[ListTapePoolsOutputTypeDef](./type_defs.md#listtapepoolsoutputtypedef)\].

<a id="listtapespaginator"></a>

## ListTapesPaginator

Type annotations for
`session.create_client("storagegateway").get_paginator("list_tapes")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_storagegateway.paginator import ListTapesPaginator

session = get_session()
async with session.create_client("storagegateway") as client:
    client: StorageGatewayClient
    paginator: ListTapesPaginator = client.get_paginator("list_tapes")
```

Boto3 documentation:
[StorageGateway.Paginator.ListTapes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListTapes)

Arguments for `ListTapesPaginator.paginate` method:

- `TapeARNs`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTapesPaginator.paginate` returns
`AsyncIterator`\[[ListTapesOutputTypeDef](./type_defs.md#listtapesoutputtypedef)\].

<a id="listvolumespaginator"></a>

## ListVolumesPaginator

Type annotations for
`session.create_client("storagegateway").get_paginator("list_volumes")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_storagegateway.paginator import ListVolumesPaginator

session = get_session()
async with session.create_client("storagegateway") as client:
    client: StorageGatewayClient
    paginator: ListVolumesPaginator = client.get_paginator("list_volumes")
```

Boto3 documentation:
[StorageGateway.Paginator.ListVolumes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#StorageGateway.Paginator.ListVolumes)

Arguments for `ListVolumesPaginator.paginate` method:

- `GatewayARN`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListVolumesPaginator.paginate` returns
`AsyncIterator`\[[ListVolumesOutputTypeDef](./type_defs.md#listvolumesoutputtypedef)\].
