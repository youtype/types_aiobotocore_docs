<a id="appmeshclient-for-aiobotocore-appmesh-module"></a>

# AppMeshClient for aiobotocore AppMesh module

> [Index](..) > [AppMesh](.) > AppMeshClient

Auto-generated documentation for
[AppMesh](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
type annotations stubs module
[types-aiobotocore-appmesh](https://pypi.org/project/types-aiobotocore-appmesh/).

- [AppMeshClient for aiobotocore AppMesh module](#appmeshclient-for-aiobotocore-appmesh-module)
  - [AppMeshClient](#appmeshclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_gateway_route](#create_gateway_route)
    - [create_mesh](#create_mesh)
    - [create_route](#create_route)
    - [create_virtual_gateway](#create_virtual_gateway)
    - [create_virtual_node](#create_virtual_node)
    - [create_virtual_router](#create_virtual_router)
    - [create_virtual_service](#create_virtual_service)
    - [delete_gateway_route](#delete_gateway_route)
    - [delete_mesh](#delete_mesh)
    - [delete_route](#delete_route)
    - [delete_virtual_gateway](#delete_virtual_gateway)
    - [delete_virtual_node](#delete_virtual_node)
    - [delete_virtual_router](#delete_virtual_router)
    - [delete_virtual_service](#delete_virtual_service)
    - [describe_gateway_route](#describe_gateway_route)
    - [describe_mesh](#describe_mesh)
    - [describe_route](#describe_route)
    - [describe_virtual_gateway](#describe_virtual_gateway)
    - [describe_virtual_node](#describe_virtual_node)
    - [describe_virtual_router](#describe_virtual_router)
    - [describe_virtual_service](#describe_virtual_service)
    - [generate_presigned_url](#generate_presigned_url)
    - [list_gateway_routes](#list_gateway_routes)
    - [list_meshes](#list_meshes)
    - [list_routes](#list_routes)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [list_virtual_gateways](#list_virtual_gateways)
    - [list_virtual_nodes](#list_virtual_nodes)
    - [list_virtual_routers](#list_virtual_routers)
    - [list_virtual_services](#list_virtual_services)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_gateway_route](#update_gateway_route)
    - [update_mesh](#update_mesh)
    - [update_route](#update_route)
    - [update_virtual_gateway](#update_virtual_gateway)
    - [update_virtual_node](#update_virtual_node)
    - [update_virtual_router](#update_virtual_router)
    - [update_virtual_service](#update_virtual_service)
    - [get_paginator](#get_paginator)

<a id="appmeshclient"></a>

## AppMeshClient

Type annotations for `aiobotocore.create_client("appmesh")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_appmesh.client import AppMeshClient

def get_appmesh_client() -> AppMeshClient:
    return Session().client("appmesh")
```

Boto3 documentation:
[AppMesh.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_appmesh.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```

Exceptions:

- `Exceptions.BadRequestException`
- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.ForbiddenException`
- `Exceptions.InternalServerErrorException`
- `Exceptions.LimitExceededException`
- `Exceptions.NotFoundException`
- `Exceptions.ResourceInUseException`
- `Exceptions.ServiceUnavailableException`
- `Exceptions.TooManyRequestsException`
- `Exceptions.TooManyTagsException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

AppMeshClient exceptions.

Type annotations for `aiobotocore.create_client("appmesh").exceptions` method.

Boto3 documentation:
[AppMesh.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `aiobotocore.create_client("appmesh").can_paginate`
method.

Boto3 documentation:
[AppMesh.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="create_gateway_route"></a>

### create_gateway_route

Creates a gateway route.

Type annotations for
`aiobotocore.create_client("appmesh").create_gateway_route` method.

Boto3 documentation:
[AppMesh.Client.create_gateway_route](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_gateway_route)

Asynchronous method. Use `await create_gateway_route(...)` for a synchronous
call.

Arguments mapping described in
[CreateGatewayRouteInputRequestTypeDef](./type_defs.md#creategatewayrouteinputrequesttypedef).

Keyword-only arguments:

- `gatewayRouteName`: `str` *(required)*
- `meshName`: `str` *(required)*
- `spec`: [GatewayRouteSpecTypeDef](./type_defs.md#gatewayroutespectypedef)
  *(required)*
- `virtualGatewayName`: `str` *(required)*
- `clientToken`: `str`
- `meshOwner`: `str`
- `tags`: `Sequence`\[[TagRefTypeDef](./type_defs.md#tagreftypedef)\]

Returns a `Coroutine` for
[CreateGatewayRouteOutputTypeDef](./type_defs.md#creategatewayrouteoutputtypedef).

<a id="create_mesh"></a>

### create_mesh

Creates a service mesh.

Type annotations for `aiobotocore.create_client("appmesh").create_mesh` method.

Boto3 documentation:
[AppMesh.Client.create_mesh](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_mesh)

Asynchronous method. Use `await create_mesh(...)` for a synchronous call.

Arguments mapping described in
[CreateMeshInputRequestTypeDef](./type_defs.md#createmeshinputrequesttypedef).

Keyword-only arguments:

- `meshName`: `str` *(required)*
- `clientToken`: `str`
- `spec`: [MeshSpecTypeDef](./type_defs.md#meshspectypedef)
- `tags`: `Sequence`\[[TagRefTypeDef](./type_defs.md#tagreftypedef)\]

Returns a `Coroutine` for
[CreateMeshOutputTypeDef](./type_defs.md#createmeshoutputtypedef).

<a id="create_route"></a>

### create_route

Creates a route that is associated with a virtual router.

Type annotations for `aiobotocore.create_client("appmesh").create_route`
method.

Boto3 documentation:
[AppMesh.Client.create_route](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_route)

Asynchronous method. Use `await create_route(...)` for a synchronous call.

Arguments mapping described in
[CreateRouteInputRequestTypeDef](./type_defs.md#createrouteinputrequesttypedef).

Keyword-only arguments:

- `meshName`: `str` *(required)*
- `routeName`: `str` *(required)*
- `spec`: [RouteSpecTypeDef](./type_defs.md#routespectypedef) *(required)*
- `virtualRouterName`: `str` *(required)*
- `clientToken`: `str`
- `meshOwner`: `str`
- `tags`: `Sequence`\[[TagRefTypeDef](./type_defs.md#tagreftypedef)\]

Returns a `Coroutine` for
[CreateRouteOutputTypeDef](./type_defs.md#createrouteoutputtypedef).

<a id="create_virtual_gateway"></a>

### create_virtual_gateway

Creates a virtual gateway.

Type annotations for
`aiobotocore.create_client("appmesh").create_virtual_gateway` method.

Boto3 documentation:
[AppMesh.Client.create_virtual_gateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_gateway)

Asynchronous method. Use `await create_virtual_gateway(...)` for a synchronous
call.

Arguments mapping described in
[CreateVirtualGatewayInputRequestTypeDef](./type_defs.md#createvirtualgatewayinputrequesttypedef).

Keyword-only arguments:

- `meshName`: `str` *(required)*
- `spec`: [VirtualGatewaySpecTypeDef](./type_defs.md#virtualgatewayspectypedef)
  *(required)*
- `virtualGatewayName`: `str` *(required)*
- `clientToken`: `str`
- `meshOwner`: `str`
- `tags`: `Sequence`\[[TagRefTypeDef](./type_defs.md#tagreftypedef)\]

Returns a `Coroutine` for
[CreateVirtualGatewayOutputTypeDef](./type_defs.md#createvirtualgatewayoutputtypedef).

<a id="create_virtual_node"></a>

### create_virtual_node

Creates a virtual node within a service mesh.

Type annotations for `aiobotocore.create_client("appmesh").create_virtual_node`
method.

Boto3 documentation:
[AppMesh.Client.create_virtual_node](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_node)

Asynchronous method. Use `await create_virtual_node(...)` for a synchronous
call.

Arguments mapping described in
[CreateVirtualNodeInputRequestTypeDef](./type_defs.md#createvirtualnodeinputrequesttypedef).

Keyword-only arguments:

- `meshName`: `str` *(required)*
- `spec`: [VirtualNodeSpecTypeDef](./type_defs.md#virtualnodespectypedef)
  *(required)*
- `virtualNodeName`: `str` *(required)*
- `clientToken`: `str`
- `meshOwner`: `str`
- `tags`: `Sequence`\[[TagRefTypeDef](./type_defs.md#tagreftypedef)\]

Returns a `Coroutine` for
[CreateVirtualNodeOutputTypeDef](./type_defs.md#createvirtualnodeoutputtypedef).

<a id="create_virtual_router"></a>

### create_virtual_router

Creates a virtual router within a service mesh.

Type annotations for
`aiobotocore.create_client("appmesh").create_virtual_router` method.

Boto3 documentation:
[AppMesh.Client.create_virtual_router](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_router)

Asynchronous method. Use `await create_virtual_router(...)` for a synchronous
call.

Arguments mapping described in
[CreateVirtualRouterInputRequestTypeDef](./type_defs.md#createvirtualrouterinputrequesttypedef).

Keyword-only arguments:

- `meshName`: `str` *(required)*
- `spec`: [VirtualRouterSpecTypeDef](./type_defs.md#virtualrouterspectypedef)
  *(required)*
- `virtualRouterName`: `str` *(required)*
- `clientToken`: `str`
- `meshOwner`: `str`
- `tags`: `Sequence`\[[TagRefTypeDef](./type_defs.md#tagreftypedef)\]

Returns a `Coroutine` for
[CreateVirtualRouterOutputTypeDef](./type_defs.md#createvirtualrouteroutputtypedef).

<a id="create_virtual_service"></a>

### create_virtual_service

Creates a virtual service within a service mesh.

Type annotations for
`aiobotocore.create_client("appmesh").create_virtual_service` method.

Boto3 documentation:
[AppMesh.Client.create_virtual_service](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_service)

Asynchronous method. Use `await create_virtual_service(...)` for a synchronous
call.

Arguments mapping described in
[CreateVirtualServiceInputRequestTypeDef](./type_defs.md#createvirtualserviceinputrequesttypedef).

Keyword-only arguments:

- `meshName`: `str` *(required)*
- `spec`: [VirtualServiceSpecTypeDef](./type_defs.md#virtualservicespectypedef)
  *(required)*
- `virtualServiceName`: `str` *(required)*
- `clientToken`: `str`
- `meshOwner`: `str`
- `tags`: `Sequence`\[[TagRefTypeDef](./type_defs.md#tagreftypedef)\]

Returns a `Coroutine` for
[CreateVirtualServiceOutputTypeDef](./type_defs.md#createvirtualserviceoutputtypedef).

<a id="delete_gateway_route"></a>

### delete_gateway_route

Deletes an existing gateway route.

Type annotations for
`aiobotocore.create_client("appmesh").delete_gateway_route` method.

Boto3 documentation:
[AppMesh.Client.delete_gateway_route](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_gateway_route)

Asynchronous method. Use `await delete_gateway_route(...)` for a synchronous
call.

Arguments mapping described in
[DeleteGatewayRouteInputRequestTypeDef](./type_defs.md#deletegatewayrouteinputrequesttypedef).

Keyword-only arguments:

- `gatewayRouteName`: `str` *(required)*
- `meshName`: `str` *(required)*
- `virtualGatewayName`: `str` *(required)*
- `meshOwner`: `str`

Returns a `Coroutine` for
[DeleteGatewayRouteOutputTypeDef](./type_defs.md#deletegatewayrouteoutputtypedef).

<a id="delete_mesh"></a>

### delete_mesh

Deletes an existing service mesh.

Type annotations for `aiobotocore.create_client("appmesh").delete_mesh` method.

Boto3 documentation:
[AppMesh.Client.delete_mesh](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_mesh)

Asynchronous method. Use `await delete_mesh(...)` for a synchronous call.

Arguments mapping described in
[DeleteMeshInputRequestTypeDef](./type_defs.md#deletemeshinputrequesttypedef).

Keyword-only arguments:

- `meshName`: `str` *(required)*

Returns a `Coroutine` for
[DeleteMeshOutputTypeDef](./type_defs.md#deletemeshoutputtypedef).

<a id="delete_route"></a>

### delete_route

Deletes an existing route.

Type annotations for `aiobotocore.create_client("appmesh").delete_route`
method.

Boto3 documentation:
[AppMesh.Client.delete_route](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_route)

Asynchronous method. Use `await delete_route(...)` for a synchronous call.

Arguments mapping described in
[DeleteRouteInputRequestTypeDef](./type_defs.md#deleterouteinputrequesttypedef).

Keyword-only arguments:

- `meshName`: `str` *(required)*
- `routeName`: `str` *(required)*
- `virtualRouterName`: `str` *(required)*
- `meshOwner`: `str`

Returns a `Coroutine` for
[DeleteRouteOutputTypeDef](./type_defs.md#deleterouteoutputtypedef).

<a id="delete_virtual_gateway"></a>

### delete_virtual_gateway

Deletes an existing virtual gateway.

Type annotations for
`aiobotocore.create_client("appmesh").delete_virtual_gateway` method.

Boto3 documentation:
[AppMesh.Client.delete_virtual_gateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_virtual_gateway)

Asynchronous method. Use `await delete_virtual_gateway(...)` for a synchronous
call.

Arguments mapping described in
[DeleteVirtualGatewayInputRequestTypeDef](./type_defs.md#deletevirtualgatewayinputrequesttypedef).

Keyword-only arguments:

- `meshName`: `str` *(required)*
- `virtualGatewayName`: `str` *(required)*
- `meshOwner`: `str`

Returns a `Coroutine` for
[DeleteVirtualGatewayOutputTypeDef](./type_defs.md#deletevirtualgatewayoutputtypedef).

<a id="delete_virtual_node"></a>

### delete_virtual_node

Deletes an existing virtual node.

Type annotations for `aiobotocore.create_client("appmesh").delete_virtual_node`
method.

Boto3 documentation:
[AppMesh.Client.delete_virtual_node](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_virtual_node)

Asynchronous method. Use `await delete_virtual_node(...)` for a synchronous
call.

Arguments mapping described in
[DeleteVirtualNodeInputRequestTypeDef](./type_defs.md#deletevirtualnodeinputrequesttypedef).

Keyword-only arguments:

- `meshName`: `str` *(required)*
- `virtualNodeName`: `str` *(required)*
- `meshOwner`: `str`

Returns a `Coroutine` for
[DeleteVirtualNodeOutputTypeDef](./type_defs.md#deletevirtualnodeoutputtypedef).

<a id="delete_virtual_router"></a>

### delete_virtual_router

Deletes an existing virtual router.

Type annotations for
`aiobotocore.create_client("appmesh").delete_virtual_router` method.

Boto3 documentation:
[AppMesh.Client.delete_virtual_router](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_virtual_router)

Asynchronous method. Use `await delete_virtual_router(...)` for a synchronous
call.

Arguments mapping described in
[DeleteVirtualRouterInputRequestTypeDef](./type_defs.md#deletevirtualrouterinputrequesttypedef).

Keyword-only arguments:

- `meshName`: `str` *(required)*
- `virtualRouterName`: `str` *(required)*
- `meshOwner`: `str`

Returns a `Coroutine` for
[DeleteVirtualRouterOutputTypeDef](./type_defs.md#deletevirtualrouteroutputtypedef).

<a id="delete_virtual_service"></a>

### delete_virtual_service

Deletes an existing virtual service.

Type annotations for
`aiobotocore.create_client("appmesh").delete_virtual_service` method.

Boto3 documentation:
[AppMesh.Client.delete_virtual_service](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_virtual_service)

Asynchronous method. Use `await delete_virtual_service(...)` for a synchronous
call.

Arguments mapping described in
[DeleteVirtualServiceInputRequestTypeDef](./type_defs.md#deletevirtualserviceinputrequesttypedef).

Keyword-only arguments:

- `meshName`: `str` *(required)*
- `virtualServiceName`: `str` *(required)*
- `meshOwner`: `str`

Returns a `Coroutine` for
[DeleteVirtualServiceOutputTypeDef](./type_defs.md#deletevirtualserviceoutputtypedef).

<a id="describe_gateway_route"></a>

### describe_gateway_route

Describes an existing gateway route.

Type annotations for
`aiobotocore.create_client("appmesh").describe_gateway_route` method.

Boto3 documentation:
[AppMesh.Client.describe_gateway_route](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_gateway_route)

Asynchronous method. Use `await describe_gateway_route(...)` for a synchronous
call.

Arguments mapping described in
[DescribeGatewayRouteInputRequestTypeDef](./type_defs.md#describegatewayrouteinputrequesttypedef).

Keyword-only arguments:

- `gatewayRouteName`: `str` *(required)*
- `meshName`: `str` *(required)*
- `virtualGatewayName`: `str` *(required)*
- `meshOwner`: `str`

Returns a `Coroutine` for
[DescribeGatewayRouteOutputTypeDef](./type_defs.md#describegatewayrouteoutputtypedef).

<a id="describe_mesh"></a>

### describe_mesh

Describes an existing service mesh.

Type annotations for `aiobotocore.create_client("appmesh").describe_mesh`
method.

Boto3 documentation:
[AppMesh.Client.describe_mesh](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_mesh)

Asynchronous method. Use `await describe_mesh(...)` for a synchronous call.

Arguments mapping described in
[DescribeMeshInputRequestTypeDef](./type_defs.md#describemeshinputrequesttypedef).

Keyword-only arguments:

- `meshName`: `str` *(required)*
- `meshOwner`: `str`

Returns a `Coroutine` for
[DescribeMeshOutputTypeDef](./type_defs.md#describemeshoutputtypedef).

<a id="describe_route"></a>

### describe_route

Describes an existing route.

Type annotations for `aiobotocore.create_client("appmesh").describe_route`
method.

Boto3 documentation:
[AppMesh.Client.describe_route](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_route)

Asynchronous method. Use `await describe_route(...)` for a synchronous call.

Arguments mapping described in
[DescribeRouteInputRequestTypeDef](./type_defs.md#describerouteinputrequesttypedef).

Keyword-only arguments:

- `meshName`: `str` *(required)*
- `routeName`: `str` *(required)*
- `virtualRouterName`: `str` *(required)*
- `meshOwner`: `str`

Returns a `Coroutine` for
[DescribeRouteOutputTypeDef](./type_defs.md#describerouteoutputtypedef).

<a id="describe_virtual_gateway"></a>

### describe_virtual_gateway

Describes an existing virtual gateway.

Type annotations for
`aiobotocore.create_client("appmesh").describe_virtual_gateway` method.

Boto3 documentation:
[AppMesh.Client.describe_virtual_gateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_virtual_gateway)

Asynchronous method. Use `await describe_virtual_gateway(...)` for a
synchronous call.

Arguments mapping described in
[DescribeVirtualGatewayInputRequestTypeDef](./type_defs.md#describevirtualgatewayinputrequesttypedef).

Keyword-only arguments:

- `meshName`: `str` *(required)*
- `virtualGatewayName`: `str` *(required)*
- `meshOwner`: `str`

Returns a `Coroutine` for
[DescribeVirtualGatewayOutputTypeDef](./type_defs.md#describevirtualgatewayoutputtypedef).

<a id="describe_virtual_node"></a>

### describe_virtual_node

Describes an existing virtual node.

Type annotations for
`aiobotocore.create_client("appmesh").describe_virtual_node` method.

Boto3 documentation:
[AppMesh.Client.describe_virtual_node](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_virtual_node)

Asynchronous method. Use `await describe_virtual_node(...)` for a synchronous
call.

Arguments mapping described in
[DescribeVirtualNodeInputRequestTypeDef](./type_defs.md#describevirtualnodeinputrequesttypedef).

Keyword-only arguments:

- `meshName`: `str` *(required)*
- `virtualNodeName`: `str` *(required)*
- `meshOwner`: `str`

Returns a `Coroutine` for
[DescribeVirtualNodeOutputTypeDef](./type_defs.md#describevirtualnodeoutputtypedef).

<a id="describe_virtual_router"></a>

### describe_virtual_router

Describes an existing virtual router.

Type annotations for
`aiobotocore.create_client("appmesh").describe_virtual_router` method.

Boto3 documentation:
[AppMesh.Client.describe_virtual_router](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_virtual_router)

Asynchronous method. Use `await describe_virtual_router(...)` for a synchronous
call.

Arguments mapping described in
[DescribeVirtualRouterInputRequestTypeDef](./type_defs.md#describevirtualrouterinputrequesttypedef).

Keyword-only arguments:

- `meshName`: `str` *(required)*
- `virtualRouterName`: `str` *(required)*
- `meshOwner`: `str`

Returns a `Coroutine` for
[DescribeVirtualRouterOutputTypeDef](./type_defs.md#describevirtualrouteroutputtypedef).

<a id="describe_virtual_service"></a>

### describe_virtual_service

Describes an existing virtual service.

Type annotations for
`aiobotocore.create_client("appmesh").describe_virtual_service` method.

Boto3 documentation:
[AppMesh.Client.describe_virtual_service](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_virtual_service)

Asynchronous method. Use `await describe_virtual_service(...)` for a
synchronous call.

Arguments mapping described in
[DescribeVirtualServiceInputRequestTypeDef](./type_defs.md#describevirtualserviceinputrequesttypedef).

Keyword-only arguments:

- `meshName`: `str` *(required)*
- `virtualServiceName`: `str` *(required)*
- `meshOwner`: `str`

Returns a `Coroutine` for
[DescribeVirtualServiceOutputTypeDef](./type_defs.md#describevirtualserviceoutputtypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`aiobotocore.create_client("appmesh").generate_presigned_url` method.

Boto3 documentation:
[AppMesh.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="list_gateway_routes"></a>

### list_gateway_routes

Returns a list of existing gateway routes that are associated to a virtual
gateway.

Type annotations for `aiobotocore.create_client("appmesh").list_gateway_routes`
method.

Boto3 documentation:
[AppMesh.Client.list_gateway_routes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_gateway_routes)

Asynchronous method. Use `await list_gateway_routes(...)` for a synchronous
call.

Arguments mapping described in
[ListGatewayRoutesInputRequestTypeDef](./type_defs.md#listgatewayroutesinputrequesttypedef).

Keyword-only arguments:

- `meshName`: `str` *(required)*
- `virtualGatewayName`: `str` *(required)*
- `limit`: `int`
- `meshOwner`: `str`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListGatewayRoutesOutputTypeDef](./type_defs.md#listgatewayroutesoutputtypedef).

<a id="list_meshes"></a>

### list_meshes

Returns a list of existing service meshes.

Type annotations for `aiobotocore.create_client("appmesh").list_meshes` method.

Boto3 documentation:
[AppMesh.Client.list_meshes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_meshes)

Asynchronous method. Use `await list_meshes(...)` for a synchronous call.

Arguments mapping described in
[ListMeshesInputRequestTypeDef](./type_defs.md#listmeshesinputrequesttypedef).

Keyword-only arguments:

- `limit`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListMeshesOutputTypeDef](./type_defs.md#listmeshesoutputtypedef).

<a id="list_routes"></a>

### list_routes

Returns a list of existing routes in a service mesh.

Type annotations for `aiobotocore.create_client("appmesh").list_routes` method.

Boto3 documentation:
[AppMesh.Client.list_routes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_routes)

Asynchronous method. Use `await list_routes(...)` for a synchronous call.

Arguments mapping described in
[ListRoutesInputRequestTypeDef](./type_defs.md#listroutesinputrequesttypedef).

Keyword-only arguments:

- `meshName`: `str` *(required)*
- `virtualRouterName`: `str` *(required)*
- `limit`: `int`
- `meshOwner`: `str`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListRoutesOutputTypeDef](./type_defs.md#listroutesoutputtypedef).

<a id="list_tags_for_resource"></a>

### list_tags_for_resource

List the tags for an App Mesh resource.

Type annotations for
`aiobotocore.create_client("appmesh").list_tags_for_resource` method.

Boto3 documentation:
[AppMesh.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `limit`: `int`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef).

<a id="list_virtual_gateways"></a>

### list_virtual_gateways

Returns a list of existing virtual gateways in a service mesh.

Type annotations for
`aiobotocore.create_client("appmesh").list_virtual_gateways` method.

Boto3 documentation:
[AppMesh.Client.list_virtual_gateways](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_virtual_gateways)

Asynchronous method. Use `await list_virtual_gateways(...)` for a synchronous
call.

Arguments mapping described in
[ListVirtualGatewaysInputRequestTypeDef](./type_defs.md#listvirtualgatewaysinputrequesttypedef).

Keyword-only arguments:

- `meshName`: `str` *(required)*
- `limit`: `int`
- `meshOwner`: `str`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListVirtualGatewaysOutputTypeDef](./type_defs.md#listvirtualgatewaysoutputtypedef).

<a id="list_virtual_nodes"></a>

### list_virtual_nodes

Returns a list of existing virtual nodes.

Type annotations for `aiobotocore.create_client("appmesh").list_virtual_nodes`
method.

Boto3 documentation:
[AppMesh.Client.list_virtual_nodes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_virtual_nodes)

Asynchronous method. Use `await list_virtual_nodes(...)` for a synchronous
call.

Arguments mapping described in
[ListVirtualNodesInputRequestTypeDef](./type_defs.md#listvirtualnodesinputrequesttypedef).

Keyword-only arguments:

- `meshName`: `str` *(required)*
- `limit`: `int`
- `meshOwner`: `str`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListVirtualNodesOutputTypeDef](./type_defs.md#listvirtualnodesoutputtypedef).

<a id="list_virtual_routers"></a>

### list_virtual_routers

Returns a list of existing virtual routers in a service mesh.

Type annotations for
`aiobotocore.create_client("appmesh").list_virtual_routers` method.

Boto3 documentation:
[AppMesh.Client.list_virtual_routers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_virtual_routers)

Asynchronous method. Use `await list_virtual_routers(...)` for a synchronous
call.

Arguments mapping described in
[ListVirtualRoutersInputRequestTypeDef](./type_defs.md#listvirtualroutersinputrequesttypedef).

Keyword-only arguments:

- `meshName`: `str` *(required)*
- `limit`: `int`
- `meshOwner`: `str`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListVirtualRoutersOutputTypeDef](./type_defs.md#listvirtualroutersoutputtypedef).

<a id="list_virtual_services"></a>

### list_virtual_services

Returns a list of existing virtual services in a service mesh.

Type annotations for
`aiobotocore.create_client("appmesh").list_virtual_services` method.

Boto3 documentation:
[AppMesh.Client.list_virtual_services](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_virtual_services)

Asynchronous method. Use `await list_virtual_services(...)` for a synchronous
call.

Arguments mapping described in
[ListVirtualServicesInputRequestTypeDef](./type_defs.md#listvirtualservicesinputrequesttypedef).

Keyword-only arguments:

- `meshName`: `str` *(required)*
- `limit`: `int`
- `meshOwner`: `str`
- `nextToken`: `str`

Returns a `Coroutine` for
[ListVirtualServicesOutputTypeDef](./type_defs.md#listvirtualservicesoutputtypedef).

<a id="tag_resource"></a>

### tag_resource

Associates the specified tags to a resource with the specified `resourceArn`.

Type annotations for `aiobotocore.create_client("appmesh").tag_resource`
method.

Boto3 documentation:
[AppMesh.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tags`: `Sequence`\[[TagRefTypeDef](./type_defs.md#tagreftypedef)\]
  *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag_resource"></a>

### untag_resource

Deletes specified tags from a resource.

Type annotations for `aiobotocore.create_client("appmesh").untag_resource`
method.

Boto3 documentation:
[AppMesh.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_gateway_route"></a>

### update_gateway_route

Updates an existing gateway route that is associated to a specified virtual
gateway in a service mesh.

Type annotations for
`aiobotocore.create_client("appmesh").update_gateway_route` method.

Boto3 documentation:
[AppMesh.Client.update_gateway_route](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_gateway_route)

Asynchronous method. Use `await update_gateway_route(...)` for a synchronous
call.

Arguments mapping described in
[UpdateGatewayRouteInputRequestTypeDef](./type_defs.md#updategatewayrouteinputrequesttypedef).

Keyword-only arguments:

- `gatewayRouteName`: `str` *(required)*
- `meshName`: `str` *(required)*
- `spec`: [GatewayRouteSpecTypeDef](./type_defs.md#gatewayroutespectypedef)
  *(required)*
- `virtualGatewayName`: `str` *(required)*
- `clientToken`: `str`
- `meshOwner`: `str`

Returns a `Coroutine` for
[UpdateGatewayRouteOutputTypeDef](./type_defs.md#updategatewayrouteoutputtypedef).

<a id="update_mesh"></a>

### update_mesh

Updates an existing service mesh.

Type annotations for `aiobotocore.create_client("appmesh").update_mesh` method.

Boto3 documentation:
[AppMesh.Client.update_mesh](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_mesh)

Asynchronous method. Use `await update_mesh(...)` for a synchronous call.

Arguments mapping described in
[UpdateMeshInputRequestTypeDef](./type_defs.md#updatemeshinputrequesttypedef).

Keyword-only arguments:

- `meshName`: `str` *(required)*
- `clientToken`: `str`
- `spec`: [MeshSpecTypeDef](./type_defs.md#meshspectypedef)

Returns a `Coroutine` for
[UpdateMeshOutputTypeDef](./type_defs.md#updatemeshoutputtypedef).

<a id="update_route"></a>

### update_route

Updates an existing route for a specified service mesh and virtual router.

Type annotations for `aiobotocore.create_client("appmesh").update_route`
method.

Boto3 documentation:
[AppMesh.Client.update_route](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_route)

Asynchronous method. Use `await update_route(...)` for a synchronous call.

Arguments mapping described in
[UpdateRouteInputRequestTypeDef](./type_defs.md#updaterouteinputrequesttypedef).

Keyword-only arguments:

- `meshName`: `str` *(required)*
- `routeName`: `str` *(required)*
- `spec`: [RouteSpecTypeDef](./type_defs.md#routespectypedef) *(required)*
- `virtualRouterName`: `str` *(required)*
- `clientToken`: `str`
- `meshOwner`: `str`

Returns a `Coroutine` for
[UpdateRouteOutputTypeDef](./type_defs.md#updaterouteoutputtypedef).

<a id="update_virtual_gateway"></a>

### update_virtual_gateway

Updates an existing virtual gateway in a specified service mesh.

Type annotations for
`aiobotocore.create_client("appmesh").update_virtual_gateway` method.

Boto3 documentation:
[AppMesh.Client.update_virtual_gateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_gateway)

Asynchronous method. Use `await update_virtual_gateway(...)` for a synchronous
call.

Arguments mapping described in
[UpdateVirtualGatewayInputRequestTypeDef](./type_defs.md#updatevirtualgatewayinputrequesttypedef).

Keyword-only arguments:

- `meshName`: `str` *(required)*
- `spec`: [VirtualGatewaySpecTypeDef](./type_defs.md#virtualgatewayspectypedef)
  *(required)*
- `virtualGatewayName`: `str` *(required)*
- `clientToken`: `str`
- `meshOwner`: `str`

Returns a `Coroutine` for
[UpdateVirtualGatewayOutputTypeDef](./type_defs.md#updatevirtualgatewayoutputtypedef).

<a id="update_virtual_node"></a>

### update_virtual_node

Updates an existing virtual node in a specified service mesh.

Type annotations for `aiobotocore.create_client("appmesh").update_virtual_node`
method.

Boto3 documentation:
[AppMesh.Client.update_virtual_node](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_node)

Asynchronous method. Use `await update_virtual_node(...)` for a synchronous
call.

Arguments mapping described in
[UpdateVirtualNodeInputRequestTypeDef](./type_defs.md#updatevirtualnodeinputrequesttypedef).

Keyword-only arguments:

- `meshName`: `str` *(required)*
- `spec`: [VirtualNodeSpecTypeDef](./type_defs.md#virtualnodespectypedef)
  *(required)*
- `virtualNodeName`: `str` *(required)*
- `clientToken`: `str`
- `meshOwner`: `str`

Returns a `Coroutine` for
[UpdateVirtualNodeOutputTypeDef](./type_defs.md#updatevirtualnodeoutputtypedef).

<a id="update_virtual_router"></a>

### update_virtual_router

Updates an existing virtual router in a specified service mesh.

Type annotations for
`aiobotocore.create_client("appmesh").update_virtual_router` method.

Boto3 documentation:
[AppMesh.Client.update_virtual_router](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_router)

Asynchronous method. Use `await update_virtual_router(...)` for a synchronous
call.

Arguments mapping described in
[UpdateVirtualRouterInputRequestTypeDef](./type_defs.md#updatevirtualrouterinputrequesttypedef).

Keyword-only arguments:

- `meshName`: `str` *(required)*
- `spec`: [VirtualRouterSpecTypeDef](./type_defs.md#virtualrouterspectypedef)
  *(required)*
- `virtualRouterName`: `str` *(required)*
- `clientToken`: `str`
- `meshOwner`: `str`

Returns a `Coroutine` for
[UpdateVirtualRouterOutputTypeDef](./type_defs.md#updatevirtualrouteroutputtypedef).

<a id="update_virtual_service"></a>

### update_virtual_service

Updates an existing virtual service in a specified service mesh.

Type annotations for
`aiobotocore.create_client("appmesh").update_virtual_service` method.

Boto3 documentation:
[AppMesh.Client.update_virtual_service](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_service)

Asynchronous method. Use `await update_virtual_service(...)` for a synchronous
call.

Arguments mapping described in
[UpdateVirtualServiceInputRequestTypeDef](./type_defs.md#updatevirtualserviceinputrequesttypedef).

Keyword-only arguments:

- `meshName`: `str` *(required)*
- `spec`: [VirtualServiceSpecTypeDef](./type_defs.md#virtualservicespectypedef)
  *(required)*
- `virtualServiceName`: `str` *(required)*
- `clientToken`: `str`
- `meshOwner`: `str`

Returns a `Coroutine` for
[UpdateVirtualServiceOutputTypeDef](./type_defs.md#updatevirtualserviceoutputtypedef).

<a id="get_paginator"></a>

### get_paginator

Type annotations for `aiobotocore.create_client("appmesh").get_paginator`
method with overloads.

- `client.get_paginator("list_gateway_routes")` ->
  [ListGatewayRoutesPaginator](./paginators.md#listgatewayroutespaginator)
- `client.get_paginator("list_meshes")` ->
  [ListMeshesPaginator](./paginators.md#listmeshespaginator)
- `client.get_paginator("list_routes")` ->
  [ListRoutesPaginator](./paginators.md#listroutespaginator)
- `client.get_paginator("list_tags_for_resource")` ->
  [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
- `client.get_paginator("list_virtual_gateways")` ->
  [ListVirtualGatewaysPaginator](./paginators.md#listvirtualgatewayspaginator)
- `client.get_paginator("list_virtual_nodes")` ->
  [ListVirtualNodesPaginator](./paginators.md#listvirtualnodespaginator)
- `client.get_paginator("list_virtual_routers")` ->
  [ListVirtualRoutersPaginator](./paginators.md#listvirtualrouterspaginator)
- `client.get_paginator("list_virtual_services")` ->
  [ListVirtualServicesPaginator](./paginators.md#listvirtualservicespaginator)
