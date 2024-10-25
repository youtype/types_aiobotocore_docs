# Type definitions

> [Index](../README.md) > [ApiGatewayV2](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ApiGatewayV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
    type annotations stubs module [types-aiobotocore-apigatewayv2](https://pypi.org/project/types-aiobotocore-apigatewayv2/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## DomainNameConfigurationUnionTypeDef

```python
# DomainNameConfigurationUnionTypeDef definition

DomainNameConfigurationUnionTypeDef = Union[
    DomainNameConfigurationTypeDef,  # (1)
    DomainNameConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DomainNameConfigurationTypeDef](./type_defs.md#domainnameconfigurationtypedef) 
2. See [:material-code-braces: DomainNameConfigurationOutputTypeDef](./type_defs.md#domainnameconfigurationoutputtypedef) 



## AccessLogSettingsTypeDef

```python
# AccessLogSettingsTypeDef definition

class AccessLogSettingsTypeDef(TypedDict):
    DestinationArn: NotRequired[str],
    Format: NotRequired[str],
```

## ApiMappingTypeDef

```python
# ApiMappingTypeDef definition

class ApiMappingTypeDef(TypedDict):
    ApiId: str,
    Stage: str,
    ApiMappingId: NotRequired[str],
    ApiMappingKey: NotRequired[str],
```

## CorsOutputTypeDef

```python
# CorsOutputTypeDef definition

class CorsOutputTypeDef(TypedDict):
    AllowCredentials: NotRequired[bool],
    AllowHeaders: NotRequired[List[str]],
    AllowMethods: NotRequired[List[str]],
    AllowOrigins: NotRequired[List[str]],
    ExposeHeaders: NotRequired[List[str]],
    MaxAge: NotRequired[int],
```

## JWTConfigurationOutputTypeDef

```python
# JWTConfigurationOutputTypeDef definition

class JWTConfigurationOutputTypeDef(TypedDict):
    Audience: NotRequired[List[str]],
    Issuer: NotRequired[str],
```

## CorsTypeDef

```python
# CorsTypeDef definition

class CorsTypeDef(TypedDict):
    AllowCredentials: NotRequired[bool],
    AllowHeaders: NotRequired[Sequence[str]],
    AllowMethods: NotRequired[Sequence[str]],
    AllowOrigins: NotRequired[Sequence[str]],
    ExposeHeaders: NotRequired[Sequence[str]],
    MaxAge: NotRequired[int],
```

## CreateApiMappingRequestRequestTypeDef

```python
# CreateApiMappingRequestRequestTypeDef definition

class CreateApiMappingRequestRequestTypeDef(TypedDict):
    ApiId: str,
    DomainName: str,
    Stage: str,
    ApiMappingKey: NotRequired[str],
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

## JWTConfigurationTypeDef

```python
# JWTConfigurationTypeDef definition

class JWTConfigurationTypeDef(TypedDict):
    Audience: NotRequired[Sequence[str]],
    Issuer: NotRequired[str],
```

## CreateDeploymentRequestRequestTypeDef

```python
# CreateDeploymentRequestRequestTypeDef definition

class CreateDeploymentRequestRequestTypeDef(TypedDict):
    ApiId: str,
    Description: NotRequired[str],
    StageName: NotRequired[str],
```

## MutualTlsAuthenticationInputTypeDef

```python
# MutualTlsAuthenticationInputTypeDef definition

class MutualTlsAuthenticationInputTypeDef(TypedDict):
    TruststoreUri: NotRequired[str],
    TruststoreVersion: NotRequired[str],
```

## DomainNameConfigurationOutputTypeDef

```python
# DomainNameConfigurationOutputTypeDef definition

class DomainNameConfigurationOutputTypeDef(TypedDict):
    ApiGatewayDomainName: NotRequired[str],
    CertificateArn: NotRequired[str],
    CertificateName: NotRequired[str],
    CertificateUploadDate: NotRequired[datetime],
    DomainNameStatus: NotRequired[DomainNameStatusType],  # (1)
    DomainNameStatusMessage: NotRequired[str],
    EndpointType: NotRequired[EndpointTypeType],  # (2)
    HostedZoneId: NotRequired[str],
    SecurityPolicy: NotRequired[SecurityPolicyType],  # (3)
    OwnershipVerificationCertificateArn: NotRequired[str],
```

1. See [:material-code-brackets: DomainNameStatusType](./literals.md#domainnamestatustype) 
2. See [:material-code-brackets: EndpointTypeType](./literals.md#endpointtypetype) 
3. See [:material-code-brackets: SecurityPolicyType](./literals.md#securitypolicytype) 
## MutualTlsAuthenticationTypeDef

```python
# MutualTlsAuthenticationTypeDef definition

class MutualTlsAuthenticationTypeDef(TypedDict):
    TruststoreUri: NotRequired[str],
    TruststoreVersion: NotRequired[str],
    TruststoreWarnings: NotRequired[List[str]],
```

## TlsConfigInputTypeDef

```python
# TlsConfigInputTypeDef definition

class TlsConfigInputTypeDef(TypedDict):
    ServerNameToVerify: NotRequired[str],
```

## CreateIntegrationResponseRequestRequestTypeDef

```python
# CreateIntegrationResponseRequestRequestTypeDef definition

class CreateIntegrationResponseRequestRequestTypeDef(TypedDict):
    ApiId: str,
    IntegrationId: str,
    IntegrationResponseKey: str,
    ContentHandlingStrategy: NotRequired[ContentHandlingStrategyType],  # (1)
    ResponseParameters: NotRequired[Mapping[str, str]],
    ResponseTemplates: NotRequired[Mapping[str, str]],
    TemplateSelectionExpression: NotRequired[str],
```

1. See [:material-code-brackets: ContentHandlingStrategyType](./literals.md#contenthandlingstrategytype) 
## TlsConfigTypeDef

```python
# TlsConfigTypeDef definition

class TlsConfigTypeDef(TypedDict):
    ServerNameToVerify: NotRequired[str],
```

## CreateModelRequestRequestTypeDef

```python
# CreateModelRequestRequestTypeDef definition

class CreateModelRequestRequestTypeDef(TypedDict):
    ApiId: str,
    Name: str,
    Schema: str,
    ContentType: NotRequired[str],
    Description: NotRequired[str],
```

## ParameterConstraintsTypeDef

```python
# ParameterConstraintsTypeDef definition

class ParameterConstraintsTypeDef(TypedDict):
    Required: NotRequired[bool],
```

## RouteSettingsTypeDef

```python
# RouteSettingsTypeDef definition

class RouteSettingsTypeDef(TypedDict):
    DataTraceEnabled: NotRequired[bool],
    DetailedMetricsEnabled: NotRequired[bool],
    LoggingLevel: NotRequired[LoggingLevelType],  # (1)
    ThrottlingBurstLimit: NotRequired[int],
    ThrottlingRateLimit: NotRequired[float],
```

1. See [:material-code-brackets: LoggingLevelType](./literals.md#loggingleveltype) 
## CreateVpcLinkRequestRequestTypeDef

```python
# CreateVpcLinkRequestRequestTypeDef definition

class CreateVpcLinkRequestRequestTypeDef(TypedDict):
    Name: str,
    SubnetIds: Sequence[str],
    SecurityGroupIds: NotRequired[Sequence[str]],
    Tags: NotRequired[Mapping[str, str]],
```

## DeleteAccessLogSettingsRequestRequestTypeDef

```python
# DeleteAccessLogSettingsRequestRequestTypeDef definition

class DeleteAccessLogSettingsRequestRequestTypeDef(TypedDict):
    ApiId: str,
    StageName: str,
```

## DeleteApiMappingRequestRequestTypeDef

```python
# DeleteApiMappingRequestRequestTypeDef definition

class DeleteApiMappingRequestRequestTypeDef(TypedDict):
    ApiMappingId: str,
    DomainName: str,
```

## DeleteApiRequestRequestTypeDef

```python
# DeleteApiRequestRequestTypeDef definition

class DeleteApiRequestRequestTypeDef(TypedDict):
    ApiId: str,
```

## DeleteAuthorizerRequestRequestTypeDef

```python
# DeleteAuthorizerRequestRequestTypeDef definition

class DeleteAuthorizerRequestRequestTypeDef(TypedDict):
    ApiId: str,
    AuthorizerId: str,
```

## DeleteCorsConfigurationRequestRequestTypeDef

```python
# DeleteCorsConfigurationRequestRequestTypeDef definition

class DeleteCorsConfigurationRequestRequestTypeDef(TypedDict):
    ApiId: str,
```

## DeleteDeploymentRequestRequestTypeDef

```python
# DeleteDeploymentRequestRequestTypeDef definition

class DeleteDeploymentRequestRequestTypeDef(TypedDict):
    ApiId: str,
    DeploymentId: str,
```

## DeleteDomainNameRequestRequestTypeDef

```python
# DeleteDomainNameRequestRequestTypeDef definition

class DeleteDomainNameRequestRequestTypeDef(TypedDict):
    DomainName: str,
```

## DeleteIntegrationRequestRequestTypeDef

```python
# DeleteIntegrationRequestRequestTypeDef definition

class DeleteIntegrationRequestRequestTypeDef(TypedDict):
    ApiId: str,
    IntegrationId: str,
```

## DeleteIntegrationResponseRequestRequestTypeDef

```python
# DeleteIntegrationResponseRequestRequestTypeDef definition

class DeleteIntegrationResponseRequestRequestTypeDef(TypedDict):
    ApiId: str,
    IntegrationId: str,
    IntegrationResponseId: str,
```

## DeleteModelRequestRequestTypeDef

```python
# DeleteModelRequestRequestTypeDef definition

class DeleteModelRequestRequestTypeDef(TypedDict):
    ApiId: str,
    ModelId: str,
```

## DeleteRouteRequestParameterRequestRequestTypeDef

```python
# DeleteRouteRequestParameterRequestRequestTypeDef definition

class DeleteRouteRequestParameterRequestRequestTypeDef(TypedDict):
    ApiId: str,
    RequestParameterKey: str,
    RouteId: str,
```

## DeleteRouteRequestRequestTypeDef

```python
# DeleteRouteRequestRequestTypeDef definition

class DeleteRouteRequestRequestTypeDef(TypedDict):
    ApiId: str,
    RouteId: str,
```

## DeleteRouteResponseRequestRequestTypeDef

```python
# DeleteRouteResponseRequestRequestTypeDef definition

class DeleteRouteResponseRequestRequestTypeDef(TypedDict):
    ApiId: str,
    RouteId: str,
    RouteResponseId: str,
```

## DeleteRouteSettingsRequestRequestTypeDef

```python
# DeleteRouteSettingsRequestRequestTypeDef definition

class DeleteRouteSettingsRequestRequestTypeDef(TypedDict):
    ApiId: str,
    RouteKey: str,
    StageName: str,
```

## DeleteStageRequestRequestTypeDef

```python
# DeleteStageRequestRequestTypeDef definition

class DeleteStageRequestRequestTypeDef(TypedDict):
    ApiId: str,
    StageName: str,
```

## DeleteVpcLinkRequestRequestTypeDef

```python
# DeleteVpcLinkRequestRequestTypeDef definition

class DeleteVpcLinkRequestRequestTypeDef(TypedDict):
    VpcLinkId: str,
```

## DeploymentTypeDef

```python
# DeploymentTypeDef definition

class DeploymentTypeDef(TypedDict):
    AutoDeployed: NotRequired[bool],
    CreatedDate: NotRequired[datetime],
    DeploymentId: NotRequired[str],
    DeploymentStatus: NotRequired[DeploymentStatusType],  # (1)
    DeploymentStatusMessage: NotRequired[str],
    Description: NotRequired[str],
```

1. See [:material-code-brackets: DeploymentStatusType](./literals.md#deploymentstatustype) 
## ExportApiRequestRequestTypeDef

```python
# ExportApiRequestRequestTypeDef definition

class ExportApiRequestRequestTypeDef(TypedDict):
    ApiId: str,
    OutputType: JSONYAMLType,  # (1)
    Specification: OAS30Type,  # (2)
    ExportVersion: NotRequired[str],
    IncludeExtensions: NotRequired[bool],
    StageName: NotRequired[str],
```

1. See [:material-code-brackets: JSONYAMLType](./literals.md#jsonyamltype) 
2. See [:material-code-brackets: OAS30Type](./literals.md#oas30type) 
## GetApiMappingRequestRequestTypeDef

```python
# GetApiMappingRequestRequestTypeDef definition

class GetApiMappingRequestRequestTypeDef(TypedDict):
    ApiMappingId: str,
    DomainName: str,
```

## GetApiMappingsRequestRequestTypeDef

```python
# GetApiMappingsRequestRequestTypeDef definition

class GetApiMappingsRequestRequestTypeDef(TypedDict):
    DomainName: str,
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## GetApiRequestRequestTypeDef

```python
# GetApiRequestRequestTypeDef definition

class GetApiRequestRequestTypeDef(TypedDict):
    ApiId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetApisRequestRequestTypeDef

```python
# GetApisRequestRequestTypeDef definition

class GetApisRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## GetAuthorizerRequestRequestTypeDef

```python
# GetAuthorizerRequestRequestTypeDef definition

class GetAuthorizerRequestRequestTypeDef(TypedDict):
    ApiId: str,
    AuthorizerId: str,
```

## GetAuthorizersRequestRequestTypeDef

```python
# GetAuthorizersRequestRequestTypeDef definition

class GetAuthorizersRequestRequestTypeDef(TypedDict):
    ApiId: str,
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## GetDeploymentRequestRequestTypeDef

```python
# GetDeploymentRequestRequestTypeDef definition

class GetDeploymentRequestRequestTypeDef(TypedDict):
    ApiId: str,
    DeploymentId: str,
```

## GetDeploymentsRequestRequestTypeDef

```python
# GetDeploymentsRequestRequestTypeDef definition

class GetDeploymentsRequestRequestTypeDef(TypedDict):
    ApiId: str,
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## GetDomainNameRequestRequestTypeDef

```python
# GetDomainNameRequestRequestTypeDef definition

class GetDomainNameRequestRequestTypeDef(TypedDict):
    DomainName: str,
```

## GetDomainNamesRequestRequestTypeDef

```python
# GetDomainNamesRequestRequestTypeDef definition

class GetDomainNamesRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## GetIntegrationRequestRequestTypeDef

```python
# GetIntegrationRequestRequestTypeDef definition

class GetIntegrationRequestRequestTypeDef(TypedDict):
    ApiId: str,
    IntegrationId: str,
```

## GetIntegrationResponseRequestRequestTypeDef

```python
# GetIntegrationResponseRequestRequestTypeDef definition

class GetIntegrationResponseRequestRequestTypeDef(TypedDict):
    ApiId: str,
    IntegrationId: str,
    IntegrationResponseId: str,
```

## GetIntegrationResponsesRequestRequestTypeDef

```python
# GetIntegrationResponsesRequestRequestTypeDef definition

class GetIntegrationResponsesRequestRequestTypeDef(TypedDict):
    ApiId: str,
    IntegrationId: str,
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## IntegrationResponseTypeDef

```python
# IntegrationResponseTypeDef definition

class IntegrationResponseTypeDef(TypedDict):
    IntegrationResponseKey: str,
    ContentHandlingStrategy: NotRequired[ContentHandlingStrategyType],  # (1)
    IntegrationResponseId: NotRequired[str],
    ResponseParameters: NotRequired[Dict[str, str]],
    ResponseTemplates: NotRequired[Dict[str, str]],
    TemplateSelectionExpression: NotRequired[str],
```

1. See [:material-code-brackets: ContentHandlingStrategyType](./literals.md#contenthandlingstrategytype) 
## GetIntegrationsRequestRequestTypeDef

```python
# GetIntegrationsRequestRequestTypeDef definition

class GetIntegrationsRequestRequestTypeDef(TypedDict):
    ApiId: str,
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## GetModelRequestRequestTypeDef

```python
# GetModelRequestRequestTypeDef definition

class GetModelRequestRequestTypeDef(TypedDict):
    ApiId: str,
    ModelId: str,
```

## GetModelTemplateRequestRequestTypeDef

```python
# GetModelTemplateRequestRequestTypeDef definition

class GetModelTemplateRequestRequestTypeDef(TypedDict):
    ApiId: str,
    ModelId: str,
```

## GetModelsRequestRequestTypeDef

```python
# GetModelsRequestRequestTypeDef definition

class GetModelsRequestRequestTypeDef(TypedDict):
    ApiId: str,
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## ModelTypeDef

```python
# ModelTypeDef definition

class ModelTypeDef(TypedDict):
    Name: str,
    ContentType: NotRequired[str],
    Description: NotRequired[str],
    ModelId: NotRequired[str],
    Schema: NotRequired[str],
```

## GetRouteRequestRequestTypeDef

```python
# GetRouteRequestRequestTypeDef definition

class GetRouteRequestRequestTypeDef(TypedDict):
    ApiId: str,
    RouteId: str,
```

## GetRouteResponseRequestRequestTypeDef

```python
# GetRouteResponseRequestRequestTypeDef definition

class GetRouteResponseRequestRequestTypeDef(TypedDict):
    ApiId: str,
    RouteId: str,
    RouteResponseId: str,
```

## GetRouteResponsesRequestRequestTypeDef

```python
# GetRouteResponsesRequestRequestTypeDef definition

class GetRouteResponsesRequestRequestTypeDef(TypedDict):
    ApiId: str,
    RouteId: str,
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## GetRoutesRequestRequestTypeDef

```python
# GetRoutesRequestRequestTypeDef definition

class GetRoutesRequestRequestTypeDef(TypedDict):
    ApiId: str,
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## GetStageRequestRequestTypeDef

```python
# GetStageRequestRequestTypeDef definition

class GetStageRequestRequestTypeDef(TypedDict):
    ApiId: str,
    StageName: str,
```

## GetStagesRequestRequestTypeDef

```python
# GetStagesRequestRequestTypeDef definition

class GetStagesRequestRequestTypeDef(TypedDict):
    ApiId: str,
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## GetTagsRequestRequestTypeDef

```python
# GetTagsRequestRequestTypeDef definition

class GetTagsRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## GetVpcLinkRequestRequestTypeDef

```python
# GetVpcLinkRequestRequestTypeDef definition

class GetVpcLinkRequestRequestTypeDef(TypedDict):
    VpcLinkId: str,
```

## GetVpcLinksRequestRequestTypeDef

```python
# GetVpcLinksRequestRequestTypeDef definition

class GetVpcLinksRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## VpcLinkTypeDef

```python
# VpcLinkTypeDef definition

class VpcLinkTypeDef(TypedDict):
    Name: str,
    SecurityGroupIds: List[str],
    SubnetIds: List[str],
    VpcLinkId: str,
    CreatedDate: NotRequired[datetime],
    Tags: NotRequired[Dict[str, str]],
    VpcLinkStatus: NotRequired[VpcLinkStatusType],  # (1)
    VpcLinkStatusMessage: NotRequired[str],
    VpcLinkVersion: NotRequired[VpcLinkVersionType],  # (2)
```

1. See [:material-code-brackets: VpcLinkStatusType](./literals.md#vpclinkstatustype) 
2. See [:material-code-brackets: VpcLinkVersionType](./literals.md#vpclinkversiontype) 
## ImportApiRequestRequestTypeDef

```python
# ImportApiRequestRequestTypeDef definition

class ImportApiRequestRequestTypeDef(TypedDict):
    Body: str,
    Basepath: NotRequired[str],
    FailOnWarnings: NotRequired[bool],
```

## ReimportApiRequestRequestTypeDef

```python
# ReimportApiRequestRequestTypeDef definition

class ReimportApiRequestRequestTypeDef(TypedDict):
    ApiId: str,
    Body: str,
    Basepath: NotRequired[str],
    FailOnWarnings: NotRequired[bool],
```

## ResetAuthorizersCacheRequestRequestTypeDef

```python
# ResetAuthorizersCacheRequestRequestTypeDef definition

class ResetAuthorizersCacheRequestRequestTypeDef(TypedDict):
    ApiId: str,
    StageName: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: NotRequired[Mapping[str, str]],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateApiMappingRequestRequestTypeDef

```python
# UpdateApiMappingRequestRequestTypeDef definition

class UpdateApiMappingRequestRequestTypeDef(TypedDict):
    ApiId: str,
    ApiMappingId: str,
    DomainName: str,
    ApiMappingKey: NotRequired[str],
    Stage: NotRequired[str],
```

## UpdateDeploymentRequestRequestTypeDef

```python
# UpdateDeploymentRequestRequestTypeDef definition

class UpdateDeploymentRequestRequestTypeDef(TypedDict):
    ApiId: str,
    DeploymentId: str,
    Description: NotRequired[str],
```

## UpdateIntegrationResponseRequestRequestTypeDef

```python
# UpdateIntegrationResponseRequestRequestTypeDef definition

class UpdateIntegrationResponseRequestRequestTypeDef(TypedDict):
    ApiId: str,
    IntegrationId: str,
    IntegrationResponseId: str,
    ContentHandlingStrategy: NotRequired[ContentHandlingStrategyType],  # (1)
    IntegrationResponseKey: NotRequired[str],
    ResponseParameters: NotRequired[Mapping[str, str]],
    ResponseTemplates: NotRequired[Mapping[str, str]],
    TemplateSelectionExpression: NotRequired[str],
```

1. See [:material-code-brackets: ContentHandlingStrategyType](./literals.md#contenthandlingstrategytype) 
## UpdateModelRequestRequestTypeDef

```python
# UpdateModelRequestRequestTypeDef definition

class UpdateModelRequestRequestTypeDef(TypedDict):
    ApiId: str,
    ModelId: str,
    ContentType: NotRequired[str],
    Description: NotRequired[str],
    Name: NotRequired[str],
    Schema: NotRequired[str],
```

## UpdateVpcLinkRequestRequestTypeDef

```python
# UpdateVpcLinkRequestRequestTypeDef definition

class UpdateVpcLinkRequestRequestTypeDef(TypedDict):
    VpcLinkId: str,
    Name: NotRequired[str],
```

## ApiTypeDef

```python
# ApiTypeDef definition

class ApiTypeDef(TypedDict):
    Name: str,
    ProtocolType: ProtocolTypeType,  # (2)
    RouteSelectionExpression: str,
    ApiEndpoint: NotRequired[str],
    ApiGatewayManaged: NotRequired[bool],
    ApiId: NotRequired[str],
    ApiKeySelectionExpression: NotRequired[str],
    CorsConfiguration: NotRequired[CorsOutputTypeDef],  # (1)
    CreatedDate: NotRequired[datetime],
    Description: NotRequired[str],
    DisableSchemaValidation: NotRequired[bool],
    DisableExecuteApiEndpoint: NotRequired[bool],
    ImportInfo: NotRequired[List[str]],
    Tags: NotRequired[Dict[str, str]],
    Version: NotRequired[str],
    Warnings: NotRequired[List[str]],
```

1. See [:material-code-braces: CorsOutputTypeDef](./type_defs.md#corsoutputtypedef) 
2. See [:material-code-brackets: ProtocolTypeType](./literals.md#protocoltypetype) 
## AuthorizerTypeDef

```python
# AuthorizerTypeDef definition

class AuthorizerTypeDef(TypedDict):
    Name: str,
    AuthorizerCredentialsArn: NotRequired[str],
    AuthorizerId: NotRequired[str],
    AuthorizerPayloadFormatVersion: NotRequired[str],
    AuthorizerResultTtlInSeconds: NotRequired[int],
    AuthorizerType: NotRequired[AuthorizerTypeType],  # (1)
    AuthorizerUri: NotRequired[str],
    EnableSimpleResponses: NotRequired[bool],
    IdentitySource: NotRequired[List[str]],
    IdentityValidationExpression: NotRequired[str],
    JwtConfiguration: NotRequired[JWTConfigurationOutputTypeDef],  # (2)
```

1. See [:material-code-brackets: AuthorizerTypeType](./literals.md#authorizertypetype) 
2. See [:material-code-braces: JWTConfigurationOutputTypeDef](./type_defs.md#jwtconfigurationoutputtypedef) 
## CreateApiRequestRequestTypeDef

```python
# CreateApiRequestRequestTypeDef definition

class CreateApiRequestRequestTypeDef(TypedDict):
    Name: str,
    ProtocolType: ProtocolTypeType,  # (1)
    ApiKeySelectionExpression: NotRequired[str],
    CorsConfiguration: NotRequired[CorsTypeDef],  # (2)
    CredentialsArn: NotRequired[str],
    Description: NotRequired[str],
    DisableSchemaValidation: NotRequired[bool],
    DisableExecuteApiEndpoint: NotRequired[bool],
    RouteKey: NotRequired[str],
    RouteSelectionExpression: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    Target: NotRequired[str],
    Version: NotRequired[str],
```

1. See [:material-code-brackets: ProtocolTypeType](./literals.md#protocoltypetype) 
2. See [:material-code-braces: CorsTypeDef](./type_defs.md#corstypedef) 
## UpdateApiRequestRequestTypeDef

```python
# UpdateApiRequestRequestTypeDef definition

class UpdateApiRequestRequestTypeDef(TypedDict):
    ApiId: str,
    ApiKeySelectionExpression: NotRequired[str],
    CorsConfiguration: NotRequired[CorsTypeDef],  # (1)
    CredentialsArn: NotRequired[str],
    Description: NotRequired[str],
    DisableSchemaValidation: NotRequired[bool],
    DisableExecuteApiEndpoint: NotRequired[bool],
    Name: NotRequired[str],
    RouteKey: NotRequired[str],
    RouteSelectionExpression: NotRequired[str],
    Target: NotRequired[str],
    Version: NotRequired[str],
```

1. See [:material-code-braces: CorsTypeDef](./type_defs.md#corstypedef) 
## CreateApiMappingResponseTypeDef

```python
# CreateApiMappingResponseTypeDef definition

class CreateApiMappingResponseTypeDef(TypedDict):
    ApiId: str,
    ApiMappingId: str,
    ApiMappingKey: str,
    Stage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateApiResponseTypeDef

```python
# CreateApiResponseTypeDef definition

class CreateApiResponseTypeDef(TypedDict):
    ApiEndpoint: str,
    ApiGatewayManaged: bool,
    ApiId: str,
    ApiKeySelectionExpression: str,
    CorsConfiguration: CorsOutputTypeDef,  # (1)
    CreatedDate: datetime,
    Description: str,
    DisableSchemaValidation: bool,
    DisableExecuteApiEndpoint: bool,
    ImportInfo: List[str],
    Name: str,
    ProtocolType: ProtocolTypeType,  # (2)
    RouteSelectionExpression: str,
    Tags: Dict[str, str],
    Version: str,
    Warnings: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: CorsOutputTypeDef](./type_defs.md#corsoutputtypedef) 
2. See [:material-code-brackets: ProtocolTypeType](./literals.md#protocoltypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAuthorizerResponseTypeDef

```python
# CreateAuthorizerResponseTypeDef definition

class CreateAuthorizerResponseTypeDef(TypedDict):
    AuthorizerCredentialsArn: str,
    AuthorizerId: str,
    AuthorizerPayloadFormatVersion: str,
    AuthorizerResultTtlInSeconds: int,
    AuthorizerType: AuthorizerTypeType,  # (1)
    AuthorizerUri: str,
    EnableSimpleResponses: bool,
    IdentitySource: List[str],
    IdentityValidationExpression: str,
    JwtConfiguration: JWTConfigurationOutputTypeDef,  # (2)
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: AuthorizerTypeType](./literals.md#authorizertypetype) 
2. See [:material-code-braces: JWTConfigurationOutputTypeDef](./type_defs.md#jwtconfigurationoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDeploymentResponseTypeDef

```python
# CreateDeploymentResponseTypeDef definition

class CreateDeploymentResponseTypeDef(TypedDict):
    AutoDeployed: bool,
    CreatedDate: datetime,
    DeploymentId: str,
    DeploymentStatus: DeploymentStatusType,  # (1)
    DeploymentStatusMessage: str,
    Description: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DeploymentStatusType](./literals.md#deploymentstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateIntegrationResponseResponseTypeDef

```python
# CreateIntegrationResponseResponseTypeDef definition

class CreateIntegrationResponseResponseTypeDef(TypedDict):
    ContentHandlingStrategy: ContentHandlingStrategyType,  # (1)
    IntegrationResponseId: str,
    IntegrationResponseKey: str,
    ResponseParameters: Dict[str, str],
    ResponseTemplates: Dict[str, str],
    TemplateSelectionExpression: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ContentHandlingStrategyType](./literals.md#contenthandlingstrategytype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateModelResponseTypeDef

```python
# CreateModelResponseTypeDef definition

class CreateModelResponseTypeDef(TypedDict):
    ContentType: str,
    Description: str,
    ModelId: str,
    Name: str,
    Schema: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateVpcLinkResponseTypeDef

```python
# CreateVpcLinkResponseTypeDef definition

class CreateVpcLinkResponseTypeDef(TypedDict):
    CreatedDate: datetime,
    Name: str,
    SecurityGroupIds: List[str],
    SubnetIds: List[str],
    Tags: Dict[str, str],
    VpcLinkId: str,
    VpcLinkStatus: VpcLinkStatusType,  # (1)
    VpcLinkStatusMessage: str,
    VpcLinkVersion: VpcLinkVersionType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: VpcLinkStatusType](./literals.md#vpclinkstatustype) 
2. See [:material-code-brackets: VpcLinkVersionType](./literals.md#vpclinkversiontype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportApiResponseTypeDef

```python
# ExportApiResponseTypeDef definition

class ExportApiResponseTypeDef(TypedDict):
    body: StreamingBody,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetApiMappingResponseTypeDef

```python
# GetApiMappingResponseTypeDef definition

class GetApiMappingResponseTypeDef(TypedDict):
    ApiId: str,
    ApiMappingId: str,
    ApiMappingKey: str,
    Stage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetApiMappingsResponseTypeDef

```python
# GetApiMappingsResponseTypeDef definition

class GetApiMappingsResponseTypeDef(TypedDict):
    Items: List[ApiMappingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ApiMappingTypeDef](./type_defs.md#apimappingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetApiResponseTypeDef

```python
# GetApiResponseTypeDef definition

class GetApiResponseTypeDef(TypedDict):
    ApiEndpoint: str,
    ApiGatewayManaged: bool,
    ApiId: str,
    ApiKeySelectionExpression: str,
    CorsConfiguration: CorsOutputTypeDef,  # (1)
    CreatedDate: datetime,
    Description: str,
    DisableSchemaValidation: bool,
    DisableExecuteApiEndpoint: bool,
    ImportInfo: List[str],
    Name: str,
    ProtocolType: ProtocolTypeType,  # (2)
    RouteSelectionExpression: str,
    Tags: Dict[str, str],
    Version: str,
    Warnings: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: CorsOutputTypeDef](./type_defs.md#corsoutputtypedef) 
2. See [:material-code-brackets: ProtocolTypeType](./literals.md#protocoltypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAuthorizerResponseTypeDef

```python
# GetAuthorizerResponseTypeDef definition

class GetAuthorizerResponseTypeDef(TypedDict):
    AuthorizerCredentialsArn: str,
    AuthorizerId: str,
    AuthorizerPayloadFormatVersion: str,
    AuthorizerResultTtlInSeconds: int,
    AuthorizerType: AuthorizerTypeType,  # (1)
    AuthorizerUri: str,
    EnableSimpleResponses: bool,
    IdentitySource: List[str],
    IdentityValidationExpression: str,
    JwtConfiguration: JWTConfigurationOutputTypeDef,  # (2)
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: AuthorizerTypeType](./literals.md#authorizertypetype) 
2. See [:material-code-braces: JWTConfigurationOutputTypeDef](./type_defs.md#jwtconfigurationoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDeploymentResponseTypeDef

```python
# GetDeploymentResponseTypeDef definition

class GetDeploymentResponseTypeDef(TypedDict):
    AutoDeployed: bool,
    CreatedDate: datetime,
    DeploymentId: str,
    DeploymentStatus: DeploymentStatusType,  # (1)
    DeploymentStatusMessage: str,
    Description: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DeploymentStatusType](./literals.md#deploymentstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIntegrationResponseResponseTypeDef

```python
# GetIntegrationResponseResponseTypeDef definition

class GetIntegrationResponseResponseTypeDef(TypedDict):
    ContentHandlingStrategy: ContentHandlingStrategyType,  # (1)
    IntegrationResponseId: str,
    IntegrationResponseKey: str,
    ResponseParameters: Dict[str, str],
    ResponseTemplates: Dict[str, str],
    TemplateSelectionExpression: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ContentHandlingStrategyType](./literals.md#contenthandlingstrategytype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetModelResponseTypeDef

```python
# GetModelResponseTypeDef definition

class GetModelResponseTypeDef(TypedDict):
    ContentType: str,
    Description: str,
    ModelId: str,
    Name: str,
    Schema: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetModelTemplateResponseTypeDef

```python
# GetModelTemplateResponseTypeDef definition

class GetModelTemplateResponseTypeDef(TypedDict):
    Value: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTagsResponseTypeDef

```python
# GetTagsResponseTypeDef definition

class GetTagsResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetVpcLinkResponseTypeDef

```python
# GetVpcLinkResponseTypeDef definition

class GetVpcLinkResponseTypeDef(TypedDict):
    CreatedDate: datetime,
    Name: str,
    SecurityGroupIds: List[str],
    SubnetIds: List[str],
    Tags: Dict[str, str],
    VpcLinkId: str,
    VpcLinkStatus: VpcLinkStatusType,  # (1)
    VpcLinkStatusMessage: str,
    VpcLinkVersion: VpcLinkVersionType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: VpcLinkStatusType](./literals.md#vpclinkstatustype) 
2. See [:material-code-brackets: VpcLinkVersionType](./literals.md#vpclinkversiontype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportApiResponseTypeDef

```python
# ImportApiResponseTypeDef definition

class ImportApiResponseTypeDef(TypedDict):
    ApiEndpoint: str,
    ApiGatewayManaged: bool,
    ApiId: str,
    ApiKeySelectionExpression: str,
    CorsConfiguration: CorsOutputTypeDef,  # (1)
    CreatedDate: datetime,
    Description: str,
    DisableSchemaValidation: bool,
    DisableExecuteApiEndpoint: bool,
    ImportInfo: List[str],
    Name: str,
    ProtocolType: ProtocolTypeType,  # (2)
    RouteSelectionExpression: str,
    Tags: Dict[str, str],
    Version: str,
    Warnings: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: CorsOutputTypeDef](./type_defs.md#corsoutputtypedef) 
2. See [:material-code-brackets: ProtocolTypeType](./literals.md#protocoltypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReimportApiResponseTypeDef

```python
# ReimportApiResponseTypeDef definition

class ReimportApiResponseTypeDef(TypedDict):
    ApiEndpoint: str,
    ApiGatewayManaged: bool,
    ApiId: str,
    ApiKeySelectionExpression: str,
    CorsConfiguration: CorsOutputTypeDef,  # (1)
    CreatedDate: datetime,
    Description: str,
    DisableSchemaValidation: bool,
    DisableExecuteApiEndpoint: bool,
    ImportInfo: List[str],
    Name: str,
    ProtocolType: ProtocolTypeType,  # (2)
    RouteSelectionExpression: str,
    Tags: Dict[str, str],
    Version: str,
    Warnings: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: CorsOutputTypeDef](./type_defs.md#corsoutputtypedef) 
2. See [:material-code-brackets: ProtocolTypeType](./literals.md#protocoltypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateApiMappingResponseTypeDef

```python
# UpdateApiMappingResponseTypeDef definition

class UpdateApiMappingResponseTypeDef(TypedDict):
    ApiId: str,
    ApiMappingId: str,
    ApiMappingKey: str,
    Stage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateApiResponseTypeDef

```python
# UpdateApiResponseTypeDef definition

class UpdateApiResponseTypeDef(TypedDict):
    ApiEndpoint: str,
    ApiGatewayManaged: bool,
    ApiId: str,
    ApiKeySelectionExpression: str,
    CorsConfiguration: CorsOutputTypeDef,  # (1)
    CreatedDate: datetime,
    Description: str,
    DisableSchemaValidation: bool,
    DisableExecuteApiEndpoint: bool,
    ImportInfo: List[str],
    Name: str,
    ProtocolType: ProtocolTypeType,  # (2)
    RouteSelectionExpression: str,
    Tags: Dict[str, str],
    Version: str,
    Warnings: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: CorsOutputTypeDef](./type_defs.md#corsoutputtypedef) 
2. See [:material-code-brackets: ProtocolTypeType](./literals.md#protocoltypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAuthorizerResponseTypeDef

```python
# UpdateAuthorizerResponseTypeDef definition

class UpdateAuthorizerResponseTypeDef(TypedDict):
    AuthorizerCredentialsArn: str,
    AuthorizerId: str,
    AuthorizerPayloadFormatVersion: str,
    AuthorizerResultTtlInSeconds: int,
    AuthorizerType: AuthorizerTypeType,  # (1)
    AuthorizerUri: str,
    EnableSimpleResponses: bool,
    IdentitySource: List[str],
    IdentityValidationExpression: str,
    JwtConfiguration: JWTConfigurationOutputTypeDef,  # (2)
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: AuthorizerTypeType](./literals.md#authorizertypetype) 
2. See [:material-code-braces: JWTConfigurationOutputTypeDef](./type_defs.md#jwtconfigurationoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDeploymentResponseTypeDef

```python
# UpdateDeploymentResponseTypeDef definition

class UpdateDeploymentResponseTypeDef(TypedDict):
    AutoDeployed: bool,
    CreatedDate: datetime,
    DeploymentId: str,
    DeploymentStatus: DeploymentStatusType,  # (1)
    DeploymentStatusMessage: str,
    Description: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DeploymentStatusType](./literals.md#deploymentstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateIntegrationResponseResponseTypeDef

```python
# UpdateIntegrationResponseResponseTypeDef definition

class UpdateIntegrationResponseResponseTypeDef(TypedDict):
    ContentHandlingStrategy: ContentHandlingStrategyType,  # (1)
    IntegrationResponseId: str,
    IntegrationResponseKey: str,
    ResponseParameters: Dict[str, str],
    ResponseTemplates: Dict[str, str],
    TemplateSelectionExpression: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ContentHandlingStrategyType](./literals.md#contenthandlingstrategytype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateModelResponseTypeDef

```python
# UpdateModelResponseTypeDef definition

class UpdateModelResponseTypeDef(TypedDict):
    ContentType: str,
    Description: str,
    ModelId: str,
    Name: str,
    Schema: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateVpcLinkResponseTypeDef

```python
# UpdateVpcLinkResponseTypeDef definition

class UpdateVpcLinkResponseTypeDef(TypedDict):
    CreatedDate: datetime,
    Name: str,
    SecurityGroupIds: List[str],
    SubnetIds: List[str],
    Tags: Dict[str, str],
    VpcLinkId: str,
    VpcLinkStatus: VpcLinkStatusType,  # (1)
    VpcLinkStatusMessage: str,
    VpcLinkVersion: VpcLinkVersionType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: VpcLinkStatusType](./literals.md#vpclinkstatustype) 
2. See [:material-code-brackets: VpcLinkVersionType](./literals.md#vpclinkversiontype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAuthorizerRequestRequestTypeDef

```python
# CreateAuthorizerRequestRequestTypeDef definition

class CreateAuthorizerRequestRequestTypeDef(TypedDict):
    ApiId: str,
    AuthorizerType: AuthorizerTypeType,  # (1)
    IdentitySource: Sequence[str],
    Name: str,
    AuthorizerCredentialsArn: NotRequired[str],
    AuthorizerPayloadFormatVersion: NotRequired[str],
    AuthorizerResultTtlInSeconds: NotRequired[int],
    AuthorizerUri: NotRequired[str],
    EnableSimpleResponses: NotRequired[bool],
    IdentityValidationExpression: NotRequired[str],
    JwtConfiguration: NotRequired[JWTConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: AuthorizerTypeType](./literals.md#authorizertypetype) 
2. See [:material-code-braces: JWTConfigurationTypeDef](./type_defs.md#jwtconfigurationtypedef) 
## UpdateAuthorizerRequestRequestTypeDef

```python
# UpdateAuthorizerRequestRequestTypeDef definition

class UpdateAuthorizerRequestRequestTypeDef(TypedDict):
    ApiId: str,
    AuthorizerId: str,
    AuthorizerCredentialsArn: NotRequired[str],
    AuthorizerPayloadFormatVersion: NotRequired[str],
    AuthorizerResultTtlInSeconds: NotRequired[int],
    AuthorizerType: NotRequired[AuthorizerTypeType],  # (1)
    AuthorizerUri: NotRequired[str],
    EnableSimpleResponses: NotRequired[bool],
    IdentitySource: NotRequired[Sequence[str]],
    IdentityValidationExpression: NotRequired[str],
    JwtConfiguration: NotRequired[JWTConfigurationTypeDef],  # (2)
    Name: NotRequired[str],
```

1. See [:material-code-brackets: AuthorizerTypeType](./literals.md#authorizertypetype) 
2. See [:material-code-braces: JWTConfigurationTypeDef](./type_defs.md#jwtconfigurationtypedef) 
## CreateDomainNameResponseTypeDef

```python
# CreateDomainNameResponseTypeDef definition

class CreateDomainNameResponseTypeDef(TypedDict):
    ApiMappingSelectionExpression: str,
    DomainName: str,
    DomainNameConfigurations: List[DomainNameConfigurationOutputTypeDef],  # (1)
    MutualTlsAuthentication: MutualTlsAuthenticationTypeDef,  # (2)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: DomainNameConfigurationOutputTypeDef](./type_defs.md#domainnameconfigurationoutputtypedef) 
2. See [:material-code-braces: MutualTlsAuthenticationTypeDef](./type_defs.md#mutualtlsauthenticationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DomainNameTypeDef

```python
# DomainNameTypeDef definition

class DomainNameTypeDef(TypedDict):
    DomainName: str,
    ApiMappingSelectionExpression: NotRequired[str],
    DomainNameConfigurations: NotRequired[List[DomainNameConfigurationOutputTypeDef]],  # (1)
    MutualTlsAuthentication: NotRequired[MutualTlsAuthenticationTypeDef],  # (2)
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: DomainNameConfigurationOutputTypeDef](./type_defs.md#domainnameconfigurationoutputtypedef) 
2. See [:material-code-braces: MutualTlsAuthenticationTypeDef](./type_defs.md#mutualtlsauthenticationtypedef) 
## GetDomainNameResponseTypeDef

```python
# GetDomainNameResponseTypeDef definition

class GetDomainNameResponseTypeDef(TypedDict):
    ApiMappingSelectionExpression: str,
    DomainName: str,
    DomainNameConfigurations: List[DomainNameConfigurationOutputTypeDef],  # (1)
    MutualTlsAuthentication: MutualTlsAuthenticationTypeDef,  # (2)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: DomainNameConfigurationOutputTypeDef](./type_defs.md#domainnameconfigurationoutputtypedef) 
2. See [:material-code-braces: MutualTlsAuthenticationTypeDef](./type_defs.md#mutualtlsauthenticationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDomainNameResponseTypeDef

```python
# UpdateDomainNameResponseTypeDef definition

class UpdateDomainNameResponseTypeDef(TypedDict):
    ApiMappingSelectionExpression: str,
    DomainName: str,
    DomainNameConfigurations: List[DomainNameConfigurationOutputTypeDef],  # (1)
    MutualTlsAuthentication: MutualTlsAuthenticationTypeDef,  # (2)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: DomainNameConfigurationOutputTypeDef](./type_defs.md#domainnameconfigurationoutputtypedef) 
2. See [:material-code-braces: MutualTlsAuthenticationTypeDef](./type_defs.md#mutualtlsauthenticationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateIntegrationRequestRequestTypeDef

```python
# CreateIntegrationRequestRequestTypeDef definition

class CreateIntegrationRequestRequestTypeDef(TypedDict):
    ApiId: str,
    IntegrationType: IntegrationTypeType,  # (1)
    ConnectionId: NotRequired[str],
    ConnectionType: NotRequired[ConnectionTypeType],  # (2)
    ContentHandlingStrategy: NotRequired[ContentHandlingStrategyType],  # (3)
    CredentialsArn: NotRequired[str],
    Description: NotRequired[str],
    IntegrationMethod: NotRequired[str],
    IntegrationSubtype: NotRequired[str],
    IntegrationUri: NotRequired[str],
    PassthroughBehavior: NotRequired[PassthroughBehaviorType],  # (4)
    PayloadFormatVersion: NotRequired[str],
    RequestParameters: NotRequired[Mapping[str, str]],
    RequestTemplates: NotRequired[Mapping[str, str]],
    ResponseParameters: NotRequired[Mapping[str, Mapping[str, str]]],
    TemplateSelectionExpression: NotRequired[str],
    TimeoutInMillis: NotRequired[int],
    TlsConfig: NotRequired[TlsConfigInputTypeDef],  # (5)
```

1. See [:material-code-brackets: IntegrationTypeType](./literals.md#integrationtypetype) 
2. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
3. See [:material-code-brackets: ContentHandlingStrategyType](./literals.md#contenthandlingstrategytype) 
4. See [:material-code-brackets: PassthroughBehaviorType](./literals.md#passthroughbehaviortype) 
5. See [:material-code-braces: TlsConfigInputTypeDef](./type_defs.md#tlsconfiginputtypedef) 
## UpdateIntegrationRequestRequestTypeDef

```python
# UpdateIntegrationRequestRequestTypeDef definition

class UpdateIntegrationRequestRequestTypeDef(TypedDict):
    ApiId: str,
    IntegrationId: str,
    ConnectionId: NotRequired[str],
    ConnectionType: NotRequired[ConnectionTypeType],  # (1)
    ContentHandlingStrategy: NotRequired[ContentHandlingStrategyType],  # (2)
    CredentialsArn: NotRequired[str],
    Description: NotRequired[str],
    IntegrationMethod: NotRequired[str],
    IntegrationSubtype: NotRequired[str],
    IntegrationType: NotRequired[IntegrationTypeType],  # (3)
    IntegrationUri: NotRequired[str],
    PassthroughBehavior: NotRequired[PassthroughBehaviorType],  # (4)
    PayloadFormatVersion: NotRequired[str],
    RequestParameters: NotRequired[Mapping[str, str]],
    RequestTemplates: NotRequired[Mapping[str, str]],
    ResponseParameters: NotRequired[Mapping[str, Mapping[str, str]]],
    TemplateSelectionExpression: NotRequired[str],
    TimeoutInMillis: NotRequired[int],
    TlsConfig: NotRequired[TlsConfigInputTypeDef],  # (5)
```

1. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
2. See [:material-code-brackets: ContentHandlingStrategyType](./literals.md#contenthandlingstrategytype) 
3. See [:material-code-brackets: IntegrationTypeType](./literals.md#integrationtypetype) 
4. See [:material-code-brackets: PassthroughBehaviorType](./literals.md#passthroughbehaviortype) 
5. See [:material-code-braces: TlsConfigInputTypeDef](./type_defs.md#tlsconfiginputtypedef) 
## CreateIntegrationResultTypeDef

```python
# CreateIntegrationResultTypeDef definition

class CreateIntegrationResultTypeDef(TypedDict):
    ApiGatewayManaged: bool,
    ConnectionId: str,
    ConnectionType: ConnectionTypeType,  # (1)
    ContentHandlingStrategy: ContentHandlingStrategyType,  # (2)
    CredentialsArn: str,
    Description: str,
    IntegrationId: str,
    IntegrationMethod: str,
    IntegrationResponseSelectionExpression: str,
    IntegrationSubtype: str,
    IntegrationType: IntegrationTypeType,  # (3)
    IntegrationUri: str,
    PassthroughBehavior: PassthroughBehaviorType,  # (4)
    PayloadFormatVersion: str,
    RequestParameters: Dict[str, str],
    RequestTemplates: Dict[str, str],
    ResponseParameters: Dict[str, Dict[str, str]],
    TemplateSelectionExpression: str,
    TimeoutInMillis: int,
    TlsConfig: TlsConfigTypeDef,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
2. See [:material-code-brackets: ContentHandlingStrategyType](./literals.md#contenthandlingstrategytype) 
3. See [:material-code-brackets: IntegrationTypeType](./literals.md#integrationtypetype) 
4. See [:material-code-brackets: PassthroughBehaviorType](./literals.md#passthroughbehaviortype) 
5. See [:material-code-braces: TlsConfigTypeDef](./type_defs.md#tlsconfigtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIntegrationResultTypeDef

```python
# GetIntegrationResultTypeDef definition

class GetIntegrationResultTypeDef(TypedDict):
    ApiGatewayManaged: bool,
    ConnectionId: str,
    ConnectionType: ConnectionTypeType,  # (1)
    ContentHandlingStrategy: ContentHandlingStrategyType,  # (2)
    CredentialsArn: str,
    Description: str,
    IntegrationId: str,
    IntegrationMethod: str,
    IntegrationResponseSelectionExpression: str,
    IntegrationSubtype: str,
    IntegrationType: IntegrationTypeType,  # (3)
    IntegrationUri: str,
    PassthroughBehavior: PassthroughBehaviorType,  # (4)
    PayloadFormatVersion: str,
    RequestParameters: Dict[str, str],
    RequestTemplates: Dict[str, str],
    ResponseParameters: Dict[str, Dict[str, str]],
    TemplateSelectionExpression: str,
    TimeoutInMillis: int,
    TlsConfig: TlsConfigTypeDef,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
2. See [:material-code-brackets: ContentHandlingStrategyType](./literals.md#contenthandlingstrategytype) 
3. See [:material-code-brackets: IntegrationTypeType](./literals.md#integrationtypetype) 
4. See [:material-code-brackets: PassthroughBehaviorType](./literals.md#passthroughbehaviortype) 
5. See [:material-code-braces: TlsConfigTypeDef](./type_defs.md#tlsconfigtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IntegrationTypeDef

```python
# IntegrationTypeDef definition

class IntegrationTypeDef(TypedDict):
    ApiGatewayManaged: NotRequired[bool],
    ConnectionId: NotRequired[str],
    ConnectionType: NotRequired[ConnectionTypeType],  # (1)
    ContentHandlingStrategy: NotRequired[ContentHandlingStrategyType],  # (2)
    CredentialsArn: NotRequired[str],
    Description: NotRequired[str],
    IntegrationId: NotRequired[str],
    IntegrationMethod: NotRequired[str],
    IntegrationResponseSelectionExpression: NotRequired[str],
    IntegrationSubtype: NotRequired[str],
    IntegrationType: NotRequired[IntegrationTypeType],  # (3)
    IntegrationUri: NotRequired[str],
    PassthroughBehavior: NotRequired[PassthroughBehaviorType],  # (4)
    PayloadFormatVersion: NotRequired[str],
    RequestParameters: NotRequired[Dict[str, str]],
    RequestTemplates: NotRequired[Dict[str, str]],
    ResponseParameters: NotRequired[Dict[str, Dict[str, str]]],
    TemplateSelectionExpression: NotRequired[str],
    TimeoutInMillis: NotRequired[int],
    TlsConfig: NotRequired[TlsConfigTypeDef],  # (5)
```

1. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
2. See [:material-code-brackets: ContentHandlingStrategyType](./literals.md#contenthandlingstrategytype) 
3. See [:material-code-brackets: IntegrationTypeType](./literals.md#integrationtypetype) 
4. See [:material-code-brackets: PassthroughBehaviorType](./literals.md#passthroughbehaviortype) 
5. See [:material-code-braces: TlsConfigTypeDef](./type_defs.md#tlsconfigtypedef) 
## UpdateIntegrationResultTypeDef

```python
# UpdateIntegrationResultTypeDef definition

class UpdateIntegrationResultTypeDef(TypedDict):
    ApiGatewayManaged: bool,
    ConnectionId: str,
    ConnectionType: ConnectionTypeType,  # (1)
    ContentHandlingStrategy: ContentHandlingStrategyType,  # (2)
    CredentialsArn: str,
    Description: str,
    IntegrationId: str,
    IntegrationMethod: str,
    IntegrationResponseSelectionExpression: str,
    IntegrationSubtype: str,
    IntegrationType: IntegrationTypeType,  # (3)
    IntegrationUri: str,
    PassthroughBehavior: PassthroughBehaviorType,  # (4)
    PayloadFormatVersion: str,
    RequestParameters: Dict[str, str],
    RequestTemplates: Dict[str, str],
    ResponseParameters: Dict[str, Dict[str, str]],
    TemplateSelectionExpression: str,
    TimeoutInMillis: int,
    TlsConfig: TlsConfigTypeDef,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
2. See [:material-code-brackets: ContentHandlingStrategyType](./literals.md#contenthandlingstrategytype) 
3. See [:material-code-brackets: IntegrationTypeType](./literals.md#integrationtypetype) 
4. See [:material-code-brackets: PassthroughBehaviorType](./literals.md#passthroughbehaviortype) 
5. See [:material-code-braces: TlsConfigTypeDef](./type_defs.md#tlsconfigtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRouteRequestRequestTypeDef

```python
# CreateRouteRequestRequestTypeDef definition

class CreateRouteRequestRequestTypeDef(TypedDict):
    ApiId: str,
    RouteKey: str,
    ApiKeyRequired: NotRequired[bool],
    AuthorizationScopes: NotRequired[Sequence[str]],
    AuthorizationType: NotRequired[AuthorizationTypeType],  # (1)
    AuthorizerId: NotRequired[str],
    ModelSelectionExpression: NotRequired[str],
    OperationName: NotRequired[str],
    RequestModels: NotRequired[Mapping[str, str]],
    RequestParameters: NotRequired[Mapping[str, ParameterConstraintsTypeDef]],  # (2)
    RouteResponseSelectionExpression: NotRequired[str],
    Target: NotRequired[str],
```

1. See [:material-code-brackets: AuthorizationTypeType](./literals.md#authorizationtypetype) 
2. See [:material-code-braces: ParameterConstraintsTypeDef](./type_defs.md#parameterconstraintstypedef) 
## CreateRouteResponseRequestRequestTypeDef

```python
# CreateRouteResponseRequestRequestTypeDef definition

class CreateRouteResponseRequestRequestTypeDef(TypedDict):
    ApiId: str,
    RouteId: str,
    RouteResponseKey: str,
    ModelSelectionExpression: NotRequired[str],
    ResponseModels: NotRequired[Mapping[str, str]],
    ResponseParameters: NotRequired[Mapping[str, ParameterConstraintsTypeDef]],  # (1)
```

1. See [:material-code-braces: ParameterConstraintsTypeDef](./type_defs.md#parameterconstraintstypedef) 
## CreateRouteResponseResponseTypeDef

```python
# CreateRouteResponseResponseTypeDef definition

class CreateRouteResponseResponseTypeDef(TypedDict):
    ModelSelectionExpression: str,
    ResponseModels: Dict[str, str],
    ResponseParameters: Dict[str, ParameterConstraintsTypeDef],  # (1)
    RouteResponseId: str,
    RouteResponseKey: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ParameterConstraintsTypeDef](./type_defs.md#parameterconstraintstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRouteResultTypeDef

```python
# CreateRouteResultTypeDef definition

class CreateRouteResultTypeDef(TypedDict):
    ApiGatewayManaged: bool,
    ApiKeyRequired: bool,
    AuthorizationScopes: List[str],
    AuthorizationType: AuthorizationTypeType,  # (1)
    AuthorizerId: str,
    ModelSelectionExpression: str,
    OperationName: str,
    RequestModels: Dict[str, str],
    RequestParameters: Dict[str, ParameterConstraintsTypeDef],  # (2)
    RouteId: str,
    RouteKey: str,
    RouteResponseSelectionExpression: str,
    Target: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: AuthorizationTypeType](./literals.md#authorizationtypetype) 
2. See [:material-code-braces: ParameterConstraintsTypeDef](./type_defs.md#parameterconstraintstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRouteResponseResponseTypeDef

```python
# GetRouteResponseResponseTypeDef definition

class GetRouteResponseResponseTypeDef(TypedDict):
    ModelSelectionExpression: str,
    ResponseModels: Dict[str, str],
    ResponseParameters: Dict[str, ParameterConstraintsTypeDef],  # (1)
    RouteResponseId: str,
    RouteResponseKey: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ParameterConstraintsTypeDef](./type_defs.md#parameterconstraintstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRouteResultTypeDef

```python
# GetRouteResultTypeDef definition

class GetRouteResultTypeDef(TypedDict):
    ApiGatewayManaged: bool,
    ApiKeyRequired: bool,
    AuthorizationScopes: List[str],
    AuthorizationType: AuthorizationTypeType,  # (1)
    AuthorizerId: str,
    ModelSelectionExpression: str,
    OperationName: str,
    RequestModels: Dict[str, str],
    RequestParameters: Dict[str, ParameterConstraintsTypeDef],  # (2)
    RouteId: str,
    RouteKey: str,
    RouteResponseSelectionExpression: str,
    Target: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: AuthorizationTypeType](./literals.md#authorizationtypetype) 
2. See [:material-code-braces: ParameterConstraintsTypeDef](./type_defs.md#parameterconstraintstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RouteResponseTypeDef

```python
# RouteResponseTypeDef definition

class RouteResponseTypeDef(TypedDict):
    RouteResponseKey: str,
    ModelSelectionExpression: NotRequired[str],
    ResponseModels: NotRequired[Dict[str, str]],
    ResponseParameters: NotRequired[Dict[str, ParameterConstraintsTypeDef]],  # (1)
    RouteResponseId: NotRequired[str],
```

1. See [:material-code-braces: ParameterConstraintsTypeDef](./type_defs.md#parameterconstraintstypedef) 
## RouteTypeDef

```python
# RouteTypeDef definition

class RouteTypeDef(TypedDict):
    RouteKey: str,
    ApiGatewayManaged: NotRequired[bool],
    ApiKeyRequired: NotRequired[bool],
    AuthorizationScopes: NotRequired[List[str]],
    AuthorizationType: NotRequired[AuthorizationTypeType],  # (1)
    AuthorizerId: NotRequired[str],
    ModelSelectionExpression: NotRequired[str],
    OperationName: NotRequired[str],
    RequestModels: NotRequired[Dict[str, str]],
    RequestParameters: NotRequired[Dict[str, ParameterConstraintsTypeDef]],  # (2)
    RouteId: NotRequired[str],
    RouteResponseSelectionExpression: NotRequired[str],
    Target: NotRequired[str],
```

1. See [:material-code-brackets: AuthorizationTypeType](./literals.md#authorizationtypetype) 
2. See [:material-code-braces: ParameterConstraintsTypeDef](./type_defs.md#parameterconstraintstypedef) 
## UpdateRouteRequestRequestTypeDef

```python
# UpdateRouteRequestRequestTypeDef definition

class UpdateRouteRequestRequestTypeDef(TypedDict):
    ApiId: str,
    RouteId: str,
    ApiKeyRequired: NotRequired[bool],
    AuthorizationScopes: NotRequired[Sequence[str]],
    AuthorizationType: NotRequired[AuthorizationTypeType],  # (1)
    AuthorizerId: NotRequired[str],
    ModelSelectionExpression: NotRequired[str],
    OperationName: NotRequired[str],
    RequestModels: NotRequired[Mapping[str, str]],
    RequestParameters: NotRequired[Mapping[str, ParameterConstraintsTypeDef]],  # (2)
    RouteKey: NotRequired[str],
    RouteResponseSelectionExpression: NotRequired[str],
    Target: NotRequired[str],
```

1. See [:material-code-brackets: AuthorizationTypeType](./literals.md#authorizationtypetype) 
2. See [:material-code-braces: ParameterConstraintsTypeDef](./type_defs.md#parameterconstraintstypedef) 
## UpdateRouteResponseRequestRequestTypeDef

```python
# UpdateRouteResponseRequestRequestTypeDef definition

class UpdateRouteResponseRequestRequestTypeDef(TypedDict):
    ApiId: str,
    RouteId: str,
    RouteResponseId: str,
    ModelSelectionExpression: NotRequired[str],
    ResponseModels: NotRequired[Mapping[str, str]],
    ResponseParameters: NotRequired[Mapping[str, ParameterConstraintsTypeDef]],  # (1)
    RouteResponseKey: NotRequired[str],
```

1. See [:material-code-braces: ParameterConstraintsTypeDef](./type_defs.md#parameterconstraintstypedef) 
## UpdateRouteResponseResponseTypeDef

```python
# UpdateRouteResponseResponseTypeDef definition

class UpdateRouteResponseResponseTypeDef(TypedDict):
    ModelSelectionExpression: str,
    ResponseModels: Dict[str, str],
    ResponseParameters: Dict[str, ParameterConstraintsTypeDef],  # (1)
    RouteResponseId: str,
    RouteResponseKey: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ParameterConstraintsTypeDef](./type_defs.md#parameterconstraintstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRouteResultTypeDef

```python
# UpdateRouteResultTypeDef definition

class UpdateRouteResultTypeDef(TypedDict):
    ApiGatewayManaged: bool,
    ApiKeyRequired: bool,
    AuthorizationScopes: List[str],
    AuthorizationType: AuthorizationTypeType,  # (1)
    AuthorizerId: str,
    ModelSelectionExpression: str,
    OperationName: str,
    RequestModels: Dict[str, str],
    RequestParameters: Dict[str, ParameterConstraintsTypeDef],  # (2)
    RouteId: str,
    RouteKey: str,
    RouteResponseSelectionExpression: str,
    Target: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: AuthorizationTypeType](./literals.md#authorizationtypetype) 
2. See [:material-code-braces: ParameterConstraintsTypeDef](./type_defs.md#parameterconstraintstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStageRequestRequestTypeDef

```python
# CreateStageRequestRequestTypeDef definition

class CreateStageRequestRequestTypeDef(TypedDict):
    ApiId: str,
    StageName: str,
    AccessLogSettings: NotRequired[AccessLogSettingsTypeDef],  # (1)
    AutoDeploy: NotRequired[bool],
    ClientCertificateId: NotRequired[str],
    DefaultRouteSettings: NotRequired[RouteSettingsTypeDef],  # (2)
    DeploymentId: NotRequired[str],
    Description: NotRequired[str],
    RouteSettings: NotRequired[Mapping[str, RouteSettingsTypeDef]],  # (3)
    StageVariables: NotRequired[Mapping[str, str]],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AccessLogSettingsTypeDef](./type_defs.md#accesslogsettingstypedef) 
2. See [:material-code-braces: RouteSettingsTypeDef](./type_defs.md#routesettingstypedef) 
3. See [:material-code-braces: RouteSettingsTypeDef](./type_defs.md#routesettingstypedef) 
## CreateStageResponseTypeDef

```python
# CreateStageResponseTypeDef definition

class CreateStageResponseTypeDef(TypedDict):
    AccessLogSettings: AccessLogSettingsTypeDef,  # (1)
    ApiGatewayManaged: bool,
    AutoDeploy: bool,
    ClientCertificateId: str,
    CreatedDate: datetime,
    DefaultRouteSettings: RouteSettingsTypeDef,  # (2)
    DeploymentId: str,
    Description: str,
    LastDeploymentStatusMessage: str,
    LastUpdatedDate: datetime,
    RouteSettings: Dict[str, RouteSettingsTypeDef],  # (3)
    StageName: str,
    StageVariables: Dict[str, str],
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: AccessLogSettingsTypeDef](./type_defs.md#accesslogsettingstypedef) 
2. See [:material-code-braces: RouteSettingsTypeDef](./type_defs.md#routesettingstypedef) 
3. See [:material-code-braces: RouteSettingsTypeDef](./type_defs.md#routesettingstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetStageResponseTypeDef

```python
# GetStageResponseTypeDef definition

class GetStageResponseTypeDef(TypedDict):
    AccessLogSettings: AccessLogSettingsTypeDef,  # (1)
    ApiGatewayManaged: bool,
    AutoDeploy: bool,
    ClientCertificateId: str,
    CreatedDate: datetime,
    DefaultRouteSettings: RouteSettingsTypeDef,  # (2)
    DeploymentId: str,
    Description: str,
    LastDeploymentStatusMessage: str,
    LastUpdatedDate: datetime,
    RouteSettings: Dict[str, RouteSettingsTypeDef],  # (3)
    StageName: str,
    StageVariables: Dict[str, str],
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: AccessLogSettingsTypeDef](./type_defs.md#accesslogsettingstypedef) 
2. See [:material-code-braces: RouteSettingsTypeDef](./type_defs.md#routesettingstypedef) 
3. See [:material-code-braces: RouteSettingsTypeDef](./type_defs.md#routesettingstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StageTypeDef

```python
# StageTypeDef definition

class StageTypeDef(TypedDict):
    StageName: str,
    AccessLogSettings: NotRequired[AccessLogSettingsTypeDef],  # (1)
    ApiGatewayManaged: NotRequired[bool],
    AutoDeploy: NotRequired[bool],
    ClientCertificateId: NotRequired[str],
    CreatedDate: NotRequired[datetime],
    DefaultRouteSettings: NotRequired[RouteSettingsTypeDef],  # (2)
    DeploymentId: NotRequired[str],
    Description: NotRequired[str],
    LastDeploymentStatusMessage: NotRequired[str],
    LastUpdatedDate: NotRequired[datetime],
    RouteSettings: NotRequired[Dict[str, RouteSettingsTypeDef]],  # (3)
    StageVariables: NotRequired[Dict[str, str]],
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: AccessLogSettingsTypeDef](./type_defs.md#accesslogsettingstypedef) 
2. See [:material-code-braces: RouteSettingsTypeDef](./type_defs.md#routesettingstypedef) 
3. See [:material-code-braces: RouteSettingsTypeDef](./type_defs.md#routesettingstypedef) 
## UpdateStageRequestRequestTypeDef

```python
# UpdateStageRequestRequestTypeDef definition

class UpdateStageRequestRequestTypeDef(TypedDict):
    ApiId: str,
    StageName: str,
    AccessLogSettings: NotRequired[AccessLogSettingsTypeDef],  # (1)
    AutoDeploy: NotRequired[bool],
    ClientCertificateId: NotRequired[str],
    DefaultRouteSettings: NotRequired[RouteSettingsTypeDef],  # (2)
    DeploymentId: NotRequired[str],
    Description: NotRequired[str],
    RouteSettings: NotRequired[Mapping[str, RouteSettingsTypeDef]],  # (3)
    StageVariables: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AccessLogSettingsTypeDef](./type_defs.md#accesslogsettingstypedef) 
2. See [:material-code-braces: RouteSettingsTypeDef](./type_defs.md#routesettingstypedef) 
3. See [:material-code-braces: RouteSettingsTypeDef](./type_defs.md#routesettingstypedef) 
## UpdateStageResponseTypeDef

```python
# UpdateStageResponseTypeDef definition

class UpdateStageResponseTypeDef(TypedDict):
    AccessLogSettings: AccessLogSettingsTypeDef,  # (1)
    ApiGatewayManaged: bool,
    AutoDeploy: bool,
    ClientCertificateId: str,
    CreatedDate: datetime,
    DefaultRouteSettings: RouteSettingsTypeDef,  # (2)
    DeploymentId: str,
    Description: str,
    LastDeploymentStatusMessage: str,
    LastUpdatedDate: datetime,
    RouteSettings: Dict[str, RouteSettingsTypeDef],  # (3)
    StageName: str,
    StageVariables: Dict[str, str],
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: AccessLogSettingsTypeDef](./type_defs.md#accesslogsettingstypedef) 
2. See [:material-code-braces: RouteSettingsTypeDef](./type_defs.md#routesettingstypedef) 
3. See [:material-code-braces: RouteSettingsTypeDef](./type_defs.md#routesettingstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDeploymentsResponseTypeDef

```python
# GetDeploymentsResponseTypeDef definition

class GetDeploymentsResponseTypeDef(TypedDict):
    Items: List[DeploymentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DeploymentTypeDef](./type_defs.md#deploymenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DomainNameConfigurationTypeDef

```python
# DomainNameConfigurationTypeDef definition

class DomainNameConfigurationTypeDef(TypedDict):
    ApiGatewayDomainName: NotRequired[str],
    CertificateArn: NotRequired[str],
    CertificateName: NotRequired[str],
    CertificateUploadDate: NotRequired[TimestampTypeDef],
    DomainNameStatus: NotRequired[DomainNameStatusType],  # (1)
    DomainNameStatusMessage: NotRequired[str],
    EndpointType: NotRequired[EndpointTypeType],  # (2)
    HostedZoneId: NotRequired[str],
    SecurityPolicy: NotRequired[SecurityPolicyType],  # (3)
    OwnershipVerificationCertificateArn: NotRequired[str],
```

1. See [:material-code-brackets: DomainNameStatusType](./literals.md#domainnamestatustype) 
2. See [:material-code-brackets: EndpointTypeType](./literals.md#endpointtypetype) 
3. See [:material-code-brackets: SecurityPolicyType](./literals.md#securitypolicytype) 
## GetApisRequestGetApisPaginateTypeDef

```python
# GetApisRequestGetApisPaginateTypeDef definition

class GetApisRequestGetApisPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetAuthorizersRequestGetAuthorizersPaginateTypeDef

```python
# GetAuthorizersRequestGetAuthorizersPaginateTypeDef definition

class GetAuthorizersRequestGetAuthorizersPaginateTypeDef(TypedDict):
    ApiId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetDeploymentsRequestGetDeploymentsPaginateTypeDef

```python
# GetDeploymentsRequestGetDeploymentsPaginateTypeDef definition

class GetDeploymentsRequestGetDeploymentsPaginateTypeDef(TypedDict):
    ApiId: str,
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
## GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef

```python
# GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef definition

class GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef(TypedDict):
    ApiId: str,
    IntegrationId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetIntegrationsRequestGetIntegrationsPaginateTypeDef

```python
# GetIntegrationsRequestGetIntegrationsPaginateTypeDef definition

class GetIntegrationsRequestGetIntegrationsPaginateTypeDef(TypedDict):
    ApiId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetModelsRequestGetModelsPaginateTypeDef

```python
# GetModelsRequestGetModelsPaginateTypeDef definition

class GetModelsRequestGetModelsPaginateTypeDef(TypedDict):
    ApiId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef

```python
# GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef definition

class GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef(TypedDict):
    ApiId: str,
    RouteId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetRoutesRequestGetRoutesPaginateTypeDef

```python
# GetRoutesRequestGetRoutesPaginateTypeDef definition

class GetRoutesRequestGetRoutesPaginateTypeDef(TypedDict):
    ApiId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetStagesRequestGetStagesPaginateTypeDef

```python
# GetStagesRequestGetStagesPaginateTypeDef definition

class GetStagesRequestGetStagesPaginateTypeDef(TypedDict):
    ApiId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetIntegrationResponsesResponseTypeDef

```python
# GetIntegrationResponsesResponseTypeDef definition

class GetIntegrationResponsesResponseTypeDef(TypedDict):
    Items: List[IntegrationResponseTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: IntegrationResponseTypeDef](./type_defs.md#integrationresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetModelsResponseTypeDef

```python
# GetModelsResponseTypeDef definition

class GetModelsResponseTypeDef(TypedDict):
    Items: List[ModelTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ModelTypeDef](./type_defs.md#modeltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetVpcLinksResponseTypeDef

```python
# GetVpcLinksResponseTypeDef definition

class GetVpcLinksResponseTypeDef(TypedDict):
    Items: List[VpcLinkTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: VpcLinkTypeDef](./type_defs.md#vpclinktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetApisResponseTypeDef

```python
# GetApisResponseTypeDef definition

class GetApisResponseTypeDef(TypedDict):
    Items: List[ApiTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ApiTypeDef](./type_defs.md#apitypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAuthorizersResponseTypeDef

```python
# GetAuthorizersResponseTypeDef definition

class GetAuthorizersResponseTypeDef(TypedDict):
    Items: List[AuthorizerTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AuthorizerTypeDef](./type_defs.md#authorizertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDomainNamesResponseTypeDef

```python
# GetDomainNamesResponseTypeDef definition

class GetDomainNamesResponseTypeDef(TypedDict):
    Items: List[DomainNameTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DomainNameTypeDef](./type_defs.md#domainnametypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIntegrationsResponseTypeDef

```python
# GetIntegrationsResponseTypeDef definition

class GetIntegrationsResponseTypeDef(TypedDict):
    Items: List[IntegrationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: IntegrationTypeDef](./type_defs.md#integrationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRouteResponsesResponseTypeDef

```python
# GetRouteResponsesResponseTypeDef definition

class GetRouteResponsesResponseTypeDef(TypedDict):
    Items: List[RouteResponseTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RouteResponseTypeDef](./type_defs.md#routeresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRoutesResponseTypeDef

```python
# GetRoutesResponseTypeDef definition

class GetRoutesResponseTypeDef(TypedDict):
    Items: List[RouteTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RouteTypeDef](./type_defs.md#routetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetStagesResponseTypeDef

```python
# GetStagesResponseTypeDef definition

class GetStagesResponseTypeDef(TypedDict):
    Items: List[StageTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: StageTypeDef](./type_defs.md#stagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDomainNameRequestRequestTypeDef

```python
# UpdateDomainNameRequestRequestTypeDef definition

class UpdateDomainNameRequestRequestTypeDef(TypedDict):
    DomainName: str,
    DomainNameConfigurations: NotRequired[Sequence[DomainNameConfigurationTypeDef]],  # (1)
    MutualTlsAuthentication: NotRequired[MutualTlsAuthenticationInputTypeDef],  # (2)
```

1. See [:material-code-braces: DomainNameConfigurationTypeDef](./type_defs.md#domainnameconfigurationtypedef) 
2. See [:material-code-braces: MutualTlsAuthenticationInputTypeDef](./type_defs.md#mutualtlsauthenticationinputtypedef) 
## CreateDomainNameRequestRequestTypeDef

```python
# CreateDomainNameRequestRequestTypeDef definition

class CreateDomainNameRequestRequestTypeDef(TypedDict):
    DomainName: str,
    DomainNameConfigurations: NotRequired[Sequence[DomainNameConfigurationUnionTypeDef]],  # (1)
    MutualTlsAuthentication: NotRequired[MutualTlsAuthenticationInputTypeDef],  # (2)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: DomainNameConfigurationTypeDef](./type_defs.md#domainnameconfigurationtypedef) [:material-code-braces: DomainNameConfigurationOutputTypeDef](./type_defs.md#domainnameconfigurationoutputtypedef) 
2. See [:material-code-braces: MutualTlsAuthenticationInputTypeDef](./type_defs.md#mutualtlsauthenticationinputtypedef) 
