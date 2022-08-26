# Paginators

> [Index](../README.md) > [Lightsail](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Lightsail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
    type annotations stubs module [types-aiobotocore-lightsail](https://pypi.org/project/types-aiobotocore-lightsail/).

## GetActiveNamesPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_active_names")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetActiveNames)

```python title="Usage example"
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
3. item: [:material-code-braces: GetActiveNamesResultTypeDef](./type_defs.md#getactivenamesresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetActiveNamesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetActiveNamesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetActiveNamesResultTypeDef](./type_defs.md#getactivenamesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetActiveNamesRequestGetActiveNamesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetActiveNamesRequestGetActiveNamesPaginateTypeDef](./type_defs.md#getactivenamesrequestgetactivenamespaginatetypedef) 
## GetBlueprintsPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_blueprints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetBlueprints)

```python title="Usage example"
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
3. item: [:material-code-braces: GetBlueprintsResultTypeDef](./type_defs.md#getblueprintsresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetBlueprintsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    includeInactive: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetBlueprintsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetBlueprintsResultTypeDef](./type_defs.md#getblueprintsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetBlueprintsRequestGetBlueprintsPaginateTypeDef = {  # (1)
    "includeInactive": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetBlueprintsRequestGetBlueprintsPaginateTypeDef](./type_defs.md#getblueprintsrequestgetblueprintspaginatetypedef) 
## GetBundlesPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_bundles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetBundles)

```python title="Usage example"
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
3. item: [:material-code-braces: GetBundlesResultTypeDef](./type_defs.md#getbundlesresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetBundlesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    includeInactive: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetBundlesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetBundlesResultTypeDef](./type_defs.md#getbundlesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetBundlesRequestGetBundlesPaginateTypeDef = {  # (1)
    "includeInactive": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetBundlesRequestGetBundlesPaginateTypeDef](./type_defs.md#getbundlesrequestgetbundlespaginatetypedef) 
## GetCloudFormationStackRecordsPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_cloud_formation_stack_records")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetCloudFormationStackRecords)

```python title="Usage example"
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
3. item: [:material-code-braces: GetCloudFormationStackRecordsResultTypeDef](./type_defs.md#getcloudformationstackrecordsresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetCloudFormationStackRecordsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetCloudFormationStackRecordsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetCloudFormationStackRecordsResultTypeDef](./type_defs.md#getcloudformationstackrecordsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef](./type_defs.md#getcloudformationstackrecordsrequestgetcloudformationstackrecordspaginatetypedef) 
## GetDiskSnapshotsPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_disk_snapshots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetDiskSnapshots)

```python title="Usage example"
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
3. item: [:material-code-braces: GetDiskSnapshotsResultTypeDef](./type_defs.md#getdisksnapshotsresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetDiskSnapshotsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetDiskSnapshotsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetDiskSnapshotsResultTypeDef](./type_defs.md#getdisksnapshotsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef](./type_defs.md#getdisksnapshotsrequestgetdisksnapshotspaginatetypedef) 
## GetDisksPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_disks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetDisks)

```python title="Usage example"
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
3. item: [:material-code-braces: GetDisksResultTypeDef](./type_defs.md#getdisksresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetDisksPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetDisksResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetDisksResultTypeDef](./type_defs.md#getdisksresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetDisksRequestGetDisksPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetDisksRequestGetDisksPaginateTypeDef](./type_defs.md#getdisksrequestgetdiskspaginatetypedef) 
## GetDomainsPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_domains")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetDomains)

```python title="Usage example"
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
3. item: [:material-code-braces: GetDomainsResultTypeDef](./type_defs.md#getdomainsresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetDomainsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetDomainsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetDomainsResultTypeDef](./type_defs.md#getdomainsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetDomainsRequestGetDomainsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetDomainsRequestGetDomainsPaginateTypeDef](./type_defs.md#getdomainsrequestgetdomainspaginatetypedef) 
## GetExportSnapshotRecordsPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_export_snapshot_records")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetExportSnapshotRecords)

```python title="Usage example"
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
3. item: [:material-code-braces: GetExportSnapshotRecordsResultTypeDef](./type_defs.md#getexportsnapshotrecordsresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetExportSnapshotRecordsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetExportSnapshotRecordsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetExportSnapshotRecordsResultTypeDef](./type_defs.md#getexportsnapshotrecordsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef](./type_defs.md#getexportsnapshotrecordsrequestgetexportsnapshotrecordspaginatetypedef) 
## GetInstanceSnapshotsPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_instance_snapshots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetInstanceSnapshots)

```python title="Usage example"
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
3. item: [:material-code-braces: GetInstanceSnapshotsResultTypeDef](./type_defs.md#getinstancesnapshotsresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetInstanceSnapshotsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetInstanceSnapshotsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetInstanceSnapshotsResultTypeDef](./type_defs.md#getinstancesnapshotsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef](./type_defs.md#getinstancesnapshotsrequestgetinstancesnapshotspaginatetypedef) 
## GetInstancesPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetInstances)

```python title="Usage example"
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
3. item: [:material-code-braces: GetInstancesResultTypeDef](./type_defs.md#getinstancesresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetInstancesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetInstancesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetInstancesResultTypeDef](./type_defs.md#getinstancesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetInstancesRequestGetInstancesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetInstancesRequestGetInstancesPaginateTypeDef](./type_defs.md#getinstancesrequestgetinstancespaginatetypedef) 
## GetKeyPairsPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_key_pairs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetKeyPairs)

```python title="Usage example"
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
3. item: [:material-code-braces: GetKeyPairsResultTypeDef](./type_defs.md#getkeypairsresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetKeyPairsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    includeDefaultKeyPair: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetKeyPairsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetKeyPairsResultTypeDef](./type_defs.md#getkeypairsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetKeyPairsRequestGetKeyPairsPaginateTypeDef = {  # (1)
    "includeDefaultKeyPair": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetKeyPairsRequestGetKeyPairsPaginateTypeDef](./type_defs.md#getkeypairsrequestgetkeypairspaginatetypedef) 
## GetLoadBalancersPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_load_balancers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetLoadBalancers)

```python title="Usage example"
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
3. item: [:material-code-braces: GetLoadBalancersResultTypeDef](./type_defs.md#getloadbalancersresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetLoadBalancersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetLoadBalancersResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetLoadBalancersResultTypeDef](./type_defs.md#getloadbalancersresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef](./type_defs.md#getloadbalancersrequestgetloadbalancerspaginatetypedef) 
## GetOperationsPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_operations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetOperations)

```python title="Usage example"
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
3. item: [:material-code-braces: GetOperationsResultTypeDef](./type_defs.md#getoperationsresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetOperationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetOperationsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetOperationsResultTypeDef](./type_defs.md#getoperationsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetOperationsRequestGetOperationsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetOperationsRequestGetOperationsPaginateTypeDef](./type_defs.md#getoperationsrequestgetoperationspaginatetypedef) 
## GetRelationalDatabaseBlueprintsPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_relational_database_blueprints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseBlueprints)

```python title="Usage example"
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
3. item: [:material-code-braces: GetRelationalDatabaseBlueprintsResultTypeDef](./type_defs.md#getrelationaldatabaseblueprintsresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetRelationalDatabaseBlueprintsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetRelationalDatabaseBlueprintsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetRelationalDatabaseBlueprintsResultTypeDef](./type_defs.md#getrelationaldatabaseblueprintsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef](./type_defs.md#getrelationaldatabaseblueprintsrequestgetrelationaldatabaseblueprintspaginatetypedef) 
## GetRelationalDatabaseBundlesPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_relational_database_bundles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseBundles)

```python title="Usage example"
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
3. item: [:material-code-braces: GetRelationalDatabaseBundlesResultTypeDef](./type_defs.md#getrelationaldatabasebundlesresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetRelationalDatabaseBundlesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    includeInactive: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetRelationalDatabaseBundlesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetRelationalDatabaseBundlesResultTypeDef](./type_defs.md#getrelationaldatabasebundlesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef = {  # (1)
    "includeInactive": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef](./type_defs.md#getrelationaldatabasebundlesrequestgetrelationaldatabasebundlespaginatetypedef) 
## GetRelationalDatabaseEventsPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_relational_database_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseEvents)

```python title="Usage example"
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
3. item: [:material-code-braces: GetRelationalDatabaseEventsResultTypeDef](./type_defs.md#getrelationaldatabaseeventsresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetRelationalDatabaseEventsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    relationalDatabaseName: str,
    durationInMinutes: int = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetRelationalDatabaseEventsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetRelationalDatabaseEventsResultTypeDef](./type_defs.md#getrelationaldatabaseeventsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef = {  # (1)
    "relationalDatabaseName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef](./type_defs.md#getrelationaldatabaseeventsrequestgetrelationaldatabaseeventspaginatetypedef) 
## GetRelationalDatabaseParametersPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_relational_database_parameters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseParameters)

```python title="Usage example"
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
3. item: [:material-code-braces: GetRelationalDatabaseParametersResultTypeDef](./type_defs.md#getrelationaldatabaseparametersresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetRelationalDatabaseParametersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    relationalDatabaseName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetRelationalDatabaseParametersResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetRelationalDatabaseParametersResultTypeDef](./type_defs.md#getrelationaldatabaseparametersresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef = {  # (1)
    "relationalDatabaseName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef](./type_defs.md#getrelationaldatabaseparametersrequestgetrelationaldatabaseparameterspaginatetypedef) 
## GetRelationalDatabaseSnapshotsPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_relational_database_snapshots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseSnapshots)

```python title="Usage example"
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
3. item: [:material-code-braces: GetRelationalDatabaseSnapshotsResultTypeDef](./type_defs.md#getrelationaldatabasesnapshotsresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetRelationalDatabaseSnapshotsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetRelationalDatabaseSnapshotsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetRelationalDatabaseSnapshotsResultTypeDef](./type_defs.md#getrelationaldatabasesnapshotsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef](./type_defs.md#getrelationaldatabasesnapshotsrequestgetrelationaldatabasesnapshotspaginatetypedef) 
## GetRelationalDatabasesPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_relational_databases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabases)

```python title="Usage example"
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
3. item: [:material-code-braces: GetRelationalDatabasesResultTypeDef](./type_defs.md#getrelationaldatabasesresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetRelationalDatabasesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetRelationalDatabasesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetRelationalDatabasesResultTypeDef](./type_defs.md#getrelationaldatabasesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef](./type_defs.md#getrelationaldatabasesrequestgetrelationaldatabasespaginatetypedef) 
## GetStaticIpsPaginator

Type annotations and code completion for `#!python session.create_client("lightsail").get_paginator("get_static_ips")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetStaticIps)

```python title="Usage example"
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
3. item: [:material-code-braces: GetStaticIpsResultTypeDef](./type_defs.md#getstaticipsresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetStaticIpsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetStaticIpsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetStaticIpsResultTypeDef](./type_defs.md#getstaticipsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetStaticIpsRequestGetStaticIpsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetStaticIpsRequestGetStaticIpsPaginateTypeDef](./type_defs.md#getstaticipsrequestgetstaticipspaginatetypedef) 
