# Type definitions

> [Index](../README.md) > [ApiGatewayV2](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ApiGatewayV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#apigatewayv2)
    type annotations stubs module [types-aiobotocore-apigatewayv2](https://pypi.org/project/types-aiobotocore-apigatewayv2/).

## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_apigatewayv2.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## CorsUnionTypeDef

```python
# CorsUnionTypeDef Union usage example

from types_aiobotocore_apigatewayv2.type_defs import CorsUnionTypeDef


def get_value() -> CorsUnionTypeDef:
    return ...


# CorsUnionTypeDef definition

CorsUnionTypeDef = Union[
    CorsTypeDef,  # (1)
    CorsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CorsTypeDef](./type_defs.md#corstypedef) 
2. See [:material-code-braces: CorsOutputTypeDef](./type_defs.md#corsoutputtypedef) 

## JWTConfigurationUnionTypeDef

```python
# JWTConfigurationUnionTypeDef Union usage example

from types_aiobotocore_apigatewayv2.type_defs import JWTConfigurationUnionTypeDef


def get_value() -> JWTConfigurationUnionTypeDef:
    return ...


# JWTConfigurationUnionTypeDef definition

JWTConfigurationUnionTypeDef = Union[
    JWTConfigurationTypeDef,  # (1)
    JWTConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: JWTConfigurationTypeDef](./type_defs.md#jwtconfigurationtypedef) 
2. See [:material-code-braces: JWTConfigurationOutputTypeDef](./type_defs.md#jwtconfigurationoutputtypedef) 

## DomainNameConfigurationUnionTypeDef

```python
# DomainNameConfigurationUnionTypeDef Union usage example

from types_aiobotocore_apigatewayv2.type_defs import DomainNameConfigurationUnionTypeDef


def get_value() -> DomainNameConfigurationUnionTypeDef:
    return ...


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
# AccessLogSettingsTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import AccessLogSettingsTypeDef


def get_value() -> AccessLogSettingsTypeDef:
    return {
        "DestinationArn": ...,
    }


# AccessLogSettingsTypeDef definition

class AccessLogSettingsTypeDef(TypedDict):
    DestinationArn: NotRequired[str],
    Format: NotRequired[str],
```

## ApiMappingTypeDef

```python
# ApiMappingTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import ApiMappingTypeDef


def get_value() -> ApiMappingTypeDef:
    return {
        "ApiId": ...,
    }


# ApiMappingTypeDef definition

class ApiMappingTypeDef(TypedDict):
    ApiId: str,
    Stage: str,
    ApiMappingId: NotRequired[str],
    ApiMappingKey: NotRequired[str],
```

## CorsOutputTypeDef

```python
# CorsOutputTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import CorsOutputTypeDef


def get_value() -> CorsOutputTypeDef:
    return {
        "AllowCredentials": ...,
    }


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
# JWTConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import JWTConfigurationOutputTypeDef


def get_value() -> JWTConfigurationOutputTypeDef:
    return {
        "Audience": ...,
    }


# JWTConfigurationOutputTypeDef definition

class JWTConfigurationOutputTypeDef(TypedDict):
    Audience: NotRequired[List[str]],
    Issuer: NotRequired[str],
```

## CorsTypeDef

```python
# CorsTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import CorsTypeDef


def get_value() -> CorsTypeDef:
    return {
        "AllowCredentials": ...,
    }


# CorsTypeDef definition

class CorsTypeDef(TypedDict):
    AllowCredentials: NotRequired[bool],
    AllowHeaders: NotRequired[Sequence[str]],
    AllowMethods: NotRequired[Sequence[str]],
    AllowOrigins: NotRequired[Sequence[str]],
    ExposeHeaders: NotRequired[Sequence[str]],
    MaxAge: NotRequired[int],
```

## CreateApiMappingRequestTypeDef

```python
# CreateApiMappingRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import CreateApiMappingRequestTypeDef


def get_value() -> CreateApiMappingRequestTypeDef:
    return {
        "ApiId": ...,
    }


# CreateApiMappingRequestTypeDef definition

class CreateApiMappingRequestTypeDef(TypedDict):
    ApiId: str,
    DomainName: str,
    Stage: str,
    ApiMappingKey: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## CreateDeploymentRequestTypeDef

```python
# CreateDeploymentRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import CreateDeploymentRequestTypeDef


def get_value() -> CreateDeploymentRequestTypeDef:
    return {
        "ApiId": ...,
    }


# CreateDeploymentRequestTypeDef definition

class CreateDeploymentRequestTypeDef(TypedDict):
    ApiId: str,
    Description: NotRequired[str],
    StageName: NotRequired[str],
```

## MutualTlsAuthenticationInputTypeDef

```python
# MutualTlsAuthenticationInputTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import MutualTlsAuthenticationInputTypeDef


def get_value() -> MutualTlsAuthenticationInputTypeDef:
    return {
        "TruststoreUri": ...,
    }


# MutualTlsAuthenticationInputTypeDef definition

class MutualTlsAuthenticationInputTypeDef(TypedDict):
    TruststoreUri: NotRequired[str],
    TruststoreVersion: NotRequired[str],
```

## DomainNameConfigurationOutputTypeDef

```python
# DomainNameConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import DomainNameConfigurationOutputTypeDef


def get_value() -> DomainNameConfigurationOutputTypeDef:
    return {
        "ApiGatewayDomainName": ...,
    }


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
# MutualTlsAuthenticationTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import MutualTlsAuthenticationTypeDef


def get_value() -> MutualTlsAuthenticationTypeDef:
    return {
        "TruststoreUri": ...,
    }


# MutualTlsAuthenticationTypeDef definition

class MutualTlsAuthenticationTypeDef(TypedDict):
    TruststoreUri: NotRequired[str],
    TruststoreVersion: NotRequired[str],
    TruststoreWarnings: NotRequired[List[str]],
```

## TlsConfigInputTypeDef

```python
# TlsConfigInputTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import TlsConfigInputTypeDef


def get_value() -> TlsConfigInputTypeDef:
    return {
        "ServerNameToVerify": ...,
    }


# TlsConfigInputTypeDef definition

class TlsConfigInputTypeDef(TypedDict):
    ServerNameToVerify: NotRequired[str],
```

## CreateIntegrationResponseRequestTypeDef

```python
# CreateIntegrationResponseRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import CreateIntegrationResponseRequestTypeDef


def get_value() -> CreateIntegrationResponseRequestTypeDef:
    return {
        "ApiId": ...,
    }


# CreateIntegrationResponseRequestTypeDef definition

class CreateIntegrationResponseRequestTypeDef(TypedDict):
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
# TlsConfigTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import TlsConfigTypeDef


def get_value() -> TlsConfigTypeDef:
    return {
        "ServerNameToVerify": ...,
    }


# TlsConfigTypeDef definition

class TlsConfigTypeDef(TypedDict):
    ServerNameToVerify: NotRequired[str],
```

## CreateModelRequestTypeDef

```python
# CreateModelRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import CreateModelRequestTypeDef


def get_value() -> CreateModelRequestTypeDef:
    return {
        "ApiId": ...,
    }


# CreateModelRequestTypeDef definition

class CreateModelRequestTypeDef(TypedDict):
    ApiId: str,
    Name: str,
    Schema: str,
    ContentType: NotRequired[str],
    Description: NotRequired[str],
```

## ParameterConstraintsTypeDef

```python
# ParameterConstraintsTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import ParameterConstraintsTypeDef


def get_value() -> ParameterConstraintsTypeDef:
    return {
        "Required": ...,
    }


# ParameterConstraintsTypeDef definition

class ParameterConstraintsTypeDef(TypedDict):
    Required: NotRequired[bool],
```

## RouteSettingsTypeDef

```python
# RouteSettingsTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import RouteSettingsTypeDef


def get_value() -> RouteSettingsTypeDef:
    return {
        "DataTraceEnabled": ...,
    }


# RouteSettingsTypeDef definition

class RouteSettingsTypeDef(TypedDict):
    DataTraceEnabled: NotRequired[bool],
    DetailedMetricsEnabled: NotRequired[bool],
    LoggingLevel: NotRequired[LoggingLevelType],  # (1)
    ThrottlingBurstLimit: NotRequired[int],
    ThrottlingRateLimit: NotRequired[float],
```

1. See [:material-code-brackets: LoggingLevelType](./literals.md#loggingleveltype) 
## CreateVpcLinkRequestTypeDef

```python
# CreateVpcLinkRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import CreateVpcLinkRequestTypeDef


def get_value() -> CreateVpcLinkRequestTypeDef:
    return {
        "Name": ...,
    }


# CreateVpcLinkRequestTypeDef definition

class CreateVpcLinkRequestTypeDef(TypedDict):
    Name: str,
    SubnetIds: Sequence[str],
    SecurityGroupIds: NotRequired[Sequence[str]],
    Tags: NotRequired[Mapping[str, str]],
```

## DeleteAccessLogSettingsRequestTypeDef

```python
# DeleteAccessLogSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import DeleteAccessLogSettingsRequestTypeDef


def get_value() -> DeleteAccessLogSettingsRequestTypeDef:
    return {
        "ApiId": ...,
    }


# DeleteAccessLogSettingsRequestTypeDef definition

class DeleteAccessLogSettingsRequestTypeDef(TypedDict):
    ApiId: str,
    StageName: str,
```

## DeleteApiMappingRequestTypeDef

```python
# DeleteApiMappingRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import DeleteApiMappingRequestTypeDef


def get_value() -> DeleteApiMappingRequestTypeDef:
    return {
        "ApiMappingId": ...,
    }


# DeleteApiMappingRequestTypeDef definition

class DeleteApiMappingRequestTypeDef(TypedDict):
    ApiMappingId: str,
    DomainName: str,
```

## DeleteApiRequestTypeDef

```python
# DeleteApiRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import DeleteApiRequestTypeDef


def get_value() -> DeleteApiRequestTypeDef:
    return {
        "ApiId": ...,
    }


# DeleteApiRequestTypeDef definition

class DeleteApiRequestTypeDef(TypedDict):
    ApiId: str,
```

## DeleteAuthorizerRequestTypeDef

```python
# DeleteAuthorizerRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import DeleteAuthorizerRequestTypeDef


def get_value() -> DeleteAuthorizerRequestTypeDef:
    return {
        "ApiId": ...,
    }


# DeleteAuthorizerRequestTypeDef definition

class DeleteAuthorizerRequestTypeDef(TypedDict):
    ApiId: str,
    AuthorizerId: str,
```

## DeleteCorsConfigurationRequestTypeDef

```python
# DeleteCorsConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import DeleteCorsConfigurationRequestTypeDef


def get_value() -> DeleteCorsConfigurationRequestTypeDef:
    return {
        "ApiId": ...,
    }


# DeleteCorsConfigurationRequestTypeDef definition

class DeleteCorsConfigurationRequestTypeDef(TypedDict):
    ApiId: str,
```

## DeleteDeploymentRequestTypeDef

```python
# DeleteDeploymentRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import DeleteDeploymentRequestTypeDef


def get_value() -> DeleteDeploymentRequestTypeDef:
    return {
        "ApiId": ...,
    }


# DeleteDeploymentRequestTypeDef definition

class DeleteDeploymentRequestTypeDef(TypedDict):
    ApiId: str,
    DeploymentId: str,
```

## DeleteDomainNameRequestTypeDef

```python
# DeleteDomainNameRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import DeleteDomainNameRequestTypeDef


def get_value() -> DeleteDomainNameRequestTypeDef:
    return {
        "DomainName": ...,
    }


# DeleteDomainNameRequestTypeDef definition

class DeleteDomainNameRequestTypeDef(TypedDict):
    DomainName: str,
```

## DeleteIntegrationRequestTypeDef

```python
# DeleteIntegrationRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import DeleteIntegrationRequestTypeDef


def get_value() -> DeleteIntegrationRequestTypeDef:
    return {
        "ApiId": ...,
    }


# DeleteIntegrationRequestTypeDef definition

class DeleteIntegrationRequestTypeDef(TypedDict):
    ApiId: str,
    IntegrationId: str,
```

## DeleteIntegrationResponseRequestTypeDef

```python
# DeleteIntegrationResponseRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import DeleteIntegrationResponseRequestTypeDef


def get_value() -> DeleteIntegrationResponseRequestTypeDef:
    return {
        "ApiId": ...,
    }


# DeleteIntegrationResponseRequestTypeDef definition

class DeleteIntegrationResponseRequestTypeDef(TypedDict):
    ApiId: str,
    IntegrationId: str,
    IntegrationResponseId: str,
```

## DeleteModelRequestTypeDef

```python
# DeleteModelRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import DeleteModelRequestTypeDef


def get_value() -> DeleteModelRequestTypeDef:
    return {
        "ApiId": ...,
    }


# DeleteModelRequestTypeDef definition

class DeleteModelRequestTypeDef(TypedDict):
    ApiId: str,
    ModelId: str,
```

## DeleteRouteRequestParameterRequestTypeDef

```python
# DeleteRouteRequestParameterRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import DeleteRouteRequestParameterRequestTypeDef


def get_value() -> DeleteRouteRequestParameterRequestTypeDef:
    return {
        "ApiId": ...,
    }


# DeleteRouteRequestParameterRequestTypeDef definition

class DeleteRouteRequestParameterRequestTypeDef(TypedDict):
    ApiId: str,
    RequestParameterKey: str,
    RouteId: str,
```

## DeleteRouteRequestTypeDef

```python
# DeleteRouteRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import DeleteRouteRequestTypeDef


def get_value() -> DeleteRouteRequestTypeDef:
    return {
        "ApiId": ...,
    }


# DeleteRouteRequestTypeDef definition

class DeleteRouteRequestTypeDef(TypedDict):
    ApiId: str,
    RouteId: str,
```

## DeleteRouteResponseRequestTypeDef

```python
# DeleteRouteResponseRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import DeleteRouteResponseRequestTypeDef


def get_value() -> DeleteRouteResponseRequestTypeDef:
    return {
        "ApiId": ...,
    }


# DeleteRouteResponseRequestTypeDef definition

class DeleteRouteResponseRequestTypeDef(TypedDict):
    ApiId: str,
    RouteId: str,
    RouteResponseId: str,
```

## DeleteRouteSettingsRequestTypeDef

```python
# DeleteRouteSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import DeleteRouteSettingsRequestTypeDef


def get_value() -> DeleteRouteSettingsRequestTypeDef:
    return {
        "ApiId": ...,
    }


# DeleteRouteSettingsRequestTypeDef definition

class DeleteRouteSettingsRequestTypeDef(TypedDict):
    ApiId: str,
    RouteKey: str,
    StageName: str,
```

## DeleteStageRequestTypeDef

```python
# DeleteStageRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import DeleteStageRequestTypeDef


def get_value() -> DeleteStageRequestTypeDef:
    return {
        "ApiId": ...,
    }


# DeleteStageRequestTypeDef definition

class DeleteStageRequestTypeDef(TypedDict):
    ApiId: str,
    StageName: str,
```

## DeleteVpcLinkRequestTypeDef

```python
# DeleteVpcLinkRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import DeleteVpcLinkRequestTypeDef


def get_value() -> DeleteVpcLinkRequestTypeDef:
    return {
        "VpcLinkId": ...,
    }


# DeleteVpcLinkRequestTypeDef definition

class DeleteVpcLinkRequestTypeDef(TypedDict):
    VpcLinkId: str,
```

## DeploymentTypeDef

```python
# DeploymentTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import DeploymentTypeDef


def get_value() -> DeploymentTypeDef:
    return {
        "AutoDeployed": ...,
    }


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
## ExportApiRequestTypeDef

```python
# ExportApiRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import ExportApiRequestTypeDef


def get_value() -> ExportApiRequestTypeDef:
    return {
        "ApiId": ...,
    }


# ExportApiRequestTypeDef definition

class ExportApiRequestTypeDef(TypedDict):
    ApiId: str,
    OutputType: JSONYAMLType,  # (1)
    Specification: OAS30Type,  # (2)
    ExportVersion: NotRequired[str],
    IncludeExtensions: NotRequired[bool],
    StageName: NotRequired[str],
```

1. See [:material-code-brackets: JSONYAMLType](./literals.md#jsonyamltype) 
2. See [:material-code-brackets: OAS30Type](./literals.md#oas30type) 
## GetApiMappingRequestTypeDef

```python
# GetApiMappingRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetApiMappingRequestTypeDef


def get_value() -> GetApiMappingRequestTypeDef:
    return {
        "ApiMappingId": ...,
    }


# GetApiMappingRequestTypeDef definition

class GetApiMappingRequestTypeDef(TypedDict):
    ApiMappingId: str,
    DomainName: str,
```

## GetApiMappingsRequestTypeDef

```python
# GetApiMappingsRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetApiMappingsRequestTypeDef


def get_value() -> GetApiMappingsRequestTypeDef:
    return {
        "DomainName": ...,
    }


# GetApiMappingsRequestTypeDef definition

class GetApiMappingsRequestTypeDef(TypedDict):
    DomainName: str,
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## GetApiRequestTypeDef

```python
# GetApiRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetApiRequestTypeDef


def get_value() -> GetApiRequestTypeDef:
    return {
        "ApiId": ...,
    }


# GetApiRequestTypeDef definition

class GetApiRequestTypeDef(TypedDict):
    ApiId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetApisRequestTypeDef

```python
# GetApisRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetApisRequestTypeDef


def get_value() -> GetApisRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# GetApisRequestTypeDef definition

class GetApisRequestTypeDef(TypedDict):
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## GetAuthorizerRequestTypeDef

```python
# GetAuthorizerRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetAuthorizerRequestTypeDef


def get_value() -> GetAuthorizerRequestTypeDef:
    return {
        "ApiId": ...,
    }


# GetAuthorizerRequestTypeDef definition

class GetAuthorizerRequestTypeDef(TypedDict):
    ApiId: str,
    AuthorizerId: str,
```

## GetAuthorizersRequestTypeDef

```python
# GetAuthorizersRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetAuthorizersRequestTypeDef


def get_value() -> GetAuthorizersRequestTypeDef:
    return {
        "ApiId": ...,
    }


# GetAuthorizersRequestTypeDef definition

class GetAuthorizersRequestTypeDef(TypedDict):
    ApiId: str,
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## GetDeploymentRequestTypeDef

```python
# GetDeploymentRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetDeploymentRequestTypeDef


def get_value() -> GetDeploymentRequestTypeDef:
    return {
        "ApiId": ...,
    }


# GetDeploymentRequestTypeDef definition

class GetDeploymentRequestTypeDef(TypedDict):
    ApiId: str,
    DeploymentId: str,
```

## GetDeploymentsRequestTypeDef

```python
# GetDeploymentsRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetDeploymentsRequestTypeDef


def get_value() -> GetDeploymentsRequestTypeDef:
    return {
        "ApiId": ...,
    }


# GetDeploymentsRequestTypeDef definition

class GetDeploymentsRequestTypeDef(TypedDict):
    ApiId: str,
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## GetDomainNameRequestTypeDef

```python
# GetDomainNameRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetDomainNameRequestTypeDef


def get_value() -> GetDomainNameRequestTypeDef:
    return {
        "DomainName": ...,
    }


# GetDomainNameRequestTypeDef definition

class GetDomainNameRequestTypeDef(TypedDict):
    DomainName: str,
```

## GetDomainNamesRequestTypeDef

```python
# GetDomainNamesRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetDomainNamesRequestTypeDef


def get_value() -> GetDomainNamesRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# GetDomainNamesRequestTypeDef definition

class GetDomainNamesRequestTypeDef(TypedDict):
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## GetIntegrationRequestTypeDef

```python
# GetIntegrationRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetIntegrationRequestTypeDef


def get_value() -> GetIntegrationRequestTypeDef:
    return {
        "ApiId": ...,
    }


# GetIntegrationRequestTypeDef definition

class GetIntegrationRequestTypeDef(TypedDict):
    ApiId: str,
    IntegrationId: str,
```

## GetIntegrationResponseRequestTypeDef

```python
# GetIntegrationResponseRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetIntegrationResponseRequestTypeDef


def get_value() -> GetIntegrationResponseRequestTypeDef:
    return {
        "ApiId": ...,
    }


# GetIntegrationResponseRequestTypeDef definition

class GetIntegrationResponseRequestTypeDef(TypedDict):
    ApiId: str,
    IntegrationId: str,
    IntegrationResponseId: str,
```

## GetIntegrationResponsesRequestTypeDef

```python
# GetIntegrationResponsesRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetIntegrationResponsesRequestTypeDef


def get_value() -> GetIntegrationResponsesRequestTypeDef:
    return {
        "ApiId": ...,
    }


# GetIntegrationResponsesRequestTypeDef definition

class GetIntegrationResponsesRequestTypeDef(TypedDict):
    ApiId: str,
    IntegrationId: str,
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## IntegrationResponseTypeDef

```python
# IntegrationResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import IntegrationResponseTypeDef


def get_value() -> IntegrationResponseTypeDef:
    return {
        "ContentHandlingStrategy": ...,
    }


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
## GetIntegrationsRequestTypeDef

```python
# GetIntegrationsRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetIntegrationsRequestTypeDef


def get_value() -> GetIntegrationsRequestTypeDef:
    return {
        "ApiId": ...,
    }


# GetIntegrationsRequestTypeDef definition

class GetIntegrationsRequestTypeDef(TypedDict):
    ApiId: str,
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## GetModelRequestTypeDef

```python
# GetModelRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetModelRequestTypeDef


def get_value() -> GetModelRequestTypeDef:
    return {
        "ApiId": ...,
    }


# GetModelRequestTypeDef definition

class GetModelRequestTypeDef(TypedDict):
    ApiId: str,
    ModelId: str,
```

## GetModelTemplateRequestTypeDef

```python
# GetModelTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetModelTemplateRequestTypeDef


def get_value() -> GetModelTemplateRequestTypeDef:
    return {
        "ApiId": ...,
    }


# GetModelTemplateRequestTypeDef definition

class GetModelTemplateRequestTypeDef(TypedDict):
    ApiId: str,
    ModelId: str,
```

## GetModelsRequestTypeDef

```python
# GetModelsRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetModelsRequestTypeDef


def get_value() -> GetModelsRequestTypeDef:
    return {
        "ApiId": ...,
    }


# GetModelsRequestTypeDef definition

class GetModelsRequestTypeDef(TypedDict):
    ApiId: str,
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## ModelTypeDef

```python
# ModelTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import ModelTypeDef


def get_value() -> ModelTypeDef:
    return {
        "ContentType": ...,
    }


# ModelTypeDef definition

class ModelTypeDef(TypedDict):
    Name: str,
    ContentType: NotRequired[str],
    Description: NotRequired[str],
    ModelId: NotRequired[str],
    Schema: NotRequired[str],
```

## GetRouteRequestTypeDef

```python
# GetRouteRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetRouteRequestTypeDef


def get_value() -> GetRouteRequestTypeDef:
    return {
        "ApiId": ...,
    }


# GetRouteRequestTypeDef definition

class GetRouteRequestTypeDef(TypedDict):
    ApiId: str,
    RouteId: str,
```

## GetRouteResponseRequestTypeDef

```python
# GetRouteResponseRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetRouteResponseRequestTypeDef


def get_value() -> GetRouteResponseRequestTypeDef:
    return {
        "ApiId": ...,
    }


# GetRouteResponseRequestTypeDef definition

class GetRouteResponseRequestTypeDef(TypedDict):
    ApiId: str,
    RouteId: str,
    RouteResponseId: str,
```

## GetRouteResponsesRequestTypeDef

```python
# GetRouteResponsesRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetRouteResponsesRequestTypeDef


def get_value() -> GetRouteResponsesRequestTypeDef:
    return {
        "ApiId": ...,
    }


# GetRouteResponsesRequestTypeDef definition

class GetRouteResponsesRequestTypeDef(TypedDict):
    ApiId: str,
    RouteId: str,
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## GetRoutesRequestTypeDef

```python
# GetRoutesRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetRoutesRequestTypeDef


def get_value() -> GetRoutesRequestTypeDef:
    return {
        "ApiId": ...,
    }


# GetRoutesRequestTypeDef definition

class GetRoutesRequestTypeDef(TypedDict):
    ApiId: str,
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## GetStageRequestTypeDef

```python
# GetStageRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetStageRequestTypeDef


def get_value() -> GetStageRequestTypeDef:
    return {
        "ApiId": ...,
    }


# GetStageRequestTypeDef definition

class GetStageRequestTypeDef(TypedDict):
    ApiId: str,
    StageName: str,
```

## GetStagesRequestTypeDef

```python
# GetStagesRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetStagesRequestTypeDef


def get_value() -> GetStagesRequestTypeDef:
    return {
        "ApiId": ...,
    }


# GetStagesRequestTypeDef definition

class GetStagesRequestTypeDef(TypedDict):
    ApiId: str,
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## GetTagsRequestTypeDef

```python
# GetTagsRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetTagsRequestTypeDef


def get_value() -> GetTagsRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# GetTagsRequestTypeDef definition

class GetTagsRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## GetVpcLinkRequestTypeDef

```python
# GetVpcLinkRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetVpcLinkRequestTypeDef


def get_value() -> GetVpcLinkRequestTypeDef:
    return {
        "VpcLinkId": ...,
    }


# GetVpcLinkRequestTypeDef definition

class GetVpcLinkRequestTypeDef(TypedDict):
    VpcLinkId: str,
```

## GetVpcLinksRequestTypeDef

```python
# GetVpcLinksRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetVpcLinksRequestTypeDef


def get_value() -> GetVpcLinksRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# GetVpcLinksRequestTypeDef definition

class GetVpcLinksRequestTypeDef(TypedDict):
    MaxResults: NotRequired[str],
    NextToken: NotRequired[str],
```

## VpcLinkTypeDef

```python
# VpcLinkTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import VpcLinkTypeDef


def get_value() -> VpcLinkTypeDef:
    return {
        "CreatedDate": ...,
    }


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
## ImportApiRequestTypeDef

```python
# ImportApiRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import ImportApiRequestTypeDef


def get_value() -> ImportApiRequestTypeDef:
    return {
        "Body": ...,
    }


# ImportApiRequestTypeDef definition

class ImportApiRequestTypeDef(TypedDict):
    Body: str,
    Basepath: NotRequired[str],
    FailOnWarnings: NotRequired[bool],
```

## JWTConfigurationTypeDef

```python
# JWTConfigurationTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import JWTConfigurationTypeDef


def get_value() -> JWTConfigurationTypeDef:
    return {
        "Audience": ...,
    }


# JWTConfigurationTypeDef definition

class JWTConfigurationTypeDef(TypedDict):
    Audience: NotRequired[Sequence[str]],
    Issuer: NotRequired[str],
```

## ReimportApiRequestTypeDef

```python
# ReimportApiRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import ReimportApiRequestTypeDef


def get_value() -> ReimportApiRequestTypeDef:
    return {
        "ApiId": ...,
    }


# ReimportApiRequestTypeDef definition

class ReimportApiRequestTypeDef(TypedDict):
    ApiId: str,
    Body: str,
    Basepath: NotRequired[str],
    FailOnWarnings: NotRequired[bool],
```

## ResetAuthorizersCacheRequestTypeDef

```python
# ResetAuthorizersCacheRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import ResetAuthorizersCacheRequestTypeDef


def get_value() -> ResetAuthorizersCacheRequestTypeDef:
    return {
        "ApiId": ...,
    }


# ResetAuthorizersCacheRequestTypeDef definition

class ResetAuthorizersCacheRequestTypeDef(TypedDict):
    ApiId: str,
    StageName: str,
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: NotRequired[Mapping[str, str]],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateApiMappingRequestTypeDef

```python
# UpdateApiMappingRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import UpdateApiMappingRequestTypeDef


def get_value() -> UpdateApiMappingRequestTypeDef:
    return {
        "ApiId": ...,
    }


# UpdateApiMappingRequestTypeDef definition

class UpdateApiMappingRequestTypeDef(TypedDict):
    ApiId: str,
    ApiMappingId: str,
    DomainName: str,
    ApiMappingKey: NotRequired[str],
    Stage: NotRequired[str],
```

## UpdateDeploymentRequestTypeDef

```python
# UpdateDeploymentRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import UpdateDeploymentRequestTypeDef


def get_value() -> UpdateDeploymentRequestTypeDef:
    return {
        "ApiId": ...,
    }


# UpdateDeploymentRequestTypeDef definition

class UpdateDeploymentRequestTypeDef(TypedDict):
    ApiId: str,
    DeploymentId: str,
    Description: NotRequired[str],
```

## UpdateIntegrationResponseRequestTypeDef

```python
# UpdateIntegrationResponseRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import UpdateIntegrationResponseRequestTypeDef


def get_value() -> UpdateIntegrationResponseRequestTypeDef:
    return {
        "ApiId": ...,
    }


# UpdateIntegrationResponseRequestTypeDef definition

class UpdateIntegrationResponseRequestTypeDef(TypedDict):
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
## UpdateModelRequestTypeDef

```python
# UpdateModelRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import UpdateModelRequestTypeDef


def get_value() -> UpdateModelRequestTypeDef:
    return {
        "ApiId": ...,
    }


# UpdateModelRequestTypeDef definition

class UpdateModelRequestTypeDef(TypedDict):
    ApiId: str,
    ModelId: str,
    ContentType: NotRequired[str],
    Description: NotRequired[str],
    Name: NotRequired[str],
    Schema: NotRequired[str],
```

## UpdateVpcLinkRequestTypeDef

```python
# UpdateVpcLinkRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import UpdateVpcLinkRequestTypeDef


def get_value() -> UpdateVpcLinkRequestTypeDef:
    return {
        "VpcLinkId": ...,
    }


# UpdateVpcLinkRequestTypeDef definition

class UpdateVpcLinkRequestTypeDef(TypedDict):
    VpcLinkId: str,
    Name: NotRequired[str],
```

## ApiTypeDef

```python
# ApiTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import ApiTypeDef


def get_value() -> ApiTypeDef:
    return {
        "ApiEndpoint": ...,
    }


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
# AuthorizerTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import AuthorizerTypeDef


def get_value() -> AuthorizerTypeDef:
    return {
        "AuthorizerCredentialsArn": ...,
    }


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
## CreateApiMappingResponseTypeDef

```python
# CreateApiMappingResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import CreateApiMappingResponseTypeDef


def get_value() -> CreateApiMappingResponseTypeDef:
    return {
        "ApiId": ...,
    }


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
# CreateApiResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import CreateApiResponseTypeDef


def get_value() -> CreateApiResponseTypeDef:
    return {
        "ApiEndpoint": ...,
    }


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
# CreateAuthorizerResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import CreateAuthorizerResponseTypeDef


def get_value() -> CreateAuthorizerResponseTypeDef:
    return {
        "AuthorizerCredentialsArn": ...,
    }


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
# CreateDeploymentResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import CreateDeploymentResponseTypeDef


def get_value() -> CreateDeploymentResponseTypeDef:
    return {
        "AutoDeployed": ...,
    }


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
# CreateIntegrationResponseResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import CreateIntegrationResponseResponseTypeDef


def get_value() -> CreateIntegrationResponseResponseTypeDef:
    return {
        "ContentHandlingStrategy": ...,
    }


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
# CreateModelResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import CreateModelResponseTypeDef


def get_value() -> CreateModelResponseTypeDef:
    return {
        "ContentType": ...,
    }


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
# CreateVpcLinkResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import CreateVpcLinkResponseTypeDef


def get_value() -> CreateVpcLinkResponseTypeDef:
    return {
        "CreatedDate": ...,
    }


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
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportApiResponseTypeDef

```python
# ExportApiResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import ExportApiResponseTypeDef


def get_value() -> ExportApiResponseTypeDef:
    return {
        "body": ...,
    }


# ExportApiResponseTypeDef definition

class ExportApiResponseTypeDef(TypedDict):
    body: StreamingBody,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetApiMappingResponseTypeDef

```python
# GetApiMappingResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetApiMappingResponseTypeDef


def get_value() -> GetApiMappingResponseTypeDef:
    return {
        "ApiId": ...,
    }


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
# GetApiMappingsResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetApiMappingsResponseTypeDef


def get_value() -> GetApiMappingsResponseTypeDef:
    return {
        "Items": ...,
    }


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
# GetApiResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetApiResponseTypeDef


def get_value() -> GetApiResponseTypeDef:
    return {
        "ApiEndpoint": ...,
    }


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
# GetAuthorizerResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetAuthorizerResponseTypeDef


def get_value() -> GetAuthorizerResponseTypeDef:
    return {
        "AuthorizerCredentialsArn": ...,
    }


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
# GetDeploymentResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetDeploymentResponseTypeDef


def get_value() -> GetDeploymentResponseTypeDef:
    return {
        "AutoDeployed": ...,
    }


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
# GetIntegrationResponseResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetIntegrationResponseResponseTypeDef


def get_value() -> GetIntegrationResponseResponseTypeDef:
    return {
        "ContentHandlingStrategy": ...,
    }


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
# GetModelResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetModelResponseTypeDef


def get_value() -> GetModelResponseTypeDef:
    return {
        "ContentType": ...,
    }


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
# GetModelTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetModelTemplateResponseTypeDef


def get_value() -> GetModelTemplateResponseTypeDef:
    return {
        "Value": ...,
    }


# GetModelTemplateResponseTypeDef definition

class GetModelTemplateResponseTypeDef(TypedDict):
    Value: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTagsResponseTypeDef

```python
# GetTagsResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetTagsResponseTypeDef


def get_value() -> GetTagsResponseTypeDef:
    return {
        "Tags": ...,
    }


# GetTagsResponseTypeDef definition

class GetTagsResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetVpcLinkResponseTypeDef

```python
# GetVpcLinkResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetVpcLinkResponseTypeDef


def get_value() -> GetVpcLinkResponseTypeDef:
    return {
        "CreatedDate": ...,
    }


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
# ImportApiResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import ImportApiResponseTypeDef


def get_value() -> ImportApiResponseTypeDef:
    return {
        "ApiEndpoint": ...,
    }


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
# ReimportApiResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import ReimportApiResponseTypeDef


def get_value() -> ReimportApiResponseTypeDef:
    return {
        "ApiEndpoint": ...,
    }


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
# UpdateApiMappingResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import UpdateApiMappingResponseTypeDef


def get_value() -> UpdateApiMappingResponseTypeDef:
    return {
        "ApiId": ...,
    }


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
# UpdateApiResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import UpdateApiResponseTypeDef


def get_value() -> UpdateApiResponseTypeDef:
    return {
        "ApiEndpoint": ...,
    }


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
# UpdateAuthorizerResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import UpdateAuthorizerResponseTypeDef


def get_value() -> UpdateAuthorizerResponseTypeDef:
    return {
        "AuthorizerCredentialsArn": ...,
    }


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
# UpdateDeploymentResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import UpdateDeploymentResponseTypeDef


def get_value() -> UpdateDeploymentResponseTypeDef:
    return {
        "AutoDeployed": ...,
    }


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
# UpdateIntegrationResponseResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import UpdateIntegrationResponseResponseTypeDef


def get_value() -> UpdateIntegrationResponseResponseTypeDef:
    return {
        "ContentHandlingStrategy": ...,
    }


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
# UpdateModelResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import UpdateModelResponseTypeDef


def get_value() -> UpdateModelResponseTypeDef:
    return {
        "ContentType": ...,
    }


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
# UpdateVpcLinkResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import UpdateVpcLinkResponseTypeDef


def get_value() -> UpdateVpcLinkResponseTypeDef:
    return {
        "CreatedDate": ...,
    }


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
## CreateDomainNameResponseTypeDef

```python
# CreateDomainNameResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import CreateDomainNameResponseTypeDef


def get_value() -> CreateDomainNameResponseTypeDef:
    return {
        "ApiMappingSelectionExpression": ...,
    }


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
# DomainNameTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import DomainNameTypeDef


def get_value() -> DomainNameTypeDef:
    return {
        "ApiMappingSelectionExpression": ...,
    }


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
# GetDomainNameResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetDomainNameResponseTypeDef


def get_value() -> GetDomainNameResponseTypeDef:
    return {
        "ApiMappingSelectionExpression": ...,
    }


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
# UpdateDomainNameResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import UpdateDomainNameResponseTypeDef


def get_value() -> UpdateDomainNameResponseTypeDef:
    return {
        "ApiMappingSelectionExpression": ...,
    }


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
## CreateIntegrationRequestTypeDef

```python
# CreateIntegrationRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import CreateIntegrationRequestTypeDef


def get_value() -> CreateIntegrationRequestTypeDef:
    return {
        "ApiId": ...,
    }


# CreateIntegrationRequestTypeDef definition

class CreateIntegrationRequestTypeDef(TypedDict):
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
## UpdateIntegrationRequestTypeDef

```python
# UpdateIntegrationRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import UpdateIntegrationRequestTypeDef


def get_value() -> UpdateIntegrationRequestTypeDef:
    return {
        "ApiId": ...,
    }


# UpdateIntegrationRequestTypeDef definition

class UpdateIntegrationRequestTypeDef(TypedDict):
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
# CreateIntegrationResultTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import CreateIntegrationResultTypeDef


def get_value() -> CreateIntegrationResultTypeDef:
    return {
        "ApiGatewayManaged": ...,
    }


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
# GetIntegrationResultTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetIntegrationResultTypeDef


def get_value() -> GetIntegrationResultTypeDef:
    return {
        "ApiGatewayManaged": ...,
    }


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
# IntegrationTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import IntegrationTypeDef


def get_value() -> IntegrationTypeDef:
    return {
        "ApiGatewayManaged": ...,
    }


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
# UpdateIntegrationResultTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import UpdateIntegrationResultTypeDef


def get_value() -> UpdateIntegrationResultTypeDef:
    return {
        "ApiGatewayManaged": ...,
    }


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
## CreateRouteRequestTypeDef

```python
# CreateRouteRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import CreateRouteRequestTypeDef


def get_value() -> CreateRouteRequestTypeDef:
    return {
        "ApiId": ...,
    }


# CreateRouteRequestTypeDef definition

class CreateRouteRequestTypeDef(TypedDict):
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
## CreateRouteResponseRequestTypeDef

```python
# CreateRouteResponseRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import CreateRouteResponseRequestTypeDef


def get_value() -> CreateRouteResponseRequestTypeDef:
    return {
        "ApiId": ...,
    }


# CreateRouteResponseRequestTypeDef definition

class CreateRouteResponseRequestTypeDef(TypedDict):
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
# CreateRouteResponseResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import CreateRouteResponseResponseTypeDef


def get_value() -> CreateRouteResponseResponseTypeDef:
    return {
        "ModelSelectionExpression": ...,
    }


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
# CreateRouteResultTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import CreateRouteResultTypeDef


def get_value() -> CreateRouteResultTypeDef:
    return {
        "ApiGatewayManaged": ...,
    }


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
# GetRouteResponseResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetRouteResponseResponseTypeDef


def get_value() -> GetRouteResponseResponseTypeDef:
    return {
        "ModelSelectionExpression": ...,
    }


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
# GetRouteResultTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetRouteResultTypeDef


def get_value() -> GetRouteResultTypeDef:
    return {
        "ApiGatewayManaged": ...,
    }


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
# RouteResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import RouteResponseTypeDef


def get_value() -> RouteResponseTypeDef:
    return {
        "ModelSelectionExpression": ...,
    }


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
# RouteTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import RouteTypeDef


def get_value() -> RouteTypeDef:
    return {
        "ApiGatewayManaged": ...,
    }


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
## UpdateRouteRequestTypeDef

```python
# UpdateRouteRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import UpdateRouteRequestTypeDef


def get_value() -> UpdateRouteRequestTypeDef:
    return {
        "ApiId": ...,
    }


# UpdateRouteRequestTypeDef definition

class UpdateRouteRequestTypeDef(TypedDict):
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
## UpdateRouteResponseRequestTypeDef

```python
# UpdateRouteResponseRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import UpdateRouteResponseRequestTypeDef


def get_value() -> UpdateRouteResponseRequestTypeDef:
    return {
        "ApiId": ...,
    }


# UpdateRouteResponseRequestTypeDef definition

class UpdateRouteResponseRequestTypeDef(TypedDict):
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
# UpdateRouteResponseResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import UpdateRouteResponseResponseTypeDef


def get_value() -> UpdateRouteResponseResponseTypeDef:
    return {
        "ModelSelectionExpression": ...,
    }


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
# UpdateRouteResultTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import UpdateRouteResultTypeDef


def get_value() -> UpdateRouteResultTypeDef:
    return {
        "ApiGatewayManaged": ...,
    }


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
## CreateStageRequestTypeDef

```python
# CreateStageRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import CreateStageRequestTypeDef


def get_value() -> CreateStageRequestTypeDef:
    return {
        "ApiId": ...,
    }


# CreateStageRequestTypeDef definition

class CreateStageRequestTypeDef(TypedDict):
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
# CreateStageResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import CreateStageResponseTypeDef


def get_value() -> CreateStageResponseTypeDef:
    return {
        "AccessLogSettings": ...,
    }


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
# GetStageResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetStageResponseTypeDef


def get_value() -> GetStageResponseTypeDef:
    return {
        "AccessLogSettings": ...,
    }


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
# StageTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import StageTypeDef


def get_value() -> StageTypeDef:
    return {
        "AccessLogSettings": ...,
    }


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
## UpdateStageRequestTypeDef

```python
# UpdateStageRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import UpdateStageRequestTypeDef


def get_value() -> UpdateStageRequestTypeDef:
    return {
        "ApiId": ...,
    }


# UpdateStageRequestTypeDef definition

class UpdateStageRequestTypeDef(TypedDict):
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
# UpdateStageResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import UpdateStageResponseTypeDef


def get_value() -> UpdateStageResponseTypeDef:
    return {
        "AccessLogSettings": ...,
    }


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
# GetDeploymentsResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetDeploymentsResponseTypeDef


def get_value() -> GetDeploymentsResponseTypeDef:
    return {
        "Items": ...,
    }


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
# DomainNameConfigurationTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import DomainNameConfigurationTypeDef


def get_value() -> DomainNameConfigurationTypeDef:
    return {
        "ApiGatewayDomainName": ...,
    }


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
## GetApisRequestPaginateTypeDef

```python
# GetApisRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetApisRequestPaginateTypeDef


def get_value() -> GetApisRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# GetApisRequestPaginateTypeDef definition

class GetApisRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetAuthorizersRequestPaginateTypeDef

```python
# GetAuthorizersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetAuthorizersRequestPaginateTypeDef


def get_value() -> GetAuthorizersRequestPaginateTypeDef:
    return {
        "ApiId": ...,
    }


# GetAuthorizersRequestPaginateTypeDef definition

class GetAuthorizersRequestPaginateTypeDef(TypedDict):
    ApiId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetDeploymentsRequestPaginateTypeDef

```python
# GetDeploymentsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetDeploymentsRequestPaginateTypeDef


def get_value() -> GetDeploymentsRequestPaginateTypeDef:
    return {
        "ApiId": ...,
    }


# GetDeploymentsRequestPaginateTypeDef definition

class GetDeploymentsRequestPaginateTypeDef(TypedDict):
    ApiId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetDomainNamesRequestPaginateTypeDef

```python
# GetDomainNamesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetDomainNamesRequestPaginateTypeDef


def get_value() -> GetDomainNamesRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# GetDomainNamesRequestPaginateTypeDef definition

class GetDomainNamesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetIntegrationResponsesRequestPaginateTypeDef

```python
# GetIntegrationResponsesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetIntegrationResponsesRequestPaginateTypeDef


def get_value() -> GetIntegrationResponsesRequestPaginateTypeDef:
    return {
        "ApiId": ...,
    }


# GetIntegrationResponsesRequestPaginateTypeDef definition

class GetIntegrationResponsesRequestPaginateTypeDef(TypedDict):
    ApiId: str,
    IntegrationId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetIntegrationsRequestPaginateTypeDef

```python
# GetIntegrationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetIntegrationsRequestPaginateTypeDef


def get_value() -> GetIntegrationsRequestPaginateTypeDef:
    return {
        "ApiId": ...,
    }


# GetIntegrationsRequestPaginateTypeDef definition

class GetIntegrationsRequestPaginateTypeDef(TypedDict):
    ApiId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetModelsRequestPaginateTypeDef

```python
# GetModelsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetModelsRequestPaginateTypeDef


def get_value() -> GetModelsRequestPaginateTypeDef:
    return {
        "ApiId": ...,
    }


# GetModelsRequestPaginateTypeDef definition

class GetModelsRequestPaginateTypeDef(TypedDict):
    ApiId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetRouteResponsesRequestPaginateTypeDef

```python
# GetRouteResponsesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetRouteResponsesRequestPaginateTypeDef


def get_value() -> GetRouteResponsesRequestPaginateTypeDef:
    return {
        "ApiId": ...,
    }


# GetRouteResponsesRequestPaginateTypeDef definition

class GetRouteResponsesRequestPaginateTypeDef(TypedDict):
    ApiId: str,
    RouteId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetRoutesRequestPaginateTypeDef

```python
# GetRoutesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetRoutesRequestPaginateTypeDef


def get_value() -> GetRoutesRequestPaginateTypeDef:
    return {
        "ApiId": ...,
    }


# GetRoutesRequestPaginateTypeDef definition

class GetRoutesRequestPaginateTypeDef(TypedDict):
    ApiId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetStagesRequestPaginateTypeDef

```python
# GetStagesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetStagesRequestPaginateTypeDef


def get_value() -> GetStagesRequestPaginateTypeDef:
    return {
        "ApiId": ...,
    }


# GetStagesRequestPaginateTypeDef definition

class GetStagesRequestPaginateTypeDef(TypedDict):
    ApiId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetIntegrationResponsesResponseTypeDef

```python
# GetIntegrationResponsesResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetIntegrationResponsesResponseTypeDef


def get_value() -> GetIntegrationResponsesResponseTypeDef:
    return {
        "Items": ...,
    }


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
# GetModelsResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetModelsResponseTypeDef


def get_value() -> GetModelsResponseTypeDef:
    return {
        "Items": ...,
    }


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
# GetVpcLinksResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetVpcLinksResponseTypeDef


def get_value() -> GetVpcLinksResponseTypeDef:
    return {
        "Items": ...,
    }


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
# GetApisResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetApisResponseTypeDef


def get_value() -> GetApisResponseTypeDef:
    return {
        "Items": ...,
    }


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
# GetAuthorizersResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetAuthorizersResponseTypeDef


def get_value() -> GetAuthorizersResponseTypeDef:
    return {
        "Items": ...,
    }


# GetAuthorizersResponseTypeDef definition

class GetAuthorizersResponseTypeDef(TypedDict):
    Items: List[AuthorizerTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AuthorizerTypeDef](./type_defs.md#authorizertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateApiRequestTypeDef

```python
# CreateApiRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import CreateApiRequestTypeDef


def get_value() -> CreateApiRequestTypeDef:
    return {
        "Name": ...,
    }


# CreateApiRequestTypeDef definition

class CreateApiRequestTypeDef(TypedDict):
    Name: str,
    ProtocolType: ProtocolTypeType,  # (1)
    ApiKeySelectionExpression: NotRequired[str],
    CorsConfiguration: NotRequired[CorsUnionTypeDef],  # (2)
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
2. See [:material-code-braces: CorsTypeDef](./type_defs.md#corstypedef) [:material-code-braces: CorsOutputTypeDef](./type_defs.md#corsoutputtypedef) 
## UpdateApiRequestTypeDef

```python
# UpdateApiRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import UpdateApiRequestTypeDef


def get_value() -> UpdateApiRequestTypeDef:
    return {
        "ApiId": ...,
    }


# UpdateApiRequestTypeDef definition

class UpdateApiRequestTypeDef(TypedDict):
    ApiId: str,
    ApiKeySelectionExpression: NotRequired[str],
    CorsConfiguration: NotRequired[CorsUnionTypeDef],  # (1)
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

1. See [:material-code-braces: CorsTypeDef](./type_defs.md#corstypedef) [:material-code-braces: CorsOutputTypeDef](./type_defs.md#corsoutputtypedef) 
## GetDomainNamesResponseTypeDef

```python
# GetDomainNamesResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetDomainNamesResponseTypeDef


def get_value() -> GetDomainNamesResponseTypeDef:
    return {
        "Items": ...,
    }


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
# GetIntegrationsResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetIntegrationsResponseTypeDef


def get_value() -> GetIntegrationsResponseTypeDef:
    return {
        "Items": ...,
    }


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
# GetRouteResponsesResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetRouteResponsesResponseTypeDef


def get_value() -> GetRouteResponsesResponseTypeDef:
    return {
        "Items": ...,
    }


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
# GetRoutesResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetRoutesResponseTypeDef


def get_value() -> GetRoutesResponseTypeDef:
    return {
        "Items": ...,
    }


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
# GetStagesResponseTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import GetStagesResponseTypeDef


def get_value() -> GetStagesResponseTypeDef:
    return {
        "Items": ...,
    }


# GetStagesResponseTypeDef definition

class GetStagesResponseTypeDef(TypedDict):
    Items: List[StageTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: StageTypeDef](./type_defs.md#stagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAuthorizerRequestTypeDef

```python
# CreateAuthorizerRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import CreateAuthorizerRequestTypeDef


def get_value() -> CreateAuthorizerRequestTypeDef:
    return {
        "ApiId": ...,
    }


# CreateAuthorizerRequestTypeDef definition

class CreateAuthorizerRequestTypeDef(TypedDict):
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
    JwtConfiguration: NotRequired[JWTConfigurationUnionTypeDef],  # (2)
```

1. See [:material-code-brackets: AuthorizerTypeType](./literals.md#authorizertypetype) 
2. See [:material-code-braces: JWTConfigurationTypeDef](./type_defs.md#jwtconfigurationtypedef) [:material-code-braces: JWTConfigurationOutputTypeDef](./type_defs.md#jwtconfigurationoutputtypedef) 
## UpdateAuthorizerRequestTypeDef

```python
# UpdateAuthorizerRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import UpdateAuthorizerRequestTypeDef


def get_value() -> UpdateAuthorizerRequestTypeDef:
    return {
        "ApiId": ...,
    }


# UpdateAuthorizerRequestTypeDef definition

class UpdateAuthorizerRequestTypeDef(TypedDict):
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
    JwtConfiguration: NotRequired[JWTConfigurationUnionTypeDef],  # (2)
    Name: NotRequired[str],
```

1. See [:material-code-brackets: AuthorizerTypeType](./literals.md#authorizertypetype) 
2. See [:material-code-braces: JWTConfigurationTypeDef](./type_defs.md#jwtconfigurationtypedef) [:material-code-braces: JWTConfigurationOutputTypeDef](./type_defs.md#jwtconfigurationoutputtypedef) 
## CreateDomainNameRequestTypeDef

```python
# CreateDomainNameRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import CreateDomainNameRequestTypeDef


def get_value() -> CreateDomainNameRequestTypeDef:
    return {
        "DomainName": ...,
    }


# CreateDomainNameRequestTypeDef definition

class CreateDomainNameRequestTypeDef(TypedDict):
    DomainName: str,
    DomainNameConfigurations: NotRequired[Sequence[DomainNameConfigurationUnionTypeDef]],  # (1)
    MutualTlsAuthentication: NotRequired[MutualTlsAuthenticationInputTypeDef],  # (2)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: DomainNameConfigurationTypeDef](./type_defs.md#domainnameconfigurationtypedef) [:material-code-braces: DomainNameConfigurationOutputTypeDef](./type_defs.md#domainnameconfigurationoutputtypedef) 
2. See [:material-code-braces: MutualTlsAuthenticationInputTypeDef](./type_defs.md#mutualtlsauthenticationinputtypedef) 
## UpdateDomainNameRequestTypeDef

```python
# UpdateDomainNameRequestTypeDef TypedDict usage example

from types_aiobotocore_apigatewayv2.type_defs import UpdateDomainNameRequestTypeDef


def get_value() -> UpdateDomainNameRequestTypeDef:
    return {
        "DomainName": ...,
    }


# UpdateDomainNameRequestTypeDef definition

class UpdateDomainNameRequestTypeDef(TypedDict):
    DomainName: str,
    DomainNameConfigurations: NotRequired[Sequence[DomainNameConfigurationUnionTypeDef]],  # (1)
    MutualTlsAuthentication: NotRequired[MutualTlsAuthenticationInputTypeDef],  # (2)
```

1. See [:material-code-braces: DomainNameConfigurationTypeDef](./type_defs.md#domainnameconfigurationtypedef) [:material-code-braces: DomainNameConfigurationOutputTypeDef](./type_defs.md#domainnameconfigurationoutputtypedef) 
2. See [:material-code-braces: MutualTlsAuthenticationInputTypeDef](./type_defs.md#mutualtlsauthenticationinputtypedef) 
