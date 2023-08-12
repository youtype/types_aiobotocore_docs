# AppSync module

> [Index](../README.md) > AppSync


!!! note ""

    Auto-generated documentation for [AppSync](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
    type annotations stubs module [types-aiobotocore-appsync](https://pypi.org/project/types-aiobotocore-appsync/).

## How to install



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
- [ListDataSourcesPaginator](./paginators.md#listdatasourcespaginator)
- [ListFunctionsPaginator](./paginators.md#listfunctionspaginator)
- [ListGraphqlApisPaginator](./paginators.md#listgraphqlapispaginator)
- [ListResolversPaginator](./paginators.md#listresolverspaginator)
- [ListResolversByFunctionPaginator](./paginators.md#listresolversbyfunctionpaginator)
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
- [ConflictDetectionTypeType](./literals.md#conflictdetectiontypetype)
- [ConflictHandlerTypeType](./literals.md#conflicthandlertypetype)
- [DataSourceTypeType](./literals.md#datasourcetypetype)
- [DefaultActionType](./literals.md#defaultactiontype)
- [FieldLogLevelType](./literals.md#fieldlogleveltype)
- [GraphQLApiTypeType](./literals.md#graphqlapitypetype)
- [GraphQLApiVisibilityType](./literals.md#graphqlapivisibilitytype)
- [ListApiKeysPaginatorName](./literals.md#listapikeyspaginatorname)
- [ListDataSourcesPaginatorName](./literals.md#listdatasourcespaginatorname)
- [ListFunctionsPaginatorName](./literals.md#listfunctionspaginatorname)
- [ListGraphqlApisPaginatorName](./literals.md#listgraphqlapispaginatorname)
- [ListResolversByFunctionPaginatorName](./literals.md#listresolversbyfunctionpaginatorname)
- [ListResolversPaginatorName](./literals.md#listresolverspaginatorname)
- [ListTypesPaginatorName](./literals.md#listtypespaginatorname)
- [MergeTypeType](./literals.md#mergetypetype)
- [OutputTypeType](./literals.md#outputtypetype)
- [OwnershipType](./literals.md#ownershiptype)
- [RelationalDatabaseSourceTypeType](./literals.md#relationaldatabasesourcetypetype)
- [ResolverKindType](./literals.md#resolverkindtype)
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
- [AwsIamConfigTypeDef](./type_defs.md#awsiamconfigtypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
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
- [LogConfigTypeDef](./type_defs.md#logconfigtypedef)
- [UserPoolConfigTypeDef](./type_defs.md#userpoolconfigtypedef)
- [PipelineConfigTypeDef](./type_defs.md#pipelineconfigtypedef)
- [CreateTypeRequestRequestTypeDef](./type_defs.md#createtyperequestrequesttypedef)
- [TypeTypeDef](./type_defs.md#typetypedef)
- [DeleteApiCacheRequestRequestTypeDef](./type_defs.md#deleteapicacherequestrequesttypedef)
- [DeleteApiKeyRequestRequestTypeDef](./type_defs.md#deleteapikeyrequestrequesttypedef)
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
- [FlushApiCacheRequestRequestTypeDef](./type_defs.md#flushapicacherequestrequesttypedef)
- [GetApiAssociationRequestRequestTypeDef](./type_defs.md#getapiassociationrequestrequesttypedef)
- [GetApiCacheRequestRequestTypeDef](./type_defs.md#getapicacherequestrequesttypedef)
- [GetDataSourceRequestRequestTypeDef](./type_defs.md#getdatasourcerequestrequesttypedef)
- [GetDomainNameRequestRequestTypeDef](./type_defs.md#getdomainnamerequestrequesttypedef)
- [GetFunctionRequestRequestTypeDef](./type_defs.md#getfunctionrequestrequesttypedef)
- [GetGraphqlApiRequestRequestTypeDef](./type_defs.md#getgraphqlapirequestrequesttypedef)
- [GetIntrospectionSchemaRequestRequestTypeDef](./type_defs.md#getintrospectionschemarequestrequesttypedef)
- [GetResolverRequestRequestTypeDef](./type_defs.md#getresolverrequestrequesttypedef)
- [GetSchemaCreationStatusRequestRequestTypeDef](./type_defs.md#getschemacreationstatusrequestrequesttypedef)
- [GetSourceApiAssociationRequestRequestTypeDef](./type_defs.md#getsourceapiassociationrequestrequesttypedef)
- [GetTypeRequestRequestTypeDef](./type_defs.md#gettyperequestrequesttypedef)
- [LambdaConflictHandlerConfigTypeDef](./type_defs.md#lambdaconflicthandlerconfigtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListApiKeysRequestRequestTypeDef](./type_defs.md#listapikeysrequestrequesttypedef)
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
- [GetIntrospectionSchemaResponseTypeDef](./type_defs.md#getintrospectionschemaresponsetypedef)
- [GetSchemaCreationStatusResponseTypeDef](./type_defs.md#getschemacreationstatusresponsetypedef)
- [ListApiKeysResponseTypeDef](./type_defs.md#listapikeysresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [StartSchemaCreationResponseTypeDef](./type_defs.md#startschemacreationresponsetypedef)
- [StartSchemaMergeResponseTypeDef](./type_defs.md#startschemamergeresponsetypedef)
- [UpdateApiCacheResponseTypeDef](./type_defs.md#updateapicacheresponsetypedef)
- [UpdateApiKeyResponseTypeDef](./type_defs.md#updateapikeyresponsetypedef)
- [AssociateMergedGraphqlApiRequestRequestTypeDef](./type_defs.md#associatemergedgraphqlapirequestrequesttypedef)
- [AssociateSourceGraphqlApiRequestRequestTypeDef](./type_defs.md#associatesourcegraphqlapirequestrequesttypedef)
- [SourceApiAssociationTypeDef](./type_defs.md#sourceapiassociationtypedef)
- [UpdateSourceApiAssociationRequestRequestTypeDef](./type_defs.md#updatesourceapiassociationrequestrequesttypedef)
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
- [DynamodbDataSourceConfigTypeDef](./type_defs.md#dynamodbdatasourceconfigtypedef)
- [EvaluateMappingTemplateResponseTypeDef](./type_defs.md#evaluatemappingtemplateresponsetypedef)
- [SyncConfigTypeDef](./type_defs.md#syncconfigtypedef)
- [ListApiKeysRequestListApiKeysPaginateTypeDef](./type_defs.md#listapikeysrequestlistapikeyspaginatetypedef)
- [ListDataSourcesRequestListDataSourcesPaginateTypeDef](./type_defs.md#listdatasourcesrequestlistdatasourcespaginatetypedef)
- [ListFunctionsRequestListFunctionsPaginateTypeDef](./type_defs.md#listfunctionsrequestlistfunctionspaginatetypedef)
- [ListGraphqlApisRequestListGraphqlApisPaginateTypeDef](./type_defs.md#listgraphqlapisrequestlistgraphqlapispaginatetypedef)
- [ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef](./type_defs.md#listresolversbyfunctionrequestlistresolversbyfunctionpaginatetypedef)
- [ListResolversRequestListResolversPaginateTypeDef](./type_defs.md#listresolversrequestlistresolverspaginatetypedef)
- [ListTypesRequestListTypesPaginateTypeDef](./type_defs.md#listtypesrequestlisttypespaginatetypedef)
- [ListSourceApiAssociationsResponseTypeDef](./type_defs.md#listsourceapiassociationsresponsetypedef)
- [RelationalDatabaseDataSourceConfigTypeDef](./type_defs.md#relationaldatabasedatasourceconfigtypedef)
- [CreateGraphqlApiRequestRequestTypeDef](./type_defs.md#creategraphqlapirequestrequesttypedef)
- [GraphqlApiTypeDef](./type_defs.md#graphqlapitypedef)
- [UpdateGraphqlApiRequestRequestTypeDef](./type_defs.md#updategraphqlapirequestrequesttypedef)
- [AssociateMergedGraphqlApiResponseTypeDef](./type_defs.md#associatemergedgraphqlapiresponsetypedef)
- [AssociateSourceGraphqlApiResponseTypeDef](./type_defs.md#associatesourcegraphqlapiresponsetypedef)
- [GetSourceApiAssociationResponseTypeDef](./type_defs.md#getsourceapiassociationresponsetypedef)
- [UpdateSourceApiAssociationResponseTypeDef](./type_defs.md#updatesourceapiassociationresponsetypedef)
- [HttpDataSourceConfigTypeDef](./type_defs.md#httpdatasourceconfigtypedef)
- [EvaluateCodeErrorDetailTypeDef](./type_defs.md#evaluatecodeerrordetailtypedef)
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
- [CreateDataSourceRequestRequestTypeDef](./type_defs.md#createdatasourcerequestrequesttypedef)
- [DataSourceTypeDef](./type_defs.md#datasourcetypedef)
- [UpdateDataSourceRequestRequestTypeDef](./type_defs.md#updatedatasourcerequestrequesttypedef)
- [EvaluateCodeResponseTypeDef](./type_defs.md#evaluatecoderesponsetypedef)
- [CreateFunctionResponseTypeDef](./type_defs.md#createfunctionresponsetypedef)
- [GetFunctionResponseTypeDef](./type_defs.md#getfunctionresponsetypedef)
- [ListFunctionsResponseTypeDef](./type_defs.md#listfunctionsresponsetypedef)
- [UpdateFunctionResponseTypeDef](./type_defs.md#updatefunctionresponsetypedef)
- [CreateResolverResponseTypeDef](./type_defs.md#createresolverresponsetypedef)
- [GetResolverResponseTypeDef](./type_defs.md#getresolverresponsetypedef)
- [ListResolversByFunctionResponseTypeDef](./type_defs.md#listresolversbyfunctionresponsetypedef)
- [ListResolversResponseTypeDef](./type_defs.md#listresolversresponsetypedef)
- [UpdateResolverResponseTypeDef](./type_defs.md#updateresolverresponsetypedef)
- [CreateDataSourceResponseTypeDef](./type_defs.md#createdatasourceresponsetypedef)
- [GetDataSourceResponseTypeDef](./type_defs.md#getdatasourceresponsetypedef)
- [ListDataSourcesResponseTypeDef](./type_defs.md#listdatasourcesresponsetypedef)
- [UpdateDataSourceResponseTypeDef](./type_defs.md#updatedatasourceresponsetypedef)

