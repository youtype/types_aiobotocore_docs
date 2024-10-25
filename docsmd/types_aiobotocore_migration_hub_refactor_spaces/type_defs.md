# Type definitions

> [Index](../README.md) > [MigrationHubRefactorSpaces](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MigrationHubRefactorSpaces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
    type annotations stubs module [types-aiobotocore-migration-hub-refactor-spaces](https://pypi.org/project/types-aiobotocore-migration-hub-refactor-spaces/).



## ApiGatewayProxyConfigTypeDef

```python
# ApiGatewayProxyConfigTypeDef definition

class ApiGatewayProxyConfigTypeDef(TypedDict):
    ApiGatewayId: NotRequired[str],
    EndpointType: NotRequired[ApiGatewayEndpointTypeType],  # (1)
    NlbArn: NotRequired[str],
    NlbName: NotRequired[str],
    ProxyUrl: NotRequired[str],
    StageName: NotRequired[str],
    VpcLinkId: NotRequired[str],
```

1. See [:material-code-brackets: ApiGatewayEndpointTypeType](./literals.md#apigatewayendpointtypetype) 
## ApiGatewayProxyInputTypeDef

```python
# ApiGatewayProxyInputTypeDef definition

class ApiGatewayProxyInputTypeDef(TypedDict):
    EndpointType: NotRequired[ApiGatewayEndpointTypeType],  # (1)
    StageName: NotRequired[str],
```

1. See [:material-code-brackets: ApiGatewayEndpointTypeType](./literals.md#apigatewayendpointtypetype) 
## ApiGatewayProxySummaryTypeDef

```python
# ApiGatewayProxySummaryTypeDef definition

class ApiGatewayProxySummaryTypeDef(TypedDict):
    ApiGatewayId: NotRequired[str],
    EndpointType: NotRequired[ApiGatewayEndpointTypeType],  # (1)
    NlbArn: NotRequired[str],
    NlbName: NotRequired[str],
    ProxyUrl: NotRequired[str],
    StageName: NotRequired[str],
    VpcLinkId: NotRequired[str],
```

1. See [:material-code-brackets: ApiGatewayEndpointTypeType](./literals.md#apigatewayendpointtypetype) 
## ErrorResponseTypeDef

```python
# ErrorResponseTypeDef definition

class ErrorResponseTypeDef(TypedDict):
    AccountId: NotRequired[str],
    AdditionalDetails: NotRequired[Dict[str, str]],
    Code: NotRequired[ErrorCodeType],  # (1)
    Message: NotRequired[str],
    ResourceIdentifier: NotRequired[str],
    ResourceType: NotRequired[ErrorResourceTypeType],  # (2)
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
2. See [:material-code-brackets: ErrorResourceTypeType](./literals.md#errorresourcetypetype) 
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

## CreateEnvironmentRequestRequestTypeDef

```python
# CreateEnvironmentRequestRequestTypeDef definition

class CreateEnvironmentRequestRequestTypeDef(TypedDict):
    Name: str,
    NetworkFabricType: NetworkFabricTypeType,  # (1)
    ClientToken: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: NetworkFabricTypeType](./literals.md#networkfabrictypetype) 
## DefaultRouteInputTypeDef

```python
# DefaultRouteInputTypeDef definition

class DefaultRouteInputTypeDef(TypedDict):
    ActivationState: NotRequired[RouteActivationStateType],  # (1)
```

1. See [:material-code-brackets: RouteActivationStateType](./literals.md#routeactivationstatetype) 
## UriPathRouteInputTypeDef

```python
# UriPathRouteInputTypeDef definition

class UriPathRouteInputTypeDef(TypedDict):
    ActivationState: RouteActivationStateType,  # (1)
    SourcePath: str,
    AppendSourcePath: NotRequired[bool],
    IncludeChildPaths: NotRequired[bool],
    Methods: NotRequired[Sequence[HttpMethodType]],  # (2)
```

1. See [:material-code-brackets: RouteActivationStateType](./literals.md#routeactivationstatetype) 
2. See [:material-code-brackets: HttpMethodType](./literals.md#httpmethodtype) 
## UriPathRouteInputOutputTypeDef

```python
# UriPathRouteInputOutputTypeDef definition

class UriPathRouteInputOutputTypeDef(TypedDict):
    ActivationState: RouteActivationStateType,  # (1)
    SourcePath: str,
    AppendSourcePath: NotRequired[bool],
    IncludeChildPaths: NotRequired[bool],
    Methods: NotRequired[List[HttpMethodType]],  # (2)
```

1. See [:material-code-brackets: RouteActivationStateType](./literals.md#routeactivationstatetype) 
2. See [:material-code-brackets: HttpMethodType](./literals.md#httpmethodtype) 
## LambdaEndpointInputTypeDef

```python
# LambdaEndpointInputTypeDef definition

class LambdaEndpointInputTypeDef(TypedDict):
    Arn: str,
```

## UrlEndpointInputTypeDef

```python
# UrlEndpointInputTypeDef definition

class UrlEndpointInputTypeDef(TypedDict):
    Url: str,
    HealthUrl: NotRequired[str],
```

## DeleteApplicationRequestRequestTypeDef

```python
# DeleteApplicationRequestRequestTypeDef definition

class DeleteApplicationRequestRequestTypeDef(TypedDict):
    ApplicationIdentifier: str,
    EnvironmentIdentifier: str,
```

## DeleteEnvironmentRequestRequestTypeDef

```python
# DeleteEnvironmentRequestRequestTypeDef definition

class DeleteEnvironmentRequestRequestTypeDef(TypedDict):
    EnvironmentIdentifier: str,
```

## DeleteResourcePolicyRequestRequestTypeDef

```python
# DeleteResourcePolicyRequestRequestTypeDef definition

class DeleteResourcePolicyRequestRequestTypeDef(TypedDict):
    Identifier: str,
```

## DeleteRouteRequestRequestTypeDef

```python
# DeleteRouteRequestRequestTypeDef definition

class DeleteRouteRequestRequestTypeDef(TypedDict):
    ApplicationIdentifier: str,
    EnvironmentIdentifier: str,
    RouteIdentifier: str,
```

## DeleteServiceRequestRequestTypeDef

```python
# DeleteServiceRequestRequestTypeDef definition

class DeleteServiceRequestRequestTypeDef(TypedDict):
    ApplicationIdentifier: str,
    EnvironmentIdentifier: str,
    ServiceIdentifier: str,
```

## EnvironmentVpcTypeDef

```python
# EnvironmentVpcTypeDef definition

class EnvironmentVpcTypeDef(TypedDict):
    AccountId: NotRequired[str],
    CidrBlocks: NotRequired[List[str]],
    CreatedTime: NotRequired[datetime],
    EnvironmentId: NotRequired[str],
    LastUpdatedTime: NotRequired[datetime],
    VpcId: NotRequired[str],
    VpcName: NotRequired[str],
```

## GetApplicationRequestRequestTypeDef

```python
# GetApplicationRequestRequestTypeDef definition

class GetApplicationRequestRequestTypeDef(TypedDict):
    ApplicationIdentifier: str,
    EnvironmentIdentifier: str,
```

## GetEnvironmentRequestRequestTypeDef

```python
# GetEnvironmentRequestRequestTypeDef definition

class GetEnvironmentRequestRequestTypeDef(TypedDict):
    EnvironmentIdentifier: str,
```

## GetResourcePolicyRequestRequestTypeDef

```python
# GetResourcePolicyRequestRequestTypeDef definition

class GetResourcePolicyRequestRequestTypeDef(TypedDict):
    Identifier: str,
```

## GetRouteRequestRequestTypeDef

```python
# GetRouteRequestRequestTypeDef definition

class GetRouteRequestRequestTypeDef(TypedDict):
    ApplicationIdentifier: str,
    EnvironmentIdentifier: str,
    RouteIdentifier: str,
```

## GetServiceRequestRequestTypeDef

```python
# GetServiceRequestRequestTypeDef definition

class GetServiceRequestRequestTypeDef(TypedDict):
    ApplicationIdentifier: str,
    EnvironmentIdentifier: str,
    ServiceIdentifier: str,
```

## LambdaEndpointConfigTypeDef

```python
# LambdaEndpointConfigTypeDef definition

class LambdaEndpointConfigTypeDef(TypedDict):
    Arn: NotRequired[str],
```

## UrlEndpointConfigTypeDef

```python
# UrlEndpointConfigTypeDef definition

class UrlEndpointConfigTypeDef(TypedDict):
    HealthUrl: NotRequired[str],
    Url: NotRequired[str],
```

## LambdaEndpointSummaryTypeDef

```python
# LambdaEndpointSummaryTypeDef definition

class LambdaEndpointSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListApplicationsRequestRequestTypeDef

```python
# ListApplicationsRequestRequestTypeDef definition

class ListApplicationsRequestRequestTypeDef(TypedDict):
    EnvironmentIdentifier: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListEnvironmentVpcsRequestRequestTypeDef

```python
# ListEnvironmentVpcsRequestRequestTypeDef definition

class ListEnvironmentVpcsRequestRequestTypeDef(TypedDict):
    EnvironmentIdentifier: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListEnvironmentsRequestRequestTypeDef

```python
# ListEnvironmentsRequestRequestTypeDef definition

class ListEnvironmentsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListRoutesRequestRequestTypeDef

```python
# ListRoutesRequestRequestTypeDef definition

class ListRoutesRequestRequestTypeDef(TypedDict):
    ApplicationIdentifier: str,
    EnvironmentIdentifier: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListServicesRequestRequestTypeDef

```python
# ListServicesRequestRequestTypeDef definition

class ListServicesRequestRequestTypeDef(TypedDict):
    ApplicationIdentifier: str,
    EnvironmentIdentifier: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## PutResourcePolicyRequestRequestTypeDef

```python
# PutResourcePolicyRequestRequestTypeDef definition

class PutResourcePolicyRequestRequestTypeDef(TypedDict):
    Policy: str,
    ResourceArn: str,
```

## UrlEndpointSummaryTypeDef

```python
# UrlEndpointSummaryTypeDef definition

class UrlEndpointSummaryTypeDef(TypedDict):
    HealthUrl: NotRequired[str],
    Url: NotRequired[str],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateRouteRequestRequestTypeDef

```python
# UpdateRouteRequestRequestTypeDef definition

class UpdateRouteRequestRequestTypeDef(TypedDict):
    ActivationState: RouteActivationStateType,  # (1)
    ApplicationIdentifier: str,
    EnvironmentIdentifier: str,
    RouteIdentifier: str,
```

1. See [:material-code-brackets: RouteActivationStateType](./literals.md#routeactivationstatetype) 
## CreateApplicationRequestRequestTypeDef

```python
# CreateApplicationRequestRequestTypeDef definition

class CreateApplicationRequestRequestTypeDef(TypedDict):
    EnvironmentIdentifier: str,
    Name: str,
    ProxyType: ProxyTypeType,  # (1)
    VpcId: str,
    ApiGatewayProxy: NotRequired[ApiGatewayProxyInputTypeDef],  # (2)
    ClientToken: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ProxyTypeType](./literals.md#proxytypetype) 
2. See [:material-code-braces: ApiGatewayProxyInputTypeDef](./type_defs.md#apigatewayproxyinputtypedef) 
## ApplicationSummaryTypeDef

```python
# ApplicationSummaryTypeDef definition

class ApplicationSummaryTypeDef(TypedDict):
    ApiGatewayProxy: NotRequired[ApiGatewayProxySummaryTypeDef],  # (1)
    ApplicationId: NotRequired[str],
    Arn: NotRequired[str],
    CreatedByAccountId: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    EnvironmentId: NotRequired[str],
    Error: NotRequired[ErrorResponseTypeDef],  # (2)
    LastUpdatedTime: NotRequired[datetime],
    Name: NotRequired[str],
    OwnerAccountId: NotRequired[str],
    ProxyType: NotRequired[ProxyTypeType],  # (3)
    State: NotRequired[ApplicationStateType],  # (4)
    Tags: NotRequired[Dict[str, str]],
    VpcId: NotRequired[str],
```

1. See [:material-code-braces: ApiGatewayProxySummaryTypeDef](./type_defs.md#apigatewayproxysummarytypedef) 
2. See [:material-code-braces: ErrorResponseTypeDef](./type_defs.md#errorresponsetypedef) 
3. See [:material-code-brackets: ProxyTypeType](./literals.md#proxytypetype) 
4. See [:material-code-brackets: ApplicationStateType](./literals.md#applicationstatetype) 
## EnvironmentSummaryTypeDef

```python
# EnvironmentSummaryTypeDef definition

class EnvironmentSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    Description: NotRequired[str],
    EnvironmentId: NotRequired[str],
    Error: NotRequired[ErrorResponseTypeDef],  # (1)
    LastUpdatedTime: NotRequired[datetime],
    Name: NotRequired[str],
    NetworkFabricType: NotRequired[NetworkFabricTypeType],  # (2)
    OwnerAccountId: NotRequired[str],
    State: NotRequired[EnvironmentStateType],  # (3)
    Tags: NotRequired[Dict[str, str]],
    TransitGatewayId: NotRequired[str],
```

1. See [:material-code-braces: ErrorResponseTypeDef](./type_defs.md#errorresponsetypedef) 
2. See [:material-code-brackets: NetworkFabricTypeType](./literals.md#networkfabrictypetype) 
3. See [:material-code-brackets: EnvironmentStateType](./literals.md#environmentstatetype) 
## RouteSummaryTypeDef

```python
# RouteSummaryTypeDef definition

class RouteSummaryTypeDef(TypedDict):
    AppendSourcePath: NotRequired[bool],
    ApplicationId: NotRequired[str],
    Arn: NotRequired[str],
    CreatedByAccountId: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    EnvironmentId: NotRequired[str],
    Error: NotRequired[ErrorResponseTypeDef],  # (1)
    IncludeChildPaths: NotRequired[bool],
    LastUpdatedTime: NotRequired[datetime],
    Methods: NotRequired[List[HttpMethodType]],  # (2)
    OwnerAccountId: NotRequired[str],
    PathResourceToId: NotRequired[Dict[str, str]],
    RouteId: NotRequired[str],
    RouteType: NotRequired[RouteTypeType],  # (3)
    ServiceId: NotRequired[str],
    SourcePath: NotRequired[str],
    State: NotRequired[RouteStateType],  # (4)
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: ErrorResponseTypeDef](./type_defs.md#errorresponsetypedef) 
2. See [:material-code-brackets: HttpMethodType](./literals.md#httpmethodtype) 
3. See [:material-code-brackets: RouteTypeType](./literals.md#routetypetype) 
4. See [:material-code-brackets: RouteStateType](./literals.md#routestatetype) 
## CreateApplicationResponseTypeDef

```python
# CreateApplicationResponseTypeDef definition

class CreateApplicationResponseTypeDef(TypedDict):
    ApiGatewayProxy: ApiGatewayProxyInputTypeDef,  # (1)
    ApplicationId: str,
    Arn: str,
    CreatedByAccountId: str,
    CreatedTime: datetime,
    EnvironmentId: str,
    LastUpdatedTime: datetime,
    Name: str,
    OwnerAccountId: str,
    ProxyType: ProxyTypeType,  # (2)
    State: ApplicationStateType,  # (3)
    Tags: Dict[str, str],
    VpcId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ApiGatewayProxyInputTypeDef](./type_defs.md#apigatewayproxyinputtypedef) 
2. See [:material-code-brackets: ProxyTypeType](./literals.md#proxytypetype) 
3. See [:material-code-brackets: ApplicationStateType](./literals.md#applicationstatetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEnvironmentResponseTypeDef

```python
# CreateEnvironmentResponseTypeDef definition

class CreateEnvironmentResponseTypeDef(TypedDict):
    Arn: str,
    CreatedTime: datetime,
    Description: str,
    EnvironmentId: str,
    LastUpdatedTime: datetime,
    Name: str,
    NetworkFabricType: NetworkFabricTypeType,  # (1)
    OwnerAccountId: str,
    State: EnvironmentStateType,  # (2)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: NetworkFabricTypeType](./literals.md#networkfabrictypetype) 
2. See [:material-code-brackets: EnvironmentStateType](./literals.md#environmentstatetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteApplicationResponseTypeDef

```python
# DeleteApplicationResponseTypeDef definition

class DeleteApplicationResponseTypeDef(TypedDict):
    ApplicationId: str,
    Arn: str,
    EnvironmentId: str,
    LastUpdatedTime: datetime,
    Name: str,
    State: ApplicationStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ApplicationStateType](./literals.md#applicationstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteEnvironmentResponseTypeDef

```python
# DeleteEnvironmentResponseTypeDef definition

class DeleteEnvironmentResponseTypeDef(TypedDict):
    Arn: str,
    EnvironmentId: str,
    LastUpdatedTime: datetime,
    Name: str,
    State: EnvironmentStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: EnvironmentStateType](./literals.md#environmentstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRouteResponseTypeDef

```python
# DeleteRouteResponseTypeDef definition

class DeleteRouteResponseTypeDef(TypedDict):
    ApplicationId: str,
    Arn: str,
    LastUpdatedTime: datetime,
    RouteId: str,
    ServiceId: str,
    State: RouteStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RouteStateType](./literals.md#routestatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteServiceResponseTypeDef

```python
# DeleteServiceResponseTypeDef definition

class DeleteServiceResponseTypeDef(TypedDict):
    ApplicationId: str,
    Arn: str,
    EnvironmentId: str,
    LastUpdatedTime: datetime,
    Name: str,
    ServiceId: str,
    State: ServiceStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ServiceStateType](./literals.md#servicestatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetApplicationResponseTypeDef

```python
# GetApplicationResponseTypeDef definition

class GetApplicationResponseTypeDef(TypedDict):
    ApiGatewayProxy: ApiGatewayProxyConfigTypeDef,  # (1)
    ApplicationId: str,
    Arn: str,
    CreatedByAccountId: str,
    CreatedTime: datetime,
    EnvironmentId: str,
    Error: ErrorResponseTypeDef,  # (2)
    LastUpdatedTime: datetime,
    Name: str,
    OwnerAccountId: str,
    ProxyType: ProxyTypeType,  # (3)
    State: ApplicationStateType,  # (4)
    Tags: Dict[str, str],
    VpcId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: ApiGatewayProxyConfigTypeDef](./type_defs.md#apigatewayproxyconfigtypedef) 
2. See [:material-code-braces: ErrorResponseTypeDef](./type_defs.md#errorresponsetypedef) 
3. See [:material-code-brackets: ProxyTypeType](./literals.md#proxytypetype) 
4. See [:material-code-brackets: ApplicationStateType](./literals.md#applicationstatetype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEnvironmentResponseTypeDef

```python
# GetEnvironmentResponseTypeDef definition

class GetEnvironmentResponseTypeDef(TypedDict):
    Arn: str,
    CreatedTime: datetime,
    Description: str,
    EnvironmentId: str,
    Error: ErrorResponseTypeDef,  # (1)
    LastUpdatedTime: datetime,
    Name: str,
    NetworkFabricType: NetworkFabricTypeType,  # (2)
    OwnerAccountId: str,
    State: EnvironmentStateType,  # (3)
    Tags: Dict[str, str],
    TransitGatewayId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ErrorResponseTypeDef](./type_defs.md#errorresponsetypedef) 
2. See [:material-code-brackets: NetworkFabricTypeType](./literals.md#networkfabrictypetype) 
3. See [:material-code-brackets: EnvironmentStateType](./literals.md#environmentstatetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourcePolicyResponseTypeDef

```python
# GetResourcePolicyResponseTypeDef definition

class GetResourcePolicyResponseTypeDef(TypedDict):
    Policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRouteResponseTypeDef

```python
# GetRouteResponseTypeDef definition

class GetRouteResponseTypeDef(TypedDict):
    AppendSourcePath: bool,
    ApplicationId: str,
    Arn: str,
    CreatedByAccountId: str,
    CreatedTime: datetime,
    EnvironmentId: str,
    Error: ErrorResponseTypeDef,  # (1)
    IncludeChildPaths: bool,
    LastUpdatedTime: datetime,
    Methods: List[HttpMethodType],  # (2)
    OwnerAccountId: str,
    PathResourceToId: Dict[str, str],
    RouteId: str,
    RouteType: RouteTypeType,  # (3)
    ServiceId: str,
    SourcePath: str,
    State: RouteStateType,  # (4)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: ErrorResponseTypeDef](./type_defs.md#errorresponsetypedef) 
2. See [:material-code-brackets: HttpMethodType](./literals.md#httpmethodtype) 
3. See [:material-code-brackets: RouteTypeType](./literals.md#routetypetype) 
4. See [:material-code-brackets: RouteStateType](./literals.md#routestatetype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRouteResponseTypeDef

```python
# UpdateRouteResponseTypeDef definition

class UpdateRouteResponseTypeDef(TypedDict):
    ApplicationId: str,
    Arn: str,
    LastUpdatedTime: datetime,
    RouteId: str,
    ServiceId: str,
    State: RouteStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RouteStateType](./literals.md#routestatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRouteRequestRequestTypeDef

```python
# CreateRouteRequestRequestTypeDef definition

class CreateRouteRequestRequestTypeDef(TypedDict):
    ApplicationIdentifier: str,
    EnvironmentIdentifier: str,
    RouteType: RouteTypeType,  # (1)
    ServiceIdentifier: str,
    ClientToken: NotRequired[str],
    DefaultRoute: NotRequired[DefaultRouteInputTypeDef],  # (2)
    Tags: NotRequired[Mapping[str, str]],
    UriPathRoute: NotRequired[UriPathRouteInputTypeDef],  # (3)
```

1. See [:material-code-brackets: RouteTypeType](./literals.md#routetypetype) 
2. See [:material-code-braces: DefaultRouteInputTypeDef](./type_defs.md#defaultrouteinputtypedef) 
3. See [:material-code-braces: UriPathRouteInputTypeDef](./type_defs.md#uripathrouteinputtypedef) 
## CreateRouteResponseTypeDef

```python
# CreateRouteResponseTypeDef definition

class CreateRouteResponseTypeDef(TypedDict):
    ApplicationId: str,
    Arn: str,
    CreatedByAccountId: str,
    CreatedTime: datetime,
    LastUpdatedTime: datetime,
    OwnerAccountId: str,
    RouteId: str,
    RouteType: RouteTypeType,  # (1)
    ServiceId: str,
    State: RouteStateType,  # (2)
    Tags: Dict[str, str],
    UriPathRoute: UriPathRouteInputOutputTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: RouteTypeType](./literals.md#routetypetype) 
2. See [:material-code-brackets: RouteStateType](./literals.md#routestatetype) 
3. See [:material-code-braces: UriPathRouteInputOutputTypeDef](./type_defs.md#uripathrouteinputoutputtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateServiceRequestRequestTypeDef

```python
# CreateServiceRequestRequestTypeDef definition

class CreateServiceRequestRequestTypeDef(TypedDict):
    ApplicationIdentifier: str,
    EndpointType: ServiceEndpointTypeType,  # (1)
    EnvironmentIdentifier: str,
    Name: str,
    ClientToken: NotRequired[str],
    Description: NotRequired[str],
    LambdaEndpoint: NotRequired[LambdaEndpointInputTypeDef],  # (2)
    Tags: NotRequired[Mapping[str, str]],
    UrlEndpoint: NotRequired[UrlEndpointInputTypeDef],  # (3)
    VpcId: NotRequired[str],
```

1. See [:material-code-brackets: ServiceEndpointTypeType](./literals.md#serviceendpointtypetype) 
2. See [:material-code-braces: LambdaEndpointInputTypeDef](./type_defs.md#lambdaendpointinputtypedef) 
3. See [:material-code-braces: UrlEndpointInputTypeDef](./type_defs.md#urlendpointinputtypedef) 
## CreateServiceResponseTypeDef

```python
# CreateServiceResponseTypeDef definition

class CreateServiceResponseTypeDef(TypedDict):
    ApplicationId: str,
    Arn: str,
    CreatedByAccountId: str,
    CreatedTime: datetime,
    Description: str,
    EndpointType: ServiceEndpointTypeType,  # (1)
    EnvironmentId: str,
    LambdaEndpoint: LambdaEndpointInputTypeDef,  # (2)
    LastUpdatedTime: datetime,
    Name: str,
    OwnerAccountId: str,
    ServiceId: str,
    State: ServiceStateType,  # (3)
    Tags: Dict[str, str],
    UrlEndpoint: UrlEndpointInputTypeDef,  # (4)
    VpcId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: ServiceEndpointTypeType](./literals.md#serviceendpointtypetype) 
2. See [:material-code-braces: LambdaEndpointInputTypeDef](./type_defs.md#lambdaendpointinputtypedef) 
3. See [:material-code-brackets: ServiceStateType](./literals.md#servicestatetype) 
4. See [:material-code-braces: UrlEndpointInputTypeDef](./type_defs.md#urlendpointinputtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEnvironmentVpcsResponseTypeDef

```python
# ListEnvironmentVpcsResponseTypeDef definition

class ListEnvironmentVpcsResponseTypeDef(TypedDict):
    EnvironmentVpcList: List[EnvironmentVpcTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EnvironmentVpcTypeDef](./type_defs.md#environmentvpctypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServiceResponseTypeDef

```python
# GetServiceResponseTypeDef definition

class GetServiceResponseTypeDef(TypedDict):
    ApplicationId: str,
    Arn: str,
    CreatedByAccountId: str,
    CreatedTime: datetime,
    Description: str,
    EndpointType: ServiceEndpointTypeType,  # (1)
    EnvironmentId: str,
    Error: ErrorResponseTypeDef,  # (2)
    LambdaEndpoint: LambdaEndpointConfigTypeDef,  # (3)
    LastUpdatedTime: datetime,
    Name: str,
    OwnerAccountId: str,
    ServiceId: str,
    State: ServiceStateType,  # (4)
    Tags: Dict[str, str],
    UrlEndpoint: UrlEndpointConfigTypeDef,  # (5)
    VpcId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: ServiceEndpointTypeType](./literals.md#serviceendpointtypetype) 
2. See [:material-code-braces: ErrorResponseTypeDef](./type_defs.md#errorresponsetypedef) 
3. See [:material-code-braces: LambdaEndpointConfigTypeDef](./type_defs.md#lambdaendpointconfigtypedef) 
4. See [:material-code-brackets: ServiceStateType](./literals.md#servicestatetype) 
5. See [:material-code-braces: UrlEndpointConfigTypeDef](./type_defs.md#urlendpointconfigtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApplicationsRequestListApplicationsPaginateTypeDef

```python
# ListApplicationsRequestListApplicationsPaginateTypeDef definition

class ListApplicationsRequestListApplicationsPaginateTypeDef(TypedDict):
    EnvironmentIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef

```python
# ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef definition

class ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef(TypedDict):
    EnvironmentIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEnvironmentsRequestListEnvironmentsPaginateTypeDef

```python
# ListEnvironmentsRequestListEnvironmentsPaginateTypeDef definition

class ListEnvironmentsRequestListEnvironmentsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRoutesRequestListRoutesPaginateTypeDef

```python
# ListRoutesRequestListRoutesPaginateTypeDef definition

class ListRoutesRequestListRoutesPaginateTypeDef(TypedDict):
    ApplicationIdentifier: str,
    EnvironmentIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServicesRequestListServicesPaginateTypeDef

```python
# ListServicesRequestListServicesPaginateTypeDef definition

class ListServicesRequestListServicesPaginateTypeDef(TypedDict):
    ApplicationIdentifier: str,
    EnvironmentIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ServiceSummaryTypeDef

```python
# ServiceSummaryTypeDef definition

class ServiceSummaryTypeDef(TypedDict):
    ApplicationId: NotRequired[str],
    Arn: NotRequired[str],
    CreatedByAccountId: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    Description: NotRequired[str],
    EndpointType: NotRequired[ServiceEndpointTypeType],  # (1)
    EnvironmentId: NotRequired[str],
    Error: NotRequired[ErrorResponseTypeDef],  # (2)
    LambdaEndpoint: NotRequired[LambdaEndpointSummaryTypeDef],  # (3)
    LastUpdatedTime: NotRequired[datetime],
    Name: NotRequired[str],
    OwnerAccountId: NotRequired[str],
    ServiceId: NotRequired[str],
    State: NotRequired[ServiceStateType],  # (4)
    Tags: NotRequired[Dict[str, str]],
    UrlEndpoint: NotRequired[UrlEndpointSummaryTypeDef],  # (5)
    VpcId: NotRequired[str],
```

1. See [:material-code-brackets: ServiceEndpointTypeType](./literals.md#serviceendpointtypetype) 
2. See [:material-code-braces: ErrorResponseTypeDef](./type_defs.md#errorresponsetypedef) 
3. See [:material-code-braces: LambdaEndpointSummaryTypeDef](./type_defs.md#lambdaendpointsummarytypedef) 
4. See [:material-code-brackets: ServiceStateType](./literals.md#servicestatetype) 
5. See [:material-code-braces: UrlEndpointSummaryTypeDef](./type_defs.md#urlendpointsummarytypedef) 
## ListApplicationsResponseTypeDef

```python
# ListApplicationsResponseTypeDef definition

class ListApplicationsResponseTypeDef(TypedDict):
    ApplicationSummaryList: List[ApplicationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ApplicationSummaryTypeDef](./type_defs.md#applicationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEnvironmentsResponseTypeDef

```python
# ListEnvironmentsResponseTypeDef definition

class ListEnvironmentsResponseTypeDef(TypedDict):
    EnvironmentSummaryList: List[EnvironmentSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EnvironmentSummaryTypeDef](./type_defs.md#environmentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRoutesResponseTypeDef

```python
# ListRoutesResponseTypeDef definition

class ListRoutesResponseTypeDef(TypedDict):
    RouteSummaryList: List[RouteSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RouteSummaryTypeDef](./type_defs.md#routesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServicesResponseTypeDef

```python
# ListServicesResponseTypeDef definition

class ListServicesResponseTypeDef(TypedDict):
    ServiceSummaryList: List[ServiceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ServiceSummaryTypeDef](./type_defs.md#servicesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
