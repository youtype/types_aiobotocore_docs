# Type definitions

> [Index](../README.md) > [APIGateway](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [APIGateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway)
    type annotations stubs module [types-aiobotocore-apigateway](https://pypi.org/project/types-aiobotocore-apigateway/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```


## ApiStageUnionTypeDef

```python
# ApiStageUnionTypeDef definition

ApiStageUnionTypeDef = Union[
    ApiStageTypeDef,  # (1)
    ApiStageOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ApiStageTypeDef](./type_defs.md#apistagetypedef) 
2. See [:material-code-braces: ApiStageOutputTypeDef](./type_defs.md#apistageoutputtypedef) 



## AccessLogSettingsTypeDef

```python
# AccessLogSettingsTypeDef definition

class AccessLogSettingsTypeDef(TypedDict):
    format: NotRequired[str],
    destinationArn: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## ThrottleSettingsTypeDef

```python
# ThrottleSettingsTypeDef definition

class ThrottleSettingsTypeDef(TypedDict):
    burstLimit: NotRequired[int],
    rateLimit: NotRequired[float],
```

## ApiKeyTypeDef

```python
# ApiKeyTypeDef definition

class ApiKeyTypeDef(TypedDict):
    id: NotRequired[str],
    value: NotRequired[str],
    name: NotRequired[str],
    customerId: NotRequired[str],
    description: NotRequired[str],
    enabled: NotRequired[bool],
    createdDate: NotRequired[datetime],
    lastUpdatedDate: NotRequired[datetime],
    stageKeys: NotRequired[List[str]],
    tags: NotRequired[Dict[str, str]],
```

## AuthorizerTypeDef

```python
# AuthorizerTypeDef definition

class AuthorizerTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    type: NotRequired[AuthorizerTypeType],  # (1)
    providerARNs: NotRequired[List[str]],
    authType: NotRequired[str],
    authorizerUri: NotRequired[str],
    authorizerCredentials: NotRequired[str],
    identitySource: NotRequired[str],
    identityValidationExpression: NotRequired[str],
    authorizerResultTtlInSeconds: NotRequired[int],
```

1. See [:material-code-brackets: AuthorizerTypeType](./literals.md#authorizertypetype) 
## BasePathMappingTypeDef

```python
# BasePathMappingTypeDef definition

class BasePathMappingTypeDef(TypedDict):
    basePath: NotRequired[str],
    restApiId: NotRequired[str],
    stage: NotRequired[str],
```

## CanarySettingsOutputTypeDef

```python
# CanarySettingsOutputTypeDef definition

class CanarySettingsOutputTypeDef(TypedDict):
    percentTraffic: NotRequired[float],
    deploymentId: NotRequired[str],
    stageVariableOverrides: NotRequired[Dict[str, str]],
    useStageCache: NotRequired[bool],
```

## CanarySettingsTypeDef

```python
# CanarySettingsTypeDef definition

class CanarySettingsTypeDef(TypedDict):
    percentTraffic: NotRequired[float],
    deploymentId: NotRequired[str],
    stageVariableOverrides: NotRequired[Mapping[str, str]],
    useStageCache: NotRequired[bool],
```

## ClientCertificateTypeDef

```python
# ClientCertificateTypeDef definition

class ClientCertificateTypeDef(TypedDict):
    clientCertificateId: NotRequired[str],
    description: NotRequired[str],
    pemEncodedCertificate: NotRequired[str],
    createdDate: NotRequired[datetime],
    expirationDate: NotRequired[datetime],
    tags: NotRequired[Dict[str, str]],
```

## StageKeyTypeDef

```python
# StageKeyTypeDef definition

class StageKeyTypeDef(TypedDict):
    restApiId: NotRequired[str],
    stageName: NotRequired[str],
```

## CreateAuthorizerRequestRequestTypeDef

```python
# CreateAuthorizerRequestRequestTypeDef definition

class CreateAuthorizerRequestRequestTypeDef(TypedDict):
    restApiId: str,
    name: str,
    type: AuthorizerTypeType,  # (1)
    providerARNs: NotRequired[Sequence[str]],
    authType: NotRequired[str],
    authorizerUri: NotRequired[str],
    authorizerCredentials: NotRequired[str],
    identitySource: NotRequired[str],
    identityValidationExpression: NotRequired[str],
    authorizerResultTtlInSeconds: NotRequired[int],
```

1. See [:material-code-brackets: AuthorizerTypeType](./literals.md#authorizertypetype) 
## CreateBasePathMappingRequestRequestTypeDef

```python
# CreateBasePathMappingRequestRequestTypeDef definition

class CreateBasePathMappingRequestRequestTypeDef(TypedDict):
    domainName: str,
    restApiId: str,
    basePath: NotRequired[str],
    stage: NotRequired[str],
```

## DeploymentCanarySettingsTypeDef

```python
# DeploymentCanarySettingsTypeDef definition

class DeploymentCanarySettingsTypeDef(TypedDict):
    percentTraffic: NotRequired[float],
    stageVariableOverrides: NotRequired[Mapping[str, str]],
    useStageCache: NotRequired[bool],
```

## DocumentationPartLocationTypeDef

```python
# DocumentationPartLocationTypeDef definition

class DocumentationPartLocationTypeDef(TypedDict):
    type: DocumentationPartTypeType,  # (1)
    path: NotRequired[str],
    method: NotRequired[str],
    statusCode: NotRequired[str],
    name: NotRequired[str],
```

1. See [:material-code-brackets: DocumentationPartTypeType](./literals.md#documentationparttypetype) 
## CreateDocumentationVersionRequestRequestTypeDef

```python
# CreateDocumentationVersionRequestRequestTypeDef definition

class CreateDocumentationVersionRequestRequestTypeDef(TypedDict):
    restApiId: str,
    documentationVersion: str,
    stageName: NotRequired[str],
    description: NotRequired[str],
```

## EndpointConfigurationTypeDef

```python
# EndpointConfigurationTypeDef definition

class EndpointConfigurationTypeDef(TypedDict):
    types: NotRequired[Sequence[EndpointTypeType]],  # (1)
    vpcEndpointIds: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: EndpointTypeType](./literals.md#endpointtypetype) 
## MutualTlsAuthenticationInputTypeDef

```python
# MutualTlsAuthenticationInputTypeDef definition

class MutualTlsAuthenticationInputTypeDef(TypedDict):
    truststoreUri: NotRequired[str],
    truststoreVersion: NotRequired[str],
```

## CreateModelRequestRequestTypeDef

```python
# CreateModelRequestRequestTypeDef definition

class CreateModelRequestRequestTypeDef(TypedDict):
    restApiId: str,
    name: str,
    contentType: str,
    description: NotRequired[str],
    schema: NotRequired[str],
```

## CreateRequestValidatorRequestRequestTypeDef

```python
# CreateRequestValidatorRequestRequestTypeDef definition

class CreateRequestValidatorRequestRequestTypeDef(TypedDict):
    restApiId: str,
    name: NotRequired[str],
    validateRequestBody: NotRequired[bool],
    validateRequestParameters: NotRequired[bool],
```

## CreateResourceRequestRequestTypeDef

```python
# CreateResourceRequestRequestTypeDef definition

class CreateResourceRequestRequestTypeDef(TypedDict):
    restApiId: str,
    parentId: str,
    pathPart: str,
```

## CreateUsagePlanKeyRequestRequestTypeDef

```python
# CreateUsagePlanKeyRequestRequestTypeDef definition

class CreateUsagePlanKeyRequestRequestTypeDef(TypedDict):
    usagePlanId: str,
    keyId: str,
    keyType: str,
```

## QuotaSettingsTypeDef

```python
# QuotaSettingsTypeDef definition

class QuotaSettingsTypeDef(TypedDict):
    limit: NotRequired[int],
    offset: NotRequired[int],
    period: NotRequired[QuotaPeriodTypeType],  # (1)
```

1. See [:material-code-brackets: QuotaPeriodTypeType](./literals.md#quotaperiodtypetype) 
## CreateVpcLinkRequestRequestTypeDef

```python
# CreateVpcLinkRequestRequestTypeDef definition

class CreateVpcLinkRequestRequestTypeDef(TypedDict):
    name: str,
    targetArns: Sequence[str],
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## DeleteApiKeyRequestRequestTypeDef

```python
# DeleteApiKeyRequestRequestTypeDef definition

class DeleteApiKeyRequestRequestTypeDef(TypedDict):
    apiKey: str,
```

## DeleteAuthorizerRequestRequestTypeDef

```python
# DeleteAuthorizerRequestRequestTypeDef definition

class DeleteAuthorizerRequestRequestTypeDef(TypedDict):
    restApiId: str,
    authorizerId: str,
```

## DeleteBasePathMappingRequestRequestTypeDef

```python
# DeleteBasePathMappingRequestRequestTypeDef definition

class DeleteBasePathMappingRequestRequestTypeDef(TypedDict):
    domainName: str,
    basePath: str,
```

## DeleteClientCertificateRequestRequestTypeDef

```python
# DeleteClientCertificateRequestRequestTypeDef definition

class DeleteClientCertificateRequestRequestTypeDef(TypedDict):
    clientCertificateId: str,
```

## DeleteDeploymentRequestRequestTypeDef

```python
# DeleteDeploymentRequestRequestTypeDef definition

class DeleteDeploymentRequestRequestTypeDef(TypedDict):
    restApiId: str,
    deploymentId: str,
```

## DeleteDocumentationPartRequestRequestTypeDef

```python
# DeleteDocumentationPartRequestRequestTypeDef definition

class DeleteDocumentationPartRequestRequestTypeDef(TypedDict):
    restApiId: str,
    documentationPartId: str,
```

## DeleteDocumentationVersionRequestRequestTypeDef

```python
# DeleteDocumentationVersionRequestRequestTypeDef definition

class DeleteDocumentationVersionRequestRequestTypeDef(TypedDict):
    restApiId: str,
    documentationVersion: str,
```

## DeleteDomainNameRequestRequestTypeDef

```python
# DeleteDomainNameRequestRequestTypeDef definition

class DeleteDomainNameRequestRequestTypeDef(TypedDict):
    domainName: str,
```

## DeleteGatewayResponseRequestRequestTypeDef

```python
# DeleteGatewayResponseRequestRequestTypeDef definition

class DeleteGatewayResponseRequestRequestTypeDef(TypedDict):
    restApiId: str,
    responseType: GatewayResponseTypeType,  # (1)
```

1. See [:material-code-brackets: GatewayResponseTypeType](./literals.md#gatewayresponsetypetype) 
## DeleteIntegrationRequestRequestTypeDef

```python
# DeleteIntegrationRequestRequestTypeDef definition

class DeleteIntegrationRequestRequestTypeDef(TypedDict):
    restApiId: str,
    resourceId: str,
    httpMethod: str,
```

## DeleteIntegrationResponseRequestRequestTypeDef

```python
# DeleteIntegrationResponseRequestRequestTypeDef definition

class DeleteIntegrationResponseRequestRequestTypeDef(TypedDict):
    restApiId: str,
    resourceId: str,
    httpMethod: str,
    statusCode: str,
```

## DeleteMethodRequestRequestTypeDef

```python
# DeleteMethodRequestRequestTypeDef definition

class DeleteMethodRequestRequestTypeDef(TypedDict):
    restApiId: str,
    resourceId: str,
    httpMethod: str,
```

## DeleteMethodResponseRequestRequestTypeDef

```python
# DeleteMethodResponseRequestRequestTypeDef definition

class DeleteMethodResponseRequestRequestTypeDef(TypedDict):
    restApiId: str,
    resourceId: str,
    httpMethod: str,
    statusCode: str,
```

## DeleteModelRequestRequestTypeDef

```python
# DeleteModelRequestRequestTypeDef definition

class DeleteModelRequestRequestTypeDef(TypedDict):
    restApiId: str,
    modelName: str,
```

## DeleteRequestValidatorRequestRequestTypeDef

```python
# DeleteRequestValidatorRequestRequestTypeDef definition

class DeleteRequestValidatorRequestRequestTypeDef(TypedDict):
    restApiId: str,
    requestValidatorId: str,
```

## DeleteResourceRequestRequestTypeDef

```python
# DeleteResourceRequestRequestTypeDef definition

class DeleteResourceRequestRequestTypeDef(TypedDict):
    restApiId: str,
    resourceId: str,
```

## DeleteRestApiRequestRequestTypeDef

```python
# DeleteRestApiRequestRequestTypeDef definition

class DeleteRestApiRequestRequestTypeDef(TypedDict):
    restApiId: str,
```

## DeleteStageRequestRequestTypeDef

```python
# DeleteStageRequestRequestTypeDef definition

class DeleteStageRequestRequestTypeDef(TypedDict):
    restApiId: str,
    stageName: str,
```

## DeleteUsagePlanKeyRequestRequestTypeDef

```python
# DeleteUsagePlanKeyRequestRequestTypeDef definition

class DeleteUsagePlanKeyRequestRequestTypeDef(TypedDict):
    usagePlanId: str,
    keyId: str,
```

## DeleteUsagePlanRequestRequestTypeDef

```python
# DeleteUsagePlanRequestRequestTypeDef definition

class DeleteUsagePlanRequestRequestTypeDef(TypedDict):
    usagePlanId: str,
```

## DeleteVpcLinkRequestRequestTypeDef

```python
# DeleteVpcLinkRequestRequestTypeDef definition

class DeleteVpcLinkRequestRequestTypeDef(TypedDict):
    vpcLinkId: str,
```

## MethodSnapshotTypeDef

```python
# MethodSnapshotTypeDef definition

class MethodSnapshotTypeDef(TypedDict):
    authorizationType: NotRequired[str],
    apiKeyRequired: NotRequired[bool],
```

## DocumentationVersionTypeDef

```python
# DocumentationVersionTypeDef definition

class DocumentationVersionTypeDef(TypedDict):
    version: NotRequired[str],
    createdDate: NotRequired[datetime],
    description: NotRequired[str],
```

## EndpointConfigurationOutputTypeDef

```python
# EndpointConfigurationOutputTypeDef definition

class EndpointConfigurationOutputTypeDef(TypedDict):
    types: NotRequired[List[EndpointTypeType]],  # (1)
    vpcEndpointIds: NotRequired[List[str]],
```

1. See [:material-code-brackets: EndpointTypeType](./literals.md#endpointtypetype) 
## MutualTlsAuthenticationTypeDef

```python
# MutualTlsAuthenticationTypeDef definition

class MutualTlsAuthenticationTypeDef(TypedDict):
    truststoreUri: NotRequired[str],
    truststoreVersion: NotRequired[str],
    truststoreWarnings: NotRequired[List[str]],
```

## FlushStageAuthorizersCacheRequestRequestTypeDef

```python
# FlushStageAuthorizersCacheRequestRequestTypeDef definition

class FlushStageAuthorizersCacheRequestRequestTypeDef(TypedDict):
    restApiId: str,
    stageName: str,
```

## FlushStageCacheRequestRequestTypeDef

```python
# FlushStageCacheRequestRequestTypeDef definition

class FlushStageCacheRequestRequestTypeDef(TypedDict):
    restApiId: str,
    stageName: str,
```

## GatewayResponseTypeDef

```python
# GatewayResponseTypeDef definition

class GatewayResponseTypeDef(TypedDict):
    responseType: NotRequired[GatewayResponseTypeType],  # (1)
    statusCode: NotRequired[str],
    responseParameters: NotRequired[Dict[str, str]],
    responseTemplates: NotRequired[Dict[str, str]],
    defaultResponse: NotRequired[bool],
```

1. See [:material-code-brackets: GatewayResponseTypeType](./literals.md#gatewayresponsetypetype) 
## GenerateClientCertificateRequestRequestTypeDef

```python
# GenerateClientCertificateRequestRequestTypeDef definition

class GenerateClientCertificateRequestRequestTypeDef(TypedDict):
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## GetApiKeyRequestRequestTypeDef

```python
# GetApiKeyRequestRequestTypeDef definition

class GetApiKeyRequestRequestTypeDef(TypedDict):
    apiKey: str,
    includeValue: NotRequired[bool],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetApiKeysRequestRequestTypeDef

```python
# GetApiKeysRequestRequestTypeDef definition

class GetApiKeysRequestRequestTypeDef(TypedDict):
    position: NotRequired[str],
    limit: NotRequired[int],
    nameQuery: NotRequired[str],
    customerId: NotRequired[str],
    includeValues: NotRequired[bool],
```

## GetAuthorizerRequestRequestTypeDef

```python
# GetAuthorizerRequestRequestTypeDef definition

class GetAuthorizerRequestRequestTypeDef(TypedDict):
    restApiId: str,
    authorizerId: str,
```

## GetAuthorizersRequestRequestTypeDef

```python
# GetAuthorizersRequestRequestTypeDef definition

class GetAuthorizersRequestRequestTypeDef(TypedDict):
    restApiId: str,
    position: NotRequired[str],
    limit: NotRequired[int],
```

## GetBasePathMappingRequestRequestTypeDef

```python
# GetBasePathMappingRequestRequestTypeDef definition

class GetBasePathMappingRequestRequestTypeDef(TypedDict):
    domainName: str,
    basePath: str,
```

## GetBasePathMappingsRequestRequestTypeDef

```python
# GetBasePathMappingsRequestRequestTypeDef definition

class GetBasePathMappingsRequestRequestTypeDef(TypedDict):
    domainName: str,
    position: NotRequired[str],
    limit: NotRequired[int],
```

## GetClientCertificateRequestRequestTypeDef

```python
# GetClientCertificateRequestRequestTypeDef definition

class GetClientCertificateRequestRequestTypeDef(TypedDict):
    clientCertificateId: str,
```

## GetClientCertificatesRequestRequestTypeDef

```python
# GetClientCertificatesRequestRequestTypeDef definition

class GetClientCertificatesRequestRequestTypeDef(TypedDict):
    position: NotRequired[str],
    limit: NotRequired[int],
```

## GetDeploymentRequestRequestTypeDef

```python
# GetDeploymentRequestRequestTypeDef definition

class GetDeploymentRequestRequestTypeDef(TypedDict):
    restApiId: str,
    deploymentId: str,
    embed: NotRequired[Sequence[str]],
```

## GetDeploymentsRequestRequestTypeDef

```python
# GetDeploymentsRequestRequestTypeDef definition

class GetDeploymentsRequestRequestTypeDef(TypedDict):
    restApiId: str,
    position: NotRequired[str],
    limit: NotRequired[int],
```

## GetDocumentationPartRequestRequestTypeDef

```python
# GetDocumentationPartRequestRequestTypeDef definition

class GetDocumentationPartRequestRequestTypeDef(TypedDict):
    restApiId: str,
    documentationPartId: str,
```

## GetDocumentationPartsRequestRequestTypeDef

```python
# GetDocumentationPartsRequestRequestTypeDef definition

class GetDocumentationPartsRequestRequestTypeDef(TypedDict):
    restApiId: str,
    type: NotRequired[DocumentationPartTypeType],  # (1)
    nameQuery: NotRequired[str],
    path: NotRequired[str],
    position: NotRequired[str],
    limit: NotRequired[int],
    locationStatus: NotRequired[LocationStatusTypeType],  # (2)
```

1. See [:material-code-brackets: DocumentationPartTypeType](./literals.md#documentationparttypetype) 
2. See [:material-code-brackets: LocationStatusTypeType](./literals.md#locationstatustypetype) 
## GetDocumentationVersionRequestRequestTypeDef

```python
# GetDocumentationVersionRequestRequestTypeDef definition

class GetDocumentationVersionRequestRequestTypeDef(TypedDict):
    restApiId: str,
    documentationVersion: str,
```

## GetDocumentationVersionsRequestRequestTypeDef

```python
# GetDocumentationVersionsRequestRequestTypeDef definition

class GetDocumentationVersionsRequestRequestTypeDef(TypedDict):
    restApiId: str,
    position: NotRequired[str],
    limit: NotRequired[int],
```

## GetDomainNameRequestRequestTypeDef

```python
# GetDomainNameRequestRequestTypeDef definition

class GetDomainNameRequestRequestTypeDef(TypedDict):
    domainName: str,
```

## GetDomainNamesRequestRequestTypeDef

```python
# GetDomainNamesRequestRequestTypeDef definition

class GetDomainNamesRequestRequestTypeDef(TypedDict):
    position: NotRequired[str],
    limit: NotRequired[int],
```

## GetExportRequestRequestTypeDef

```python
# GetExportRequestRequestTypeDef definition

class GetExportRequestRequestTypeDef(TypedDict):
    restApiId: str,
    stageName: str,
    exportType: str,
    parameters: NotRequired[Mapping[str, str]],
    accepts: NotRequired[str],
```

## GetGatewayResponseRequestRequestTypeDef

```python
# GetGatewayResponseRequestRequestTypeDef definition

class GetGatewayResponseRequestRequestTypeDef(TypedDict):
    restApiId: str,
    responseType: GatewayResponseTypeType,  # (1)
```

1. See [:material-code-brackets: GatewayResponseTypeType](./literals.md#gatewayresponsetypetype) 
## GetGatewayResponsesRequestRequestTypeDef

```python
# GetGatewayResponsesRequestRequestTypeDef definition

class GetGatewayResponsesRequestRequestTypeDef(TypedDict):
    restApiId: str,
    position: NotRequired[str],
    limit: NotRequired[int],
```

## GetIntegrationRequestRequestTypeDef

```python
# GetIntegrationRequestRequestTypeDef definition

class GetIntegrationRequestRequestTypeDef(TypedDict):
    restApiId: str,
    resourceId: str,
    httpMethod: str,
```

## GetIntegrationResponseRequestRequestTypeDef

```python
# GetIntegrationResponseRequestRequestTypeDef definition

class GetIntegrationResponseRequestRequestTypeDef(TypedDict):
    restApiId: str,
    resourceId: str,
    httpMethod: str,
    statusCode: str,
```

## GetMethodRequestRequestTypeDef

```python
# GetMethodRequestRequestTypeDef definition

class GetMethodRequestRequestTypeDef(TypedDict):
    restApiId: str,
    resourceId: str,
    httpMethod: str,
```

## GetMethodResponseRequestRequestTypeDef

```python
# GetMethodResponseRequestRequestTypeDef definition

class GetMethodResponseRequestRequestTypeDef(TypedDict):
    restApiId: str,
    resourceId: str,
    httpMethod: str,
    statusCode: str,
```

## GetModelRequestRequestTypeDef

```python
# GetModelRequestRequestTypeDef definition

class GetModelRequestRequestTypeDef(TypedDict):
    restApiId: str,
    modelName: str,
    flatten: NotRequired[bool],
```

## GetModelTemplateRequestRequestTypeDef

```python
# GetModelTemplateRequestRequestTypeDef definition

class GetModelTemplateRequestRequestTypeDef(TypedDict):
    restApiId: str,
    modelName: str,
```

## GetModelsRequestRequestTypeDef

```python
# GetModelsRequestRequestTypeDef definition

class GetModelsRequestRequestTypeDef(TypedDict):
    restApiId: str,
    position: NotRequired[str],
    limit: NotRequired[int],
```

## GetRequestValidatorRequestRequestTypeDef

```python
# GetRequestValidatorRequestRequestTypeDef definition

class GetRequestValidatorRequestRequestTypeDef(TypedDict):
    restApiId: str,
    requestValidatorId: str,
```

## GetRequestValidatorsRequestRequestTypeDef

```python
# GetRequestValidatorsRequestRequestTypeDef definition

class GetRequestValidatorsRequestRequestTypeDef(TypedDict):
    restApiId: str,
    position: NotRequired[str],
    limit: NotRequired[int],
```

## GetResourceRequestRequestTypeDef

```python
# GetResourceRequestRequestTypeDef definition

class GetResourceRequestRequestTypeDef(TypedDict):
    restApiId: str,
    resourceId: str,
    embed: NotRequired[Sequence[str]],
```

## GetResourcesRequestRequestTypeDef

```python
# GetResourcesRequestRequestTypeDef definition

class GetResourcesRequestRequestTypeDef(TypedDict):
    restApiId: str,
    position: NotRequired[str],
    limit: NotRequired[int],
    embed: NotRequired[Sequence[str]],
```

## GetRestApiRequestRequestTypeDef

```python
# GetRestApiRequestRequestTypeDef definition

class GetRestApiRequestRequestTypeDef(TypedDict):
    restApiId: str,
```

## GetRestApisRequestRequestTypeDef

```python
# GetRestApisRequestRequestTypeDef definition

class GetRestApisRequestRequestTypeDef(TypedDict):
    position: NotRequired[str],
    limit: NotRequired[int],
```

## GetSdkRequestRequestTypeDef

```python
# GetSdkRequestRequestTypeDef definition

class GetSdkRequestRequestTypeDef(TypedDict):
    restApiId: str,
    stageName: str,
    sdkType: str,
    parameters: NotRequired[Mapping[str, str]],
```

## GetSdkTypeRequestRequestTypeDef

```python
# GetSdkTypeRequestRequestTypeDef definition

class GetSdkTypeRequestRequestTypeDef(TypedDict):
    id: str,
```

## GetSdkTypesRequestRequestTypeDef

```python
# GetSdkTypesRequestRequestTypeDef definition

class GetSdkTypesRequestRequestTypeDef(TypedDict):
    position: NotRequired[str],
    limit: NotRequired[int],
```

## GetStageRequestRequestTypeDef

```python
# GetStageRequestRequestTypeDef definition

class GetStageRequestRequestTypeDef(TypedDict):
    restApiId: str,
    stageName: str,
```

## GetStagesRequestRequestTypeDef

```python
# GetStagesRequestRequestTypeDef definition

class GetStagesRequestRequestTypeDef(TypedDict):
    restApiId: str,
    deploymentId: NotRequired[str],
```

## GetTagsRequestRequestTypeDef

```python
# GetTagsRequestRequestTypeDef definition

class GetTagsRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    position: NotRequired[str],
    limit: NotRequired[int],
```

## GetUsagePlanKeyRequestRequestTypeDef

```python
# GetUsagePlanKeyRequestRequestTypeDef definition

class GetUsagePlanKeyRequestRequestTypeDef(TypedDict):
    usagePlanId: str,
    keyId: str,
```

## GetUsagePlanKeysRequestRequestTypeDef

```python
# GetUsagePlanKeysRequestRequestTypeDef definition

class GetUsagePlanKeysRequestRequestTypeDef(TypedDict):
    usagePlanId: str,
    position: NotRequired[str],
    limit: NotRequired[int],
    nameQuery: NotRequired[str],
```

## GetUsagePlanRequestRequestTypeDef

```python
# GetUsagePlanRequestRequestTypeDef definition

class GetUsagePlanRequestRequestTypeDef(TypedDict):
    usagePlanId: str,
```

## GetUsagePlansRequestRequestTypeDef

```python
# GetUsagePlansRequestRequestTypeDef definition

class GetUsagePlansRequestRequestTypeDef(TypedDict):
    position: NotRequired[str],
    keyId: NotRequired[str],
    limit: NotRequired[int],
```

## GetUsageRequestRequestTypeDef

```python
# GetUsageRequestRequestTypeDef definition

class GetUsageRequestRequestTypeDef(TypedDict):
    usagePlanId: str,
    startDate: str,
    endDate: str,
    keyId: NotRequired[str],
    position: NotRequired[str],
    limit: NotRequired[int],
```

## GetVpcLinkRequestRequestTypeDef

```python
# GetVpcLinkRequestRequestTypeDef definition

class GetVpcLinkRequestRequestTypeDef(TypedDict):
    vpcLinkId: str,
```

## GetVpcLinksRequestRequestTypeDef

```python
# GetVpcLinksRequestRequestTypeDef definition

class GetVpcLinksRequestRequestTypeDef(TypedDict):
    position: NotRequired[str],
    limit: NotRequired[int],
```

## IntegrationResponseTypeDef

```python
# IntegrationResponseTypeDef definition

class IntegrationResponseTypeDef(TypedDict):
    statusCode: NotRequired[str],
    selectionPattern: NotRequired[str],
    responseParameters: NotRequired[Dict[str, str]],
    responseTemplates: NotRequired[Dict[str, str]],
    contentHandling: NotRequired[ContentHandlingStrategyType],  # (1)
```

1. See [:material-code-brackets: ContentHandlingStrategyType](./literals.md#contenthandlingstrategytype) 
## TlsConfigTypeDef

```python
# TlsConfigTypeDef definition

class TlsConfigTypeDef(TypedDict):
    insecureSkipVerification: NotRequired[bool],
```

## MethodResponseTypeDef

```python
# MethodResponseTypeDef definition

class MethodResponseTypeDef(TypedDict):
    statusCode: NotRequired[str],
    responseParameters: NotRequired[Dict[str, bool]],
    responseModels: NotRequired[Dict[str, str]],
```

## MethodSettingTypeDef

```python
# MethodSettingTypeDef definition

class MethodSettingTypeDef(TypedDict):
    metricsEnabled: NotRequired[bool],
    loggingLevel: NotRequired[str],
    dataTraceEnabled: NotRequired[bool],
    throttlingBurstLimit: NotRequired[int],
    throttlingRateLimit: NotRequired[float],
    cachingEnabled: NotRequired[bool],
    cacheTtlInSeconds: NotRequired[int],
    cacheDataEncrypted: NotRequired[bool],
    requireAuthorizationForCacheControl: NotRequired[bool],
    unauthorizedCacheControlHeaderStrategy: NotRequired[UnauthorizedCacheControlHeaderStrategyType],  # (1)
```

1. See [:material-code-brackets: UnauthorizedCacheControlHeaderStrategyType](./literals.md#unauthorizedcachecontrolheaderstrategytype) 
## ModelTypeDef

```python
# ModelTypeDef definition

class ModelTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    schema: NotRequired[str],
    contentType: NotRequired[str],
```

## PatchOperationTypeDef

```python
# PatchOperationTypeDef definition

class PatchOperationTypeDef(TypedDict):
    op: NotRequired[OpType],  # (1)
    path: NotRequired[str],
    value: NotRequired[str],
    from: NotRequired[str],
```

1. See [:material-code-brackets: OpType](./literals.md#optype) 
## PutGatewayResponseRequestRequestTypeDef

```python
# PutGatewayResponseRequestRequestTypeDef definition

class PutGatewayResponseRequestRequestTypeDef(TypedDict):
    restApiId: str,
    responseType: GatewayResponseTypeType,  # (1)
    statusCode: NotRequired[str],
    responseParameters: NotRequired[Mapping[str, str]],
    responseTemplates: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: GatewayResponseTypeType](./literals.md#gatewayresponsetypetype) 
## PutIntegrationResponseRequestRequestTypeDef

```python
# PutIntegrationResponseRequestRequestTypeDef definition

class PutIntegrationResponseRequestRequestTypeDef(TypedDict):
    restApiId: str,
    resourceId: str,
    httpMethod: str,
    statusCode: str,
    selectionPattern: NotRequired[str],
    responseParameters: NotRequired[Mapping[str, str]],
    responseTemplates: NotRequired[Mapping[str, str]],
    contentHandling: NotRequired[ContentHandlingStrategyType],  # (1)
```

1. See [:material-code-brackets: ContentHandlingStrategyType](./literals.md#contenthandlingstrategytype) 
## PutMethodRequestRequestTypeDef

```python
# PutMethodRequestRequestTypeDef definition

class PutMethodRequestRequestTypeDef(TypedDict):
    restApiId: str,
    resourceId: str,
    httpMethod: str,
    authorizationType: str,
    authorizerId: NotRequired[str],
    apiKeyRequired: NotRequired[bool],
    operationName: NotRequired[str],
    requestParameters: NotRequired[Mapping[str, bool]],
    requestModels: NotRequired[Mapping[str, str]],
    requestValidatorId: NotRequired[str],
    authorizationScopes: NotRequired[Sequence[str]],
```

## PutMethodResponseRequestRequestTypeDef

```python
# PutMethodResponseRequestRequestTypeDef definition

class PutMethodResponseRequestRequestTypeDef(TypedDict):
    restApiId: str,
    resourceId: str,
    httpMethod: str,
    statusCode: str,
    responseParameters: NotRequired[Mapping[str, bool]],
    responseModels: NotRequired[Mapping[str, str]],
```

## RequestValidatorTypeDef

```python
# RequestValidatorTypeDef definition

class RequestValidatorTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    validateRequestBody: NotRequired[bool],
    validateRequestParameters: NotRequired[bool],
```

## SdkConfigurationPropertyTypeDef

```python
# SdkConfigurationPropertyTypeDef definition

class SdkConfigurationPropertyTypeDef(TypedDict):
    name: NotRequired[str],
    friendlyName: NotRequired[str],
    description: NotRequired[str],
    required: NotRequired[bool],
    defaultValue: NotRequired[str],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## TestInvokeAuthorizerRequestRequestTypeDef

```python
# TestInvokeAuthorizerRequestRequestTypeDef definition

class TestInvokeAuthorizerRequestRequestTypeDef(TypedDict):
    restApiId: str,
    authorizerId: str,
    headers: NotRequired[Mapping[str, str]],
    multiValueHeaders: NotRequired[Mapping[str, Sequence[str]]],
    pathWithQueryString: NotRequired[str],
    body: NotRequired[str],
    stageVariables: NotRequired[Mapping[str, str]],
    additionalContext: NotRequired[Mapping[str, str]],
```

## TestInvokeMethodRequestRequestTypeDef

```python
# TestInvokeMethodRequestRequestTypeDef definition

class TestInvokeMethodRequestRequestTypeDef(TypedDict):
    restApiId: str,
    resourceId: str,
    httpMethod: str,
    pathWithQueryString: NotRequired[str],
    body: NotRequired[str],
    headers: NotRequired[Mapping[str, str]],
    multiValueHeaders: NotRequired[Mapping[str, Sequence[str]]],
    clientCertificateId: NotRequired[str],
    stageVariables: NotRequired[Mapping[str, str]],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UsagePlanKeyTypeDef

```python
# UsagePlanKeyTypeDef definition

class UsagePlanKeyTypeDef(TypedDict):
    id: NotRequired[str],
    type: NotRequired[str],
    value: NotRequired[str],
    name: NotRequired[str],
```

## VpcLinkTypeDef

```python
# VpcLinkTypeDef definition

class VpcLinkTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    targetArns: NotRequired[List[str]],
    status: NotRequired[VpcLinkStatusType],  # (1)
    statusMessage: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: VpcLinkStatusType](./literals.md#vpclinkstatustype) 
## ApiKeyIdsTypeDef

```python
# ApiKeyIdsTypeDef definition

class ApiKeyIdsTypeDef(TypedDict):
    ids: List[str],
    warnings: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ApiKeyResponseTypeDef

```python
# ApiKeyResponseTypeDef definition

class ApiKeyResponseTypeDef(TypedDict):
    id: str,
    value: str,
    name: str,
    customerId: str,
    description: str,
    enabled: bool,
    createdDate: datetime,
    lastUpdatedDate: datetime,
    stageKeys: List[str],
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AuthorizerResponseTypeDef

```python
# AuthorizerResponseTypeDef definition

class AuthorizerResponseTypeDef(TypedDict):
    id: str,
    name: str,
    type: AuthorizerTypeType,  # (1)
    providerARNs: List[str],
    authType: str,
    authorizerUri: str,
    authorizerCredentials: str,
    identitySource: str,
    identityValidationExpression: str,
    authorizerResultTtlInSeconds: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AuthorizerTypeType](./literals.md#authorizertypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BasePathMappingResponseTypeDef

```python
# BasePathMappingResponseTypeDef definition

class BasePathMappingResponseTypeDef(TypedDict):
    basePath: str,
    restApiId: str,
    stage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ClientCertificateResponseTypeDef

```python
# ClientCertificateResponseTypeDef definition

class ClientCertificateResponseTypeDef(TypedDict):
    clientCertificateId: str,
    description: str,
    pemEncodedCertificate: str,
    createdDate: datetime,
    expirationDate: datetime,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DocumentationPartIdsTypeDef

```python
# DocumentationPartIdsTypeDef definition

class DocumentationPartIdsTypeDef(TypedDict):
    ids: List[str],
    warnings: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DocumentationVersionResponseTypeDef

```python
# DocumentationVersionResponseTypeDef definition

class DocumentationVersionResponseTypeDef(TypedDict):
    version: str,
    createdDate: datetime,
    description: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportResponseTypeDef

```python
# ExportResponseTypeDef definition

class ExportResponseTypeDef(TypedDict):
    contentType: str,
    contentDisposition: str,
    body: StreamingBody,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GatewayResponseResponseTypeDef

```python
# GatewayResponseResponseTypeDef definition

class GatewayResponseResponseTypeDef(TypedDict):
    responseType: GatewayResponseTypeType,  # (1)
    statusCode: str,
    responseParameters: Dict[str, str],
    responseTemplates: Dict[str, str],
    defaultResponse: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: GatewayResponseTypeType](./literals.md#gatewayresponsetypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IntegrationResponseResponseTypeDef

```python
# IntegrationResponseResponseTypeDef definition

class IntegrationResponseResponseTypeDef(TypedDict):
    statusCode: str,
    selectionPattern: str,
    responseParameters: Dict[str, str],
    responseTemplates: Dict[str, str],
    contentHandling: ContentHandlingStrategyType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ContentHandlingStrategyType](./literals.md#contenthandlingstrategytype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MethodResponseResponseTypeDef

```python
# MethodResponseResponseTypeDef definition

class MethodResponseResponseTypeDef(TypedDict):
    statusCode: str,
    responseParameters: Dict[str, bool],
    responseModels: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModelResponseTypeDef

```python
# ModelResponseTypeDef definition

class ModelResponseTypeDef(TypedDict):
    id: str,
    name: str,
    description: str,
    schema: str,
    contentType: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RequestValidatorResponseTypeDef

```python
# RequestValidatorResponseTypeDef definition

class RequestValidatorResponseTypeDef(TypedDict):
    id: str,
    name: str,
    validateRequestBody: bool,
    validateRequestParameters: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SdkResponseTypeDef

```python
# SdkResponseTypeDef definition

class SdkResponseTypeDef(TypedDict):
    contentType: str,
    contentDisposition: str,
    body: StreamingBody,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagsTypeDef

```python
# TagsTypeDef definition

class TagsTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TemplateTypeDef

```python
# TemplateTypeDef definition

class TemplateTypeDef(TypedDict):
    value: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TestInvokeAuthorizerResponseTypeDef

```python
# TestInvokeAuthorizerResponseTypeDef definition

class TestInvokeAuthorizerResponseTypeDef(TypedDict):
    clientStatus: int,
    log: str,
    latency: int,
    principalId: str,
    policy: str,
    authorization: Dict[str, List[str]],
    claims: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TestInvokeMethodResponseTypeDef

```python
# TestInvokeMethodResponseTypeDef definition

class TestInvokeMethodResponseTypeDef(TypedDict):
    status: int,
    body: str,
    headers: Dict[str, str],
    multiValueHeaders: Dict[str, List[str]],
    log: str,
    latency: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UsagePlanKeyResponseTypeDef

```python
# UsagePlanKeyResponseTypeDef definition

class UsagePlanKeyResponseTypeDef(TypedDict):
    id: str,
    type: str,
    value: str,
    name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UsageTypeDef

```python
# UsageTypeDef definition

class UsageTypeDef(TypedDict):
    usagePlanId: str,
    startDate: str,
    endDate: str,
    position: str,
    items: Dict[str, List[List[int]]],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VpcLinkResponseTypeDef

```python
# VpcLinkResponseTypeDef definition

class VpcLinkResponseTypeDef(TypedDict):
    id: str,
    name: str,
    description: str,
    targetArns: List[str],
    status: VpcLinkStatusType,  # (1)
    statusMessage: str,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: VpcLinkStatusType](./literals.md#vpclinkstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AccountTypeDef

```python
# AccountTypeDef definition

class AccountTypeDef(TypedDict):
    cloudwatchRoleArn: str,
    throttleSettings: ThrottleSettingsTypeDef,  # (1)
    features: List[str],
    apiKeyVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ThrottleSettingsTypeDef](./type_defs.md#throttlesettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ApiStageOutputTypeDef

```python
# ApiStageOutputTypeDef definition

class ApiStageOutputTypeDef(TypedDict):
    apiId: NotRequired[str],
    stage: NotRequired[str],
    throttle: NotRequired[Dict[str, ThrottleSettingsTypeDef]],  # (1)
```

1. See [:material-code-braces: ThrottleSettingsTypeDef](./type_defs.md#throttlesettingstypedef) 
## ApiStageTypeDef

```python
# ApiStageTypeDef definition

class ApiStageTypeDef(TypedDict):
    apiId: NotRequired[str],
    stage: NotRequired[str],
    throttle: NotRequired[Mapping[str, ThrottleSettingsTypeDef]],  # (1)
```

1. See [:material-code-braces: ThrottleSettingsTypeDef](./type_defs.md#throttlesettingstypedef) 
## ApiKeysTypeDef

```python
# ApiKeysTypeDef definition

class ApiKeysTypeDef(TypedDict):
    warnings: List[str],
    position: str,
    items: List[ApiKeyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApiKeyTypeDef](./type_defs.md#apikeytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AuthorizersTypeDef

```python
# AuthorizersTypeDef definition

class AuthorizersTypeDef(TypedDict):
    position: str,
    items: List[AuthorizerTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AuthorizerTypeDef](./type_defs.md#authorizertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BasePathMappingsTypeDef

```python
# BasePathMappingsTypeDef definition

class BasePathMappingsTypeDef(TypedDict):
    position: str,
    items: List[BasePathMappingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BasePathMappingTypeDef](./type_defs.md#basepathmappingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportApiKeysRequestRequestTypeDef

```python
# ImportApiKeysRequestRequestTypeDef definition

class ImportApiKeysRequestRequestTypeDef(TypedDict):
    body: BlobTypeDef,
    format: ApiKeysFormatType,  # (1)
    failOnWarnings: NotRequired[bool],
```

1. See [:material-code-brackets: ApiKeysFormatType](./literals.md#apikeysformattype) 
## ImportDocumentationPartsRequestRequestTypeDef

```python
# ImportDocumentationPartsRequestRequestTypeDef definition

class ImportDocumentationPartsRequestRequestTypeDef(TypedDict):
    restApiId: str,
    body: BlobTypeDef,
    mode: NotRequired[PutModeType],  # (1)
    failOnWarnings: NotRequired[bool],
```

1. See [:material-code-brackets: PutModeType](./literals.md#putmodetype) 
## ImportRestApiRequestRequestTypeDef

```python
# ImportRestApiRequestRequestTypeDef definition

class ImportRestApiRequestRequestTypeDef(TypedDict):
    body: BlobTypeDef,
    failOnWarnings: NotRequired[bool],
    parameters: NotRequired[Mapping[str, str]],
```

## PutRestApiRequestRequestTypeDef

```python
# PutRestApiRequestRequestTypeDef definition

class PutRestApiRequestRequestTypeDef(TypedDict):
    restApiId: str,
    body: BlobTypeDef,
    mode: NotRequired[PutModeType],  # (1)
    failOnWarnings: NotRequired[bool],
    parameters: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: PutModeType](./literals.md#putmodetype) 
## CreateStageRequestRequestTypeDef

```python
# CreateStageRequestRequestTypeDef definition

class CreateStageRequestRequestTypeDef(TypedDict):
    restApiId: str,
    stageName: str,
    deploymentId: str,
    description: NotRequired[str],
    cacheClusterEnabled: NotRequired[bool],
    cacheClusterSize: NotRequired[CacheClusterSizeType],  # (1)
    variables: NotRequired[Mapping[str, str]],
    documentationVersion: NotRequired[str],
    canarySettings: NotRequired[CanarySettingsTypeDef],  # (2)
    tracingEnabled: NotRequired[bool],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: CacheClusterSizeType](./literals.md#cacheclustersizetype) 
2. See [:material-code-braces: CanarySettingsTypeDef](./type_defs.md#canarysettingstypedef) 
## ClientCertificatesTypeDef

```python
# ClientCertificatesTypeDef definition

class ClientCertificatesTypeDef(TypedDict):
    position: str,
    items: List[ClientCertificateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClientCertificateTypeDef](./type_defs.md#clientcertificatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateApiKeyRequestRequestTypeDef

```python
# CreateApiKeyRequestRequestTypeDef definition

class CreateApiKeyRequestRequestTypeDef(TypedDict):
    name: NotRequired[str],
    description: NotRequired[str],
    enabled: NotRequired[bool],
    generateDistinctId: NotRequired[bool],
    value: NotRequired[str],
    stageKeys: NotRequired[Sequence[StageKeyTypeDef]],  # (1)
    customerId: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: StageKeyTypeDef](./type_defs.md#stagekeytypedef) 
## CreateDeploymentRequestRequestTypeDef

```python
# CreateDeploymentRequestRequestTypeDef definition

class CreateDeploymentRequestRequestTypeDef(TypedDict):
    restApiId: str,
    stageName: NotRequired[str],
    stageDescription: NotRequired[str],
    description: NotRequired[str],
    cacheClusterEnabled: NotRequired[bool],
    cacheClusterSize: NotRequired[CacheClusterSizeType],  # (1)
    variables: NotRequired[Mapping[str, str]],
    canarySettings: NotRequired[DeploymentCanarySettingsTypeDef],  # (2)
    tracingEnabled: NotRequired[bool],
```

1. See [:material-code-brackets: CacheClusterSizeType](./literals.md#cacheclustersizetype) 
2. See [:material-code-braces: DeploymentCanarySettingsTypeDef](./type_defs.md#deploymentcanarysettingstypedef) 
## CreateDocumentationPartRequestRequestTypeDef

```python
# CreateDocumentationPartRequestRequestTypeDef definition

class CreateDocumentationPartRequestRequestTypeDef(TypedDict):
    restApiId: str,
    location: DocumentationPartLocationTypeDef,  # (1)
    properties: str,
```

1. See [:material-code-braces: DocumentationPartLocationTypeDef](./type_defs.md#documentationpartlocationtypedef) 
## DocumentationPartResponseTypeDef

```python
# DocumentationPartResponseTypeDef definition

class DocumentationPartResponseTypeDef(TypedDict):
    id: str,
    location: DocumentationPartLocationTypeDef,  # (1)
    properties: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DocumentationPartLocationTypeDef](./type_defs.md#documentationpartlocationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DocumentationPartTypeDef

```python
# DocumentationPartTypeDef definition

class DocumentationPartTypeDef(TypedDict):
    id: NotRequired[str],
    location: NotRequired[DocumentationPartLocationTypeDef],  # (1)
    properties: NotRequired[str],
```

1. See [:material-code-braces: DocumentationPartLocationTypeDef](./type_defs.md#documentationpartlocationtypedef) 
## CreateRestApiRequestRequestTypeDef

```python
# CreateRestApiRequestRequestTypeDef definition

class CreateRestApiRequestRequestTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    version: NotRequired[str],
    cloneFrom: NotRequired[str],
    binaryMediaTypes: NotRequired[Sequence[str]],
    minimumCompressionSize: NotRequired[int],
    apiKeySource: NotRequired[ApiKeySourceTypeType],  # (1)
    endpointConfiguration: NotRequired[EndpointConfigurationTypeDef],  # (2)
    policy: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    disableExecuteApiEndpoint: NotRequired[bool],
```

1. See [:material-code-brackets: ApiKeySourceTypeType](./literals.md#apikeysourcetypetype) 
2. See [:material-code-braces: EndpointConfigurationTypeDef](./type_defs.md#endpointconfigurationtypedef) 
## CreateDomainNameRequestRequestTypeDef

```python
# CreateDomainNameRequestRequestTypeDef definition

class CreateDomainNameRequestRequestTypeDef(TypedDict):
    domainName: str,
    certificateName: NotRequired[str],
    certificateBody: NotRequired[str],
    certificatePrivateKey: NotRequired[str],
    certificateChain: NotRequired[str],
    certificateArn: NotRequired[str],
    regionalCertificateName: NotRequired[str],
    regionalCertificateArn: NotRequired[str],
    endpointConfiguration: NotRequired[EndpointConfigurationTypeDef],  # (1)
    tags: NotRequired[Mapping[str, str]],
    securityPolicy: NotRequired[SecurityPolicyType],  # (2)
    mutualTlsAuthentication: NotRequired[MutualTlsAuthenticationInputTypeDef],  # (3)
    ownershipVerificationCertificateArn: NotRequired[str],
```

1. See [:material-code-braces: EndpointConfigurationTypeDef](./type_defs.md#endpointconfigurationtypedef) 
2. See [:material-code-brackets: SecurityPolicyType](./literals.md#securitypolicytype) 
3. See [:material-code-braces: MutualTlsAuthenticationInputTypeDef](./type_defs.md#mutualtlsauthenticationinputtypedef) 
## DeploymentResponseTypeDef

```python
# DeploymentResponseTypeDef definition

class DeploymentResponseTypeDef(TypedDict):
    id: str,
    description: str,
    createdDate: datetime,
    apiSummary: Dict[str, Dict[str, MethodSnapshotTypeDef]],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MethodSnapshotTypeDef](./type_defs.md#methodsnapshottypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeploymentTypeDef

```python
# DeploymentTypeDef definition

class DeploymentTypeDef(TypedDict):
    id: NotRequired[str],
    description: NotRequired[str],
    createdDate: NotRequired[datetime],
    apiSummary: NotRequired[Dict[str, Dict[str, MethodSnapshotTypeDef]]],  # (1)
```

1. See [:material-code-braces: MethodSnapshotTypeDef](./type_defs.md#methodsnapshottypedef) 
## DocumentationVersionsTypeDef

```python
# DocumentationVersionsTypeDef definition

class DocumentationVersionsTypeDef(TypedDict):
    position: str,
    items: List[DocumentationVersionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DocumentationVersionTypeDef](./type_defs.md#documentationversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestApiResponseTypeDef

```python
# RestApiResponseTypeDef definition

class RestApiResponseTypeDef(TypedDict):
    id: str,
    name: str,
    description: str,
    createdDate: datetime,
    version: str,
    warnings: List[str],
    binaryMediaTypes: List[str],
    minimumCompressionSize: int,
    apiKeySource: ApiKeySourceTypeType,  # (1)
    endpointConfiguration: EndpointConfigurationOutputTypeDef,  # (2)
    policy: str,
    tags: Dict[str, str],
    disableExecuteApiEndpoint: bool,
    rootResourceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ApiKeySourceTypeType](./literals.md#apikeysourcetypetype) 
2. See [:material-code-braces: EndpointConfigurationOutputTypeDef](./type_defs.md#endpointconfigurationoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestApiTypeDef

```python
# RestApiTypeDef definition

class RestApiTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    createdDate: NotRequired[datetime],
    version: NotRequired[str],
    warnings: NotRequired[List[str]],
    binaryMediaTypes: NotRequired[List[str]],
    minimumCompressionSize: NotRequired[int],
    apiKeySource: NotRequired[ApiKeySourceTypeType],  # (1)
    endpointConfiguration: NotRequired[EndpointConfigurationOutputTypeDef],  # (2)
    policy: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    disableExecuteApiEndpoint: NotRequired[bool],
    rootResourceId: NotRequired[str],
```

1. See [:material-code-brackets: ApiKeySourceTypeType](./literals.md#apikeysourcetypetype) 
2. See [:material-code-braces: EndpointConfigurationOutputTypeDef](./type_defs.md#endpointconfigurationoutputtypedef) 
## DomainNameResponseTypeDef

```python
# DomainNameResponseTypeDef definition

class DomainNameResponseTypeDef(TypedDict):
    domainName: str,
    certificateName: str,
    certificateArn: str,
    certificateUploadDate: datetime,
    regionalDomainName: str,
    regionalHostedZoneId: str,
    regionalCertificateName: str,
    regionalCertificateArn: str,
    distributionDomainName: str,
    distributionHostedZoneId: str,
    endpointConfiguration: EndpointConfigurationOutputTypeDef,  # (1)
    domainNameStatus: DomainNameStatusType,  # (2)
    domainNameStatusMessage: str,
    securityPolicy: SecurityPolicyType,  # (3)
    tags: Dict[str, str],
    mutualTlsAuthentication: MutualTlsAuthenticationTypeDef,  # (4)
    ownershipVerificationCertificateArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: EndpointConfigurationOutputTypeDef](./type_defs.md#endpointconfigurationoutputtypedef) 
2. See [:material-code-brackets: DomainNameStatusType](./literals.md#domainnamestatustype) 
3. See [:material-code-brackets: SecurityPolicyType](./literals.md#securitypolicytype) 
4. See [:material-code-braces: MutualTlsAuthenticationTypeDef](./type_defs.md#mutualtlsauthenticationtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DomainNameTypeDef

```python
# DomainNameTypeDef definition

class DomainNameTypeDef(TypedDict):
    domainName: NotRequired[str],
    certificateName: NotRequired[str],
    certificateArn: NotRequired[str],
    certificateUploadDate: NotRequired[datetime],
    regionalDomainName: NotRequired[str],
    regionalHostedZoneId: NotRequired[str],
    regionalCertificateName: NotRequired[str],
    regionalCertificateArn: NotRequired[str],
    distributionDomainName: NotRequired[str],
    distributionHostedZoneId: NotRequired[str],
    endpointConfiguration: NotRequired[EndpointConfigurationOutputTypeDef],  # (1)
    domainNameStatus: NotRequired[DomainNameStatusType],  # (2)
    domainNameStatusMessage: NotRequired[str],
    securityPolicy: NotRequired[SecurityPolicyType],  # (3)
    tags: NotRequired[Dict[str, str]],
    mutualTlsAuthentication: NotRequired[MutualTlsAuthenticationTypeDef],  # (4)
    ownershipVerificationCertificateArn: NotRequired[str],
```

1. See [:material-code-braces: EndpointConfigurationOutputTypeDef](./type_defs.md#endpointconfigurationoutputtypedef) 
2. See [:material-code-brackets: DomainNameStatusType](./literals.md#domainnamestatustype) 
3. See [:material-code-brackets: SecurityPolicyType](./literals.md#securitypolicytype) 
4. See [:material-code-braces: MutualTlsAuthenticationTypeDef](./type_defs.md#mutualtlsauthenticationtypedef) 
## GatewayResponsesTypeDef

```python
# GatewayResponsesTypeDef definition

class GatewayResponsesTypeDef(TypedDict):
    position: str,
    items: List[GatewayResponseTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GatewayResponseTypeDef](./type_defs.md#gatewayresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetApiKeysRequestGetApiKeysPaginateTypeDef

```python
# GetApiKeysRequestGetApiKeysPaginateTypeDef definition

class GetApiKeysRequestGetApiKeysPaginateTypeDef(TypedDict):
    nameQuery: NotRequired[str],
    customerId: NotRequired[str],
    includeValues: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetAuthorizersRequestGetAuthorizersPaginateTypeDef

```python
# GetAuthorizersRequestGetAuthorizersPaginateTypeDef definition

class GetAuthorizersRequestGetAuthorizersPaginateTypeDef(TypedDict):
    restApiId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef

```python
# GetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef definition

class GetBasePathMappingsRequestGetBasePathMappingsPaginateTypeDef(TypedDict):
    domainName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetClientCertificatesRequestGetClientCertificatesPaginateTypeDef

```python
# GetClientCertificatesRequestGetClientCertificatesPaginateTypeDef definition

class GetClientCertificatesRequestGetClientCertificatesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetDeploymentsRequestGetDeploymentsPaginateTypeDef

```python
# GetDeploymentsRequestGetDeploymentsPaginateTypeDef definition

class GetDeploymentsRequestGetDeploymentsPaginateTypeDef(TypedDict):
    restApiId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef

```python
# GetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef definition

class GetDocumentationPartsRequestGetDocumentationPartsPaginateTypeDef(TypedDict):
    restApiId: str,
    type: NotRequired[DocumentationPartTypeType],  # (1)
    nameQuery: NotRequired[str],
    path: NotRequired[str],
    locationStatus: NotRequired[LocationStatusTypeType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: DocumentationPartTypeType](./literals.md#documentationparttypetype) 
2. See [:material-code-brackets: LocationStatusTypeType](./literals.md#locationstatustypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef

```python
# GetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef definition

class GetDocumentationVersionsRequestGetDocumentationVersionsPaginateTypeDef(TypedDict):
    restApiId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetDomainNamesRequestGetDomainNamesPaginateTypeDef

```python
# GetDomainNamesRequestGetDomainNamesPaginateTypeDef definition

class GetDomainNamesRequestGetDomainNamesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef

```python
# GetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef definition

class GetGatewayResponsesRequestGetGatewayResponsesPaginateTypeDef(TypedDict):
    restApiId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetModelsRequestGetModelsPaginateTypeDef

```python
# GetModelsRequestGetModelsPaginateTypeDef definition

class GetModelsRequestGetModelsPaginateTypeDef(TypedDict):
    restApiId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef

```python
# GetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef definition

class GetRequestValidatorsRequestGetRequestValidatorsPaginateTypeDef(TypedDict):
    restApiId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetResourcesRequestGetResourcesPaginateTypeDef

```python
# GetResourcesRequestGetResourcesPaginateTypeDef definition

class GetResourcesRequestGetResourcesPaginateTypeDef(TypedDict):
    restApiId: str,
    embed: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetRestApisRequestGetRestApisPaginateTypeDef

```python
# GetRestApisRequestGetRestApisPaginateTypeDef definition

class GetRestApisRequestGetRestApisPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetSdkTypesRequestGetSdkTypesPaginateTypeDef

```python
# GetSdkTypesRequestGetSdkTypesPaginateTypeDef definition

class GetSdkTypesRequestGetSdkTypesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef

```python
# GetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef definition

class GetUsagePlanKeysRequestGetUsagePlanKeysPaginateTypeDef(TypedDict):
    usagePlanId: str,
    nameQuery: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetUsagePlansRequestGetUsagePlansPaginateTypeDef

```python
# GetUsagePlansRequestGetUsagePlansPaginateTypeDef definition

class GetUsagePlansRequestGetUsagePlansPaginateTypeDef(TypedDict):
    keyId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetUsageRequestGetUsagePaginateTypeDef

```python
# GetUsageRequestGetUsagePaginateTypeDef definition

class GetUsageRequestGetUsagePaginateTypeDef(TypedDict):
    usagePlanId: str,
    startDate: str,
    endDate: str,
    keyId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetVpcLinksRequestGetVpcLinksPaginateTypeDef

```python
# GetVpcLinksRequestGetVpcLinksPaginateTypeDef definition

class GetVpcLinksRequestGetVpcLinksPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## IntegrationExtraResponseTypeDef

```python
# IntegrationExtraResponseTypeDef definition

class IntegrationExtraResponseTypeDef(TypedDict):
    type: IntegrationTypeType,  # (1)
    httpMethod: str,
    uri: str,
    connectionType: ConnectionTypeType,  # (2)
    connectionId: str,
    credentials: str,
    requestParameters: Dict[str, str],
    requestTemplates: Dict[str, str],
    passthroughBehavior: str,
    contentHandling: ContentHandlingStrategyType,  # (3)
    timeoutInMillis: int,
    cacheNamespace: str,
    cacheKeyParameters: List[str],
    integrationResponses: Dict[str, IntegrationResponseTypeDef],  # (4)
    tlsConfig: TlsConfigTypeDef,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: IntegrationTypeType](./literals.md#integrationtypetype) 
2. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
3. See [:material-code-brackets: ContentHandlingStrategyType](./literals.md#contenthandlingstrategytype) 
4. See [:material-code-braces: IntegrationResponseTypeDef](./type_defs.md#integrationresponsetypedef) 
5. See [:material-code-braces: TlsConfigTypeDef](./type_defs.md#tlsconfigtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IntegrationTypeDef

```python
# IntegrationTypeDef definition

class IntegrationTypeDef(TypedDict):
    type: NotRequired[IntegrationTypeType],  # (1)
    httpMethod: NotRequired[str],
    uri: NotRequired[str],
    connectionType: NotRequired[ConnectionTypeType],  # (2)
    connectionId: NotRequired[str],
    credentials: NotRequired[str],
    requestParameters: NotRequired[Dict[str, str]],
    requestTemplates: NotRequired[Dict[str, str]],
    passthroughBehavior: NotRequired[str],
    contentHandling: NotRequired[ContentHandlingStrategyType],  # (3)
    timeoutInMillis: NotRequired[int],
    cacheNamespace: NotRequired[str],
    cacheKeyParameters: NotRequired[List[str]],
    integrationResponses: NotRequired[Dict[str, IntegrationResponseTypeDef]],  # (4)
    tlsConfig: NotRequired[TlsConfigTypeDef],  # (5)
```

1. See [:material-code-brackets: IntegrationTypeType](./literals.md#integrationtypetype) 
2. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
3. See [:material-code-brackets: ContentHandlingStrategyType](./literals.md#contenthandlingstrategytype) 
4. See [:material-code-braces: IntegrationResponseTypeDef](./type_defs.md#integrationresponsetypedef) 
5. See [:material-code-braces: TlsConfigTypeDef](./type_defs.md#tlsconfigtypedef) 
## PutIntegrationRequestRequestTypeDef

```python
# PutIntegrationRequestRequestTypeDef definition

class PutIntegrationRequestRequestTypeDef(TypedDict):
    restApiId: str,
    resourceId: str,
    httpMethod: str,
    type: IntegrationTypeType,  # (1)
    integrationHttpMethod: NotRequired[str],
    uri: NotRequired[str],
    connectionType: NotRequired[ConnectionTypeType],  # (2)
    connectionId: NotRequired[str],
    credentials: NotRequired[str],
    requestParameters: NotRequired[Mapping[str, str]],
    requestTemplates: NotRequired[Mapping[str, str]],
    passthroughBehavior: NotRequired[str],
    cacheNamespace: NotRequired[str],
    cacheKeyParameters: NotRequired[Sequence[str]],
    contentHandling: NotRequired[ContentHandlingStrategyType],  # (3)
    timeoutInMillis: NotRequired[int],
    tlsConfig: NotRequired[TlsConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: IntegrationTypeType](./literals.md#integrationtypetype) 
2. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
3. See [:material-code-brackets: ContentHandlingStrategyType](./literals.md#contenthandlingstrategytype) 
4. See [:material-code-braces: TlsConfigTypeDef](./type_defs.md#tlsconfigtypedef) 
## StageResponseTypeDef

```python
# StageResponseTypeDef definition

class StageResponseTypeDef(TypedDict):
    deploymentId: str,
    clientCertificateId: str,
    stageName: str,
    description: str,
    cacheClusterEnabled: bool,
    cacheClusterSize: CacheClusterSizeType,  # (1)
    cacheClusterStatus: CacheClusterStatusType,  # (2)
    methodSettings: Dict[str, MethodSettingTypeDef],  # (3)
    variables: Dict[str, str],
    documentationVersion: str,
    accessLogSettings: AccessLogSettingsTypeDef,  # (4)
    canarySettings: CanarySettingsOutputTypeDef,  # (5)
    tracingEnabled: bool,
    webAclArn: str,
    tags: Dict[str, str],
    createdDate: datetime,
    lastUpdatedDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: CacheClusterSizeType](./literals.md#cacheclustersizetype) 
2. See [:material-code-brackets: CacheClusterStatusType](./literals.md#cacheclusterstatustype) 
3. See [:material-code-braces: MethodSettingTypeDef](./type_defs.md#methodsettingtypedef) 
4. See [:material-code-braces: AccessLogSettingsTypeDef](./type_defs.md#accesslogsettingstypedef) 
5. See [:material-code-braces: CanarySettingsOutputTypeDef](./type_defs.md#canarysettingsoutputtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StageTypeDef

```python
# StageTypeDef definition

class StageTypeDef(TypedDict):
    deploymentId: NotRequired[str],
    clientCertificateId: NotRequired[str],
    stageName: NotRequired[str],
    description: NotRequired[str],
    cacheClusterEnabled: NotRequired[bool],
    cacheClusterSize: NotRequired[CacheClusterSizeType],  # (1)
    cacheClusterStatus: NotRequired[CacheClusterStatusType],  # (2)
    methodSettings: NotRequired[Dict[str, MethodSettingTypeDef]],  # (3)
    variables: NotRequired[Dict[str, str]],
    documentationVersion: NotRequired[str],
    accessLogSettings: NotRequired[AccessLogSettingsTypeDef],  # (4)
    canarySettings: NotRequired[CanarySettingsOutputTypeDef],  # (5)
    tracingEnabled: NotRequired[bool],
    webAclArn: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    createdDate: NotRequired[datetime],
    lastUpdatedDate: NotRequired[datetime],
```

1. See [:material-code-brackets: CacheClusterSizeType](./literals.md#cacheclustersizetype) 
2. See [:material-code-brackets: CacheClusterStatusType](./literals.md#cacheclusterstatustype) 
3. See [:material-code-braces: MethodSettingTypeDef](./type_defs.md#methodsettingtypedef) 
4. See [:material-code-braces: AccessLogSettingsTypeDef](./type_defs.md#accesslogsettingstypedef) 
5. See [:material-code-braces: CanarySettingsOutputTypeDef](./type_defs.md#canarysettingsoutputtypedef) 
## ModelsTypeDef

```python
# ModelsTypeDef definition

class ModelsTypeDef(TypedDict):
    position: str,
    items: List[ModelTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ModelTypeDef](./type_defs.md#modeltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAccountRequestRequestTypeDef

```python
# UpdateAccountRequestRequestTypeDef definition

class UpdateAccountRequestRequestTypeDef(TypedDict):
    patchOperations: NotRequired[Sequence[PatchOperationTypeDef]],  # (1)
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
## UpdateApiKeyRequestRequestTypeDef

```python
# UpdateApiKeyRequestRequestTypeDef definition

class UpdateApiKeyRequestRequestTypeDef(TypedDict):
    apiKey: str,
    patchOperations: NotRequired[Sequence[PatchOperationTypeDef]],  # (1)
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
## UpdateAuthorizerRequestRequestTypeDef

```python
# UpdateAuthorizerRequestRequestTypeDef definition

class UpdateAuthorizerRequestRequestTypeDef(TypedDict):
    restApiId: str,
    authorizerId: str,
    patchOperations: NotRequired[Sequence[PatchOperationTypeDef]],  # (1)
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
## UpdateBasePathMappingRequestRequestTypeDef

```python
# UpdateBasePathMappingRequestRequestTypeDef definition

class UpdateBasePathMappingRequestRequestTypeDef(TypedDict):
    domainName: str,
    basePath: str,
    patchOperations: NotRequired[Sequence[PatchOperationTypeDef]],  # (1)
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
## UpdateClientCertificateRequestRequestTypeDef

```python
# UpdateClientCertificateRequestRequestTypeDef definition

class UpdateClientCertificateRequestRequestTypeDef(TypedDict):
    clientCertificateId: str,
    patchOperations: NotRequired[Sequence[PatchOperationTypeDef]],  # (1)
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
## UpdateDeploymentRequestRequestTypeDef

```python
# UpdateDeploymentRequestRequestTypeDef definition

class UpdateDeploymentRequestRequestTypeDef(TypedDict):
    restApiId: str,
    deploymentId: str,
    patchOperations: NotRequired[Sequence[PatchOperationTypeDef]],  # (1)
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
## UpdateDocumentationPartRequestRequestTypeDef

```python
# UpdateDocumentationPartRequestRequestTypeDef definition

class UpdateDocumentationPartRequestRequestTypeDef(TypedDict):
    restApiId: str,
    documentationPartId: str,
    patchOperations: NotRequired[Sequence[PatchOperationTypeDef]],  # (1)
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
## UpdateDocumentationVersionRequestRequestTypeDef

```python
# UpdateDocumentationVersionRequestRequestTypeDef definition

class UpdateDocumentationVersionRequestRequestTypeDef(TypedDict):
    restApiId: str,
    documentationVersion: str,
    patchOperations: NotRequired[Sequence[PatchOperationTypeDef]],  # (1)
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
## UpdateDomainNameRequestRequestTypeDef

```python
# UpdateDomainNameRequestRequestTypeDef definition

class UpdateDomainNameRequestRequestTypeDef(TypedDict):
    domainName: str,
    patchOperations: NotRequired[Sequence[PatchOperationTypeDef]],  # (1)
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
## UpdateGatewayResponseRequestRequestTypeDef

```python
# UpdateGatewayResponseRequestRequestTypeDef definition

class UpdateGatewayResponseRequestRequestTypeDef(TypedDict):
    restApiId: str,
    responseType: GatewayResponseTypeType,  # (1)
    patchOperations: NotRequired[Sequence[PatchOperationTypeDef]],  # (2)
```

1. See [:material-code-brackets: GatewayResponseTypeType](./literals.md#gatewayresponsetypetype) 
2. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
## UpdateIntegrationRequestRequestTypeDef

```python
# UpdateIntegrationRequestRequestTypeDef definition

class UpdateIntegrationRequestRequestTypeDef(TypedDict):
    restApiId: str,
    resourceId: str,
    httpMethod: str,
    patchOperations: NotRequired[Sequence[PatchOperationTypeDef]],  # (1)
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
## UpdateIntegrationResponseRequestRequestTypeDef

```python
# UpdateIntegrationResponseRequestRequestTypeDef definition

class UpdateIntegrationResponseRequestRequestTypeDef(TypedDict):
    restApiId: str,
    resourceId: str,
    httpMethod: str,
    statusCode: str,
    patchOperations: NotRequired[Sequence[PatchOperationTypeDef]],  # (1)
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
## UpdateMethodRequestRequestTypeDef

```python
# UpdateMethodRequestRequestTypeDef definition

class UpdateMethodRequestRequestTypeDef(TypedDict):
    restApiId: str,
    resourceId: str,
    httpMethod: str,
    patchOperations: NotRequired[Sequence[PatchOperationTypeDef]],  # (1)
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
## UpdateMethodResponseRequestRequestTypeDef

```python
# UpdateMethodResponseRequestRequestTypeDef definition

class UpdateMethodResponseRequestRequestTypeDef(TypedDict):
    restApiId: str,
    resourceId: str,
    httpMethod: str,
    statusCode: str,
    patchOperations: NotRequired[Sequence[PatchOperationTypeDef]],  # (1)
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
## UpdateModelRequestRequestTypeDef

```python
# UpdateModelRequestRequestTypeDef definition

class UpdateModelRequestRequestTypeDef(TypedDict):
    restApiId: str,
    modelName: str,
    patchOperations: NotRequired[Sequence[PatchOperationTypeDef]],  # (1)
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
## UpdateRequestValidatorRequestRequestTypeDef

```python
# UpdateRequestValidatorRequestRequestTypeDef definition

class UpdateRequestValidatorRequestRequestTypeDef(TypedDict):
    restApiId: str,
    requestValidatorId: str,
    patchOperations: NotRequired[Sequence[PatchOperationTypeDef]],  # (1)
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
## UpdateResourceRequestRequestTypeDef

```python
# UpdateResourceRequestRequestTypeDef definition

class UpdateResourceRequestRequestTypeDef(TypedDict):
    restApiId: str,
    resourceId: str,
    patchOperations: NotRequired[Sequence[PatchOperationTypeDef]],  # (1)
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
## UpdateRestApiRequestRequestTypeDef

```python
# UpdateRestApiRequestRequestTypeDef definition

class UpdateRestApiRequestRequestTypeDef(TypedDict):
    restApiId: str,
    patchOperations: NotRequired[Sequence[PatchOperationTypeDef]],  # (1)
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
## UpdateStageRequestRequestTypeDef

```python
# UpdateStageRequestRequestTypeDef definition

class UpdateStageRequestRequestTypeDef(TypedDict):
    restApiId: str,
    stageName: str,
    patchOperations: NotRequired[Sequence[PatchOperationTypeDef]],  # (1)
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
## UpdateUsagePlanRequestRequestTypeDef

```python
# UpdateUsagePlanRequestRequestTypeDef definition

class UpdateUsagePlanRequestRequestTypeDef(TypedDict):
    usagePlanId: str,
    patchOperations: NotRequired[Sequence[PatchOperationTypeDef]],  # (1)
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
## UpdateUsageRequestRequestTypeDef

```python
# UpdateUsageRequestRequestTypeDef definition

class UpdateUsageRequestRequestTypeDef(TypedDict):
    usagePlanId: str,
    keyId: str,
    patchOperations: NotRequired[Sequence[PatchOperationTypeDef]],  # (1)
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
## UpdateVpcLinkRequestRequestTypeDef

```python
# UpdateVpcLinkRequestRequestTypeDef definition

class UpdateVpcLinkRequestRequestTypeDef(TypedDict):
    vpcLinkId: str,
    patchOperations: NotRequired[Sequence[PatchOperationTypeDef]],  # (1)
```

1. See [:material-code-braces: PatchOperationTypeDef](./type_defs.md#patchoperationtypedef) 
## RequestValidatorsTypeDef

```python
# RequestValidatorsTypeDef definition

class RequestValidatorsTypeDef(TypedDict):
    position: str,
    items: List[RequestValidatorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RequestValidatorTypeDef](./type_defs.md#requestvalidatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SdkTypeResponseTypeDef

```python
# SdkTypeResponseTypeDef definition

class SdkTypeResponseTypeDef(TypedDict):
    id: str,
    friendlyName: str,
    description: str,
    configurationProperties: List[SdkConfigurationPropertyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SdkConfigurationPropertyTypeDef](./type_defs.md#sdkconfigurationpropertytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SdkTypeTypeDef

```python
# SdkTypeTypeDef definition

class SdkTypeTypeDef(TypedDict):
    id: NotRequired[str],
    friendlyName: NotRequired[str],
    description: NotRequired[str],
    configurationProperties: NotRequired[List[SdkConfigurationPropertyTypeDef]],  # (1)
```

1. See [:material-code-braces: SdkConfigurationPropertyTypeDef](./type_defs.md#sdkconfigurationpropertytypedef) 
## UsagePlanKeysTypeDef

```python
# UsagePlanKeysTypeDef definition

class UsagePlanKeysTypeDef(TypedDict):
    position: str,
    items: List[UsagePlanKeyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UsagePlanKeyTypeDef](./type_defs.md#usageplankeytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VpcLinksTypeDef

```python
# VpcLinksTypeDef definition

class VpcLinksTypeDef(TypedDict):
    position: str,
    items: List[VpcLinkTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VpcLinkTypeDef](./type_defs.md#vpclinktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UsagePlanResponseTypeDef

```python
# UsagePlanResponseTypeDef definition

class UsagePlanResponseTypeDef(TypedDict):
    id: str,
    name: str,
    description: str,
    apiStages: List[ApiStageOutputTypeDef],  # (1)
    throttle: ThrottleSettingsTypeDef,  # (2)
    quota: QuotaSettingsTypeDef,  # (3)
    productCode: str,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ApiStageOutputTypeDef](./type_defs.md#apistageoutputtypedef) 
2. See [:material-code-braces: ThrottleSettingsTypeDef](./type_defs.md#throttlesettingstypedef) 
3. See [:material-code-braces: QuotaSettingsTypeDef](./type_defs.md#quotasettingstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UsagePlanTypeDef

```python
# UsagePlanTypeDef definition

class UsagePlanTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    apiStages: NotRequired[List[ApiStageOutputTypeDef]],  # (1)
    throttle: NotRequired[ThrottleSettingsTypeDef],  # (2)
    quota: NotRequired[QuotaSettingsTypeDef],  # (3)
    productCode: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: ApiStageOutputTypeDef](./type_defs.md#apistageoutputtypedef) 
2. See [:material-code-braces: ThrottleSettingsTypeDef](./type_defs.md#throttlesettingstypedef) 
3. See [:material-code-braces: QuotaSettingsTypeDef](./type_defs.md#quotasettingstypedef) 
## DocumentationPartsTypeDef

```python
# DocumentationPartsTypeDef definition

class DocumentationPartsTypeDef(TypedDict):
    position: str,
    items: List[DocumentationPartTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DocumentationPartTypeDef](./type_defs.md#documentationparttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeploymentsTypeDef

```python
# DeploymentsTypeDef definition

class DeploymentsTypeDef(TypedDict):
    position: str,
    items: List[DeploymentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeploymentTypeDef](./type_defs.md#deploymenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestApisTypeDef

```python
# RestApisTypeDef definition

class RestApisTypeDef(TypedDict):
    position: str,
    items: List[RestApiTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RestApiTypeDef](./type_defs.md#restapitypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DomainNamesTypeDef

```python
# DomainNamesTypeDef definition

class DomainNamesTypeDef(TypedDict):
    position: str,
    items: List[DomainNameTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainNameTypeDef](./type_defs.md#domainnametypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MethodExtraResponseTypeDef

```python
# MethodExtraResponseTypeDef definition

class MethodExtraResponseTypeDef(TypedDict):
    httpMethod: str,
    authorizationType: str,
    authorizerId: str,
    apiKeyRequired: bool,
    requestValidatorId: str,
    operationName: str,
    requestParameters: Dict[str, bool],
    requestModels: Dict[str, str],
    methodResponses: Dict[str, MethodResponseTypeDef],  # (1)
    methodIntegration: IntegrationTypeDef,  # (2)
    authorizationScopes: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: MethodResponseTypeDef](./type_defs.md#methodresponsetypedef) 
2. See [:material-code-braces: IntegrationTypeDef](./type_defs.md#integrationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MethodTypeDef

```python
# MethodTypeDef definition

class MethodTypeDef(TypedDict):
    httpMethod: NotRequired[str],
    authorizationType: NotRequired[str],
    authorizerId: NotRequired[str],
    apiKeyRequired: NotRequired[bool],
    requestValidatorId: NotRequired[str],
    operationName: NotRequired[str],
    requestParameters: NotRequired[Dict[str, bool]],
    requestModels: NotRequired[Dict[str, str]],
    methodResponses: NotRequired[Dict[str, MethodResponseTypeDef]],  # (1)
    methodIntegration: NotRequired[IntegrationTypeDef],  # (2)
    authorizationScopes: NotRequired[List[str]],
```

1. See [:material-code-braces: MethodResponseTypeDef](./type_defs.md#methodresponsetypedef) 
2. See [:material-code-braces: IntegrationTypeDef](./type_defs.md#integrationtypedef) 
## StagesTypeDef

```python
# StagesTypeDef definition

class StagesTypeDef(TypedDict):
    item: List[StageTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StageTypeDef](./type_defs.md#stagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SdkTypesTypeDef

```python
# SdkTypesTypeDef definition

class SdkTypesTypeDef(TypedDict):
    position: str,
    items: List[SdkTypeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SdkTypeTypeDef](./type_defs.md#sdktypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UsagePlansTypeDef

```python
# UsagePlansTypeDef definition

class UsagePlansTypeDef(TypedDict):
    position: str,
    items: List[UsagePlanTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UsagePlanTypeDef](./type_defs.md#usageplantypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUsagePlanRequestRequestTypeDef

```python
# CreateUsagePlanRequestRequestTypeDef definition

class CreateUsagePlanRequestRequestTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    apiStages: NotRequired[Sequence[ApiStageUnionTypeDef]],  # (1)
    throttle: NotRequired[ThrottleSettingsTypeDef],  # (2)
    quota: NotRequired[QuotaSettingsTypeDef],  # (3)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ApiStageTypeDef](./type_defs.md#apistagetypedef) [:material-code-braces: ApiStageOutputTypeDef](./type_defs.md#apistageoutputtypedef) 
2. See [:material-code-braces: ThrottleSettingsTypeDef](./type_defs.md#throttlesettingstypedef) 
3. See [:material-code-braces: QuotaSettingsTypeDef](./type_defs.md#quotasettingstypedef) 
## ResourceResponseTypeDef

```python
# ResourceResponseTypeDef definition

class ResourceResponseTypeDef(TypedDict):
    id: str,
    parentId: str,
    pathPart: str,
    path: str,
    resourceMethods: Dict[str, MethodTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MethodTypeDef](./type_defs.md#methodtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResourceTypeDef

```python
# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    id: NotRequired[str],
    parentId: NotRequired[str],
    pathPart: NotRequired[str],
    path: NotRequired[str],
    resourceMethods: NotRequired[Dict[str, MethodTypeDef]],  # (1)
```

1. See [:material-code-braces: MethodTypeDef](./type_defs.md#methodtypedef) 
## ResourcesTypeDef

```python
# ResourcesTypeDef definition

class ResourcesTypeDef(TypedDict):
    position: str,
    items: List[ResourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
