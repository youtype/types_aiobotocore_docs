# Type definitions

> [Index](../README.md) > [AppMesh](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [AppMesh](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
    type annotations stubs module [types-aiobotocore-appmesh](https://pypi.org/project/types-aiobotocore-appmesh/).



## AwsCloudMapInstanceAttributeTypeDef

```python
# AwsCloudMapInstanceAttributeTypeDef definition

class AwsCloudMapInstanceAttributeTypeDef(TypedDict):
    key: str,
    value: str,
```

## ListenerTlsFileCertificateTypeDef

```python
# ListenerTlsFileCertificateTypeDef definition

class ListenerTlsFileCertificateTypeDef(TypedDict):
    certificateChain: str,
    privateKey: str,
```

## ListenerTlsSdsCertificateTypeDef

```python
# ListenerTlsSdsCertificateTypeDef definition

class ListenerTlsSdsCertificateTypeDef(TypedDict):
    secretName: str,
```

## TagRefTypeDef

```python
# TagRefTypeDef definition

class TagRefTypeDef(TypedDict):
    key: str,
    value: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## DeleteGatewayRouteInputRequestTypeDef

```python
# DeleteGatewayRouteInputRequestTypeDef definition

class DeleteGatewayRouteInputRequestTypeDef(TypedDict):
    gatewayRouteName: str,
    meshName: str,
    virtualGatewayName: str,
    meshOwner: NotRequired[str],
```

## DeleteMeshInputRequestTypeDef

```python
# DeleteMeshInputRequestTypeDef definition

class DeleteMeshInputRequestTypeDef(TypedDict):
    meshName: str,
```

## DeleteRouteInputRequestTypeDef

```python
# DeleteRouteInputRequestTypeDef definition

class DeleteRouteInputRequestTypeDef(TypedDict):
    meshName: str,
    routeName: str,
    virtualRouterName: str,
    meshOwner: NotRequired[str],
```

## DeleteVirtualGatewayInputRequestTypeDef

```python
# DeleteVirtualGatewayInputRequestTypeDef definition

class DeleteVirtualGatewayInputRequestTypeDef(TypedDict):
    meshName: str,
    virtualGatewayName: str,
    meshOwner: NotRequired[str],
```

## DeleteVirtualNodeInputRequestTypeDef

```python
# DeleteVirtualNodeInputRequestTypeDef definition

class DeleteVirtualNodeInputRequestTypeDef(TypedDict):
    meshName: str,
    virtualNodeName: str,
    meshOwner: NotRequired[str],
```

## DeleteVirtualRouterInputRequestTypeDef

```python
# DeleteVirtualRouterInputRequestTypeDef definition

class DeleteVirtualRouterInputRequestTypeDef(TypedDict):
    meshName: str,
    virtualRouterName: str,
    meshOwner: NotRequired[str],
```

## DeleteVirtualServiceInputRequestTypeDef

```python
# DeleteVirtualServiceInputRequestTypeDef definition

class DeleteVirtualServiceInputRequestTypeDef(TypedDict):
    meshName: str,
    virtualServiceName: str,
    meshOwner: NotRequired[str],
```

## DescribeGatewayRouteInputRequestTypeDef

```python
# DescribeGatewayRouteInputRequestTypeDef definition

class DescribeGatewayRouteInputRequestTypeDef(TypedDict):
    gatewayRouteName: str,
    meshName: str,
    virtualGatewayName: str,
    meshOwner: NotRequired[str],
```

## DescribeMeshInputRequestTypeDef

```python
# DescribeMeshInputRequestTypeDef definition

class DescribeMeshInputRequestTypeDef(TypedDict):
    meshName: str,
    meshOwner: NotRequired[str],
```

## DescribeRouteInputRequestTypeDef

```python
# DescribeRouteInputRequestTypeDef definition

class DescribeRouteInputRequestTypeDef(TypedDict):
    meshName: str,
    routeName: str,
    virtualRouterName: str,
    meshOwner: NotRequired[str],
```

## DescribeVirtualGatewayInputRequestTypeDef

```python
# DescribeVirtualGatewayInputRequestTypeDef definition

class DescribeVirtualGatewayInputRequestTypeDef(TypedDict):
    meshName: str,
    virtualGatewayName: str,
    meshOwner: NotRequired[str],
```

## DescribeVirtualNodeInputRequestTypeDef

```python
# DescribeVirtualNodeInputRequestTypeDef definition

class DescribeVirtualNodeInputRequestTypeDef(TypedDict):
    meshName: str,
    virtualNodeName: str,
    meshOwner: NotRequired[str],
```

## DescribeVirtualRouterInputRequestTypeDef

```python
# DescribeVirtualRouterInputRequestTypeDef definition

class DescribeVirtualRouterInputRequestTypeDef(TypedDict):
    meshName: str,
    virtualRouterName: str,
    meshOwner: NotRequired[str],
```

## DescribeVirtualServiceInputRequestTypeDef

```python
# DescribeVirtualServiceInputRequestTypeDef definition

class DescribeVirtualServiceInputRequestTypeDef(TypedDict):
    meshName: str,
    virtualServiceName: str,
    meshOwner: NotRequired[str],
```

## DnsServiceDiscoveryTypeDef

```python
# DnsServiceDiscoveryTypeDef definition

class DnsServiceDiscoveryTypeDef(TypedDict):
    hostname: str,
    ipPreference: NotRequired[IpPreferenceType],  # (1)
    responseType: NotRequired[DnsResponseTypeType],  # (2)
```

1. See [:material-code-brackets: IpPreferenceType](./literals.md#ippreferencetype) 
2. See [:material-code-brackets: DnsResponseTypeType](./literals.md#dnsresponsetypetype) 
## DurationTypeDef

```python
# DurationTypeDef definition

class DurationTypeDef(TypedDict):
    unit: NotRequired[DurationUnitType],  # (1)
    value: NotRequired[int],
```

1. See [:material-code-brackets: DurationUnitType](./literals.md#durationunittype) 
## EgressFilterTypeDef

```python
# EgressFilterTypeDef definition

class EgressFilterTypeDef(TypedDict):
    type: EgressFilterTypeType,  # (1)
```

1. See [:material-code-brackets: EgressFilterTypeType](./literals.md#egressfiltertypetype) 
## GatewayRouteStatusTypeDef

```python
# GatewayRouteStatusTypeDef definition

class GatewayRouteStatusTypeDef(TypedDict):
    status: GatewayRouteStatusCodeType,  # (1)
```

1. See [:material-code-brackets: GatewayRouteStatusCodeType](./literals.md#gatewayroutestatuscodetype) 
## ResourceMetadataTypeDef

```python
# ResourceMetadataTypeDef definition

class ResourceMetadataTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    lastUpdatedAt: datetime,
    meshOwner: str,
    resourceOwner: str,
    uid: str,
    version: int,
```

## GatewayRouteHostnameMatchTypeDef

```python
# GatewayRouteHostnameMatchTypeDef definition

class GatewayRouteHostnameMatchTypeDef(TypedDict):
    exact: NotRequired[str],
    suffix: NotRequired[str],
```

## GatewayRouteHostnameRewriteTypeDef

```python
# GatewayRouteHostnameRewriteTypeDef definition

class GatewayRouteHostnameRewriteTypeDef(TypedDict):
    defaultTargetHostname: NotRequired[DefaultGatewayRouteRewriteType],  # (1)
```

1. See [:material-code-brackets: DefaultGatewayRouteRewriteType](./literals.md#defaultgatewayrouterewritetype) 
## GatewayRouteRefTypeDef

```python
# GatewayRouteRefTypeDef definition

class GatewayRouteRefTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    gatewayRouteName: str,
    lastUpdatedAt: datetime,
    meshName: str,
    meshOwner: str,
    resourceOwner: str,
    version: int,
    virtualGatewayName: str,
```

## GatewayRouteVirtualServiceTypeDef

```python
# GatewayRouteVirtualServiceTypeDef definition

class GatewayRouteVirtualServiceTypeDef(TypedDict):
    virtualServiceName: str,
```

## MatchRangeTypeDef

```python
# MatchRangeTypeDef definition

class MatchRangeTypeDef(TypedDict):
    end: int,
    start: int,
```

## WeightedTargetTypeDef

```python
# WeightedTargetTypeDef definition

class WeightedTargetTypeDef(TypedDict):
    virtualNode: str,
    weight: int,
    port: NotRequired[int],
```

## HealthCheckPolicyTypeDef

```python
# HealthCheckPolicyTypeDef definition

class HealthCheckPolicyTypeDef(TypedDict):
    healthyThreshold: int,
    intervalMillis: int,
    protocol: PortProtocolType,  # (1)
    timeoutMillis: int,
    unhealthyThreshold: int,
    path: NotRequired[str],
    port: NotRequired[int],
```

1. See [:material-code-brackets: PortProtocolType](./literals.md#portprotocoltype) 
## HttpPathMatchTypeDef

```python
# HttpPathMatchTypeDef definition

class HttpPathMatchTypeDef(TypedDict):
    exact: NotRequired[str],
    regex: NotRequired[str],
```

## HttpGatewayRoutePathRewriteTypeDef

```python
# HttpGatewayRoutePathRewriteTypeDef definition

class HttpGatewayRoutePathRewriteTypeDef(TypedDict):
    exact: NotRequired[str],
```

## HttpGatewayRoutePrefixRewriteTypeDef

```python
# HttpGatewayRoutePrefixRewriteTypeDef definition

class HttpGatewayRoutePrefixRewriteTypeDef(TypedDict):
    defaultPrefix: NotRequired[DefaultGatewayRouteRewriteType],  # (1)
    value: NotRequired[str],
```

1. See [:material-code-brackets: DefaultGatewayRouteRewriteType](./literals.md#defaultgatewayrouterewritetype) 
## QueryParameterMatchTypeDef

```python
# QueryParameterMatchTypeDef definition

class QueryParameterMatchTypeDef(TypedDict):
    exact: NotRequired[str],
```

## JsonFormatRefTypeDef

```python
# JsonFormatRefTypeDef definition

class JsonFormatRefTypeDef(TypedDict):
    key: str,
    value: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListGatewayRoutesInputRequestTypeDef

```python
# ListGatewayRoutesInputRequestTypeDef definition

class ListGatewayRoutesInputRequestTypeDef(TypedDict):
    meshName: str,
    virtualGatewayName: str,
    limit: NotRequired[int],
    meshOwner: NotRequired[str],
    nextToken: NotRequired[str],
```

## ListMeshesInputRequestTypeDef

```python
# ListMeshesInputRequestTypeDef definition

class ListMeshesInputRequestTypeDef(TypedDict):
    limit: NotRequired[int],
    nextToken: NotRequired[str],
```

## MeshRefTypeDef

```python
# MeshRefTypeDef definition

class MeshRefTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    lastUpdatedAt: datetime,
    meshName: str,
    meshOwner: str,
    resourceOwner: str,
    version: int,
```

## ListRoutesInputRequestTypeDef

```python
# ListRoutesInputRequestTypeDef definition

class ListRoutesInputRequestTypeDef(TypedDict):
    meshName: str,
    virtualRouterName: str,
    limit: NotRequired[int],
    meshOwner: NotRequired[str],
    nextToken: NotRequired[str],
```

## RouteRefTypeDef

```python
# RouteRefTypeDef definition

class RouteRefTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    lastUpdatedAt: datetime,
    meshName: str,
    meshOwner: str,
    resourceOwner: str,
    routeName: str,
    version: int,
    virtualRouterName: str,
```

## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    limit: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListVirtualGatewaysInputRequestTypeDef

```python
# ListVirtualGatewaysInputRequestTypeDef definition

class ListVirtualGatewaysInputRequestTypeDef(TypedDict):
    meshName: str,
    limit: NotRequired[int],
    meshOwner: NotRequired[str],
    nextToken: NotRequired[str],
```

## VirtualGatewayRefTypeDef

```python
# VirtualGatewayRefTypeDef definition

class VirtualGatewayRefTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    lastUpdatedAt: datetime,
    meshName: str,
    meshOwner: str,
    resourceOwner: str,
    version: int,
    virtualGatewayName: str,
```

## ListVirtualNodesInputRequestTypeDef

```python
# ListVirtualNodesInputRequestTypeDef definition

class ListVirtualNodesInputRequestTypeDef(TypedDict):
    meshName: str,
    limit: NotRequired[int],
    meshOwner: NotRequired[str],
    nextToken: NotRequired[str],
```

## VirtualNodeRefTypeDef

```python
# VirtualNodeRefTypeDef definition

class VirtualNodeRefTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    lastUpdatedAt: datetime,
    meshName: str,
    meshOwner: str,
    resourceOwner: str,
    version: int,
    virtualNodeName: str,
```

## ListVirtualRoutersInputRequestTypeDef

```python
# ListVirtualRoutersInputRequestTypeDef definition

class ListVirtualRoutersInputRequestTypeDef(TypedDict):
    meshName: str,
    limit: NotRequired[int],
    meshOwner: NotRequired[str],
    nextToken: NotRequired[str],
```

## VirtualRouterRefTypeDef

```python
# VirtualRouterRefTypeDef definition

class VirtualRouterRefTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    lastUpdatedAt: datetime,
    meshName: str,
    meshOwner: str,
    resourceOwner: str,
    version: int,
    virtualRouterName: str,
```

## ListVirtualServicesInputRequestTypeDef

```python
# ListVirtualServicesInputRequestTypeDef definition

class ListVirtualServicesInputRequestTypeDef(TypedDict):
    meshName: str,
    limit: NotRequired[int],
    meshOwner: NotRequired[str],
    nextToken: NotRequired[str],
```

## VirtualServiceRefTypeDef

```python
# VirtualServiceRefTypeDef definition

class VirtualServiceRefTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    lastUpdatedAt: datetime,
    meshName: str,
    meshOwner: str,
    resourceOwner: str,
    version: int,
    virtualServiceName: str,
```

## ListenerTlsAcmCertificateTypeDef

```python
# ListenerTlsAcmCertificateTypeDef definition

class ListenerTlsAcmCertificateTypeDef(TypedDict):
    certificateArn: str,
```

## TlsValidationContextFileTrustTypeDef

```python
# TlsValidationContextFileTrustTypeDef definition

class TlsValidationContextFileTrustTypeDef(TypedDict):
    certificateChain: str,
```

## TlsValidationContextSdsTrustTypeDef

```python
# TlsValidationContextSdsTrustTypeDef definition

class TlsValidationContextSdsTrustTypeDef(TypedDict):
    secretName: str,
```

## PortMappingTypeDef

```python
# PortMappingTypeDef definition

class PortMappingTypeDef(TypedDict):
    port: int,
    protocol: PortProtocolType,  # (1)
```

1. See [:material-code-brackets: PortProtocolType](./literals.md#portprotocoltype) 
## MeshStatusTypeDef

```python
# MeshStatusTypeDef definition

class MeshStatusTypeDef(TypedDict):
    status: NotRequired[MeshStatusCodeType],  # (1)
```

1. See [:material-code-brackets: MeshStatusCodeType](./literals.md#meshstatuscodetype) 
## MeshServiceDiscoveryTypeDef

```python
# MeshServiceDiscoveryTypeDef definition

class MeshServiceDiscoveryTypeDef(TypedDict):
    ipPreference: NotRequired[IpPreferenceType],  # (1)
```

1. See [:material-code-brackets: IpPreferenceType](./literals.md#ippreferencetype) 
## RouteStatusTypeDef

```python
# RouteStatusTypeDef definition

class RouteStatusTypeDef(TypedDict):
    status: RouteStatusCodeType,  # (1)
```

1. See [:material-code-brackets: RouteStatusCodeType](./literals.md#routestatuscodetype) 
## SubjectAlternativeNameMatchersTypeDef

```python
# SubjectAlternativeNameMatchersTypeDef definition

class SubjectAlternativeNameMatchersTypeDef(TypedDict):
    exact: Sequence[str],
```

## TcpRouteMatchTypeDef

```python
# TcpRouteMatchTypeDef definition

class TcpRouteMatchTypeDef(TypedDict):
    port: NotRequired[int],
```

## TlsValidationContextAcmTrustTypeDef

```python
# TlsValidationContextAcmTrustTypeDef definition

class TlsValidationContextAcmTrustTypeDef(TypedDict):
    certificateAuthorityArns: Sequence[str],
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## VirtualGatewayListenerTlsFileCertificateTypeDef

```python
# VirtualGatewayListenerTlsFileCertificateTypeDef definition

class VirtualGatewayListenerTlsFileCertificateTypeDef(TypedDict):
    certificateChain: str,
    privateKey: str,
```

## VirtualGatewayListenerTlsSdsCertificateTypeDef

```python
# VirtualGatewayListenerTlsSdsCertificateTypeDef definition

class VirtualGatewayListenerTlsSdsCertificateTypeDef(TypedDict):
    secretName: str,
```

## VirtualGatewayGrpcConnectionPoolTypeDef

```python
# VirtualGatewayGrpcConnectionPoolTypeDef definition

class VirtualGatewayGrpcConnectionPoolTypeDef(TypedDict):
    maxRequests: int,
```

## VirtualGatewayHttp2ConnectionPoolTypeDef

```python
# VirtualGatewayHttp2ConnectionPoolTypeDef definition

class VirtualGatewayHttp2ConnectionPoolTypeDef(TypedDict):
    maxRequests: int,
```

## VirtualGatewayHttpConnectionPoolTypeDef

```python
# VirtualGatewayHttpConnectionPoolTypeDef definition

class VirtualGatewayHttpConnectionPoolTypeDef(TypedDict):
    maxConnections: int,
    maxPendingRequests: NotRequired[int],
```

## VirtualGatewayStatusTypeDef

```python
# VirtualGatewayStatusTypeDef definition

class VirtualGatewayStatusTypeDef(TypedDict):
    status: VirtualGatewayStatusCodeType,  # (1)
```

1. See [:material-code-brackets: VirtualGatewayStatusCodeType](./literals.md#virtualgatewaystatuscodetype) 
## VirtualGatewayHealthCheckPolicyTypeDef

```python
# VirtualGatewayHealthCheckPolicyTypeDef definition

class VirtualGatewayHealthCheckPolicyTypeDef(TypedDict):
    healthyThreshold: int,
    intervalMillis: int,
    protocol: VirtualGatewayPortProtocolType,  # (1)
    timeoutMillis: int,
    unhealthyThreshold: int,
    path: NotRequired[str],
    port: NotRequired[int],
```

1. See [:material-code-brackets: VirtualGatewayPortProtocolType](./literals.md#virtualgatewayportprotocoltype) 
## VirtualGatewayListenerTlsAcmCertificateTypeDef

```python
# VirtualGatewayListenerTlsAcmCertificateTypeDef definition

class VirtualGatewayListenerTlsAcmCertificateTypeDef(TypedDict):
    certificateArn: str,
```

## VirtualGatewayTlsValidationContextFileTrustTypeDef

```python
# VirtualGatewayTlsValidationContextFileTrustTypeDef definition

class VirtualGatewayTlsValidationContextFileTrustTypeDef(TypedDict):
    certificateChain: str,
```

## VirtualGatewayTlsValidationContextSdsTrustTypeDef

```python
# VirtualGatewayTlsValidationContextSdsTrustTypeDef definition

class VirtualGatewayTlsValidationContextSdsTrustTypeDef(TypedDict):
    secretName: str,
```

## VirtualGatewayPortMappingTypeDef

```python
# VirtualGatewayPortMappingTypeDef definition

class VirtualGatewayPortMappingTypeDef(TypedDict):
    port: int,
    protocol: VirtualGatewayPortProtocolType,  # (1)
```

1. See [:material-code-brackets: VirtualGatewayPortProtocolType](./literals.md#virtualgatewayportprotocoltype) 
## VirtualGatewayTlsValidationContextAcmTrustTypeDef

```python
# VirtualGatewayTlsValidationContextAcmTrustTypeDef definition

class VirtualGatewayTlsValidationContextAcmTrustTypeDef(TypedDict):
    certificateAuthorityArns: Sequence[str],
```

## VirtualNodeGrpcConnectionPoolTypeDef

```python
# VirtualNodeGrpcConnectionPoolTypeDef definition

class VirtualNodeGrpcConnectionPoolTypeDef(TypedDict):
    maxRequests: int,
```

## VirtualNodeHttp2ConnectionPoolTypeDef

```python
# VirtualNodeHttp2ConnectionPoolTypeDef definition

class VirtualNodeHttp2ConnectionPoolTypeDef(TypedDict):
    maxRequests: int,
```

## VirtualNodeHttpConnectionPoolTypeDef

```python
# VirtualNodeHttpConnectionPoolTypeDef definition

class VirtualNodeHttpConnectionPoolTypeDef(TypedDict):
    maxConnections: int,
    maxPendingRequests: NotRequired[int],
```

## VirtualNodeTcpConnectionPoolTypeDef

```python
# VirtualNodeTcpConnectionPoolTypeDef definition

class VirtualNodeTcpConnectionPoolTypeDef(TypedDict):
    maxConnections: int,
```

## VirtualNodeStatusTypeDef

```python
# VirtualNodeStatusTypeDef definition

class VirtualNodeStatusTypeDef(TypedDict):
    status: VirtualNodeStatusCodeType,  # (1)
```

1. See [:material-code-brackets: VirtualNodeStatusCodeType](./literals.md#virtualnodestatuscodetype) 
## VirtualNodeServiceProviderTypeDef

```python
# VirtualNodeServiceProviderTypeDef definition

class VirtualNodeServiceProviderTypeDef(TypedDict):
    virtualNodeName: str,
```

## VirtualRouterStatusTypeDef

```python
# VirtualRouterStatusTypeDef definition

class VirtualRouterStatusTypeDef(TypedDict):
    status: VirtualRouterStatusCodeType,  # (1)
```

1. See [:material-code-brackets: VirtualRouterStatusCodeType](./literals.md#virtualrouterstatuscodetype) 
## VirtualRouterServiceProviderTypeDef

```python
# VirtualRouterServiceProviderTypeDef definition

class VirtualRouterServiceProviderTypeDef(TypedDict):
    virtualRouterName: str,
```

## VirtualServiceStatusTypeDef

```python
# VirtualServiceStatusTypeDef definition

class VirtualServiceStatusTypeDef(TypedDict):
    status: VirtualServiceStatusCodeType,  # (1)
```

1. See [:material-code-brackets: VirtualServiceStatusCodeType](./literals.md#virtualservicestatuscodetype) 
## AwsCloudMapServiceDiscoveryTypeDef

```python
# AwsCloudMapServiceDiscoveryTypeDef definition

class AwsCloudMapServiceDiscoveryTypeDef(TypedDict):
    namespaceName: str,
    serviceName: str,
    attributes: NotRequired[Sequence[AwsCloudMapInstanceAttributeTypeDef]],  # (1)
    ipPreference: NotRequired[IpPreferenceType],  # (2)
```

1. See [:material-code-braces: AwsCloudMapInstanceAttributeTypeDef](./type_defs.md#awscloudmapinstanceattributetypedef) 
2. See [:material-code-brackets: IpPreferenceType](./literals.md#ippreferencetype) 
## ClientTlsCertificateTypeDef

```python
# ClientTlsCertificateTypeDef definition

class ClientTlsCertificateTypeDef(TypedDict):
    file: NotRequired[ListenerTlsFileCertificateTypeDef],  # (1)
    sds: NotRequired[ListenerTlsSdsCertificateTypeDef],  # (2)
```

1. See [:material-code-braces: ListenerTlsFileCertificateTypeDef](./type_defs.md#listenertlsfilecertificatetypedef) 
2. See [:material-code-braces: ListenerTlsSdsCertificateTypeDef](./type_defs.md#listenertlssdscertificatetypedef) 
## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Sequence[TagRefTypeDef],  # (1)
```

1. See [:material-code-braces: TagRefTypeDef](./type_defs.md#tagreftypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    nextToken: str,
    tags: List[TagRefTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagRefTypeDef](./type_defs.md#tagreftypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GrpcRetryPolicyTypeDef

```python
# GrpcRetryPolicyTypeDef definition

class GrpcRetryPolicyTypeDef(TypedDict):
    maxRetries: int,
    perRetryTimeout: DurationTypeDef,  # (2)
    grpcRetryEvents: NotRequired[Sequence[GrpcRetryPolicyEventType]],  # (1)
    httpRetryEvents: NotRequired[Sequence[str]],
    tcpRetryEvents: NotRequired[Sequence[TcpRetryPolicyEventType]],  # (3)
```

1. See [:material-code-brackets: GrpcRetryPolicyEventType](./literals.md#grpcretrypolicyeventtype) 
2. See [:material-code-braces: DurationTypeDef](./type_defs.md#durationtypedef) 
3. See [:material-code-brackets: TcpRetryPolicyEventType](./literals.md#tcpretrypolicyeventtype) 
## GrpcTimeoutTypeDef

```python
# GrpcTimeoutTypeDef definition

class GrpcTimeoutTypeDef(TypedDict):
    idle: NotRequired[DurationTypeDef],  # (1)
    perRequest: NotRequired[DurationTypeDef],  # (1)
```

1. See [:material-code-braces: DurationTypeDef](./type_defs.md#durationtypedef) 
2. See [:material-code-braces: DurationTypeDef](./type_defs.md#durationtypedef) 
## HttpRetryPolicyTypeDef

```python
# HttpRetryPolicyTypeDef definition

class HttpRetryPolicyTypeDef(TypedDict):
    maxRetries: int,
    perRetryTimeout: DurationTypeDef,  # (1)
    httpRetryEvents: NotRequired[Sequence[str]],
    tcpRetryEvents: NotRequired[Sequence[TcpRetryPolicyEventType]],  # (2)
```

1. See [:material-code-braces: DurationTypeDef](./type_defs.md#durationtypedef) 
2. See [:material-code-brackets: TcpRetryPolicyEventType](./literals.md#tcpretrypolicyeventtype) 
## HttpTimeoutTypeDef

```python
# HttpTimeoutTypeDef definition

class HttpTimeoutTypeDef(TypedDict):
    idle: NotRequired[DurationTypeDef],  # (1)
    perRequest: NotRequired[DurationTypeDef],  # (1)
```

1. See [:material-code-braces: DurationTypeDef](./type_defs.md#durationtypedef) 
2. See [:material-code-braces: DurationTypeDef](./type_defs.md#durationtypedef) 
## OutlierDetectionTypeDef

```python
# OutlierDetectionTypeDef definition

class OutlierDetectionTypeDef(TypedDict):
    baseEjectionDuration: DurationTypeDef,  # (1)
    interval: DurationTypeDef,  # (1)
    maxEjectionPercent: int,
    maxServerErrors: int,
```

1. See [:material-code-braces: DurationTypeDef](./type_defs.md#durationtypedef) 
2. See [:material-code-braces: DurationTypeDef](./type_defs.md#durationtypedef) 
## TcpTimeoutTypeDef

```python
# TcpTimeoutTypeDef definition

class TcpTimeoutTypeDef(TypedDict):
    idle: NotRequired[DurationTypeDef],  # (1)
```

1. See [:material-code-braces: DurationTypeDef](./type_defs.md#durationtypedef) 
## GrpcGatewayRouteRewriteTypeDef

```python
# GrpcGatewayRouteRewriteTypeDef definition

class GrpcGatewayRouteRewriteTypeDef(TypedDict):
    hostname: NotRequired[GatewayRouteHostnameRewriteTypeDef],  # (1)
```

1. See [:material-code-braces: GatewayRouteHostnameRewriteTypeDef](./type_defs.md#gatewayroutehostnamerewritetypedef) 
## ListGatewayRoutesOutputTypeDef

```python
# ListGatewayRoutesOutputTypeDef definition

class ListGatewayRoutesOutputTypeDef(TypedDict):
    gatewayRoutes: List[GatewayRouteRefTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GatewayRouteRefTypeDef](./type_defs.md#gatewayroutereftypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GatewayRouteTargetTypeDef

```python
# GatewayRouteTargetTypeDef definition

class GatewayRouteTargetTypeDef(TypedDict):
    virtualService: GatewayRouteVirtualServiceTypeDef,  # (1)
    port: NotRequired[int],
```

1. See [:material-code-braces: GatewayRouteVirtualServiceTypeDef](./type_defs.md#gatewayroutevirtualservicetypedef) 
## GrpcMetadataMatchMethodTypeDef

```python
# GrpcMetadataMatchMethodTypeDef definition

class GrpcMetadataMatchMethodTypeDef(TypedDict):
    exact: NotRequired[str],
    prefix: NotRequired[str],
    range: NotRequired[MatchRangeTypeDef],  # (1)
    regex: NotRequired[str],
    suffix: NotRequired[str],
```

1. See [:material-code-braces: MatchRangeTypeDef](./type_defs.md#matchrangetypedef) 
## GrpcRouteMetadataMatchMethodTypeDef

```python
# GrpcRouteMetadataMatchMethodTypeDef definition

class GrpcRouteMetadataMatchMethodTypeDef(TypedDict):
    exact: NotRequired[str],
    prefix: NotRequired[str],
    range: NotRequired[MatchRangeTypeDef],  # (1)
    regex: NotRequired[str],
    suffix: NotRequired[str],
```

1. See [:material-code-braces: MatchRangeTypeDef](./type_defs.md#matchrangetypedef) 
## HeaderMatchMethodTypeDef

```python
# HeaderMatchMethodTypeDef definition

class HeaderMatchMethodTypeDef(TypedDict):
    exact: NotRequired[str],
    prefix: NotRequired[str],
    range: NotRequired[MatchRangeTypeDef],  # (1)
    regex: NotRequired[str],
    suffix: NotRequired[str],
```

1. See [:material-code-braces: MatchRangeTypeDef](./type_defs.md#matchrangetypedef) 
## GrpcRouteActionTypeDef

```python
# GrpcRouteActionTypeDef definition

class GrpcRouteActionTypeDef(TypedDict):
    weightedTargets: Sequence[WeightedTargetTypeDef],  # (1)
```

1. See [:material-code-braces: WeightedTargetTypeDef](./type_defs.md#weightedtargettypedef) 
## HttpRouteActionTypeDef

```python
# HttpRouteActionTypeDef definition

class HttpRouteActionTypeDef(TypedDict):
    weightedTargets: Sequence[WeightedTargetTypeDef],  # (1)
```

1. See [:material-code-braces: WeightedTargetTypeDef](./type_defs.md#weightedtargettypedef) 
## TcpRouteActionTypeDef

```python
# TcpRouteActionTypeDef definition

class TcpRouteActionTypeDef(TypedDict):
    weightedTargets: Sequence[WeightedTargetTypeDef],  # (1)
```

1. See [:material-code-braces: WeightedTargetTypeDef](./type_defs.md#weightedtargettypedef) 
## HttpGatewayRouteRewriteTypeDef

```python
# HttpGatewayRouteRewriteTypeDef definition

class HttpGatewayRouteRewriteTypeDef(TypedDict):
    hostname: NotRequired[GatewayRouteHostnameRewriteTypeDef],  # (1)
    path: NotRequired[HttpGatewayRoutePathRewriteTypeDef],  # (2)
    prefix: NotRequired[HttpGatewayRoutePrefixRewriteTypeDef],  # (3)
```

1. See [:material-code-braces: GatewayRouteHostnameRewriteTypeDef](./type_defs.md#gatewayroutehostnamerewritetypedef) 
2. See [:material-code-braces: HttpGatewayRoutePathRewriteTypeDef](./type_defs.md#httpgatewayroutepathrewritetypedef) 
3. See [:material-code-braces: HttpGatewayRoutePrefixRewriteTypeDef](./type_defs.md#httpgatewayrouteprefixrewritetypedef) 
## HttpQueryParameterTypeDef

```python
# HttpQueryParameterTypeDef definition

class HttpQueryParameterTypeDef(TypedDict):
    name: str,
    match: NotRequired[QueryParameterMatchTypeDef],  # (1)
```

1. See [:material-code-braces: QueryParameterMatchTypeDef](./type_defs.md#queryparametermatchtypedef) 
## LoggingFormatTypeDef

```python
# LoggingFormatTypeDef definition

class LoggingFormatTypeDef(TypedDict):
    json: NotRequired[Sequence[JsonFormatRefTypeDef]],  # (1)
    text: NotRequired[str],
```

1. See [:material-code-braces: JsonFormatRefTypeDef](./type_defs.md#jsonformatreftypedef) 
## ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef

```python
# ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef definition

class ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef(TypedDict):
    meshName: str,
    virtualGatewayName: str,
    meshOwner: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMeshesInputListMeshesPaginateTypeDef

```python
# ListMeshesInputListMeshesPaginateTypeDef definition

class ListMeshesInputListMeshesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRoutesInputListRoutesPaginateTypeDef

```python
# ListRoutesInputListRoutesPaginateTypeDef definition

class ListRoutesInputListRoutesPaginateTypeDef(TypedDict):
    meshName: str,
    virtualRouterName: str,
    meshOwner: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsForResourceInputListTagsForResourcePaginateTypeDef

```python
# ListTagsForResourceInputListTagsForResourcePaginateTypeDef definition

class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(TypedDict):
    resourceArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef

```python
# ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef definition

class ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef(TypedDict):
    meshName: str,
    meshOwner: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListVirtualNodesInputListVirtualNodesPaginateTypeDef

```python
# ListVirtualNodesInputListVirtualNodesPaginateTypeDef definition

class ListVirtualNodesInputListVirtualNodesPaginateTypeDef(TypedDict):
    meshName: str,
    meshOwner: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef

```python
# ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef definition

class ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef(TypedDict):
    meshName: str,
    meshOwner: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListVirtualServicesInputListVirtualServicesPaginateTypeDef

```python
# ListVirtualServicesInputListVirtualServicesPaginateTypeDef definition

class ListVirtualServicesInputListVirtualServicesPaginateTypeDef(TypedDict):
    meshName: str,
    meshOwner: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMeshesOutputTypeDef

```python
# ListMeshesOutputTypeDef definition

class ListMeshesOutputTypeDef(TypedDict):
    meshes: List[MeshRefTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MeshRefTypeDef](./type_defs.md#meshreftypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRoutesOutputTypeDef

```python
# ListRoutesOutputTypeDef definition

class ListRoutesOutputTypeDef(TypedDict):
    nextToken: str,
    routes: List[RouteRefTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RouteRefTypeDef](./type_defs.md#routereftypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVirtualGatewaysOutputTypeDef

```python
# ListVirtualGatewaysOutputTypeDef definition

class ListVirtualGatewaysOutputTypeDef(TypedDict):
    nextToken: str,
    virtualGateways: List[VirtualGatewayRefTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualGatewayRefTypeDef](./type_defs.md#virtualgatewayreftypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVirtualNodesOutputTypeDef

```python
# ListVirtualNodesOutputTypeDef definition

class ListVirtualNodesOutputTypeDef(TypedDict):
    nextToken: str,
    virtualNodes: List[VirtualNodeRefTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualNodeRefTypeDef](./type_defs.md#virtualnodereftypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVirtualRoutersOutputTypeDef

```python
# ListVirtualRoutersOutputTypeDef definition

class ListVirtualRoutersOutputTypeDef(TypedDict):
    nextToken: str,
    virtualRouters: List[VirtualRouterRefTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualRouterRefTypeDef](./type_defs.md#virtualrouterreftypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVirtualServicesOutputTypeDef

```python
# ListVirtualServicesOutputTypeDef definition

class ListVirtualServicesOutputTypeDef(TypedDict):
    nextToken: str,
    virtualServices: List[VirtualServiceRefTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualServiceRefTypeDef](./type_defs.md#virtualservicereftypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListenerTlsCertificateTypeDef

```python
# ListenerTlsCertificateTypeDef definition

class ListenerTlsCertificateTypeDef(TypedDict):
    acm: NotRequired[ListenerTlsAcmCertificateTypeDef],  # (1)
    file: NotRequired[ListenerTlsFileCertificateTypeDef],  # (2)
    sds: NotRequired[ListenerTlsSdsCertificateTypeDef],  # (3)
```

1. See [:material-code-braces: ListenerTlsAcmCertificateTypeDef](./type_defs.md#listenertlsacmcertificatetypedef) 
2. See [:material-code-braces: ListenerTlsFileCertificateTypeDef](./type_defs.md#listenertlsfilecertificatetypedef) 
3. See [:material-code-braces: ListenerTlsSdsCertificateTypeDef](./type_defs.md#listenertlssdscertificatetypedef) 
## ListenerTlsValidationContextTrustTypeDef

```python
# ListenerTlsValidationContextTrustTypeDef definition

class ListenerTlsValidationContextTrustTypeDef(TypedDict):
    file: NotRequired[TlsValidationContextFileTrustTypeDef],  # (1)
    sds: NotRequired[TlsValidationContextSdsTrustTypeDef],  # (2)
```

1. See [:material-code-braces: TlsValidationContextFileTrustTypeDef](./type_defs.md#tlsvalidationcontextfiletrusttypedef) 
2. See [:material-code-braces: TlsValidationContextSdsTrustTypeDef](./type_defs.md#tlsvalidationcontextsdstrusttypedef) 
## VirtualRouterListenerTypeDef

```python
# VirtualRouterListenerTypeDef definition

class VirtualRouterListenerTypeDef(TypedDict):
    portMapping: PortMappingTypeDef,  # (1)
```

1. See [:material-code-braces: PortMappingTypeDef](./type_defs.md#portmappingtypedef) 
## MeshSpecTypeDef

```python
# MeshSpecTypeDef definition

class MeshSpecTypeDef(TypedDict):
    egressFilter: NotRequired[EgressFilterTypeDef],  # (1)
    serviceDiscovery: NotRequired[MeshServiceDiscoveryTypeDef],  # (2)
```

1. See [:material-code-braces: EgressFilterTypeDef](./type_defs.md#egressfiltertypedef) 
2. See [:material-code-braces: MeshServiceDiscoveryTypeDef](./type_defs.md#meshservicediscoverytypedef) 
## SubjectAlternativeNamesTypeDef

```python
# SubjectAlternativeNamesTypeDef definition

class SubjectAlternativeNamesTypeDef(TypedDict):
    match: SubjectAlternativeNameMatchersTypeDef,  # (1)
```

1. See [:material-code-braces: SubjectAlternativeNameMatchersTypeDef](./type_defs.md#subjectalternativenamematcherstypedef) 
## TlsValidationContextTrustTypeDef

```python
# TlsValidationContextTrustTypeDef definition

class TlsValidationContextTrustTypeDef(TypedDict):
    acm: NotRequired[TlsValidationContextAcmTrustTypeDef],  # (1)
    file: NotRequired[TlsValidationContextFileTrustTypeDef],  # (2)
    sds: NotRequired[TlsValidationContextSdsTrustTypeDef],  # (3)
```

1. See [:material-code-braces: TlsValidationContextAcmTrustTypeDef](./type_defs.md#tlsvalidationcontextacmtrusttypedef) 
2. See [:material-code-braces: TlsValidationContextFileTrustTypeDef](./type_defs.md#tlsvalidationcontextfiletrusttypedef) 
3. See [:material-code-braces: TlsValidationContextSdsTrustTypeDef](./type_defs.md#tlsvalidationcontextsdstrusttypedef) 
## VirtualGatewayClientTlsCertificateTypeDef

```python
# VirtualGatewayClientTlsCertificateTypeDef definition

class VirtualGatewayClientTlsCertificateTypeDef(TypedDict):
    file: NotRequired[VirtualGatewayListenerTlsFileCertificateTypeDef],  # (1)
    sds: NotRequired[VirtualGatewayListenerTlsSdsCertificateTypeDef],  # (2)
```

1. See [:material-code-braces: VirtualGatewayListenerTlsFileCertificateTypeDef](./type_defs.md#virtualgatewaylistenertlsfilecertificatetypedef) 
2. See [:material-code-braces: VirtualGatewayListenerTlsSdsCertificateTypeDef](./type_defs.md#virtualgatewaylistenertlssdscertificatetypedef) 
## VirtualGatewayConnectionPoolTypeDef

```python
# VirtualGatewayConnectionPoolTypeDef definition

class VirtualGatewayConnectionPoolTypeDef(TypedDict):
    grpc: NotRequired[VirtualGatewayGrpcConnectionPoolTypeDef],  # (1)
    http: NotRequired[VirtualGatewayHttpConnectionPoolTypeDef],  # (2)
    http2: NotRequired[VirtualGatewayHttp2ConnectionPoolTypeDef],  # (3)
```

1. See [:material-code-braces: VirtualGatewayGrpcConnectionPoolTypeDef](./type_defs.md#virtualgatewaygrpcconnectionpooltypedef) 
2. See [:material-code-braces: VirtualGatewayHttpConnectionPoolTypeDef](./type_defs.md#virtualgatewayhttpconnectionpooltypedef) 
3. See [:material-code-braces: VirtualGatewayHttp2ConnectionPoolTypeDef](./type_defs.md#virtualgatewayhttp2connectionpooltypedef) 
## VirtualGatewayListenerTlsCertificateTypeDef

```python
# VirtualGatewayListenerTlsCertificateTypeDef definition

class VirtualGatewayListenerTlsCertificateTypeDef(TypedDict):
    acm: NotRequired[VirtualGatewayListenerTlsAcmCertificateTypeDef],  # (1)
    file: NotRequired[VirtualGatewayListenerTlsFileCertificateTypeDef],  # (2)
    sds: NotRequired[VirtualGatewayListenerTlsSdsCertificateTypeDef],  # (3)
```

1. See [:material-code-braces: VirtualGatewayListenerTlsAcmCertificateTypeDef](./type_defs.md#virtualgatewaylistenertlsacmcertificatetypedef) 
2. See [:material-code-braces: VirtualGatewayListenerTlsFileCertificateTypeDef](./type_defs.md#virtualgatewaylistenertlsfilecertificatetypedef) 
3. See [:material-code-braces: VirtualGatewayListenerTlsSdsCertificateTypeDef](./type_defs.md#virtualgatewaylistenertlssdscertificatetypedef) 
## VirtualGatewayListenerTlsValidationContextTrustTypeDef

```python
# VirtualGatewayListenerTlsValidationContextTrustTypeDef definition

class VirtualGatewayListenerTlsValidationContextTrustTypeDef(TypedDict):
    file: NotRequired[VirtualGatewayTlsValidationContextFileTrustTypeDef],  # (1)
    sds: NotRequired[VirtualGatewayTlsValidationContextSdsTrustTypeDef],  # (2)
```

1. See [:material-code-braces: VirtualGatewayTlsValidationContextFileTrustTypeDef](./type_defs.md#virtualgatewaytlsvalidationcontextfiletrusttypedef) 
2. See [:material-code-braces: VirtualGatewayTlsValidationContextSdsTrustTypeDef](./type_defs.md#virtualgatewaytlsvalidationcontextsdstrusttypedef) 
## VirtualGatewayTlsValidationContextTrustTypeDef

```python
# VirtualGatewayTlsValidationContextTrustTypeDef definition

class VirtualGatewayTlsValidationContextTrustTypeDef(TypedDict):
    acm: NotRequired[VirtualGatewayTlsValidationContextAcmTrustTypeDef],  # (1)
    file: NotRequired[VirtualGatewayTlsValidationContextFileTrustTypeDef],  # (2)
    sds: NotRequired[VirtualGatewayTlsValidationContextSdsTrustTypeDef],  # (3)
```

1. See [:material-code-braces: VirtualGatewayTlsValidationContextAcmTrustTypeDef](./type_defs.md#virtualgatewaytlsvalidationcontextacmtrusttypedef) 
2. See [:material-code-braces: VirtualGatewayTlsValidationContextFileTrustTypeDef](./type_defs.md#virtualgatewaytlsvalidationcontextfiletrusttypedef) 
3. See [:material-code-braces: VirtualGatewayTlsValidationContextSdsTrustTypeDef](./type_defs.md#virtualgatewaytlsvalidationcontextsdstrusttypedef) 
## VirtualNodeConnectionPoolTypeDef

```python
# VirtualNodeConnectionPoolTypeDef definition

class VirtualNodeConnectionPoolTypeDef(TypedDict):
    grpc: NotRequired[VirtualNodeGrpcConnectionPoolTypeDef],  # (1)
    http: NotRequired[VirtualNodeHttpConnectionPoolTypeDef],  # (2)
    http2: NotRequired[VirtualNodeHttp2ConnectionPoolTypeDef],  # (3)
    tcp: NotRequired[VirtualNodeTcpConnectionPoolTypeDef],  # (4)
```

1. See [:material-code-braces: VirtualNodeGrpcConnectionPoolTypeDef](./type_defs.md#virtualnodegrpcconnectionpooltypedef) 
2. See [:material-code-braces: VirtualNodeHttpConnectionPoolTypeDef](./type_defs.md#virtualnodehttpconnectionpooltypedef) 
3. See [:material-code-braces: VirtualNodeHttp2ConnectionPoolTypeDef](./type_defs.md#virtualnodehttp2connectionpooltypedef) 
4. See [:material-code-braces: VirtualNodeTcpConnectionPoolTypeDef](./type_defs.md#virtualnodetcpconnectionpooltypedef) 
## VirtualServiceProviderTypeDef

```python
# VirtualServiceProviderTypeDef definition

class VirtualServiceProviderTypeDef(TypedDict):
    virtualNode: NotRequired[VirtualNodeServiceProviderTypeDef],  # (1)
    virtualRouter: NotRequired[VirtualRouterServiceProviderTypeDef],  # (2)
```

1. See [:material-code-braces: VirtualNodeServiceProviderTypeDef](./type_defs.md#virtualnodeserviceprovidertypedef) 
2. See [:material-code-braces: VirtualRouterServiceProviderTypeDef](./type_defs.md#virtualrouterserviceprovidertypedef) 
## ServiceDiscoveryTypeDef

```python
# ServiceDiscoveryTypeDef definition

class ServiceDiscoveryTypeDef(TypedDict):
    awsCloudMap: NotRequired[AwsCloudMapServiceDiscoveryTypeDef],  # (1)
    dns: NotRequired[DnsServiceDiscoveryTypeDef],  # (2)
```

1. See [:material-code-braces: AwsCloudMapServiceDiscoveryTypeDef](./type_defs.md#awscloudmapservicediscoverytypedef) 
2. See [:material-code-braces: DnsServiceDiscoveryTypeDef](./type_defs.md#dnsservicediscoverytypedef) 
## ListenerTimeoutTypeDef

```python
# ListenerTimeoutTypeDef definition

class ListenerTimeoutTypeDef(TypedDict):
    grpc: NotRequired[GrpcTimeoutTypeDef],  # (1)
    http: NotRequired[HttpTimeoutTypeDef],  # (2)
    http2: NotRequired[HttpTimeoutTypeDef],  # (2)
    tcp: NotRequired[TcpTimeoutTypeDef],  # (4)
```

1. See [:material-code-braces: GrpcTimeoutTypeDef](./type_defs.md#grpctimeouttypedef) 
2. See [:material-code-braces: HttpTimeoutTypeDef](./type_defs.md#httptimeouttypedef) 
3. See [:material-code-braces: HttpTimeoutTypeDef](./type_defs.md#httptimeouttypedef) 
4. See [:material-code-braces: TcpTimeoutTypeDef](./type_defs.md#tcptimeouttypedef) 
## GrpcGatewayRouteActionTypeDef

```python
# GrpcGatewayRouteActionTypeDef definition

class GrpcGatewayRouteActionTypeDef(TypedDict):
    target: GatewayRouteTargetTypeDef,  # (2)
    rewrite: NotRequired[GrpcGatewayRouteRewriteTypeDef],  # (1)
```

1. See [:material-code-braces: GrpcGatewayRouteRewriteTypeDef](./type_defs.md#grpcgatewayrouterewritetypedef) 
2. See [:material-code-braces: GatewayRouteTargetTypeDef](./type_defs.md#gatewayroutetargettypedef) 
## GrpcGatewayRouteMetadataTypeDef

```python
# GrpcGatewayRouteMetadataTypeDef definition

class GrpcGatewayRouteMetadataTypeDef(TypedDict):
    name: str,
    invert: NotRequired[bool],
    match: NotRequired[GrpcMetadataMatchMethodTypeDef],  # (1)
```

1. See [:material-code-braces: GrpcMetadataMatchMethodTypeDef](./type_defs.md#grpcmetadatamatchmethodtypedef) 
## GrpcRouteMetadataTypeDef

```python
# GrpcRouteMetadataTypeDef definition

class GrpcRouteMetadataTypeDef(TypedDict):
    name: str,
    invert: NotRequired[bool],
    match: NotRequired[GrpcRouteMetadataMatchMethodTypeDef],  # (1)
```

1. See [:material-code-braces: GrpcRouteMetadataMatchMethodTypeDef](./type_defs.md#grpcroutemetadatamatchmethodtypedef) 
## HttpGatewayRouteHeaderTypeDef

```python
# HttpGatewayRouteHeaderTypeDef definition

class HttpGatewayRouteHeaderTypeDef(TypedDict):
    name: str,
    invert: NotRequired[bool],
    match: NotRequired[HeaderMatchMethodTypeDef],  # (1)
```

1. See [:material-code-braces: HeaderMatchMethodTypeDef](./type_defs.md#headermatchmethodtypedef) 
## HttpRouteHeaderTypeDef

```python
# HttpRouteHeaderTypeDef definition

class HttpRouteHeaderTypeDef(TypedDict):
    name: str,
    invert: NotRequired[bool],
    match: NotRequired[HeaderMatchMethodTypeDef],  # (1)
```

1. See [:material-code-braces: HeaderMatchMethodTypeDef](./type_defs.md#headermatchmethodtypedef) 
## TcpRouteTypeDef

```python
# TcpRouteTypeDef definition

class TcpRouteTypeDef(TypedDict):
    action: TcpRouteActionTypeDef,  # (1)
    match: NotRequired[TcpRouteMatchTypeDef],  # (2)
    timeout: NotRequired[TcpTimeoutTypeDef],  # (3)
```

1. See [:material-code-braces: TcpRouteActionTypeDef](./type_defs.md#tcprouteactiontypedef) 
2. See [:material-code-braces: TcpRouteMatchTypeDef](./type_defs.md#tcproutematchtypedef) 
3. See [:material-code-braces: TcpTimeoutTypeDef](./type_defs.md#tcptimeouttypedef) 
## HttpGatewayRouteActionTypeDef

```python
# HttpGatewayRouteActionTypeDef definition

class HttpGatewayRouteActionTypeDef(TypedDict):
    target: GatewayRouteTargetTypeDef,  # (2)
    rewrite: NotRequired[HttpGatewayRouteRewriteTypeDef],  # (1)
```

1. See [:material-code-braces: HttpGatewayRouteRewriteTypeDef](./type_defs.md#httpgatewayrouterewritetypedef) 
2. See [:material-code-braces: GatewayRouteTargetTypeDef](./type_defs.md#gatewayroutetargettypedef) 
## FileAccessLogTypeDef

```python
# FileAccessLogTypeDef definition

class FileAccessLogTypeDef(TypedDict):
    path: str,
    format: NotRequired[LoggingFormatTypeDef],  # (1)
```

1. See [:material-code-braces: LoggingFormatTypeDef](./type_defs.md#loggingformattypedef) 
## VirtualGatewayFileAccessLogTypeDef

```python
# VirtualGatewayFileAccessLogTypeDef definition

class VirtualGatewayFileAccessLogTypeDef(TypedDict):
    path: str,
    format: NotRequired[LoggingFormatTypeDef],  # (1)
```

1. See [:material-code-braces: LoggingFormatTypeDef](./type_defs.md#loggingformattypedef) 
## VirtualRouterSpecTypeDef

```python
# VirtualRouterSpecTypeDef definition

class VirtualRouterSpecTypeDef(TypedDict):
    listeners: NotRequired[Sequence[VirtualRouterListenerTypeDef]],  # (1)
```

1. See [:material-code-braces: VirtualRouterListenerTypeDef](./type_defs.md#virtualrouterlistenertypedef) 
## CreateMeshInputRequestTypeDef

```python
# CreateMeshInputRequestTypeDef definition

class CreateMeshInputRequestTypeDef(TypedDict):
    meshName: str,
    clientToken: NotRequired[str],
    spec: NotRequired[MeshSpecTypeDef],  # (1)
    tags: NotRequired[Sequence[TagRefTypeDef]],  # (2)
```

1. See [:material-code-braces: MeshSpecTypeDef](./type_defs.md#meshspectypedef) 
2. See [:material-code-braces: TagRefTypeDef](./type_defs.md#tagreftypedef) 
## MeshDataTypeDef

```python
# MeshDataTypeDef definition

class MeshDataTypeDef(TypedDict):
    meshName: str,
    metadata: ResourceMetadataTypeDef,  # (1)
    spec: MeshSpecTypeDef,  # (2)
    status: MeshStatusTypeDef,  # (3)
```

1. See [:material-code-braces: ResourceMetadataTypeDef](./type_defs.md#resourcemetadatatypedef) 
2. See [:material-code-braces: MeshSpecTypeDef](./type_defs.md#meshspectypedef) 
3. See [:material-code-braces: MeshStatusTypeDef](./type_defs.md#meshstatustypedef) 
## UpdateMeshInputRequestTypeDef

```python
# UpdateMeshInputRequestTypeDef definition

class UpdateMeshInputRequestTypeDef(TypedDict):
    meshName: str,
    clientToken: NotRequired[str],
    spec: NotRequired[MeshSpecTypeDef],  # (1)
```

1. See [:material-code-braces: MeshSpecTypeDef](./type_defs.md#meshspectypedef) 
## ListenerTlsValidationContextTypeDef

```python
# ListenerTlsValidationContextTypeDef definition

class ListenerTlsValidationContextTypeDef(TypedDict):
    trust: ListenerTlsValidationContextTrustTypeDef,  # (2)
    subjectAlternativeNames: NotRequired[SubjectAlternativeNamesTypeDef],  # (1)
```

1. See [:material-code-braces: SubjectAlternativeNamesTypeDef](./type_defs.md#subjectalternativenamestypedef) 
2. See [:material-code-braces: ListenerTlsValidationContextTrustTypeDef](./type_defs.md#listenertlsvalidationcontexttrusttypedef) 
## TlsValidationContextTypeDef

```python
# TlsValidationContextTypeDef definition

class TlsValidationContextTypeDef(TypedDict):
    trust: TlsValidationContextTrustTypeDef,  # (2)
    subjectAlternativeNames: NotRequired[SubjectAlternativeNamesTypeDef],  # (1)
```

1. See [:material-code-braces: SubjectAlternativeNamesTypeDef](./type_defs.md#subjectalternativenamestypedef) 
2. See [:material-code-braces: TlsValidationContextTrustTypeDef](./type_defs.md#tlsvalidationcontexttrusttypedef) 
## VirtualGatewayListenerTlsValidationContextTypeDef

```python
# VirtualGatewayListenerTlsValidationContextTypeDef definition

class VirtualGatewayListenerTlsValidationContextTypeDef(TypedDict):
    trust: VirtualGatewayListenerTlsValidationContextTrustTypeDef,  # (2)
    subjectAlternativeNames: NotRequired[SubjectAlternativeNamesTypeDef],  # (1)
```

1. See [:material-code-braces: SubjectAlternativeNamesTypeDef](./type_defs.md#subjectalternativenamestypedef) 
2. See [:material-code-braces: VirtualGatewayListenerTlsValidationContextTrustTypeDef](./type_defs.md#virtualgatewaylistenertlsvalidationcontexttrusttypedef) 
## VirtualGatewayTlsValidationContextTypeDef

```python
# VirtualGatewayTlsValidationContextTypeDef definition

class VirtualGatewayTlsValidationContextTypeDef(TypedDict):
    trust: VirtualGatewayTlsValidationContextTrustTypeDef,  # (2)
    subjectAlternativeNames: NotRequired[SubjectAlternativeNamesTypeDef],  # (1)
```

1. See [:material-code-braces: SubjectAlternativeNamesTypeDef](./type_defs.md#subjectalternativenamestypedef) 
2. See [:material-code-braces: VirtualGatewayTlsValidationContextTrustTypeDef](./type_defs.md#virtualgatewaytlsvalidationcontexttrusttypedef) 
## VirtualServiceSpecTypeDef

```python
# VirtualServiceSpecTypeDef definition

class VirtualServiceSpecTypeDef(TypedDict):
    provider: NotRequired[VirtualServiceProviderTypeDef],  # (1)
```

1. See [:material-code-braces: VirtualServiceProviderTypeDef](./type_defs.md#virtualserviceprovidertypedef) 
## GrpcGatewayRouteMatchTypeDef

```python
# GrpcGatewayRouteMatchTypeDef definition

class GrpcGatewayRouteMatchTypeDef(TypedDict):
    hostname: NotRequired[GatewayRouteHostnameMatchTypeDef],  # (1)
    metadata: NotRequired[Sequence[GrpcGatewayRouteMetadataTypeDef]],  # (2)
    port: NotRequired[int],
    serviceName: NotRequired[str],
```

1. See [:material-code-braces: GatewayRouteHostnameMatchTypeDef](./type_defs.md#gatewayroutehostnamematchtypedef) 
2. See [:material-code-braces: GrpcGatewayRouteMetadataTypeDef](./type_defs.md#grpcgatewayroutemetadatatypedef) 
## GrpcRouteMatchTypeDef

```python
# GrpcRouteMatchTypeDef definition

class GrpcRouteMatchTypeDef(TypedDict):
    metadata: NotRequired[Sequence[GrpcRouteMetadataTypeDef]],  # (1)
    methodName: NotRequired[str],
    port: NotRequired[int],
    serviceName: NotRequired[str],
```

1. See [:material-code-braces: GrpcRouteMetadataTypeDef](./type_defs.md#grpcroutemetadatatypedef) 
## HttpGatewayRouteMatchTypeDef

```python
# HttpGatewayRouteMatchTypeDef definition

class HttpGatewayRouteMatchTypeDef(TypedDict):
    headers: NotRequired[Sequence[HttpGatewayRouteHeaderTypeDef]],  # (1)
    hostname: NotRequired[GatewayRouteHostnameMatchTypeDef],  # (2)
    method: NotRequired[HttpMethodType],  # (3)
    path: NotRequired[HttpPathMatchTypeDef],  # (4)
    port: NotRequired[int],
    prefix: NotRequired[str],
    queryParameters: NotRequired[Sequence[HttpQueryParameterTypeDef]],  # (5)
```

1. See [:material-code-braces: HttpGatewayRouteHeaderTypeDef](./type_defs.md#httpgatewayrouteheadertypedef) 
2. See [:material-code-braces: GatewayRouteHostnameMatchTypeDef](./type_defs.md#gatewayroutehostnamematchtypedef) 
3. See [:material-code-brackets: HttpMethodType](./literals.md#httpmethodtype) 
4. See [:material-code-braces: HttpPathMatchTypeDef](./type_defs.md#httppathmatchtypedef) 
5. See [:material-code-braces: HttpQueryParameterTypeDef](./type_defs.md#httpqueryparametertypedef) 
## HttpRouteMatchTypeDef

```python
# HttpRouteMatchTypeDef definition

class HttpRouteMatchTypeDef(TypedDict):
    headers: NotRequired[Sequence[HttpRouteHeaderTypeDef]],  # (1)
    method: NotRequired[HttpMethodType],  # (2)
    path: NotRequired[HttpPathMatchTypeDef],  # (3)
    port: NotRequired[int],
    prefix: NotRequired[str],
    queryParameters: NotRequired[Sequence[HttpQueryParameterTypeDef]],  # (4)
    scheme: NotRequired[HttpSchemeType],  # (5)
```

1. See [:material-code-braces: HttpRouteHeaderTypeDef](./type_defs.md#httprouteheadertypedef) 
2. See [:material-code-brackets: HttpMethodType](./literals.md#httpmethodtype) 
3. See [:material-code-braces: HttpPathMatchTypeDef](./type_defs.md#httppathmatchtypedef) 
4. See [:material-code-braces: HttpQueryParameterTypeDef](./type_defs.md#httpqueryparametertypedef) 
5. See [:material-code-brackets: HttpSchemeType](./literals.md#httpschemetype) 
## AccessLogTypeDef

```python
# AccessLogTypeDef definition

class AccessLogTypeDef(TypedDict):
    file: NotRequired[FileAccessLogTypeDef],  # (1)
```

1. See [:material-code-braces: FileAccessLogTypeDef](./type_defs.md#fileaccesslogtypedef) 
## VirtualGatewayAccessLogTypeDef

```python
# VirtualGatewayAccessLogTypeDef definition

class VirtualGatewayAccessLogTypeDef(TypedDict):
    file: NotRequired[VirtualGatewayFileAccessLogTypeDef],  # (1)
```

1. See [:material-code-braces: VirtualGatewayFileAccessLogTypeDef](./type_defs.md#virtualgatewayfileaccesslogtypedef) 
## CreateVirtualRouterInputRequestTypeDef

```python
# CreateVirtualRouterInputRequestTypeDef definition

class CreateVirtualRouterInputRequestTypeDef(TypedDict):
    meshName: str,
    spec: VirtualRouterSpecTypeDef,  # (1)
    virtualRouterName: str,
    clientToken: NotRequired[str],
    meshOwner: NotRequired[str],
    tags: NotRequired[Sequence[TagRefTypeDef]],  # (2)
```

1. See [:material-code-braces: VirtualRouterSpecTypeDef](./type_defs.md#virtualrouterspectypedef) 
2. See [:material-code-braces: TagRefTypeDef](./type_defs.md#tagreftypedef) 
## UpdateVirtualRouterInputRequestTypeDef

```python
# UpdateVirtualRouterInputRequestTypeDef definition

class UpdateVirtualRouterInputRequestTypeDef(TypedDict):
    meshName: str,
    spec: VirtualRouterSpecTypeDef,  # (1)
    virtualRouterName: str,
    clientToken: NotRequired[str],
    meshOwner: NotRequired[str],
```

1. See [:material-code-braces: VirtualRouterSpecTypeDef](./type_defs.md#virtualrouterspectypedef) 
## VirtualRouterDataTypeDef

```python
# VirtualRouterDataTypeDef definition

class VirtualRouterDataTypeDef(TypedDict):
    meshName: str,
    metadata: ResourceMetadataTypeDef,  # (1)
    spec: VirtualRouterSpecTypeDef,  # (2)
    status: VirtualRouterStatusTypeDef,  # (3)
    virtualRouterName: str,
```

1. See [:material-code-braces: ResourceMetadataTypeDef](./type_defs.md#resourcemetadatatypedef) 
2. See [:material-code-braces: VirtualRouterSpecTypeDef](./type_defs.md#virtualrouterspectypedef) 
3. See [:material-code-braces: VirtualRouterStatusTypeDef](./type_defs.md#virtualrouterstatustypedef) 
## CreateMeshOutputTypeDef

```python
# CreateMeshOutputTypeDef definition

class CreateMeshOutputTypeDef(TypedDict):
    mesh: MeshDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MeshDataTypeDef](./type_defs.md#meshdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteMeshOutputTypeDef

```python
# DeleteMeshOutputTypeDef definition

class DeleteMeshOutputTypeDef(TypedDict):
    mesh: MeshDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MeshDataTypeDef](./type_defs.md#meshdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeMeshOutputTypeDef

```python
# DescribeMeshOutputTypeDef definition

class DescribeMeshOutputTypeDef(TypedDict):
    mesh: MeshDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MeshDataTypeDef](./type_defs.md#meshdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMeshOutputTypeDef

```python
# UpdateMeshOutputTypeDef definition

class UpdateMeshOutputTypeDef(TypedDict):
    mesh: MeshDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MeshDataTypeDef](./type_defs.md#meshdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListenerTlsTypeDef

```python
# ListenerTlsTypeDef definition

class ListenerTlsTypeDef(TypedDict):
    certificate: ListenerTlsCertificateTypeDef,  # (1)
    mode: ListenerTlsModeType,  # (2)
    validation: NotRequired[ListenerTlsValidationContextTypeDef],  # (3)
```

1. See [:material-code-braces: ListenerTlsCertificateTypeDef](./type_defs.md#listenertlscertificatetypedef) 
2. See [:material-code-brackets: ListenerTlsModeType](./literals.md#listenertlsmodetype) 
3. See [:material-code-braces: ListenerTlsValidationContextTypeDef](./type_defs.md#listenertlsvalidationcontexttypedef) 
## ClientPolicyTlsTypeDef

```python
# ClientPolicyTlsTypeDef definition

class ClientPolicyTlsTypeDef(TypedDict):
    validation: TlsValidationContextTypeDef,  # (2)
    certificate: NotRequired[ClientTlsCertificateTypeDef],  # (1)
    enforce: NotRequired[bool],
    ports: NotRequired[Sequence[int]],
```

1. See [:material-code-braces: ClientTlsCertificateTypeDef](./type_defs.md#clienttlscertificatetypedef) 
2. See [:material-code-braces: TlsValidationContextTypeDef](./type_defs.md#tlsvalidationcontexttypedef) 
## VirtualGatewayListenerTlsTypeDef

```python
# VirtualGatewayListenerTlsTypeDef definition

class VirtualGatewayListenerTlsTypeDef(TypedDict):
    certificate: VirtualGatewayListenerTlsCertificateTypeDef,  # (1)
    mode: VirtualGatewayListenerTlsModeType,  # (2)
    validation: NotRequired[VirtualGatewayListenerTlsValidationContextTypeDef],  # (3)
```

1. See [:material-code-braces: VirtualGatewayListenerTlsCertificateTypeDef](./type_defs.md#virtualgatewaylistenertlscertificatetypedef) 
2. See [:material-code-brackets: VirtualGatewayListenerTlsModeType](./literals.md#virtualgatewaylistenertlsmodetype) 
3. See [:material-code-braces: VirtualGatewayListenerTlsValidationContextTypeDef](./type_defs.md#virtualgatewaylistenertlsvalidationcontexttypedef) 
## VirtualGatewayClientPolicyTlsTypeDef

```python
# VirtualGatewayClientPolicyTlsTypeDef definition

class VirtualGatewayClientPolicyTlsTypeDef(TypedDict):
    validation: VirtualGatewayTlsValidationContextTypeDef,  # (2)
    certificate: NotRequired[VirtualGatewayClientTlsCertificateTypeDef],  # (1)
    enforce: NotRequired[bool],
    ports: NotRequired[Sequence[int]],
```

1. See [:material-code-braces: VirtualGatewayClientTlsCertificateTypeDef](./type_defs.md#virtualgatewayclienttlscertificatetypedef) 
2. See [:material-code-braces: VirtualGatewayTlsValidationContextTypeDef](./type_defs.md#virtualgatewaytlsvalidationcontexttypedef) 
## CreateVirtualServiceInputRequestTypeDef

```python
# CreateVirtualServiceInputRequestTypeDef definition

class CreateVirtualServiceInputRequestTypeDef(TypedDict):
    meshName: str,
    spec: VirtualServiceSpecTypeDef,  # (1)
    virtualServiceName: str,
    clientToken: NotRequired[str],
    meshOwner: NotRequired[str],
    tags: NotRequired[Sequence[TagRefTypeDef]],  # (2)
```

1. See [:material-code-braces: VirtualServiceSpecTypeDef](./type_defs.md#virtualservicespectypedef) 
2. See [:material-code-braces: TagRefTypeDef](./type_defs.md#tagreftypedef) 
## UpdateVirtualServiceInputRequestTypeDef

```python
# UpdateVirtualServiceInputRequestTypeDef definition

class UpdateVirtualServiceInputRequestTypeDef(TypedDict):
    meshName: str,
    spec: VirtualServiceSpecTypeDef,  # (1)
    virtualServiceName: str,
    clientToken: NotRequired[str],
    meshOwner: NotRequired[str],
```

1. See [:material-code-braces: VirtualServiceSpecTypeDef](./type_defs.md#virtualservicespectypedef) 
## VirtualServiceDataTypeDef

```python
# VirtualServiceDataTypeDef definition

class VirtualServiceDataTypeDef(TypedDict):
    meshName: str,
    metadata: ResourceMetadataTypeDef,  # (1)
    spec: VirtualServiceSpecTypeDef,  # (2)
    status: VirtualServiceStatusTypeDef,  # (3)
    virtualServiceName: str,
```

1. See [:material-code-braces: ResourceMetadataTypeDef](./type_defs.md#resourcemetadatatypedef) 
2. See [:material-code-braces: VirtualServiceSpecTypeDef](./type_defs.md#virtualservicespectypedef) 
3. See [:material-code-braces: VirtualServiceStatusTypeDef](./type_defs.md#virtualservicestatustypedef) 
## GrpcGatewayRouteTypeDef

```python
# GrpcGatewayRouteTypeDef definition

class GrpcGatewayRouteTypeDef(TypedDict):
    action: GrpcGatewayRouteActionTypeDef,  # (1)
    match: GrpcGatewayRouteMatchTypeDef,  # (2)
```

1. See [:material-code-braces: GrpcGatewayRouteActionTypeDef](./type_defs.md#grpcgatewayrouteactiontypedef) 
2. See [:material-code-braces: GrpcGatewayRouteMatchTypeDef](./type_defs.md#grpcgatewayroutematchtypedef) 
## GrpcRouteTypeDef

```python
# GrpcRouteTypeDef definition

class GrpcRouteTypeDef(TypedDict):
    action: GrpcRouteActionTypeDef,  # (1)
    match: GrpcRouteMatchTypeDef,  # (2)
    retryPolicy: NotRequired[GrpcRetryPolicyTypeDef],  # (3)
    timeout: NotRequired[GrpcTimeoutTypeDef],  # (4)
```

1. See [:material-code-braces: GrpcRouteActionTypeDef](./type_defs.md#grpcrouteactiontypedef) 
2. See [:material-code-braces: GrpcRouteMatchTypeDef](./type_defs.md#grpcroutematchtypedef) 
3. See [:material-code-braces: GrpcRetryPolicyTypeDef](./type_defs.md#grpcretrypolicytypedef) 
4. See [:material-code-braces: GrpcTimeoutTypeDef](./type_defs.md#grpctimeouttypedef) 
## HttpGatewayRouteTypeDef

```python
# HttpGatewayRouteTypeDef definition

class HttpGatewayRouteTypeDef(TypedDict):
    action: HttpGatewayRouteActionTypeDef,  # (1)
    match: HttpGatewayRouteMatchTypeDef,  # (2)
```

1. See [:material-code-braces: HttpGatewayRouteActionTypeDef](./type_defs.md#httpgatewayrouteactiontypedef) 
2. See [:material-code-braces: HttpGatewayRouteMatchTypeDef](./type_defs.md#httpgatewayroutematchtypedef) 
## HttpRouteTypeDef

```python
# HttpRouteTypeDef definition

class HttpRouteTypeDef(TypedDict):
    action: HttpRouteActionTypeDef,  # (1)
    match: HttpRouteMatchTypeDef,  # (2)
    retryPolicy: NotRequired[HttpRetryPolicyTypeDef],  # (3)
    timeout: NotRequired[HttpTimeoutTypeDef],  # (4)
```

1. See [:material-code-braces: HttpRouteActionTypeDef](./type_defs.md#httprouteactiontypedef) 
2. See [:material-code-braces: HttpRouteMatchTypeDef](./type_defs.md#httproutematchtypedef) 
3. See [:material-code-braces: HttpRetryPolicyTypeDef](./type_defs.md#httpretrypolicytypedef) 
4. See [:material-code-braces: HttpTimeoutTypeDef](./type_defs.md#httptimeouttypedef) 
## LoggingTypeDef

```python
# LoggingTypeDef definition

class LoggingTypeDef(TypedDict):
    accessLog: NotRequired[AccessLogTypeDef],  # (1)
```

1. See [:material-code-braces: AccessLogTypeDef](./type_defs.md#accesslogtypedef) 
## VirtualGatewayLoggingTypeDef

```python
# VirtualGatewayLoggingTypeDef definition

class VirtualGatewayLoggingTypeDef(TypedDict):
    accessLog: NotRequired[VirtualGatewayAccessLogTypeDef],  # (1)
```

1. See [:material-code-braces: VirtualGatewayAccessLogTypeDef](./type_defs.md#virtualgatewayaccesslogtypedef) 
## CreateVirtualRouterOutputTypeDef

```python
# CreateVirtualRouterOutputTypeDef definition

class CreateVirtualRouterOutputTypeDef(TypedDict):
    virtualRouter: VirtualRouterDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualRouterDataTypeDef](./type_defs.md#virtualrouterdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteVirtualRouterOutputTypeDef

```python
# DeleteVirtualRouterOutputTypeDef definition

class DeleteVirtualRouterOutputTypeDef(TypedDict):
    virtualRouter: VirtualRouterDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualRouterDataTypeDef](./type_defs.md#virtualrouterdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeVirtualRouterOutputTypeDef

```python
# DescribeVirtualRouterOutputTypeDef definition

class DescribeVirtualRouterOutputTypeDef(TypedDict):
    virtualRouter: VirtualRouterDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualRouterDataTypeDef](./type_defs.md#virtualrouterdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateVirtualRouterOutputTypeDef

```python
# UpdateVirtualRouterOutputTypeDef definition

class UpdateVirtualRouterOutputTypeDef(TypedDict):
    virtualRouter: VirtualRouterDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualRouterDataTypeDef](./type_defs.md#virtualrouterdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListenerTypeDef

```python
# ListenerTypeDef definition

class ListenerTypeDef(TypedDict):
    portMapping: PortMappingTypeDef,  # (4)
    connectionPool: NotRequired[VirtualNodeConnectionPoolTypeDef],  # (1)
    healthCheck: NotRequired[HealthCheckPolicyTypeDef],  # (2)
    outlierDetection: NotRequired[OutlierDetectionTypeDef],  # (3)
    timeout: NotRequired[ListenerTimeoutTypeDef],  # (5)
    tls: NotRequired[ListenerTlsTypeDef],  # (6)
```

1. See [:material-code-braces: VirtualNodeConnectionPoolTypeDef](./type_defs.md#virtualnodeconnectionpooltypedef) 
2. See [:material-code-braces: HealthCheckPolicyTypeDef](./type_defs.md#healthcheckpolicytypedef) 
3. See [:material-code-braces: OutlierDetectionTypeDef](./type_defs.md#outlierdetectiontypedef) 
4. See [:material-code-braces: PortMappingTypeDef](./type_defs.md#portmappingtypedef) 
5. See [:material-code-braces: ListenerTimeoutTypeDef](./type_defs.md#listenertimeouttypedef) 
6. See [:material-code-braces: ListenerTlsTypeDef](./type_defs.md#listenertlstypedef) 
## ClientPolicyTypeDef

```python
# ClientPolicyTypeDef definition

class ClientPolicyTypeDef(TypedDict):
    tls: NotRequired[ClientPolicyTlsTypeDef],  # (1)
```

1. See [:material-code-braces: ClientPolicyTlsTypeDef](./type_defs.md#clientpolicytlstypedef) 
## VirtualGatewayListenerTypeDef

```python
# VirtualGatewayListenerTypeDef definition

class VirtualGatewayListenerTypeDef(TypedDict):
    portMapping: VirtualGatewayPortMappingTypeDef,  # (3)
    connectionPool: NotRequired[VirtualGatewayConnectionPoolTypeDef],  # (1)
    healthCheck: NotRequired[VirtualGatewayHealthCheckPolicyTypeDef],  # (2)
    tls: NotRequired[VirtualGatewayListenerTlsTypeDef],  # (4)
```

1. See [:material-code-braces: VirtualGatewayConnectionPoolTypeDef](./type_defs.md#virtualgatewayconnectionpooltypedef) 
2. See [:material-code-braces: VirtualGatewayHealthCheckPolicyTypeDef](./type_defs.md#virtualgatewayhealthcheckpolicytypedef) 
3. See [:material-code-braces: VirtualGatewayPortMappingTypeDef](./type_defs.md#virtualgatewayportmappingtypedef) 
4. See [:material-code-braces: VirtualGatewayListenerTlsTypeDef](./type_defs.md#virtualgatewaylistenertlstypedef) 
## VirtualGatewayClientPolicyTypeDef

```python
# VirtualGatewayClientPolicyTypeDef definition

class VirtualGatewayClientPolicyTypeDef(TypedDict):
    tls: NotRequired[VirtualGatewayClientPolicyTlsTypeDef],  # (1)
```

1. See [:material-code-braces: VirtualGatewayClientPolicyTlsTypeDef](./type_defs.md#virtualgatewayclientpolicytlstypedef) 
## CreateVirtualServiceOutputTypeDef

```python
# CreateVirtualServiceOutputTypeDef definition

class CreateVirtualServiceOutputTypeDef(TypedDict):
    virtualService: VirtualServiceDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualServiceDataTypeDef](./type_defs.md#virtualservicedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteVirtualServiceOutputTypeDef

```python
# DeleteVirtualServiceOutputTypeDef definition

class DeleteVirtualServiceOutputTypeDef(TypedDict):
    virtualService: VirtualServiceDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualServiceDataTypeDef](./type_defs.md#virtualservicedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeVirtualServiceOutputTypeDef

```python
# DescribeVirtualServiceOutputTypeDef definition

class DescribeVirtualServiceOutputTypeDef(TypedDict):
    virtualService: VirtualServiceDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualServiceDataTypeDef](./type_defs.md#virtualservicedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateVirtualServiceOutputTypeDef

```python
# UpdateVirtualServiceOutputTypeDef definition

class UpdateVirtualServiceOutputTypeDef(TypedDict):
    virtualService: VirtualServiceDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualServiceDataTypeDef](./type_defs.md#virtualservicedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GatewayRouteSpecTypeDef

```python
# GatewayRouteSpecTypeDef definition

class GatewayRouteSpecTypeDef(TypedDict):
    grpcRoute: NotRequired[GrpcGatewayRouteTypeDef],  # (1)
    http2Route: NotRequired[HttpGatewayRouteTypeDef],  # (2)
    httpRoute: NotRequired[HttpGatewayRouteTypeDef],  # (2)
    priority: NotRequired[int],
```

1. See [:material-code-braces: GrpcGatewayRouteTypeDef](./type_defs.md#grpcgatewayroutetypedef) 
2. See [:material-code-braces: HttpGatewayRouteTypeDef](./type_defs.md#httpgatewayroutetypedef) 
3. See [:material-code-braces: HttpGatewayRouteTypeDef](./type_defs.md#httpgatewayroutetypedef) 
## RouteSpecTypeDef

```python
# RouteSpecTypeDef definition

class RouteSpecTypeDef(TypedDict):
    grpcRoute: NotRequired[GrpcRouteTypeDef],  # (1)
    http2Route: NotRequired[HttpRouteTypeDef],  # (2)
    httpRoute: NotRequired[HttpRouteTypeDef],  # (2)
    priority: NotRequired[int],
    tcpRoute: NotRequired[TcpRouteTypeDef],  # (4)
```

1. See [:material-code-braces: GrpcRouteTypeDef](./type_defs.md#grpcroutetypedef) 
2. See [:material-code-braces: HttpRouteTypeDef](./type_defs.md#httproutetypedef) 
3. See [:material-code-braces: HttpRouteTypeDef](./type_defs.md#httproutetypedef) 
4. See [:material-code-braces: TcpRouteTypeDef](./type_defs.md#tcproutetypedef) 
## BackendDefaultsTypeDef

```python
# BackendDefaultsTypeDef definition

class BackendDefaultsTypeDef(TypedDict):
    clientPolicy: NotRequired[ClientPolicyTypeDef],  # (1)
```

1. See [:material-code-braces: ClientPolicyTypeDef](./type_defs.md#clientpolicytypedef) 
## VirtualServiceBackendTypeDef

```python
# VirtualServiceBackendTypeDef definition

class VirtualServiceBackendTypeDef(TypedDict):
    virtualServiceName: str,
    clientPolicy: NotRequired[ClientPolicyTypeDef],  # (1)
```

1. See [:material-code-braces: ClientPolicyTypeDef](./type_defs.md#clientpolicytypedef) 
## VirtualGatewayBackendDefaultsTypeDef

```python
# VirtualGatewayBackendDefaultsTypeDef definition

class VirtualGatewayBackendDefaultsTypeDef(TypedDict):
    clientPolicy: NotRequired[VirtualGatewayClientPolicyTypeDef],  # (1)
```

1. See [:material-code-braces: VirtualGatewayClientPolicyTypeDef](./type_defs.md#virtualgatewayclientpolicytypedef) 
## CreateGatewayRouteInputRequestTypeDef

```python
# CreateGatewayRouteInputRequestTypeDef definition

class CreateGatewayRouteInputRequestTypeDef(TypedDict):
    gatewayRouteName: str,
    meshName: str,
    spec: GatewayRouteSpecTypeDef,  # (1)
    virtualGatewayName: str,
    clientToken: NotRequired[str],
    meshOwner: NotRequired[str],
    tags: NotRequired[Sequence[TagRefTypeDef]],  # (2)
```

1. See [:material-code-braces: GatewayRouteSpecTypeDef](./type_defs.md#gatewayroutespectypedef) 
2. See [:material-code-braces: TagRefTypeDef](./type_defs.md#tagreftypedef) 
## GatewayRouteDataTypeDef

```python
# GatewayRouteDataTypeDef definition

class GatewayRouteDataTypeDef(TypedDict):
    gatewayRouteName: str,
    meshName: str,
    metadata: ResourceMetadataTypeDef,  # (1)
    spec: GatewayRouteSpecTypeDef,  # (2)
    status: GatewayRouteStatusTypeDef,  # (3)
    virtualGatewayName: str,
```

1. See [:material-code-braces: ResourceMetadataTypeDef](./type_defs.md#resourcemetadatatypedef) 
2. See [:material-code-braces: GatewayRouteSpecTypeDef](./type_defs.md#gatewayroutespectypedef) 
3. See [:material-code-braces: GatewayRouteStatusTypeDef](./type_defs.md#gatewayroutestatustypedef) 
## UpdateGatewayRouteInputRequestTypeDef

```python
# UpdateGatewayRouteInputRequestTypeDef definition

class UpdateGatewayRouteInputRequestTypeDef(TypedDict):
    gatewayRouteName: str,
    meshName: str,
    spec: GatewayRouteSpecTypeDef,  # (1)
    virtualGatewayName: str,
    clientToken: NotRequired[str],
    meshOwner: NotRequired[str],
```

1. See [:material-code-braces: GatewayRouteSpecTypeDef](./type_defs.md#gatewayroutespectypedef) 
## CreateRouteInputRequestTypeDef

```python
# CreateRouteInputRequestTypeDef definition

class CreateRouteInputRequestTypeDef(TypedDict):
    meshName: str,
    routeName: str,
    spec: RouteSpecTypeDef,  # (1)
    virtualRouterName: str,
    clientToken: NotRequired[str],
    meshOwner: NotRequired[str],
    tags: NotRequired[Sequence[TagRefTypeDef]],  # (2)
```

1. See [:material-code-braces: RouteSpecTypeDef](./type_defs.md#routespectypedef) 
2. See [:material-code-braces: TagRefTypeDef](./type_defs.md#tagreftypedef) 
## RouteDataTypeDef

```python
# RouteDataTypeDef definition

class RouteDataTypeDef(TypedDict):
    meshName: str,
    metadata: ResourceMetadataTypeDef,  # (1)
    routeName: str,
    spec: RouteSpecTypeDef,  # (2)
    status: RouteStatusTypeDef,  # (3)
    virtualRouterName: str,
```

1. See [:material-code-braces: ResourceMetadataTypeDef](./type_defs.md#resourcemetadatatypedef) 
2. See [:material-code-braces: RouteSpecTypeDef](./type_defs.md#routespectypedef) 
3. See [:material-code-braces: RouteStatusTypeDef](./type_defs.md#routestatustypedef) 
## UpdateRouteInputRequestTypeDef

```python
# UpdateRouteInputRequestTypeDef definition

class UpdateRouteInputRequestTypeDef(TypedDict):
    meshName: str,
    routeName: str,
    spec: RouteSpecTypeDef,  # (1)
    virtualRouterName: str,
    clientToken: NotRequired[str],
    meshOwner: NotRequired[str],
```

1. See [:material-code-braces: RouteSpecTypeDef](./type_defs.md#routespectypedef) 
## BackendTypeDef

```python
# BackendTypeDef definition

class BackendTypeDef(TypedDict):
    virtualService: NotRequired[VirtualServiceBackendTypeDef],  # (1)
```

1. See [:material-code-braces: VirtualServiceBackendTypeDef](./type_defs.md#virtualservicebackendtypedef) 
## VirtualGatewaySpecTypeDef

```python
# VirtualGatewaySpecTypeDef definition

class VirtualGatewaySpecTypeDef(TypedDict):
    listeners: Sequence[VirtualGatewayListenerTypeDef],  # (2)
    backendDefaults: NotRequired[VirtualGatewayBackendDefaultsTypeDef],  # (1)
    logging: NotRequired[VirtualGatewayLoggingTypeDef],  # (3)
```

1. See [:material-code-braces: VirtualGatewayBackendDefaultsTypeDef](./type_defs.md#virtualgatewaybackenddefaultstypedef) 
2. See [:material-code-braces: VirtualGatewayListenerTypeDef](./type_defs.md#virtualgatewaylistenertypedef) 
3. See [:material-code-braces: VirtualGatewayLoggingTypeDef](./type_defs.md#virtualgatewayloggingtypedef) 
## CreateGatewayRouteOutputTypeDef

```python
# CreateGatewayRouteOutputTypeDef definition

class CreateGatewayRouteOutputTypeDef(TypedDict):
    gatewayRoute: GatewayRouteDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GatewayRouteDataTypeDef](./type_defs.md#gatewayroutedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteGatewayRouteOutputTypeDef

```python
# DeleteGatewayRouteOutputTypeDef definition

class DeleteGatewayRouteOutputTypeDef(TypedDict):
    gatewayRoute: GatewayRouteDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GatewayRouteDataTypeDef](./type_defs.md#gatewayroutedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeGatewayRouteOutputTypeDef

```python
# DescribeGatewayRouteOutputTypeDef definition

class DescribeGatewayRouteOutputTypeDef(TypedDict):
    gatewayRoute: GatewayRouteDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GatewayRouteDataTypeDef](./type_defs.md#gatewayroutedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGatewayRouteOutputTypeDef

```python
# UpdateGatewayRouteOutputTypeDef definition

class UpdateGatewayRouteOutputTypeDef(TypedDict):
    gatewayRoute: GatewayRouteDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GatewayRouteDataTypeDef](./type_defs.md#gatewayroutedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRouteOutputTypeDef

```python
# CreateRouteOutputTypeDef definition

class CreateRouteOutputTypeDef(TypedDict):
    route: RouteDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RouteDataTypeDef](./type_defs.md#routedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRouteOutputTypeDef

```python
# DeleteRouteOutputTypeDef definition

class DeleteRouteOutputTypeDef(TypedDict):
    route: RouteDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RouteDataTypeDef](./type_defs.md#routedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRouteOutputTypeDef

```python
# DescribeRouteOutputTypeDef definition

class DescribeRouteOutputTypeDef(TypedDict):
    route: RouteDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RouteDataTypeDef](./type_defs.md#routedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRouteOutputTypeDef

```python
# UpdateRouteOutputTypeDef definition

class UpdateRouteOutputTypeDef(TypedDict):
    route: RouteDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RouteDataTypeDef](./type_defs.md#routedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VirtualNodeSpecTypeDef

```python
# VirtualNodeSpecTypeDef definition

class VirtualNodeSpecTypeDef(TypedDict):
    backendDefaults: NotRequired[BackendDefaultsTypeDef],  # (1)
    backends: NotRequired[Sequence[BackendTypeDef]],  # (2)
    listeners: NotRequired[Sequence[ListenerTypeDef]],  # (3)
    logging: NotRequired[LoggingTypeDef],  # (4)
    serviceDiscovery: NotRequired[ServiceDiscoveryTypeDef],  # (5)
```

1. See [:material-code-braces: BackendDefaultsTypeDef](./type_defs.md#backenddefaultstypedef) 
2. See [:material-code-braces: BackendTypeDef](./type_defs.md#backendtypedef) 
3. See [:material-code-braces: ListenerTypeDef](./type_defs.md#listenertypedef) 
4. See [:material-code-braces: LoggingTypeDef](./type_defs.md#loggingtypedef) 
5. See [:material-code-braces: ServiceDiscoveryTypeDef](./type_defs.md#servicediscoverytypedef) 
## CreateVirtualGatewayInputRequestTypeDef

```python
# CreateVirtualGatewayInputRequestTypeDef definition

class CreateVirtualGatewayInputRequestTypeDef(TypedDict):
    meshName: str,
    spec: VirtualGatewaySpecTypeDef,  # (1)
    virtualGatewayName: str,
    clientToken: NotRequired[str],
    meshOwner: NotRequired[str],
    tags: NotRequired[Sequence[TagRefTypeDef]],  # (2)
```

1. See [:material-code-braces: VirtualGatewaySpecTypeDef](./type_defs.md#virtualgatewayspectypedef) 
2. See [:material-code-braces: TagRefTypeDef](./type_defs.md#tagreftypedef) 
## UpdateVirtualGatewayInputRequestTypeDef

```python
# UpdateVirtualGatewayInputRequestTypeDef definition

class UpdateVirtualGatewayInputRequestTypeDef(TypedDict):
    meshName: str,
    spec: VirtualGatewaySpecTypeDef,  # (1)
    virtualGatewayName: str,
    clientToken: NotRequired[str],
    meshOwner: NotRequired[str],
```

1. See [:material-code-braces: VirtualGatewaySpecTypeDef](./type_defs.md#virtualgatewayspectypedef) 
## VirtualGatewayDataTypeDef

```python
# VirtualGatewayDataTypeDef definition

class VirtualGatewayDataTypeDef(TypedDict):
    meshName: str,
    metadata: ResourceMetadataTypeDef,  # (1)
    spec: VirtualGatewaySpecTypeDef,  # (2)
    status: VirtualGatewayStatusTypeDef,  # (3)
    virtualGatewayName: str,
```

1. See [:material-code-braces: ResourceMetadataTypeDef](./type_defs.md#resourcemetadatatypedef) 
2. See [:material-code-braces: VirtualGatewaySpecTypeDef](./type_defs.md#virtualgatewayspectypedef) 
3. See [:material-code-braces: VirtualGatewayStatusTypeDef](./type_defs.md#virtualgatewaystatustypedef) 
## CreateVirtualNodeInputRequestTypeDef

```python
# CreateVirtualNodeInputRequestTypeDef definition

class CreateVirtualNodeInputRequestTypeDef(TypedDict):
    meshName: str,
    spec: VirtualNodeSpecTypeDef,  # (1)
    virtualNodeName: str,
    clientToken: NotRequired[str],
    meshOwner: NotRequired[str],
    tags: NotRequired[Sequence[TagRefTypeDef]],  # (2)
```

1. See [:material-code-braces: VirtualNodeSpecTypeDef](./type_defs.md#virtualnodespectypedef) 
2. See [:material-code-braces: TagRefTypeDef](./type_defs.md#tagreftypedef) 
## UpdateVirtualNodeInputRequestTypeDef

```python
# UpdateVirtualNodeInputRequestTypeDef definition

class UpdateVirtualNodeInputRequestTypeDef(TypedDict):
    meshName: str,
    spec: VirtualNodeSpecTypeDef,  # (1)
    virtualNodeName: str,
    clientToken: NotRequired[str],
    meshOwner: NotRequired[str],
```

1. See [:material-code-braces: VirtualNodeSpecTypeDef](./type_defs.md#virtualnodespectypedef) 
## VirtualNodeDataTypeDef

```python
# VirtualNodeDataTypeDef definition

class VirtualNodeDataTypeDef(TypedDict):
    meshName: str,
    metadata: ResourceMetadataTypeDef,  # (1)
    spec: VirtualNodeSpecTypeDef,  # (2)
    status: VirtualNodeStatusTypeDef,  # (3)
    virtualNodeName: str,
```

1. See [:material-code-braces: ResourceMetadataTypeDef](./type_defs.md#resourcemetadatatypedef) 
2. See [:material-code-braces: VirtualNodeSpecTypeDef](./type_defs.md#virtualnodespectypedef) 
3. See [:material-code-braces: VirtualNodeStatusTypeDef](./type_defs.md#virtualnodestatustypedef) 
## CreateVirtualGatewayOutputTypeDef

```python
# CreateVirtualGatewayOutputTypeDef definition

class CreateVirtualGatewayOutputTypeDef(TypedDict):
    virtualGateway: VirtualGatewayDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualGatewayDataTypeDef](./type_defs.md#virtualgatewaydatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteVirtualGatewayOutputTypeDef

```python
# DeleteVirtualGatewayOutputTypeDef definition

class DeleteVirtualGatewayOutputTypeDef(TypedDict):
    virtualGateway: VirtualGatewayDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualGatewayDataTypeDef](./type_defs.md#virtualgatewaydatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeVirtualGatewayOutputTypeDef

```python
# DescribeVirtualGatewayOutputTypeDef definition

class DescribeVirtualGatewayOutputTypeDef(TypedDict):
    virtualGateway: VirtualGatewayDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualGatewayDataTypeDef](./type_defs.md#virtualgatewaydatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateVirtualGatewayOutputTypeDef

```python
# UpdateVirtualGatewayOutputTypeDef definition

class UpdateVirtualGatewayOutputTypeDef(TypedDict):
    virtualGateway: VirtualGatewayDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualGatewayDataTypeDef](./type_defs.md#virtualgatewaydatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateVirtualNodeOutputTypeDef

```python
# CreateVirtualNodeOutputTypeDef definition

class CreateVirtualNodeOutputTypeDef(TypedDict):
    virtualNode: VirtualNodeDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualNodeDataTypeDef](./type_defs.md#virtualnodedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteVirtualNodeOutputTypeDef

```python
# DeleteVirtualNodeOutputTypeDef definition

class DeleteVirtualNodeOutputTypeDef(TypedDict):
    virtualNode: VirtualNodeDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualNodeDataTypeDef](./type_defs.md#virtualnodedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeVirtualNodeOutputTypeDef

```python
# DescribeVirtualNodeOutputTypeDef definition

class DescribeVirtualNodeOutputTypeDef(TypedDict):
    virtualNode: VirtualNodeDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualNodeDataTypeDef](./type_defs.md#virtualnodedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateVirtualNodeOutputTypeDef

```python
# UpdateVirtualNodeOutputTypeDef definition

class UpdateVirtualNodeOutputTypeDef(TypedDict):
    virtualNode: VirtualNodeDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VirtualNodeDataTypeDef](./type_defs.md#virtualnodedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
