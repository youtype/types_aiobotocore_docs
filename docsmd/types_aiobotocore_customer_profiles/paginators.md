# Paginators

> [Index](../README.md) > [CustomerProfiles](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CustomerProfiles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#customerprofiles)
    type annotations stubs module [types-aiobotocore-customer-profiles](https://pypi.org/project/types-aiobotocore-customer-profiles/).

## GetSimilarProfilesPaginator

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_paginator("get_similar_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles/paginator/GetSimilarProfiles.html#CustomerProfiles.Paginator.GetSimilarProfiles)

```python
# GetSimilarProfilesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_customer_profiles.paginator import GetSimilarProfilesPaginator

session = get_session()
async with session.create_client("customer-profiles") as client:  # (1)
    paginator: GetSimilarProfilesPaginator = client.get_paginator("get_similar_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: GetSimilarProfilesResponseTypeDef
        print(item)  # (3)
```

1. client: [CustomerProfilesClient](./client.md)
2. paginator: [GetSimilarProfilesPaginator](./paginators.md#getsimilarprofilespaginator)
3. item: `AioPageIterator[GetSimilarProfilesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetSimilarProfilesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DomainName: str,
    MatchType: MatchTypeType,  # (1)
    SearchKey: str,
    SearchValue: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[GetSimilarProfilesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: MatchTypeType](./literals.md#matchtypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[GetSimilarProfilesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetSimilarProfilesRequestPaginateTypeDef = {  # (1)
    "DomainName": ...,
    "MatchType": ...,
    "SearchKey": ...,
    "SearchValue": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetSimilarProfilesRequestPaginateTypeDef](./type_defs.md#getsimilarprofilesrequestpaginatetypedef)
## ListDomainLayoutsPaginator

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_paginator("list_domain_layouts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles/paginator/ListDomainLayouts.html#CustomerProfiles.Paginator.ListDomainLayouts)

```python
# ListDomainLayoutsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_customer_profiles.paginator import ListDomainLayoutsPaginator

session = get_session()
async with session.create_client("customer-profiles") as client:  # (1)
    paginator: ListDomainLayoutsPaginator = client.get_paginator("list_domain_layouts")  # (2)
    async for item in paginator.paginate(...):
        item: ListDomainLayoutsResponseTypeDef
        print(item)  # (3)
```

1. client: [CustomerProfilesClient](./client.md)
2. paginator: [ListDomainLayoutsPaginator](./paginators.md#listdomainlayoutspaginator)
3. item: `AioPageIterator[ListDomainLayoutsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDomainLayoutsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DomainName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDomainLayoutsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDomainLayoutsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDomainLayoutsRequestPaginateTypeDef = {  # (1)
    "DomainName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDomainLayoutsRequestPaginateTypeDef](./type_defs.md#listdomainlayoutsrequestpaginatetypedef)
## ListDomainObjectTypesPaginator

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_paginator("list_domain_object_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles/paginator/ListDomainObjectTypes.html#CustomerProfiles.Paginator.ListDomainObjectTypes)

```python
# ListDomainObjectTypesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_customer_profiles.paginator import ListDomainObjectTypesPaginator

session = get_session()
async with session.create_client("customer-profiles") as client:  # (1)
    paginator: ListDomainObjectTypesPaginator = client.get_paginator("list_domain_object_types")  # (2)
    async for item in paginator.paginate(...):
        item: ListDomainObjectTypesResponseTypeDef
        print(item)  # (3)
```

1. client: [CustomerProfilesClient](./client.md)
2. paginator: [ListDomainObjectTypesPaginator](./paginators.md#listdomainobjecttypespaginator)
3. item: `AioPageIterator[ListDomainObjectTypesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDomainObjectTypesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DomainName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDomainObjectTypesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDomainObjectTypesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDomainObjectTypesRequestPaginateTypeDef = {  # (1)
    "DomainName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDomainObjectTypesRequestPaginateTypeDef](./type_defs.md#listdomainobjecttypesrequestpaginatetypedef)
## ListEventStreamsPaginator

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_paginator("list_event_streams")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles/paginator/ListEventStreams.html#CustomerProfiles.Paginator.ListEventStreams)

```python
# ListEventStreamsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_customer_profiles.paginator import ListEventStreamsPaginator

session = get_session()
async with session.create_client("customer-profiles") as client:  # (1)
    paginator: ListEventStreamsPaginator = client.get_paginator("list_event_streams")  # (2)
    async for item in paginator.paginate(...):
        item: ListEventStreamsResponseTypeDef
        print(item)  # (3)
```

1. client: [CustomerProfilesClient](./client.md)
2. paginator: [ListEventStreamsPaginator](./paginators.md#listeventstreamspaginator)
3. item: `AioPageIterator[ListEventStreamsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListEventStreamsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DomainName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListEventStreamsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListEventStreamsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListEventStreamsRequestPaginateTypeDef = {  # (1)
    "DomainName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEventStreamsRequestPaginateTypeDef](./type_defs.md#listeventstreamsrequestpaginatetypedef)
## ListEventTriggersPaginator

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_paginator("list_event_triggers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles/paginator/ListEventTriggers.html#CustomerProfiles.Paginator.ListEventTriggers)

```python
# ListEventTriggersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_customer_profiles.paginator import ListEventTriggersPaginator

session = get_session()
async with session.create_client("customer-profiles") as client:  # (1)
    paginator: ListEventTriggersPaginator = client.get_paginator("list_event_triggers")  # (2)
    async for item in paginator.paginate(...):
        item: ListEventTriggersResponseTypeDef
        print(item)  # (3)
```

1. client: [CustomerProfilesClient](./client.md)
2. paginator: [ListEventTriggersPaginator](./paginators.md#listeventtriggerspaginator)
3. item: `AioPageIterator[ListEventTriggersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListEventTriggersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DomainName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListEventTriggersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListEventTriggersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListEventTriggersRequestPaginateTypeDef = {  # (1)
    "DomainName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEventTriggersRequestPaginateTypeDef](./type_defs.md#listeventtriggersrequestpaginatetypedef)
## ListObjectTypeAttributesPaginator

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_paginator("list_object_type_attributes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles/paginator/ListObjectTypeAttributes.html#CustomerProfiles.Paginator.ListObjectTypeAttributes)

```python
# ListObjectTypeAttributesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_customer_profiles.paginator import ListObjectTypeAttributesPaginator

session = get_session()
async with session.create_client("customer-profiles") as client:  # (1)
    paginator: ListObjectTypeAttributesPaginator = client.get_paginator("list_object_type_attributes")  # (2)
    async for item in paginator.paginate(...):
        item: ListObjectTypeAttributesResponseTypeDef
        print(item)  # (3)
```

1. client: [CustomerProfilesClient](./client.md)
2. paginator: [ListObjectTypeAttributesPaginator](./paginators.md#listobjecttypeattributespaginator)
3. item: `AioPageIterator[ListObjectTypeAttributesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListObjectTypeAttributesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DomainName: str,
    ObjectTypeName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListObjectTypeAttributesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListObjectTypeAttributesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListObjectTypeAttributesRequestPaginateTypeDef = {  # (1)
    "DomainName": ...,
    "ObjectTypeName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListObjectTypeAttributesRequestPaginateTypeDef](./type_defs.md#listobjecttypeattributesrequestpaginatetypedef)
## ListRecommenderRecipesPaginator

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_paginator("list_recommender_recipes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles/paginator/ListRecommenderRecipes.html#CustomerProfiles.Paginator.ListRecommenderRecipes)

```python
# ListRecommenderRecipesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_customer_profiles.paginator import ListRecommenderRecipesPaginator

session = get_session()
async with session.create_client("customer-profiles") as client:  # (1)
    paginator: ListRecommenderRecipesPaginator = client.get_paginator("list_recommender_recipes")  # (2)
    async for item in paginator.paginate(...):
        item: ListRecommenderRecipesResponseTypeDef
        print(item)  # (3)
```

1. client: [CustomerProfilesClient](./client.md)
2. paginator: [ListRecommenderRecipesPaginator](./paginators.md#listrecommenderrecipespaginator)
3. item: `AioPageIterator[ListRecommenderRecipesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRecommenderRecipesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListRecommenderRecipesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListRecommenderRecipesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRecommenderRecipesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecommenderRecipesRequestPaginateTypeDef](./type_defs.md#listrecommenderrecipesrequestpaginatetypedef)
## ListRecommendersPaginator

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_paginator("list_recommenders")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles/paginator/ListRecommenders.html#CustomerProfiles.Paginator.ListRecommenders)

```python
# ListRecommendersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_customer_profiles.paginator import ListRecommendersPaginator

session = get_session()
async with session.create_client("customer-profiles") as client:  # (1)
    paginator: ListRecommendersPaginator = client.get_paginator("list_recommenders")  # (2)
    async for item in paginator.paginate(...):
        item: ListRecommendersResponseTypeDef
        print(item)  # (3)
```

1. client: [CustomerProfilesClient](./client.md)
2. paginator: [ListRecommendersPaginator](./paginators.md#listrecommenderspaginator)
3. item: `AioPageIterator[ListRecommendersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRecommendersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DomainName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListRecommendersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListRecommendersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRecommendersRequestPaginateTypeDef = {  # (1)
    "DomainName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecommendersRequestPaginateTypeDef](./type_defs.md#listrecommendersrequestpaginatetypedef)
## ListRuleBasedMatchesPaginator

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_paginator("list_rule_based_matches")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles/paginator/ListRuleBasedMatches.html#CustomerProfiles.Paginator.ListRuleBasedMatches)

```python
# ListRuleBasedMatchesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_customer_profiles.paginator import ListRuleBasedMatchesPaginator

session = get_session()
async with session.create_client("customer-profiles") as client:  # (1)
    paginator: ListRuleBasedMatchesPaginator = client.get_paginator("list_rule_based_matches")  # (2)
    async for item in paginator.paginate(...):
        item: ListRuleBasedMatchesResponseTypeDef
        print(item)  # (3)
```

1. client: [CustomerProfilesClient](./client.md)
2. paginator: [ListRuleBasedMatchesPaginator](./paginators.md#listrulebasedmatchespaginator)
3. item: `AioPageIterator[ListRuleBasedMatchesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRuleBasedMatchesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DomainName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListRuleBasedMatchesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListRuleBasedMatchesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRuleBasedMatchesRequestPaginateTypeDef = {  # (1)
    "DomainName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRuleBasedMatchesRequestPaginateTypeDef](./type_defs.md#listrulebasedmatchesrequestpaginatetypedef)
## ListSegmentDefinitionsPaginator

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_paginator("list_segment_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles/paginator/ListSegmentDefinitions.html#CustomerProfiles.Paginator.ListSegmentDefinitions)

```python
# ListSegmentDefinitionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_customer_profiles.paginator import ListSegmentDefinitionsPaginator

session = get_session()
async with session.create_client("customer-profiles") as client:  # (1)
    paginator: ListSegmentDefinitionsPaginator = client.get_paginator("list_segment_definitions")  # (2)
    async for item in paginator.paginate(...):
        item: ListSegmentDefinitionsResponseTypeDef
        print(item)  # (3)
```

1. client: [CustomerProfilesClient](./client.md)
2. paginator: [ListSegmentDefinitionsPaginator](./paginators.md#listsegmentdefinitionspaginator)
3. item: `AioPageIterator[ListSegmentDefinitionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSegmentDefinitionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DomainName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListSegmentDefinitionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListSegmentDefinitionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSegmentDefinitionsRequestPaginateTypeDef = {  # (1)
    "DomainName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSegmentDefinitionsRequestPaginateTypeDef](./type_defs.md#listsegmentdefinitionsrequestpaginatetypedef)
## ListUploadJobsPaginator

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_paginator("list_upload_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles/paginator/ListUploadJobs.html#CustomerProfiles.Paginator.ListUploadJobs)

```python
# ListUploadJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_customer_profiles.paginator import ListUploadJobsPaginator

session = get_session()
async with session.create_client("customer-profiles") as client:  # (1)
    paginator: ListUploadJobsPaginator = client.get_paginator("list_upload_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListUploadJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [CustomerProfilesClient](./client.md)
2. paginator: [ListUploadJobsPaginator](./paginators.md#listuploadjobspaginator)
3. item: `AioPageIterator[ListUploadJobsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListUploadJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DomainName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListUploadJobsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListUploadJobsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListUploadJobsRequestPaginateTypeDef = {  # (1)
    "DomainName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUploadJobsRequestPaginateTypeDef](./type_defs.md#listuploadjobsrequestpaginatetypedef)
