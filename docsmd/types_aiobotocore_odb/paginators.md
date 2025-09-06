# Paginators

> [Index](../README.md) > [Odb](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Odb](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb.html#odb)
    type annotations stubs module [types-aiobotocore-odb](https://pypi.org/project/types-aiobotocore-odb/).

## ListAutonomousVirtualMachinesPaginator

Type annotations and code completion for `#!python session.create_client("odb").get_paginator("list_autonomous_virtual_machines")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/paginator/ListAutonomousVirtualMachines.html#Odb.Paginator.ListAutonomousVirtualMachines)

```python
# ListAutonomousVirtualMachinesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_odb.paginator import ListAutonomousVirtualMachinesPaginator

session = get_session()
async with session.create_client("odb") as client:  # (1)
    paginator: ListAutonomousVirtualMachinesPaginator = client.get_paginator("list_autonomous_virtual_machines")  # (2)
    async for item in paginator.paginate(...):
        item: ListAutonomousVirtualMachinesOutputTypeDef
        print(item)  # (3)
```

1. client: [OdbClient](./client.md)
2. paginator: [ListAutonomousVirtualMachinesPaginator](./paginators.md#listautonomousvirtualmachinespaginator)
3. item: `AioPageIterator[ListAutonomousVirtualMachinesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAutonomousVirtualMachinesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    cloudAutonomousVmClusterId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAutonomousVirtualMachinesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAutonomousVirtualMachinesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAutonomousVirtualMachinesInputPaginateTypeDef = {  # (1)
    "cloudAutonomousVmClusterId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAutonomousVirtualMachinesInputPaginateTypeDef](./type_defs.md#listautonomousvirtualmachinesinputpaginatetypedef)
## ListCloudAutonomousVmClustersPaginator

Type annotations and code completion for `#!python session.create_client("odb").get_paginator("list_cloud_autonomous_vm_clusters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/paginator/ListCloudAutonomousVmClusters.html#Odb.Paginator.ListCloudAutonomousVmClusters)

```python
# ListCloudAutonomousVmClustersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_odb.paginator import ListCloudAutonomousVmClustersPaginator

session = get_session()
async with session.create_client("odb") as client:  # (1)
    paginator: ListCloudAutonomousVmClustersPaginator = client.get_paginator("list_cloud_autonomous_vm_clusters")  # (2)
    async for item in paginator.paginate(...):
        item: ListCloudAutonomousVmClustersOutputTypeDef
        print(item)  # (3)
```

1. client: [OdbClient](./client.md)
2. paginator: [ListCloudAutonomousVmClustersPaginator](./paginators.md#listcloudautonomousvmclusterspaginator)
3. item: `AioPageIterator[ListCloudAutonomousVmClustersOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCloudAutonomousVmClustersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    cloudExadataInfrastructureId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListCloudAutonomousVmClustersOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListCloudAutonomousVmClustersOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCloudAutonomousVmClustersInputPaginateTypeDef = {  # (1)
    "cloudExadataInfrastructureId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCloudAutonomousVmClustersInputPaginateTypeDef](./type_defs.md#listcloudautonomousvmclustersinputpaginatetypedef)
## ListCloudExadataInfrastructuresPaginator

Type annotations and code completion for `#!python session.create_client("odb").get_paginator("list_cloud_exadata_infrastructures")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/paginator/ListCloudExadataInfrastructures.html#Odb.Paginator.ListCloudExadataInfrastructures)

```python
# ListCloudExadataInfrastructuresPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_odb.paginator import ListCloudExadataInfrastructuresPaginator

session = get_session()
async with session.create_client("odb") as client:  # (1)
    paginator: ListCloudExadataInfrastructuresPaginator = client.get_paginator("list_cloud_exadata_infrastructures")  # (2)
    async for item in paginator.paginate(...):
        item: ListCloudExadataInfrastructuresOutputTypeDef
        print(item)  # (3)
```

1. client: [OdbClient](./client.md)
2. paginator: [ListCloudExadataInfrastructuresPaginator](./paginators.md#listcloudexadatainfrastructurespaginator)
3. item: `AioPageIterator[ListCloudExadataInfrastructuresOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCloudExadataInfrastructuresPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListCloudExadataInfrastructuresOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListCloudExadataInfrastructuresOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCloudExadataInfrastructuresInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCloudExadataInfrastructuresInputPaginateTypeDef](./type_defs.md#listcloudexadatainfrastructuresinputpaginatetypedef)
## ListCloudVmClustersPaginator

Type annotations and code completion for `#!python session.create_client("odb").get_paginator("list_cloud_vm_clusters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/paginator/ListCloudVmClusters.html#Odb.Paginator.ListCloudVmClusters)

```python
# ListCloudVmClustersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_odb.paginator import ListCloudVmClustersPaginator

session = get_session()
async with session.create_client("odb") as client:  # (1)
    paginator: ListCloudVmClustersPaginator = client.get_paginator("list_cloud_vm_clusters")  # (2)
    async for item in paginator.paginate(...):
        item: ListCloudVmClustersOutputTypeDef
        print(item)  # (3)
```

1. client: [OdbClient](./client.md)
2. paginator: [ListCloudVmClustersPaginator](./paginators.md#listcloudvmclusterspaginator)
3. item: `AioPageIterator[ListCloudVmClustersOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCloudVmClustersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    cloudExadataInfrastructureId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListCloudVmClustersOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListCloudVmClustersOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCloudVmClustersInputPaginateTypeDef = {  # (1)
    "cloudExadataInfrastructureId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCloudVmClustersInputPaginateTypeDef](./type_defs.md#listcloudvmclustersinputpaginatetypedef)
## ListDbNodesPaginator

Type annotations and code completion for `#!python session.create_client("odb").get_paginator("list_db_nodes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/paginator/ListDbNodes.html#Odb.Paginator.ListDbNodes)

```python
# ListDbNodesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_odb.paginator import ListDbNodesPaginator

session = get_session()
async with session.create_client("odb") as client:  # (1)
    paginator: ListDbNodesPaginator = client.get_paginator("list_db_nodes")  # (2)
    async for item in paginator.paginate(...):
        item: ListDbNodesOutputTypeDef
        print(item)  # (3)
```

1. client: [OdbClient](./client.md)
2. paginator: [ListDbNodesPaginator](./paginators.md#listdbnodespaginator)
3. item: `AioPageIterator[ListDbNodesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDbNodesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    cloudVmClusterId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDbNodesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDbNodesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDbNodesInputPaginateTypeDef = {  # (1)
    "cloudVmClusterId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDbNodesInputPaginateTypeDef](./type_defs.md#listdbnodesinputpaginatetypedef)
## ListDbServersPaginator

Type annotations and code completion for `#!python session.create_client("odb").get_paginator("list_db_servers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/paginator/ListDbServers.html#Odb.Paginator.ListDbServers)

```python
# ListDbServersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_odb.paginator import ListDbServersPaginator

session = get_session()
async with session.create_client("odb") as client:  # (1)
    paginator: ListDbServersPaginator = client.get_paginator("list_db_servers")  # (2)
    async for item in paginator.paginate(...):
        item: ListDbServersOutputTypeDef
        print(item)  # (3)
```

1. client: [OdbClient](./client.md)
2. paginator: [ListDbServersPaginator](./paginators.md#listdbserverspaginator)
3. item: `AioPageIterator[ListDbServersOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDbServersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    cloudExadataInfrastructureId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDbServersOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDbServersOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDbServersInputPaginateTypeDef = {  # (1)
    "cloudExadataInfrastructureId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDbServersInputPaginateTypeDef](./type_defs.md#listdbserversinputpaginatetypedef)
## ListDbSystemShapesPaginator

Type annotations and code completion for `#!python session.create_client("odb").get_paginator("list_db_system_shapes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/paginator/ListDbSystemShapes.html#Odb.Paginator.ListDbSystemShapes)

```python
# ListDbSystemShapesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_odb.paginator import ListDbSystemShapesPaginator

session = get_session()
async with session.create_client("odb") as client:  # (1)
    paginator: ListDbSystemShapesPaginator = client.get_paginator("list_db_system_shapes")  # (2)
    async for item in paginator.paginate(...):
        item: ListDbSystemShapesOutputTypeDef
        print(item)  # (3)
```

1. client: [OdbClient](./client.md)
2. paginator: [ListDbSystemShapesPaginator](./paginators.md#listdbsystemshapespaginator)
3. item: `AioPageIterator[ListDbSystemShapesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDbSystemShapesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    availabilityZone: str = ...,
    availabilityZoneId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDbSystemShapesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDbSystemShapesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDbSystemShapesInputPaginateTypeDef = {  # (1)
    "availabilityZone": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDbSystemShapesInputPaginateTypeDef](./type_defs.md#listdbsystemshapesinputpaginatetypedef)
## ListGiVersionsPaginator

Type annotations and code completion for `#!python session.create_client("odb").get_paginator("list_gi_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/paginator/ListGiVersions.html#Odb.Paginator.ListGiVersions)

```python
# ListGiVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_odb.paginator import ListGiVersionsPaginator

session = get_session()
async with session.create_client("odb") as client:  # (1)
    paginator: ListGiVersionsPaginator = client.get_paginator("list_gi_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListGiVersionsOutputTypeDef
        print(item)  # (3)
```

1. client: [OdbClient](./client.md)
2. paginator: [ListGiVersionsPaginator](./paginators.md#listgiversionspaginator)
3. item: `AioPageIterator[ListGiVersionsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListGiVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    shape: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListGiVersionsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListGiVersionsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListGiVersionsInputPaginateTypeDef = {  # (1)
    "shape": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGiVersionsInputPaginateTypeDef](./type_defs.md#listgiversionsinputpaginatetypedef)
## ListOdbNetworksPaginator

Type annotations and code completion for `#!python session.create_client("odb").get_paginator("list_odb_networks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/paginator/ListOdbNetworks.html#Odb.Paginator.ListOdbNetworks)

```python
# ListOdbNetworksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_odb.paginator import ListOdbNetworksPaginator

session = get_session()
async with session.create_client("odb") as client:  # (1)
    paginator: ListOdbNetworksPaginator = client.get_paginator("list_odb_networks")  # (2)
    async for item in paginator.paginate(...):
        item: ListOdbNetworksOutputTypeDef
        print(item)  # (3)
```

1. client: [OdbClient](./client.md)
2. paginator: [ListOdbNetworksPaginator](./paginators.md#listodbnetworkspaginator)
3. item: `AioPageIterator[ListOdbNetworksOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListOdbNetworksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListOdbNetworksOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListOdbNetworksOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListOdbNetworksInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOdbNetworksInputPaginateTypeDef](./type_defs.md#listodbnetworksinputpaginatetypedef)
## ListOdbPeeringConnectionsPaginator

Type annotations and code completion for `#!python session.create_client("odb").get_paginator("list_odb_peering_connections")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/paginator/ListOdbPeeringConnections.html#Odb.Paginator.ListOdbPeeringConnections)

```python
# ListOdbPeeringConnectionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_odb.paginator import ListOdbPeeringConnectionsPaginator

session = get_session()
async with session.create_client("odb") as client:  # (1)
    paginator: ListOdbPeeringConnectionsPaginator = client.get_paginator("list_odb_peering_connections")  # (2)
    async for item in paginator.paginate(...):
        item: ListOdbPeeringConnectionsOutputTypeDef
        print(item)  # (3)
```

1. client: [OdbClient](./client.md)
2. paginator: [ListOdbPeeringConnectionsPaginator](./paginators.md#listodbpeeringconnectionspaginator)
3. item: `AioPageIterator[ListOdbPeeringConnectionsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListOdbPeeringConnectionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    odbNetworkId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListOdbPeeringConnectionsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListOdbPeeringConnectionsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListOdbPeeringConnectionsInputPaginateTypeDef = {  # (1)
    "odbNetworkId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOdbPeeringConnectionsInputPaginateTypeDef](./type_defs.md#listodbpeeringconnectionsinputpaginatetypedef)
## ListSystemVersionsPaginator

Type annotations and code completion for `#!python session.create_client("odb").get_paginator("list_system_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb/paginator/ListSystemVersions.html#Odb.Paginator.ListSystemVersions)

```python
# ListSystemVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_odb.paginator import ListSystemVersionsPaginator

session = get_session()
async with session.create_client("odb") as client:  # (1)
    paginator: ListSystemVersionsPaginator = client.get_paginator("list_system_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListSystemVersionsOutputTypeDef
        print(item)  # (3)
```

1. client: [OdbClient](./client.md)
2. paginator: [ListSystemVersionsPaginator](./paginators.md#listsystemversionspaginator)
3. item: `AioPageIterator[ListSystemVersionsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSystemVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    giVersion: str,
    shape: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListSystemVersionsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListSystemVersionsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSystemVersionsInputPaginateTypeDef = {  # (1)
    "giVersion": ...,
    "shape": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSystemVersionsInputPaginateTypeDef](./type_defs.md#listsystemversionsinputpaginatetypedef)
