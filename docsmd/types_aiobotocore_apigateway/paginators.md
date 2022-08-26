# Paginators

> [Index](../README.md) > [APIGateway](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [APIGateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway)
    type annotations stubs module [types-aiobotocore-apigateway](https://pypi.org/project/types-aiobotocore-apigateway/).

## GetApiKeysPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_api_keys")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetApiKeys)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    nameQuery: str = ...,
    customerId: str = ...,
    includeValues: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ApiKeysTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ApiKeysTypeDef](./type_defs.md#apikeystypedef) 


```python title="Usage example with kwargs"
kwargs: GetApiKeysRequestGetApiKeysPaginateTypeDef = {  # (1)
    "nameQuery": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetApiKeysRequestGetApiKeysPaginateTypeDef](./type_defs.md#getapikeysrequestgetapikeyspaginatetypedef) 
## GetAuthorizersPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_authorizers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetAuthorizers)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    restApiId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[AuthorizersTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: AuthorizersTypeDef](./type_defs.md#authorizerstypedef) 


```python title="Usage example with kwargs"
kwargs: GetAuthorizersRequestGetAuthorizersPaginateTypeDef = {  # (1)
    "restApiId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetAuthorizersRequestGetAuthorizersPaginateTypeDef](./type_defs.md#getauthorizersrequestgetauthorizerspaginatetypedef) 
## GetBasePathMappingsPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_base_path_mappings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetBasePathMappings)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    domainName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[BasePathMappingsTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: BasePathMappingsTypeDef](./type_defs.md#basepathmappingstypedef) 


```python title="Usage example with kwargs"
kwargs: GetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef = {  # (1)
    "domainName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef](./type_defs.md#getbasepathmappingsrequestgetbasepathmappingspaginatetypedef) 
## GetClientCertificatesPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_client_certificates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetClientCertificates)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ClientCertificatesTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ClientCertificatesTypeDef](./type_defs.md#clientcertificatestypedef) 


```python title="Usage example with kwargs"
kwargs: GetClientCertificatesRequestGetClientCertificatesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetClientCertificatesRequestGetClientCertificatesPaginateTypeDef](./type_defs.md#getclientcertificatesrequestgetclientcertificatespaginatetypedef) 
## GetDeploymentsPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_deployments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetDeployments)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    restApiId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DeploymentsTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DeploymentsTypeDef](./type_defs.md#deploymentstypedef) 


```python title="Usage example with kwargs"
kwargs: GetDeploymentsRequestGetDeploymentsPaginateTypeDef = {  # (1)
    "restApiId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetDeploymentsRequestGetDeploymentsPaginateTypeDef](./type_defs.md#getdeploymentsrequestgetdeploymentspaginatetypedef) 
## GetDocumentationPartsPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_documentation_parts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetDocumentationParts)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    restApiId: str,
    type: DocumentationPartTypeType = ...,  # (1)
    nameQuery: str = ...,
    path: str = ...,
    locationStatus: LocationStatusTypeType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[DocumentationPartsTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: DocumentationPartTypeType](./literals.md#documentationparttypetype) 
2. See [:material-code-brackets: LocationStatusTypeType](./literals.md#locationstatustypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: DocumentationPartsTypeDef](./type_defs.md#documentationpartstypedef) 


```python title="Usage example with kwargs"
kwargs: GetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef = {  # (1)
    "restApiId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef](./type_defs.md#getdocumentationpartsrequestgetdocumentationpartspaginatetypedef) 
## GetDocumentationVersionsPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_documentation_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetDocumentationVersions)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    restApiId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DocumentationVersionsTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DocumentationVersionsTypeDef](./type_defs.md#documentationversionstypedef) 


```python title="Usage example with kwargs"
kwargs: GetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef = {  # (1)
    "restApiId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef](./type_defs.md#getdocumentationversionsrequestgetdocumentationversionspaginatetypedef) 
## GetDomainNamesPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_domain_names")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetDomainNames)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DomainNamesTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DomainNamesTypeDef](./type_defs.md#domainnamestypedef) 


```python title="Usage example with kwargs"
kwargs: GetDomainNamesRequestGetDomainNamesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetDomainNamesRequestGetDomainNamesPaginateTypeDef](./type_defs.md#getdomainnamesrequestgetdomainnamespaginatetypedef) 
## GetGatewayResponsesPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_gateway_responses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetGatewayResponses)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    restApiId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GatewayResponsesTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GatewayResponsesTypeDef](./type_defs.md#gatewayresponsestypedef) 


```python title="Usage example with kwargs"
kwargs: GetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef = {  # (1)
    "restApiId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef](./type_defs.md#getgatewayresponsesrequestgetgatewayresponsespaginatetypedef) 
## GetModelsPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_models")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetModels)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    restApiId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ModelsTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ModelsTypeDef](./type_defs.md#modelstypedef) 


```python title="Usage example with kwargs"
kwargs: GetModelsRequestGetModelsPaginateTypeDef = {  # (1)
    "restApiId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetModelsRequestGetModelsPaginateTypeDef](./type_defs.md#getmodelsrequestgetmodelspaginatetypedef) 
## GetRequestValidatorsPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_request_validators")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetRequestValidators)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    restApiId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[RequestValidatorsTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: RequestValidatorsTypeDef](./type_defs.md#requestvalidatorstypedef) 


```python title="Usage example with kwargs"
kwargs: GetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef = {  # (1)
    "restApiId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef](./type_defs.md#getrequestvalidatorsrequestgetrequestvalidatorspaginatetypedef) 
## GetResourcesPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetResources)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    restApiId: str,
    embed: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ResourcesTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ResourcesTypeDef](./type_defs.md#resourcestypedef) 


```python title="Usage example with kwargs"
kwargs: GetResourcesRequestGetResourcesPaginateTypeDef = {  # (1)
    "restApiId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetResourcesRequestGetResourcesPaginateTypeDef](./type_defs.md#getresourcesrequestgetresourcespaginatetypedef) 
## GetRestApisPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_rest_apis")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetRestApis)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[RestApisTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: RestApisTypeDef](./type_defs.md#restapistypedef) 


```python title="Usage example with kwargs"
kwargs: GetRestApisRequestGetRestApisPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetRestApisRequestGetRestApisPaginateTypeDef](./type_defs.md#getrestapisrequestgetrestapispaginatetypedef) 
## GetSdkTypesPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_sdk_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetSdkTypes)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[SdkTypesTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: SdkTypesTypeDef](./type_defs.md#sdktypestypedef) 


```python title="Usage example with kwargs"
kwargs: GetSdkTypesRequestGetSdkTypesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetSdkTypesRequestGetSdkTypesPaginateTypeDef](./type_defs.md#getsdktypesrequestgetsdktypespaginatetypedef) 
## GetUsagePaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_usage")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetUsage)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    usagePlanId: str,
    startDate: str,
    endDate: str,
    keyId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[UsageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: UsageTypeDef](./type_defs.md#usagetypedef) 


```python title="Usage example with kwargs"
kwargs: GetUsageRequestGetUsagePaginateTypeDef = {  # (1)
    "usagePlanId": ...,
    "startDate": ...,
    "endDate": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetUsageRequestGetUsagePaginateTypeDef](./type_defs.md#getusagerequestgetusagepaginatetypedef) 
## GetUsagePlanKeysPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_usage_plan_keys")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetUsagePlanKeys)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    usagePlanId: str,
    nameQuery: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[UsagePlanKeysTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: UsagePlanKeysTypeDef](./type_defs.md#usageplankeystypedef) 


```python title="Usage example with kwargs"
kwargs: GetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef = {  # (1)
    "usagePlanId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef](./type_defs.md#getusageplankeysrequestgetusageplankeyspaginatetypedef) 
## GetUsagePlansPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_usage_plans")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetUsagePlans)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    keyId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[UsagePlansTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: UsagePlansTypeDef](./type_defs.md#usageplanstypedef) 


```python title="Usage example with kwargs"
kwargs: GetUsagePlansRequestGetUsagePlansPaginateTypeDef = {  # (1)
    "keyId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetUsagePlansRequestGetUsagePlansPaginateTypeDef](./type_defs.md#getusageplansrequestgetusageplanspaginatetypedef) 
## GetVpcLinksPaginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator("get_vpc_links")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetVpcLinks)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[VpcLinksTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: VpcLinksTypeDef](./type_defs.md#vpclinkstypedef) 


```python title="Usage example with kwargs"
kwargs: GetVpcLinksRequestGetVpcLinksPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetVpcLinksRequestGetVpcLinksPaginateTypeDef](./type_defs.md#getvpclinksrequestgetvpclinkspaginatetypedef) 
