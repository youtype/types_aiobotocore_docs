# Paginators

> [Index](../README.md) > [ApiGatewayV2](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ApiGatewayV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#apigatewayv2)
    type annotations stubs module [types-aiobotocore-apigatewayv2](https://pypi.org/project/types-aiobotocore-apigatewayv2/).

## GetApisPaginator

Type annotations and code completion for `#!python session.create_client("apigatewayv2").get_paginator("get_apis")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2/paginator/GetApis.html#ApiGatewayV2.Paginator.GetApis)

```python
# GetApisPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigatewayv2.paginator import GetApisPaginator

session = get_session()
async with session.create_client("apigatewayv2") as client:  # (1)
    paginator: GetApisPaginator = client.get_paginator("get_apis")  # (2)
    async for item in paginator.paginate(...):
        item: GetApisResponseTypeDef
        print(item)  # (3)
```

1. client: [ApiGatewayV2Client](./client.md)
2. paginator: [GetApisPaginator](./paginators.md#getapispaginator)
3. item: `AioPageIterator[GetApisResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetApisPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetApisResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetApisResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetApisRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetApisRequestPaginateTypeDef](./type_defs.md#getapisrequestpaginatetypedef)
## GetAuthorizersPaginator

Type annotations and code completion for `#!python session.create_client("apigatewayv2").get_paginator("get_authorizers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2/paginator/GetAuthorizers.html#ApiGatewayV2.Paginator.GetAuthorizers)

```python
# GetAuthorizersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigatewayv2.paginator import GetAuthorizersPaginator

session = get_session()
async with session.create_client("apigatewayv2") as client:  # (1)
    paginator: GetAuthorizersPaginator = client.get_paginator("get_authorizers")  # (2)
    async for item in paginator.paginate(...):
        item: GetAuthorizersResponseTypeDef
        print(item)  # (3)
```

1. client: [ApiGatewayV2Client](./client.md)
2. paginator: [GetAuthorizersPaginator](./paginators.md#getauthorizerspaginator)
3. item: `AioPageIterator[GetAuthorizersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetAuthorizersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ApiId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetAuthorizersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetAuthorizersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetAuthorizersRequestPaginateTypeDef = {  # (1)
    "ApiId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetAuthorizersRequestPaginateTypeDef](./type_defs.md#getauthorizersrequestpaginatetypedef)
## GetDeploymentsPaginator

Type annotations and code completion for `#!python session.create_client("apigatewayv2").get_paginator("get_deployments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2/paginator/GetDeployments.html#ApiGatewayV2.Paginator.GetDeployments)

```python
# GetDeploymentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigatewayv2.paginator import GetDeploymentsPaginator

session = get_session()
async with session.create_client("apigatewayv2") as client:  # (1)
    paginator: GetDeploymentsPaginator = client.get_paginator("get_deployments")  # (2)
    async for item in paginator.paginate(...):
        item: GetDeploymentsResponseTypeDef
        print(item)  # (3)
```

1. client: [ApiGatewayV2Client](./client.md)
2. paginator: [GetDeploymentsPaginator](./paginators.md#getdeploymentspaginator)
3. item: `AioPageIterator[GetDeploymentsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetDeploymentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ApiId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetDeploymentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetDeploymentsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetDeploymentsRequestPaginateTypeDef = {  # (1)
    "ApiId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetDeploymentsRequestPaginateTypeDef](./type_defs.md#getdeploymentsrequestpaginatetypedef)
## GetDomainNamesPaginator

Type annotations and code completion for `#!python session.create_client("apigatewayv2").get_paginator("get_domain_names")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2/paginator/GetDomainNames.html#ApiGatewayV2.Paginator.GetDomainNames)

```python
# GetDomainNamesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigatewayv2.paginator import GetDomainNamesPaginator

session = get_session()
async with session.create_client("apigatewayv2") as client:  # (1)
    paginator: GetDomainNamesPaginator = client.get_paginator("get_domain_names")  # (2)
    async for item in paginator.paginate(...):
        item: GetDomainNamesResponseTypeDef
        print(item)  # (3)
```

1. client: [ApiGatewayV2Client](./client.md)
2. paginator: [GetDomainNamesPaginator](./paginators.md#getdomainnamespaginator)
3. item: `AioPageIterator[GetDomainNamesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetDomainNamesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetDomainNamesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetDomainNamesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetDomainNamesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetDomainNamesRequestPaginateTypeDef](./type_defs.md#getdomainnamesrequestpaginatetypedef)
## GetIntegrationResponsesPaginator

Type annotations and code completion for `#!python session.create_client("apigatewayv2").get_paginator("get_integration_responses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2/paginator/GetIntegrationResponses.html#ApiGatewayV2.Paginator.GetIntegrationResponses)

```python
# GetIntegrationResponsesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigatewayv2.paginator import GetIntegrationResponsesPaginator

session = get_session()
async with session.create_client("apigatewayv2") as client:  # (1)
    paginator: GetIntegrationResponsesPaginator = client.get_paginator("get_integration_responses")  # (2)
    async for item in paginator.paginate(...):
        item: GetIntegrationResponsesResponseTypeDef
        print(item)  # (3)
```

1. client: [ApiGatewayV2Client](./client.md)
2. paginator: [GetIntegrationResponsesPaginator](./paginators.md#getintegrationresponsespaginator)
3. item: `AioPageIterator[GetIntegrationResponsesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetIntegrationResponsesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ApiId: str,
    IntegrationId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetIntegrationResponsesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetIntegrationResponsesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetIntegrationResponsesRequestPaginateTypeDef = {  # (1)
    "ApiId": ...,
    "IntegrationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetIntegrationResponsesRequestPaginateTypeDef](./type_defs.md#getintegrationresponsesrequestpaginatetypedef)
## GetIntegrationsPaginator

Type annotations and code completion for `#!python session.create_client("apigatewayv2").get_paginator("get_integrations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2/paginator/GetIntegrations.html#ApiGatewayV2.Paginator.GetIntegrations)

```python
# GetIntegrationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigatewayv2.paginator import GetIntegrationsPaginator

session = get_session()
async with session.create_client("apigatewayv2") as client:  # (1)
    paginator: GetIntegrationsPaginator = client.get_paginator("get_integrations")  # (2)
    async for item in paginator.paginate(...):
        item: GetIntegrationsResponseTypeDef
        print(item)  # (3)
```

1. client: [ApiGatewayV2Client](./client.md)
2. paginator: [GetIntegrationsPaginator](./paginators.md#getintegrationspaginator)
3. item: `AioPageIterator[GetIntegrationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetIntegrationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ApiId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetIntegrationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetIntegrationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetIntegrationsRequestPaginateTypeDef = {  # (1)
    "ApiId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetIntegrationsRequestPaginateTypeDef](./type_defs.md#getintegrationsrequestpaginatetypedef)
## GetModelsPaginator

Type annotations and code completion for `#!python session.create_client("apigatewayv2").get_paginator("get_models")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2/paginator/GetModels.html#ApiGatewayV2.Paginator.GetModels)

```python
# GetModelsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigatewayv2.paginator import GetModelsPaginator

session = get_session()
async with session.create_client("apigatewayv2") as client:  # (1)
    paginator: GetModelsPaginator = client.get_paginator("get_models")  # (2)
    async for item in paginator.paginate(...):
        item: GetModelsResponseTypeDef
        print(item)  # (3)
```

1. client: [ApiGatewayV2Client](./client.md)
2. paginator: [GetModelsPaginator](./paginators.md#getmodelspaginator)
3. item: `AioPageIterator[GetModelsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetModelsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ApiId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetModelsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetModelsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetModelsRequestPaginateTypeDef = {  # (1)
    "ApiId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetModelsRequestPaginateTypeDef](./type_defs.md#getmodelsrequestpaginatetypedef)
## GetRouteResponsesPaginator

Type annotations and code completion for `#!python session.create_client("apigatewayv2").get_paginator("get_route_responses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2/paginator/GetRouteResponses.html#ApiGatewayV2.Paginator.GetRouteResponses)

```python
# GetRouteResponsesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigatewayv2.paginator import GetRouteResponsesPaginator

session = get_session()
async with session.create_client("apigatewayv2") as client:  # (1)
    paginator: GetRouteResponsesPaginator = client.get_paginator("get_route_responses")  # (2)
    async for item in paginator.paginate(...):
        item: GetRouteResponsesResponseTypeDef
        print(item)  # (3)
```

1. client: [ApiGatewayV2Client](./client.md)
2. paginator: [GetRouteResponsesPaginator](./paginators.md#getrouteresponsespaginator)
3. item: `AioPageIterator[GetRouteResponsesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetRouteResponsesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ApiId: str,
    RouteId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetRouteResponsesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetRouteResponsesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetRouteResponsesRequestPaginateTypeDef = {  # (1)
    "ApiId": ...,
    "RouteId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetRouteResponsesRequestPaginateTypeDef](./type_defs.md#getrouteresponsesrequestpaginatetypedef)
## GetRoutesPaginator

Type annotations and code completion for `#!python session.create_client("apigatewayv2").get_paginator("get_routes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2/paginator/GetRoutes.html#ApiGatewayV2.Paginator.GetRoutes)

```python
# GetRoutesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigatewayv2.paginator import GetRoutesPaginator

session = get_session()
async with session.create_client("apigatewayv2") as client:  # (1)
    paginator: GetRoutesPaginator = client.get_paginator("get_routes")  # (2)
    async for item in paginator.paginate(...):
        item: GetRoutesResponseTypeDef
        print(item)  # (3)
```

1. client: [ApiGatewayV2Client](./client.md)
2. paginator: [GetRoutesPaginator](./paginators.md#getroutespaginator)
3. item: `AioPageIterator[GetRoutesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetRoutesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ApiId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetRoutesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetRoutesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetRoutesRequestPaginateTypeDef = {  # (1)
    "ApiId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetRoutesRequestPaginateTypeDef](./type_defs.md#getroutesrequestpaginatetypedef)
## GetStagesPaginator

Type annotations and code completion for `#!python session.create_client("apigatewayv2").get_paginator("get_stages")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2/paginator/GetStages.html#ApiGatewayV2.Paginator.GetStages)

```python
# GetStagesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigatewayv2.paginator import GetStagesPaginator

session = get_session()
async with session.create_client("apigatewayv2") as client:  # (1)
    paginator: GetStagesPaginator = client.get_paginator("get_stages")  # (2)
    async for item in paginator.paginate(...):
        item: GetStagesResponseTypeDef
        print(item)  # (3)
```

1. client: [ApiGatewayV2Client](./client.md)
2. paginator: [GetStagesPaginator](./paginators.md#getstagespaginator)
3. item: `AioPageIterator[GetStagesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetStagesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ApiId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetStagesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetStagesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetStagesRequestPaginateTypeDef = {  # (1)
    "ApiId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetStagesRequestPaginateTypeDef](./type_defs.md#getstagesrequestpaginatetypedef)
## ListPortalProductsPaginator

Type annotations and code completion for `#!python session.create_client("apigatewayv2").get_paginator("list_portal_products")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2/paginator/ListPortalProducts.html#ApiGatewayV2.Paginator.ListPortalProducts)

```python
# ListPortalProductsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigatewayv2.paginator import ListPortalProductsPaginator

session = get_session()
async with session.create_client("apigatewayv2") as client:  # (1)
    paginator: ListPortalProductsPaginator = client.get_paginator("list_portal_products")  # (2)
    async for item in paginator.paginate(...):
        item: ListPortalProductsResponseTypeDef
        print(item)  # (3)
```

1. client: [ApiGatewayV2Client](./client.md)
2. paginator: [ListPortalProductsPaginator](./paginators.md#listportalproductspaginator)
3. item: `AioPageIterator[ListPortalProductsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPortalProductsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceOwner: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListPortalProductsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListPortalProductsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPortalProductsRequestPaginateTypeDef = {  # (1)
    "ResourceOwner": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPortalProductsRequestPaginateTypeDef](./type_defs.md#listportalproductsrequestpaginatetypedef)
## ListPortalsPaginator

Type annotations and code completion for `#!python session.create_client("apigatewayv2").get_paginator("list_portals")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2/paginator/ListPortals.html#ApiGatewayV2.Paginator.ListPortals)

```python
# ListPortalsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigatewayv2.paginator import ListPortalsPaginator

session = get_session()
async with session.create_client("apigatewayv2") as client:  # (1)
    paginator: ListPortalsPaginator = client.get_paginator("list_portals")  # (2)
    async for item in paginator.paginate(...):
        item: ListPortalsResponseTypeDef
        print(item)  # (3)
```

1. client: [ApiGatewayV2Client](./client.md)
2. paginator: [ListPortalsPaginator](./paginators.md#listportalspaginator)
3. item: `AioPageIterator[ListPortalsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPortalsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListPortalsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListPortalsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPortalsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPortalsRequestPaginateTypeDef](./type_defs.md#listportalsrequestpaginatetypedef)
## ListProductPagesPaginator

Type annotations and code completion for `#!python session.create_client("apigatewayv2").get_paginator("list_product_pages")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2/paginator/ListProductPages.html#ApiGatewayV2.Paginator.ListProductPages)

```python
# ListProductPagesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigatewayv2.paginator import ListProductPagesPaginator

session = get_session()
async with session.create_client("apigatewayv2") as client:  # (1)
    paginator: ListProductPagesPaginator = client.get_paginator("list_product_pages")  # (2)
    async for item in paginator.paginate(...):
        item: ListProductPagesResponseTypeDef
        print(item)  # (3)
```

1. client: [ApiGatewayV2Client](./client.md)
2. paginator: [ListProductPagesPaginator](./paginators.md#listproductpagespaginator)
3. item: `AioPageIterator[ListProductPagesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListProductPagesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PortalProductId: str,
    ResourceOwnerAccountId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListProductPagesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListProductPagesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListProductPagesRequestPaginateTypeDef = {  # (1)
    "PortalProductId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProductPagesRequestPaginateTypeDef](./type_defs.md#listproductpagesrequestpaginatetypedef)
## ListProductRestEndpointPagesPaginator

Type annotations and code completion for `#!python session.create_client("apigatewayv2").get_paginator("list_product_rest_endpoint_pages")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2/paginator/ListProductRestEndpointPages.html#ApiGatewayV2.Paginator.ListProductRestEndpointPages)

```python
# ListProductRestEndpointPagesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigatewayv2.paginator import ListProductRestEndpointPagesPaginator

session = get_session()
async with session.create_client("apigatewayv2") as client:  # (1)
    paginator: ListProductRestEndpointPagesPaginator = client.get_paginator("list_product_rest_endpoint_pages")  # (2)
    async for item in paginator.paginate(...):
        item: ListProductRestEndpointPagesResponseTypeDef
        print(item)  # (3)
```

1. client: [ApiGatewayV2Client](./client.md)
2. paginator: [ListProductRestEndpointPagesPaginator](./paginators.md#listproductrestendpointpagespaginator)
3. item: `AioPageIterator[ListProductRestEndpointPagesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListProductRestEndpointPagesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PortalProductId: str,
    ResourceOwnerAccountId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListProductRestEndpointPagesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListProductRestEndpointPagesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListProductRestEndpointPagesRequestPaginateTypeDef = {  # (1)
    "PortalProductId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProductRestEndpointPagesRequestPaginateTypeDef](./type_defs.md#listproductrestendpointpagesrequestpaginatetypedef)
## ListRoutingRulesPaginator

Type annotations and code completion for `#!python session.create_client("apigatewayv2").get_paginator("list_routing_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2/paginator/ListRoutingRules.html#ApiGatewayV2.Paginator.ListRoutingRules)

```python
# ListRoutingRulesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigatewayv2.paginator import ListRoutingRulesPaginator

session = get_session()
async with session.create_client("apigatewayv2") as client:  # (1)
    paginator: ListRoutingRulesPaginator = client.get_paginator("list_routing_rules")  # (2)
    async for item in paginator.paginate(...):
        item: ListRoutingRulesResponseTypeDef
        print(item)  # (3)
```

1. client: [ApiGatewayV2Client](./client.md)
2. paginator: [ListRoutingRulesPaginator](./paginators.md#listroutingrulespaginator)
3. item: `AioPageIterator[ListRoutingRulesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRoutingRulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DomainName: str,
    DomainNameId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListRoutingRulesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListRoutingRulesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRoutingRulesRequestPaginateTypeDef = {  # (1)
    "DomainName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRoutingRulesRequestPaginateTypeDef](./type_defs.md#listroutingrulesrequestpaginatetypedef)
