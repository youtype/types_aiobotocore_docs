<a id="paginators-for-aiobotocore-apigateway-module"></a>

# Paginators for aiobotocore APIGateway module

> [Index](..) > [APIGateway](.) > Paginators

Auto-generated documentation for
[APIGateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway)
type annotations stubs module
[types-aiobotocore-apigateway](https://pypi.org/project/types-aiobotocore-apigateway/).

- [Paginators for aiobotocore APIGateway module](#paginators-for-aiobotocore-apigateway-module)
  - [GetApiKeysPaginator](#getapikeyspaginator)
  - [GetAuthorizersPaginator](#getauthorizerspaginator)
  - [GetBasePathMappingsPaginator](#getbasepathmappingspaginator)
  - [GetClientCertificatesPaginator](#getclientcertificatespaginator)
  - [GetDeploymentsPaginator](#getdeploymentspaginator)
  - [GetDocumentationPartsPaginator](#getdocumentationpartspaginator)
  - [GetDocumentationVersionsPaginator](#getdocumentationversionspaginator)
  - [GetDomainNamesPaginator](#getdomainnamespaginator)
  - [GetGatewayResponsesPaginator](#getgatewayresponsespaginator)
  - [GetModelsPaginator](#getmodelspaginator)
  - [GetRequestValidatorsPaginator](#getrequestvalidatorspaginator)
  - [GetResourcesPaginator](#getresourcespaginator)
  - [GetRestApisPaginator](#getrestapispaginator)
  - [GetSdkTypesPaginator](#getsdktypespaginator)
  - [GetUsagePaginator](#getusagepaginator)
  - [GetUsagePlanKeysPaginator](#getusageplankeyspaginator)
  - [GetUsagePlansPaginator](#getusageplanspaginator)
  - [GetVpcLinksPaginator](#getvpclinkspaginator)

<a id="getapikeyspaginator"></a>

## GetApiKeysPaginator

Type annotations for
`session.create_client("apigateway").get_paginator("get_api_keys")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetApiKeysPaginator

session = get_session()
async with session.create_client("apigateway") as client:
    client: APIGatewayClient
    paginator: GetApiKeysPaginator = client.get_paginator("get_api_keys")
```

Boto3 documentation:
[APIGateway.Paginator.GetApiKeys](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetApiKeys)

Arguments for `GetApiKeysPaginator.paginate` method:

- `nameQuery`: `str`
- `customerId`: `str`
- `includeValues`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetApiKeysPaginator.paginate` returns
`_PageIterator`\[[ApiKeysTypeDef](./type_defs.md#apikeystypedef)\].

<a id="getauthorizerspaginator"></a>

## GetAuthorizersPaginator

Type annotations for
`session.create_client("apigateway").get_paginator("get_authorizers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetAuthorizersPaginator

session = get_session()
async with session.create_client("apigateway") as client:
    client: APIGatewayClient
    paginator: GetAuthorizersPaginator = client.get_paginator("get_authorizers")
```

Boto3 documentation:
[APIGateway.Paginator.GetAuthorizers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetAuthorizers)

Arguments for `GetAuthorizersPaginator.paginate` method:

- `restApiId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetAuthorizersPaginator.paginate` returns
`_PageIterator`\[[AuthorizersTypeDef](./type_defs.md#authorizerstypedef)\].

<a id="getbasepathmappingspaginator"></a>

## GetBasePathMappingsPaginator

Type annotations for
`session.create_client("apigateway").get_paginator("get_base_path_mappings")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetBasePathMappingsPaginator

session = get_session()
async with session.create_client("apigateway") as client:
    client: APIGatewayClient
    paginator: GetBasePathMappingsPaginator = client.get_paginator("get_base_path_mappings")
```

Boto3 documentation:
[APIGateway.Paginator.GetBasePathMappings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetBasePathMappings)

Arguments for `GetBasePathMappingsPaginator.paginate` method:

- `domainName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetBasePathMappingsPaginator.paginate` returns
`_PageIterator`\[[BasePathMappingsTypeDef](./type_defs.md#basepathmappingstypedef)\].

<a id="getclientcertificatespaginator"></a>

## GetClientCertificatesPaginator

Type annotations for
`session.create_client("apigateway").get_paginator("get_client_certificates")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetClientCertificatesPaginator

session = get_session()
async with session.create_client("apigateway") as client:
    client: APIGatewayClient
    paginator: GetClientCertificatesPaginator = client.get_paginator("get_client_certificates")
```

Boto3 documentation:
[APIGateway.Paginator.GetClientCertificates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetClientCertificates)

Arguments for `GetClientCertificatesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetClientCertificatesPaginator.paginate` returns
`_PageIterator`\[[ClientCertificatesTypeDef](./type_defs.md#clientcertificatestypedef)\].

<a id="getdeploymentspaginator"></a>

## GetDeploymentsPaginator

Type annotations for
`session.create_client("apigateway").get_paginator("get_deployments")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetDeploymentsPaginator

session = get_session()
async with session.create_client("apigateway") as client:
    client: APIGatewayClient
    paginator: GetDeploymentsPaginator = client.get_paginator("get_deployments")
```

Boto3 documentation:
[APIGateway.Paginator.GetDeployments](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetDeployments)

Arguments for `GetDeploymentsPaginator.paginate` method:

- `restApiId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetDeploymentsPaginator.paginate` returns
`_PageIterator`\[[DeploymentsTypeDef](./type_defs.md#deploymentstypedef)\].

<a id="getdocumentationpartspaginator"></a>

## GetDocumentationPartsPaginator

Type annotations for
`session.create_client("apigateway").get_paginator("get_documentation_parts")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetDocumentationPartsPaginator

session = get_session()
async with session.create_client("apigateway") as client:
    client: APIGatewayClient
    paginator: GetDocumentationPartsPaginator = client.get_paginator("get_documentation_parts")
```

Boto3 documentation:
[APIGateway.Paginator.GetDocumentationParts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetDocumentationParts)

Arguments for `GetDocumentationPartsPaginator.paginate` method:

- `restApiId`: `str` *(required)*
- `type`: [DocumentationPartTypeType](./literals.md#documentationparttypetype)
- `nameQuery`: `str`
- `path`: `str`
- `locationStatus`:
  [LocationStatusTypeType](./literals.md#locationstatustypetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetDocumentationPartsPaginator.paginate` returns
`_PageIterator`\[[DocumentationPartsTypeDef](./type_defs.md#documentationpartstypedef)\].

<a id="getdocumentationversionspaginator"></a>

## GetDocumentationVersionsPaginator

Type annotations for
`session.create_client("apigateway").get_paginator("get_documentation_versions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetDocumentationVersionsPaginator

session = get_session()
async with session.create_client("apigateway") as client:
    client: APIGatewayClient
    paginator: GetDocumentationVersionsPaginator = client.get_paginator("get_documentation_versions")
```

Boto3 documentation:
[APIGateway.Paginator.GetDocumentationVersions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetDocumentationVersions)

Arguments for `GetDocumentationVersionsPaginator.paginate` method:

- `restApiId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetDocumentationVersionsPaginator.paginate` returns
`_PageIterator`\[[DocumentationVersionsTypeDef](./type_defs.md#documentationversionstypedef)\].

<a id="getdomainnamespaginator"></a>

## GetDomainNamesPaginator

Type annotations for
`session.create_client("apigateway").get_paginator("get_domain_names")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetDomainNamesPaginator

session = get_session()
async with session.create_client("apigateway") as client:
    client: APIGatewayClient
    paginator: GetDomainNamesPaginator = client.get_paginator("get_domain_names")
```

Boto3 documentation:
[APIGateway.Paginator.GetDomainNames](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetDomainNames)

Arguments for `GetDomainNamesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetDomainNamesPaginator.paginate` returns
`_PageIterator`\[[DomainNamesTypeDef](./type_defs.md#domainnamestypedef)\].

<a id="getgatewayresponsespaginator"></a>

## GetGatewayResponsesPaginator

Type annotations for
`session.create_client("apigateway").get_paginator("get_gateway_responses")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetGatewayResponsesPaginator

session = get_session()
async with session.create_client("apigateway") as client:
    client: APIGatewayClient
    paginator: GetGatewayResponsesPaginator = client.get_paginator("get_gateway_responses")
```

Boto3 documentation:
[APIGateway.Paginator.GetGatewayResponses](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetGatewayResponses)

Arguments for `GetGatewayResponsesPaginator.paginate` method:

- `restApiId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetGatewayResponsesPaginator.paginate` returns
`_PageIterator`\[[GatewayResponsesTypeDef](./type_defs.md#gatewayresponsestypedef)\].

<a id="getmodelspaginator"></a>

## GetModelsPaginator

Type annotations for
`session.create_client("apigateway").get_paginator("get_models")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetModelsPaginator

session = get_session()
async with session.create_client("apigateway") as client:
    client: APIGatewayClient
    paginator: GetModelsPaginator = client.get_paginator("get_models")
```

Boto3 documentation:
[APIGateway.Paginator.GetModels](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetModels)

Arguments for `GetModelsPaginator.paginate` method:

- `restApiId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetModelsPaginator.paginate` returns
`_PageIterator`\[[ModelsTypeDef](./type_defs.md#modelstypedef)\].

<a id="getrequestvalidatorspaginator"></a>

## GetRequestValidatorsPaginator

Type annotations for
`session.create_client("apigateway").get_paginator("get_request_validators")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetRequestValidatorsPaginator

session = get_session()
async with session.create_client("apigateway") as client:
    client: APIGatewayClient
    paginator: GetRequestValidatorsPaginator = client.get_paginator("get_request_validators")
```

Boto3 documentation:
[APIGateway.Paginator.GetRequestValidators](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetRequestValidators)

Arguments for `GetRequestValidatorsPaginator.paginate` method:

- `restApiId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetRequestValidatorsPaginator.paginate` returns
`_PageIterator`\[[RequestValidatorsTypeDef](./type_defs.md#requestvalidatorstypedef)\].

<a id="getresourcespaginator"></a>

## GetResourcesPaginator

Type annotations for
`session.create_client("apigateway").get_paginator("get_resources")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetResourcesPaginator

session = get_session()
async with session.create_client("apigateway") as client:
    client: APIGatewayClient
    paginator: GetResourcesPaginator = client.get_paginator("get_resources")
```

Boto3 documentation:
[APIGateway.Paginator.GetResources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetResources)

Arguments for `GetResourcesPaginator.paginate` method:

- `restApiId`: `str` *(required)*
- `embed`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetResourcesPaginator.paginate` returns
`_PageIterator`\[[ResourcesTypeDef](./type_defs.md#resourcestypedef)\].

<a id="getrestapispaginator"></a>

## GetRestApisPaginator

Type annotations for
`session.create_client("apigateway").get_paginator("get_rest_apis")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetRestApisPaginator

session = get_session()
async with session.create_client("apigateway") as client:
    client: APIGatewayClient
    paginator: GetRestApisPaginator = client.get_paginator("get_rest_apis")
```

Boto3 documentation:
[APIGateway.Paginator.GetRestApis](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetRestApis)

Arguments for `GetRestApisPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetRestApisPaginator.paginate` returns
`_PageIterator`\[[RestApisTypeDef](./type_defs.md#restapistypedef)\].

<a id="getsdktypespaginator"></a>

## GetSdkTypesPaginator

Type annotations for
`session.create_client("apigateway").get_paginator("get_sdk_types")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetSdkTypesPaginator

session = get_session()
async with session.create_client("apigateway") as client:
    client: APIGatewayClient
    paginator: GetSdkTypesPaginator = client.get_paginator("get_sdk_types")
```

Boto3 documentation:
[APIGateway.Paginator.GetSdkTypes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetSdkTypes)

Arguments for `GetSdkTypesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetSdkTypesPaginator.paginate` returns
`_PageIterator`\[[SdkTypesTypeDef](./type_defs.md#sdktypestypedef)\].

<a id="getusagepaginator"></a>

## GetUsagePaginator

Type annotations for
`session.create_client("apigateway").get_paginator("get_usage")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetUsagePaginator

session = get_session()
async with session.create_client("apigateway") as client:
    client: APIGatewayClient
    paginator: GetUsagePaginator = client.get_paginator("get_usage")
```

Boto3 documentation:
[APIGateway.Paginator.GetUsage](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetUsage)

Arguments for `GetUsagePaginator.paginate` method:

- `usagePlanId`: `str` *(required)*
- `startDate`: `str` *(required)*
- `endDate`: `str` *(required)*
- `keyId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetUsagePaginator.paginate` returns
`_PageIterator`\[[UsageTypeDef](./type_defs.md#usagetypedef)\].

<a id="getusageplankeyspaginator"></a>

## GetUsagePlanKeysPaginator

Type annotations for
`session.create_client("apigateway").get_paginator("get_usage_plan_keys")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetUsagePlanKeysPaginator

session = get_session()
async with session.create_client("apigateway") as client:
    client: APIGatewayClient
    paginator: GetUsagePlanKeysPaginator = client.get_paginator("get_usage_plan_keys")
```

Boto3 documentation:
[APIGateway.Paginator.GetUsagePlanKeys](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetUsagePlanKeys)

Arguments for `GetUsagePlanKeysPaginator.paginate` method:

- `usagePlanId`: `str` *(required)*
- `nameQuery`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetUsagePlanKeysPaginator.paginate` returns
`_PageIterator`\[[UsagePlanKeysTypeDef](./type_defs.md#usageplankeystypedef)\].

<a id="getusageplanspaginator"></a>

## GetUsagePlansPaginator

Type annotations for
`session.create_client("apigateway").get_paginator("get_usage_plans")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetUsagePlansPaginator

session = get_session()
async with session.create_client("apigateway") as client:
    client: APIGatewayClient
    paginator: GetUsagePlansPaginator = client.get_paginator("get_usage_plans")
```

Boto3 documentation:
[APIGateway.Paginator.GetUsagePlans](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetUsagePlans)

Arguments for `GetUsagePlansPaginator.paginate` method:

- `keyId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetUsagePlansPaginator.paginate` returns
`_PageIterator`\[[UsagePlansTypeDef](./type_defs.md#usageplanstypedef)\].

<a id="getvpclinkspaginator"></a>

## GetVpcLinksPaginator

Type annotations for
`session.create_client("apigateway").get_paginator("get_vpc_links")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetVpcLinksPaginator

session = get_session()
async with session.create_client("apigateway") as client:
    client: APIGatewayClient
    paginator: GetVpcLinksPaginator = client.get_paginator("get_vpc_links")
```

Boto3 documentation:
[APIGateway.Paginator.GetVpcLinks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetVpcLinks)

Arguments for `GetVpcLinksPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetVpcLinksPaginator.paginate` returns
`_PageIterator`\[[VpcLinksTypeDef](./type_defs.md#vpclinkstypedef)\].
