# Paginators

> [Index](../README.md) > [AppMesh](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [AppMesh](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
    type annotations stubs module [types-aiobotocore-appmesh](https://pypi.org/project/types-aiobotocore-appmesh/).

## ListGatewayRoutesPaginator

Type annotations and code completion for `#!python session.create_client("appmesh").get_paginator("list_gateway_routes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListGatewayRoutes)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_appmesh.paginator import ListGatewayRoutesPaginator

session = get_session()
async with session.create_client("appmesh") as client:  # (1)
    paginator: ListGatewayRoutesPaginator = client.get_paginator("list_gateway_routes")  # (2)
    async for item in paginator.paginate(...):
        item: ListGatewayRoutesOutputTypeDef
        print(item)  # (3)
```

1. client: [AppMeshClient](./client.md)
2. paginator: [ListGatewayRoutesPaginator](./paginators.md#listgatewayroutespaginator)
3. item: [:material-code-braces: ListGatewayRoutesOutputTypeDef](./type_defs.md#listgatewayroutesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListGatewayRoutesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    meshName: str,
    virtualGatewayName: str,
    meshOwner: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListGatewayRoutesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGatewayRoutesOutputTypeDef](./type_defs.md#listgatewayroutesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef = {  # (1)
    "meshName": ...,
    "virtualGatewayName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef](./type_defs.md#listgatewayroutesinputlistgatewayroutespaginatetypedef) 
## ListMeshesPaginator

Type annotations and code completion for `#!python session.create_client("appmesh").get_paginator("list_meshes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListMeshes)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_appmesh.paginator import ListMeshesPaginator

session = get_session()
async with session.create_client("appmesh") as client:  # (1)
    paginator: ListMeshesPaginator = client.get_paginator("list_meshes")  # (2)
    async for item in paginator.paginate(...):
        item: ListMeshesOutputTypeDef
        print(item)  # (3)
```

1. client: [AppMeshClient](./client.md)
2. paginator: [ListMeshesPaginator](./paginators.md#listmeshespaginator)
3. item: [:material-code-braces: ListMeshesOutputTypeDef](./type_defs.md#listmeshesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListMeshesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListMeshesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMeshesOutputTypeDef](./type_defs.md#listmeshesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListMeshesInputListMeshesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMeshesInputListMeshesPaginateTypeDef](./type_defs.md#listmeshesinputlistmeshespaginatetypedef) 
## ListRoutesPaginator

Type annotations and code completion for `#!python session.create_client("appmesh").get_paginator("list_routes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListRoutes)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_appmesh.paginator import ListRoutesPaginator

session = get_session()
async with session.create_client("appmesh") as client:  # (1)
    paginator: ListRoutesPaginator = client.get_paginator("list_routes")  # (2)
    async for item in paginator.paginate(...):
        item: ListRoutesOutputTypeDef
        print(item)  # (3)
```

1. client: [AppMeshClient](./client.md)
2. paginator: [ListRoutesPaginator](./paginators.md#listroutespaginator)
3. item: [:material-code-braces: ListRoutesOutputTypeDef](./type_defs.md#listroutesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListRoutesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    meshName: str,
    virtualRouterName: str,
    meshOwner: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRoutesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRoutesOutputTypeDef](./type_defs.md#listroutesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListRoutesInputListRoutesPaginateTypeDef = {  # (1)
    "meshName": ...,
    "virtualRouterName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRoutesInputListRoutesPaginateTypeDef](./type_defs.md#listroutesinputlistroutespaginatetypedef) 
## ListTagsForResourcePaginator

Type annotations and code completion for `#!python session.create_client("appmesh").get_paginator("list_tags_for_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListTagsForResource)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_appmesh.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("appmesh") as client:  # (1)
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")  # (2)
    async for item in paginator.paginate(...):
        item: ListTagsForResourceOutputTypeDef
        print(item)  # (3)
```

1. client: [AppMeshClient](./client.md)
2. paginator: [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
3. item: [:material-code-braces: ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListTagsForResourcePaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    resourceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTagsForResourceOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListTagsForResourceInputListTagsForResourcePaginateTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceInputListTagsForResourcePaginateTypeDef](./type_defs.md#listtagsforresourceinputlisttagsforresourcepaginatetypedef) 
## ListVirtualGatewaysPaginator

Type annotations and code completion for `#!python session.create_client("appmesh").get_paginator("list_virtual_gateways")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualGateways)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_appmesh.paginator import ListVirtualGatewaysPaginator

session = get_session()
async with session.create_client("appmesh") as client:  # (1)
    paginator: ListVirtualGatewaysPaginator = client.get_paginator("list_virtual_gateways")  # (2)
    async for item in paginator.paginate(...):
        item: ListVirtualGatewaysOutputTypeDef
        print(item)  # (3)
```

1. client: [AppMeshClient](./client.md)
2. paginator: [ListVirtualGatewaysPaginator](./paginators.md#listvirtualgatewayspaginator)
3. item: [:material-code-braces: ListVirtualGatewaysOutputTypeDef](./type_defs.md#listvirtualgatewaysoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListVirtualGatewaysPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    meshName: str,
    meshOwner: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListVirtualGatewaysOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListVirtualGatewaysOutputTypeDef](./type_defs.md#listvirtualgatewaysoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef = {  # (1)
    "meshName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef](./type_defs.md#listvirtualgatewaysinputlistvirtualgatewayspaginatetypedef) 
## ListVirtualNodesPaginator

Type annotations and code completion for `#!python session.create_client("appmesh").get_paginator("list_virtual_nodes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualNodes)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_appmesh.paginator import ListVirtualNodesPaginator

session = get_session()
async with session.create_client("appmesh") as client:  # (1)
    paginator: ListVirtualNodesPaginator = client.get_paginator("list_virtual_nodes")  # (2)
    async for item in paginator.paginate(...):
        item: ListVirtualNodesOutputTypeDef
        print(item)  # (3)
```

1. client: [AppMeshClient](./client.md)
2. paginator: [ListVirtualNodesPaginator](./paginators.md#listvirtualnodespaginator)
3. item: [:material-code-braces: ListVirtualNodesOutputTypeDef](./type_defs.md#listvirtualnodesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListVirtualNodesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    meshName: str,
    meshOwner: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListVirtualNodesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListVirtualNodesOutputTypeDef](./type_defs.md#listvirtualnodesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListVirtualNodesInputListVirtualNodesPaginateTypeDef = {  # (1)
    "meshName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListVirtualNodesInputListVirtualNodesPaginateTypeDef](./type_defs.md#listvirtualnodesinputlistvirtualnodespaginatetypedef) 
## ListVirtualRoutersPaginator

Type annotations and code completion for `#!python session.create_client("appmesh").get_paginator("list_virtual_routers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualRouters)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_appmesh.paginator import ListVirtualRoutersPaginator

session = get_session()
async with session.create_client("appmesh") as client:  # (1)
    paginator: ListVirtualRoutersPaginator = client.get_paginator("list_virtual_routers")  # (2)
    async for item in paginator.paginate(...):
        item: ListVirtualRoutersOutputTypeDef
        print(item)  # (3)
```

1. client: [AppMeshClient](./client.md)
2. paginator: [ListVirtualRoutersPaginator](./paginators.md#listvirtualrouterspaginator)
3. item: [:material-code-braces: ListVirtualRoutersOutputTypeDef](./type_defs.md#listvirtualroutersoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListVirtualRoutersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    meshName: str,
    meshOwner: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListVirtualRoutersOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListVirtualRoutersOutputTypeDef](./type_defs.md#listvirtualroutersoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef = {  # (1)
    "meshName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef](./type_defs.md#listvirtualroutersinputlistvirtualrouterspaginatetypedef) 
## ListVirtualServicesPaginator

Type annotations and code completion for `#!python session.create_client("appmesh").get_paginator("list_virtual_services")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualServices)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_appmesh.paginator import ListVirtualServicesPaginator

session = get_session()
async with session.create_client("appmesh") as client:  # (1)
    paginator: ListVirtualServicesPaginator = client.get_paginator("list_virtual_services")  # (2)
    async for item in paginator.paginate(...):
        item: ListVirtualServicesOutputTypeDef
        print(item)  # (3)
```

1. client: [AppMeshClient](./client.md)
2. paginator: [ListVirtualServicesPaginator](./paginators.md#listvirtualservicespaginator)
3. item: [:material-code-braces: ListVirtualServicesOutputTypeDef](./type_defs.md#listvirtualservicesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListVirtualServicesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    meshName: str,
    meshOwner: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListVirtualServicesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListVirtualServicesOutputTypeDef](./type_defs.md#listvirtualservicesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListVirtualServicesInputListVirtualServicesPaginateTypeDef = {  # (1)
    "meshName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListVirtualServicesInputListVirtualServicesPaginateTypeDef](./type_defs.md#listvirtualservicesinputlistvirtualservicespaginatetypedef) 
