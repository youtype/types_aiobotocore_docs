# Paginators

> [Index](../README.md) > [APIGateway](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [APIGateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#apigateway)
    type annotations stubs module [types-aiobotocore-apigateway](https://pypi.org/project/types-aiobotocore-apigateway/).

## GetApiKeysPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_api_keys")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway/paginator/GetApiKeys.html#APIGateway.Paginator.GetApiKeys)

```python
# GetApiKeysPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetApiKeysPaginator

session = get_session()
async with session.create_client("apigateway") as client:  # (1)
    paginator: GetApiKeysPaginator = client.get_paginator("get_api_keys")  # (2)
    async for item in paginator.paginate(...):
        item: ApiKeysTypeDef
        print(item)  # (3)
```

1. client: [APIGatewayClient](./client.md)
2. paginator: [GetApiKeysPaginator](./paginators.md#getapikeyspaginator)
3. item: [:material-code-braces: ApiKeysTypeDef](./type_defs.md#apikeystypedef) 


### paginate

Type annotations and code completion for `#!python GetApiKeysPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    nameQuery: str = ...,
    customerId: str = ...,
    includeValues: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ApiKeysTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ApiKeysTypeDef](./type_defs.md#apikeystypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetApiKeysRequestPaginateTypeDef = {  # (1)
    "nameQuery": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetApiKeysRequestPaginateTypeDef](./type_defs.md#getapikeysrequestpaginatetypedef) 
## GetAuthorizersPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_authorizers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway/paginator/GetAuthorizers.html#APIGateway.Paginator.GetAuthorizers)

```python
# GetAuthorizersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetAuthorizersPaginator

session = get_session()
async with session.create_client("apigateway") as client:  # (1)
    paginator: GetAuthorizersPaginator = client.get_paginator("get_authorizers")  # (2)
    async for item in paginator.paginate(...):
        item: AuthorizersTypeDef
        print(item)  # (3)
```

1. client: [APIGatewayClient](./client.md)
2. paginator: [GetAuthorizersPaginator](./paginators.md#getauthorizerspaginator)
3. item: [:material-code-braces: AuthorizersTypeDef](./type_defs.md#authorizerstypedef) 


### paginate

Type annotations and code completion for `#!python GetAuthorizersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    restApiId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[AuthorizersTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: AuthorizersTypeDef](./type_defs.md#authorizerstypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetAuthorizersRequestPaginateTypeDef = {  # (1)
    "restApiId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetAuthorizersRequestPaginateTypeDef](./type_defs.md#getauthorizersrequestpaginatetypedef) 
## GetBasePathMappingsPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_base_path_mappings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway/paginator/GetBasePathMappings.html#APIGateway.Paginator.GetBasePathMappings)

```python
# GetBasePathMappingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetBasePathMappingsPaginator

session = get_session()
async with session.create_client("apigateway") as client:  # (1)
    paginator: GetBasePathMappingsPaginator = client.get_paginator("get_base_path_mappings")  # (2)
    async for item in paginator.paginate(...):
        item: BasePathMappingsTypeDef
        print(item)  # (3)
```

1. client: [APIGatewayClient](./client.md)
2. paginator: [GetBasePathMappingsPaginator](./paginators.md#getbasepathmappingspaginator)
3. item: [:material-code-braces: BasePathMappingsTypeDef](./type_defs.md#basepathmappingstypedef) 


### paginate

Type annotations and code completion for `#!python GetBasePathMappingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    domainName: str,
    domainNameId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[BasePathMappingsTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: BasePathMappingsTypeDef](./type_defs.md#basepathmappingstypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetBasePathMappingsRequestPaginateTypeDef = {  # (1)
    "domainName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetBasePathMappingsRequestPaginateTypeDef](./type_defs.md#getbasepathmappingsrequestpaginatetypedef) 
## GetClientCertificatesPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_client_certificates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway/paginator/GetClientCertificates.html#APIGateway.Paginator.GetClientCertificates)

```python
# GetClientCertificatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetClientCertificatesPaginator

session = get_session()
async with session.create_client("apigateway") as client:  # (1)
    paginator: GetClientCertificatesPaginator = client.get_paginator("get_client_certificates")  # (2)
    async for item in paginator.paginate(...):
        item: ClientCertificatesTypeDef
        print(item)  # (3)
```

1. client: [APIGatewayClient](./client.md)
2. paginator: [GetClientCertificatesPaginator](./paginators.md#getclientcertificatespaginator)
3. item: [:material-code-braces: ClientCertificatesTypeDef](./type_defs.md#clientcertificatestypedef) 


### paginate

Type annotations and code completion for `#!python GetClientCertificatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ClientCertificatesTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ClientCertificatesTypeDef](./type_defs.md#clientcertificatestypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetClientCertificatesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetClientCertificatesRequestPaginateTypeDef](./type_defs.md#getclientcertificatesrequestpaginatetypedef) 
## GetDeploymentsPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_deployments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway/paginator/GetDeployments.html#APIGateway.Paginator.GetDeployments)

```python
# GetDeploymentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetDeploymentsPaginator

session = get_session()
async with session.create_client("apigateway") as client:  # (1)
    paginator: GetDeploymentsPaginator = client.get_paginator("get_deployments")  # (2)
    async for item in paginator.paginate(...):
        item: DeploymentsTypeDef
        print(item)  # (3)
```

1. client: [APIGatewayClient](./client.md)
2. paginator: [GetDeploymentsPaginator](./paginators.md#getdeploymentspaginator)
3. item: [:material-code-braces: DeploymentsTypeDef](./type_defs.md#deploymentstypedef) 


### paginate

Type annotations and code completion for `#!python GetDeploymentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    restApiId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DeploymentsTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DeploymentsTypeDef](./type_defs.md#deploymentstypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetDeploymentsRequestPaginateTypeDef = {  # (1)
    "restApiId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetDeploymentsRequestPaginateTypeDef](./type_defs.md#getdeploymentsrequestpaginatetypedef) 
## GetDocumentationPartsPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_documentation_parts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway/paginator/GetDocumentationParts.html#APIGateway.Paginator.GetDocumentationParts)

```python
# GetDocumentationPartsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetDocumentationPartsPaginator

session = get_session()
async with session.create_client("apigateway") as client:  # (1)
    paginator: GetDocumentationPartsPaginator = client.get_paginator("get_documentation_parts")  # (2)
    async for item in paginator.paginate(...):
        item: DocumentationPartsTypeDef
        print(item)  # (3)
```

1. client: [APIGatewayClient](./client.md)
2. paginator: [GetDocumentationPartsPaginator](./paginators.md#getdocumentationpartspaginator)
3. item: [:material-code-braces: DocumentationPartsTypeDef](./type_defs.md#documentationpartstypedef) 


### paginate

Type annotations and code completion for `#!python GetDocumentationPartsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    restApiId: str,
    type: DocumentationPartTypeType = ...,  # (1)
    nameQuery: str = ...,
    path: str = ...,
    locationStatus: LocationStatusTypeType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[DocumentationPartsTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: DocumentationPartTypeType](./literals.md#documentationparttypetype) 
2. See [:material-code-brackets: LocationStatusTypeType](./literals.md#locationstatustypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: DocumentationPartsTypeDef](./type_defs.md#documentationpartstypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetDocumentationPartsRequestPaginateTypeDef = {  # (1)
    "restApiId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetDocumentationPartsRequestPaginateTypeDef](./type_defs.md#getdocumentationpartsrequestpaginatetypedef) 
## GetDocumentationVersionsPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_documentation_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway/paginator/GetDocumentationVersions.html#APIGateway.Paginator.GetDocumentationVersions)

```python
# GetDocumentationVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetDocumentationVersionsPaginator

session = get_session()
async with session.create_client("apigateway") as client:  # (1)
    paginator: GetDocumentationVersionsPaginator = client.get_paginator("get_documentation_versions")  # (2)
    async for item in paginator.paginate(...):
        item: DocumentationVersionsTypeDef
        print(item)  # (3)
```

1. client: [APIGatewayClient](./client.md)
2. paginator: [GetDocumentationVersionsPaginator](./paginators.md#getdocumentationversionspaginator)
3. item: [:material-code-braces: DocumentationVersionsTypeDef](./type_defs.md#documentationversionstypedef) 


### paginate

Type annotations and code completion for `#!python GetDocumentationVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    restApiId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DocumentationVersionsTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DocumentationVersionsTypeDef](./type_defs.md#documentationversionstypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetDocumentationVersionsRequestPaginateTypeDef = {  # (1)
    "restApiId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetDocumentationVersionsRequestPaginateTypeDef](./type_defs.md#getdocumentationversionsrequestpaginatetypedef) 
## GetDomainNamesPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_domain_names")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway/paginator/GetDomainNames.html#APIGateway.Paginator.GetDomainNames)

```python
# GetDomainNamesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetDomainNamesPaginator

session = get_session()
async with session.create_client("apigateway") as client:  # (1)
    paginator: GetDomainNamesPaginator = client.get_paginator("get_domain_names")  # (2)
    async for item in paginator.paginate(...):
        item: DomainNamesTypeDef
        print(item)  # (3)
```

1. client: [APIGatewayClient](./client.md)
2. paginator: [GetDomainNamesPaginator](./paginators.md#getdomainnamespaginator)
3. item: [:material-code-braces: DomainNamesTypeDef](./type_defs.md#domainnamestypedef) 


### paginate

Type annotations and code completion for `#!python GetDomainNamesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    resourceOwner: ResourceOwnerType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DomainNamesTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ResourceOwnerType](./literals.md#resourceownertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DomainNamesTypeDef](./type_defs.md#domainnamestypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetDomainNamesRequestPaginateTypeDef = {  # (1)
    "resourceOwner": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetDomainNamesRequestPaginateTypeDef](./type_defs.md#getdomainnamesrequestpaginatetypedef) 
## GetGatewayResponsesPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_gateway_responses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway/paginator/GetGatewayResponses.html#APIGateway.Paginator.GetGatewayResponses)

```python
# GetGatewayResponsesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetGatewayResponsesPaginator

session = get_session()
async with session.create_client("apigateway") as client:  # (1)
    paginator: GetGatewayResponsesPaginator = client.get_paginator("get_gateway_responses")  # (2)
    async for item in paginator.paginate(...):
        item: GatewayResponsesTypeDef
        print(item)  # (3)
```

1. client: [APIGatewayClient](./client.md)
2. paginator: [GetGatewayResponsesPaginator](./paginators.md#getgatewayresponsespaginator)
3. item: [:material-code-braces: GatewayResponsesTypeDef](./type_defs.md#gatewayresponsestypedef) 


### paginate

Type annotations and code completion for `#!python GetGatewayResponsesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    restApiId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GatewayResponsesTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GatewayResponsesTypeDef](./type_defs.md#gatewayresponsestypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetGatewayResponsesRequestPaginateTypeDef = {  # (1)
    "restApiId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetGatewayResponsesRequestPaginateTypeDef](./type_defs.md#getgatewayresponsesrequestpaginatetypedef) 
## GetModelsPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_models")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway/paginator/GetModels.html#APIGateway.Paginator.GetModels)

```python
# GetModelsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetModelsPaginator

session = get_session()
async with session.create_client("apigateway") as client:  # (1)
    paginator: GetModelsPaginator = client.get_paginator("get_models")  # (2)
    async for item in paginator.paginate(...):
        item: ModelsTypeDef
        print(item)  # (3)
```

1. client: [APIGatewayClient](./client.md)
2. paginator: [GetModelsPaginator](./paginators.md#getmodelspaginator)
3. item: [:material-code-braces: ModelsTypeDef](./type_defs.md#modelstypedef) 


### paginate

Type annotations and code completion for `#!python GetModelsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    restApiId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ModelsTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ModelsTypeDef](./type_defs.md#modelstypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetModelsRequestPaginateTypeDef = {  # (1)
    "restApiId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetModelsRequestPaginateTypeDef](./type_defs.md#getmodelsrequestpaginatetypedef) 
## GetRequestValidatorsPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_request_validators")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway/paginator/GetRequestValidators.html#APIGateway.Paginator.GetRequestValidators)

```python
# GetRequestValidatorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetRequestValidatorsPaginator

session = get_session()
async with session.create_client("apigateway") as client:  # (1)
    paginator: GetRequestValidatorsPaginator = client.get_paginator("get_request_validators")  # (2)
    async for item in paginator.paginate(...):
        item: RequestValidatorsTypeDef
        print(item)  # (3)
```

1. client: [APIGatewayClient](./client.md)
2. paginator: [GetRequestValidatorsPaginator](./paginators.md#getrequestvalidatorspaginator)
3. item: [:material-code-braces: RequestValidatorsTypeDef](./type_defs.md#requestvalidatorstypedef) 


### paginate

Type annotations and code completion for `#!python GetRequestValidatorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    restApiId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[RequestValidatorsTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: RequestValidatorsTypeDef](./type_defs.md#requestvalidatorstypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetRequestValidatorsRequestPaginateTypeDef = {  # (1)
    "restApiId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetRequestValidatorsRequestPaginateTypeDef](./type_defs.md#getrequestvalidatorsrequestpaginatetypedef) 
## GetResourcesPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway/paginator/GetResources.html#APIGateway.Paginator.GetResources)

```python
# GetResourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetResourcesPaginator

session = get_session()
async with session.create_client("apigateway") as client:  # (1)
    paginator: GetResourcesPaginator = client.get_paginator("get_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ResourcesTypeDef
        print(item)  # (3)
```

1. client: [APIGatewayClient](./client.md)
2. paginator: [GetResourcesPaginator](./paginators.md#getresourcespaginator)
3. item: [:material-code-braces: ResourcesTypeDef](./type_defs.md#resourcestypedef) 


### paginate

Type annotations and code completion for `#!python GetResourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    restApiId: str,
    embed: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ResourcesTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ResourcesTypeDef](./type_defs.md#resourcestypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetResourcesRequestPaginateTypeDef = {  # (1)
    "restApiId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetResourcesRequestPaginateTypeDef](./type_defs.md#getresourcesrequestpaginatetypedef) 
## GetRestApisPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_rest_apis")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway/paginator/GetRestApis.html#APIGateway.Paginator.GetRestApis)

```python
# GetRestApisPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetRestApisPaginator

session = get_session()
async with session.create_client("apigateway") as client:  # (1)
    paginator: GetRestApisPaginator = client.get_paginator("get_rest_apis")  # (2)
    async for item in paginator.paginate(...):
        item: RestApisTypeDef
        print(item)  # (3)
```

1. client: [APIGatewayClient](./client.md)
2. paginator: [GetRestApisPaginator](./paginators.md#getrestapispaginator)
3. item: [:material-code-braces: RestApisTypeDef](./type_defs.md#restapistypedef) 


### paginate

Type annotations and code completion for `#!python GetRestApisPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[RestApisTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: RestApisTypeDef](./type_defs.md#restapistypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetRestApisRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetRestApisRequestPaginateTypeDef](./type_defs.md#getrestapisrequestpaginatetypedef) 
## GetSdkTypesPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_sdk_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway/paginator/GetSdkTypes.html#APIGateway.Paginator.GetSdkTypes)

```python
# GetSdkTypesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetSdkTypesPaginator

session = get_session()
async with session.create_client("apigateway") as client:  # (1)
    paginator: GetSdkTypesPaginator = client.get_paginator("get_sdk_types")  # (2)
    async for item in paginator.paginate(...):
        item: SdkTypesTypeDef
        print(item)  # (3)
```

1. client: [APIGatewayClient](./client.md)
2. paginator: [GetSdkTypesPaginator](./paginators.md#getsdktypespaginator)
3. item: [:material-code-braces: SdkTypesTypeDef](./type_defs.md#sdktypestypedef) 


### paginate

Type annotations and code completion for `#!python GetSdkTypesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[SdkTypesTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: SdkTypesTypeDef](./type_defs.md#sdktypestypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetSdkTypesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetSdkTypesRequestPaginateTypeDef](./type_defs.md#getsdktypesrequestpaginatetypedef) 
## GetUsagePaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_usage")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway/paginator/GetUsage.html#APIGateway.Paginator.GetUsage)

```python
# GetUsagePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetUsagePaginator

session = get_session()
async with session.create_client("apigateway") as client:  # (1)
    paginator: GetUsagePaginator = client.get_paginator("get_usage")  # (2)
    async for item in paginator.paginate(...):
        item: UsageTypeDef
        print(item)  # (3)
```

1. client: [APIGatewayClient](./client.md)
2. paginator: [GetUsagePaginator](./paginators.md#getusagepaginator)
3. item: [:material-code-braces: UsageTypeDef](./type_defs.md#usagetypedef) 


### paginate

Type annotations and code completion for `#!python GetUsagePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    usagePlanId: str,
    startDate: str,
    endDate: str,
    keyId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[UsageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: UsageTypeDef](./type_defs.md#usagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetUsageRequestPaginateTypeDef = {  # (1)
    "usagePlanId": ...,
    "startDate": ...,
    "endDate": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetUsageRequestPaginateTypeDef](./type_defs.md#getusagerequestpaginatetypedef) 
## GetUsagePlanKeysPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_usage_plan_keys")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway/paginator/GetUsagePlanKeys.html#APIGateway.Paginator.GetUsagePlanKeys)

```python
# GetUsagePlanKeysPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetUsagePlanKeysPaginator

session = get_session()
async with session.create_client("apigateway") as client:  # (1)
    paginator: GetUsagePlanKeysPaginator = client.get_paginator("get_usage_plan_keys")  # (2)
    async for item in paginator.paginate(...):
        item: UsagePlanKeysTypeDef
        print(item)  # (3)
```

1. client: [APIGatewayClient](./client.md)
2. paginator: [GetUsagePlanKeysPaginator](./paginators.md#getusageplankeyspaginator)
3. item: [:material-code-braces: UsagePlanKeysTypeDef](./type_defs.md#usageplankeystypedef) 


### paginate

Type annotations and code completion for `#!python GetUsagePlanKeysPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    usagePlanId: str,
    nameQuery: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[UsagePlanKeysTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: UsagePlanKeysTypeDef](./type_defs.md#usageplankeystypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetUsagePlanKeysRequestPaginateTypeDef = {  # (1)
    "usagePlanId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetUsagePlanKeysRequestPaginateTypeDef](./type_defs.md#getusageplankeysrequestpaginatetypedef) 
## GetUsagePlansPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_usage_plans")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway/paginator/GetUsagePlans.html#APIGateway.Paginator.GetUsagePlans)

```python
# GetUsagePlansPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetUsagePlansPaginator

session = get_session()
async with session.create_client("apigateway") as client:  # (1)
    paginator: GetUsagePlansPaginator = client.get_paginator("get_usage_plans")  # (2)
    async for item in paginator.paginate(...):
        item: UsagePlansTypeDef
        print(item)  # (3)
```

1. client: [APIGatewayClient](./client.md)
2. paginator: [GetUsagePlansPaginator](./paginators.md#getusageplanspaginator)
3. item: [:material-code-braces: UsagePlansTypeDef](./type_defs.md#usageplanstypedef) 


### paginate

Type annotations and code completion for `#!python GetUsagePlansPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    keyId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[UsagePlansTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: UsagePlansTypeDef](./type_defs.md#usageplanstypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetUsagePlansRequestPaginateTypeDef = {  # (1)
    "keyId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetUsagePlansRequestPaginateTypeDef](./type_defs.md#getusageplansrequestpaginatetypedef) 
## GetVpcLinksPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_vpc_links")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway/paginator/GetVpcLinks.html#APIGateway.Paginator.GetVpcLinks)

```python
# GetVpcLinksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigateway.paginator import GetVpcLinksPaginator

session = get_session()
async with session.create_client("apigateway") as client:  # (1)
    paginator: GetVpcLinksPaginator = client.get_paginator("get_vpc_links")  # (2)
    async for item in paginator.paginate(...):
        item: VpcLinksTypeDef
        print(item)  # (3)
```

1. client: [APIGatewayClient](./client.md)
2. paginator: [GetVpcLinksPaginator](./paginators.md#getvpclinkspaginator)
3. item: [:material-code-braces: VpcLinksTypeDef](./type_defs.md#vpclinkstypedef) 


### paginate

Type annotations and code completion for `#!python GetVpcLinksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[VpcLinksTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: VpcLinksTypeDef](./type_defs.md#vpclinkstypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetVpcLinksRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetVpcLinksRequestPaginateTypeDef](./type_defs.md#getvpclinksrequestpaginatetypedef) 
