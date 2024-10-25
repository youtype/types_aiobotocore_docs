# APIGatewayClient

> [Index](../README.md) > [APIGateway](./README.md) > APIGatewayClient

!!! note ""

    Auto-generated documentation for [APIGateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway)
    type annotations stubs module [types-aiobotocore-apigateway](https://pypi.org/project/types-aiobotocore-apigateway/).

## APIGatewayClient

Type annotations and code completion for `#!python session.create_client("apigateway")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client)

```python
# APIGatewayClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_apigateway.client import APIGatewayClient

session = get_session()
async with session.create_client("apigateway") as client:
    client: APIGatewayClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("apigateway").exceptions` structure.

```python
# APIGatewayClient.exceptions usage example

async with session.create_client("apigateway") as client:
    try:
        do_something(client)
    except (
            client.BadRequestException,
        client.ClientError,
        client.ConflictException,
        client.LimitExceededException,
        client.NotFoundException,
        client.ServiceUnavailableException,
        client.TooManyRequestsException,
        client.UnauthorizedException,
    ) as e:
        print(e)
```

```python
# APIGatewayClient usage type checking example

from types_aiobotocore_apigateway.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("apigateway").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("apigateway").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_api\_key

Create an ApiKey resource.

Type annotations and code completion for `#!python session.create_client("apigateway").create_api_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_api_key)

```python
# create_api_key method definition

await def create_api_key(
    self,
    *,
    name: str = ...,
    description: str = ...,
    enabled: bool = ...,
    generateDistinctId: bool = ...,
    value: str = ...,
    stageKeys: Sequence[StageKeyTypeDef] = ...,  # (1)
    customerId: str = ...,
    tags: Mapping[str, str] = ...,
) -> ApiKeyResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StageKeyTypeDef](./type_defs.md#stagekeytypedef) 
2. See [:material-code-braces: ApiKeyResponseTypeDef](./type_defs.md#apikeyresponsetypedef) 


```python
# create_api_key method usage example with argument unpacking

kwargs: CreateApiKeyRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.create_api_key(**kwargs)
```

1. See [:material-code-braces: CreateApiKeyRequestRequestTypeDef](./type_defs.md#createapikeyrequestrequesttypedef) 

### create\_authorizer

Adds a new Authorizer resource to an existing RestApi resource.

Type annotations and code completion for `#!python session.create_client("apigateway").create_authorizer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_authorizer)

```python
# create_authorizer method definition

await def create_authorizer(
    self,
    *,
    restApiId: str,
    name: str,
    type: AuthorizerTypeType,  # (1)
    providerARNs: Sequence[str] = ...,
    authType: str = ...,
    authorizerUri: str = ...,
    authorizerCredentials: str = ...,
    identitySource: str = ...,
    identityValidationExpression: str = ...,
    authorizerResultTtlInSeconds: int = ...,
) -> AuthorizerResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AuthorizerTypeType](./literals.md#authorizertypetype) 
2. See [:material-code-braces: AuthorizerResponseTypeDef](./type_defs.md#authorizerresponsetypedef) 


```python
# create_authorizer method usage example with argument unpacking

kwargs: CreateAuthorizerRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "name": ...,
    "type": ...,
}

parent.create_authorizer(**kwargs)
```

1. See [:material-code-braces: CreateAuthorizerRequestRequestTypeDef](./type_defs.md#createauthorizerrequestrequesttypedef) 

### create\_base\_path\_mapping

Creates a new BasePathMapping resource.

Type annotations and code completion for `#!python session.create_client("apigateway").create_base_path_mapping` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_base_path_mapping)

```python
# create_base_path_mapping method definition

await def create_base_path_mapping(
    self,
    *,
    domainName: str,
    restApiId: str,
    basePath: str = ...,
    stage: str = ...,
) -> BasePathMappingResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BasePathMappingResponseTypeDef](./type_defs.md#basepathmappingresponsetypedef) 


```python
# create_base_path_mapping method usage example with argument unpacking

kwargs: CreateBasePathMappingRequestRequestTypeDef = {  # (1)
    "domainName": ...,
    "restApiId": ...,
}

parent.create_base_path_mapping(**kwargs)
```

1. See [:material-code-braces: CreateBasePathMappingRequestRequestTypeDef](./type_defs.md#createbasepathmappingrequestrequesttypedef) 

### create\_deployment

Creates a Deployment resource, which makes a specified RestApi callable over
the
internet.

Type annotations and code completion for `#!python session.create_client("apigateway").create_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_deployment)

```python
# create_deployment method definition

await def create_deployment(
    self,
    *,
    restApiId: str,
    stageName: str = ...,
    stageDescription: str = ...,
    description: str = ...,
    cacheClusterEnabled: bool = ...,
    cacheClusterSize: CacheClusterSizeType = ...,  # (1)
    variables: Mapping[str, str] = ...,
    canarySettings: DeploymentCanarySettingsTypeDef = ...,  # (2)
    tracingEnabled: bool = ...,
) -> DeploymentResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: CacheClusterSizeType](./literals.md#cacheclustersizetype) 
2. See [:material-code-braces: DeploymentCanarySettingsTypeDef](./type_defs.md#deploymentcanarysettingstypedef) 
3. See [:material-code-braces: DeploymentResponseTypeDef](./type_defs.md#deploymentresponsetypedef) 


```python
# create_deployment method usage example with argument unpacking

kwargs: CreateDeploymentRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
}

parent.create_deployment(**kwargs)
```

1. See [:material-code-braces: CreateDeploymentRequestRequestTypeDef](./type_defs.md#createdeploymentrequestrequesttypedef) 

### create\_documentation\_part

Creates a documentation part.

Type annotations and code completion for `#!python session.create_client("apigateway").create_documentation_part` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_documentation_part)

```python
# create_documentation_part method definition

await def create_documentation_part(
    self,
    *,
    restApiId: str,
    location: DocumentationPartLocationTypeDef,  # (1)
    properties: str,
) -> DocumentationPartResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DocumentationPartLocationTypeDef](./type_defs.md#documentationpartlocationtypedef) 
2. See [:material-code-braces: DocumentationPartResponseTypeDef](./type_defs.md#documentationpartresponsetypedef) 


```python
# create_documentation_part method usage example with argument unpacking

kwargs: CreateDocumentationPartRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "location": ...,
    "properties": ...,
}

parent.create_documentation_part(**kwargs)
```

1. See [:material-code-braces: CreateDocumentationPartRequestRequestTypeDef](./type_defs.md#createdocumentationpartrequestrequesttypedef) 

### create\_documentation\_version

Creates a documentation version See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/apigateway-2015-07-09/CreateDocumentationVersion).

Type annotations and code completion for `#!python session.create_client("apigateway").create_documentation_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_documentation_version)

```python
# create_documentation_version method definition

await def create_documentation_version(
    self,
    *,
    restApiId: str,
    documentationVersion: str,
    stageName: str = ...,
    description: str = ...,
) -> DocumentationVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DocumentationVersionResponseTypeDef](./type_defs.md#documentationversionresponsetypedef) 


```python
# create_documentation_version method usage example with argument unpacking

kwargs: CreateDocumentationVersionRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "documentationVersion": ...,
}

parent.create_documentation_version(**kwargs)
```

1. See [:material-code-braces: CreateDocumentationVersionRequestRequestTypeDef](./type_defs.md#createdocumentationversionrequestrequesttypedef) 

### create\_domain\_name

Creates a new domain name.

Type annotations and code completion for `#!python session.create_client("apigateway").create_domain_name` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_domain_name)

```python
# create_domain_name method definition

await def create_domain_name(
    self,
    *,
    domainName: str,
    certificateName: str = ...,
    certificateBody: str = ...,
    certificatePrivateKey: str = ...,
    certificateChain: str = ...,
    certificateArn: str = ...,
    regionalCertificateName: str = ...,
    regionalCertificateArn: str = ...,
    endpointConfiguration: EndpointConfigurationTypeDef = ...,  # (1)
    tags: Mapping[str, str] = ...,
    securityPolicy: SecurityPolicyType = ...,  # (2)
    mutualTlsAuthentication: MutualTlsAuthenticationInputTypeDef = ...,  # (3)
    ownershipVerificationCertificateArn: str = ...,
) -> DomainNameResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: EndpointConfigurationTypeDef](./type_defs.md#endpointconfigurationtypedef) 
2. See [:material-code-brackets: SecurityPolicyType](./literals.md#securitypolicytype) 
3. See [:material-code-braces: MutualTlsAuthenticationInputTypeDef](./type_defs.md#mutualtlsauthenticationinputtypedef) 
4. See [:material-code-braces: DomainNameResponseTypeDef](./type_defs.md#domainnameresponsetypedef) 


```python
# create_domain_name method usage example with argument unpacking

kwargs: CreateDomainNameRequestRequestTypeDef = {  # (1)
    "domainName": ...,
}

parent.create_domain_name(**kwargs)
```

1. See [:material-code-braces: CreateDomainNameRequestRequestTypeDef](./type_defs.md#createdomainnamerequestrequesttypedef) 

### create\_model

Adds a new Model resource to an existing RestApi resource.

Type annotations and code completion for `#!python session.create_client("apigateway").create_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_model)

```python
# create_model method definition

await def create_model(
    self,
    *,
    restApiId: str,
    name: str,
    contentType: str,
    description: str = ...,
    schema: str = ...,
) -> ModelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ModelResponseTypeDef](./type_defs.md#modelresponsetypedef) 


```python
# create_model method usage example with argument unpacking

kwargs: CreateModelRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "name": ...,
    "contentType": ...,
}

parent.create_model(**kwargs)
```

1. See [:material-code-braces: CreateModelRequestRequestTypeDef](./type_defs.md#createmodelrequestrequesttypedef) 

### create\_request\_validator

Creates a RequestValidator of a given RestApi.

Type annotations and code completion for `#!python session.create_client("apigateway").create_request_validator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_request_validator)

```python
# create_request_validator method definition

await def create_request_validator(
    self,
    *,
    restApiId: str,
    name: str = ...,
    validateRequestBody: bool = ...,
    validateRequestParameters: bool = ...,
) -> RequestValidatorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RequestValidatorResponseTypeDef](./type_defs.md#requestvalidatorresponsetypedef) 


```python
# create_request_validator method usage example with argument unpacking

kwargs: CreateRequestValidatorRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
}

parent.create_request_validator(**kwargs)
```

1. See [:material-code-braces: CreateRequestValidatorRequestRequestTypeDef](./type_defs.md#createrequestvalidatorrequestrequesttypedef) 

### create\_resource

Creates a Resource resource.

Type annotations and code completion for `#!python session.create_client("apigateway").create_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_resource)

```python
# create_resource method definition

await def create_resource(
    self,
    *,
    restApiId: str,
    parentId: str,
    pathPart: str,
) -> ResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ResourceResponseTypeDef](./type_defs.md#resourceresponsetypedef) 


```python
# create_resource method usage example with argument unpacking

kwargs: CreateResourceRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "parentId": ...,
    "pathPart": ...,
}

parent.create_resource(**kwargs)
```

1. See [:material-code-braces: CreateResourceRequestRequestTypeDef](./type_defs.md#createresourcerequestrequesttypedef) 

### create\_rest\_api

Creates a new RestApi resource.

Type annotations and code completion for `#!python session.create_client("apigateway").create_rest_api` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_rest_api)

```python
# create_rest_api method definition

await def create_rest_api(
    self,
    *,
    name: str,
    description: str = ...,
    version: str = ...,
    cloneFrom: str = ...,
    binaryMediaTypes: Sequence[str] = ...,
    minimumCompressionSize: int = ...,
    apiKeySource: ApiKeySourceTypeType = ...,  # (1)
    endpointConfiguration: EndpointConfigurationTypeDef = ...,  # (2)
    policy: str = ...,
    tags: Mapping[str, str] = ...,
    disableExecuteApiEndpoint: bool = ...,
) -> RestApiResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ApiKeySourceTypeType](./literals.md#apikeysourcetypetype) 
2. See [:material-code-braces: EndpointConfigurationTypeDef](./type_defs.md#endpointconfigurationtypedef) 
3. See [:material-code-braces: RestApiResponseTypeDef](./type_defs.md#restapiresponsetypedef) 


```python
# create_rest_api method usage example with argument unpacking

kwargs: CreateRestApiRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.create_rest_api(**kwargs)
```

1. See [:material-code-braces: CreateRestApiRequestRequestTypeDef](./type_defs.md#createrestapirequestrequesttypedef) 

### create\_stage

Creates a new Stage resource that references a pre-existing Deployment for the
API.

Type annotations and code completion for `#!python session.create_client("apigateway").create_stage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_stage)

```python
# create_stage method definition

await def create_stage(
    self,
    *,
    restApiId: str,
    stageName: str,
    deploymentId: str,
    description: str = ...,
    cacheClusterEnabled: bool = ...,
    cacheClusterSize: CacheClusterSizeType = ...,  # (1)
    variables: Mapping[str, str] = ...,
    documentationVersion: str = ...,
    canarySettings: CanarySettingsTypeDef = ...,  # (2)
    tracingEnabled: bool = ...,
    tags: Mapping[str, str] = ...,
) -> StageResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: CacheClusterSizeType](./literals.md#cacheclustersizetype) 
2. See [:material-code-braces: CanarySettingsTypeDef](./type_defs.md#canarysettingstypedef) 
3. See [:material-code-braces: StageResponseTypeDef](./type_defs.md#stageresponsetypedef) 


```python
# create_stage method usage example with argument unpacking

kwargs: CreateStageRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "stageName": ...,
    "deploymentId": ...,
}

parent.create_stage(**kwargs)
```

1. See [:material-code-braces: CreateStageRequestRequestTypeDef](./type_defs.md#createstagerequestrequesttypedef) 

### create\_usage\_plan

Creates a usage plan with the throttle and quota limits, as well as the
associated API stages, specified in the
payload.

Type annotations and code completion for `#!python session.create_client("apigateway").create_usage_plan` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_usage_plan)

```python
# create_usage_plan method definition

await def create_usage_plan(
    self,
    *,
    name: str,
    description: str = ...,
    apiStages: Sequence[ApiStageUnionTypeDef] = ...,  # (1)
    throttle: ThrottleSettingsTypeDef = ...,  # (2)
    quota: QuotaSettingsTypeDef = ...,  # (3)
    tags: Mapping[str, str] = ...,
) -> UsagePlanResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: ApiStageTypeDef](./type_defs.md#apistagetypedef) [:material-code-braces: ApiStageOutputTypeDef](./type_defs.md#apistageoutputtypedef) 
2. See [:material-code-braces: ThrottleSettingsTypeDef](./type_defs.md#throttlesettingstypedef) 
3. See [:material-code-braces: QuotaSettingsTypeDef](./type_defs.md#quotasettingstypedef) 
4. See [:material-code-braces: UsagePlanResponseTypeDef](./type_defs.md#usageplanresponsetypedef) 


```python
# create_usage_plan method usage example with argument unpacking

kwargs: CreateUsagePlanRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.create_usage_plan(**kwargs)
```

1. See [:material-code-braces: CreateUsagePlanRequestRequestTypeDef](./type_defs.md#createusageplanrequestrequesttypedef) 

### create\_usage\_plan\_key

Creates a usage plan key for adding an existing API key to a usage plan.

Type annotations and code completion for `#!python session.create_client("apigateway").create_usage_plan_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_usage_plan_key)

```python
# create_usage_plan_key method definition

await def create_usage_plan_key(
    self,
    *,
    usagePlanId: str,
    keyId: str,
    keyType: str,
) -> UsagePlanKeyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UsagePlanKeyResponseTypeDef](./type_defs.md#usageplankeyresponsetypedef) 


```python
# create_usage_plan_key method usage example with argument unpacking

kwargs: CreateUsagePlanKeyRequestRequestTypeDef = {  # (1)
    "usagePlanId": ...,
    "keyId": ...,
    "keyType": ...,
}

parent.create_usage_plan_key(**kwargs)
```

1. See [:material-code-braces: CreateUsagePlanKeyRequestRequestTypeDef](./type_defs.md#createusageplankeyrequestrequesttypedef) 

### create\_vpc\_link

Creates a VPC link, under the caller's account in a selected region, in an
asynchronous operation that typically takes 2-4 minutes to complete and become
operational.

Type annotations and code completion for `#!python session.create_client("apigateway").create_vpc_link` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_vpc_link)

```python
# create_vpc_link method definition

await def create_vpc_link(
    self,
    *,
    name: str,
    targetArns: Sequence[str],
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> VpcLinkResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: VpcLinkResponseTypeDef](./type_defs.md#vpclinkresponsetypedef) 


```python
# create_vpc_link method usage example with argument unpacking

kwargs: CreateVpcLinkRequestRequestTypeDef = {  # (1)
    "name": ...,
    "targetArns": ...,
}

parent.create_vpc_link(**kwargs)
```

1. See [:material-code-braces: CreateVpcLinkRequestRequestTypeDef](./type_defs.md#createvpclinkrequestrequesttypedef) 

### delete\_api\_key

Deletes the ApiKey resource.

Type annotations and code completion for `#!python session.create_client("apigateway").delete_api_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.delete_api_key)

```python
# delete_api_key method definition

await def delete_api_key(
    self,
    *,
    apiKey: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_api_key method usage example with argument unpacking

kwargs: DeleteApiKeyRequestRequestTypeDef = {  # (1)
    "apiKey": ...,
}

parent.delete_api_key(**kwargs)
```

1. See [:material-code-braces: DeleteApiKeyRequestRequestTypeDef](./type_defs.md#deleteapikeyrequestrequesttypedef) 

### delete\_authorizer

Deletes an existing Authorizer resource.

Type annotations and code completion for `#!python session.create_client("apigateway").delete_authorizer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.delete_authorizer)

```python
# delete_authorizer method definition

await def delete_authorizer(
    self,
    *,
    restApiId: str,
    authorizerId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_authorizer method usage example with argument unpacking

kwargs: DeleteAuthorizerRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "authorizerId": ...,
}

parent.delete_authorizer(**kwargs)
```

1. See [:material-code-braces: DeleteAuthorizerRequestRequestTypeDef](./type_defs.md#deleteauthorizerrequestrequesttypedef) 

### delete\_base\_path\_mapping

Deletes the BasePathMapping resource.

Type annotations and code completion for `#!python session.create_client("apigateway").delete_base_path_mapping` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.delete_base_path_mapping)

```python
# delete_base_path_mapping method definition

await def delete_base_path_mapping(
    self,
    *,
    domainName: str,
    basePath: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_base_path_mapping method usage example with argument unpacking

kwargs: DeleteBasePathMappingRequestRequestTypeDef = {  # (1)
    "domainName": ...,
    "basePath": ...,
}

parent.delete_base_path_mapping(**kwargs)
```

1. See [:material-code-braces: DeleteBasePathMappingRequestRequestTypeDef](./type_defs.md#deletebasepathmappingrequestrequesttypedef) 

### delete\_client\_certificate

Deletes the ClientCertificate resource.

Type annotations and code completion for `#!python session.create_client("apigateway").delete_client_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.delete_client_certificate)

```python
# delete_client_certificate method definition

await def delete_client_certificate(
    self,
    *,
    clientCertificateId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_client_certificate method usage example with argument unpacking

kwargs: DeleteClientCertificateRequestRequestTypeDef = {  # (1)
    "clientCertificateId": ...,
}

parent.delete_client_certificate(**kwargs)
```

1. See [:material-code-braces: DeleteClientCertificateRequestRequestTypeDef](./type_defs.md#deleteclientcertificaterequestrequesttypedef) 

### delete\_deployment

Deletes a Deployment resource.

Type annotations and code completion for `#!python session.create_client("apigateway").delete_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.delete_deployment)

```python
# delete_deployment method definition

await def delete_deployment(
    self,
    *,
    restApiId: str,
    deploymentId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_deployment method usage example with argument unpacking

kwargs: DeleteDeploymentRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "deploymentId": ...,
}

parent.delete_deployment(**kwargs)
```

1. See [:material-code-braces: DeleteDeploymentRequestRequestTypeDef](./type_defs.md#deletedeploymentrequestrequesttypedef) 

### delete\_documentation\_part

Deletes a documentation part See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/apigateway-2015-07-09/DeleteDocumentationPart).

Type annotations and code completion for `#!python session.create_client("apigateway").delete_documentation_part` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.delete_documentation_part)

```python
# delete_documentation_part method definition

await def delete_documentation_part(
    self,
    *,
    restApiId: str,
    documentationPartId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_documentation_part method usage example with argument unpacking

kwargs: DeleteDocumentationPartRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "documentationPartId": ...,
}

parent.delete_documentation_part(**kwargs)
```

1. See [:material-code-braces: DeleteDocumentationPartRequestRequestTypeDef](./type_defs.md#deletedocumentationpartrequestrequesttypedef) 

### delete\_documentation\_version

Deletes a documentation version.

Type annotations and code completion for `#!python session.create_client("apigateway").delete_documentation_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.delete_documentation_version)

```python
# delete_documentation_version method definition

await def delete_documentation_version(
    self,
    *,
    restApiId: str,
    documentationVersion: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_documentation_version method usage example with argument unpacking

kwargs: DeleteDocumentationVersionRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "documentationVersion": ...,
}

parent.delete_documentation_version(**kwargs)
```

1. See [:material-code-braces: DeleteDocumentationVersionRequestRequestTypeDef](./type_defs.md#deletedocumentationversionrequestrequesttypedef) 

### delete\_domain\_name

Deletes the DomainName resource.

Type annotations and code completion for `#!python session.create_client("apigateway").delete_domain_name` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.delete_domain_name)

```python
# delete_domain_name method definition

await def delete_domain_name(
    self,
    *,
    domainName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_domain_name method usage example with argument unpacking

kwargs: DeleteDomainNameRequestRequestTypeDef = {  # (1)
    "domainName": ...,
}

parent.delete_domain_name(**kwargs)
```

1. See [:material-code-braces: DeleteDomainNameRequestRequestTypeDef](./type_defs.md#deletedomainnamerequestrequesttypedef) 

### delete\_gateway\_response

Clears any customization of a GatewayResponse of a specified response type on
the given RestApi and resets it with the default
settings.

Type annotations and code completion for `#!python session.create_client("apigateway").delete_gateway_response` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.delete_gateway_response)

```python
# delete_gateway_response method definition

await def delete_gateway_response(
    self,
    *,
    restApiId: str,
    responseType: GatewayResponseTypeType,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: GatewayResponseTypeType](./literals.md#gatewayresponsetypetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_gateway_response method usage example with argument unpacking

kwargs: DeleteGatewayResponseRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "responseType": ...,
}

parent.delete_gateway_response(**kwargs)
```

1. See [:material-code-braces: DeleteGatewayResponseRequestRequestTypeDef](./type_defs.md#deletegatewayresponserequestrequesttypedef) 

### delete\_integration

Represents a delete integration.

Type annotations and code completion for `#!python session.create_client("apigateway").delete_integration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.delete_integration)

```python
# delete_integration method definition

await def delete_integration(
    self,
    *,
    restApiId: str,
    resourceId: str,
    httpMethod: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_integration method usage example with argument unpacking

kwargs: DeleteIntegrationRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "resourceId": ...,
    "httpMethod": ...,
}

parent.delete_integration(**kwargs)
```

1. See [:material-code-braces: DeleteIntegrationRequestRequestTypeDef](./type_defs.md#deleteintegrationrequestrequesttypedef) 

### delete\_integration\_response

Represents a delete integration response.

Type annotations and code completion for `#!python session.create_client("apigateway").delete_integration_response` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.delete_integration_response)

```python
# delete_integration_response method definition

await def delete_integration_response(
    self,
    *,
    restApiId: str,
    resourceId: str,
    httpMethod: str,
    statusCode: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_integration_response method usage example with argument unpacking

kwargs: DeleteIntegrationResponseRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "resourceId": ...,
    "httpMethod": ...,
    "statusCode": ...,
}

parent.delete_integration_response(**kwargs)
```

1. See [:material-code-braces: DeleteIntegrationResponseRequestRequestTypeDef](./type_defs.md#deleteintegrationresponserequestrequesttypedef) 

### delete\_method

Deletes an existing Method resource.

Type annotations and code completion for `#!python session.create_client("apigateway").delete_method` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.delete_method)

```python
# delete_method method definition

await def delete_method(
    self,
    *,
    restApiId: str,
    resourceId: str,
    httpMethod: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_method method usage example with argument unpacking

kwargs: DeleteMethodRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "resourceId": ...,
    "httpMethod": ...,
}

parent.delete_method(**kwargs)
```

1. See [:material-code-braces: DeleteMethodRequestRequestTypeDef](./type_defs.md#deletemethodrequestrequesttypedef) 

### delete\_method\_response

Deletes an existing MethodResponse resource.

Type annotations and code completion for `#!python session.create_client("apigateway").delete_method_response` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.delete_method_response)

```python
# delete_method_response method definition

await def delete_method_response(
    self,
    *,
    restApiId: str,
    resourceId: str,
    httpMethod: str,
    statusCode: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_method_response method usage example with argument unpacking

kwargs: DeleteMethodResponseRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "resourceId": ...,
    "httpMethod": ...,
    "statusCode": ...,
}

parent.delete_method_response(**kwargs)
```

1. See [:material-code-braces: DeleteMethodResponseRequestRequestTypeDef](./type_defs.md#deletemethodresponserequestrequesttypedef) 

### delete\_model

Deletes a model.

Type annotations and code completion for `#!python session.create_client("apigateway").delete_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.delete_model)

```python
# delete_model method definition

await def delete_model(
    self,
    *,
    restApiId: str,
    modelName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_model method usage example with argument unpacking

kwargs: DeleteModelRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "modelName": ...,
}

parent.delete_model(**kwargs)
```

1. See [:material-code-braces: DeleteModelRequestRequestTypeDef](./type_defs.md#deletemodelrequestrequesttypedef) 

### delete\_request\_validator

Deletes a RequestValidator of a given RestApi.

Type annotations and code completion for `#!python session.create_client("apigateway").delete_request_validator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.delete_request_validator)

```python
# delete_request_validator method definition

await def delete_request_validator(
    self,
    *,
    restApiId: str,
    requestValidatorId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_request_validator method usage example with argument unpacking

kwargs: DeleteRequestValidatorRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "requestValidatorId": ...,
}

parent.delete_request_validator(**kwargs)
```

1. See [:material-code-braces: DeleteRequestValidatorRequestRequestTypeDef](./type_defs.md#deleterequestvalidatorrequestrequesttypedef) 

### delete\_resource

Deletes a Resource resource.

Type annotations and code completion for `#!python session.create_client("apigateway").delete_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.delete_resource)

```python
# delete_resource method definition

await def delete_resource(
    self,
    *,
    restApiId: str,
    resourceId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_resource method usage example with argument unpacking

kwargs: DeleteResourceRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "resourceId": ...,
}

parent.delete_resource(**kwargs)
```

1. See [:material-code-braces: DeleteResourceRequestRequestTypeDef](./type_defs.md#deleteresourcerequestrequesttypedef) 

### delete\_rest\_api

Deletes the specified API.

Type annotations and code completion for `#!python session.create_client("apigateway").delete_rest_api` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.delete_rest_api)

```python
# delete_rest_api method definition

await def delete_rest_api(
    self,
    *,
    restApiId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_rest_api method usage example with argument unpacking

kwargs: DeleteRestApiRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
}

parent.delete_rest_api(**kwargs)
```

1. See [:material-code-braces: DeleteRestApiRequestRequestTypeDef](./type_defs.md#deleterestapirequestrequesttypedef) 

### delete\_stage

Deletes a Stage resource.

Type annotations and code completion for `#!python session.create_client("apigateway").delete_stage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.delete_stage)

```python
# delete_stage method definition

await def delete_stage(
    self,
    *,
    restApiId: str,
    stageName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_stage method usage example with argument unpacking

kwargs: DeleteStageRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "stageName": ...,
}

parent.delete_stage(**kwargs)
```

1. See [:material-code-braces: DeleteStageRequestRequestTypeDef](./type_defs.md#deletestagerequestrequesttypedef) 

### delete\_usage\_plan

Deletes a usage plan of a given plan Id.

Type annotations and code completion for `#!python session.create_client("apigateway").delete_usage_plan` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.delete_usage_plan)

```python
# delete_usage_plan method definition

await def delete_usage_plan(
    self,
    *,
    usagePlanId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_usage_plan method usage example with argument unpacking

kwargs: DeleteUsagePlanRequestRequestTypeDef = {  # (1)
    "usagePlanId": ...,
}

parent.delete_usage_plan(**kwargs)
```

1. See [:material-code-braces: DeleteUsagePlanRequestRequestTypeDef](./type_defs.md#deleteusageplanrequestrequesttypedef) 

### delete\_usage\_plan\_key

Deletes a usage plan key and remove the underlying API key from the associated
usage
plan.

Type annotations and code completion for `#!python session.create_client("apigateway").delete_usage_plan_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.delete_usage_plan_key)

```python
# delete_usage_plan_key method definition

await def delete_usage_plan_key(
    self,
    *,
    usagePlanId: str,
    keyId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_usage_plan_key method usage example with argument unpacking

kwargs: DeleteUsagePlanKeyRequestRequestTypeDef = {  # (1)
    "usagePlanId": ...,
    "keyId": ...,
}

parent.delete_usage_plan_key(**kwargs)
```

1. See [:material-code-braces: DeleteUsagePlanKeyRequestRequestTypeDef](./type_defs.md#deleteusageplankeyrequestrequesttypedef) 

### delete\_vpc\_link

Deletes an existing VpcLink of a specified identifier.

Type annotations and code completion for `#!python session.create_client("apigateway").delete_vpc_link` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.delete_vpc_link)

```python
# delete_vpc_link method definition

await def delete_vpc_link(
    self,
    *,
    vpcLinkId: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_vpc_link method usage example with argument unpacking

kwargs: DeleteVpcLinkRequestRequestTypeDef = {  # (1)
    "vpcLinkId": ...,
}

parent.delete_vpc_link(**kwargs)
```

1. See [:material-code-braces: DeleteVpcLinkRequestRequestTypeDef](./type_defs.md#deletevpclinkrequestrequesttypedef) 

### flush\_stage\_authorizers\_cache

Flushes all authorizer cache entries on a stage.

Type annotations and code completion for `#!python session.create_client("apigateway").flush_stage_authorizers_cache` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.flush_stage_authorizers_cache)

```python
# flush_stage_authorizers_cache method definition

await def flush_stage_authorizers_cache(
    self,
    *,
    restApiId: str,
    stageName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# flush_stage_authorizers_cache method usage example with argument unpacking

kwargs: FlushStageAuthorizersCacheRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "stageName": ...,
}

parent.flush_stage_authorizers_cache(**kwargs)
```

1. See [:material-code-braces: FlushStageAuthorizersCacheRequestRequestTypeDef](./type_defs.md#flushstageauthorizerscacherequestrequesttypedef) 

### flush\_stage\_cache

Flushes a stage's cache.

Type annotations and code completion for `#!python session.create_client("apigateway").flush_stage_cache` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.flush_stage_cache)

```python
# flush_stage_cache method definition

await def flush_stage_cache(
    self,
    *,
    restApiId: str,
    stageName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# flush_stage_cache method usage example with argument unpacking

kwargs: FlushStageCacheRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "stageName": ...,
}

parent.flush_stage_cache(**kwargs)
```

1. See [:material-code-braces: FlushStageCacheRequestRequestTypeDef](./type_defs.md#flushstagecacherequestrequesttypedef) 

### generate\_client\_certificate

Generates a ClientCertificate resource.

Type annotations and code completion for `#!python session.create_client("apigateway").generate_client_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.generate_client_certificate)

```python
# generate_client_certificate method definition

await def generate_client_certificate(
    self,
    *,
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> ClientCertificateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ClientCertificateResponseTypeDef](./type_defs.md#clientcertificateresponsetypedef) 


```python
# generate_client_certificate method usage example with argument unpacking

kwargs: GenerateClientCertificateRequestRequestTypeDef = {  # (1)
    "description": ...,
}

parent.generate_client_certificate(**kwargs)
```

1. See [:material-code-braces: GenerateClientCertificateRequestRequestTypeDef](./type_defs.md#generateclientcertificaterequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("apigateway").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.generate_presigned_url)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### get\_account

Gets information about the current Account resource.

Type annotations and code completion for `#!python session.create_client("apigateway").get_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_account)

```python
# get_account method definition

await def get_account(
    self,
) -> AccountTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AccountTypeDef](./type_defs.md#accounttypedef) 

### get\_api\_key

Gets information about the current ApiKey resource.

Type annotations and code completion for `#!python session.create_client("apigateway").get_api_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_api_key)

```python
# get_api_key method definition

await def get_api_key(
    self,
    *,
    apiKey: str,
    includeValue: bool = ...,
) -> ApiKeyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ApiKeyResponseTypeDef](./type_defs.md#apikeyresponsetypedef) 


```python
# get_api_key method usage example with argument unpacking

kwargs: GetApiKeyRequestRequestTypeDef = {  # (1)
    "apiKey": ...,
}

parent.get_api_key(**kwargs)
```

1. See [:material-code-braces: GetApiKeyRequestRequestTypeDef](./type_defs.md#getapikeyrequestrequesttypedef) 

### get\_api\_keys

Gets information about the current ApiKeys resource.

Type annotations and code completion for `#!python session.create_client("apigateway").get_api_keys` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_api_keys)

```python
# get_api_keys method definition

await def get_api_keys(
    self,
    *,
    position: str = ...,
    limit: int = ...,
    nameQuery: str = ...,
    customerId: str = ...,
    includeValues: bool = ...,
) -> ApiKeysTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ApiKeysTypeDef](./type_defs.md#apikeystypedef) 


```python
# get_api_keys method usage example with argument unpacking

kwargs: GetApiKeysRequestRequestTypeDef = {  # (1)
    "position": ...,
}

parent.get_api_keys(**kwargs)
```

1. See [:material-code-braces: GetApiKeysRequestRequestTypeDef](./type_defs.md#getapikeysrequestrequesttypedef) 

### get\_authorizer

Describe an existing Authorizer resource.

Type annotations and code completion for `#!python session.create_client("apigateway").get_authorizer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_authorizer)

```python
# get_authorizer method definition

await def get_authorizer(
    self,
    *,
    restApiId: str,
    authorizerId: str,
) -> AuthorizerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AuthorizerResponseTypeDef](./type_defs.md#authorizerresponsetypedef) 


```python
# get_authorizer method usage example with argument unpacking

kwargs: GetAuthorizerRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "authorizerId": ...,
}

parent.get_authorizer(**kwargs)
```

1. See [:material-code-braces: GetAuthorizerRequestRequestTypeDef](./type_defs.md#getauthorizerrequestrequesttypedef) 

### get\_authorizers

Describe an existing Authorizers resource.

Type annotations and code completion for `#!python session.create_client("apigateway").get_authorizers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_authorizers)

```python
# get_authorizers method definition

await def get_authorizers(
    self,
    *,
    restApiId: str,
    position: str = ...,
    limit: int = ...,
) -> AuthorizersTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AuthorizersTypeDef](./type_defs.md#authorizerstypedef) 


```python
# get_authorizers method usage example with argument unpacking

kwargs: GetAuthorizersRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
}

parent.get_authorizers(**kwargs)
```

1. See [:material-code-braces: GetAuthorizersRequestRequestTypeDef](./type_defs.md#getauthorizersrequestrequesttypedef) 

### get\_base\_path\_mapping

Describe a BasePathMapping resource.

Type annotations and code completion for `#!python session.create_client("apigateway").get_base_path_mapping` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_base_path_mapping)

```python
# get_base_path_mapping method definition

await def get_base_path_mapping(
    self,
    *,
    domainName: str,
    basePath: str,
) -> BasePathMappingResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BasePathMappingResponseTypeDef](./type_defs.md#basepathmappingresponsetypedef) 


```python
# get_base_path_mapping method usage example with argument unpacking

kwargs: GetBasePathMappingRequestRequestTypeDef = {  # (1)
    "domainName": ...,
    "basePath": ...,
}

parent.get_base_path_mapping(**kwargs)
```

1. See [:material-code-braces: GetBasePathMappingRequestRequestTypeDef](./type_defs.md#getbasepathmappingrequestrequesttypedef) 

### get\_base\_path\_mappings

Represents a collection of BasePathMapping resources.

Type annotations and code completion for `#!python session.create_client("apigateway").get_base_path_mappings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_base_path_mappings)

```python
# get_base_path_mappings method definition

await def get_base_path_mappings(
    self,
    *,
    domainName: str,
    position: str = ...,
    limit: int = ...,
) -> BasePathMappingsTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BasePathMappingsTypeDef](./type_defs.md#basepathmappingstypedef) 


```python
# get_base_path_mappings method usage example with argument unpacking

kwargs: GetBasePathMappingsRequestRequestTypeDef = {  # (1)
    "domainName": ...,
}

parent.get_base_path_mappings(**kwargs)
```

1. See [:material-code-braces: GetBasePathMappingsRequestRequestTypeDef](./type_defs.md#getbasepathmappingsrequestrequesttypedef) 

### get\_client\_certificate

Gets information about the current ClientCertificate resource.

Type annotations and code completion for `#!python session.create_client("apigateway").get_client_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_client_certificate)

```python
# get_client_certificate method definition

await def get_client_certificate(
    self,
    *,
    clientCertificateId: str,
) -> ClientCertificateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ClientCertificateResponseTypeDef](./type_defs.md#clientcertificateresponsetypedef) 


```python
# get_client_certificate method usage example with argument unpacking

kwargs: GetClientCertificateRequestRequestTypeDef = {  # (1)
    "clientCertificateId": ...,
}

parent.get_client_certificate(**kwargs)
```

1. See [:material-code-braces: GetClientCertificateRequestRequestTypeDef](./type_defs.md#getclientcertificaterequestrequesttypedef) 

### get\_client\_certificates

Gets a collection of ClientCertificate resources.

Type annotations and code completion for `#!python session.create_client("apigateway").get_client_certificates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_client_certificates)

```python
# get_client_certificates method definition

await def get_client_certificates(
    self,
    *,
    position: str = ...,
    limit: int = ...,
) -> ClientCertificatesTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ClientCertificatesTypeDef](./type_defs.md#clientcertificatestypedef) 


```python
# get_client_certificates method usage example with argument unpacking

kwargs: GetClientCertificatesRequestRequestTypeDef = {  # (1)
    "position": ...,
}

parent.get_client_certificates(**kwargs)
```

1. See [:material-code-braces: GetClientCertificatesRequestRequestTypeDef](./type_defs.md#getclientcertificatesrequestrequesttypedef) 

### get\_deployment

Gets information about a Deployment resource.

Type annotations and code completion for `#!python session.create_client("apigateway").get_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_deployment)

```python
# get_deployment method definition

await def get_deployment(
    self,
    *,
    restApiId: str,
    deploymentId: str,
    embed: Sequence[str] = ...,
) -> DeploymentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeploymentResponseTypeDef](./type_defs.md#deploymentresponsetypedef) 


```python
# get_deployment method usage example with argument unpacking

kwargs: GetDeploymentRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "deploymentId": ...,
}

parent.get_deployment(**kwargs)
```

1. See [:material-code-braces: GetDeploymentRequestRequestTypeDef](./type_defs.md#getdeploymentrequestrequesttypedef) 

### get\_deployments

Gets information about a Deployments collection.

Type annotations and code completion for `#!python session.create_client("apigateway").get_deployments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_deployments)

```python
# get_deployments method definition

await def get_deployments(
    self,
    *,
    restApiId: str,
    position: str = ...,
    limit: int = ...,
) -> DeploymentsTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeploymentsTypeDef](./type_defs.md#deploymentstypedef) 


```python
# get_deployments method usage example with argument unpacking

kwargs: GetDeploymentsRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
}

parent.get_deployments(**kwargs)
```

1. See [:material-code-braces: GetDeploymentsRequestRequestTypeDef](./type_defs.md#getdeploymentsrequestrequesttypedef) 

### get\_documentation\_part

Gets a documentation part.

Type annotations and code completion for `#!python session.create_client("apigateway").get_documentation_part` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_documentation_part)

```python
# get_documentation_part method definition

await def get_documentation_part(
    self,
    *,
    restApiId: str,
    documentationPartId: str,
) -> DocumentationPartResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DocumentationPartResponseTypeDef](./type_defs.md#documentationpartresponsetypedef) 


```python
# get_documentation_part method usage example with argument unpacking

kwargs: GetDocumentationPartRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "documentationPartId": ...,
}

parent.get_documentation_part(**kwargs)
```

1. See [:material-code-braces: GetDocumentationPartRequestRequestTypeDef](./type_defs.md#getdocumentationpartrequestrequesttypedef) 

### get\_documentation\_parts

Gets documentation parts.

Type annotations and code completion for `#!python session.create_client("apigateway").get_documentation_parts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_documentation_parts)

```python
# get_documentation_parts method definition

await def get_documentation_parts(
    self,
    *,
    restApiId: str,
    type: DocumentationPartTypeType = ...,  # (1)
    nameQuery: str = ...,
    path: str = ...,
    position: str = ...,
    limit: int = ...,
    locationStatus: LocationStatusTypeType = ...,  # (2)
) -> DocumentationPartsTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: DocumentationPartTypeType](./literals.md#documentationparttypetype) 
2. See [:material-code-brackets: LocationStatusTypeType](./literals.md#locationstatustypetype) 
3. See [:material-code-braces: DocumentationPartsTypeDef](./type_defs.md#documentationpartstypedef) 


```python
# get_documentation_parts method usage example with argument unpacking

kwargs: GetDocumentationPartsRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
}

parent.get_documentation_parts(**kwargs)
```

1. See [:material-code-braces: GetDocumentationPartsRequestRequestTypeDef](./type_defs.md#getdocumentationpartsrequestrequesttypedef) 

### get\_documentation\_version

Gets a documentation version.

Type annotations and code completion for `#!python session.create_client("apigateway").get_documentation_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_documentation_version)

```python
# get_documentation_version method definition

await def get_documentation_version(
    self,
    *,
    restApiId: str,
    documentationVersion: str,
) -> DocumentationVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DocumentationVersionResponseTypeDef](./type_defs.md#documentationversionresponsetypedef) 


```python
# get_documentation_version method usage example with argument unpacking

kwargs: GetDocumentationVersionRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "documentationVersion": ...,
}

parent.get_documentation_version(**kwargs)
```

1. See [:material-code-braces: GetDocumentationVersionRequestRequestTypeDef](./type_defs.md#getdocumentationversionrequestrequesttypedef) 

### get\_documentation\_versions

Gets documentation versions.

Type annotations and code completion for `#!python session.create_client("apigateway").get_documentation_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_documentation_versions)

```python
# get_documentation_versions method definition

await def get_documentation_versions(
    self,
    *,
    restApiId: str,
    position: str = ...,
    limit: int = ...,
) -> DocumentationVersionsTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DocumentationVersionsTypeDef](./type_defs.md#documentationversionstypedef) 


```python
# get_documentation_versions method usage example with argument unpacking

kwargs: GetDocumentationVersionsRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
}

parent.get_documentation_versions(**kwargs)
```

1. See [:material-code-braces: GetDocumentationVersionsRequestRequestTypeDef](./type_defs.md#getdocumentationversionsrequestrequesttypedef) 

### get\_domain\_name

Represents a domain name that is contained in a simpler, more intuitive URL
that can be
called.

Type annotations and code completion for `#!python session.create_client("apigateway").get_domain_name` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_domain_name)

```python
# get_domain_name method definition

await def get_domain_name(
    self,
    *,
    domainName: str,
) -> DomainNameResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DomainNameResponseTypeDef](./type_defs.md#domainnameresponsetypedef) 


```python
# get_domain_name method usage example with argument unpacking

kwargs: GetDomainNameRequestRequestTypeDef = {  # (1)
    "domainName": ...,
}

parent.get_domain_name(**kwargs)
```

1. See [:material-code-braces: GetDomainNameRequestRequestTypeDef](./type_defs.md#getdomainnamerequestrequesttypedef) 

### get\_domain\_names

Represents a collection of DomainName resources.

Type annotations and code completion for `#!python session.create_client("apigateway").get_domain_names` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_domain_names)

```python
# get_domain_names method definition

await def get_domain_names(
    self,
    *,
    position: str = ...,
    limit: int = ...,
) -> DomainNamesTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DomainNamesTypeDef](./type_defs.md#domainnamestypedef) 


```python
# get_domain_names method usage example with argument unpacking

kwargs: GetDomainNamesRequestRequestTypeDef = {  # (1)
    "position": ...,
}

parent.get_domain_names(**kwargs)
```

1. See [:material-code-braces: GetDomainNamesRequestRequestTypeDef](./type_defs.md#getdomainnamesrequestrequesttypedef) 

### get\_export

Exports a deployed version of a RestApi in a specified format.

Type annotations and code completion for `#!python session.create_client("apigateway").get_export` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_export)

```python
# get_export method definition

await def get_export(
    self,
    *,
    restApiId: str,
    stageName: str,
    exportType: str,
    parameters: Mapping[str, str] = ...,
    accepts: str = ...,
) -> ExportResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ExportResponseTypeDef](./type_defs.md#exportresponsetypedef) 


```python
# get_export method usage example with argument unpacking

kwargs: GetExportRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "stageName": ...,
    "exportType": ...,
}

parent.get_export(**kwargs)
```

1. See [:material-code-braces: GetExportRequestRequestTypeDef](./type_defs.md#getexportrequestrequesttypedef) 

### get\_gateway\_response

Gets a GatewayResponse of a specified response type on the given RestApi.

Type annotations and code completion for `#!python session.create_client("apigateway").get_gateway_response` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_gateway_response)

```python
# get_gateway_response method definition

await def get_gateway_response(
    self,
    *,
    restApiId: str,
    responseType: GatewayResponseTypeType,  # (1)
) -> GatewayResponseResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: GatewayResponseTypeType](./literals.md#gatewayresponsetypetype) 
2. See [:material-code-braces: GatewayResponseResponseTypeDef](./type_defs.md#gatewayresponseresponsetypedef) 


```python
# get_gateway_response method usage example with argument unpacking

kwargs: GetGatewayResponseRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "responseType": ...,
}

parent.get_gateway_response(**kwargs)
```

1. See [:material-code-braces: GetGatewayResponseRequestRequestTypeDef](./type_defs.md#getgatewayresponserequestrequesttypedef) 

### get\_gateway\_responses

Gets the GatewayResponses collection on the given RestApi.

Type annotations and code completion for `#!python session.create_client("apigateway").get_gateway_responses` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_gateway_responses)

```python
# get_gateway_responses method definition

await def get_gateway_responses(
    self,
    *,
    restApiId: str,
    position: str = ...,
    limit: int = ...,
) -> GatewayResponsesTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GatewayResponsesTypeDef](./type_defs.md#gatewayresponsestypedef) 


```python
# get_gateway_responses method usage example with argument unpacking

kwargs: GetGatewayResponsesRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
}

parent.get_gateway_responses(**kwargs)
```

1. See [:material-code-braces: GetGatewayResponsesRequestRequestTypeDef](./type_defs.md#getgatewayresponsesrequestrequesttypedef) 

### get\_integration

Get the integration settings.

Type annotations and code completion for `#!python session.create_client("apigateway").get_integration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_integration)

```python
# get_integration method definition

await def get_integration(
    self,
    *,
    restApiId: str,
    resourceId: str,
    httpMethod: str,
) -> IntegrationExtraResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: IntegrationExtraResponseTypeDef](./type_defs.md#integrationextraresponsetypedef) 


```python
# get_integration method usage example with argument unpacking

kwargs: GetIntegrationRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "resourceId": ...,
    "httpMethod": ...,
}

parent.get_integration(**kwargs)
```

1. See [:material-code-braces: GetIntegrationRequestRequestTypeDef](./type_defs.md#getintegrationrequestrequesttypedef) 

### get\_integration\_response

Represents a get integration response.

Type annotations and code completion for `#!python session.create_client("apigateway").get_integration_response` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_integration_response)

```python
# get_integration_response method definition

await def get_integration_response(
    self,
    *,
    restApiId: str,
    resourceId: str,
    httpMethod: str,
    statusCode: str,
) -> IntegrationResponseResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: IntegrationResponseResponseTypeDef](./type_defs.md#integrationresponseresponsetypedef) 


```python
# get_integration_response method usage example with argument unpacking

kwargs: GetIntegrationResponseRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "resourceId": ...,
    "httpMethod": ...,
    "statusCode": ...,
}

parent.get_integration_response(**kwargs)
```

1. See [:material-code-braces: GetIntegrationResponseRequestRequestTypeDef](./type_defs.md#getintegrationresponserequestrequesttypedef) 

### get\_method

Describe an existing Method resource.

Type annotations and code completion for `#!python session.create_client("apigateway").get_method` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_method)

```python
# get_method method definition

await def get_method(
    self,
    *,
    restApiId: str,
    resourceId: str,
    httpMethod: str,
) -> MethodExtraResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: MethodExtraResponseTypeDef](./type_defs.md#methodextraresponsetypedef) 


```python
# get_method method usage example with argument unpacking

kwargs: GetMethodRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "resourceId": ...,
    "httpMethod": ...,
}

parent.get_method(**kwargs)
```

1. See [:material-code-braces: GetMethodRequestRequestTypeDef](./type_defs.md#getmethodrequestrequesttypedef) 

### get\_method\_response

Describes a MethodResponse resource.

Type annotations and code completion for `#!python session.create_client("apigateway").get_method_response` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_method_response)

```python
# get_method_response method definition

await def get_method_response(
    self,
    *,
    restApiId: str,
    resourceId: str,
    httpMethod: str,
    statusCode: str,
) -> MethodResponseResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: MethodResponseResponseTypeDef](./type_defs.md#methodresponseresponsetypedef) 


```python
# get_method_response method usage example with argument unpacking

kwargs: GetMethodResponseRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "resourceId": ...,
    "httpMethod": ...,
    "statusCode": ...,
}

parent.get_method_response(**kwargs)
```

1. See [:material-code-braces: GetMethodResponseRequestRequestTypeDef](./type_defs.md#getmethodresponserequestrequesttypedef) 

### get\_model

Describes an existing model defined for a RestApi resource.

Type annotations and code completion for `#!python session.create_client("apigateway").get_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_model)

```python
# get_model method definition

await def get_model(
    self,
    *,
    restApiId: str,
    modelName: str,
    flatten: bool = ...,
) -> ModelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ModelResponseTypeDef](./type_defs.md#modelresponsetypedef) 


```python
# get_model method usage example with argument unpacking

kwargs: GetModelRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "modelName": ...,
}

parent.get_model(**kwargs)
```

1. See [:material-code-braces: GetModelRequestRequestTypeDef](./type_defs.md#getmodelrequestrequesttypedef) 

### get\_model\_template

Generates a sample mapping template that can be used to transform a payload
into the structure of a
model.

Type annotations and code completion for `#!python session.create_client("apigateway").get_model_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_model_template)

```python
# get_model_template method definition

await def get_model_template(
    self,
    *,
    restApiId: str,
    modelName: str,
) -> TemplateTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: TemplateTypeDef](./type_defs.md#templatetypedef) 


```python
# get_model_template method usage example with argument unpacking

kwargs: GetModelTemplateRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "modelName": ...,
}

parent.get_model_template(**kwargs)
```

1. See [:material-code-braces: GetModelTemplateRequestRequestTypeDef](./type_defs.md#getmodeltemplaterequestrequesttypedef) 

### get\_models

Describes existing Models defined for a RestApi resource.

Type annotations and code completion for `#!python session.create_client("apigateway").get_models` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_models)

```python
# get_models method definition

await def get_models(
    self,
    *,
    restApiId: str,
    position: str = ...,
    limit: int = ...,
) -> ModelsTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ModelsTypeDef](./type_defs.md#modelstypedef) 


```python
# get_models method usage example with argument unpacking

kwargs: GetModelsRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
}

parent.get_models(**kwargs)
```

1. See [:material-code-braces: GetModelsRequestRequestTypeDef](./type_defs.md#getmodelsrequestrequesttypedef) 

### get\_request\_validator

Gets a RequestValidator of a given RestApi.

Type annotations and code completion for `#!python session.create_client("apigateway").get_request_validator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_request_validator)

```python
# get_request_validator method definition

await def get_request_validator(
    self,
    *,
    restApiId: str,
    requestValidatorId: str,
) -> RequestValidatorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RequestValidatorResponseTypeDef](./type_defs.md#requestvalidatorresponsetypedef) 


```python
# get_request_validator method usage example with argument unpacking

kwargs: GetRequestValidatorRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "requestValidatorId": ...,
}

parent.get_request_validator(**kwargs)
```

1. See [:material-code-braces: GetRequestValidatorRequestRequestTypeDef](./type_defs.md#getrequestvalidatorrequestrequesttypedef) 

### get\_request\_validators

Gets the RequestValidators collection of a given RestApi.

Type annotations and code completion for `#!python session.create_client("apigateway").get_request_validators` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_request_validators)

```python
# get_request_validators method definition

await def get_request_validators(
    self,
    *,
    restApiId: str,
    position: str = ...,
    limit: int = ...,
) -> RequestValidatorsTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RequestValidatorsTypeDef](./type_defs.md#requestvalidatorstypedef) 


```python
# get_request_validators method usage example with argument unpacking

kwargs: GetRequestValidatorsRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
}

parent.get_request_validators(**kwargs)
```

1. See [:material-code-braces: GetRequestValidatorsRequestRequestTypeDef](./type_defs.md#getrequestvalidatorsrequestrequesttypedef) 

### get\_resource

Lists information about a resource.

Type annotations and code completion for `#!python session.create_client("apigateway").get_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_resource)

```python
# get_resource method definition

await def get_resource(
    self,
    *,
    restApiId: str,
    resourceId: str,
    embed: Sequence[str] = ...,
) -> ResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ResourceResponseTypeDef](./type_defs.md#resourceresponsetypedef) 


```python
# get_resource method usage example with argument unpacking

kwargs: GetResourceRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "resourceId": ...,
}

parent.get_resource(**kwargs)
```

1. See [:material-code-braces: GetResourceRequestRequestTypeDef](./type_defs.md#getresourcerequestrequesttypedef) 

### get\_resources

Lists information about a collection of Resource resources.

Type annotations and code completion for `#!python session.create_client("apigateway").get_resources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_resources)

```python
# get_resources method definition

await def get_resources(
    self,
    *,
    restApiId: str,
    position: str = ...,
    limit: int = ...,
    embed: Sequence[str] = ...,
) -> ResourcesTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ResourcesTypeDef](./type_defs.md#resourcestypedef) 


```python
# get_resources method usage example with argument unpacking

kwargs: GetResourcesRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
}

parent.get_resources(**kwargs)
```

1. See [:material-code-braces: GetResourcesRequestRequestTypeDef](./type_defs.md#getresourcesrequestrequesttypedef) 

### get\_rest\_api

Lists the RestApi resource in the collection.

Type annotations and code completion for `#!python session.create_client("apigateway").get_rest_api` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_rest_api)

```python
# get_rest_api method definition

await def get_rest_api(
    self,
    *,
    restApiId: str,
) -> RestApiResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RestApiResponseTypeDef](./type_defs.md#restapiresponsetypedef) 


```python
# get_rest_api method usage example with argument unpacking

kwargs: GetRestApiRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
}

parent.get_rest_api(**kwargs)
```

1. See [:material-code-braces: GetRestApiRequestRequestTypeDef](./type_defs.md#getrestapirequestrequesttypedef) 

### get\_rest\_apis

Lists the RestApis resources for your collection.

Type annotations and code completion for `#!python session.create_client("apigateway").get_rest_apis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_rest_apis)

```python
# get_rest_apis method definition

await def get_rest_apis(
    self,
    *,
    position: str = ...,
    limit: int = ...,
) -> RestApisTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RestApisTypeDef](./type_defs.md#restapistypedef) 


```python
# get_rest_apis method usage example with argument unpacking

kwargs: GetRestApisRequestRequestTypeDef = {  # (1)
    "position": ...,
}

parent.get_rest_apis(**kwargs)
```

1. See [:material-code-braces: GetRestApisRequestRequestTypeDef](./type_defs.md#getrestapisrequestrequesttypedef) 

### get\_sdk

Generates a client SDK for a RestApi and Stage.

Type annotations and code completion for `#!python session.create_client("apigateway").get_sdk` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_sdk)

```python
# get_sdk method definition

await def get_sdk(
    self,
    *,
    restApiId: str,
    stageName: str,
    sdkType: str,
    parameters: Mapping[str, str] = ...,
) -> SdkResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SdkResponseTypeDef](./type_defs.md#sdkresponsetypedef) 


```python
# get_sdk method usage example with argument unpacking

kwargs: GetSdkRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "stageName": ...,
    "sdkType": ...,
}

parent.get_sdk(**kwargs)
```

1. See [:material-code-braces: GetSdkRequestRequestTypeDef](./type_defs.md#getsdkrequestrequesttypedef) 

### get\_sdk\_type

Gets an SDK type.

Type annotations and code completion for `#!python session.create_client("apigateway").get_sdk_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_sdk_type)

```python
# get_sdk_type method definition

await def get_sdk_type(
    self,
    *,
    id: str,
) -> SdkTypeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SdkTypeResponseTypeDef](./type_defs.md#sdktyperesponsetypedef) 


```python
# get_sdk_type method usage example with argument unpacking

kwargs: GetSdkTypeRequestRequestTypeDef = {  # (1)
    "id": ...,
}

parent.get_sdk_type(**kwargs)
```

1. See [:material-code-braces: GetSdkTypeRequestRequestTypeDef](./type_defs.md#getsdktyperequestrequesttypedef) 

### get\_sdk\_types

Gets SDK types See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/apigateway-2015-07-09/GetSdkTypes).

Type annotations and code completion for `#!python session.create_client("apigateway").get_sdk_types` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_sdk_types)

```python
# get_sdk_types method definition

await def get_sdk_types(
    self,
    *,
    position: str = ...,
    limit: int = ...,
) -> SdkTypesTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SdkTypesTypeDef](./type_defs.md#sdktypestypedef) 


```python
# get_sdk_types method usage example with argument unpacking

kwargs: GetSdkTypesRequestRequestTypeDef = {  # (1)
    "position": ...,
}

parent.get_sdk_types(**kwargs)
```

1. See [:material-code-braces: GetSdkTypesRequestRequestTypeDef](./type_defs.md#getsdktypesrequestrequesttypedef) 

### get\_stage

Gets information about a Stage resource.

Type annotations and code completion for `#!python session.create_client("apigateway").get_stage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_stage)

```python
# get_stage method definition

await def get_stage(
    self,
    *,
    restApiId: str,
    stageName: str,
) -> StageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StageResponseTypeDef](./type_defs.md#stageresponsetypedef) 


```python
# get_stage method usage example with argument unpacking

kwargs: GetStageRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "stageName": ...,
}

parent.get_stage(**kwargs)
```

1. See [:material-code-braces: GetStageRequestRequestTypeDef](./type_defs.md#getstagerequestrequesttypedef) 

### get\_stages

Gets information about one or more Stage resources.

Type annotations and code completion for `#!python session.create_client("apigateway").get_stages` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_stages)

```python
# get_stages method definition

await def get_stages(
    self,
    *,
    restApiId: str,
    deploymentId: str = ...,
) -> StagesTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StagesTypeDef](./type_defs.md#stagestypedef) 


```python
# get_stages method usage example with argument unpacking

kwargs: GetStagesRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
}

parent.get_stages(**kwargs)
```

1. See [:material-code-braces: GetStagesRequestRequestTypeDef](./type_defs.md#getstagesrequestrequesttypedef) 

### get\_tags

Gets the Tags collection for a given resource.

Type annotations and code completion for `#!python session.create_client("apigateway").get_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_tags)

```python
# get_tags method definition

await def get_tags(
    self,
    *,
    resourceArn: str,
    position: str = ...,
    limit: int = ...,
) -> TagsTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: TagsTypeDef](./type_defs.md#tagstypedef) 


```python
# get_tags method usage example with argument unpacking

kwargs: GetTagsRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.get_tags(**kwargs)
```

1. See [:material-code-braces: GetTagsRequestRequestTypeDef](./type_defs.md#gettagsrequestrequesttypedef) 

### get\_usage

Gets the usage data of a usage plan in a specified time interval.

Type annotations and code completion for `#!python session.create_client("apigateway").get_usage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_usage)

```python
# get_usage method definition

await def get_usage(
    self,
    *,
    usagePlanId: str,
    startDate: str,
    endDate: str,
    keyId: str = ...,
    position: str = ...,
    limit: int = ...,
) -> UsageTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UsageTypeDef](./type_defs.md#usagetypedef) 


```python
# get_usage method usage example with argument unpacking

kwargs: GetUsageRequestRequestTypeDef = {  # (1)
    "usagePlanId": ...,
    "startDate": ...,
    "endDate": ...,
}

parent.get_usage(**kwargs)
```

1. See [:material-code-braces: GetUsageRequestRequestTypeDef](./type_defs.md#getusagerequestrequesttypedef) 

### get\_usage\_plan

Gets a usage plan of a given plan identifier.

Type annotations and code completion for `#!python session.create_client("apigateway").get_usage_plan` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_usage_plan)

```python
# get_usage_plan method definition

await def get_usage_plan(
    self,
    *,
    usagePlanId: str,
) -> UsagePlanResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UsagePlanResponseTypeDef](./type_defs.md#usageplanresponsetypedef) 


```python
# get_usage_plan method usage example with argument unpacking

kwargs: GetUsagePlanRequestRequestTypeDef = {  # (1)
    "usagePlanId": ...,
}

parent.get_usage_plan(**kwargs)
```

1. See [:material-code-braces: GetUsagePlanRequestRequestTypeDef](./type_defs.md#getusageplanrequestrequesttypedef) 

### get\_usage\_plan\_key

Gets a usage plan key of a given key identifier.

Type annotations and code completion for `#!python session.create_client("apigateway").get_usage_plan_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_usage_plan_key)

```python
# get_usage_plan_key method definition

await def get_usage_plan_key(
    self,
    *,
    usagePlanId: str,
    keyId: str,
) -> UsagePlanKeyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UsagePlanKeyResponseTypeDef](./type_defs.md#usageplankeyresponsetypedef) 


```python
# get_usage_plan_key method usage example with argument unpacking

kwargs: GetUsagePlanKeyRequestRequestTypeDef = {  # (1)
    "usagePlanId": ...,
    "keyId": ...,
}

parent.get_usage_plan_key(**kwargs)
```

1. See [:material-code-braces: GetUsagePlanKeyRequestRequestTypeDef](./type_defs.md#getusageplankeyrequestrequesttypedef) 

### get\_usage\_plan\_keys

Gets all the usage plan keys representing the API keys added to a specified
usage
plan.

Type annotations and code completion for `#!python session.create_client("apigateway").get_usage_plan_keys` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_usage_plan_keys)

```python
# get_usage_plan_keys method definition

await def get_usage_plan_keys(
    self,
    *,
    usagePlanId: str,
    position: str = ...,
    limit: int = ...,
    nameQuery: str = ...,
) -> UsagePlanKeysTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UsagePlanKeysTypeDef](./type_defs.md#usageplankeystypedef) 


```python
# get_usage_plan_keys method usage example with argument unpacking

kwargs: GetUsagePlanKeysRequestRequestTypeDef = {  # (1)
    "usagePlanId": ...,
}

parent.get_usage_plan_keys(**kwargs)
```

1. See [:material-code-braces: GetUsagePlanKeysRequestRequestTypeDef](./type_defs.md#getusageplankeysrequestrequesttypedef) 

### get\_usage\_plans

Gets all the usage plans of the caller's account.

Type annotations and code completion for `#!python session.create_client("apigateway").get_usage_plans` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_usage_plans)

```python
# get_usage_plans method definition

await def get_usage_plans(
    self,
    *,
    position: str = ...,
    keyId: str = ...,
    limit: int = ...,
) -> UsagePlansTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UsagePlansTypeDef](./type_defs.md#usageplanstypedef) 


```python
# get_usage_plans method usage example with argument unpacking

kwargs: GetUsagePlansRequestRequestTypeDef = {  # (1)
    "position": ...,
}

parent.get_usage_plans(**kwargs)
```

1. See [:material-code-braces: GetUsagePlansRequestRequestTypeDef](./type_defs.md#getusageplansrequestrequesttypedef) 

### get\_vpc\_link

Gets a specified VPC link under the caller's account in a region.

Type annotations and code completion for `#!python session.create_client("apigateway").get_vpc_link` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_vpc_link)

```python
# get_vpc_link method definition

await def get_vpc_link(
    self,
    *,
    vpcLinkId: str,
) -> VpcLinkResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: VpcLinkResponseTypeDef](./type_defs.md#vpclinkresponsetypedef) 


```python
# get_vpc_link method usage example with argument unpacking

kwargs: GetVpcLinkRequestRequestTypeDef = {  # (1)
    "vpcLinkId": ...,
}

parent.get_vpc_link(**kwargs)
```

1. See [:material-code-braces: GetVpcLinkRequestRequestTypeDef](./type_defs.md#getvpclinkrequestrequesttypedef) 

### get\_vpc\_links

Gets the VpcLinks collection under the caller's account in a selected region.

Type annotations and code completion for `#!python session.create_client("apigateway").get_vpc_links` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_vpc_links)

```python
# get_vpc_links method definition

await def get_vpc_links(
    self,
    *,
    position: str = ...,
    limit: int = ...,
) -> VpcLinksTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: VpcLinksTypeDef](./type_defs.md#vpclinkstypedef) 


```python
# get_vpc_links method usage example with argument unpacking

kwargs: GetVpcLinksRequestRequestTypeDef = {  # (1)
    "position": ...,
}

parent.get_vpc_links(**kwargs)
```

1. See [:material-code-braces: GetVpcLinksRequestRequestTypeDef](./type_defs.md#getvpclinksrequestrequesttypedef) 

### import\_api\_keys

Import API keys from an external source, such as a CSV-formatted file.

Type annotations and code completion for `#!python session.create_client("apigateway").import_api_keys` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.import_api_keys)

```python
# import_api_keys method definition

await def import_api_keys(
    self,
    *,
    body: BlobTypeDef,
    format: ApiKeysFormatType,  # (1)
    failOnWarnings: bool = ...,
) -> ApiKeyIdsTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ApiKeysFormatType](./literals.md#apikeysformattype) 
2. See [:material-code-braces: ApiKeyIdsTypeDef](./type_defs.md#apikeyidstypedef) 


```python
# import_api_keys method usage example with argument unpacking

kwargs: ImportApiKeysRequestRequestTypeDef = {  # (1)
    "body": ...,
    "format": ...,
}

parent.import_api_keys(**kwargs)
```

1. See [:material-code-braces: ImportApiKeysRequestRequestTypeDef](./type_defs.md#importapikeysrequestrequesttypedef) 

### import\_documentation\_parts

Imports documentation parts See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/apigateway-2015-07-09/ImportDocumentationParts).

Type annotations and code completion for `#!python session.create_client("apigateway").import_documentation_parts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.import_documentation_parts)

```python
# import_documentation_parts method definition

await def import_documentation_parts(
    self,
    *,
    restApiId: str,
    body: BlobTypeDef,
    mode: PutModeType = ...,  # (1)
    failOnWarnings: bool = ...,
) -> DocumentationPartIdsTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PutModeType](./literals.md#putmodetype) 
2. See [:material-code-braces: DocumentationPartIdsTypeDef](./type_defs.md#documentationpartidstypedef) 


```python
# import_documentation_parts method usage example with argument unpacking

kwargs: ImportDocumentationPartsRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "body": ...,
}

parent.import_documentation_parts(**kwargs)
```

1. See [:material-code-braces: ImportDocumentationPartsRequestRequestTypeDef](./type_defs.md#importdocumentationpartsrequestrequesttypedef) 

### import\_rest\_api

A feature of the API Gateway control service for creating a new API from an
external API definition
file.

Type annotations and code completion for `#!python session.create_client("apigateway").import_rest_api` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.import_rest_api)

```python
# import_rest_api method definition

await def import_rest_api(
    self,
    *,
    body: BlobTypeDef,
    failOnWarnings: bool = ...,
    parameters: Mapping[str, str] = ...,
) -> RestApiResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RestApiResponseTypeDef](./type_defs.md#restapiresponsetypedef) 


```python
# import_rest_api method usage example with argument unpacking

kwargs: ImportRestApiRequestRequestTypeDef = {  # (1)
    "body": ...,
}

parent.import_rest_api(**kwargs)
```

1. See [:material-code-braces: ImportRestApiRequestRequestTypeDef](./type_defs.md#importrestapirequestrequesttypedef) 

### put\_gateway\_response

Creates a customization of a GatewayResponse of a specified response type and
status code on the given
RestApi.

Type annotations and code completion for `#!python session.create_client("apigateway").put_gateway_response` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.put_gateway_response)

```python
# put_gateway_response method definition

await def put_gateway_response(
    self,
    *,
    restApiId: str,
    responseType: GatewayResponseTypeType,  # (1)
    statusCode: str = ...,
    responseParameters: Mapping[str, str] = ...,
    responseTemplates: Mapping[str, str] = ...,
) -> GatewayResponseResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: GatewayResponseTypeType](./literals.md#gatewayresponsetypetype) 
2. See [:material-code-braces: GatewayResponseResponseTypeDef](./type_defs.md#gatewayresponseresponsetypedef) 


```python
# put_gateway_response method usage example with argument unpacking

kwargs: PutGatewayResponseRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "responseType": ...,
}

parent.put_gateway_response(**kwargs)
```

1. See [:material-code-braces: PutGatewayResponseRequestRequestTypeDef](./type_defs.md#putgatewayresponserequestrequesttypedef) 

### put\_integration

Sets up a method's integration.

Type annotations and code completion for `#!python session.create_client("apigateway").put_integration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.put_integration)

```python
# put_integration method definition

await def put_integration(
    self,
    *,
    restApiId: str,
    resourceId: str,
    httpMethod: str,
    type: IntegrationTypeType,  # (1)
    integrationHttpMethod: str = ...,
    uri: str = ...,
    connectionType: ConnectionTypeType = ...,  # (2)
    connectionId: str = ...,
    credentials: str = ...,
    requestParameters: Mapping[str, str] = ...,
    requestTemplates: Mapping[str, str] = ...,
    passthroughBehavior: str = ...,
    cacheNamespace: str = ...,
    cacheKeyParameters: Sequence[str] = ...,
    contentHandling: ContentHandlingStrategyType = ...,  # (3)
    timeoutInMillis: int = ...,
    tlsConfig: TlsConfigTypeDef = ...,  # (4)
) -> IntegrationExtraResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: IntegrationTypeType](./literals.md#integrationtypetype) 
2. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
3. See [:material-code-brackets: ContentHandlingStrategyType](./literals.md#contenthandlingstrategytype) 
4. See [:material-code-braces: TlsConfigTypeDef](./type_defs.md#tlsconfigtypedef) 
5. See [:material-code-braces: IntegrationExtraResponseTypeDef](./type_defs.md#integrationextraresponsetypedef) 


```python
# put_integration method usage example with argument unpacking

kwargs: PutIntegrationRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "resourceId": ...,
    "httpMethod": ...,
    "type": ...,
}

parent.put_integration(**kwargs)
```

1. See [:material-code-braces: PutIntegrationRequestRequestTypeDef](./type_defs.md#putintegrationrequestrequesttypedef) 

### put\_integration\_response

Represents a put integration.

Type annotations and code completion for `#!python session.create_client("apigateway").put_integration_response` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.put_integration_response)

```python
# put_integration_response method definition

await def put_integration_response(
    self,
    *,
    restApiId: str,
    resourceId: str,
    httpMethod: str,
    statusCode: str,
    selectionPattern: str = ...,
    responseParameters: Mapping[str, str] = ...,
    responseTemplates: Mapping[str, str] = ...,
    contentHandling: ContentHandlingStrategyType = ...,  # (1)
) -> IntegrationResponseResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ContentHandlingStrategyType](./literals.md#contenthandlingstrategytype) 
2. See [:material-code-braces: IntegrationResponseResponseTypeDef](./type_defs.md#integrationresponseresponsetypedef) 


```python
# put_integration_response method usage example with argument unpacking

kwargs: PutIntegrationResponseRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "resourceId": ...,
    "httpMethod": ...,
    "statusCode": ...,
}

parent.put_integration_response(**kwargs)
```

1. See [:material-code-braces: PutIntegrationResponseRequestRequestTypeDef](./type_defs.md#putintegrationresponserequestrequesttypedef) 

### put\_method

Add a method to an existing Resource resource.

Type annotations and code completion for `#!python session.create_client("apigateway").put_method` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.put_method)

```python
# put_method method definition

await def put_method(
    self,
    *,
    restApiId: str,
    resourceId: str,
    httpMethod: str,
    authorizationType: str,
    authorizerId: str = ...,
    apiKeyRequired: bool = ...,
    operationName: str = ...,
    requestParameters: Mapping[str, bool] = ...,
    requestModels: Mapping[str, str] = ...,
    requestValidatorId: str = ...,
    authorizationScopes: Sequence[str] = ...,
) -> MethodExtraResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: MethodExtraResponseTypeDef](./type_defs.md#methodextraresponsetypedef) 


```python
# put_method method usage example with argument unpacking

kwargs: PutMethodRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "resourceId": ...,
    "httpMethod": ...,
    "authorizationType": ...,
}

parent.put_method(**kwargs)
```

1. See [:material-code-braces: PutMethodRequestRequestTypeDef](./type_defs.md#putmethodrequestrequesttypedef) 

### put\_method\_response

Adds a MethodResponse to an existing Method resource.

Type annotations and code completion for `#!python session.create_client("apigateway").put_method_response` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.put_method_response)

```python
# put_method_response method definition

await def put_method_response(
    self,
    *,
    restApiId: str,
    resourceId: str,
    httpMethod: str,
    statusCode: str,
    responseParameters: Mapping[str, bool] = ...,
    responseModels: Mapping[str, str] = ...,
) -> MethodResponseResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: MethodResponseResponseTypeDef](./type_defs.md#methodresponseresponsetypedef) 


```python
# put_method_response method usage example with argument unpacking

kwargs: PutMethodResponseRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "resourceId": ...,
    "httpMethod": ...,
    "statusCode": ...,
}

parent.put_method_response(**kwargs)
```

1. See [:material-code-braces: PutMethodResponseRequestRequestTypeDef](./type_defs.md#putmethodresponserequestrequesttypedef) 

### put\_rest\_api

A feature of the API Gateway control service for updating an existing API with
an input of external API
definitions.

Type annotations and code completion for `#!python session.create_client("apigateway").put_rest_api` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.put_rest_api)

```python
# put_rest_api method definition

await def put_rest_api(
    self,
    *,
    restApiId: str,
    body: BlobTypeDef,
    mode: PutModeType = ...,  # (1)
    failOnWarnings: bool = ...,
    parameters: Mapping[str, str] = ...,
) -> RestApiResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PutModeType](./literals.md#putmodetype) 
2. See [:material-code-braces: RestApiResponseTypeDef](./type_defs.md#restapiresponsetypedef) 


```python
# put_rest_api method usage example with argument unpacking

kwargs: PutRestApiRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "body": ...,
}

parent.put_rest_api(**kwargs)
```

1. See [:material-code-braces: PutRestApiRequestRequestTypeDef](./type_defs.md#putrestapirequestrequesttypedef) 

### tag\_resource

Adds or updates a tag on a given resource.

Type annotations and code completion for `#!python session.create_client("apigateway").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### test\_invoke\_authorizer

Simulate the execution of an Authorizer in your RestApi with headers,
parameters, and an incoming request
body.

Type annotations and code completion for `#!python session.create_client("apigateway").test_invoke_authorizer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.test_invoke_authorizer)

```python
# test_invoke_authorizer method definition

await def test_invoke_authorizer(
    self,
    *,
    restApiId: str,
    authorizerId: str,
    headers: Mapping[str, str] = ...,
    multiValueHeaders: Mapping[str, Sequence[str]] = ...,
    pathWithQueryString: str = ...,
    body: str = ...,
    stageVariables: Mapping[str, str] = ...,
    additionalContext: Mapping[str, str] = ...,
) -> TestInvokeAuthorizerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: TestInvokeAuthorizerResponseTypeDef](./type_defs.md#testinvokeauthorizerresponsetypedef) 


```python
# test_invoke_authorizer method usage example with argument unpacking

kwargs: TestInvokeAuthorizerRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "authorizerId": ...,
}

parent.test_invoke_authorizer(**kwargs)
```

1. See [:material-code-braces: TestInvokeAuthorizerRequestRequestTypeDef](./type_defs.md#testinvokeauthorizerrequestrequesttypedef) 

### test\_invoke\_method

Simulate the invocation of a Method in your RestApi with headers, parameters,
and an incoming request
body.

Type annotations and code completion for `#!python session.create_client("apigateway").test_invoke_method` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.test_invoke_method)

```python
# test_invoke_method method definition

await def test_invoke_method(
    self,
    *,
    restApiId: str,
    resourceId: str,
    httpMethod: str,
    pathWithQueryString: str = ...,
    body: str = ...,
    headers: Mapping[str, str] = ...,
    multiValueHeaders: Mapping[str, Sequence[str]] = ...,
    clientCertificateId: str = ...,
    stageVariables: Mapping[str, str] = ...,
) -> TestInvokeMethodResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: TestInvokeMethodResponseTypeDef](./type_defs.md#testinvokemethodresponsetypedef) 


```python
# test_invoke_method method usage example with argument unpacking

kwargs: TestInvokeMethodRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "resourceId": ...,
    "httpMethod": ...,
}

parent.test_invoke_method(**kwargs)
```

1. See [:material-code-braces: TestInvokeMethodRequestRequestTypeDef](./type_defs.md#testinvokemethodrequestrequesttypedef) 

### untag\_resource

Removes a tag from a given resource.

Type annotations and code completion for `#!python session.create_client("apigateway").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_account

Changes information about the current Account resource.

Type annotations and code completion for `#!python session.create_client("apigateway").update_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_account)

```python
# update_account method definition

await def update_account(
    self,
    *,
    patchOperations: Sequence[PatchOperationTypeDef] = ...,  # (1)
) -> AccountTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
2. See [:material-code-braces: AccountTypeDef](./type_defs.md#accounttypedef) 


```python
# update_account method usage example with argument unpacking

kwargs: UpdateAccountRequestRequestTypeDef = {  # (1)
    "patchOperations": ...,
}

parent.update_account(**kwargs)
```

1. See [:material-code-braces: UpdateAccountRequestRequestTypeDef](./type_defs.md#updateaccountrequestrequesttypedef) 

### update\_api\_key

Changes information about an ApiKey resource.

Type annotations and code completion for `#!python session.create_client("apigateway").update_api_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_api_key)

```python
# update_api_key method definition

await def update_api_key(
    self,
    *,
    apiKey: str,
    patchOperations: Sequence[PatchOperationTypeDef] = ...,  # (1)
) -> ApiKeyResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
2. See [:material-code-braces: ApiKeyResponseTypeDef](./type_defs.md#apikeyresponsetypedef) 


```python
# update_api_key method usage example with argument unpacking

kwargs: UpdateApiKeyRequestRequestTypeDef = {  # (1)
    "apiKey": ...,
}

parent.update_api_key(**kwargs)
```

1. See [:material-code-braces: UpdateApiKeyRequestRequestTypeDef](./type_defs.md#updateapikeyrequestrequesttypedef) 

### update\_authorizer

Updates an existing Authorizer resource.

Type annotations and code completion for `#!python session.create_client("apigateway").update_authorizer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_authorizer)

```python
# update_authorizer method definition

await def update_authorizer(
    self,
    *,
    restApiId: str,
    authorizerId: str,
    patchOperations: Sequence[PatchOperationTypeDef] = ...,  # (1)
) -> AuthorizerResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
2. See [:material-code-braces: AuthorizerResponseTypeDef](./type_defs.md#authorizerresponsetypedef) 


```python
# update_authorizer method usage example with argument unpacking

kwargs: UpdateAuthorizerRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "authorizerId": ...,
}

parent.update_authorizer(**kwargs)
```

1. See [:material-code-braces: UpdateAuthorizerRequestRequestTypeDef](./type_defs.md#updateauthorizerrequestrequesttypedef) 

### update\_base\_path\_mapping

Changes information about the BasePathMapping resource.

Type annotations and code completion for `#!python session.create_client("apigateway").update_base_path_mapping` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_base_path_mapping)

```python
# update_base_path_mapping method definition

await def update_base_path_mapping(
    self,
    *,
    domainName: str,
    basePath: str,
    patchOperations: Sequence[PatchOperationTypeDef] = ...,  # (1)
) -> BasePathMappingResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
2. See [:material-code-braces: BasePathMappingResponseTypeDef](./type_defs.md#basepathmappingresponsetypedef) 


```python
# update_base_path_mapping method usage example with argument unpacking

kwargs: UpdateBasePathMappingRequestRequestTypeDef = {  # (1)
    "domainName": ...,
    "basePath": ...,
}

parent.update_base_path_mapping(**kwargs)
```

1. See [:material-code-braces: UpdateBasePathMappingRequestRequestTypeDef](./type_defs.md#updatebasepathmappingrequestrequesttypedef) 

### update\_client\_certificate

Changes information about an ClientCertificate resource.

Type annotations and code completion for `#!python session.create_client("apigateway").update_client_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_client_certificate)

```python
# update_client_certificate method definition

await def update_client_certificate(
    self,
    *,
    clientCertificateId: str,
    patchOperations: Sequence[PatchOperationTypeDef] = ...,  # (1)
) -> ClientCertificateResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
2. See [:material-code-braces: ClientCertificateResponseTypeDef](./type_defs.md#clientcertificateresponsetypedef) 


```python
# update_client_certificate method usage example with argument unpacking

kwargs: UpdateClientCertificateRequestRequestTypeDef = {  # (1)
    "clientCertificateId": ...,
}

parent.update_client_certificate(**kwargs)
```

1. See [:material-code-braces: UpdateClientCertificateRequestRequestTypeDef](./type_defs.md#updateclientcertificaterequestrequesttypedef) 

### update\_deployment

Changes information about a Deployment resource.

Type annotations and code completion for `#!python session.create_client("apigateway").update_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_deployment)

```python
# update_deployment method definition

await def update_deployment(
    self,
    *,
    restApiId: str,
    deploymentId: str,
    patchOperations: Sequence[PatchOperationTypeDef] = ...,  # (1)
) -> DeploymentResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
2. See [:material-code-braces: DeploymentResponseTypeDef](./type_defs.md#deploymentresponsetypedef) 


```python
# update_deployment method usage example with argument unpacking

kwargs: UpdateDeploymentRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "deploymentId": ...,
}

parent.update_deployment(**kwargs)
```

1. See [:material-code-braces: UpdateDeploymentRequestRequestTypeDef](./type_defs.md#updatedeploymentrequestrequesttypedef) 

### update\_documentation\_part

Updates a documentation part.

Type annotations and code completion for `#!python session.create_client("apigateway").update_documentation_part` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_documentation_part)

```python
# update_documentation_part method definition

await def update_documentation_part(
    self,
    *,
    restApiId: str,
    documentationPartId: str,
    patchOperations: Sequence[PatchOperationTypeDef] = ...,  # (1)
) -> DocumentationPartResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
2. See [:material-code-braces: DocumentationPartResponseTypeDef](./type_defs.md#documentationpartresponsetypedef) 


```python
# update_documentation_part method usage example with argument unpacking

kwargs: UpdateDocumentationPartRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "documentationPartId": ...,
}

parent.update_documentation_part(**kwargs)
```

1. See [:material-code-braces: UpdateDocumentationPartRequestRequestTypeDef](./type_defs.md#updatedocumentationpartrequestrequesttypedef) 

### update\_documentation\_version

Updates a documentation version.

Type annotations and code completion for `#!python session.create_client("apigateway").update_documentation_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_documentation_version)

```python
# update_documentation_version method definition

await def update_documentation_version(
    self,
    *,
    restApiId: str,
    documentationVersion: str,
    patchOperations: Sequence[PatchOperationTypeDef] = ...,  # (1)
) -> DocumentationVersionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
2. See [:material-code-braces: DocumentationVersionResponseTypeDef](./type_defs.md#documentationversionresponsetypedef) 


```python
# update_documentation_version method usage example with argument unpacking

kwargs: UpdateDocumentationVersionRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "documentationVersion": ...,
}

parent.update_documentation_version(**kwargs)
```

1. See [:material-code-braces: UpdateDocumentationVersionRequestRequestTypeDef](./type_defs.md#updatedocumentationversionrequestrequesttypedef) 

### update\_domain\_name

Changes information about the DomainName resource.

Type annotations and code completion for `#!python session.create_client("apigateway").update_domain_name` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_domain_name)

```python
# update_domain_name method definition

await def update_domain_name(
    self,
    *,
    domainName: str,
    patchOperations: Sequence[PatchOperationTypeDef] = ...,  # (1)
) -> DomainNameResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
2. See [:material-code-braces: DomainNameResponseTypeDef](./type_defs.md#domainnameresponsetypedef) 


```python
# update_domain_name method usage example with argument unpacking

kwargs: UpdateDomainNameRequestRequestTypeDef = {  # (1)
    "domainName": ...,
}

parent.update_domain_name(**kwargs)
```

1. See [:material-code-braces: UpdateDomainNameRequestRequestTypeDef](./type_defs.md#updatedomainnamerequestrequesttypedef) 

### update\_gateway\_response

Updates a GatewayResponse of a specified response type on the given RestApi.

Type annotations and code completion for `#!python session.create_client("apigateway").update_gateway_response` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_gateway_response)

```python
# update_gateway_response method definition

await def update_gateway_response(
    self,
    *,
    restApiId: str,
    responseType: GatewayResponseTypeType,  # (1)
    patchOperations: Sequence[PatchOperationTypeDef] = ...,  # (2)
) -> GatewayResponseResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: GatewayResponseTypeType](./literals.md#gatewayresponsetypetype) 
2. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
3. See [:material-code-braces: GatewayResponseResponseTypeDef](./type_defs.md#gatewayresponseresponsetypedef) 


```python
# update_gateway_response method usage example with argument unpacking

kwargs: UpdateGatewayResponseRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "responseType": ...,
}

parent.update_gateway_response(**kwargs)
```

1. See [:material-code-braces: UpdateGatewayResponseRequestRequestTypeDef](./type_defs.md#updategatewayresponserequestrequesttypedef) 

### update\_integration

Represents an update integration.

Type annotations and code completion for `#!python session.create_client("apigateway").update_integration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_integration)

```python
# update_integration method definition

await def update_integration(
    self,
    *,
    restApiId: str,
    resourceId: str,
    httpMethod: str,
    patchOperations: Sequence[PatchOperationTypeDef] = ...,  # (1)
) -> IntegrationExtraResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
2. See [:material-code-braces: IntegrationExtraResponseTypeDef](./type_defs.md#integrationextraresponsetypedef) 


```python
# update_integration method usage example with argument unpacking

kwargs: UpdateIntegrationRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "resourceId": ...,
    "httpMethod": ...,
}

parent.update_integration(**kwargs)
```

1. See [:material-code-braces: UpdateIntegrationRequestRequestTypeDef](./type_defs.md#updateintegrationrequestrequesttypedef) 

### update\_integration\_response

Represents an update integration response.

Type annotations and code completion for `#!python session.create_client("apigateway").update_integration_response` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_integration_response)

```python
# update_integration_response method definition

await def update_integration_response(
    self,
    *,
    restApiId: str,
    resourceId: str,
    httpMethod: str,
    statusCode: str,
    patchOperations: Sequence[PatchOperationTypeDef] = ...,  # (1)
) -> IntegrationResponseResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
2. See [:material-code-braces: IntegrationResponseResponseTypeDef](./type_defs.md#integrationresponseresponsetypedef) 


```python
# update_integration_response method usage example with argument unpacking

kwargs: UpdateIntegrationResponseRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "resourceId": ...,
    "httpMethod": ...,
    "statusCode": ...,
}

parent.update_integration_response(**kwargs)
```

1. See [:material-code-braces: UpdateIntegrationResponseRequestRequestTypeDef](./type_defs.md#updateintegrationresponserequestrequesttypedef) 

### update\_method

Updates an existing Method resource.

Type annotations and code completion for `#!python session.create_client("apigateway").update_method` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_method)

```python
# update_method method definition

await def update_method(
    self,
    *,
    restApiId: str,
    resourceId: str,
    httpMethod: str,
    patchOperations: Sequence[PatchOperationTypeDef] = ...,  # (1)
) -> MethodExtraResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
2. See [:material-code-braces: MethodExtraResponseTypeDef](./type_defs.md#methodextraresponsetypedef) 


```python
# update_method method usage example with argument unpacking

kwargs: UpdateMethodRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "resourceId": ...,
    "httpMethod": ...,
}

parent.update_method(**kwargs)
```

1. See [:material-code-braces: UpdateMethodRequestRequestTypeDef](./type_defs.md#updatemethodrequestrequesttypedef) 

### update\_method\_response

Updates an existing MethodResponse resource.

Type annotations and code completion for `#!python session.create_client("apigateway").update_method_response` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_method_response)

```python
# update_method_response method definition

await def update_method_response(
    self,
    *,
    restApiId: str,
    resourceId: str,
    httpMethod: str,
    statusCode: str,
    patchOperations: Sequence[PatchOperationTypeDef] = ...,  # (1)
) -> MethodResponseResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
2. See [:material-code-braces: MethodResponseResponseTypeDef](./type_defs.md#methodresponseresponsetypedef) 


```python
# update_method_response method usage example with argument unpacking

kwargs: UpdateMethodResponseRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "resourceId": ...,
    "httpMethod": ...,
    "statusCode": ...,
}

parent.update_method_response(**kwargs)
```

1. See [:material-code-braces: UpdateMethodResponseRequestRequestTypeDef](./type_defs.md#updatemethodresponserequestrequesttypedef) 

### update\_model

Changes information about a model.

Type annotations and code completion for `#!python session.create_client("apigateway").update_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_model)

```python
# update_model method definition

await def update_model(
    self,
    *,
    restApiId: str,
    modelName: str,
    patchOperations: Sequence[PatchOperationTypeDef] = ...,  # (1)
) -> ModelResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
2. See [:material-code-braces: ModelResponseTypeDef](./type_defs.md#modelresponsetypedef) 


```python
# update_model method usage example with argument unpacking

kwargs: UpdateModelRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "modelName": ...,
}

parent.update_model(**kwargs)
```

1. See [:material-code-braces: UpdateModelRequestRequestTypeDef](./type_defs.md#updatemodelrequestrequesttypedef) 

### update\_request\_validator

Updates a RequestValidator of a given RestApi.

Type annotations and code completion for `#!python session.create_client("apigateway").update_request_validator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_request_validator)

```python
# update_request_validator method definition

await def update_request_validator(
    self,
    *,
    restApiId: str,
    requestValidatorId: str,
    patchOperations: Sequence[PatchOperationTypeDef] = ...,  # (1)
) -> RequestValidatorResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
2. See [:material-code-braces: RequestValidatorResponseTypeDef](./type_defs.md#requestvalidatorresponsetypedef) 


```python
# update_request_validator method usage example with argument unpacking

kwargs: UpdateRequestValidatorRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "requestValidatorId": ...,
}

parent.update_request_validator(**kwargs)
```

1. See [:material-code-braces: UpdateRequestValidatorRequestRequestTypeDef](./type_defs.md#updaterequestvalidatorrequestrequesttypedef) 

### update\_resource

Changes information about a Resource resource.

Type annotations and code completion for `#!python session.create_client("apigateway").update_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_resource)

```python
# update_resource method definition

await def update_resource(
    self,
    *,
    restApiId: str,
    resourceId: str,
    patchOperations: Sequence[PatchOperationTypeDef] = ...,  # (1)
) -> ResourceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
2. See [:material-code-braces: ResourceResponseTypeDef](./type_defs.md#resourceresponsetypedef) 


```python
# update_resource method usage example with argument unpacking

kwargs: UpdateResourceRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "resourceId": ...,
}

parent.update_resource(**kwargs)
```

1. See [:material-code-braces: UpdateResourceRequestRequestTypeDef](./type_defs.md#updateresourcerequestrequesttypedef) 

### update\_rest\_api

Changes information about the specified API.

Type annotations and code completion for `#!python session.create_client("apigateway").update_rest_api` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_rest_api)

```python
# update_rest_api method definition

await def update_rest_api(
    self,
    *,
    restApiId: str,
    patchOperations: Sequence[PatchOperationTypeDef] = ...,  # (1)
) -> RestApiResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
2. See [:material-code-braces: RestApiResponseTypeDef](./type_defs.md#restapiresponsetypedef) 


```python
# update_rest_api method usage example with argument unpacking

kwargs: UpdateRestApiRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
}

parent.update_rest_api(**kwargs)
```

1. See [:material-code-braces: UpdateRestApiRequestRequestTypeDef](./type_defs.md#updaterestapirequestrequesttypedef) 

### update\_stage

Changes information about a Stage resource.

Type annotations and code completion for `#!python session.create_client("apigateway").update_stage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_stage)

```python
# update_stage method definition

await def update_stage(
    self,
    *,
    restApiId: str,
    stageName: str,
    patchOperations: Sequence[PatchOperationTypeDef] = ...,  # (1)
) -> StageResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
2. See [:material-code-braces: StageResponseTypeDef](./type_defs.md#stageresponsetypedef) 


```python
# update_stage method usage example with argument unpacking

kwargs: UpdateStageRequestRequestTypeDef = {  # (1)
    "restApiId": ...,
    "stageName": ...,
}

parent.update_stage(**kwargs)
```

1. See [:material-code-braces: UpdateStageRequestRequestTypeDef](./type_defs.md#updatestagerequestrequesttypedef) 

### update\_usage

Grants a temporary extension to the remaining quota of a usage plan associated
with a specified API
key.

Type annotations and code completion for `#!python session.create_client("apigateway").update_usage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_usage)

```python
# update_usage method definition

await def update_usage(
    self,
    *,
    usagePlanId: str,
    keyId: str,
    patchOperations: Sequence[PatchOperationTypeDef] = ...,  # (1)
) -> UsageTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
2. See [:material-code-braces: UsageTypeDef](./type_defs.md#usagetypedef) 


```python
# update_usage method usage example with argument unpacking

kwargs: UpdateUsageRequestRequestTypeDef = {  # (1)
    "usagePlanId": ...,
    "keyId": ...,
}

parent.update_usage(**kwargs)
```

1. See [:material-code-braces: UpdateUsageRequestRequestTypeDef](./type_defs.md#updateusagerequestrequesttypedef) 

### update\_usage\_plan

Updates a usage plan of a given plan Id.

Type annotations and code completion for `#!python session.create_client("apigateway").update_usage_plan` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_usage_plan)

```python
# update_usage_plan method definition

await def update_usage_plan(
    self,
    *,
    usagePlanId: str,
    patchOperations: Sequence[PatchOperationTypeDef] = ...,  # (1)
) -> UsagePlanResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
2. See [:material-code-braces: UsagePlanResponseTypeDef](./type_defs.md#usageplanresponsetypedef) 


```python
# update_usage_plan method usage example with argument unpacking

kwargs: UpdateUsagePlanRequestRequestTypeDef = {  # (1)
    "usagePlanId": ...,
}

parent.update_usage_plan(**kwargs)
```

1. See [:material-code-braces: UpdateUsagePlanRequestRequestTypeDef](./type_defs.md#updateusageplanrequestrequesttypedef) 

### update\_vpc\_link

Updates an existing VpcLink of a specified identifier.

Type annotations and code completion for `#!python session.create_client("apigateway").update_vpc_link` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_vpc_link)

```python
# update_vpc_link method definition

await def update_vpc_link(
    self,
    *,
    vpcLinkId: str,
    patchOperations: Sequence[PatchOperationTypeDef] = ...,  # (1)
) -> VpcLinkResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
2. See [:material-code-braces: VpcLinkResponseTypeDef](./type_defs.md#vpclinkresponsetypedef) 


```python
# update_vpc_link method usage example with argument unpacking

kwargs: UpdateVpcLinkRequestRequestTypeDef = {  # (1)
    "vpcLinkId": ...,
}

parent.update_vpc_link(**kwargs)
```

1. See [:material-code-braces: UpdateVpcLinkRequestRequestTypeDef](./type_defs.md#updatevpclinkrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("apigateway").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "APIGatewayClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("apigateway").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.__aexit__)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("apigateway").get_paginator` method with overloads.

- `client.get_paginator("get_api_keys")` -> [GetApiKeysPaginator](./paginators.md#getapikeyspaginator)
- `client.get_paginator("get_authorizers")` -> [GetAuthorizersPaginator](./paginators.md#getauthorizerspaginator)
- `client.get_paginator("get_base_path_mappings")` -> [GetBasePathMappingsPaginator](./paginators.md#getbasepathmappingspaginator)
- `client.get_paginator("get_client_certificates")` -> [GetClientCertificatesPaginator](./paginators.md#getclientcertificatespaginator)
- `client.get_paginator("get_deployments")` -> [GetDeploymentsPaginator](./paginators.md#getdeploymentspaginator)
- `client.get_paginator("get_documentation_parts")` -> [GetDocumentationPartsPaginator](./paginators.md#getdocumentationpartspaginator)
- `client.get_paginator("get_documentation_versions")` -> [GetDocumentationVersionsPaginator](./paginators.md#getdocumentationversionspaginator)
- `client.get_paginator("get_domain_names")` -> [GetDomainNamesPaginator](./paginators.md#getdomainnamespaginator)
- `client.get_paginator("get_gateway_responses")` -> [GetGatewayResponsesPaginator](./paginators.md#getgatewayresponsespaginator)
- `client.get_paginator("get_models")` -> [GetModelsPaginator](./paginators.md#getmodelspaginator)
- `client.get_paginator("get_request_validators")` -> [GetRequestValidatorsPaginator](./paginators.md#getrequestvalidatorspaginator)
- `client.get_paginator("get_resources")` -> [GetResourcesPaginator](./paginators.md#getresourcespaginator)
- `client.get_paginator("get_rest_apis")` -> [GetRestApisPaginator](./paginators.md#getrestapispaginator)
- `client.get_paginator("get_sdk_types")` -> [GetSdkTypesPaginator](./paginators.md#getsdktypespaginator)
- `client.get_paginator("get_usage")` -> [GetUsagePaginator](./paginators.md#getusagepaginator)
- `client.get_paginator("get_usage_plan_keys")` -> [GetUsagePlanKeysPaginator](./paginators.md#getusageplankeyspaginator)
- `client.get_paginator("get_usage_plans")` -> [GetUsagePlansPaginator](./paginators.md#getusageplanspaginator)
- `client.get_paginator("get_vpc_links")` -> [GetVpcLinksPaginator](./paginators.md#getvpclinkspaginator)



