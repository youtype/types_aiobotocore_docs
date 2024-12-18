# AppMesh module

> [Index](../README.md) > AppMesh


!!! note ""

    Auto-generated documentation for [AppMesh](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#appmesh)
    type annotations stubs module [types-aiobotocore-appmesh](https://pypi.org/project/types-aiobotocore-appmesh/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `AppMesh` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `AppMesh` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[appmesh]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[appmesh]'

# standalone installation
python -m pip install types-aiobotocore-appmesh
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-appmesh
```

## Usage

Code samples can be found in [Examples](./usage.md).

## AppMeshClient

Type annotations and code completion for  `#!python session.create_client("appmesh")` as [AppMeshClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)

```python
# AppMeshClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_appmesh.client import AppMeshClient


session = get_session()
async with session.create_client("appmesh") as client:
    client: AppMeshClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("appmesh").get_paginator("...")`.

```python
# ListGatewayRoutesPaginator usage example

from types_aiobotocore_appmesh.paginator import ListGatewayRoutesPaginator

def get_list_gateway_routes_paginator() -> ListGatewayRoutesPaginator:
    return client.get_paginator("list_gateway_routes"))
```

- [ListGatewayRoutesPaginator](./paginators.md#listgatewayroutespaginator)
- [ListMeshesPaginator](./paginators.md#listmeshespaginator)
- [ListRoutesPaginator](./paginators.md#listroutespaginator)
- [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
- [ListVirtualGatewaysPaginator](./paginators.md#listvirtualgatewayspaginator)
- [ListVirtualNodesPaginator](./paginators.md#listvirtualnodespaginator)
- [ListVirtualRoutersPaginator](./paginators.md#listvirtualrouterspaginator)
- [ListVirtualServicesPaginator](./paginators.md#listvirtualservicespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# DefaultGatewayRouteRewriteType usage example

from types_aiobotocore_appmesh.literals import DefaultGatewayRouteRewriteType

def get_value() -> DefaultGatewayRouteRewriteType:
    return "DISABLED"
```

- [DefaultGatewayRouteRewriteType](./literals.md#defaultgatewayrouterewritetype)
- [DnsResponseTypeType](./literals.md#dnsresponsetypetype)
- [DurationUnitType](./literals.md#durationunittype)
- [EgressFilterTypeType](./literals.md#egressfiltertypetype)
- [GatewayRouteStatusCodeType](./literals.md#gatewayroutestatuscodetype)
- [GrpcRetryPolicyEventType](./literals.md#grpcretrypolicyeventtype)
- [HttpMethodType](./literals.md#httpmethodtype)
- [HttpSchemeType](./literals.md#httpschemetype)
- [IpPreferenceType](./literals.md#ippreferencetype)
- [ListGatewayRoutesPaginatorName](./literals.md#listgatewayroutespaginatorname)
- [ListMeshesPaginatorName](./literals.md#listmeshespaginatorname)
- [ListRoutesPaginatorName](./literals.md#listroutespaginatorname)
- [ListTagsForResourcePaginatorName](./literals.md#listtagsforresourcepaginatorname)
- [ListVirtualGatewaysPaginatorName](./literals.md#listvirtualgatewayspaginatorname)
- [ListVirtualNodesPaginatorName](./literals.md#listvirtualnodespaginatorname)
- [ListVirtualRoutersPaginatorName](./literals.md#listvirtualrouterspaginatorname)
- [ListVirtualServicesPaginatorName](./literals.md#listvirtualservicespaginatorname)
- [ListenerTlsModeType](./literals.md#listenertlsmodetype)
- [MeshStatusCodeType](./literals.md#meshstatuscodetype)
- [PortProtocolType](./literals.md#portprotocoltype)
- [RouteStatusCodeType](./literals.md#routestatuscodetype)
- [TcpRetryPolicyEventType](./literals.md#tcpretrypolicyeventtype)
- [VirtualGatewayListenerTlsModeType](./literals.md#virtualgatewaylistenertlsmodetype)
- [VirtualGatewayPortProtocolType](./literals.md#virtualgatewayportprotocoltype)
- [VirtualGatewayStatusCodeType](./literals.md#virtualgatewaystatuscodetype)
- [VirtualNodeStatusCodeType](./literals.md#virtualnodestatuscodetype)
- [VirtualRouterStatusCodeType](./literals.md#virtualrouterstatuscodetype)
- [VirtualServiceStatusCodeType](./literals.md#virtualservicestatuscodetype)
- [AppMeshServiceName](./literals.md#appmeshservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AwsCloudMapInstanceAttributeTypeDef](./type_defs.md#awscloudmapinstanceattributetypedef)
- [ListenerTlsFileCertificateTypeDef](./type_defs.md#listenertlsfilecertificatetypedef)
- [ListenerTlsSdsCertificateTypeDef](./type_defs.md#listenertlssdscertificatetypedef)
- [TagRefTypeDef](./type_defs.md#tagreftypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteGatewayRouteInputRequestTypeDef](./type_defs.md#deletegatewayrouteinputrequesttypedef)
- [DeleteMeshInputRequestTypeDef](./type_defs.md#deletemeshinputrequesttypedef)
- [DeleteRouteInputRequestTypeDef](./type_defs.md#deleterouteinputrequesttypedef)
- [DeleteVirtualGatewayInputRequestTypeDef](./type_defs.md#deletevirtualgatewayinputrequesttypedef)
- [DeleteVirtualNodeInputRequestTypeDef](./type_defs.md#deletevirtualnodeinputrequesttypedef)
- [DeleteVirtualRouterInputRequestTypeDef](./type_defs.md#deletevirtualrouterinputrequesttypedef)
- [DeleteVirtualServiceInputRequestTypeDef](./type_defs.md#deletevirtualserviceinputrequesttypedef)
- [DescribeGatewayRouteInputRequestTypeDef](./type_defs.md#describegatewayrouteinputrequesttypedef)
- [DescribeMeshInputRequestTypeDef](./type_defs.md#describemeshinputrequesttypedef)
- [DescribeRouteInputRequestTypeDef](./type_defs.md#describerouteinputrequesttypedef)
- [DescribeVirtualGatewayInputRequestTypeDef](./type_defs.md#describevirtualgatewayinputrequesttypedef)
- [DescribeVirtualNodeInputRequestTypeDef](./type_defs.md#describevirtualnodeinputrequesttypedef)
- [DescribeVirtualRouterInputRequestTypeDef](./type_defs.md#describevirtualrouterinputrequesttypedef)
- [DescribeVirtualServiceInputRequestTypeDef](./type_defs.md#describevirtualserviceinputrequesttypedef)
- [DnsServiceDiscoveryTypeDef](./type_defs.md#dnsservicediscoverytypedef)
- [DurationTypeDef](./type_defs.md#durationtypedef)
- [EgressFilterTypeDef](./type_defs.md#egressfiltertypedef)
- [GatewayRouteStatusTypeDef](./type_defs.md#gatewayroutestatustypedef)
- [ResourceMetadataTypeDef](./type_defs.md#resourcemetadatatypedef)
- [GatewayRouteHostnameMatchTypeDef](./type_defs.md#gatewayroutehostnamematchtypedef)
- [GatewayRouteHostnameRewriteTypeDef](./type_defs.md#gatewayroutehostnamerewritetypedef)
- [GatewayRouteRefTypeDef](./type_defs.md#gatewayroutereftypedef)
- [GatewayRouteVirtualServiceTypeDef](./type_defs.md#gatewayroutevirtualservicetypedef)
- [MatchRangeTypeDef](./type_defs.md#matchrangetypedef)
- [WeightedTargetTypeDef](./type_defs.md#weightedtargettypedef)
- [HealthCheckPolicyTypeDef](./type_defs.md#healthcheckpolicytypedef)
- [HttpPathMatchTypeDef](./type_defs.md#httppathmatchtypedef)
- [HttpGatewayRoutePathRewriteTypeDef](./type_defs.md#httpgatewayroutepathrewritetypedef)
- [HttpGatewayRoutePrefixRewriteTypeDef](./type_defs.md#httpgatewayrouteprefixrewritetypedef)
- [QueryParameterMatchTypeDef](./type_defs.md#queryparametermatchtypedef)
- [JsonFormatRefTypeDef](./type_defs.md#jsonformatreftypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListGatewayRoutesInputRequestTypeDef](./type_defs.md#listgatewayroutesinputrequesttypedef)
- [ListMeshesInputRequestTypeDef](./type_defs.md#listmeshesinputrequesttypedef)
- [MeshRefTypeDef](./type_defs.md#meshreftypedef)
- [ListRoutesInputRequestTypeDef](./type_defs.md#listroutesinputrequesttypedef)
- [RouteRefTypeDef](./type_defs.md#routereftypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [ListVirtualGatewaysInputRequestTypeDef](./type_defs.md#listvirtualgatewaysinputrequesttypedef)
- [VirtualGatewayRefTypeDef](./type_defs.md#virtualgatewayreftypedef)
- [ListVirtualNodesInputRequestTypeDef](./type_defs.md#listvirtualnodesinputrequesttypedef)
- [VirtualNodeRefTypeDef](./type_defs.md#virtualnodereftypedef)
- [ListVirtualRoutersInputRequestTypeDef](./type_defs.md#listvirtualroutersinputrequesttypedef)
- [VirtualRouterRefTypeDef](./type_defs.md#virtualrouterreftypedef)
- [ListVirtualServicesInputRequestTypeDef](./type_defs.md#listvirtualservicesinputrequesttypedef)
- [VirtualServiceRefTypeDef](./type_defs.md#virtualservicereftypedef)
- [PortMappingTypeDef](./type_defs.md#portmappingtypedef)
- [ListenerTlsAcmCertificateTypeDef](./type_defs.md#listenertlsacmcertificatetypedef)
- [TlsValidationContextFileTrustTypeDef](./type_defs.md#tlsvalidationcontextfiletrusttypedef)
- [TlsValidationContextSdsTrustTypeDef](./type_defs.md#tlsvalidationcontextsdstrusttypedef)
- [MeshStatusTypeDef](./type_defs.md#meshstatustypedef)
- [MeshServiceDiscoveryTypeDef](./type_defs.md#meshservicediscoverytypedef)
- [RouteStatusTypeDef](./type_defs.md#routestatustypedef)
- [SubjectAlternativeNameMatchersOutputTypeDef](./type_defs.md#subjectalternativenamematchersoutputtypedef)
- [SubjectAlternativeNameMatchersTypeDef](./type_defs.md#subjectalternativenamematcherstypedef)
- [TcpRouteMatchTypeDef](./type_defs.md#tcproutematchtypedef)
- [TlsValidationContextAcmTrustOutputTypeDef](./type_defs.md#tlsvalidationcontextacmtrustoutputtypedef)
- [TlsValidationContextAcmTrustTypeDef](./type_defs.md#tlsvalidationcontextacmtrusttypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [VirtualGatewayListenerTlsFileCertificateTypeDef](./type_defs.md#virtualgatewaylistenertlsfilecertificatetypedef)
- [VirtualGatewayListenerTlsSdsCertificateTypeDef](./type_defs.md#virtualgatewaylistenertlssdscertificatetypedef)
- [VirtualGatewayGrpcConnectionPoolTypeDef](./type_defs.md#virtualgatewaygrpcconnectionpooltypedef)
- [VirtualGatewayHttp2ConnectionPoolTypeDef](./type_defs.md#virtualgatewayhttp2connectionpooltypedef)
- [VirtualGatewayHttpConnectionPoolTypeDef](./type_defs.md#virtualgatewayhttpconnectionpooltypedef)
- [VirtualGatewayStatusTypeDef](./type_defs.md#virtualgatewaystatustypedef)
- [VirtualGatewayHealthCheckPolicyTypeDef](./type_defs.md#virtualgatewayhealthcheckpolicytypedef)
- [VirtualGatewayPortMappingTypeDef](./type_defs.md#virtualgatewayportmappingtypedef)
- [VirtualGatewayListenerTlsAcmCertificateTypeDef](./type_defs.md#virtualgatewaylistenertlsacmcertificatetypedef)
- [VirtualGatewayTlsValidationContextFileTrustTypeDef](./type_defs.md#virtualgatewaytlsvalidationcontextfiletrusttypedef)
- [VirtualGatewayTlsValidationContextSdsTrustTypeDef](./type_defs.md#virtualgatewaytlsvalidationcontextsdstrusttypedef)
- [VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef](./type_defs.md#virtualgatewaytlsvalidationcontextacmtrustoutputtypedef)
- [VirtualGatewayTlsValidationContextAcmTrustTypeDef](./type_defs.md#virtualgatewaytlsvalidationcontextacmtrusttypedef)
- [VirtualNodeGrpcConnectionPoolTypeDef](./type_defs.md#virtualnodegrpcconnectionpooltypedef)
- [VirtualNodeHttp2ConnectionPoolTypeDef](./type_defs.md#virtualnodehttp2connectionpooltypedef)
- [VirtualNodeHttpConnectionPoolTypeDef](./type_defs.md#virtualnodehttpconnectionpooltypedef)
- [VirtualNodeTcpConnectionPoolTypeDef](./type_defs.md#virtualnodetcpconnectionpooltypedef)
- [VirtualNodeStatusTypeDef](./type_defs.md#virtualnodestatustypedef)
- [VirtualNodeServiceProviderTypeDef](./type_defs.md#virtualnodeserviceprovidertypedef)
- [VirtualRouterStatusTypeDef](./type_defs.md#virtualrouterstatustypedef)
- [VirtualRouterServiceProviderTypeDef](./type_defs.md#virtualrouterserviceprovidertypedef)
- [VirtualServiceStatusTypeDef](./type_defs.md#virtualservicestatustypedef)
- [AwsCloudMapServiceDiscoveryOutputTypeDef](./type_defs.md#awscloudmapservicediscoveryoutputtypedef)
- [AwsCloudMapServiceDiscoveryTypeDef](./type_defs.md#awscloudmapservicediscoverytypedef)
- [ClientTlsCertificateTypeDef](./type_defs.md#clienttlscertificatetypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [GrpcRetryPolicyOutputTypeDef](./type_defs.md#grpcretrypolicyoutputtypedef)
- [GrpcRetryPolicyTypeDef](./type_defs.md#grpcretrypolicytypedef)
- [GrpcTimeoutTypeDef](./type_defs.md#grpctimeouttypedef)
- [HttpRetryPolicyOutputTypeDef](./type_defs.md#httpretrypolicyoutputtypedef)
- [HttpRetryPolicyTypeDef](./type_defs.md#httpretrypolicytypedef)
- [HttpTimeoutTypeDef](./type_defs.md#httptimeouttypedef)
- [OutlierDetectionTypeDef](./type_defs.md#outlierdetectiontypedef)
- [TcpTimeoutTypeDef](./type_defs.md#tcptimeouttypedef)
- [GrpcGatewayRouteRewriteTypeDef](./type_defs.md#grpcgatewayrouterewritetypedef)
- [ListGatewayRoutesOutputTypeDef](./type_defs.md#listgatewayroutesoutputtypedef)
- [GatewayRouteTargetTypeDef](./type_defs.md#gatewayroutetargettypedef)
- [GrpcMetadataMatchMethodTypeDef](./type_defs.md#grpcmetadatamatchmethodtypedef)
- [GrpcRouteMetadataMatchMethodTypeDef](./type_defs.md#grpcroutemetadatamatchmethodtypedef)
- [HeaderMatchMethodTypeDef](./type_defs.md#headermatchmethodtypedef)
- [GrpcRouteActionOutputTypeDef](./type_defs.md#grpcrouteactionoutputtypedef)
- [GrpcRouteActionTypeDef](./type_defs.md#grpcrouteactiontypedef)
- [HttpRouteActionOutputTypeDef](./type_defs.md#httprouteactionoutputtypedef)
- [HttpRouteActionTypeDef](./type_defs.md#httprouteactiontypedef)
- [TcpRouteActionOutputTypeDef](./type_defs.md#tcprouteactionoutputtypedef)
- [TcpRouteActionTypeDef](./type_defs.md#tcprouteactiontypedef)
- [HttpGatewayRouteRewriteTypeDef](./type_defs.md#httpgatewayrouterewritetypedef)
- [HttpQueryParameterTypeDef](./type_defs.md#httpqueryparametertypedef)
- [LoggingFormatOutputTypeDef](./type_defs.md#loggingformatoutputtypedef)
- [LoggingFormatTypeDef](./type_defs.md#loggingformattypedef)
- [ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef](./type_defs.md#listgatewayroutesinputlistgatewayroutespaginatetypedef)
- [ListMeshesInputListMeshesPaginateTypeDef](./type_defs.md#listmeshesinputlistmeshespaginatetypedef)
- [ListRoutesInputListRoutesPaginateTypeDef](./type_defs.md#listroutesinputlistroutespaginatetypedef)
- [ListTagsForResourceInputListTagsForResourcePaginateTypeDef](./type_defs.md#listtagsforresourceinputlisttagsforresourcepaginatetypedef)
- [ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef](./type_defs.md#listvirtualgatewaysinputlistvirtualgatewayspaginatetypedef)
- [ListVirtualNodesInputListVirtualNodesPaginateTypeDef](./type_defs.md#listvirtualnodesinputlistvirtualnodespaginatetypedef)
- [ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef](./type_defs.md#listvirtualroutersinputlistvirtualrouterspaginatetypedef)
- [ListVirtualServicesInputListVirtualServicesPaginateTypeDef](./type_defs.md#listvirtualservicesinputlistvirtualservicespaginatetypedef)
- [ListMeshesOutputTypeDef](./type_defs.md#listmeshesoutputtypedef)
- [ListRoutesOutputTypeDef](./type_defs.md#listroutesoutputtypedef)
- [ListVirtualGatewaysOutputTypeDef](./type_defs.md#listvirtualgatewaysoutputtypedef)
- [ListVirtualNodesOutputTypeDef](./type_defs.md#listvirtualnodesoutputtypedef)
- [ListVirtualRoutersOutputTypeDef](./type_defs.md#listvirtualroutersoutputtypedef)
- [ListVirtualServicesOutputTypeDef](./type_defs.md#listvirtualservicesoutputtypedef)
- [VirtualRouterListenerTypeDef](./type_defs.md#virtualrouterlistenertypedef)
- [ListenerTlsCertificateTypeDef](./type_defs.md#listenertlscertificatetypedef)
- [ListenerTlsValidationContextTrustTypeDef](./type_defs.md#listenertlsvalidationcontexttrusttypedef)
- [MeshSpecTypeDef](./type_defs.md#meshspectypedef)
- [SubjectAlternativeNamesOutputTypeDef](./type_defs.md#subjectalternativenamesoutputtypedef)
- [SubjectAlternativeNameMatchersUnionTypeDef](./type_defs.md#subjectalternativenamematchersuniontypedef)
- [TlsValidationContextTrustOutputTypeDef](./type_defs.md#tlsvalidationcontexttrustoutputtypedef)
- [TlsValidationContextAcmTrustUnionTypeDef](./type_defs.md#tlsvalidationcontextacmtrustuniontypedef)
- [VirtualGatewayClientTlsCertificateTypeDef](./type_defs.md#virtualgatewayclienttlscertificatetypedef)
- [VirtualGatewayConnectionPoolTypeDef](./type_defs.md#virtualgatewayconnectionpooltypedef)
- [VirtualGatewayListenerTlsCertificateTypeDef](./type_defs.md#virtualgatewaylistenertlscertificatetypedef)
- [VirtualGatewayListenerTlsValidationContextTrustTypeDef](./type_defs.md#virtualgatewaylistenertlsvalidationcontexttrusttypedef)
- [VirtualGatewayTlsValidationContextTrustOutputTypeDef](./type_defs.md#virtualgatewaytlsvalidationcontexttrustoutputtypedef)
- [VirtualGatewayTlsValidationContextAcmTrustUnionTypeDef](./type_defs.md#virtualgatewaytlsvalidationcontextacmtrustuniontypedef)
- [VirtualNodeConnectionPoolTypeDef](./type_defs.md#virtualnodeconnectionpooltypedef)
- [VirtualServiceProviderTypeDef](./type_defs.md#virtualserviceprovidertypedef)
- [ServiceDiscoveryOutputTypeDef](./type_defs.md#servicediscoveryoutputtypedef)
- [AwsCloudMapServiceDiscoveryUnionTypeDef](./type_defs.md#awscloudmapservicediscoveryuniontypedef)
- [GrpcRetryPolicyUnionTypeDef](./type_defs.md#grpcretrypolicyuniontypedef)
- [HttpRetryPolicyUnionTypeDef](./type_defs.md#httpretrypolicyuniontypedef)
- [ListenerTimeoutTypeDef](./type_defs.md#listenertimeouttypedef)
- [GrpcGatewayRouteActionTypeDef](./type_defs.md#grpcgatewayrouteactiontypedef)
- [GrpcGatewayRouteMetadataTypeDef](./type_defs.md#grpcgatewayroutemetadatatypedef)
- [GrpcRouteMetadataTypeDef](./type_defs.md#grpcroutemetadatatypedef)
- [HttpGatewayRouteHeaderTypeDef](./type_defs.md#httpgatewayrouteheadertypedef)
- [HttpRouteHeaderTypeDef](./type_defs.md#httprouteheadertypedef)
- [GrpcRouteActionUnionTypeDef](./type_defs.md#grpcrouteactionuniontypedef)
- [HttpRouteActionUnionTypeDef](./type_defs.md#httprouteactionuniontypedef)
- [TcpRouteOutputTypeDef](./type_defs.md#tcprouteoutputtypedef)
- [TcpRouteActionUnionTypeDef](./type_defs.md#tcprouteactionuniontypedef)
- [HttpGatewayRouteActionTypeDef](./type_defs.md#httpgatewayrouteactiontypedef)
- [FileAccessLogOutputTypeDef](./type_defs.md#fileaccesslogoutputtypedef)
- [VirtualGatewayFileAccessLogOutputTypeDef](./type_defs.md#virtualgatewayfileaccesslogoutputtypedef)
- [LoggingFormatUnionTypeDef](./type_defs.md#loggingformatuniontypedef)
- [VirtualRouterSpecOutputTypeDef](./type_defs.md#virtualrouterspecoutputtypedef)
- [VirtualRouterSpecTypeDef](./type_defs.md#virtualrouterspectypedef)
- [CreateMeshInputRequestTypeDef](./type_defs.md#createmeshinputrequesttypedef)
- [MeshDataTypeDef](./type_defs.md#meshdatatypedef)
- [UpdateMeshInputRequestTypeDef](./type_defs.md#updatemeshinputrequesttypedef)
- [ListenerTlsValidationContextOutputTypeDef](./type_defs.md#listenertlsvalidationcontextoutputtypedef)
- [SubjectAlternativeNamesTypeDef](./type_defs.md#subjectalternativenamestypedef)
- [TlsValidationContextOutputTypeDef](./type_defs.md#tlsvalidationcontextoutputtypedef)
- [TlsValidationContextTrustTypeDef](./type_defs.md#tlsvalidationcontexttrusttypedef)
- [VirtualGatewayListenerTlsValidationContextOutputTypeDef](./type_defs.md#virtualgatewaylistenertlsvalidationcontextoutputtypedef)
- [VirtualGatewayTlsValidationContextOutputTypeDef](./type_defs.md#virtualgatewaytlsvalidationcontextoutputtypedef)
- [VirtualGatewayTlsValidationContextTrustTypeDef](./type_defs.md#virtualgatewaytlsvalidationcontexttrusttypedef)
- [VirtualServiceSpecTypeDef](./type_defs.md#virtualservicespectypedef)
- [ServiceDiscoveryTypeDef](./type_defs.md#servicediscoverytypedef)
- [GrpcGatewayRouteMatchOutputTypeDef](./type_defs.md#grpcgatewayroutematchoutputtypedef)
- [GrpcGatewayRouteMatchTypeDef](./type_defs.md#grpcgatewayroutematchtypedef)
- [GrpcRouteMatchOutputTypeDef](./type_defs.md#grpcroutematchoutputtypedef)
- [GrpcRouteMatchTypeDef](./type_defs.md#grpcroutematchtypedef)
- [HttpGatewayRouteMatchOutputTypeDef](./type_defs.md#httpgatewayroutematchoutputtypedef)
- [HttpGatewayRouteMatchTypeDef](./type_defs.md#httpgatewayroutematchtypedef)
- [HttpRouteMatchOutputTypeDef](./type_defs.md#httproutematchoutputtypedef)
- [HttpRouteMatchTypeDef](./type_defs.md#httproutematchtypedef)
- [TcpRouteTypeDef](./type_defs.md#tcproutetypedef)
- [AccessLogOutputTypeDef](./type_defs.md#accesslogoutputtypedef)
- [VirtualGatewayAccessLogOutputTypeDef](./type_defs.md#virtualgatewayaccesslogoutputtypedef)
- [FileAccessLogTypeDef](./type_defs.md#fileaccesslogtypedef)
- [VirtualGatewayFileAccessLogTypeDef](./type_defs.md#virtualgatewayfileaccesslogtypedef)
- [VirtualRouterDataTypeDef](./type_defs.md#virtualrouterdatatypedef)
- [CreateVirtualRouterInputRequestTypeDef](./type_defs.md#createvirtualrouterinputrequesttypedef)
- [UpdateVirtualRouterInputRequestTypeDef](./type_defs.md#updatevirtualrouterinputrequesttypedef)
- [CreateMeshOutputTypeDef](./type_defs.md#createmeshoutputtypedef)
- [DeleteMeshOutputTypeDef](./type_defs.md#deletemeshoutputtypedef)
- [DescribeMeshOutputTypeDef](./type_defs.md#describemeshoutputtypedef)
- [UpdateMeshOutputTypeDef](./type_defs.md#updatemeshoutputtypedef)
- [ListenerTlsOutputTypeDef](./type_defs.md#listenertlsoutputtypedef)
- [SubjectAlternativeNamesUnionTypeDef](./type_defs.md#subjectalternativenamesuniontypedef)
- [ClientPolicyTlsOutputTypeDef](./type_defs.md#clientpolicytlsoutputtypedef)
- [TlsValidationContextTrustUnionTypeDef](./type_defs.md#tlsvalidationcontexttrustuniontypedef)
- [VirtualGatewayListenerTlsOutputTypeDef](./type_defs.md#virtualgatewaylistenertlsoutputtypedef)
- [VirtualGatewayClientPolicyTlsOutputTypeDef](./type_defs.md#virtualgatewayclientpolicytlsoutputtypedef)
- [VirtualGatewayTlsValidationContextTrustUnionTypeDef](./type_defs.md#virtualgatewaytlsvalidationcontexttrustuniontypedef)
- [CreateVirtualServiceInputRequestTypeDef](./type_defs.md#createvirtualserviceinputrequesttypedef)
- [UpdateVirtualServiceInputRequestTypeDef](./type_defs.md#updatevirtualserviceinputrequesttypedef)
- [VirtualServiceDataTypeDef](./type_defs.md#virtualservicedatatypedef)
- [ServiceDiscoveryUnionTypeDef](./type_defs.md#servicediscoveryuniontypedef)
- [GrpcGatewayRouteOutputTypeDef](./type_defs.md#grpcgatewayrouteoutputtypedef)
- [GrpcGatewayRouteMatchUnionTypeDef](./type_defs.md#grpcgatewayroutematchuniontypedef)
- [GrpcRouteOutputTypeDef](./type_defs.md#grpcrouteoutputtypedef)
- [GrpcRouteMatchUnionTypeDef](./type_defs.md#grpcroutematchuniontypedef)
- [HttpGatewayRouteOutputTypeDef](./type_defs.md#httpgatewayrouteoutputtypedef)
- [HttpGatewayRouteMatchUnionTypeDef](./type_defs.md#httpgatewayroutematchuniontypedef)
- [HttpRouteOutputTypeDef](./type_defs.md#httprouteoutputtypedef)
- [HttpRouteMatchUnionTypeDef](./type_defs.md#httproutematchuniontypedef)
- [TcpRouteUnionTypeDef](./type_defs.md#tcprouteuniontypedef)
- [LoggingOutputTypeDef](./type_defs.md#loggingoutputtypedef)
- [VirtualGatewayLoggingOutputTypeDef](./type_defs.md#virtualgatewayloggingoutputtypedef)
- [FileAccessLogUnionTypeDef](./type_defs.md#fileaccessloguniontypedef)
- [VirtualGatewayFileAccessLogUnionTypeDef](./type_defs.md#virtualgatewayfileaccessloguniontypedef)
- [CreateVirtualRouterOutputTypeDef](./type_defs.md#createvirtualrouteroutputtypedef)
- [DeleteVirtualRouterOutputTypeDef](./type_defs.md#deletevirtualrouteroutputtypedef)
- [DescribeVirtualRouterOutputTypeDef](./type_defs.md#describevirtualrouteroutputtypedef)
- [UpdateVirtualRouterOutputTypeDef](./type_defs.md#updatevirtualrouteroutputtypedef)
- [ListenerOutputTypeDef](./type_defs.md#listeneroutputtypedef)
- [ListenerTlsValidationContextTypeDef](./type_defs.md#listenertlsvalidationcontexttypedef)
- [VirtualGatewayListenerTlsValidationContextTypeDef](./type_defs.md#virtualgatewaylistenertlsvalidationcontexttypedef)
- [ClientPolicyOutputTypeDef](./type_defs.md#clientpolicyoutputtypedef)
- [TlsValidationContextTypeDef](./type_defs.md#tlsvalidationcontexttypedef)
- [VirtualGatewayListenerOutputTypeDef](./type_defs.md#virtualgatewaylisteneroutputtypedef)
- [VirtualGatewayClientPolicyOutputTypeDef](./type_defs.md#virtualgatewayclientpolicyoutputtypedef)
- [VirtualGatewayTlsValidationContextTypeDef](./type_defs.md#virtualgatewaytlsvalidationcontexttypedef)
- [CreateVirtualServiceOutputTypeDef](./type_defs.md#createvirtualserviceoutputtypedef)
- [DeleteVirtualServiceOutputTypeDef](./type_defs.md#deletevirtualserviceoutputtypedef)
- [DescribeVirtualServiceOutputTypeDef](./type_defs.md#describevirtualserviceoutputtypedef)
- [UpdateVirtualServiceOutputTypeDef](./type_defs.md#updatevirtualserviceoutputtypedef)
- [GrpcGatewayRouteTypeDef](./type_defs.md#grpcgatewayroutetypedef)
- [GrpcRouteTypeDef](./type_defs.md#grpcroutetypedef)
- [GatewayRouteSpecOutputTypeDef](./type_defs.md#gatewayroutespecoutputtypedef)
- [HttpGatewayRouteTypeDef](./type_defs.md#httpgatewayroutetypedef)
- [RouteSpecOutputTypeDef](./type_defs.md#routespecoutputtypedef)
- [HttpRouteTypeDef](./type_defs.md#httproutetypedef)
- [AccessLogTypeDef](./type_defs.md#accesslogtypedef)
- [VirtualGatewayAccessLogTypeDef](./type_defs.md#virtualgatewayaccesslogtypedef)
- [ListenerTlsValidationContextUnionTypeDef](./type_defs.md#listenertlsvalidationcontextuniontypedef)
- [VirtualGatewayListenerTlsValidationContextUnionTypeDef](./type_defs.md#virtualgatewaylistenertlsvalidationcontextuniontypedef)
- [BackendDefaultsOutputTypeDef](./type_defs.md#backenddefaultsoutputtypedef)
- [VirtualServiceBackendOutputTypeDef](./type_defs.md#virtualservicebackendoutputtypedef)
- [TlsValidationContextUnionTypeDef](./type_defs.md#tlsvalidationcontextuniontypedef)
- [VirtualGatewayBackendDefaultsOutputTypeDef](./type_defs.md#virtualgatewaybackenddefaultsoutputtypedef)
- [VirtualGatewayTlsValidationContextUnionTypeDef](./type_defs.md#virtualgatewaytlsvalidationcontextuniontypedef)
- [GrpcGatewayRouteUnionTypeDef](./type_defs.md#grpcgatewayrouteuniontypedef)
- [GrpcRouteUnionTypeDef](./type_defs.md#grpcrouteuniontypedef)
- [GatewayRouteDataTypeDef](./type_defs.md#gatewayroutedatatypedef)
- [HttpGatewayRouteUnionTypeDef](./type_defs.md#httpgatewayrouteuniontypedef)
- [RouteDataTypeDef](./type_defs.md#routedatatypedef)
- [HttpRouteUnionTypeDef](./type_defs.md#httprouteuniontypedef)
- [AccessLogUnionTypeDef](./type_defs.md#accessloguniontypedef)
- [VirtualGatewayAccessLogUnionTypeDef](./type_defs.md#virtualgatewayaccessloguniontypedef)
- [ListenerTlsTypeDef](./type_defs.md#listenertlstypedef)
- [VirtualGatewayListenerTlsTypeDef](./type_defs.md#virtualgatewaylistenertlstypedef)
- [BackendOutputTypeDef](./type_defs.md#backendoutputtypedef)
- [ClientPolicyTlsTypeDef](./type_defs.md#clientpolicytlstypedef)
- [VirtualGatewaySpecOutputTypeDef](./type_defs.md#virtualgatewayspecoutputtypedef)
- [VirtualGatewayClientPolicyTlsTypeDef](./type_defs.md#virtualgatewayclientpolicytlstypedef)
- [CreateGatewayRouteOutputTypeDef](./type_defs.md#creategatewayrouteoutputtypedef)
- [DeleteGatewayRouteOutputTypeDef](./type_defs.md#deletegatewayrouteoutputtypedef)
- [DescribeGatewayRouteOutputTypeDef](./type_defs.md#describegatewayrouteoutputtypedef)
- [UpdateGatewayRouteOutputTypeDef](./type_defs.md#updategatewayrouteoutputtypedef)
- [GatewayRouteSpecTypeDef](./type_defs.md#gatewayroutespectypedef)
- [CreateRouteOutputTypeDef](./type_defs.md#createrouteoutputtypedef)
- [DeleteRouteOutputTypeDef](./type_defs.md#deleterouteoutputtypedef)
- [DescribeRouteOutputTypeDef](./type_defs.md#describerouteoutputtypedef)
- [UpdateRouteOutputTypeDef](./type_defs.md#updaterouteoutputtypedef)
- [RouteSpecTypeDef](./type_defs.md#routespectypedef)
- [LoggingTypeDef](./type_defs.md#loggingtypedef)
- [VirtualGatewayLoggingTypeDef](./type_defs.md#virtualgatewayloggingtypedef)
- [ListenerTlsUnionTypeDef](./type_defs.md#listenertlsuniontypedef)
- [VirtualGatewayListenerTlsUnionTypeDef](./type_defs.md#virtualgatewaylistenertlsuniontypedef)
- [VirtualNodeSpecOutputTypeDef](./type_defs.md#virtualnodespecoutputtypedef)
- [ClientPolicyTlsUnionTypeDef](./type_defs.md#clientpolicytlsuniontypedef)
- [VirtualGatewayDataTypeDef](./type_defs.md#virtualgatewaydatatypedef)
- [VirtualGatewayClientPolicyTlsUnionTypeDef](./type_defs.md#virtualgatewayclientpolicytlsuniontypedef)
- [CreateGatewayRouteInputRequestTypeDef](./type_defs.md#creategatewayrouteinputrequesttypedef)
- [UpdateGatewayRouteInputRequestTypeDef](./type_defs.md#updategatewayrouteinputrequesttypedef)
- [CreateRouteInputRequestTypeDef](./type_defs.md#createrouteinputrequesttypedef)
- [UpdateRouteInputRequestTypeDef](./type_defs.md#updaterouteinputrequesttypedef)
- [LoggingUnionTypeDef](./type_defs.md#logginguniontypedef)
- [VirtualGatewayLoggingUnionTypeDef](./type_defs.md#virtualgatewaylogginguniontypedef)
- [ListenerTypeDef](./type_defs.md#listenertypedef)
- [VirtualGatewayListenerTypeDef](./type_defs.md#virtualgatewaylistenertypedef)
- [VirtualNodeDataTypeDef](./type_defs.md#virtualnodedatatypedef)
- [ClientPolicyTypeDef](./type_defs.md#clientpolicytypedef)
- [CreateVirtualGatewayOutputTypeDef](./type_defs.md#createvirtualgatewayoutputtypedef)
- [DeleteVirtualGatewayOutputTypeDef](./type_defs.md#deletevirtualgatewayoutputtypedef)
- [DescribeVirtualGatewayOutputTypeDef](./type_defs.md#describevirtualgatewayoutputtypedef)
- [UpdateVirtualGatewayOutputTypeDef](./type_defs.md#updatevirtualgatewayoutputtypedef)
- [VirtualGatewayClientPolicyTypeDef](./type_defs.md#virtualgatewayclientpolicytypedef)
- [ListenerUnionTypeDef](./type_defs.md#listeneruniontypedef)
- [VirtualGatewayListenerUnionTypeDef](./type_defs.md#virtualgatewaylisteneruniontypedef)
- [CreateVirtualNodeOutputTypeDef](./type_defs.md#createvirtualnodeoutputtypedef)
- [DeleteVirtualNodeOutputTypeDef](./type_defs.md#deletevirtualnodeoutputtypedef)
- [DescribeVirtualNodeOutputTypeDef](./type_defs.md#describevirtualnodeoutputtypedef)
- [UpdateVirtualNodeOutputTypeDef](./type_defs.md#updatevirtualnodeoutputtypedef)
- [ClientPolicyUnionTypeDef](./type_defs.md#clientpolicyuniontypedef)
- [VirtualGatewayClientPolicyUnionTypeDef](./type_defs.md#virtualgatewayclientpolicyuniontypedef)
- [BackendDefaultsTypeDef](./type_defs.md#backenddefaultstypedef)
- [VirtualServiceBackendTypeDef](./type_defs.md#virtualservicebackendtypedef)
- [VirtualGatewayBackendDefaultsTypeDef](./type_defs.md#virtualgatewaybackenddefaultstypedef)
- [BackendDefaultsUnionTypeDef](./type_defs.md#backenddefaultsuniontypedef)
- [VirtualServiceBackendUnionTypeDef](./type_defs.md#virtualservicebackenduniontypedef)
- [VirtualGatewayBackendDefaultsUnionTypeDef](./type_defs.md#virtualgatewaybackenddefaultsuniontypedef)
- [BackendTypeDef](./type_defs.md#backendtypedef)
- [VirtualGatewaySpecTypeDef](./type_defs.md#virtualgatewayspectypedef)
- [BackendUnionTypeDef](./type_defs.md#backenduniontypedef)
- [CreateVirtualGatewayInputRequestTypeDef](./type_defs.md#createvirtualgatewayinputrequesttypedef)
- [UpdateVirtualGatewayInputRequestTypeDef](./type_defs.md#updatevirtualgatewayinputrequesttypedef)
- [VirtualNodeSpecTypeDef](./type_defs.md#virtualnodespectypedef)
- [CreateVirtualNodeInputRequestTypeDef](./type_defs.md#createvirtualnodeinputrequesttypedef)
- [UpdateVirtualNodeInputRequestTypeDef](./type_defs.md#updatevirtualnodeinputrequesttypedef)

