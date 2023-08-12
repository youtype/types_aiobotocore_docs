# AppSyncClient

> [Index](../README.md) > [AppSync](./README.md) > AppSyncClient

!!! note ""

    Auto-generated documentation for [AppSync](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
    type annotations stubs module [types-aiobotocore-appsync](https://pypi.org/project/types-aiobotocore-appsync/).

## AppSyncClient

Type annotations and code completion for `#!python session.create_client("appsync")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client)

```python
AppSyncClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_appsync.client import AppSyncClient

session = get_session()
async with session.create_client("appsync") as client:
    client: AppSyncClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("appsync").exceptions` structure.

```python
AppSyncClient.exceptions usage example

async with session.create_client("appsync") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ApiKeyLimitExceededException,
        client.ApiKeyValidityOutOfBoundsException,
        client.ApiLimitExceededException,
        client.BadRequestException,
        client.ClientError,
        client.ConcurrentModificationException,
        client.GraphQLSchemaException,
        client.InternalFailureException,
        client.LimitExceededException,
        client.NotFoundException,
        client.UnauthorizedException,
    ) as e:
        print(e)
```

```python
AppSyncClient usage type checking example

from types_aiobotocore_appsync.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### associate\_api

Maps an endpoint to your custom domain.

Type annotations and code completion for `#!python session.create_client("appsync").associate_api` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.associate_api)

```python
# associate_api method definition

await def associate_api(
    self,
    *,
    domainName: str,
    apiId: str,
) -> AssociateApiResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssociateApiResponseTypeDef](./type_defs.md#associateapiresponsetypedef) 


```python
# associate_api method usage example with argument unpacking

kwargs: AssociateApiRequestRequestTypeDef = {  # (1)
    "domainName": ...,
    "apiId": ...,
}

parent.associate_api(**kwargs)
```

1. See [:material-code-braces: AssociateApiRequestRequestTypeDef](./type_defs.md#associateapirequestrequesttypedef) 

### associate\_merged\_graphql\_api

Creates an association between a Merged API and source API using the source
API's identifier.

Type annotations and code completion for `#!python session.create_client("appsync").associate_merged_graphql_api` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.associate_merged_graphql_api)

```python
# associate_merged_graphql_api method definition

await def associate_merged_graphql_api(
    self,
    *,
    sourceApiIdentifier: str,
    mergedApiIdentifier: str,
    description: str = ...,
    sourceApiAssociationConfig: SourceApiAssociationConfigTypeDef = ...,  # (1)
) -> AssociateMergedGraphqlApiResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SourceApiAssociationConfigTypeDef](./type_defs.md#sourceapiassociationconfigtypedef) 
2. See [:material-code-braces: AssociateMergedGraphqlApiResponseTypeDef](./type_defs.md#associatemergedgraphqlapiresponsetypedef) 


```python
# associate_merged_graphql_api method usage example with argument unpacking

kwargs: AssociateMergedGraphqlApiRequestRequestTypeDef = {  # (1)
    "sourceApiIdentifier": ...,
    "mergedApiIdentifier": ...,
}

parent.associate_merged_graphql_api(**kwargs)
```

1. See [:material-code-braces: AssociateMergedGraphqlApiRequestRequestTypeDef](./type_defs.md#associatemergedgraphqlapirequestrequesttypedef) 

### associate\_source\_graphql\_api

Creates an association between a Merged API and source API using the Merged
API's identifier.

Type annotations and code completion for `#!python session.create_client("appsync").associate_source_graphql_api` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.associate_source_graphql_api)

```python
# associate_source_graphql_api method definition

await def associate_source_graphql_api(
    self,
    *,
    mergedApiIdentifier: str,
    sourceApiIdentifier: str,
    description: str = ...,
    sourceApiAssociationConfig: SourceApiAssociationConfigTypeDef = ...,  # (1)
) -> AssociateSourceGraphqlApiResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SourceApiAssociationConfigTypeDef](./type_defs.md#sourceapiassociationconfigtypedef) 
2. See [:material-code-braces: AssociateSourceGraphqlApiResponseTypeDef](./type_defs.md#associatesourcegraphqlapiresponsetypedef) 


```python
# associate_source_graphql_api method usage example with argument unpacking

kwargs: AssociateSourceGraphqlApiRequestRequestTypeDef = {  # (1)
    "mergedApiIdentifier": ...,
    "sourceApiIdentifier": ...,
}

parent.associate_source_graphql_api(**kwargs)
```

1. See [:material-code-braces: AssociateSourceGraphqlApiRequestRequestTypeDef](./type_defs.md#associatesourcegraphqlapirequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("appsync").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("appsync").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_api\_cache

Creates a cache for the GraphQL API.

Type annotations and code completion for `#!python session.create_client("appsync").create_api_cache` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.create_api_cache)

```python
# create_api_cache method definition

await def create_api_cache(
    self,
    *,
    apiId: str,
    ttl: int,
    apiCachingBehavior: ApiCachingBehaviorType,  # (1)
    type: ApiCacheTypeType,  # (2)
    transitEncryptionEnabled: bool = ...,
    atRestEncryptionEnabled: bool = ...,
) -> CreateApiCacheResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ApiCachingBehaviorType](./literals.md#apicachingbehaviortype) 
2. See [:material-code-brackets: ApiCacheTypeType](./literals.md#apicachetypetype) 
3. See [:material-code-braces: CreateApiCacheResponseTypeDef](./type_defs.md#createapicacheresponsetypedef) 


```python
# create_api_cache method usage example with argument unpacking

kwargs: CreateApiCacheRequestRequestTypeDef = {  # (1)
    "apiId": ...,
    "ttl": ...,
    "apiCachingBehavior": ...,
    "type": ...,
}

parent.create_api_cache(**kwargs)
```

1. See [:material-code-braces: CreateApiCacheRequestRequestTypeDef](./type_defs.md#createapicacherequestrequesttypedef) 

### create\_api\_key

Creates a unique key that you can distribute to clients who invoke your API.

Type annotations and code completion for `#!python session.create_client("appsync").create_api_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.create_api_key)

```python
# create_api_key method definition

await def create_api_key(
    self,
    *,
    apiId: str,
    description: str = ...,
    expires: int = ...,
) -> CreateApiKeyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateApiKeyResponseTypeDef](./type_defs.md#createapikeyresponsetypedef) 


```python
# create_api_key method usage example with argument unpacking

kwargs: CreateApiKeyRequestRequestTypeDef = {  # (1)
    "apiId": ...,
}

parent.create_api_key(**kwargs)
```

1. See [:material-code-braces: CreateApiKeyRequestRequestTypeDef](./type_defs.md#createapikeyrequestrequesttypedef) 

### create\_data\_source

Creates a `DataSource` object.

Type annotations and code completion for `#!python session.create_client("appsync").create_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.create_data_source)

```python
# create_data_source method definition

await def create_data_source(
    self,
    *,
    apiId: str,
    name: str,
    type: DataSourceTypeType,  # (1)
    description: str = ...,
    serviceRoleArn: str = ...,
    dynamodbConfig: DynamodbDataSourceConfigTypeDef = ...,  # (2)
    lambdaConfig: LambdaDataSourceConfigTypeDef = ...,  # (3)
    elasticsearchConfig: ElasticsearchDataSourceConfigTypeDef = ...,  # (4)
    openSearchServiceConfig: OpenSearchServiceDataSourceConfigTypeDef = ...,  # (5)
    httpConfig: HttpDataSourceConfigTypeDef = ...,  # (6)
    relationalDatabaseConfig: RelationalDatabaseDataSourceConfigTypeDef = ...,  # (7)
    eventBridgeConfig: EventBridgeDataSourceConfigTypeDef = ...,  # (8)
) -> CreateDataSourceResponseTypeDef:  # (9)
    ...
```

1. See [:material-code-brackets: DataSourceTypeType](./literals.md#datasourcetypetype) 
2. See [:material-code-braces: DynamodbDataSourceConfigTypeDef](./type_defs.md#dynamodbdatasourceconfigtypedef) 
3. See [:material-code-braces: LambdaDataSourceConfigTypeDef](./type_defs.md#lambdadatasourceconfigtypedef) 
4. See [:material-code-braces: ElasticsearchDataSourceConfigTypeDef](./type_defs.md#elasticsearchdatasourceconfigtypedef) 
5. See [:material-code-braces: OpenSearchServiceDataSourceConfigTypeDef](./type_defs.md#opensearchservicedatasourceconfigtypedef) 
6. See [:material-code-braces: HttpDataSourceConfigTypeDef](./type_defs.md#httpdatasourceconfigtypedef) 
7. See [:material-code-braces: RelationalDatabaseDataSourceConfigTypeDef](./type_defs.md#relationaldatabasedatasourceconfigtypedef) 
8. See [:material-code-braces: EventBridgeDataSourceConfigTypeDef](./type_defs.md#eventbridgedatasourceconfigtypedef) 
9. See [:material-code-braces: CreateDataSourceResponseTypeDef](./type_defs.md#createdatasourceresponsetypedef) 


```python
# create_data_source method usage example with argument unpacking

kwargs: CreateDataSourceRequestRequestTypeDef = {  # (1)
    "apiId": ...,
    "name": ...,
    "type": ...,
}

parent.create_data_source(**kwargs)
```

1. See [:material-code-braces: CreateDataSourceRequestRequestTypeDef](./type_defs.md#createdatasourcerequestrequesttypedef) 

### create\_domain\_name

Creates a custom `DomainName` object.

Type annotations and code completion for `#!python session.create_client("appsync").create_domain_name` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.create_domain_name)

```python
# create_domain_name method definition

await def create_domain_name(
    self,
    *,
    domainName: str,
    certificateArn: str,
    description: str = ...,
) -> CreateDomainNameResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateDomainNameResponseTypeDef](./type_defs.md#createdomainnameresponsetypedef) 


```python
# create_domain_name method usage example with argument unpacking

kwargs: CreateDomainNameRequestRequestTypeDef = {  # (1)
    "domainName": ...,
    "certificateArn": ...,
}

parent.create_domain_name(**kwargs)
```

1. See [:material-code-braces: CreateDomainNameRequestRequestTypeDef](./type_defs.md#createdomainnamerequestrequesttypedef) 

### create\_function

Creates a `Function` object.

Type annotations and code completion for `#!python session.create_client("appsync").create_function` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.create_function)

```python
# create_function method definition

await def create_function(
    self,
    *,
    apiId: str,
    name: str,
    dataSourceName: str,
    description: str = ...,
    requestMappingTemplate: str = ...,
    responseMappingTemplate: str = ...,
    functionVersion: str = ...,
    syncConfig: SyncConfigTypeDef = ...,  # (1)
    maxBatchSize: int = ...,
    runtime: AppSyncRuntimeTypeDef = ...,  # (2)
    code: str = ...,
) -> CreateFunctionResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SyncConfigTypeDef](./type_defs.md#syncconfigtypedef) 
2. See [:material-code-braces: AppSyncRuntimeTypeDef](./type_defs.md#appsyncruntimetypedef) 
3. See [:material-code-braces: CreateFunctionResponseTypeDef](./type_defs.md#createfunctionresponsetypedef) 


```python
# create_function method usage example with argument unpacking

kwargs: CreateFunctionRequestRequestTypeDef = {  # (1)
    "apiId": ...,
    "name": ...,
    "dataSourceName": ...,
}

parent.create_function(**kwargs)
```

1. See [:material-code-braces: CreateFunctionRequestRequestTypeDef](./type_defs.md#createfunctionrequestrequesttypedef) 

### create\_graphql\_api

Creates a `GraphqlApi` object.

Type annotations and code completion for `#!python session.create_client("appsync").create_graphql_api` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.create_graphql_api)

```python
# create_graphql_api method definition

await def create_graphql_api(
    self,
    *,
    name: str,
    authenticationType: AuthenticationTypeType,  # (1)
    logConfig: LogConfigTypeDef = ...,  # (2)
    userPoolConfig: UserPoolConfigTypeDef = ...,  # (3)
    openIDConnectConfig: OpenIDConnectConfigTypeDef = ...,  # (4)
    tags: Mapping[str, str] = ...,
    additionalAuthenticationProviders: Sequence[AdditionalAuthenticationProviderTypeDef] = ...,  # (5)
    xrayEnabled: bool = ...,
    lambdaAuthorizerConfig: LambdaAuthorizerConfigTypeDef = ...,  # (6)
    visibility: GraphQLApiVisibilityType = ...,  # (7)
    apiType: GraphQLApiTypeType = ...,  # (8)
    mergedApiExecutionRoleArn: str = ...,
    ownerContact: str = ...,
) -> CreateGraphqlApiResponseTypeDef:  # (9)
    ...
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
2. See [:material-code-braces: LogConfigTypeDef](./type_defs.md#logconfigtypedef) 
3. See [:material-code-braces: UserPoolConfigTypeDef](./type_defs.md#userpoolconfigtypedef) 
4. See [:material-code-braces: OpenIDConnectConfigTypeDef](./type_defs.md#openidconnectconfigtypedef) 
5. See [:material-code-braces: AdditionalAuthenticationProviderTypeDef](./type_defs.md#additionalauthenticationprovidertypedef) 
6. See [:material-code-braces: LambdaAuthorizerConfigTypeDef](./type_defs.md#lambdaauthorizerconfigtypedef) 
7. See [:material-code-brackets: GraphQLApiVisibilityType](./literals.md#graphqlapivisibilitytype) 
8. See [:material-code-brackets: GraphQLApiTypeType](./literals.md#graphqlapitypetype) 
9. See [:material-code-braces: CreateGraphqlApiResponseTypeDef](./type_defs.md#creategraphqlapiresponsetypedef) 


```python
# create_graphql_api method usage example with argument unpacking

kwargs: CreateGraphqlApiRequestRequestTypeDef = {  # (1)
    "name": ...,
    "authenticationType": ...,
}

parent.create_graphql_api(**kwargs)
```

1. See [:material-code-braces: CreateGraphqlApiRequestRequestTypeDef](./type_defs.md#creategraphqlapirequestrequesttypedef) 

### create\_resolver

Creates a `Resolver` object.

Type annotations and code completion for `#!python session.create_client("appsync").create_resolver` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.create_resolver)

```python
# create_resolver method definition

await def create_resolver(
    self,
    *,
    apiId: str,
    typeName: str,
    fieldName: str,
    dataSourceName: str = ...,
    requestMappingTemplate: str = ...,
    responseMappingTemplate: str = ...,
    kind: ResolverKindType = ...,  # (1)
    pipelineConfig: PipelineConfigTypeDef = ...,  # (2)
    syncConfig: SyncConfigTypeDef = ...,  # (3)
    cachingConfig: CachingConfigTypeDef = ...,  # (4)
    maxBatchSize: int = ...,
    runtime: AppSyncRuntimeTypeDef = ...,  # (5)
    code: str = ...,
) -> CreateResolverResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: ResolverKindType](./literals.md#resolverkindtype) 
2. See [:material-code-braces: PipelineConfigTypeDef](./type_defs.md#pipelineconfigtypedef) 
3. See [:material-code-braces: SyncConfigTypeDef](./type_defs.md#syncconfigtypedef) 
4. See [:material-code-braces: CachingConfigTypeDef](./type_defs.md#cachingconfigtypedef) 
5. See [:material-code-braces: AppSyncRuntimeTypeDef](./type_defs.md#appsyncruntimetypedef) 
6. See [:material-code-braces: CreateResolverResponseTypeDef](./type_defs.md#createresolverresponsetypedef) 


```python
# create_resolver method usage example with argument unpacking

kwargs: CreateResolverRequestRequestTypeDef = {  # (1)
    "apiId": ...,
    "typeName": ...,
    "fieldName": ...,
}

parent.create_resolver(**kwargs)
```

1. See [:material-code-braces: CreateResolverRequestRequestTypeDef](./type_defs.md#createresolverrequestrequesttypedef) 

### create\_type

Creates a `Type` object.

Type annotations and code completion for `#!python session.create_client("appsync").create_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.create_type)

```python
# create_type method definition

await def create_type(
    self,
    *,
    apiId: str,
    definition: str,
    format: TypeDefinitionFormatType,  # (1)
) -> CreateTypeResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TypeDefinitionFormatType](./literals.md#typedefinitionformattype) 
2. See [:material-code-braces: CreateTypeResponseTypeDef](./type_defs.md#createtyperesponsetypedef) 


```python
# create_type method usage example with argument unpacking

kwargs: CreateTypeRequestRequestTypeDef = {  # (1)
    "apiId": ...,
    "definition": ...,
    "format": ...,
}

parent.create_type(**kwargs)
```

1. See [:material-code-braces: CreateTypeRequestRequestTypeDef](./type_defs.md#createtyperequestrequesttypedef) 

### delete\_api\_cache

Deletes an `ApiCache` object.

Type annotations and code completion for `#!python session.create_client("appsync").delete_api_cache` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.delete_api_cache)

```python
# delete_api_cache method definition

await def delete_api_cache(
    self,
    *,
    apiId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_api_cache method usage example with argument unpacking

kwargs: DeleteApiCacheRequestRequestTypeDef = {  # (1)
    "apiId": ...,
}

parent.delete_api_cache(**kwargs)
```

1. See [:material-code-braces: DeleteApiCacheRequestRequestTypeDef](./type_defs.md#deleteapicacherequestrequesttypedef) 

### delete\_api\_key

Deletes an API key.

Type annotations and code completion for `#!python session.create_client("appsync").delete_api_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.delete_api_key)

```python
# delete_api_key method definition

await def delete_api_key(
    self,
    *,
    apiId: str,
    id: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_api_key method usage example with argument unpacking

kwargs: DeleteApiKeyRequestRequestTypeDef = {  # (1)
    "apiId": ...,
    "id": ...,
}

parent.delete_api_key(**kwargs)
```

1. See [:material-code-braces: DeleteApiKeyRequestRequestTypeDef](./type_defs.md#deleteapikeyrequestrequesttypedef) 

### delete\_data\_source

Deletes a `DataSource` object.

Type annotations and code completion for `#!python session.create_client("appsync").delete_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.delete_data_source)

```python
# delete_data_source method definition

await def delete_data_source(
    self,
    *,
    apiId: str,
    name: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_data_source method usage example with argument unpacking

kwargs: DeleteDataSourceRequestRequestTypeDef = {  # (1)
    "apiId": ...,
    "name": ...,
}

parent.delete_data_source(**kwargs)
```

1. See [:material-code-braces: DeleteDataSourceRequestRequestTypeDef](./type_defs.md#deletedatasourcerequestrequesttypedef) 

### delete\_domain\_name

Deletes a custom `DomainName` object.

Type annotations and code completion for `#!python session.create_client("appsync").delete_domain_name` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.delete_domain_name)

```python
# delete_domain_name method definition

await def delete_domain_name(
    self,
    *,
    domainName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_domain_name method usage example with argument unpacking

kwargs: DeleteDomainNameRequestRequestTypeDef = {  # (1)
    "domainName": ...,
}

parent.delete_domain_name(**kwargs)
```

1. See [:material-code-braces: DeleteDomainNameRequestRequestTypeDef](./type_defs.md#deletedomainnamerequestrequesttypedef) 

### delete\_function

Deletes a `Function`.

Type annotations and code completion for `#!python session.create_client("appsync").delete_function` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.delete_function)

```python
# delete_function method definition

await def delete_function(
    self,
    *,
    apiId: str,
    functionId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_function method usage example with argument unpacking

kwargs: DeleteFunctionRequestRequestTypeDef = {  # (1)
    "apiId": ...,
    "functionId": ...,
}

parent.delete_function(**kwargs)
```

1. See [:material-code-braces: DeleteFunctionRequestRequestTypeDef](./type_defs.md#deletefunctionrequestrequesttypedef) 

### delete\_graphql\_api

Deletes a `GraphqlApi` object.

Type annotations and code completion for `#!python session.create_client("appsync").delete_graphql_api` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.delete_graphql_api)

```python
# delete_graphql_api method definition

await def delete_graphql_api(
    self,
    *,
    apiId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_graphql_api method usage example with argument unpacking

kwargs: DeleteGraphqlApiRequestRequestTypeDef = {  # (1)
    "apiId": ...,
}

parent.delete_graphql_api(**kwargs)
```

1. See [:material-code-braces: DeleteGraphqlApiRequestRequestTypeDef](./type_defs.md#deletegraphqlapirequestrequesttypedef) 

### delete\_resolver

Deletes a `Resolver` object.

Type annotations and code completion for `#!python session.create_client("appsync").delete_resolver` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.delete_resolver)

```python
# delete_resolver method definition

await def delete_resolver(
    self,
    *,
    apiId: str,
    typeName: str,
    fieldName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_resolver method usage example with argument unpacking

kwargs: DeleteResolverRequestRequestTypeDef = {  # (1)
    "apiId": ...,
    "typeName": ...,
    "fieldName": ...,
}

parent.delete_resolver(**kwargs)
```

1. See [:material-code-braces: DeleteResolverRequestRequestTypeDef](./type_defs.md#deleteresolverrequestrequesttypedef) 

### delete\_type

Deletes a `Type` object.

Type annotations and code completion for `#!python session.create_client("appsync").delete_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.delete_type)

```python
# delete_type method definition

await def delete_type(
    self,
    *,
    apiId: str,
    typeName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_type method usage example with argument unpacking

kwargs: DeleteTypeRequestRequestTypeDef = {  # (1)
    "apiId": ...,
    "typeName": ...,
}

parent.delete_type(**kwargs)
```

1. See [:material-code-braces: DeleteTypeRequestRequestTypeDef](./type_defs.md#deletetyperequestrequesttypedef) 

### disassociate\_api

Removes an `ApiAssociation` object from a custom domain.

Type annotations and code completion for `#!python session.create_client("appsync").disassociate_api` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.disassociate_api)

```python
# disassociate_api method definition

await def disassociate_api(
    self,
    *,
    domainName: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_api method usage example with argument unpacking

kwargs: DisassociateApiRequestRequestTypeDef = {  # (1)
    "domainName": ...,
}

parent.disassociate_api(**kwargs)
```

1. See [:material-code-braces: DisassociateApiRequestRequestTypeDef](./type_defs.md#disassociateapirequestrequesttypedef) 

### disassociate\_merged\_graphql\_api

Deletes an association between a Merged API and source API using the source
API's identifier and the association ID.

Type annotations and code completion for `#!python session.create_client("appsync").disassociate_merged_graphql_api` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.disassociate_merged_graphql_api)

```python
# disassociate_merged_graphql_api method definition

await def disassociate_merged_graphql_api(
    self,
    *,
    sourceApiIdentifier: str,
    associationId: str,
) -> DisassociateMergedGraphqlApiResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DisassociateMergedGraphqlApiResponseTypeDef](./type_defs.md#disassociatemergedgraphqlapiresponsetypedef) 


```python
# disassociate_merged_graphql_api method usage example with argument unpacking

kwargs: DisassociateMergedGraphqlApiRequestRequestTypeDef = {  # (1)
    "sourceApiIdentifier": ...,
    "associationId": ...,
}

parent.disassociate_merged_graphql_api(**kwargs)
```

1. See [:material-code-braces: DisassociateMergedGraphqlApiRequestRequestTypeDef](./type_defs.md#disassociatemergedgraphqlapirequestrequesttypedef) 

### disassociate\_source\_graphql\_api

Deletes an association between a Merged API and source API using the Merged
API's identifier and the association ID.

Type annotations and code completion for `#!python session.create_client("appsync").disassociate_source_graphql_api` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.disassociate_source_graphql_api)

```python
# disassociate_source_graphql_api method definition

await def disassociate_source_graphql_api(
    self,
    *,
    mergedApiIdentifier: str,
    associationId: str,
) -> DisassociateSourceGraphqlApiResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DisassociateSourceGraphqlApiResponseTypeDef](./type_defs.md#disassociatesourcegraphqlapiresponsetypedef) 


```python
# disassociate_source_graphql_api method usage example with argument unpacking

kwargs: DisassociateSourceGraphqlApiRequestRequestTypeDef = {  # (1)
    "mergedApiIdentifier": ...,
    "associationId": ...,
}

parent.disassociate_source_graphql_api(**kwargs)
```

1. See [:material-code-braces: DisassociateSourceGraphqlApiRequestRequestTypeDef](./type_defs.md#disassociatesourcegraphqlapirequestrequesttypedef) 

### evaluate\_code

Evaluates the given code and returns the response.

Type annotations and code completion for `#!python session.create_client("appsync").evaluate_code` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.evaluate_code)

```python
# evaluate_code method definition

await def evaluate_code(
    self,
    *,
    runtime: AppSyncRuntimeTypeDef,  # (1)
    code: str,
    context: str,
    function: str = ...,
) -> EvaluateCodeResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AppSyncRuntimeTypeDef](./type_defs.md#appsyncruntimetypedef) 
2. See [:material-code-braces: EvaluateCodeResponseTypeDef](./type_defs.md#evaluatecoderesponsetypedef) 


```python
# evaluate_code method usage example with argument unpacking

kwargs: EvaluateCodeRequestRequestTypeDef = {  # (1)
    "runtime": ...,
    "code": ...,
    "context": ...,
}

parent.evaluate_code(**kwargs)
```

1. See [:material-code-braces: EvaluateCodeRequestRequestTypeDef](./type_defs.md#evaluatecoderequestrequesttypedef) 

### evaluate\_mapping\_template

Evaluates a given template and returns the response.

Type annotations and code completion for `#!python session.create_client("appsync").evaluate_mapping_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.evaluate_mapping_template)

```python
# evaluate_mapping_template method definition

await def evaluate_mapping_template(
    self,
    *,
    template: str,
    context: str,
) -> EvaluateMappingTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EvaluateMappingTemplateResponseTypeDef](./type_defs.md#evaluatemappingtemplateresponsetypedef) 


```python
# evaluate_mapping_template method usage example with argument unpacking

kwargs: EvaluateMappingTemplateRequestRequestTypeDef = {  # (1)
    "template": ...,
    "context": ...,
}

parent.evaluate_mapping_template(**kwargs)
```

1. See [:material-code-braces: EvaluateMappingTemplateRequestRequestTypeDef](./type_defs.md#evaluatemappingtemplaterequestrequesttypedef) 

### flush\_api\_cache

Flushes an `ApiCache` object.

Type annotations and code completion for `#!python session.create_client("appsync").flush_api_cache` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.flush_api_cache)

```python
# flush_api_cache method definition

await def flush_api_cache(
    self,
    *,
    apiId: str,
) -> Dict[str, Any]:
    ...
```



```python
# flush_api_cache method usage example with argument unpacking

kwargs: FlushApiCacheRequestRequestTypeDef = {  # (1)
    "apiId": ...,
}

parent.flush_api_cache(**kwargs)
```

1. See [:material-code-braces: FlushApiCacheRequestRequestTypeDef](./type_defs.md#flushapicacherequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("appsync").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.generate_presigned_url)

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


### get\_api\_association

Retrieves an `ApiAssociation` object.

Type annotations and code completion for `#!python session.create_client("appsync").get_api_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.get_api_association)

```python
# get_api_association method definition

await def get_api_association(
    self,
    *,
    domainName: str,
) -> GetApiAssociationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetApiAssociationResponseTypeDef](./type_defs.md#getapiassociationresponsetypedef) 


```python
# get_api_association method usage example with argument unpacking

kwargs: GetApiAssociationRequestRequestTypeDef = {  # (1)
    "domainName": ...,
}

parent.get_api_association(**kwargs)
```

1. See [:material-code-braces: GetApiAssociationRequestRequestTypeDef](./type_defs.md#getapiassociationrequestrequesttypedef) 

### get\_api\_cache

Retrieves an `ApiCache` object.

Type annotations and code completion for `#!python session.create_client("appsync").get_api_cache` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.get_api_cache)

```python
# get_api_cache method definition

await def get_api_cache(
    self,
    *,
    apiId: str,
) -> GetApiCacheResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetApiCacheResponseTypeDef](./type_defs.md#getapicacheresponsetypedef) 


```python
# get_api_cache method usage example with argument unpacking

kwargs: GetApiCacheRequestRequestTypeDef = {  # (1)
    "apiId": ...,
}

parent.get_api_cache(**kwargs)
```

1. See [:material-code-braces: GetApiCacheRequestRequestTypeDef](./type_defs.md#getapicacherequestrequesttypedef) 

### get\_data\_source

Retrieves a `DataSource` object.

Type annotations and code completion for `#!python session.create_client("appsync").get_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.get_data_source)

```python
# get_data_source method definition

await def get_data_source(
    self,
    *,
    apiId: str,
    name: str,
) -> GetDataSourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataSourceResponseTypeDef](./type_defs.md#getdatasourceresponsetypedef) 


```python
# get_data_source method usage example with argument unpacking

kwargs: GetDataSourceRequestRequestTypeDef = {  # (1)
    "apiId": ...,
    "name": ...,
}

parent.get_data_source(**kwargs)
```

1. See [:material-code-braces: GetDataSourceRequestRequestTypeDef](./type_defs.md#getdatasourcerequestrequesttypedef) 

### get\_domain\_name

Retrieves a custom `DomainName` object.

Type annotations and code completion for `#!python session.create_client("appsync").get_domain_name` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.get_domain_name)

```python
# get_domain_name method definition

await def get_domain_name(
    self,
    *,
    domainName: str,
) -> GetDomainNameResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDomainNameResponseTypeDef](./type_defs.md#getdomainnameresponsetypedef) 


```python
# get_domain_name method usage example with argument unpacking

kwargs: GetDomainNameRequestRequestTypeDef = {  # (1)
    "domainName": ...,
}

parent.get_domain_name(**kwargs)
```

1. See [:material-code-braces: GetDomainNameRequestRequestTypeDef](./type_defs.md#getdomainnamerequestrequesttypedef) 

### get\_function

Get a `Function`.

Type annotations and code completion for `#!python session.create_client("appsync").get_function` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.get_function)

```python
# get_function method definition

await def get_function(
    self,
    *,
    apiId: str,
    functionId: str,
) -> GetFunctionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFunctionResponseTypeDef](./type_defs.md#getfunctionresponsetypedef) 


```python
# get_function method usage example with argument unpacking

kwargs: GetFunctionRequestRequestTypeDef = {  # (1)
    "apiId": ...,
    "functionId": ...,
}

parent.get_function(**kwargs)
```

1. See [:material-code-braces: GetFunctionRequestRequestTypeDef](./type_defs.md#getfunctionrequestrequesttypedef) 

### get\_graphql\_api

Retrieves a `GraphqlApi` object.

Type annotations and code completion for `#!python session.create_client("appsync").get_graphql_api` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.get_graphql_api)

```python
# get_graphql_api method definition

await def get_graphql_api(
    self,
    *,
    apiId: str,
) -> GetGraphqlApiResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetGraphqlApiResponseTypeDef](./type_defs.md#getgraphqlapiresponsetypedef) 


```python
# get_graphql_api method usage example with argument unpacking

kwargs: GetGraphqlApiRequestRequestTypeDef = {  # (1)
    "apiId": ...,
}

parent.get_graphql_api(**kwargs)
```

1. See [:material-code-braces: GetGraphqlApiRequestRequestTypeDef](./type_defs.md#getgraphqlapirequestrequesttypedef) 

### get\_introspection\_schema

Retrieves the introspection schema for a GraphQL API.

Type annotations and code completion for `#!python session.create_client("appsync").get_introspection_schema` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.get_introspection_schema)

```python
# get_introspection_schema method definition

await def get_introspection_schema(
    self,
    *,
    apiId: str,
    format: OutputTypeType,  # (1)
    includeDirectives: bool = ...,
) -> GetIntrospectionSchemaResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: OutputTypeType](./literals.md#outputtypetype) 
2. See [:material-code-braces: GetIntrospectionSchemaResponseTypeDef](./type_defs.md#getintrospectionschemaresponsetypedef) 


```python
# get_introspection_schema method usage example with argument unpacking

kwargs: GetIntrospectionSchemaRequestRequestTypeDef = {  # (1)
    "apiId": ...,
    "format": ...,
}

parent.get_introspection_schema(**kwargs)
```

1. See [:material-code-braces: GetIntrospectionSchemaRequestRequestTypeDef](./type_defs.md#getintrospectionschemarequestrequesttypedef) 

### get\_resolver

Retrieves a `Resolver` object.

Type annotations and code completion for `#!python session.create_client("appsync").get_resolver` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.get_resolver)

```python
# get_resolver method definition

await def get_resolver(
    self,
    *,
    apiId: str,
    typeName: str,
    fieldName: str,
) -> GetResolverResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResolverResponseTypeDef](./type_defs.md#getresolverresponsetypedef) 


```python
# get_resolver method usage example with argument unpacking

kwargs: GetResolverRequestRequestTypeDef = {  # (1)
    "apiId": ...,
    "typeName": ...,
    "fieldName": ...,
}

parent.get_resolver(**kwargs)
```

1. See [:material-code-braces: GetResolverRequestRequestTypeDef](./type_defs.md#getresolverrequestrequesttypedef) 

### get\_schema\_creation\_status

Retrieves the current status of a schema creation operation.

Type annotations and code completion for `#!python session.create_client("appsync").get_schema_creation_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.get_schema_creation_status)

```python
# get_schema_creation_status method definition

await def get_schema_creation_status(
    self,
    *,
    apiId: str,
) -> GetSchemaCreationStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSchemaCreationStatusResponseTypeDef](./type_defs.md#getschemacreationstatusresponsetypedef) 


```python
# get_schema_creation_status method usage example with argument unpacking

kwargs: GetSchemaCreationStatusRequestRequestTypeDef = {  # (1)
    "apiId": ...,
}

parent.get_schema_creation_status(**kwargs)
```

1. See [:material-code-braces: GetSchemaCreationStatusRequestRequestTypeDef](./type_defs.md#getschemacreationstatusrequestrequesttypedef) 

### get\_source\_api\_association

Retrieves a `SourceApiAssociation` object.

Type annotations and code completion for `#!python session.create_client("appsync").get_source_api_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.get_source_api_association)

```python
# get_source_api_association method definition

await def get_source_api_association(
    self,
    *,
    mergedApiIdentifier: str,
    associationId: str,
) -> GetSourceApiAssociationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSourceApiAssociationResponseTypeDef](./type_defs.md#getsourceapiassociationresponsetypedef) 


```python
# get_source_api_association method usage example with argument unpacking

kwargs: GetSourceApiAssociationRequestRequestTypeDef = {  # (1)
    "mergedApiIdentifier": ...,
    "associationId": ...,
}

parent.get_source_api_association(**kwargs)
```

1. See [:material-code-braces: GetSourceApiAssociationRequestRequestTypeDef](./type_defs.md#getsourceapiassociationrequestrequesttypedef) 

### get\_type

Retrieves a `Type` object.

Type annotations and code completion for `#!python session.create_client("appsync").get_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.get_type)

```python
# get_type method definition

await def get_type(
    self,
    *,
    apiId: str,
    typeName: str,
    format: TypeDefinitionFormatType,  # (1)
) -> GetTypeResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TypeDefinitionFormatType](./literals.md#typedefinitionformattype) 
2. See [:material-code-braces: GetTypeResponseTypeDef](./type_defs.md#gettyperesponsetypedef) 


```python
# get_type method usage example with argument unpacking

kwargs: GetTypeRequestRequestTypeDef = {  # (1)
    "apiId": ...,
    "typeName": ...,
    "format": ...,
}

parent.get_type(**kwargs)
```

1. See [:material-code-braces: GetTypeRequestRequestTypeDef](./type_defs.md#gettyperequestrequesttypedef) 

### list\_api\_keys

Lists the API keys for a given API.

Type annotations and code completion for `#!python session.create_client("appsync").list_api_keys` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_api_keys)

```python
# list_api_keys method definition

await def list_api_keys(
    self,
    *,
    apiId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListApiKeysResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListApiKeysResponseTypeDef](./type_defs.md#listapikeysresponsetypedef) 


```python
# list_api_keys method usage example with argument unpacking

kwargs: ListApiKeysRequestRequestTypeDef = {  # (1)
    "apiId": ...,
}

parent.list_api_keys(**kwargs)
```

1. See [:material-code-braces: ListApiKeysRequestRequestTypeDef](./type_defs.md#listapikeysrequestrequesttypedef) 

### list\_data\_sources

Lists the data sources for a given API.

Type annotations and code completion for `#!python session.create_client("appsync").list_data_sources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_data_sources)

```python
# list_data_sources method definition

await def list_data_sources(
    self,
    *,
    apiId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListDataSourcesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDataSourcesResponseTypeDef](./type_defs.md#listdatasourcesresponsetypedef) 


```python
# list_data_sources method usage example with argument unpacking

kwargs: ListDataSourcesRequestRequestTypeDef = {  # (1)
    "apiId": ...,
}

parent.list_data_sources(**kwargs)
```

1. See [:material-code-braces: ListDataSourcesRequestRequestTypeDef](./type_defs.md#listdatasourcesrequestrequesttypedef) 

### list\_domain\_names

Lists multiple custom domain names.

Type annotations and code completion for `#!python session.create_client("appsync").list_domain_names` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_domain_names)

```python
# list_domain_names method definition

await def list_domain_names(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListDomainNamesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDomainNamesResponseTypeDef](./type_defs.md#listdomainnamesresponsetypedef) 


```python
# list_domain_names method usage example with argument unpacking

kwargs: ListDomainNamesRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_domain_names(**kwargs)
```

1. See [:material-code-braces: ListDomainNamesRequestRequestTypeDef](./type_defs.md#listdomainnamesrequestrequesttypedef) 

### list\_functions

List multiple functions.

Type annotations and code completion for `#!python session.create_client("appsync").list_functions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_functions)

```python
# list_functions method definition

await def list_functions(
    self,
    *,
    apiId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListFunctionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFunctionsResponseTypeDef](./type_defs.md#listfunctionsresponsetypedef) 


```python
# list_functions method usage example with argument unpacking

kwargs: ListFunctionsRequestRequestTypeDef = {  # (1)
    "apiId": ...,
}

parent.list_functions(**kwargs)
```

1. See [:material-code-braces: ListFunctionsRequestRequestTypeDef](./type_defs.md#listfunctionsrequestrequesttypedef) 

### list\_graphql\_apis

Lists your GraphQL APIs.

Type annotations and code completion for `#!python session.create_client("appsync").list_graphql_apis` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_graphql_apis)

```python
# list_graphql_apis method definition

await def list_graphql_apis(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
    apiType: GraphQLApiTypeType = ...,  # (1)
    owner: OwnershipType = ...,  # (2)
) -> ListGraphqlApisResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: GraphQLApiTypeType](./literals.md#graphqlapitypetype) 
2. See [:material-code-brackets: OwnershipType](./literals.md#ownershiptype) 
3. See [:material-code-braces: ListGraphqlApisResponseTypeDef](./type_defs.md#listgraphqlapisresponsetypedef) 


```python
# list_graphql_apis method usage example with argument unpacking

kwargs: ListGraphqlApisRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_graphql_apis(**kwargs)
```

1. See [:material-code-braces: ListGraphqlApisRequestRequestTypeDef](./type_defs.md#listgraphqlapisrequestrequesttypedef) 

### list\_resolvers

Lists the resolvers for a given API and type.

Type annotations and code completion for `#!python session.create_client("appsync").list_resolvers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_resolvers)

```python
# list_resolvers method definition

await def list_resolvers(
    self,
    *,
    apiId: str,
    typeName: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListResolversResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListResolversResponseTypeDef](./type_defs.md#listresolversresponsetypedef) 


```python
# list_resolvers method usage example with argument unpacking

kwargs: ListResolversRequestRequestTypeDef = {  # (1)
    "apiId": ...,
    "typeName": ...,
}

parent.list_resolvers(**kwargs)
```

1. See [:material-code-braces: ListResolversRequestRequestTypeDef](./type_defs.md#listresolversrequestrequesttypedef) 

### list\_resolvers\_by\_function

List the resolvers that are associated with a specific function.

Type annotations and code completion for `#!python session.create_client("appsync").list_resolvers_by_function` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_resolvers_by_function)

```python
# list_resolvers_by_function method definition

await def list_resolvers_by_function(
    self,
    *,
    apiId: str,
    functionId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListResolversByFunctionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListResolversByFunctionResponseTypeDef](./type_defs.md#listresolversbyfunctionresponsetypedef) 


```python
# list_resolvers_by_function method usage example with argument unpacking

kwargs: ListResolversByFunctionRequestRequestTypeDef = {  # (1)
    "apiId": ...,
    "functionId": ...,
}

parent.list_resolvers_by_function(**kwargs)
```

1. See [:material-code-braces: ListResolversByFunctionRequestRequestTypeDef](./type_defs.md#listresolversbyfunctionrequestrequesttypedef) 

### list\_source\_api\_associations

Lists the `SourceApiAssociationSummary` data.

Type annotations and code completion for `#!python session.create_client("appsync").list_source_api_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_source_api_associations)

```python
# list_source_api_associations method definition

await def list_source_api_associations(
    self,
    *,
    apiId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListSourceApiAssociationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSourceApiAssociationsResponseTypeDef](./type_defs.md#listsourceapiassociationsresponsetypedef) 


```python
# list_source_api_associations method usage example with argument unpacking

kwargs: ListSourceApiAssociationsRequestRequestTypeDef = {  # (1)
    "apiId": ...,
}

parent.list_source_api_associations(**kwargs)
```

1. See [:material-code-braces: ListSourceApiAssociationsRequestRequestTypeDef](./type_defs.md#listsourceapiassociationsrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags for a resource.

Type annotations and code completion for `#!python session.create_client("appsync").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_types

Lists the types for a given API.

Type annotations and code completion for `#!python session.create_client("appsync").list_types` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_types)

```python
# list_types method definition

await def list_types(
    self,
    *,
    apiId: str,
    format: TypeDefinitionFormatType,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListTypesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TypeDefinitionFormatType](./literals.md#typedefinitionformattype) 
2. See [:material-code-braces: ListTypesResponseTypeDef](./type_defs.md#listtypesresponsetypedef) 


```python
# list_types method usage example with argument unpacking

kwargs: ListTypesRequestRequestTypeDef = {  # (1)
    "apiId": ...,
    "format": ...,
}

parent.list_types(**kwargs)
```

1. See [:material-code-braces: ListTypesRequestRequestTypeDef](./type_defs.md#listtypesrequestrequesttypedef) 

### list\_types\_by\_association

Lists `Type` objects by the source API association ID.

Type annotations and code completion for `#!python session.create_client("appsync").list_types_by_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_types_by_association)

```python
# list_types_by_association method definition

await def list_types_by_association(
    self,
    *,
    mergedApiIdentifier: str,
    associationId: str,
    format: TypeDefinitionFormatType,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListTypesByAssociationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TypeDefinitionFormatType](./literals.md#typedefinitionformattype) 
2. See [:material-code-braces: ListTypesByAssociationResponseTypeDef](./type_defs.md#listtypesbyassociationresponsetypedef) 


```python
# list_types_by_association method usage example with argument unpacking

kwargs: ListTypesByAssociationRequestRequestTypeDef = {  # (1)
    "mergedApiIdentifier": ...,
    "associationId": ...,
    "format": ...,
}

parent.list_types_by_association(**kwargs)
```

1. See [:material-code-braces: ListTypesByAssociationRequestRequestTypeDef](./type_defs.md#listtypesbyassociationrequestrequesttypedef) 

### start\_schema\_creation

Adds a new schema to your GraphQL API.

Type annotations and code completion for `#!python session.create_client("appsync").start_schema_creation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.start_schema_creation)

```python
# start_schema_creation method definition

await def start_schema_creation(
    self,
    *,
    apiId: str,
    definition: Union[str, bytes, IO[Any], StreamingBody],
) -> StartSchemaCreationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartSchemaCreationResponseTypeDef](./type_defs.md#startschemacreationresponsetypedef) 


```python
# start_schema_creation method usage example with argument unpacking

kwargs: StartSchemaCreationRequestRequestTypeDef = {  # (1)
    "apiId": ...,
    "definition": ...,
}

parent.start_schema_creation(**kwargs)
```

1. See [:material-code-braces: StartSchemaCreationRequestRequestTypeDef](./type_defs.md#startschemacreationrequestrequesttypedef) 

### start\_schema\_merge

Initiates a merge operation.

Type annotations and code completion for `#!python session.create_client("appsync").start_schema_merge` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.start_schema_merge)

```python
# start_schema_merge method definition

await def start_schema_merge(
    self,
    *,
    associationId: str,
    mergedApiIdentifier: str,
) -> StartSchemaMergeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartSchemaMergeResponseTypeDef](./type_defs.md#startschemamergeresponsetypedef) 


```python
# start_schema_merge method usage example with argument unpacking

kwargs: StartSchemaMergeRequestRequestTypeDef = {  # (1)
    "associationId": ...,
    "mergedApiIdentifier": ...,
}

parent.start_schema_merge(**kwargs)
```

1. See [:material-code-braces: StartSchemaMergeRequestRequestTypeDef](./type_defs.md#startschemamergerequestrequesttypedef) 

### tag\_resource

Tags a resource with user-supplied tags.

Type annotations and code completion for `#!python session.create_client("appsync").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Untags a resource.

Type annotations and code completion for `#!python session.create_client("appsync").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_api\_cache

Updates the cache for the GraphQL API.

Type annotations and code completion for `#!python session.create_client("appsync").update_api_cache` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.update_api_cache)

```python
# update_api_cache method definition

await def update_api_cache(
    self,
    *,
    apiId: str,
    ttl: int,
    apiCachingBehavior: ApiCachingBehaviorType,  # (1)
    type: ApiCacheTypeType,  # (2)
) -> UpdateApiCacheResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ApiCachingBehaviorType](./literals.md#apicachingbehaviortype) 
2. See [:material-code-brackets: ApiCacheTypeType](./literals.md#apicachetypetype) 
3. See [:material-code-braces: UpdateApiCacheResponseTypeDef](./type_defs.md#updateapicacheresponsetypedef) 


```python
# update_api_cache method usage example with argument unpacking

kwargs: UpdateApiCacheRequestRequestTypeDef = {  # (1)
    "apiId": ...,
    "ttl": ...,
    "apiCachingBehavior": ...,
    "type": ...,
}

parent.update_api_cache(**kwargs)
```

1. See [:material-code-braces: UpdateApiCacheRequestRequestTypeDef](./type_defs.md#updateapicacherequestrequesttypedef) 

### update\_api\_key

Updates an API key.

Type annotations and code completion for `#!python session.create_client("appsync").update_api_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.update_api_key)

```python
# update_api_key method definition

await def update_api_key(
    self,
    *,
    apiId: str,
    id: str,
    description: str = ...,
    expires: int = ...,
) -> UpdateApiKeyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateApiKeyResponseTypeDef](./type_defs.md#updateapikeyresponsetypedef) 


```python
# update_api_key method usage example with argument unpacking

kwargs: UpdateApiKeyRequestRequestTypeDef = {  # (1)
    "apiId": ...,
    "id": ...,
}

parent.update_api_key(**kwargs)
```

1. See [:material-code-braces: UpdateApiKeyRequestRequestTypeDef](./type_defs.md#updateapikeyrequestrequesttypedef) 

### update\_data\_source

Updates a `DataSource` object.

Type annotations and code completion for `#!python session.create_client("appsync").update_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.update_data_source)

```python
# update_data_source method definition

await def update_data_source(
    self,
    *,
    apiId: str,
    name: str,
    type: DataSourceTypeType,  # (1)
    description: str = ...,
    serviceRoleArn: str = ...,
    dynamodbConfig: DynamodbDataSourceConfigTypeDef = ...,  # (2)
    lambdaConfig: LambdaDataSourceConfigTypeDef = ...,  # (3)
    elasticsearchConfig: ElasticsearchDataSourceConfigTypeDef = ...,  # (4)
    openSearchServiceConfig: OpenSearchServiceDataSourceConfigTypeDef = ...,  # (5)
    httpConfig: HttpDataSourceConfigTypeDef = ...,  # (6)
    relationalDatabaseConfig: RelationalDatabaseDataSourceConfigTypeDef = ...,  # (7)
    eventBridgeConfig: EventBridgeDataSourceConfigTypeDef = ...,  # (8)
) -> UpdateDataSourceResponseTypeDef:  # (9)
    ...
```

1. See [:material-code-brackets: DataSourceTypeType](./literals.md#datasourcetypetype) 
2. See [:material-code-braces: DynamodbDataSourceConfigTypeDef](./type_defs.md#dynamodbdatasourceconfigtypedef) 
3. See [:material-code-braces: LambdaDataSourceConfigTypeDef](./type_defs.md#lambdadatasourceconfigtypedef) 
4. See [:material-code-braces: ElasticsearchDataSourceConfigTypeDef](./type_defs.md#elasticsearchdatasourceconfigtypedef) 
5. See [:material-code-braces: OpenSearchServiceDataSourceConfigTypeDef](./type_defs.md#opensearchservicedatasourceconfigtypedef) 
6. See [:material-code-braces: HttpDataSourceConfigTypeDef](./type_defs.md#httpdatasourceconfigtypedef) 
7. See [:material-code-braces: RelationalDatabaseDataSourceConfigTypeDef](./type_defs.md#relationaldatabasedatasourceconfigtypedef) 
8. See [:material-code-braces: EventBridgeDataSourceConfigTypeDef](./type_defs.md#eventbridgedatasourceconfigtypedef) 
9. See [:material-code-braces: UpdateDataSourceResponseTypeDef](./type_defs.md#updatedatasourceresponsetypedef) 


```python
# update_data_source method usage example with argument unpacking

kwargs: UpdateDataSourceRequestRequestTypeDef = {  # (1)
    "apiId": ...,
    "name": ...,
    "type": ...,
}

parent.update_data_source(**kwargs)
```

1. See [:material-code-braces: UpdateDataSourceRequestRequestTypeDef](./type_defs.md#updatedatasourcerequestrequesttypedef) 

### update\_domain\_name

Updates a custom `DomainName` object.

Type annotations and code completion for `#!python session.create_client("appsync").update_domain_name` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.update_domain_name)

```python
# update_domain_name method definition

await def update_domain_name(
    self,
    *,
    domainName: str,
    description: str = ...,
) -> UpdateDomainNameResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateDomainNameResponseTypeDef](./type_defs.md#updatedomainnameresponsetypedef) 


```python
# update_domain_name method usage example with argument unpacking

kwargs: UpdateDomainNameRequestRequestTypeDef = {  # (1)
    "domainName": ...,
}

parent.update_domain_name(**kwargs)
```

1. See [:material-code-braces: UpdateDomainNameRequestRequestTypeDef](./type_defs.md#updatedomainnamerequestrequesttypedef) 

### update\_function

Updates a `Function` object.

Type annotations and code completion for `#!python session.create_client("appsync").update_function` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.update_function)

```python
# update_function method definition

await def update_function(
    self,
    *,
    apiId: str,
    name: str,
    functionId: str,
    dataSourceName: str,
    description: str = ...,
    requestMappingTemplate: str = ...,
    responseMappingTemplate: str = ...,
    functionVersion: str = ...,
    syncConfig: SyncConfigTypeDef = ...,  # (1)
    maxBatchSize: int = ...,
    runtime: AppSyncRuntimeTypeDef = ...,  # (2)
    code: str = ...,
) -> UpdateFunctionResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SyncConfigTypeDef](./type_defs.md#syncconfigtypedef) 
2. See [:material-code-braces: AppSyncRuntimeTypeDef](./type_defs.md#appsyncruntimetypedef) 
3. See [:material-code-braces: UpdateFunctionResponseTypeDef](./type_defs.md#updatefunctionresponsetypedef) 


```python
# update_function method usage example with argument unpacking

kwargs: UpdateFunctionRequestRequestTypeDef = {  # (1)
    "apiId": ...,
    "name": ...,
    "functionId": ...,
    "dataSourceName": ...,
}

parent.update_function(**kwargs)
```

1. See [:material-code-braces: UpdateFunctionRequestRequestTypeDef](./type_defs.md#updatefunctionrequestrequesttypedef) 

### update\_graphql\_api

Updates a `GraphqlApi` object.

Type annotations and code completion for `#!python session.create_client("appsync").update_graphql_api` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.update_graphql_api)

```python
# update_graphql_api method definition

await def update_graphql_api(
    self,
    *,
    apiId: str,
    name: str,
    logConfig: LogConfigTypeDef = ...,  # (1)
    authenticationType: AuthenticationTypeType = ...,  # (2)
    userPoolConfig: UserPoolConfigTypeDef = ...,  # (3)
    openIDConnectConfig: OpenIDConnectConfigTypeDef = ...,  # (4)
    additionalAuthenticationProviders: Sequence[AdditionalAuthenticationProviderTypeDef] = ...,  # (5)
    xrayEnabled: bool = ...,
    lambdaAuthorizerConfig: LambdaAuthorizerConfigTypeDef = ...,  # (6)
    mergedApiExecutionRoleArn: str = ...,
    ownerContact: str = ...,
) -> UpdateGraphqlApiResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: LogConfigTypeDef](./type_defs.md#logconfigtypedef) 
2. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
3. See [:material-code-braces: UserPoolConfigTypeDef](./type_defs.md#userpoolconfigtypedef) 
4. See [:material-code-braces: OpenIDConnectConfigTypeDef](./type_defs.md#openidconnectconfigtypedef) 
5. See [:material-code-braces: AdditionalAuthenticationProviderTypeDef](./type_defs.md#additionalauthenticationprovidertypedef) 
6. See [:material-code-braces: LambdaAuthorizerConfigTypeDef](./type_defs.md#lambdaauthorizerconfigtypedef) 
7. See [:material-code-braces: UpdateGraphqlApiResponseTypeDef](./type_defs.md#updategraphqlapiresponsetypedef) 


```python
# update_graphql_api method usage example with argument unpacking

kwargs: UpdateGraphqlApiRequestRequestTypeDef = {  # (1)
    "apiId": ...,
    "name": ...,
}

parent.update_graphql_api(**kwargs)
```

1. See [:material-code-braces: UpdateGraphqlApiRequestRequestTypeDef](./type_defs.md#updategraphqlapirequestrequesttypedef) 

### update\_resolver

Updates a `Resolver` object.

Type annotations and code completion for `#!python session.create_client("appsync").update_resolver` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.update_resolver)

```python
# update_resolver method definition

await def update_resolver(
    self,
    *,
    apiId: str,
    typeName: str,
    fieldName: str,
    dataSourceName: str = ...,
    requestMappingTemplate: str = ...,
    responseMappingTemplate: str = ...,
    kind: ResolverKindType = ...,  # (1)
    pipelineConfig: PipelineConfigTypeDef = ...,  # (2)
    syncConfig: SyncConfigTypeDef = ...,  # (3)
    cachingConfig: CachingConfigTypeDef = ...,  # (4)
    maxBatchSize: int = ...,
    runtime: AppSyncRuntimeTypeDef = ...,  # (5)
    code: str = ...,
) -> UpdateResolverResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: ResolverKindType](./literals.md#resolverkindtype) 
2. See [:material-code-braces: PipelineConfigTypeDef](./type_defs.md#pipelineconfigtypedef) 
3. See [:material-code-braces: SyncConfigTypeDef](./type_defs.md#syncconfigtypedef) 
4. See [:material-code-braces: CachingConfigTypeDef](./type_defs.md#cachingconfigtypedef) 
5. See [:material-code-braces: AppSyncRuntimeTypeDef](./type_defs.md#appsyncruntimetypedef) 
6. See [:material-code-braces: UpdateResolverResponseTypeDef](./type_defs.md#updateresolverresponsetypedef) 


```python
# update_resolver method usage example with argument unpacking

kwargs: UpdateResolverRequestRequestTypeDef = {  # (1)
    "apiId": ...,
    "typeName": ...,
    "fieldName": ...,
}

parent.update_resolver(**kwargs)
```

1. See [:material-code-braces: UpdateResolverRequestRequestTypeDef](./type_defs.md#updateresolverrequestrequesttypedef) 

### update\_source\_api\_association

Updates some of the configuration choices of a particular source API
association.

Type annotations and code completion for `#!python session.create_client("appsync").update_source_api_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.update_source_api_association)

```python
# update_source_api_association method definition

await def update_source_api_association(
    self,
    *,
    associationId: str,
    mergedApiIdentifier: str,
    description: str = ...,
    sourceApiAssociationConfig: SourceApiAssociationConfigTypeDef = ...,  # (1)
) -> UpdateSourceApiAssociationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SourceApiAssociationConfigTypeDef](./type_defs.md#sourceapiassociationconfigtypedef) 
2. See [:material-code-braces: UpdateSourceApiAssociationResponseTypeDef](./type_defs.md#updatesourceapiassociationresponsetypedef) 


```python
# update_source_api_association method usage example with argument unpacking

kwargs: UpdateSourceApiAssociationRequestRequestTypeDef = {  # (1)
    "associationId": ...,
    "mergedApiIdentifier": ...,
}

parent.update_source_api_association(**kwargs)
```

1. See [:material-code-braces: UpdateSourceApiAssociationRequestRequestTypeDef](./type_defs.md#updatesourceapiassociationrequestrequesttypedef) 

### update\_type

Updates a `Type` object.

Type annotations and code completion for `#!python session.create_client("appsync").update_type` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.update_type)

```python
# update_type method definition

await def update_type(
    self,
    *,
    apiId: str,
    typeName: str,
    format: TypeDefinitionFormatType,  # (1)
    definition: str = ...,
) -> UpdateTypeResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TypeDefinitionFormatType](./literals.md#typedefinitionformattype) 
2. See [:material-code-braces: UpdateTypeResponseTypeDef](./type_defs.md#updatetyperesponsetypedef) 


```python
# update_type method usage example with argument unpacking

kwargs: UpdateTypeRequestRequestTypeDef = {  # (1)
    "apiId": ...,
    "typeName": ...,
    "format": ...,
}

parent.update_type(**kwargs)
```

1. See [:material-code-braces: UpdateTypeRequestRequestTypeDef](./type_defs.md#updatetyperequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("appsync").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> AppSyncClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("appsync").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("appsync").get_paginator` method with overloads.

- `client.get_paginator("list_api_keys")` -> [ListApiKeysPaginator](./paginators.md#listapikeyspaginator)
- `client.get_paginator("list_data_sources")` -> [ListDataSourcesPaginator](./paginators.md#listdatasourcespaginator)
- `client.get_paginator("list_functions")` -> [ListFunctionsPaginator](./paginators.md#listfunctionspaginator)
- `client.get_paginator("list_graphql_apis")` -> [ListGraphqlApisPaginator](./paginators.md#listgraphqlapispaginator)
- `client.get_paginator("list_resolvers")` -> [ListResolversPaginator](./paginators.md#listresolverspaginator)
- `client.get_paginator("list_resolvers_by_function")` -> [ListResolversByFunctionPaginator](./paginators.md#listresolversbyfunctionpaginator)
- `client.get_paginator("list_types")` -> [ListTypesPaginator](./paginators.md#listtypespaginator)



