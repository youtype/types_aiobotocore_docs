# Paginators

> [Index](../README.md) > [Lightsail](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Lightsail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#lightsail)
    type annotations stubs module [types-aiobotocore-lightsail](https://pypi.org/project/types-aiobotocore-lightsail/).

## GetActiveNamesPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_active_names")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail/paginator/GetActiveNames.html#Lightsail.Paginator.GetActiveNames)

```python
# GetActiveNamesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetActiveNamesPaginator

session = get_session()
async with session.create_client("lightsail") as client:  # (1)
    paginator: GetActiveNamesPaginator = client.get_paginator("get_active_names")  # (2)
    async for item in paginator.paginate(...):
        item: GetActiveNamesResultTypeDef
        print(item)  # (3)
```

1. client: [LightsailClient](./client.md)
2. paginator: [GetActiveNamesPaginator](./paginators.md#getactivenamespaginator)
3. item: `AioPageIterator[GetActiveNamesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetActiveNamesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetActiveNamesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetActiveNamesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetActiveNamesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetActiveNamesRequestPaginateTypeDef](./type_defs.md#getactivenamesrequestpaginatetypedef)
## GetBlueprintsPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_blueprints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail/paginator/GetBlueprints.html#Lightsail.Paginator.GetBlueprints)

```python
# GetBlueprintsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetBlueprintsPaginator

session = get_session()
async with session.create_client("lightsail") as client:  # (1)
    paginator: GetBlueprintsPaginator = client.get_paginator("get_blueprints")  # (2)
    async for item in paginator.paginate(...):
        item: GetBlueprintsResultTypeDef
        print(item)  # (3)
```

1. client: [LightsailClient](./client.md)
2. paginator: [GetBlueprintsPaginator](./paginators.md#getblueprintspaginator)
3. item: `AioPageIterator[GetBlueprintsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetBlueprintsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    includeInactive: bool = ...,
    appCategory: AppCategoryType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[GetBlueprintsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: AppCategoryType](./literals.md#appcategorytype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[GetBlueprintsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetBlueprintsRequestPaginateTypeDef = {  # (1)
    "includeInactive": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetBlueprintsRequestPaginateTypeDef](./type_defs.md#getblueprintsrequestpaginatetypedef)
## GetBundlesPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_bundles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail/paginator/GetBundles.html#Lightsail.Paginator.GetBundles)

```python
# GetBundlesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetBundlesPaginator

session = get_session()
async with session.create_client("lightsail") as client:  # (1)
    paginator: GetBundlesPaginator = client.get_paginator("get_bundles")  # (2)
    async for item in paginator.paginate(...):
        item: GetBundlesResultTypeDef
        print(item)  # (3)
```

1. client: [LightsailClient](./client.md)
2. paginator: [GetBundlesPaginator](./paginators.md#getbundlespaginator)
3. item: `AioPageIterator[GetBundlesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetBundlesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    includeInactive: bool = ...,
    appCategory: AppCategoryType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[GetBundlesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: AppCategoryType](./literals.md#appcategorytype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[GetBundlesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetBundlesRequestPaginateTypeDef = {  # (1)
    "includeInactive": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetBundlesRequestPaginateTypeDef](./type_defs.md#getbundlesrequestpaginatetypedef)
## GetCloudFormationStackRecordsPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_cloud_formation_stack_records")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail/paginator/GetCloudFormationStackRecords.html#Lightsail.Paginator.GetCloudFormationStackRecords)

```python
# GetCloudFormationStackRecordsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetCloudFormationStackRecordsPaginator

session = get_session()
async with session.create_client("lightsail") as client:  # (1)
    paginator: GetCloudFormationStackRecordsPaginator = client.get_paginator("get_cloud_formation_stack_records")  # (2)
    async for item in paginator.paginate(...):
        item: GetCloudFormationStackRecordsResultTypeDef
        print(item)  # (3)
```

1. client: [LightsailClient](./client.md)
2. paginator: [GetCloudFormationStackRecordsPaginator](./paginators.md#getcloudformationstackrecordspaginator)
3. item: `AioPageIterator[GetCloudFormationStackRecordsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetCloudFormationStackRecordsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetCloudFormationStackRecordsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetCloudFormationStackRecordsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetCloudFormationStackRecordsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetCloudFormationStackRecordsRequestPaginateTypeDef](./type_defs.md#getcloudformationstackrecordsrequestpaginatetypedef)
## GetDiskSnapshotsPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_disk_snapshots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail/paginator/GetDiskSnapshots.html#Lightsail.Paginator.GetDiskSnapshots)

```python
# GetDiskSnapshotsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetDiskSnapshotsPaginator

session = get_session()
async with session.create_client("lightsail") as client:  # (1)
    paginator: GetDiskSnapshotsPaginator = client.get_paginator("get_disk_snapshots")  # (2)
    async for item in paginator.paginate(...):
        item: GetDiskSnapshotsResultTypeDef
        print(item)  # (3)
```

1. client: [LightsailClient](./client.md)
2. paginator: [GetDiskSnapshotsPaginator](./paginators.md#getdisksnapshotspaginator)
3. item: `AioPageIterator[GetDiskSnapshotsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetDiskSnapshotsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetDiskSnapshotsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetDiskSnapshotsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetDiskSnapshotsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetDiskSnapshotsRequestPaginateTypeDef](./type_defs.md#getdisksnapshotsrequestpaginatetypedef)
## GetDisksPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_disks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail/paginator/GetDisks.html#Lightsail.Paginator.GetDisks)

```python
# GetDisksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetDisksPaginator

session = get_session()
async with session.create_client("lightsail") as client:  # (1)
    paginator: GetDisksPaginator = client.get_paginator("get_disks")  # (2)
    async for item in paginator.paginate(...):
        item: GetDisksResultTypeDef
        print(item)  # (3)
```

1. client: [LightsailClient](./client.md)
2. paginator: [GetDisksPaginator](./paginators.md#getdiskspaginator)
3. item: `AioPageIterator[GetDisksResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetDisksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetDisksResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetDisksResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetDisksRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetDisksRequestPaginateTypeDef](./type_defs.md#getdisksrequestpaginatetypedef)
## GetDomainsPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_domains")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail/paginator/GetDomains.html#Lightsail.Paginator.GetDomains)

```python
# GetDomainsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetDomainsPaginator

session = get_session()
async with session.create_client("lightsail") as client:  # (1)
    paginator: GetDomainsPaginator = client.get_paginator("get_domains")  # (2)
    async for item in paginator.paginate(...):
        item: GetDomainsResultTypeDef
        print(item)  # (3)
```

1. client: [LightsailClient](./client.md)
2. paginator: [GetDomainsPaginator](./paginators.md#getdomainspaginator)
3. item: `AioPageIterator[GetDomainsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetDomainsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetDomainsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetDomainsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetDomainsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetDomainsRequestPaginateTypeDef](./type_defs.md#getdomainsrequestpaginatetypedef)
## GetExportSnapshotRecordsPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_export_snapshot_records")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail/paginator/GetExportSnapshotRecords.html#Lightsail.Paginator.GetExportSnapshotRecords)

```python
# GetExportSnapshotRecordsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetExportSnapshotRecordsPaginator

session = get_session()
async with session.create_client("lightsail") as client:  # (1)
    paginator: GetExportSnapshotRecordsPaginator = client.get_paginator("get_export_snapshot_records")  # (2)
    async for item in paginator.paginate(...):
        item: GetExportSnapshotRecordsResultTypeDef
        print(item)  # (3)
```

1. client: [LightsailClient](./client.md)
2. paginator: [GetExportSnapshotRecordsPaginator](./paginators.md#getexportsnapshotrecordspaginator)
3. item: `AioPageIterator[GetExportSnapshotRecordsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetExportSnapshotRecordsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetExportSnapshotRecordsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetExportSnapshotRecordsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetExportSnapshotRecordsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetExportSnapshotRecordsRequestPaginateTypeDef](./type_defs.md#getexportsnapshotrecordsrequestpaginatetypedef)
## GetInstanceSnapshotsPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_instance_snapshots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail/paginator/GetInstanceSnapshots.html#Lightsail.Paginator.GetInstanceSnapshots)

```python
# GetInstanceSnapshotsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetInstanceSnapshotsPaginator

session = get_session()
async with session.create_client("lightsail") as client:  # (1)
    paginator: GetInstanceSnapshotsPaginator = client.get_paginator("get_instance_snapshots")  # (2)
    async for item in paginator.paginate(...):
        item: GetInstanceSnapshotsResultTypeDef
        print(item)  # (3)
```

1. client: [LightsailClient](./client.md)
2. paginator: [GetInstanceSnapshotsPaginator](./paginators.md#getinstancesnapshotspaginator)
3. item: `AioPageIterator[GetInstanceSnapshotsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetInstanceSnapshotsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetInstanceSnapshotsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetInstanceSnapshotsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetInstanceSnapshotsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetInstanceSnapshotsRequestPaginateTypeDef](./type_defs.md#getinstancesnapshotsrequestpaginatetypedef)
## GetInstancesPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail/paginator/GetInstances.html#Lightsail.Paginator.GetInstances)

```python
# GetInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetInstancesPaginator

session = get_session()
async with session.create_client("lightsail") as client:  # (1)
    paginator: GetInstancesPaginator = client.get_paginator("get_instances")  # (2)
    async for item in paginator.paginate(...):
        item: GetInstancesResultTypeDef
        print(item)  # (3)
```

1. client: [LightsailClient](./client.md)
2. paginator: [GetInstancesPaginator](./paginators.md#getinstancespaginator)
3. item: `AioPageIterator[GetInstancesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetInstancesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetInstancesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetInstancesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetInstancesRequestPaginateTypeDef](./type_defs.md#getinstancesrequestpaginatetypedef)
## GetKeyPairsPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_key_pairs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail/paginator/GetKeyPairs.html#Lightsail.Paginator.GetKeyPairs)

```python
# GetKeyPairsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetKeyPairsPaginator

session = get_session()
async with session.create_client("lightsail") as client:  # (1)
    paginator: GetKeyPairsPaginator = client.get_paginator("get_key_pairs")  # (2)
    async for item in paginator.paginate(...):
        item: GetKeyPairsResultTypeDef
        print(item)  # (3)
```

1. client: [LightsailClient](./client.md)
2. paginator: [GetKeyPairsPaginator](./paginators.md#getkeypairspaginator)
3. item: `AioPageIterator[GetKeyPairsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetKeyPairsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    includeDefaultKeyPair: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetKeyPairsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetKeyPairsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetKeyPairsRequestPaginateTypeDef = {  # (1)
    "includeDefaultKeyPair": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetKeyPairsRequestPaginateTypeDef](./type_defs.md#getkeypairsrequestpaginatetypedef)
## GetLoadBalancersPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_load_balancers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail/paginator/GetLoadBalancers.html#Lightsail.Paginator.GetLoadBalancers)

```python
# GetLoadBalancersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetLoadBalancersPaginator

session = get_session()
async with session.create_client("lightsail") as client:  # (1)
    paginator: GetLoadBalancersPaginator = client.get_paginator("get_load_balancers")  # (2)
    async for item in paginator.paginate(...):
        item: GetLoadBalancersResultTypeDef
        print(item)  # (3)
```

1. client: [LightsailClient](./client.md)
2. paginator: [GetLoadBalancersPaginator](./paginators.md#getloadbalancerspaginator)
3. item: `AioPageIterator[GetLoadBalancersResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetLoadBalancersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetLoadBalancersResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetLoadBalancersResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetLoadBalancersRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetLoadBalancersRequestPaginateTypeDef](./type_defs.md#getloadbalancersrequestpaginatetypedef)
## GetOperationsPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_operations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail/paginator/GetOperations.html#Lightsail.Paginator.GetOperations)

```python
# GetOperationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetOperationsPaginator

session = get_session()
async with session.create_client("lightsail") as client:  # (1)
    paginator: GetOperationsPaginator = client.get_paginator("get_operations")  # (2)
    async for item in paginator.paginate(...):
        item: GetOperationsResultTypeDef
        print(item)  # (3)
```

1. client: [LightsailClient](./client.md)
2. paginator: [GetOperationsPaginator](./paginators.md#getoperationspaginator)
3. item: `AioPageIterator[GetOperationsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetOperationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetOperationsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetOperationsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetOperationsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetOperationsRequestPaginateTypeDef](./type_defs.md#getoperationsrequestpaginatetypedef)
## GetRelationalDatabaseBlueprintsPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_relational_database_blueprints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail/paginator/GetRelationalDatabaseBlueprints.html#Lightsail.Paginator.GetRelationalDatabaseBlueprints)

```python
# GetRelationalDatabaseBlueprintsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetRelationalDatabaseBlueprintsPaginator

session = get_session()
async with session.create_client("lightsail") as client:  # (1)
    paginator: GetRelationalDatabaseBlueprintsPaginator = client.get_paginator("get_relational_database_blueprints")  # (2)
    async for item in paginator.paginate(...):
        item: GetRelationalDatabaseBlueprintsResultTypeDef
        print(item)  # (3)
```

1. client: [LightsailClient](./client.md)
2. paginator: [GetRelationalDatabaseBlueprintsPaginator](./paginators.md#getrelationaldatabaseblueprintspaginator)
3. item: `AioPageIterator[GetRelationalDatabaseBlueprintsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetRelationalDatabaseBlueprintsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetRelationalDatabaseBlueprintsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetRelationalDatabaseBlueprintsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetRelationalDatabaseBlueprintsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetRelationalDatabaseBlueprintsRequestPaginateTypeDef](./type_defs.md#getrelationaldatabaseblueprintsrequestpaginatetypedef)
## GetRelationalDatabaseBundlesPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_relational_database_bundles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail/paginator/GetRelationalDatabaseBundles.html#Lightsail.Paginator.GetRelationalDatabaseBundles)

```python
# GetRelationalDatabaseBundlesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetRelationalDatabaseBundlesPaginator

session = get_session()
async with session.create_client("lightsail") as client:  # (1)
    paginator: GetRelationalDatabaseBundlesPaginator = client.get_paginator("get_relational_database_bundles")  # (2)
    async for item in paginator.paginate(...):
        item: GetRelationalDatabaseBundlesResultTypeDef
        print(item)  # (3)
```

1. client: [LightsailClient](./client.md)
2. paginator: [GetRelationalDatabaseBundlesPaginator](./paginators.md#getrelationaldatabasebundlespaginator)
3. item: `AioPageIterator[GetRelationalDatabaseBundlesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetRelationalDatabaseBundlesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    includeInactive: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetRelationalDatabaseBundlesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetRelationalDatabaseBundlesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetRelationalDatabaseBundlesRequestPaginateTypeDef = {  # (1)
    "includeInactive": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetRelationalDatabaseBundlesRequestPaginateTypeDef](./type_defs.md#getrelationaldatabasebundlesrequestpaginatetypedef)
## GetRelationalDatabaseEventsPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_relational_database_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail/paginator/GetRelationalDatabaseEvents.html#Lightsail.Paginator.GetRelationalDatabaseEvents)

```python
# GetRelationalDatabaseEventsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetRelationalDatabaseEventsPaginator

session = get_session()
async with session.create_client("lightsail") as client:  # (1)
    paginator: GetRelationalDatabaseEventsPaginator = client.get_paginator("get_relational_database_events")  # (2)
    async for item in paginator.paginate(...):
        item: GetRelationalDatabaseEventsResultTypeDef
        print(item)  # (3)
```

1. client: [LightsailClient](./client.md)
2. paginator: [GetRelationalDatabaseEventsPaginator](./paginators.md#getrelationaldatabaseeventspaginator)
3. item: `AioPageIterator[GetRelationalDatabaseEventsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetRelationalDatabaseEventsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    relationalDatabaseName: str,
    durationInMinutes: int = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetRelationalDatabaseEventsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetRelationalDatabaseEventsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetRelationalDatabaseEventsRequestPaginateTypeDef = {  # (1)
    "relationalDatabaseName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetRelationalDatabaseEventsRequestPaginateTypeDef](./type_defs.md#getrelationaldatabaseeventsrequestpaginatetypedef)
## GetRelationalDatabaseParametersPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_relational_database_parameters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail/paginator/GetRelationalDatabaseParameters.html#Lightsail.Paginator.GetRelationalDatabaseParameters)

```python
# GetRelationalDatabaseParametersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetRelationalDatabaseParametersPaginator

session = get_session()
async with session.create_client("lightsail") as client:  # (1)
    paginator: GetRelationalDatabaseParametersPaginator = client.get_paginator("get_relational_database_parameters")  # (2)
    async for item in paginator.paginate(...):
        item: GetRelationalDatabaseParametersResultTypeDef
        print(item)  # (3)
```

1. client: [LightsailClient](./client.md)
2. paginator: [GetRelationalDatabaseParametersPaginator](./paginators.md#getrelationaldatabaseparameterspaginator)
3. item: `AioPageIterator[GetRelationalDatabaseParametersResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetRelationalDatabaseParametersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    relationalDatabaseName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetRelationalDatabaseParametersResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetRelationalDatabaseParametersResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetRelationalDatabaseParametersRequestPaginateTypeDef = {  # (1)
    "relationalDatabaseName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetRelationalDatabaseParametersRequestPaginateTypeDef](./type_defs.md#getrelationaldatabaseparametersrequestpaginatetypedef)
## GetRelationalDatabaseSnapshotsPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_relational_database_snapshots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail/paginator/GetRelationalDatabaseSnapshots.html#Lightsail.Paginator.GetRelationalDatabaseSnapshots)

```python
# GetRelationalDatabaseSnapshotsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetRelationalDatabaseSnapshotsPaginator

session = get_session()
async with session.create_client("lightsail") as client:  # (1)
    paginator: GetRelationalDatabaseSnapshotsPaginator = client.get_paginator("get_relational_database_snapshots")  # (2)
    async for item in paginator.paginate(...):
        item: GetRelationalDatabaseSnapshotsResultTypeDef
        print(item)  # (3)
```

1. client: [LightsailClient](./client.md)
2. paginator: [GetRelationalDatabaseSnapshotsPaginator](./paginators.md#getrelationaldatabasesnapshotspaginator)
3. item: `AioPageIterator[GetRelationalDatabaseSnapshotsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetRelationalDatabaseSnapshotsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetRelationalDatabaseSnapshotsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetRelationalDatabaseSnapshotsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetRelationalDatabaseSnapshotsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetRelationalDatabaseSnapshotsRequestPaginateTypeDef](./type_defs.md#getrelationaldatabasesnapshotsrequestpaginatetypedef)
## GetRelationalDatabasesPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_relational_databases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail/paginator/GetRelationalDatabases.html#Lightsail.Paginator.GetRelationalDatabases)

```python
# GetRelationalDatabasesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetRelationalDatabasesPaginator

session = get_session()
async with session.create_client("lightsail") as client:  # (1)
    paginator: GetRelationalDatabasesPaginator = client.get_paginator("get_relational_databases")  # (2)
    async for item in paginator.paginate(...):
        item: GetRelationalDatabasesResultTypeDef
        print(item)  # (3)
```

1. client: [LightsailClient](./client.md)
2. paginator: [GetRelationalDatabasesPaginator](./paginators.md#getrelationaldatabasespaginator)
3. item: `AioPageIterator[GetRelationalDatabasesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetRelationalDatabasesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetRelationalDatabasesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetRelationalDatabasesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetRelationalDatabasesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetRelationalDatabasesRequestPaginateTypeDef](./type_defs.md#getrelationaldatabasesrequestpaginatetypedef)
## GetStaticIpsPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_static_ips")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail/paginator/GetStaticIps.html#Lightsail.Paginator.GetStaticIps)

```python
# GetStaticIpsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_lightsail.paginator import GetStaticIpsPaginator

session = get_session()
async with session.create_client("lightsail") as client:  # (1)
    paginator: GetStaticIpsPaginator = client.get_paginator("get_static_ips")  # (2)
    async for item in paginator.paginate(...):
        item: GetStaticIpsResultTypeDef
        print(item)  # (3)
```

1. client: [LightsailClient](./client.md)
2. paginator: [GetStaticIpsPaginator](./paginators.md#getstaticipspaginator)
3. item: `AioPageIterator[GetStaticIpsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetStaticIpsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetStaticIpsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetStaticIpsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetStaticIpsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetStaticIpsRequestPaginateTypeDef](./type_defs.md#getstaticipsrequestpaginatetypedef)
