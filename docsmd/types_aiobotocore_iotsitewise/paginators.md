# Paginators

> [Index](../README.md) > [IoTSiteWise](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [IoTSiteWise](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#iotsitewise)
    type annotations stubs module [types-aiobotocore-iotsitewise](https://pypi.org/project/types-aiobotocore-iotsitewise/).

## ExecuteQueryPaginator

Type annotations and code completion for `#!python session.create_client("iotsitewise").get_paginator("execute_query")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/paginator/ExecuteQuery.html#IoTSiteWise.Paginator.ExecuteQuery)

```python
# ExecuteQueryPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import ExecuteQueryPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:  # (1)
    paginator: ExecuteQueryPaginator = client.get_paginator("execute_query")  # (2)
    async for item in paginator.paginate(...):
        item: ExecuteQueryResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [IoTSiteWiseClient](./client.md)
2. paginator: [ExecuteQueryPaginator](./paginators.md#executequerypaginator)
3. item: [:material-code-braces: ExecuteQueryResponsePaginatorTypeDef](./type_defs.md#executequeryresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python ExecuteQueryPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    queryStatement: str,
    clientToken: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ExecuteQueryResponsePaginatorTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ExecuteQueryResponsePaginatorTypeDef](./type_defs.md#executequeryresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ExecuteQueryRequestPaginateTypeDef = {  # (1)
    "queryStatement": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ExecuteQueryRequestPaginateTypeDef](./type_defs.md#executequeryrequestpaginatetypedef) 
## GetAssetPropertyAggregatesPaginator

Type annotations and code completion for `#!python session.create_client("iotsitewise").get_paginator("get_asset_property_aggregates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/paginator/GetAssetPropertyAggregates.html#IoTSiteWise.Paginator.GetAssetPropertyAggregates)

```python
# GetAssetPropertyAggregatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import GetAssetPropertyAggregatesPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:  # (1)
    paginator: GetAssetPropertyAggregatesPaginator = client.get_paginator("get_asset_property_aggregates")  # (2)
    async for item in paginator.paginate(...):
        item: GetAssetPropertyAggregatesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTSiteWiseClient](./client.md)
2. paginator: [GetAssetPropertyAggregatesPaginator](./paginators.md#getassetpropertyaggregatespaginator)
3. item: [:material-code-braces: GetAssetPropertyAggregatesResponseTypeDef](./type_defs.md#getassetpropertyaggregatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetAssetPropertyAggregatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    aggregateTypes: Sequence[AggregateTypeType],  # (1)
    resolution: str,
    startDate: TimestampTypeDef,
    endDate: TimestampTypeDef,
    assetId: str = ...,
    propertyId: str = ...,
    propertyAlias: str = ...,
    qualities: Sequence[QualityType] = ...,  # (2)
    timeOrdering: TimeOrderingType = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AioPageIterator[GetAssetPropertyAggregatesResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: AggregateTypeType](./literals.md#aggregatetypetype) 
2. See [:material-code-brackets: QualityType](./literals.md#qualitytype) 
3. See [:material-code-brackets: TimeOrderingType](./literals.md#timeorderingtype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: GetAssetPropertyAggregatesResponseTypeDef](./type_defs.md#getassetpropertyaggregatesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetAssetPropertyAggregatesRequestPaginateTypeDef = {  # (1)
    "aggregateTypes": ...,
    "resolution": ...,
    "startDate": ...,
    "endDate": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetAssetPropertyAggregatesRequestPaginateTypeDef](./type_defs.md#getassetpropertyaggregatesrequestpaginatetypedef) 
## GetAssetPropertyValueHistoryPaginator

Type annotations and code completion for `#!python session.create_client("iotsitewise").get_paginator("get_asset_property_value_history")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/paginator/GetAssetPropertyValueHistory.html#IoTSiteWise.Paginator.GetAssetPropertyValueHistory)

```python
# GetAssetPropertyValueHistoryPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import GetAssetPropertyValueHistoryPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:  # (1)
    paginator: GetAssetPropertyValueHistoryPaginator = client.get_paginator("get_asset_property_value_history")  # (2)
    async for item in paginator.paginate(...):
        item: GetAssetPropertyValueHistoryResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTSiteWiseClient](./client.md)
2. paginator: [GetAssetPropertyValueHistoryPaginator](./paginators.md#getassetpropertyvaluehistorypaginator)
3. item: [:material-code-braces: GetAssetPropertyValueHistoryResponseTypeDef](./type_defs.md#getassetpropertyvaluehistoryresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetAssetPropertyValueHistoryPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    assetId: str = ...,
    propertyId: str = ...,
    propertyAlias: str = ...,
    startDate: TimestampTypeDef = ...,
    endDate: TimestampTypeDef = ...,
    qualities: Sequence[QualityType] = ...,  # (1)
    timeOrdering: TimeOrderingType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[GetAssetPropertyValueHistoryResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: QualityType](./literals.md#qualitytype) 
2. See [:material-code-brackets: TimeOrderingType](./literals.md#timeorderingtype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: GetAssetPropertyValueHistoryResponseTypeDef](./type_defs.md#getassetpropertyvaluehistoryresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetAssetPropertyValueHistoryRequestPaginateTypeDef = {  # (1)
    "assetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetAssetPropertyValueHistoryRequestPaginateTypeDef](./type_defs.md#getassetpropertyvaluehistoryrequestpaginatetypedef) 
## GetInterpolatedAssetPropertyValuesPaginator

Type annotations and code completion for `#!python session.create_client("iotsitewise").get_paginator("get_interpolated_asset_property_values")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/paginator/GetInterpolatedAssetPropertyValues.html#IoTSiteWise.Paginator.GetInterpolatedAssetPropertyValues)

```python
# GetInterpolatedAssetPropertyValuesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import GetInterpolatedAssetPropertyValuesPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:  # (1)
    paginator: GetInterpolatedAssetPropertyValuesPaginator = client.get_paginator("get_interpolated_asset_property_values")  # (2)
    async for item in paginator.paginate(...):
        item: GetInterpolatedAssetPropertyValuesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTSiteWiseClient](./client.md)
2. paginator: [GetInterpolatedAssetPropertyValuesPaginator](./paginators.md#getinterpolatedassetpropertyvaluespaginator)
3. item: [:material-code-braces: GetInterpolatedAssetPropertyValuesResponseTypeDef](./type_defs.md#getinterpolatedassetpropertyvaluesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetInterpolatedAssetPropertyValuesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    startTimeInSeconds: int,
    endTimeInSeconds: int,
    quality: QualityType,  # (1)
    intervalInSeconds: int,
    type: str,
    assetId: str = ...,
    propertyId: str = ...,
    propertyAlias: str = ...,
    startTimeOffsetInNanos: int = ...,
    endTimeOffsetInNanos: int = ...,
    intervalWindowInSeconds: int = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[GetInterpolatedAssetPropertyValuesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: QualityType](./literals.md#qualitytype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetInterpolatedAssetPropertyValuesResponseTypeDef](./type_defs.md#getinterpolatedassetpropertyvaluesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetInterpolatedAssetPropertyValuesRequestPaginateTypeDef = {  # (1)
    "startTimeInSeconds": ...,
    "endTimeInSeconds": ...,
    "quality": ...,
    "intervalInSeconds": ...,
    "type": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetInterpolatedAssetPropertyValuesRequestPaginateTypeDef](./type_defs.md#getinterpolatedassetpropertyvaluesrequestpaginatetypedef) 
## ListAccessPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("iotsitewise").get_paginator("list_access_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/paginator/ListAccessPolicies.html#IoTSiteWise.Paginator.ListAccessPolicies)

```python
# ListAccessPoliciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import ListAccessPoliciesPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:  # (1)
    paginator: ListAccessPoliciesPaginator = client.get_paginator("list_access_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccessPoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTSiteWiseClient](./client.md)
2. paginator: [ListAccessPoliciesPaginator](./paginators.md#listaccesspoliciespaginator)
3. item: [:material-code-braces: ListAccessPoliciesResponseTypeDef](./type_defs.md#listaccesspoliciesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAccessPoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    identityType: IdentityTypeType = ...,  # (1)
    identityId: str = ...,
    resourceType: ResourceTypeType = ...,  # (2)
    resourceId: str = ...,
    iamArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListAccessPoliciesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListAccessPoliciesResponseTypeDef](./type_defs.md#listaccesspoliciesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAccessPoliciesRequestPaginateTypeDef = {  # (1)
    "identityType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccessPoliciesRequestPaginateTypeDef](./type_defs.md#listaccesspoliciesrequestpaginatetypedef) 
## ListActionsPaginator

Type annotations and code completion for `#!python session.create_client("iotsitewise").get_paginator("list_actions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/paginator/ListActions.html#IoTSiteWise.Paginator.ListActions)

```python
# ListActionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import ListActionsPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:  # (1)
    paginator: ListActionsPaginator = client.get_paginator("list_actions")  # (2)
    async for item in paginator.paginate(...):
        item: ListActionsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTSiteWiseClient](./client.md)
2. paginator: [ListActionsPaginator](./paginators.md#listactionspaginator)
3. item: [:material-code-braces: ListActionsResponseTypeDef](./type_defs.md#listactionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListActionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    targetResourceType: TargetResourceTypeType,  # (1)
    targetResourceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListActionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: TargetResourceTypeType](./literals.md#targetresourcetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListActionsResponseTypeDef](./type_defs.md#listactionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListActionsRequestPaginateTypeDef = {  # (1)
    "targetResourceType": ...,
    "targetResourceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListActionsRequestPaginateTypeDef](./type_defs.md#listactionsrequestpaginatetypedef) 
## ListAssetModelCompositeModelsPaginator

Type annotations and code completion for `#!python session.create_client("iotsitewise").get_paginator("list_asset_model_composite_models")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/paginator/ListAssetModelCompositeModels.html#IoTSiteWise.Paginator.ListAssetModelCompositeModels)

```python
# ListAssetModelCompositeModelsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import ListAssetModelCompositeModelsPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:  # (1)
    paginator: ListAssetModelCompositeModelsPaginator = client.get_paginator("list_asset_model_composite_models")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssetModelCompositeModelsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTSiteWiseClient](./client.md)
2. paginator: [ListAssetModelCompositeModelsPaginator](./paginators.md#listassetmodelcompositemodelspaginator)
3. item: [:material-code-braces: ListAssetModelCompositeModelsResponseTypeDef](./type_defs.md#listassetmodelcompositemodelsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAssetModelCompositeModelsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    assetModelId: str,
    assetModelVersion: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAssetModelCompositeModelsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAssetModelCompositeModelsResponseTypeDef](./type_defs.md#listassetmodelcompositemodelsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAssetModelCompositeModelsRequestPaginateTypeDef = {  # (1)
    "assetModelId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssetModelCompositeModelsRequestPaginateTypeDef](./type_defs.md#listassetmodelcompositemodelsrequestpaginatetypedef) 
## ListAssetModelPropertiesPaginator

Type annotations and code completion for `#!python session.create_client("iotsitewise").get_paginator("list_asset_model_properties")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/paginator/ListAssetModelProperties.html#IoTSiteWise.Paginator.ListAssetModelProperties)

```python
# ListAssetModelPropertiesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import ListAssetModelPropertiesPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:  # (1)
    paginator: ListAssetModelPropertiesPaginator = client.get_paginator("list_asset_model_properties")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssetModelPropertiesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTSiteWiseClient](./client.md)
2. paginator: [ListAssetModelPropertiesPaginator](./paginators.md#listassetmodelpropertiespaginator)
3. item: [:material-code-braces: ListAssetModelPropertiesResponseTypeDef](./type_defs.md#listassetmodelpropertiesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAssetModelPropertiesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    assetModelId: str,
    filter: ListAssetModelPropertiesFilterType = ...,  # (1)
    assetModelVersion: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListAssetModelPropertiesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ListAssetModelPropertiesFilterType](./literals.md#listassetmodelpropertiesfiltertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAssetModelPropertiesResponseTypeDef](./type_defs.md#listassetmodelpropertiesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAssetModelPropertiesRequestPaginateTypeDef = {  # (1)
    "assetModelId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssetModelPropertiesRequestPaginateTypeDef](./type_defs.md#listassetmodelpropertiesrequestpaginatetypedef) 
## ListAssetModelsPaginator

Type annotations and code completion for `#!python session.create_client("iotsitewise").get_paginator("list_asset_models")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/paginator/ListAssetModels.html#IoTSiteWise.Paginator.ListAssetModels)

```python
# ListAssetModelsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import ListAssetModelsPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:  # (1)
    paginator: ListAssetModelsPaginator = client.get_paginator("list_asset_models")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssetModelsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTSiteWiseClient](./client.md)
2. paginator: [ListAssetModelsPaginator](./paginators.md#listassetmodelspaginator)
3. item: [:material-code-braces: ListAssetModelsResponseTypeDef](./type_defs.md#listassetmodelsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAssetModelsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    assetModelTypes: Sequence[AssetModelTypeType] = ...,  # (1)
    assetModelVersion: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListAssetModelsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: AssetModelTypeType](./literals.md#assetmodeltypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAssetModelsResponseTypeDef](./type_defs.md#listassetmodelsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAssetModelsRequestPaginateTypeDef = {  # (1)
    "assetModelTypes": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssetModelsRequestPaginateTypeDef](./type_defs.md#listassetmodelsrequestpaginatetypedef) 
## ListAssetPropertiesPaginator

Type annotations and code completion for `#!python session.create_client("iotsitewise").get_paginator("list_asset_properties")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/paginator/ListAssetProperties.html#IoTSiteWise.Paginator.ListAssetProperties)

```python
# ListAssetPropertiesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import ListAssetPropertiesPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:  # (1)
    paginator: ListAssetPropertiesPaginator = client.get_paginator("list_asset_properties")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssetPropertiesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTSiteWiseClient](./client.md)
2. paginator: [ListAssetPropertiesPaginator](./paginators.md#listassetpropertiespaginator)
3. item: [:material-code-braces: ListAssetPropertiesResponseTypeDef](./type_defs.md#listassetpropertiesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAssetPropertiesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    assetId: str,
    filter: ListAssetPropertiesFilterType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListAssetPropertiesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ListAssetPropertiesFilterType](./literals.md#listassetpropertiesfiltertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAssetPropertiesResponseTypeDef](./type_defs.md#listassetpropertiesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAssetPropertiesRequestPaginateTypeDef = {  # (1)
    "assetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssetPropertiesRequestPaginateTypeDef](./type_defs.md#listassetpropertiesrequestpaginatetypedef) 
## ListAssetRelationshipsPaginator

Type annotations and code completion for `#!python session.create_client("iotsitewise").get_paginator("list_asset_relationships")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/paginator/ListAssetRelationships.html#IoTSiteWise.Paginator.ListAssetRelationships)

```python
# ListAssetRelationshipsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import ListAssetRelationshipsPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:  # (1)
    paginator: ListAssetRelationshipsPaginator = client.get_paginator("list_asset_relationships")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssetRelationshipsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTSiteWiseClient](./client.md)
2. paginator: [ListAssetRelationshipsPaginator](./paginators.md#listassetrelationshipspaginator)
3. item: [:material-code-braces: ListAssetRelationshipsResponseTypeDef](./type_defs.md#listassetrelationshipsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAssetRelationshipsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    assetId: str,
    traversalType: TraversalTypeType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListAssetRelationshipsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: TraversalTypeType](./literals.md#traversaltypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAssetRelationshipsResponseTypeDef](./type_defs.md#listassetrelationshipsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAssetRelationshipsRequestPaginateTypeDef = {  # (1)
    "assetId": ...,
    "traversalType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssetRelationshipsRequestPaginateTypeDef](./type_defs.md#listassetrelationshipsrequestpaginatetypedef) 
## ListAssetsPaginator

Type annotations and code completion for `#!python session.create_client("iotsitewise").get_paginator("list_assets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/paginator/ListAssets.html#IoTSiteWise.Paginator.ListAssets)

```python
# ListAssetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import ListAssetsPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:  # (1)
    paginator: ListAssetsPaginator = client.get_paginator("list_assets")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssetsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTSiteWiseClient](./client.md)
2. paginator: [ListAssetsPaginator](./paginators.md#listassetspaginator)
3. item: [:material-code-braces: ListAssetsResponseTypeDef](./type_defs.md#listassetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAssetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    assetModelId: str = ...,
    filter: ListAssetsFilterType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListAssetsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ListAssetsFilterType](./literals.md#listassetsfiltertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAssetsResponseTypeDef](./type_defs.md#listassetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAssetsRequestPaginateTypeDef = {  # (1)
    "assetModelId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssetsRequestPaginateTypeDef](./type_defs.md#listassetsrequestpaginatetypedef) 
## ListAssociatedAssetsPaginator

Type annotations and code completion for `#!python session.create_client("iotsitewise").get_paginator("list_associated_assets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/paginator/ListAssociatedAssets.html#IoTSiteWise.Paginator.ListAssociatedAssets)

```python
# ListAssociatedAssetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import ListAssociatedAssetsPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:  # (1)
    paginator: ListAssociatedAssetsPaginator = client.get_paginator("list_associated_assets")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssociatedAssetsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTSiteWiseClient](./client.md)
2. paginator: [ListAssociatedAssetsPaginator](./paginators.md#listassociatedassetspaginator)
3. item: [:material-code-braces: ListAssociatedAssetsResponseTypeDef](./type_defs.md#listassociatedassetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAssociatedAssetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    assetId: str,
    hierarchyId: str = ...,
    traversalDirection: TraversalDirectionType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListAssociatedAssetsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: TraversalDirectionType](./literals.md#traversaldirectiontype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAssociatedAssetsResponseTypeDef](./type_defs.md#listassociatedassetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAssociatedAssetsRequestPaginateTypeDef = {  # (1)
    "assetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssociatedAssetsRequestPaginateTypeDef](./type_defs.md#listassociatedassetsrequestpaginatetypedef) 
## ListBulkImportJobsPaginator

Type annotations and code completion for `#!python session.create_client("iotsitewise").get_paginator("list_bulk_import_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/paginator/ListBulkImportJobs.html#IoTSiteWise.Paginator.ListBulkImportJobs)

```python
# ListBulkImportJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import ListBulkImportJobsPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:  # (1)
    paginator: ListBulkImportJobsPaginator = client.get_paginator("list_bulk_import_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListBulkImportJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTSiteWiseClient](./client.md)
2. paginator: [ListBulkImportJobsPaginator](./paginators.md#listbulkimportjobspaginator)
3. item: [:material-code-braces: ListBulkImportJobsResponseTypeDef](./type_defs.md#listbulkimportjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListBulkImportJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filter: ListBulkImportJobsFilterType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListBulkImportJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ListBulkImportJobsFilterType](./literals.md#listbulkimportjobsfiltertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListBulkImportJobsResponseTypeDef](./type_defs.md#listbulkimportjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListBulkImportJobsRequestPaginateTypeDef = {  # (1)
    "filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBulkImportJobsRequestPaginateTypeDef](./type_defs.md#listbulkimportjobsrequestpaginatetypedef) 
## ListCompositionRelationshipsPaginator

Type annotations and code completion for `#!python session.create_client("iotsitewise").get_paginator("list_composition_relationships")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/paginator/ListCompositionRelationships.html#IoTSiteWise.Paginator.ListCompositionRelationships)

```python
# ListCompositionRelationshipsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import ListCompositionRelationshipsPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:  # (1)
    paginator: ListCompositionRelationshipsPaginator = client.get_paginator("list_composition_relationships")  # (2)
    async for item in paginator.paginate(...):
        item: ListCompositionRelationshipsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTSiteWiseClient](./client.md)
2. paginator: [ListCompositionRelationshipsPaginator](./paginators.md#listcompositionrelationshipspaginator)
3. item: [:material-code-braces: ListCompositionRelationshipsResponseTypeDef](./type_defs.md#listcompositionrelationshipsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCompositionRelationshipsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    assetModelId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListCompositionRelationshipsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCompositionRelationshipsResponseTypeDef](./type_defs.md#listcompositionrelationshipsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCompositionRelationshipsRequestPaginateTypeDef = {  # (1)
    "assetModelId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCompositionRelationshipsRequestPaginateTypeDef](./type_defs.md#listcompositionrelationshipsrequestpaginatetypedef) 
## ListDashboardsPaginator

Type annotations and code completion for `#!python session.create_client("iotsitewise").get_paginator("list_dashboards")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/paginator/ListDashboards.html#IoTSiteWise.Paginator.ListDashboards)

```python
# ListDashboardsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import ListDashboardsPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:  # (1)
    paginator: ListDashboardsPaginator = client.get_paginator("list_dashboards")  # (2)
    async for item in paginator.paginate(...):
        item: ListDashboardsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTSiteWiseClient](./client.md)
2. paginator: [ListDashboardsPaginator](./paginators.md#listdashboardspaginator)
3. item: [:material-code-braces: ListDashboardsResponseTypeDef](./type_defs.md#listdashboardsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDashboardsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    projectId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDashboardsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDashboardsResponseTypeDef](./type_defs.md#listdashboardsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDashboardsRequestPaginateTypeDef = {  # (1)
    "projectId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDashboardsRequestPaginateTypeDef](./type_defs.md#listdashboardsrequestpaginatetypedef) 
## ListDatasetsPaginator

Type annotations and code completion for `#!python session.create_client("iotsitewise").get_paginator("list_datasets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/paginator/ListDatasets.html#IoTSiteWise.Paginator.ListDatasets)

```python
# ListDatasetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import ListDatasetsPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:  # (1)
    paginator: ListDatasetsPaginator = client.get_paginator("list_datasets")  # (2)
    async for item in paginator.paginate(...):
        item: ListDatasetsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTSiteWiseClient](./client.md)
2. paginator: [ListDatasetsPaginator](./paginators.md#listdatasetspaginator)
3. item: [:material-code-braces: ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDatasetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    sourceType: DatasetSourceTypeType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListDatasetsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: DatasetSourceTypeType](./literals.md#datasetsourcetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDatasetsRequestPaginateTypeDef = {  # (1)
    "sourceType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatasetsRequestPaginateTypeDef](./type_defs.md#listdatasetsrequestpaginatetypedef) 
## ListGatewaysPaginator

Type annotations and code completion for `#!python session.create_client("iotsitewise").get_paginator("list_gateways")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/paginator/ListGateways.html#IoTSiteWise.Paginator.ListGateways)

```python
# ListGatewaysPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import ListGatewaysPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:  # (1)
    paginator: ListGatewaysPaginator = client.get_paginator("list_gateways")  # (2)
    async for item in paginator.paginate(...):
        item: ListGatewaysResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTSiteWiseClient](./client.md)
2. paginator: [ListGatewaysPaginator](./paginators.md#listgatewayspaginator)
3. item: [:material-code-braces: ListGatewaysResponseTypeDef](./type_defs.md#listgatewaysresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListGatewaysPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListGatewaysResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGatewaysResponseTypeDef](./type_defs.md#listgatewaysresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListGatewaysRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGatewaysRequestPaginateTypeDef](./type_defs.md#listgatewaysrequestpaginatetypedef) 
## ListPortalsPaginator

Type annotations and code completion for `#!python session.create_client("iotsitewise").get_paginator("list_portals")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/paginator/ListPortals.html#IoTSiteWise.Paginator.ListPortals)

```python
# ListPortalsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import ListPortalsPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:  # (1)
    paginator: ListPortalsPaginator = client.get_paginator("list_portals")  # (2)
    async for item in paginator.paginate(...):
        item: ListPortalsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTSiteWiseClient](./client.md)
2. paginator: [ListPortalsPaginator](./paginators.md#listportalspaginator)
3. item: [:material-code-braces: ListPortalsResponseTypeDef](./type_defs.md#listportalsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPortalsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListPortalsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPortalsResponseTypeDef](./type_defs.md#listportalsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPortalsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPortalsRequestPaginateTypeDef](./type_defs.md#listportalsrequestpaginatetypedef) 
## ListProjectAssetsPaginator

Type annotations and code completion for `#!python session.create_client("iotsitewise").get_paginator("list_project_assets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/paginator/ListProjectAssets.html#IoTSiteWise.Paginator.ListProjectAssets)

```python
# ListProjectAssetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import ListProjectAssetsPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:  # (1)
    paginator: ListProjectAssetsPaginator = client.get_paginator("list_project_assets")  # (2)
    async for item in paginator.paginate(...):
        item: ListProjectAssetsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTSiteWiseClient](./client.md)
2. paginator: [ListProjectAssetsPaginator](./paginators.md#listprojectassetspaginator)
3. item: [:material-code-braces: ListProjectAssetsResponseTypeDef](./type_defs.md#listprojectassetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListProjectAssetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    projectId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListProjectAssetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListProjectAssetsResponseTypeDef](./type_defs.md#listprojectassetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListProjectAssetsRequestPaginateTypeDef = {  # (1)
    "projectId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProjectAssetsRequestPaginateTypeDef](./type_defs.md#listprojectassetsrequestpaginatetypedef) 
## ListProjectsPaginator

Type annotations and code completion for `#!python session.create_client("iotsitewise").get_paginator("list_projects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/paginator/ListProjects.html#IoTSiteWise.Paginator.ListProjects)

```python
# ListProjectsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import ListProjectsPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:  # (1)
    paginator: ListProjectsPaginator = client.get_paginator("list_projects")  # (2)
    async for item in paginator.paginate(...):
        item: ListProjectsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTSiteWiseClient](./client.md)
2. paginator: [ListProjectsPaginator](./paginators.md#listprojectspaginator)
3. item: [:material-code-braces: ListProjectsResponseTypeDef](./type_defs.md#listprojectsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListProjectsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    portalId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListProjectsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListProjectsResponseTypeDef](./type_defs.md#listprojectsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListProjectsRequestPaginateTypeDef = {  # (1)
    "portalId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProjectsRequestPaginateTypeDef](./type_defs.md#listprojectsrequestpaginatetypedef) 
## ListTimeSeriesPaginator

Type annotations and code completion for `#!python session.create_client("iotsitewise").get_paginator("list_time_series")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise/paginator/ListTimeSeries.html#IoTSiteWise.Paginator.ListTimeSeries)

```python
# ListTimeSeriesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotsitewise.paginator import ListTimeSeriesPaginator

session = get_session()
async with session.create_client("iotsitewise") as client:  # (1)
    paginator: ListTimeSeriesPaginator = client.get_paginator("list_time_series")  # (2)
    async for item in paginator.paginate(...):
        item: ListTimeSeriesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTSiteWiseClient](./client.md)
2. paginator: [ListTimeSeriesPaginator](./paginators.md#listtimeseriespaginator)
3. item: [:material-code-braces: ListTimeSeriesResponseTypeDef](./type_defs.md#listtimeseriesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTimeSeriesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    assetId: str = ...,
    aliasPrefix: str = ...,
    timeSeriesType: ListTimeSeriesTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListTimeSeriesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ListTimeSeriesTypeType](./literals.md#listtimeseriestypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListTimeSeriesResponseTypeDef](./type_defs.md#listtimeseriesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTimeSeriesRequestPaginateTypeDef = {  # (1)
    "assetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTimeSeriesRequestPaginateTypeDef](./type_defs.md#listtimeseriesrequestpaginatetypedef) 
