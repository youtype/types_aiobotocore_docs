# AppSync module

> [Index](../README.md) > AppSync


!!! note ""

    Auto-generated documentation for [AppSync](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#appsync)
    type annotations stubs module [types-aiobotocore-appsync](https://pypi.org/project/types-aiobotocore-appsync/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `AppSync` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `AppSync` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[appsync]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[appsync]'

# standalone installation
python -m pip install types-aiobotocore-appsync
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-appsync
```

## Usage

Code samples can be found in [Examples](./usage.md).

## AppSyncClient

Type annotations and code completion for  `#!python session.create_client("appsync")` as [AppSyncClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client)

```python
# AppSyncClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_appsync.client import AppSyncClient


session = get_session()
async with session.create_client("appsync") as client:
    client: AppSyncClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("appsync").get_paginator("...")`.

```python
# ListApiKeysPaginator usage example

from types_aiobotocore_appsync.paginator import ListApiKeysPaginator

def get_list_api_keys_paginator() -> ListApiKeysPaginator:
    return client.get_paginator("list_api_keys"))
```

- [ListApiKeysPaginator](./paginators.md#listapikeyspaginator)
- [ListApisPaginator](./paginators.md#listapispaginator)
- [ListChannelNamespacesPaginator](./paginators.md#listchannelnamespacespaginator)
- [ListDataSourcesPaginator](./paginators.md#listdatasourcespaginator)
- [ListDomainNamesPaginator](./paginators.md#listdomainnamespaginator)
- [ListFunctionsPaginator](./paginators.md#listfunctionspaginator)
- [ListGraphqlApisPaginator](./paginators.md#listgraphqlapispaginator)
- [ListResolversByFunctionPaginator](./paginators.md#listresolversbyfunctionpaginator)
- [ListResolversPaginator](./paginators.md#listresolverspaginator)
- [ListSourceApiAssociationsPaginator](./paginators.md#listsourceapiassociationspaginator)
- [ListTypesByAssociationPaginator](./paginators.md#listtypesbyassociationpaginator)
- [ListTypesPaginator](./paginators.md#listtypespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ApiCacheStatusType usage example

from types_aiobotocore_appsync.literals import ApiCacheStatusType

def get_value() -> ApiCacheStatusType:
    return "AVAILABLE"
```

- [ApiCacheStatusType](./literals.md#apicachestatustype)
- [ApiCacheTypeType](./literals.md#apicachetypetype)
- [ApiCachingBehaviorType](./literals.md#apicachingbehaviortype)
- [AssociationStatusType](./literals.md#associationstatustype)
- [AuthenticationTypeType](./literals.md#authenticationtypetype)
- [AuthorizationTypeType](./literals.md#authorizationtypetype)
- [CacheHealthMetricsConfigType](./literals.md#cachehealthmetricsconfigtype)
- [ConflictDetectionTypeType](./literals.md#conflictdetectiontypetype)
- [ConflictHandlerTypeType](./literals.md#conflicthandlertypetype)
- [DataSourceIntrospectionStatusType](./literals.md#datasourceintrospectionstatustype)
- [DataSourceLevelMetricsBehaviorType](./literals.md#datasourcelevelmetricsbehaviortype)
- [DataSourceLevelMetricsConfigType](./literals.md#datasourcelevelmetricsconfigtype)
- [DataSourceTypeType](./literals.md#datasourcetypetype)
- [DefaultActionType](./literals.md#defaultactiontype)
- [EventLogLevelType](./literals.md#eventlogleveltype)
- [FieldLogLevelType](./literals.md#fieldlogleveltype)
- [GraphQLApiIntrospectionConfigType](./literals.md#graphqlapiintrospectionconfigtype)
- [GraphQLApiTypeType](./literals.md#graphqlapitypetype)
- [GraphQLApiVisibilityType](./literals.md#graphqlapivisibilitytype)
- [ListApiKeysPaginatorName](./literals.md#listapikeyspaginatorname)
- [ListApisPaginatorName](./literals.md#listapispaginatorname)
- [ListChannelNamespacesPaginatorName](./literals.md#listchannelnamespacespaginatorname)
- [ListDataSourcesPaginatorName](./literals.md#listdatasourcespaginatorname)
- [ListDomainNamesPaginatorName](./literals.md#listdomainnamespaginatorname)
- [ListFunctionsPaginatorName](./literals.md#listfunctionspaginatorname)
- [ListGraphqlApisPaginatorName](./literals.md#listgraphqlapispaginatorname)
- [ListResolversByFunctionPaginatorName](./literals.md#listresolversbyfunctionpaginatorname)
- [ListResolversPaginatorName](./literals.md#listresolverspaginatorname)
- [ListSourceApiAssociationsPaginatorName](./literals.md#listsourceapiassociationspaginatorname)
- [ListTypesByAssociationPaginatorName](./literals.md#listtypesbyassociationpaginatorname)
- [ListTypesPaginatorName](./literals.md#listtypespaginatorname)
- [MergeTypeType](./literals.md#mergetypetype)
- [OperationLevelMetricsConfigType](./literals.md#operationlevelmetricsconfigtype)
- [OutputTypeType](./literals.md#outputtypetype)
- [OwnershipType](./literals.md#ownershiptype)
- [RelationalDatabaseSourceTypeType](./literals.md#relationaldatabasesourcetypetype)
- [ResolverKindType](./literals.md#resolverkindtype)
- [ResolverLevelMetricsBehaviorType](./literals.md#resolverlevelmetricsbehaviortype)
- [ResolverLevelMetricsConfigType](./literals.md#resolverlevelmetricsconfigtype)
- [RuntimeNameType](./literals.md#runtimenametype)
- [SchemaStatusType](./literals.md#schemastatustype)
- [SourceApiAssociationStatusType](./literals.md#sourceapiassociationstatustype)
- [TypeDefinitionFormatType](./literals.md#typedefinitionformattype)
- [AppSyncServiceName](./literals.md#appsyncservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [CognitoUserPoolConfigTypeDef](./type_defs.md#cognitouserpoolconfigtypedef)
- [LambdaAuthorizerConfigTypeDef](./type_defs.md#lambdaauthorizerconfigtypedef)
- [OpenIDConnectConfigTypeDef](./type_defs.md#openidconnectconfigtypedef)
- [ApiAssociationTypeDef](./type_defs.md#apiassociationtypedef)
- [ApiCacheTypeDef](./type_defs.md#apicachetypedef)
- [ApiKeyTypeDef](./type_defs.md#apikeytypedef)
- [AppSyncRuntimeTypeDef](./type_defs.md#appsyncruntimetypedef)
- [AssociateApiRequestRequestTypeDef](./type_defs.md#associateapirequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [SourceApiAssociationConfigTypeDef](./type_defs.md#sourceapiassociationconfigtypedef)
- [AuthModeTypeDef](./type_defs.md#authmodetypedef)
- [CognitoConfigTypeDef](./type_defs.md#cognitoconfigtypedef)
- [AwsIamConfigTypeDef](./type_defs.md#awsiamconfigtypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [CachingConfigOutputTypeDef](./type_defs.md#cachingconfigoutputtypedef)
- [CachingConfigTypeDef](./type_defs.md#cachingconfigtypedef)
- [CodeErrorLocationTypeDef](./type_defs.md#codeerrorlocationtypedef)
- [CreateApiCacheRequestRequestTypeDef](./type_defs.md#createapicacherequestrequesttypedef)
- [CreateApiKeyRequestRequestTypeDef](./type_defs.md#createapikeyrequestrequesttypedef)
- [ElasticsearchDataSourceConfigTypeDef](./type_defs.md#elasticsearchdatasourceconfigtypedef)
- [EventBridgeDataSourceConfigTypeDef](./type_defs.md#eventbridgedatasourceconfigtypedef)
- [LambdaDataSourceConfigTypeDef](./type_defs.md#lambdadatasourceconfigtypedef)
- [OpenSearchServiceDataSourceConfigTypeDef](./type_defs.md#opensearchservicedatasourceconfigtypedef)
- [CreateDomainNameRequestRequestTypeDef](./type_defs.md#createdomainnamerequestrequesttypedef)
- [DomainNameConfigTypeDef](./type_defs.md#domainnameconfigtypedef)
- [EnhancedMetricsConfigTypeDef](./type_defs.md#enhancedmetricsconfigtypedef)
- [LogConfigTypeDef](./type_defs.md#logconfigtypedef)
- [UserPoolConfigTypeDef](./type_defs.md#userpoolconfigtypedef)
- [PipelineConfigTypeDef](./type_defs.md#pipelineconfigtypedef)
- [CreateTypeRequestRequestTypeDef](./type_defs.md#createtyperequestrequesttypedef)
- [TypeTypeDef](./type_defs.md#typetypedef)
- [DataSourceIntrospectionModelFieldTypeTypeDef](./type_defs.md#datasourceintrospectionmodelfieldtypetypedef)
- [DataSourceIntrospectionModelIndexTypeDef](./type_defs.md#datasourceintrospectionmodelindextypedef)
- [DeleteApiCacheRequestRequestTypeDef](./type_defs.md#deleteapicacherequestrequesttypedef)
- [DeleteApiKeyRequestRequestTypeDef](./type_defs.md#deleteapikeyrequestrequesttypedef)
- [DeleteApiRequestRequestTypeDef](./type_defs.md#deleteapirequestrequesttypedef)
- [DeleteChannelNamespaceRequestRequestTypeDef](./type_defs.md#deletechannelnamespacerequestrequesttypedef)
- [DeleteDataSourceRequestRequestTypeDef](./type_defs.md#deletedatasourcerequestrequesttypedef)
- [DeleteDomainNameRequestRequestTypeDef](./type_defs.md#deletedomainnamerequestrequesttypedef)
- [DeleteFunctionRequestRequestTypeDef](./type_defs.md#deletefunctionrequestrequesttypedef)
- [DeleteGraphqlApiRequestRequestTypeDef](./type_defs.md#deletegraphqlapirequestrequesttypedef)
- [DeleteResolverRequestRequestTypeDef](./type_defs.md#deleteresolverrequestrequesttypedef)
- [DeleteTypeRequestRequestTypeDef](./type_defs.md#deletetyperequestrequesttypedef)
- [DeltaSyncConfigTypeDef](./type_defs.md#deltasyncconfigtypedef)
- [DisassociateApiRequestRequestTypeDef](./type_defs.md#disassociateapirequestrequesttypedef)
- [DisassociateMergedGraphqlApiRequestRequestTypeDef](./type_defs.md#disassociatemergedgraphqlapirequestrequesttypedef)
- [DisassociateSourceGraphqlApiRequestRequestTypeDef](./type_defs.md#disassociatesourcegraphqlapirequestrequesttypedef)
- [ErrorDetailTypeDef](./type_defs.md#errordetailtypedef)
- [EvaluateMappingTemplateRequestRequestTypeDef](./type_defs.md#evaluatemappingtemplaterequestrequesttypedef)
- [EventLogConfigTypeDef](./type_defs.md#eventlogconfigtypedef)
- [FlushApiCacheRequestRequestTypeDef](./type_defs.md#flushapicacherequestrequesttypedef)
- [GetApiAssociationRequestRequestTypeDef](./type_defs.md#getapiassociationrequestrequesttypedef)
- [GetApiCacheRequestRequestTypeDef](./type_defs.md#getapicacherequestrequesttypedef)
- [GetApiRequestRequestTypeDef](./type_defs.md#getapirequestrequesttypedef)
- [GetChannelNamespaceRequestRequestTypeDef](./type_defs.md#getchannelnamespacerequestrequesttypedef)
- [GetDataSourceIntrospectionRequestRequestTypeDef](./type_defs.md#getdatasourceintrospectionrequestrequesttypedef)
- [GetDataSourceRequestRequestTypeDef](./type_defs.md#getdatasourcerequestrequesttypedef)
- [GetDomainNameRequestRequestTypeDef](./type_defs.md#getdomainnamerequestrequesttypedef)
- [GetFunctionRequestRequestTypeDef](./type_defs.md#getfunctionrequestrequesttypedef)
- [GetGraphqlApiEnvironmentVariablesRequestRequestTypeDef](./type_defs.md#getgraphqlapienvironmentvariablesrequestrequesttypedef)
- [GetGraphqlApiRequestRequestTypeDef](./type_defs.md#getgraphqlapirequestrequesttypedef)
- [GetIntrospectionSchemaRequestRequestTypeDef](./type_defs.md#getintrospectionschemarequestrequesttypedef)
- [GetResolverRequestRequestTypeDef](./type_defs.md#getresolverrequestrequesttypedef)
- [GetSchemaCreationStatusRequestRequestTypeDef](./type_defs.md#getschemacreationstatusrequestrequesttypedef)
- [GetSourceApiAssociationRequestRequestTypeDef](./type_defs.md#getsourceapiassociationrequestrequesttypedef)
- [GetTypeRequestRequestTypeDef](./type_defs.md#gettyperequestrequesttypedef)
- [LambdaConflictHandlerConfigTypeDef](./type_defs.md#lambdaconflicthandlerconfigtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListApiKeysRequestRequestTypeDef](./type_defs.md#listapikeysrequestrequesttypedef)
- [ListApisRequestRequestTypeDef](./type_defs.md#listapisrequestrequesttypedef)
- [ListChannelNamespacesRequestRequestTypeDef](./type_defs.md#listchannelnamespacesrequestrequesttypedef)
- [ListDataSourcesRequestRequestTypeDef](./type_defs.md#listdatasourcesrequestrequesttypedef)
- [ListDomainNamesRequestRequestTypeDef](./type_defs.md#listdomainnamesrequestrequesttypedef)
- [ListFunctionsRequestRequestTypeDef](./type_defs.md#listfunctionsrequestrequesttypedef)
- [ListGraphqlApisRequestRequestTypeDef](./type_defs.md#listgraphqlapisrequestrequesttypedef)
- [ListResolversByFunctionRequestRequestTypeDef](./type_defs.md#listresolversbyfunctionrequestrequesttypedef)
- [ListResolversRequestRequestTypeDef](./type_defs.md#listresolversrequestrequesttypedef)
- [ListSourceApiAssociationsRequestRequestTypeDef](./type_defs.md#listsourceapiassociationsrequestrequesttypedef)
- [SourceApiAssociationSummaryTypeDef](./type_defs.md#sourceapiassociationsummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListTypesByAssociationRequestRequestTypeDef](./type_defs.md#listtypesbyassociationrequestrequesttypedef)
- [ListTypesRequestRequestTypeDef](./type_defs.md#listtypesrequestrequesttypedef)
- [PipelineConfigOutputTypeDef](./type_defs.md#pipelineconfigoutputtypedef)
- [PutGraphqlApiEnvironmentVariablesRequestRequestTypeDef](./type_defs.md#putgraphqlapienvironmentvariablesrequestrequesttypedef)
- [RdsDataApiConfigTypeDef](./type_defs.md#rdsdataapiconfigtypedef)
- [RdsHttpEndpointConfigTypeDef](./type_defs.md#rdshttpendpointconfigtypedef)
- [StartSchemaMergeRequestRequestTypeDef](./type_defs.md#startschemamergerequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateApiCacheRequestRequestTypeDef](./type_defs.md#updateapicacherequestrequesttypedef)
- [UpdateApiKeyRequestRequestTypeDef](./type_defs.md#updateapikeyrequestrequesttypedef)
- [UpdateDomainNameRequestRequestTypeDef](./type_defs.md#updatedomainnamerequestrequesttypedef)
- [UpdateTypeRequestRequestTypeDef](./type_defs.md#updatetyperequestrequesttypedef)
- [AdditionalAuthenticationProviderTypeDef](./type_defs.md#additionalauthenticationprovidertypedef)
- [EvaluateCodeRequestRequestTypeDef](./type_defs.md#evaluatecoderequestrequesttypedef)
- [AssociateApiResponseTypeDef](./type_defs.md#associateapiresponsetypedef)
- [CreateApiCacheResponseTypeDef](./type_defs.md#createapicacheresponsetypedef)
- [CreateApiKeyResponseTypeDef](./type_defs.md#createapikeyresponsetypedef)
- [DisassociateMergedGraphqlApiResponseTypeDef](./type_defs.md#disassociatemergedgraphqlapiresponsetypedef)
- [DisassociateSourceGraphqlApiResponseTypeDef](./type_defs.md#disassociatesourcegraphqlapiresponsetypedef)
- [GetApiAssociationResponseTypeDef](./type_defs.md#getapiassociationresponsetypedef)
- [GetApiCacheResponseTypeDef](./type_defs.md#getapicacheresponsetypedef)
- [GetGraphqlApiEnvironmentVariablesResponseTypeDef](./type_defs.md#getgraphqlapienvironmentvariablesresponsetypedef)
- [GetIntrospectionSchemaResponseTypeDef](./type_defs.md#getintrospectionschemaresponsetypedef)
- [GetSchemaCreationStatusResponseTypeDef](./type_defs.md#getschemacreationstatusresponsetypedef)
- [ListApiKeysResponseTypeDef](./type_defs.md#listapikeysresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [PutGraphqlApiEnvironmentVariablesResponseTypeDef](./type_defs.md#putgraphqlapienvironmentvariablesresponsetypedef)
- [StartDataSourceIntrospectionResponseTypeDef](./type_defs.md#startdatasourceintrospectionresponsetypedef)
- [StartSchemaCreationResponseTypeDef](./type_defs.md#startschemacreationresponsetypedef)
- [StartSchemaMergeResponseTypeDef](./type_defs.md#startschemamergeresponsetypedef)
- [UpdateApiCacheResponseTypeDef](./type_defs.md#updateapicacheresponsetypedef)
- [UpdateApiKeyResponseTypeDef](./type_defs.md#updateapikeyresponsetypedef)
- [AssociateMergedGraphqlApiRequestRequestTypeDef](./type_defs.md#associatemergedgraphqlapirequestrequesttypedef)
- [AssociateSourceGraphqlApiRequestRequestTypeDef](./type_defs.md#associatesourcegraphqlapirequestrequesttypedef)
- [SourceApiAssociationTypeDef](./type_defs.md#sourceapiassociationtypedef)
- [UpdateSourceApiAssociationRequestRequestTypeDef](./type_defs.md#updatesourceapiassociationrequestrequesttypedef)
- [ChannelNamespaceTypeDef](./type_defs.md#channelnamespacetypedef)
- [CreateChannelNamespaceRequestRequestTypeDef](./type_defs.md#createchannelnamespacerequestrequesttypedef)
- [UpdateChannelNamespaceRequestRequestTypeDef](./type_defs.md#updatechannelnamespacerequestrequesttypedef)
- [AuthProviderTypeDef](./type_defs.md#authprovidertypedef)
- [AuthorizationConfigTypeDef](./type_defs.md#authorizationconfigtypedef)
- [StartSchemaCreationRequestRequestTypeDef](./type_defs.md#startschemacreationrequestrequesttypedef)
- [CodeErrorTypeDef](./type_defs.md#codeerrortypedef)
- [CreateDomainNameResponseTypeDef](./type_defs.md#createdomainnameresponsetypedef)
- [GetDomainNameResponseTypeDef](./type_defs.md#getdomainnameresponsetypedef)
- [ListDomainNamesResponseTypeDef](./type_defs.md#listdomainnamesresponsetypedef)
- [UpdateDomainNameResponseTypeDef](./type_defs.md#updatedomainnameresponsetypedef)
- [CreateTypeResponseTypeDef](./type_defs.md#createtyperesponsetypedef)
- [GetTypeResponseTypeDef](./type_defs.md#gettyperesponsetypedef)
- [ListTypesByAssociationResponseTypeDef](./type_defs.md#listtypesbyassociationresponsetypedef)
- [ListTypesResponseTypeDef](./type_defs.md#listtypesresponsetypedef)
- [UpdateTypeResponseTypeDef](./type_defs.md#updatetyperesponsetypedef)
- [DataSourceIntrospectionModelFieldTypeDef](./type_defs.md#datasourceintrospectionmodelfieldtypedef)
- [DynamodbDataSourceConfigTypeDef](./type_defs.md#dynamodbdatasourceconfigtypedef)
- [EvaluateMappingTemplateResponseTypeDef](./type_defs.md#evaluatemappingtemplateresponsetypedef)
- [SyncConfigTypeDef](./type_defs.md#syncconfigtypedef)
- [ListApiKeysRequestPaginateTypeDef](./type_defs.md#listapikeysrequestpaginatetypedef)
- [ListApisRequestPaginateTypeDef](./type_defs.md#listapisrequestpaginatetypedef)
- [ListChannelNamespacesRequestPaginateTypeDef](./type_defs.md#listchannelnamespacesrequestpaginatetypedef)
- [ListDataSourcesRequestPaginateTypeDef](./type_defs.md#listdatasourcesrequestpaginatetypedef)
- [ListDomainNamesRequestPaginateTypeDef](./type_defs.md#listdomainnamesrequestpaginatetypedef)
- [ListFunctionsRequestPaginateTypeDef](./type_defs.md#listfunctionsrequestpaginatetypedef)
- [ListGraphqlApisRequestPaginateTypeDef](./type_defs.md#listgraphqlapisrequestpaginatetypedef)
- [ListResolversByFunctionRequestPaginateTypeDef](./type_defs.md#listresolversbyfunctionrequestpaginatetypedef)
- [ListResolversRequestPaginateTypeDef](./type_defs.md#listresolversrequestpaginatetypedef)
- [ListSourceApiAssociationsRequestPaginateTypeDef](./type_defs.md#listsourceapiassociationsrequestpaginatetypedef)
- [ListTypesByAssociationRequestPaginateTypeDef](./type_defs.md#listtypesbyassociationrequestpaginatetypedef)
- [ListTypesRequestPaginateTypeDef](./type_defs.md#listtypesrequestpaginatetypedef)
- [ListSourceApiAssociationsResponseTypeDef](./type_defs.md#listsourceapiassociationsresponsetypedef)
- [StartDataSourceIntrospectionRequestRequestTypeDef](./type_defs.md#startdatasourceintrospectionrequestrequesttypedef)
- [RelationalDatabaseDataSourceConfigTypeDef](./type_defs.md#relationaldatabasedatasourceconfigtypedef)
- [CreateGraphqlApiRequestRequestTypeDef](./type_defs.md#creategraphqlapirequestrequesttypedef)
- [GraphqlApiTypeDef](./type_defs.md#graphqlapitypedef)
- [UpdateGraphqlApiRequestRequestTypeDef](./type_defs.md#updategraphqlapirequestrequesttypedef)
- [AssociateMergedGraphqlApiResponseTypeDef](./type_defs.md#associatemergedgraphqlapiresponsetypedef)
- [AssociateSourceGraphqlApiResponseTypeDef](./type_defs.md#associatesourcegraphqlapiresponsetypedef)
- [GetSourceApiAssociationResponseTypeDef](./type_defs.md#getsourceapiassociationresponsetypedef)
- [UpdateSourceApiAssociationResponseTypeDef](./type_defs.md#updatesourceapiassociationresponsetypedef)
- [CreateChannelNamespaceResponseTypeDef](./type_defs.md#createchannelnamespaceresponsetypedef)
- [GetChannelNamespaceResponseTypeDef](./type_defs.md#getchannelnamespaceresponsetypedef)
- [ListChannelNamespacesResponseTypeDef](./type_defs.md#listchannelnamespacesresponsetypedef)
- [UpdateChannelNamespaceResponseTypeDef](./type_defs.md#updatechannelnamespaceresponsetypedef)
- [EventConfigOutputTypeDef](./type_defs.md#eventconfigoutputtypedef)
- [EventConfigTypeDef](./type_defs.md#eventconfigtypedef)
- [HttpDataSourceConfigTypeDef](./type_defs.md#httpdatasourceconfigtypedef)
- [EvaluateCodeErrorDetailTypeDef](./type_defs.md#evaluatecodeerrordetailtypedef)
- [DataSourceIntrospectionModelTypeDef](./type_defs.md#datasourceintrospectionmodeltypedef)
- [CreateFunctionRequestRequestTypeDef](./type_defs.md#createfunctionrequestrequesttypedef)
- [CreateResolverRequestRequestTypeDef](./type_defs.md#createresolverrequestrequesttypedef)
- [FunctionConfigurationTypeDef](./type_defs.md#functionconfigurationtypedef)
- [ResolverTypeDef](./type_defs.md#resolvertypedef)
- [UpdateFunctionRequestRequestTypeDef](./type_defs.md#updatefunctionrequestrequesttypedef)
- [UpdateResolverRequestRequestTypeDef](./type_defs.md#updateresolverrequestrequesttypedef)
- [CreateGraphqlApiResponseTypeDef](./type_defs.md#creategraphqlapiresponsetypedef)
- [GetGraphqlApiResponseTypeDef](./type_defs.md#getgraphqlapiresponsetypedef)
- [ListGraphqlApisResponseTypeDef](./type_defs.md#listgraphqlapisresponsetypedef)
- [UpdateGraphqlApiResponseTypeDef](./type_defs.md#updategraphqlapiresponsetypedef)
- [ApiTypeDef](./type_defs.md#apitypedef)
- [CreateApiRequestRequestTypeDef](./type_defs.md#createapirequestrequesttypedef)
- [UpdateApiRequestRequestTypeDef](./type_defs.md#updateapirequestrequesttypedef)
- [CreateDataSourceRequestRequestTypeDef](./type_defs.md#createdatasourcerequestrequesttypedef)
- [DataSourceTypeDef](./type_defs.md#datasourcetypedef)
- [UpdateDataSourceRequestRequestTypeDef](./type_defs.md#updatedatasourcerequestrequesttypedef)
- [EvaluateCodeResponseTypeDef](./type_defs.md#evaluatecoderesponsetypedef)
- [DataSourceIntrospectionResultTypeDef](./type_defs.md#datasourceintrospectionresulttypedef)
- [CreateFunctionResponseTypeDef](./type_defs.md#createfunctionresponsetypedef)
- [GetFunctionResponseTypeDef](./type_defs.md#getfunctionresponsetypedef)
- [ListFunctionsResponseTypeDef](./type_defs.md#listfunctionsresponsetypedef)
- [UpdateFunctionResponseTypeDef](./type_defs.md#updatefunctionresponsetypedef)
- [CreateResolverResponseTypeDef](./type_defs.md#createresolverresponsetypedef)
- [GetResolverResponseTypeDef](./type_defs.md#getresolverresponsetypedef)
- [ListResolversByFunctionResponseTypeDef](./type_defs.md#listresolversbyfunctionresponsetypedef)
- [ListResolversResponseTypeDef](./type_defs.md#listresolversresponsetypedef)
- [UpdateResolverResponseTypeDef](./type_defs.md#updateresolverresponsetypedef)
- [CreateApiResponseTypeDef](./type_defs.md#createapiresponsetypedef)
- [GetApiResponseTypeDef](./type_defs.md#getapiresponsetypedef)
- [ListApisResponseTypeDef](./type_defs.md#listapisresponsetypedef)
- [UpdateApiResponseTypeDef](./type_defs.md#updateapiresponsetypedef)
- [CreateDataSourceResponseTypeDef](./type_defs.md#createdatasourceresponsetypedef)
- [GetDataSourceResponseTypeDef](./type_defs.md#getdatasourceresponsetypedef)
- [ListDataSourcesResponseTypeDef](./type_defs.md#listdatasourcesresponsetypedef)
- [UpdateDataSourceResponseTypeDef](./type_defs.md#updatedatasourceresponsetypedef)
- [GetDataSourceIntrospectionResponseTypeDef](./type_defs.md#getdatasourceintrospectionresponsetypedef)

