# Paginators

> [Index](../README.md) > [TrustedAdvisorPublicAPI](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [TrustedAdvisorPublicAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#trustedadvisorpublicapi)
    type annotations stubs module [types-aiobotocore-trustedadvisor](https://pypi.org/project/types-aiobotocore-trustedadvisor/).

## ListChecksPaginator

Type annotations and code completion for `#!python session.create_client("trustedadvisor").get_paginator("list_checks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor/paginator/ListChecks.html#TrustedAdvisorPublicAPI.Paginator.ListChecks)

```python
# ListChecksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_trustedadvisor.paginator import ListChecksPaginator

session = get_session()
async with session.create_client("trustedadvisor") as client:  # (1)
    paginator: ListChecksPaginator = client.get_paginator("list_checks")  # (2)
    async for item in paginator.paginate(...):
        item: ListChecksResponseTypeDef
        print(item)  # (3)
```

1. client: [TrustedAdvisorPublicAPIClient](./client.md)
2. paginator: [ListChecksPaginator](./paginators.md#listcheckspaginator)
3. item: [:material-code-braces: ListChecksResponseTypeDef](./type_defs.md#listchecksresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListChecksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    awsService: str = ...,
    language: RecommendationLanguageType = ...,  # (1)
    pillar: RecommendationPillarType = ...,  # (2)
    source: RecommendationSourceType = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AioPageIterator[ListChecksResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: RecommendationLanguageType](./literals.md#recommendationlanguagetype) 
2. See [:material-code-brackets: RecommendationPillarType](./literals.md#recommendationpillartype) 
3. See [:material-code-brackets: RecommendationSourceType](./literals.md#recommendationsourcetype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: ListChecksResponseTypeDef](./type_defs.md#listchecksresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListChecksRequestPaginateTypeDef = {  # (1)
    "awsService": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListChecksRequestPaginateTypeDef](./type_defs.md#listchecksrequestpaginatetypedef) 
## ListOrganizationRecommendationAccountsPaginator

Type annotations and code completion for `#!python session.create_client("trustedadvisor").get_paginator("list_organization_recommendation_accounts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor/paginator/ListOrganizationRecommendationAccounts.html#TrustedAdvisorPublicAPI.Paginator.ListOrganizationRecommendationAccounts)

```python
# ListOrganizationRecommendationAccountsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_trustedadvisor.paginator import ListOrganizationRecommendationAccountsPaginator

session = get_session()
async with session.create_client("trustedadvisor") as client:  # (1)
    paginator: ListOrganizationRecommendationAccountsPaginator = client.get_paginator("list_organization_recommendation_accounts")  # (2)
    async for item in paginator.paginate(...):
        item: ListOrganizationRecommendationAccountsResponseTypeDef
        print(item)  # (3)
```

1. client: [TrustedAdvisorPublicAPIClient](./client.md)
2. paginator: [ListOrganizationRecommendationAccountsPaginator](./paginators.md#listorganizationrecommendationaccountspaginator)
3. item: [:material-code-braces: ListOrganizationRecommendationAccountsResponseTypeDef](./type_defs.md#listorganizationrecommendationaccountsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListOrganizationRecommendationAccountsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    organizationRecommendationIdentifier: str,
    affectedAccountId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListOrganizationRecommendationAccountsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListOrganizationRecommendationAccountsResponseTypeDef](./type_defs.md#listorganizationrecommendationaccountsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListOrganizationRecommendationAccountsRequestPaginateTypeDef = {  # (1)
    "organizationRecommendationIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOrganizationRecommendationAccountsRequestPaginateTypeDef](./type_defs.md#listorganizationrecommendationaccountsrequestpaginatetypedef) 
## ListOrganizationRecommendationResourcesPaginator

Type annotations and code completion for `#!python session.create_client("trustedadvisor").get_paginator("list_organization_recommendation_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor/paginator/ListOrganizationRecommendationResources.html#TrustedAdvisorPublicAPI.Paginator.ListOrganizationRecommendationResources)

```python
# ListOrganizationRecommendationResourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_trustedadvisor.paginator import ListOrganizationRecommendationResourcesPaginator

session = get_session()
async with session.create_client("trustedadvisor") as client:  # (1)
    paginator: ListOrganizationRecommendationResourcesPaginator = client.get_paginator("list_organization_recommendation_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListOrganizationRecommendationResourcesResponseTypeDef
        print(item)  # (3)
```

1. client: [TrustedAdvisorPublicAPIClient](./client.md)
2. paginator: [ListOrganizationRecommendationResourcesPaginator](./paginators.md#listorganizationrecommendationresourcespaginator)
3. item: [:material-code-braces: ListOrganizationRecommendationResourcesResponseTypeDef](./type_defs.md#listorganizationrecommendationresourcesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListOrganizationRecommendationResourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    organizationRecommendationIdentifier: str,
    affectedAccountId: str = ...,
    exclusionStatus: ExclusionStatusType = ...,  # (1)
    regionCode: str = ...,
    status: ResourceStatusType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListOrganizationRecommendationResourcesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: ExclusionStatusType](./literals.md#exclusionstatustype) 
2. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListOrganizationRecommendationResourcesResponseTypeDef](./type_defs.md#listorganizationrecommendationresourcesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListOrganizationRecommendationResourcesRequestPaginateTypeDef = {  # (1)
    "organizationRecommendationIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOrganizationRecommendationResourcesRequestPaginateTypeDef](./type_defs.md#listorganizationrecommendationresourcesrequestpaginatetypedef) 
## ListOrganizationRecommendationsPaginator

Type annotations and code completion for `#!python session.create_client("trustedadvisor").get_paginator("list_organization_recommendations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor/paginator/ListOrganizationRecommendations.html#TrustedAdvisorPublicAPI.Paginator.ListOrganizationRecommendations)

```python
# ListOrganizationRecommendationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_trustedadvisor.paginator import ListOrganizationRecommendationsPaginator

session = get_session()
async with session.create_client("trustedadvisor") as client:  # (1)
    paginator: ListOrganizationRecommendationsPaginator = client.get_paginator("list_organization_recommendations")  # (2)
    async for item in paginator.paginate(...):
        item: ListOrganizationRecommendationsResponseTypeDef
        print(item)  # (3)
```

1. client: [TrustedAdvisorPublicAPIClient](./client.md)
2. paginator: [ListOrganizationRecommendationsPaginator](./paginators.md#listorganizationrecommendationspaginator)
3. item: [:material-code-braces: ListOrganizationRecommendationsResponseTypeDef](./type_defs.md#listorganizationrecommendationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListOrganizationRecommendationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    afterLastUpdatedAt: TimestampTypeDef = ...,
    awsService: str = ...,
    beforeLastUpdatedAt: TimestampTypeDef = ...,
    checkIdentifier: str = ...,
    pillar: RecommendationPillarType = ...,  # (1)
    source: RecommendationSourceType = ...,  # (2)
    status: RecommendationStatusType = ...,  # (3)
    type: RecommendationTypeType = ...,  # (4)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (5)
) -> AioPageIterator[ListOrganizationRecommendationsResponseTypeDef]:  # (6)
    ...
```

1. See [:material-code-brackets: RecommendationPillarType](./literals.md#recommendationpillartype) 
2. See [:material-code-brackets: RecommendationSourceType](./literals.md#recommendationsourcetype) 
3. See [:material-code-brackets: RecommendationStatusType](./literals.md#recommendationstatustype) 
4. See [:material-code-brackets: RecommendationTypeType](./literals.md#recommendationtypetype) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
6. See [:material-code-braces: ListOrganizationRecommendationsResponseTypeDef](./type_defs.md#listorganizationrecommendationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListOrganizationRecommendationsRequestPaginateTypeDef = {  # (1)
    "afterLastUpdatedAt": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOrganizationRecommendationsRequestPaginateTypeDef](./type_defs.md#listorganizationrecommendationsrequestpaginatetypedef) 
## ListRecommendationResourcesPaginator

Type annotations and code completion for `#!python session.create_client("trustedadvisor").get_paginator("list_recommendation_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor/paginator/ListRecommendationResources.html#TrustedAdvisorPublicAPI.Paginator.ListRecommendationResources)

```python
# ListRecommendationResourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_trustedadvisor.paginator import ListRecommendationResourcesPaginator

session = get_session()
async with session.create_client("trustedadvisor") as client:  # (1)
    paginator: ListRecommendationResourcesPaginator = client.get_paginator("list_recommendation_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListRecommendationResourcesResponseTypeDef
        print(item)  # (3)
```

1. client: [TrustedAdvisorPublicAPIClient](./client.md)
2. paginator: [ListRecommendationResourcesPaginator](./paginators.md#listrecommendationresourcespaginator)
3. item: [:material-code-braces: ListRecommendationResourcesResponseTypeDef](./type_defs.md#listrecommendationresourcesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRecommendationResourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    recommendationIdentifier: str,
    exclusionStatus: ExclusionStatusType = ...,  # (1)
    regionCode: str = ...,
    status: ResourceStatusType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListRecommendationResourcesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: ExclusionStatusType](./literals.md#exclusionstatustype) 
2. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListRecommendationResourcesResponseTypeDef](./type_defs.md#listrecommendationresourcesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRecommendationResourcesRequestPaginateTypeDef = {  # (1)
    "recommendationIdentifier": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecommendationResourcesRequestPaginateTypeDef](./type_defs.md#listrecommendationresourcesrequestpaginatetypedef) 
## ListRecommendationsPaginator

Type annotations and code completion for `#!python session.create_client("trustedadvisor").get_paginator("list_recommendations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor/paginator/ListRecommendations.html#TrustedAdvisorPublicAPI.Paginator.ListRecommendations)

```python
# ListRecommendationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_trustedadvisor.paginator import ListRecommendationsPaginator

session = get_session()
async with session.create_client("trustedadvisor") as client:  # (1)
    paginator: ListRecommendationsPaginator = client.get_paginator("list_recommendations")  # (2)
    async for item in paginator.paginate(...):
        item: ListRecommendationsResponseTypeDef
        print(item)  # (3)
```

1. client: [TrustedAdvisorPublicAPIClient](./client.md)
2. paginator: [ListRecommendationsPaginator](./paginators.md#listrecommendationspaginator)
3. item: [:material-code-braces: ListRecommendationsResponseTypeDef](./type_defs.md#listrecommendationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRecommendationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    afterLastUpdatedAt: TimestampTypeDef = ...,
    awsService: str = ...,
    beforeLastUpdatedAt: TimestampTypeDef = ...,
    checkIdentifier: str = ...,
    pillar: RecommendationPillarType = ...,  # (1)
    source: RecommendationSourceType = ...,  # (2)
    status: RecommendationStatusType = ...,  # (3)
    type: RecommendationTypeType = ...,  # (4)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (5)
) -> AioPageIterator[ListRecommendationsResponseTypeDef]:  # (6)
    ...
```

1. See [:material-code-brackets: RecommendationPillarType](./literals.md#recommendationpillartype) 
2. See [:material-code-brackets: RecommendationSourceType](./literals.md#recommendationsourcetype) 
3. See [:material-code-brackets: RecommendationStatusType](./literals.md#recommendationstatustype) 
4. See [:material-code-brackets: RecommendationTypeType](./literals.md#recommendationtypetype) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
6. See [:material-code-braces: ListRecommendationsResponseTypeDef](./type_defs.md#listrecommendationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRecommendationsRequestPaginateTypeDef = {  # (1)
    "afterLastUpdatedAt": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRecommendationsRequestPaginateTypeDef](./type_defs.md#listrecommendationsrequestpaginatetypedef) 
