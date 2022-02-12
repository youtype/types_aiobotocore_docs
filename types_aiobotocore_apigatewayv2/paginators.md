<a id="paginators-for-aiobotocore-apigatewayv2-module"></a>

# Paginators for aiobotocore ApiGatewayV2 module

> [Index](..) > [ApiGatewayV2](.) > Paginators

Auto-generated documentation for
[ApiGatewayV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
type annotations stubs module
[types-aiobotocore-apigatewayv2](https://pypi.org/project/types-aiobotocore-apigatewayv2/).

- [Paginators for aiobotocore ApiGatewayV2 module](#paginators-for-aiobotocore-apigatewayv2-module)
  - [GetApisPaginator](#getapispaginator)
  - [GetAuthorizersPaginator](#getauthorizerspaginator)
  - [GetDeploymentsPaginator](#getdeploymentspaginator)
  - [GetDomainNamesPaginator](#getdomainnamespaginator)
  - [GetIntegrationResponsesPaginator](#getintegrationresponsespaginator)
  - [GetIntegrationsPaginator](#getintegrationspaginator)
  - [GetModelsPaginator](#getmodelspaginator)
  - [GetRouteResponsesPaginator](#getrouteresponsespaginator)
  - [GetRoutesPaginator](#getroutespaginator)
  - [GetStagesPaginator](#getstagespaginator)

<a id="getapispaginator"></a>

## GetApisPaginator

Type annotations for
`session.create_client("apigatewayv2").get_paginator("get_apis")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_apigatewayv2.paginator import GetApisPaginator

session = get_session()
async with session.create_client("apigatewayv2") as client:
    client: ApiGatewayV2Client
    paginator: GetApisPaginator = client.get_paginator("get_apis")
```

Boto3 documentation:
[ApiGatewayV2.Paginator.GetApis](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetApis)

Arguments for `GetApisPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetApisPaginator.paginate` returns
`AsyncIterable`\[[GetApisResponseTypeDef](./type_defs.md#getapisresponsetypedef)\].

<a id="getauthorizerspaginator"></a>

## GetAuthorizersPaginator

Type annotations for
`session.create_client("apigatewayv2").get_paginator("get_authorizers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_apigatewayv2.paginator import GetAuthorizersPaginator

session = get_session()
async with session.create_client("apigatewayv2") as client:
    client: ApiGatewayV2Client
    paginator: GetAuthorizersPaginator = client.get_paginator("get_authorizers")
```

Boto3 documentation:
[ApiGatewayV2.Paginator.GetAuthorizers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetAuthorizers)

Arguments for `GetAuthorizersPaginator.paginate` method:

- `ApiId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetAuthorizersPaginator.paginate` returns
`AsyncIterable`\[[GetAuthorizersResponseTypeDef](./type_defs.md#getauthorizersresponsetypedef)\].

<a id="getdeploymentspaginator"></a>

## GetDeploymentsPaginator

Type annotations for
`session.create_client("apigatewayv2").get_paginator("get_deployments")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_apigatewayv2.paginator import GetDeploymentsPaginator

session = get_session()
async with session.create_client("apigatewayv2") as client:
    client: ApiGatewayV2Client
    paginator: GetDeploymentsPaginator = client.get_paginator("get_deployments")
```

Boto3 documentation:
[ApiGatewayV2.Paginator.GetDeployments](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetDeployments)

Arguments for `GetDeploymentsPaginator.paginate` method:

- `ApiId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetDeploymentsPaginator.paginate` returns
`AsyncIterable`\[[GetDeploymentsResponseTypeDef](./type_defs.md#getdeploymentsresponsetypedef)\].

<a id="getdomainnamespaginator"></a>

## GetDomainNamesPaginator

Type annotations for
`session.create_client("apigatewayv2").get_paginator("get_domain_names")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_apigatewayv2.paginator import GetDomainNamesPaginator

session = get_session()
async with session.create_client("apigatewayv2") as client:
    client: ApiGatewayV2Client
    paginator: GetDomainNamesPaginator = client.get_paginator("get_domain_names")
```

Boto3 documentation:
[ApiGatewayV2.Paginator.GetDomainNames](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetDomainNames)

Arguments for `GetDomainNamesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetDomainNamesPaginator.paginate` returns
`AsyncIterable`\[[GetDomainNamesResponseTypeDef](./type_defs.md#getdomainnamesresponsetypedef)\].

<a id="getintegrationresponsespaginator"></a>

## GetIntegrationResponsesPaginator

Type annotations for
`session.create_client("apigatewayv2").get_paginator("get_integration_responses")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_apigatewayv2.paginator import GetIntegrationResponsesPaginator

session = get_session()
async with session.create_client("apigatewayv2") as client:
    client: ApiGatewayV2Client
    paginator: GetIntegrationResponsesPaginator = client.get_paginator("get_integration_responses")
```

Boto3 documentation:
[ApiGatewayV2.Paginator.GetIntegrationResponses](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetIntegrationResponses)

Arguments for `GetIntegrationResponsesPaginator.paginate` method:

- `ApiId`: `str` *(required)*
- `IntegrationId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetIntegrationResponsesPaginator.paginate` returns
`AsyncIterable`\[[GetIntegrationResponsesResponseTypeDef](./type_defs.md#getintegrationresponsesresponsetypedef)\].

<a id="getintegrationspaginator"></a>

## GetIntegrationsPaginator

Type annotations for
`session.create_client("apigatewayv2").get_paginator("get_integrations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_apigatewayv2.paginator import GetIntegrationsPaginator

session = get_session()
async with session.create_client("apigatewayv2") as client:
    client: ApiGatewayV2Client
    paginator: GetIntegrationsPaginator = client.get_paginator("get_integrations")
```

Boto3 documentation:
[ApiGatewayV2.Paginator.GetIntegrations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetIntegrations)

Arguments for `GetIntegrationsPaginator.paginate` method:

- `ApiId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetIntegrationsPaginator.paginate` returns
`AsyncIterable`\[[GetIntegrationsResponseTypeDef](./type_defs.md#getintegrationsresponsetypedef)\].

<a id="getmodelspaginator"></a>

## GetModelsPaginator

Type annotations for
`session.create_client("apigatewayv2").get_paginator("get_models")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_apigatewayv2.paginator import GetModelsPaginator

session = get_session()
async with session.create_client("apigatewayv2") as client:
    client: ApiGatewayV2Client
    paginator: GetModelsPaginator = client.get_paginator("get_models")
```

Boto3 documentation:
[ApiGatewayV2.Paginator.GetModels](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetModels)

Arguments for `GetModelsPaginator.paginate` method:

- `ApiId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetModelsPaginator.paginate` returns
`AsyncIterable`\[[GetModelsResponseTypeDef](./type_defs.md#getmodelsresponsetypedef)\].

<a id="getrouteresponsespaginator"></a>

## GetRouteResponsesPaginator

Type annotations for
`session.create_client("apigatewayv2").get_paginator("get_route_responses")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_apigatewayv2.paginator import GetRouteResponsesPaginator

session = get_session()
async with session.create_client("apigatewayv2") as client:
    client: ApiGatewayV2Client
    paginator: GetRouteResponsesPaginator = client.get_paginator("get_route_responses")
```

Boto3 documentation:
[ApiGatewayV2.Paginator.GetRouteResponses](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetRouteResponses)

Arguments for `GetRouteResponsesPaginator.paginate` method:

- `ApiId`: `str` *(required)*
- `RouteId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetRouteResponsesPaginator.paginate` returns
`AsyncIterable`\[[GetRouteResponsesResponseTypeDef](./type_defs.md#getrouteresponsesresponsetypedef)\].

<a id="getroutespaginator"></a>

## GetRoutesPaginator

Type annotations for
`session.create_client("apigatewayv2").get_paginator("get_routes")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_apigatewayv2.paginator import GetRoutesPaginator

session = get_session()
async with session.create_client("apigatewayv2") as client:
    client: ApiGatewayV2Client
    paginator: GetRoutesPaginator = client.get_paginator("get_routes")
```

Boto3 documentation:
[ApiGatewayV2.Paginator.GetRoutes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetRoutes)

Arguments for `GetRoutesPaginator.paginate` method:

- `ApiId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetRoutesPaginator.paginate` returns
`AsyncIterable`\[[GetRoutesResponseTypeDef](./type_defs.md#getroutesresponsetypedef)\].

<a id="getstagespaginator"></a>

## GetStagesPaginator

Type annotations for
`session.create_client("apigatewayv2").get_paginator("get_stages")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_apigatewayv2.paginator import GetStagesPaginator

session = get_session()
async with session.create_client("apigatewayv2") as client:
    client: ApiGatewayV2Client
    paginator: GetStagesPaginator = client.get_paginator("get_stages")
```

Boto3 documentation:
[ApiGatewayV2.Paginator.GetStages](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetStages)

Arguments for `GetStagesPaginator.paginate` method:

- `ApiId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetStagesPaginator.paginate` returns
`AsyncIterable`\[[GetStagesResponseTypeDef](./type_defs.md#getstagesresponsetypedef)\].
