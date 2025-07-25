# ApiGatewayV2 module

> [Index](../README.md) > ApiGatewayV2


!!! note ""

    Auto-generated documentation for [ApiGatewayV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#apigatewayv2)
    type annotations stubs module [types-aiobotocore-apigatewayv2](https://pypi.org/project/types-aiobotocore-apigatewayv2/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.23.2' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `ApiGatewayV2` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `ApiGatewayV2` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[apigatewayv2]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[apigatewayv2]'

# standalone installation
python -m pip install types-aiobotocore-apigatewayv2
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-apigatewayv2
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ApiGatewayV2Client

Type annotations and code completion for  `#!python session.create_client("apigatewayv2")` as [ApiGatewayV2Client](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client)

```python
# ApiGatewayV2Client usage example

from aiobotocore.session import get_session

from types_aiobotocore_apigatewayv2.client import ApiGatewayV2Client


session = get_session()
async with session.create_client("apigatewayv2") as client:
    client: ApiGatewayV2Client
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("apigatewayv2").get_paginator("...")`.

```python
# GetApisPaginator usage example

from types_aiobotocore_apigatewayv2.paginator import GetApisPaginator

def get_get_apis_paginator() -> GetApisPaginator:
    return client.get_paginator("get_apis"))
```

- [GetApisPaginator](./paginators.md#getapispaginator)
- [GetAuthorizersPaginator](./paginators.md#getauthorizerspaginator)
- [GetDeploymentsPaginator](./paginators.md#getdeploymentspaginator)
- [GetDomainNamesPaginator](./paginators.md#getdomainnamespaginator)
- [GetIntegrationResponsesPaginator](./paginators.md#getintegrationresponsespaginator)
- [GetIntegrationsPaginator](./paginators.md#getintegrationspaginator)
- [GetModelsPaginator](./paginators.md#getmodelspaginator)
- [GetRouteResponsesPaginator](./paginators.md#getrouteresponsespaginator)
- [GetRoutesPaginator](./paginators.md#getroutespaginator)
- [GetStagesPaginator](./paginators.md#getstagespaginator)
- [ListRoutingRulesPaginator](./paginators.md#listroutingrulespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AuthorizationTypeType usage example

from types_aiobotocore_apigatewayv2.literals import AuthorizationTypeType

def get_value() -> AuthorizationTypeType:
    return "AWS_IAM"
```

- [AuthorizationTypeType](./literals.md#authorizationtypetype)
- [AuthorizerTypeType](./literals.md#authorizertypetype)
- [ConnectionTypeType](./literals.md#connectiontypetype)
- [ContentHandlingStrategyType](./literals.md#contenthandlingstrategytype)
- [DeploymentStatusType](./literals.md#deploymentstatustype)
- [DomainNameStatusType](./literals.md#domainnamestatustype)
- [EndpointTypeType](./literals.md#endpointtypetype)
- [GetApisPaginatorName](./literals.md#getapispaginatorname)
- [GetAuthorizersPaginatorName](./literals.md#getauthorizerspaginatorname)
- [GetDeploymentsPaginatorName](./literals.md#getdeploymentspaginatorname)
- [GetDomainNamesPaginatorName](./literals.md#getdomainnamespaginatorname)
- [GetIntegrationResponsesPaginatorName](./literals.md#getintegrationresponsespaginatorname)
- [GetIntegrationsPaginatorName](./literals.md#getintegrationspaginatorname)
- [GetModelsPaginatorName](./literals.md#getmodelspaginatorname)
- [GetRouteResponsesPaginatorName](./literals.md#getrouteresponsespaginatorname)
- [GetRoutesPaginatorName](./literals.md#getroutespaginatorname)
- [GetStagesPaginatorName](./literals.md#getstagespaginatorname)
- [IntegrationTypeType](./literals.md#integrationtypetype)
- [IpAddressTypeType](./literals.md#ipaddresstypetype)
- [JSONYAMLType](./literals.md#jsonyamltype)
- [ListRoutingRulesPaginatorName](./literals.md#listroutingrulespaginatorname)
- [LoggingLevelType](./literals.md#loggingleveltype)
- [OAS30Type](./literals.md#oas30type)
- [PassthroughBehaviorType](./literals.md#passthroughbehaviortype)
- [ProtocolTypeType](./literals.md#protocoltypetype)
- [RoutingModeType](./literals.md#routingmodetype)
- [SecurityPolicyType](./literals.md#securitypolicytype)
- [VpcLinkStatusType](./literals.md#vpclinkstatustype)
- [VpcLinkVersionType](./literals.md#vpclinkversiontype)
- [ApiGatewayV2ServiceName](./literals.md#apigatewayv2servicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccessLogSettingsTypeDef](./type_defs.md#accesslogsettingstypedef)
- [ApiMappingTypeDef](./type_defs.md#apimappingtypedef)
- [CorsOutputTypeDef](./type_defs.md#corsoutputtypedef)
- [JWTConfigurationOutputTypeDef](./type_defs.md#jwtconfigurationoutputtypedef)
- [CorsTypeDef](./type_defs.md#corstypedef)
- [CreateApiMappingRequestTypeDef](./type_defs.md#createapimappingrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateDeploymentRequestTypeDef](./type_defs.md#createdeploymentrequesttypedef)
- [MutualTlsAuthenticationInputTypeDef](./type_defs.md#mutualtlsauthenticationinputtypedef)
- [DomainNameConfigurationOutputTypeDef](./type_defs.md#domainnameconfigurationoutputtypedef)
- [MutualTlsAuthenticationTypeDef](./type_defs.md#mutualtlsauthenticationtypedef)
- [TlsConfigInputTypeDef](./type_defs.md#tlsconfiginputtypedef)
- [CreateIntegrationResponseRequestTypeDef](./type_defs.md#createintegrationresponserequesttypedef)
- [TlsConfigTypeDef](./type_defs.md#tlsconfigtypedef)
- [CreateModelRequestTypeDef](./type_defs.md#createmodelrequesttypedef)
- [ParameterConstraintsTypeDef](./type_defs.md#parameterconstraintstypedef)
- [RouteSettingsTypeDef](./type_defs.md#routesettingstypedef)
- [CreateVpcLinkRequestTypeDef](./type_defs.md#createvpclinkrequesttypedef)
- [DeleteAccessLogSettingsRequestTypeDef](./type_defs.md#deleteaccesslogsettingsrequesttypedef)
- [DeleteApiMappingRequestTypeDef](./type_defs.md#deleteapimappingrequesttypedef)
- [DeleteApiRequestTypeDef](./type_defs.md#deleteapirequesttypedef)
- [DeleteAuthorizerRequestTypeDef](./type_defs.md#deleteauthorizerrequesttypedef)
- [DeleteCorsConfigurationRequestTypeDef](./type_defs.md#deletecorsconfigurationrequesttypedef)
- [DeleteDeploymentRequestTypeDef](./type_defs.md#deletedeploymentrequesttypedef)
- [DeleteDomainNameRequestTypeDef](./type_defs.md#deletedomainnamerequesttypedef)
- [DeleteIntegrationRequestTypeDef](./type_defs.md#deleteintegrationrequesttypedef)
- [DeleteIntegrationResponseRequestTypeDef](./type_defs.md#deleteintegrationresponserequesttypedef)
- [DeleteModelRequestTypeDef](./type_defs.md#deletemodelrequesttypedef)
- [DeleteRouteRequestParameterRequestTypeDef](./type_defs.md#deleterouterequestparameterrequesttypedef)
- [DeleteRouteRequestTypeDef](./type_defs.md#deleterouterequesttypedef)
- [DeleteRouteResponseRequestTypeDef](./type_defs.md#deleterouteresponserequesttypedef)
- [DeleteRouteSettingsRequestTypeDef](./type_defs.md#deleteroutesettingsrequesttypedef)
- [DeleteRoutingRuleRequestTypeDef](./type_defs.md#deleteroutingrulerequesttypedef)
- [DeleteStageRequestTypeDef](./type_defs.md#deletestagerequesttypedef)
- [DeleteVpcLinkRequestTypeDef](./type_defs.md#deletevpclinkrequesttypedef)
- [DeploymentTypeDef](./type_defs.md#deploymenttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ExportApiRequestTypeDef](./type_defs.md#exportapirequesttypedef)
- [GetApiMappingRequestTypeDef](./type_defs.md#getapimappingrequesttypedef)
- [GetApiMappingsRequestTypeDef](./type_defs.md#getapimappingsrequesttypedef)
- [GetApiRequestTypeDef](./type_defs.md#getapirequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [GetApisRequestTypeDef](./type_defs.md#getapisrequesttypedef)
- [GetAuthorizerRequestTypeDef](./type_defs.md#getauthorizerrequesttypedef)
- [GetAuthorizersRequestTypeDef](./type_defs.md#getauthorizersrequesttypedef)
- [GetDeploymentRequestTypeDef](./type_defs.md#getdeploymentrequesttypedef)
- [GetDeploymentsRequestTypeDef](./type_defs.md#getdeploymentsrequesttypedef)
- [GetDomainNameRequestTypeDef](./type_defs.md#getdomainnamerequesttypedef)
- [GetDomainNamesRequestTypeDef](./type_defs.md#getdomainnamesrequesttypedef)
- [GetIntegrationRequestTypeDef](./type_defs.md#getintegrationrequesttypedef)
- [GetIntegrationResponseRequestTypeDef](./type_defs.md#getintegrationresponserequesttypedef)
- [GetIntegrationResponsesRequestTypeDef](./type_defs.md#getintegrationresponsesrequesttypedef)
- [IntegrationResponseTypeDef](./type_defs.md#integrationresponsetypedef)
- [GetIntegrationsRequestTypeDef](./type_defs.md#getintegrationsrequesttypedef)
- [GetModelRequestTypeDef](./type_defs.md#getmodelrequesttypedef)
- [GetModelTemplateRequestTypeDef](./type_defs.md#getmodeltemplaterequesttypedef)
- [GetModelsRequestTypeDef](./type_defs.md#getmodelsrequesttypedef)
- [ModelTypeDef](./type_defs.md#modeltypedef)
- [GetRouteRequestTypeDef](./type_defs.md#getrouterequesttypedef)
- [GetRouteResponseRequestTypeDef](./type_defs.md#getrouteresponserequesttypedef)
- [GetRouteResponsesRequestTypeDef](./type_defs.md#getrouteresponsesrequesttypedef)
- [GetRoutesRequestTypeDef](./type_defs.md#getroutesrequesttypedef)
- [GetRoutingRuleRequestTypeDef](./type_defs.md#getroutingrulerequesttypedef)
- [GetStageRequestTypeDef](./type_defs.md#getstagerequesttypedef)
- [GetStagesRequestTypeDef](./type_defs.md#getstagesrequesttypedef)
- [GetTagsRequestTypeDef](./type_defs.md#gettagsrequesttypedef)
- [GetVpcLinkRequestTypeDef](./type_defs.md#getvpclinkrequesttypedef)
- [GetVpcLinksRequestTypeDef](./type_defs.md#getvpclinksrequesttypedef)
- [VpcLinkTypeDef](./type_defs.md#vpclinktypedef)
- [ImportApiRequestTypeDef](./type_defs.md#importapirequesttypedef)
- [JWTConfigurationTypeDef](./type_defs.md#jwtconfigurationtypedef)
- [ListRoutingRulesRequestTypeDef](./type_defs.md#listroutingrulesrequesttypedef)
- [ReimportApiRequestTypeDef](./type_defs.md#reimportapirequesttypedef)
- [ResetAuthorizersCacheRequestTypeDef](./type_defs.md#resetauthorizerscacherequesttypedef)
- [RoutingRuleActionInvokeApiTypeDef](./type_defs.md#routingruleactioninvokeapitypedef)
- [RoutingRuleMatchBasePathsOutputTypeDef](./type_defs.md#routingrulematchbasepathsoutputtypedef)
- [RoutingRuleMatchBasePathsTypeDef](./type_defs.md#routingrulematchbasepathstypedef)
- [RoutingRuleMatchHeaderValueTypeDef](./type_defs.md#routingrulematchheadervaluetypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdateApiMappingRequestTypeDef](./type_defs.md#updateapimappingrequesttypedef)
- [UpdateDeploymentRequestTypeDef](./type_defs.md#updatedeploymentrequesttypedef)
- [UpdateIntegrationResponseRequestTypeDef](./type_defs.md#updateintegrationresponserequesttypedef)
- [UpdateModelRequestTypeDef](./type_defs.md#updatemodelrequesttypedef)
- [UpdateVpcLinkRequestTypeDef](./type_defs.md#updatevpclinkrequesttypedef)
- [ApiTypeDef](./type_defs.md#apitypedef)
- [AuthorizerTypeDef](./type_defs.md#authorizertypedef)
- [CorsUnionTypeDef](./type_defs.md#corsuniontypedef)
- [CreateApiMappingResponseTypeDef](./type_defs.md#createapimappingresponsetypedef)
- [CreateApiResponseTypeDef](./type_defs.md#createapiresponsetypedef)
- [CreateAuthorizerResponseTypeDef](./type_defs.md#createauthorizerresponsetypedef)
- [CreateDeploymentResponseTypeDef](./type_defs.md#createdeploymentresponsetypedef)
- [CreateIntegrationResponseResponseTypeDef](./type_defs.md#createintegrationresponseresponsetypedef)
- [CreateModelResponseTypeDef](./type_defs.md#createmodelresponsetypedef)
- [CreateVpcLinkResponseTypeDef](./type_defs.md#createvpclinkresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [ExportApiResponseTypeDef](./type_defs.md#exportapiresponsetypedef)
- [GetApiMappingResponseTypeDef](./type_defs.md#getapimappingresponsetypedef)
- [GetApiMappingsResponseTypeDef](./type_defs.md#getapimappingsresponsetypedef)
- [GetApiResponseTypeDef](./type_defs.md#getapiresponsetypedef)
- [GetAuthorizerResponseTypeDef](./type_defs.md#getauthorizerresponsetypedef)
- [GetDeploymentResponseTypeDef](./type_defs.md#getdeploymentresponsetypedef)
- [GetIntegrationResponseResponseTypeDef](./type_defs.md#getintegrationresponseresponsetypedef)
- [GetModelResponseTypeDef](./type_defs.md#getmodelresponsetypedef)
- [GetModelTemplateResponseTypeDef](./type_defs.md#getmodeltemplateresponsetypedef)
- [GetTagsResponseTypeDef](./type_defs.md#gettagsresponsetypedef)
- [GetVpcLinkResponseTypeDef](./type_defs.md#getvpclinkresponsetypedef)
- [ImportApiResponseTypeDef](./type_defs.md#importapiresponsetypedef)
- [ReimportApiResponseTypeDef](./type_defs.md#reimportapiresponsetypedef)
- [UpdateApiMappingResponseTypeDef](./type_defs.md#updateapimappingresponsetypedef)
- [UpdateApiResponseTypeDef](./type_defs.md#updateapiresponsetypedef)
- [UpdateAuthorizerResponseTypeDef](./type_defs.md#updateauthorizerresponsetypedef)
- [UpdateDeploymentResponseTypeDef](./type_defs.md#updatedeploymentresponsetypedef)
- [UpdateIntegrationResponseResponseTypeDef](./type_defs.md#updateintegrationresponseresponsetypedef)
- [UpdateModelResponseTypeDef](./type_defs.md#updatemodelresponsetypedef)
- [UpdateVpcLinkResponseTypeDef](./type_defs.md#updatevpclinkresponsetypedef)
- [CreateDomainNameResponseTypeDef](./type_defs.md#createdomainnameresponsetypedef)
- [DomainNameTypeDef](./type_defs.md#domainnametypedef)
- [GetDomainNameResponseTypeDef](./type_defs.md#getdomainnameresponsetypedef)
- [UpdateDomainNameResponseTypeDef](./type_defs.md#updatedomainnameresponsetypedef)
- [CreateIntegrationRequestTypeDef](./type_defs.md#createintegrationrequesttypedef)
- [UpdateIntegrationRequestTypeDef](./type_defs.md#updateintegrationrequesttypedef)
- [CreateIntegrationResultTypeDef](./type_defs.md#createintegrationresulttypedef)
- [GetIntegrationResultTypeDef](./type_defs.md#getintegrationresulttypedef)
- [IntegrationTypeDef](./type_defs.md#integrationtypedef)
- [UpdateIntegrationResultTypeDef](./type_defs.md#updateintegrationresulttypedef)
- [CreateRouteRequestTypeDef](./type_defs.md#createrouterequesttypedef)
- [CreateRouteResponseRequestTypeDef](./type_defs.md#createrouteresponserequesttypedef)
- [CreateRouteResponseResponseTypeDef](./type_defs.md#createrouteresponseresponsetypedef)
- [CreateRouteResultTypeDef](./type_defs.md#createrouteresulttypedef)
- [GetRouteResponseResponseTypeDef](./type_defs.md#getrouteresponseresponsetypedef)
- [GetRouteResultTypeDef](./type_defs.md#getrouteresulttypedef)
- [RouteResponseTypeDef](./type_defs.md#routeresponsetypedef)
- [RouteTypeDef](./type_defs.md#routetypedef)
- [UpdateRouteRequestTypeDef](./type_defs.md#updaterouterequesttypedef)
- [UpdateRouteResponseRequestTypeDef](./type_defs.md#updaterouteresponserequesttypedef)
- [UpdateRouteResponseResponseTypeDef](./type_defs.md#updaterouteresponseresponsetypedef)
- [UpdateRouteResultTypeDef](./type_defs.md#updaterouteresulttypedef)
- [CreateStageRequestTypeDef](./type_defs.md#createstagerequesttypedef)
- [CreateStageResponseTypeDef](./type_defs.md#createstageresponsetypedef)
- [GetStageResponseTypeDef](./type_defs.md#getstageresponsetypedef)
- [StageTypeDef](./type_defs.md#stagetypedef)
- [UpdateStageRequestTypeDef](./type_defs.md#updatestagerequesttypedef)
- [UpdateStageResponseTypeDef](./type_defs.md#updatestageresponsetypedef)
- [GetDeploymentsResponseTypeDef](./type_defs.md#getdeploymentsresponsetypedef)
- [DomainNameConfigurationTypeDef](./type_defs.md#domainnameconfigurationtypedef)
- [GetApisRequestPaginateTypeDef](./type_defs.md#getapisrequestpaginatetypedef)
- [GetAuthorizersRequestPaginateTypeDef](./type_defs.md#getauthorizersrequestpaginatetypedef)
- [GetDeploymentsRequestPaginateTypeDef](./type_defs.md#getdeploymentsrequestpaginatetypedef)
- [GetDomainNamesRequestPaginateTypeDef](./type_defs.md#getdomainnamesrequestpaginatetypedef)
- [GetIntegrationResponsesRequestPaginateTypeDef](./type_defs.md#getintegrationresponsesrequestpaginatetypedef)
- [GetIntegrationsRequestPaginateTypeDef](./type_defs.md#getintegrationsrequestpaginatetypedef)
- [GetModelsRequestPaginateTypeDef](./type_defs.md#getmodelsrequestpaginatetypedef)
- [GetRouteResponsesRequestPaginateTypeDef](./type_defs.md#getrouteresponsesrequestpaginatetypedef)
- [GetRoutesRequestPaginateTypeDef](./type_defs.md#getroutesrequestpaginatetypedef)
- [GetStagesRequestPaginateTypeDef](./type_defs.md#getstagesrequestpaginatetypedef)
- [ListRoutingRulesRequestPaginateTypeDef](./type_defs.md#listroutingrulesrequestpaginatetypedef)
- [GetIntegrationResponsesResponseTypeDef](./type_defs.md#getintegrationresponsesresponsetypedef)
- [GetModelsResponseTypeDef](./type_defs.md#getmodelsresponsetypedef)
- [GetVpcLinksResponseTypeDef](./type_defs.md#getvpclinksresponsetypedef)
- [JWTConfigurationUnionTypeDef](./type_defs.md#jwtconfigurationuniontypedef)
- [RoutingRuleActionTypeDef](./type_defs.md#routingruleactiontypedef)
- [RoutingRuleMatchBasePathsUnionTypeDef](./type_defs.md#routingrulematchbasepathsuniontypedef)
- [RoutingRuleMatchHeadersOutputTypeDef](./type_defs.md#routingrulematchheadersoutputtypedef)
- [RoutingRuleMatchHeadersTypeDef](./type_defs.md#routingrulematchheaderstypedef)
- [GetApisResponseTypeDef](./type_defs.md#getapisresponsetypedef)
- [GetAuthorizersResponseTypeDef](./type_defs.md#getauthorizersresponsetypedef)
- [CreateApiRequestTypeDef](./type_defs.md#createapirequesttypedef)
- [UpdateApiRequestTypeDef](./type_defs.md#updateapirequesttypedef)
- [GetDomainNamesResponseTypeDef](./type_defs.md#getdomainnamesresponsetypedef)
- [GetIntegrationsResponseTypeDef](./type_defs.md#getintegrationsresponsetypedef)
- [GetRouteResponsesResponseTypeDef](./type_defs.md#getrouteresponsesresponsetypedef)
- [GetRoutesResponseTypeDef](./type_defs.md#getroutesresponsetypedef)
- [GetStagesResponseTypeDef](./type_defs.md#getstagesresponsetypedef)
- [DomainNameConfigurationUnionTypeDef](./type_defs.md#domainnameconfigurationuniontypedef)
- [CreateAuthorizerRequestTypeDef](./type_defs.md#createauthorizerrequesttypedef)
- [UpdateAuthorizerRequestTypeDef](./type_defs.md#updateauthorizerrequesttypedef)
- [RoutingRuleConditionOutputTypeDef](./type_defs.md#routingruleconditionoutputtypedef)
- [RoutingRuleMatchHeadersUnionTypeDef](./type_defs.md#routingrulematchheadersuniontypedef)
- [CreateDomainNameRequestTypeDef](./type_defs.md#createdomainnamerequesttypedef)
- [UpdateDomainNameRequestTypeDef](./type_defs.md#updatedomainnamerequesttypedef)
- [CreateRoutingRuleResponseTypeDef](./type_defs.md#createroutingruleresponsetypedef)
- [GetRoutingRuleResponseTypeDef](./type_defs.md#getroutingruleresponsetypedef)
- [PutRoutingRuleResponseTypeDef](./type_defs.md#putroutingruleresponsetypedef)
- [RoutingRuleTypeDef](./type_defs.md#routingruletypedef)
- [RoutingRuleConditionTypeDef](./type_defs.md#routingruleconditiontypedef)
- [ListRoutingRulesResponseTypeDef](./type_defs.md#listroutingrulesresponsetypedef)
- [RoutingRuleConditionUnionTypeDef](./type_defs.md#routingruleconditionuniontypedef)
- [CreateRoutingRuleRequestTypeDef](./type_defs.md#createroutingrulerequesttypedef)
- [PutRoutingRuleRequestTypeDef](./type_defs.md#putroutingrulerequesttypedef)

