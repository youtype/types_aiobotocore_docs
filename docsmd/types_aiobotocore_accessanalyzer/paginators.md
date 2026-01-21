# Paginators

> [Index](../README.md) > [AccessAnalyzer](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [AccessAnalyzer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#accessanalyzer)
    type annotations stubs module [types-aiobotocore-accessanalyzer](https://pypi.org/project/types-aiobotocore-accessanalyzer/).

## GetFindingRecommendationPaginator

Type annotations and code completion for `#!python session.create_client("accessanalyzer").get_paginator("get_finding_recommendation")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/paginator/GetFindingRecommendation.html#AccessAnalyzer.Paginator.GetFindingRecommendation)

```python
# GetFindingRecommendationPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_accessanalyzer.paginator import GetFindingRecommendationPaginator

session = get_session()
async with session.create_client("accessanalyzer") as client:  # (1)
    paginator: GetFindingRecommendationPaginator = client.get_paginator("get_finding_recommendation")  # (2)
    async for item in paginator.paginate(...):
        item: GetFindingRecommendationResponseTypeDef
        print(item)  # (3)
```

1. client: [AccessAnalyzerClient](./client.md)
2. paginator: [GetFindingRecommendationPaginator](./paginators.md#getfindingrecommendationpaginator)
3. item: `AioPageIterator[GetFindingRecommendationResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetFindingRecommendationPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    analyzerArn: str,
    id: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetFindingRecommendationResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetFindingRecommendationResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetFindingRecommendationRequestPaginateTypeDef = {  # (1)
    "analyzerArn": ...,
    "id": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetFindingRecommendationRequestPaginateTypeDef](./type_defs.md#getfindingrecommendationrequestpaginatetypedef)
## GetFindingV2Paginator

Type annotations and code completion for `#!python session.create_client("accessanalyzer").get_paginator("get_finding_v2")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/paginator/GetFindingV2.html#AccessAnalyzer.Paginator.GetFindingV2)

```python
# GetFindingV2Paginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_accessanalyzer.paginator import GetFindingV2Paginator

session = get_session()
async with session.create_client("accessanalyzer") as client:  # (1)
    paginator: GetFindingV2Paginator = client.get_paginator("get_finding_v2")  # (2)
    async for item in paginator.paginate(...):
        item: GetFindingV2ResponseTypeDef
        print(item)  # (3)
```

1. client: [AccessAnalyzerClient](./client.md)
2. paginator: [GetFindingV2Paginator](./paginators.md#getfindingv2paginator)
3. item: `AioPageIterator[GetFindingV2ResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetFindingV2Paginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    analyzerArn: str,
    id: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetFindingV2ResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetFindingV2ResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetFindingV2RequestPaginateTypeDef = {  # (1)
    "analyzerArn": ...,
    "id": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetFindingV2RequestPaginateTypeDef](./type_defs.md#getfindingv2requestpaginatetypedef)
## ListAccessPreviewFindingsPaginator

Type annotations and code completion for `#!python session.create_client("accessanalyzer").get_paginator("list_access_preview_findings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/paginator/ListAccessPreviewFindings.html#AccessAnalyzer.Paginator.ListAccessPreviewFindings)

```python
# ListAccessPreviewFindingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_accessanalyzer.paginator import ListAccessPreviewFindingsPaginator

session = get_session()
async with session.create_client("accessanalyzer") as client:  # (1)
    paginator: ListAccessPreviewFindingsPaginator = client.get_paginator("list_access_preview_findings")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccessPreviewFindingsResponseTypeDef
        print(item)  # (3)
```

1. client: [AccessAnalyzerClient](./client.md)
2. paginator: [ListAccessPreviewFindingsPaginator](./paginators.md#listaccesspreviewfindingspaginator)
3. item: `AioPageIterator[ListAccessPreviewFindingsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAccessPreviewFindingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    accessPreviewId: str,
    analyzerArn: str,
    filter: Mapping[str, CriterionUnionTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListAccessPreviewFindingsResponseTypeDef]:  # (3)
    ...
```

1. See `Mapping[str, CriterionUnionTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListAccessPreviewFindingsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAccessPreviewFindingsRequestPaginateTypeDef = {  # (1)
    "accessPreviewId": ...,
    "analyzerArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccessPreviewFindingsRequestPaginateTypeDef](./type_defs.md#listaccesspreviewfindingsrequestpaginatetypedef)
## ListAccessPreviewsPaginator

Type annotations and code completion for `#!python session.create_client("accessanalyzer").get_paginator("list_access_previews")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/paginator/ListAccessPreviews.html#AccessAnalyzer.Paginator.ListAccessPreviews)

```python
# ListAccessPreviewsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_accessanalyzer.paginator import ListAccessPreviewsPaginator

session = get_session()
async with session.create_client("accessanalyzer") as client:  # (1)
    paginator: ListAccessPreviewsPaginator = client.get_paginator("list_access_previews")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccessPreviewsResponseTypeDef
        print(item)  # (3)
```

1. client: [AccessAnalyzerClient](./client.md)
2. paginator: [ListAccessPreviewsPaginator](./paginators.md#listaccesspreviewspaginator)
3. item: `AioPageIterator[ListAccessPreviewsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAccessPreviewsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    analyzerArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAccessPreviewsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAccessPreviewsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAccessPreviewsRequestPaginateTypeDef = {  # (1)
    "analyzerArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccessPreviewsRequestPaginateTypeDef](./type_defs.md#listaccesspreviewsrequestpaginatetypedef)
## ListAnalyzedResourcesPaginator

Type annotations and code completion for `#!python session.create_client("accessanalyzer").get_paginator("list_analyzed_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/paginator/ListAnalyzedResources.html#AccessAnalyzer.Paginator.ListAnalyzedResources)

```python
# ListAnalyzedResourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_accessanalyzer.paginator import ListAnalyzedResourcesPaginator

session = get_session()
async with session.create_client("accessanalyzer") as client:  # (1)
    paginator: ListAnalyzedResourcesPaginator = client.get_paginator("list_analyzed_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListAnalyzedResourcesResponseTypeDef
        print(item)  # (3)
```

1. client: [AccessAnalyzerClient](./client.md)
2. paginator: [ListAnalyzedResourcesPaginator](./paginators.md#listanalyzedresourcespaginator)
3. item: `AioPageIterator[ListAnalyzedResourcesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAnalyzedResourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    analyzerArn: str,
    resourceType: ResourceTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListAnalyzedResourcesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListAnalyzedResourcesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAnalyzedResourcesRequestPaginateTypeDef = {  # (1)
    "analyzerArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAnalyzedResourcesRequestPaginateTypeDef](./type_defs.md#listanalyzedresourcesrequestpaginatetypedef)
## ListAnalyzersPaginator

Type annotations and code completion for `#!python session.create_client("accessanalyzer").get_paginator("list_analyzers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/paginator/ListAnalyzers.html#AccessAnalyzer.Paginator.ListAnalyzers)

```python
# ListAnalyzersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_accessanalyzer.paginator import ListAnalyzersPaginator

session = get_session()
async with session.create_client("accessanalyzer") as client:  # (1)
    paginator: ListAnalyzersPaginator = client.get_paginator("list_analyzers")  # (2)
    async for item in paginator.paginate(...):
        item: ListAnalyzersResponseTypeDef
        print(item)  # (3)
```

1. client: [AccessAnalyzerClient](./client.md)
2. paginator: [ListAnalyzersPaginator](./paginators.md#listanalyzerspaginator)
3. item: `AioPageIterator[ListAnalyzersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAnalyzersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    type: TypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListAnalyzersResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: TypeType](./literals.md#typetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListAnalyzersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAnalyzersRequestPaginateTypeDef = {  # (1)
    "type": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAnalyzersRequestPaginateTypeDef](./type_defs.md#listanalyzersrequestpaginatetypedef)
## ListArchiveRulesPaginator

Type annotations and code completion for `#!python session.create_client("accessanalyzer").get_paginator("list_archive_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/paginator/ListArchiveRules.html#AccessAnalyzer.Paginator.ListArchiveRules)

```python
# ListArchiveRulesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_accessanalyzer.paginator import ListArchiveRulesPaginator

session = get_session()
async with session.create_client("accessanalyzer") as client:  # (1)
    paginator: ListArchiveRulesPaginator = client.get_paginator("list_archive_rules")  # (2)
    async for item in paginator.paginate(...):
        item: ListArchiveRulesResponseTypeDef
        print(item)  # (3)
```

1. client: [AccessAnalyzerClient](./client.md)
2. paginator: [ListArchiveRulesPaginator](./paginators.md#listarchiverulespaginator)
3. item: `AioPageIterator[ListArchiveRulesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListArchiveRulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    analyzerName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListArchiveRulesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListArchiveRulesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListArchiveRulesRequestPaginateTypeDef = {  # (1)
    "analyzerName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListArchiveRulesRequestPaginateTypeDef](./type_defs.md#listarchiverulesrequestpaginatetypedef)
## ListFindingsPaginator

Type annotations and code completion for `#!python session.create_client("accessanalyzer").get_paginator("list_findings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/paginator/ListFindings.html#AccessAnalyzer.Paginator.ListFindings)

```python
# ListFindingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_accessanalyzer.paginator import ListFindingsPaginator

session = get_session()
async with session.create_client("accessanalyzer") as client:  # (1)
    paginator: ListFindingsPaginator = client.get_paginator("list_findings")  # (2)
    async for item in paginator.paginate(...):
        item: ListFindingsResponseTypeDef
        print(item)  # (3)
```

1. client: [AccessAnalyzerClient](./client.md)
2. paginator: [ListFindingsPaginator](./paginators.md#listfindingspaginator)
3. item: `AioPageIterator[ListFindingsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFindingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    analyzerArn: str,
    filter: Mapping[str, CriterionUnionTypeDef] = ...,  # (1)
    sort: SortCriteriaTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListFindingsResponseTypeDef]:  # (4)
    ...
```

1. See `Mapping[str, CriterionUnionTypeDef]`
2. See [:material-code-braces: SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListFindingsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFindingsRequestPaginateTypeDef = {  # (1)
    "analyzerArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFindingsRequestPaginateTypeDef](./type_defs.md#listfindingsrequestpaginatetypedef)
## ListFindingsV2Paginator

Type annotations and code completion for `#!python session.create_client("accessanalyzer").get_paginator("list_findings_v2")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/paginator/ListFindingsV2.html#AccessAnalyzer.Paginator.ListFindingsV2)

```python
# ListFindingsV2Paginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_accessanalyzer.paginator import ListFindingsV2Paginator

session = get_session()
async with session.create_client("accessanalyzer") as client:  # (1)
    paginator: ListFindingsV2Paginator = client.get_paginator("list_findings_v2")  # (2)
    async for item in paginator.paginate(...):
        item: ListFindingsV2ResponseTypeDef
        print(item)  # (3)
```

1. client: [AccessAnalyzerClient](./client.md)
2. paginator: [ListFindingsV2Paginator](./paginators.md#listfindingsv2paginator)
3. item: `AioPageIterator[ListFindingsV2ResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFindingsV2Paginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    analyzerArn: str,
    filter: Mapping[str, CriterionUnionTypeDef] = ...,  # (1)
    sort: SortCriteriaTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListFindingsV2ResponseTypeDef]:  # (4)
    ...
```

1. See `Mapping[str, CriterionUnionTypeDef]`
2. See [:material-code-braces: SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListFindingsV2ResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFindingsV2RequestPaginateTypeDef = {  # (1)
    "analyzerArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFindingsV2RequestPaginateTypeDef](./type_defs.md#listfindingsv2requestpaginatetypedef)
## ListPolicyGenerationsPaginator

Type annotations and code completion for `#!python session.create_client("accessanalyzer").get_paginator("list_policy_generations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/paginator/ListPolicyGenerations.html#AccessAnalyzer.Paginator.ListPolicyGenerations)

```python
# ListPolicyGenerationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_accessanalyzer.paginator import ListPolicyGenerationsPaginator

session = get_session()
async with session.create_client("accessanalyzer") as client:  # (1)
    paginator: ListPolicyGenerationsPaginator = client.get_paginator("list_policy_generations")  # (2)
    async for item in paginator.paginate(...):
        item: ListPolicyGenerationsResponseTypeDef
        print(item)  # (3)
```

1. client: [AccessAnalyzerClient](./client.md)
2. paginator: [ListPolicyGenerationsPaginator](./paginators.md#listpolicygenerationspaginator)
3. item: `AioPageIterator[ListPolicyGenerationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPolicyGenerationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    principalArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListPolicyGenerationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListPolicyGenerationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPolicyGenerationsRequestPaginateTypeDef = {  # (1)
    "principalArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPolicyGenerationsRequestPaginateTypeDef](./type_defs.md#listpolicygenerationsrequestpaginatetypedef)
## ValidatePolicyPaginator

Type annotations and code completion for `#!python session.create_client("accessanalyzer").get_paginator("validate_policy")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer/paginator/ValidatePolicy.html#AccessAnalyzer.Paginator.ValidatePolicy)

```python
# ValidatePolicyPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_accessanalyzer.paginator import ValidatePolicyPaginator

session = get_session()
async with session.create_client("accessanalyzer") as client:  # (1)
    paginator: ValidatePolicyPaginator = client.get_paginator("validate_policy")  # (2)
    async for item in paginator.paginate(...):
        item: ValidatePolicyResponseTypeDef
        print(item)  # (3)
```

1. client: [AccessAnalyzerClient](./client.md)
2. paginator: [ValidatePolicyPaginator](./paginators.md#validatepolicypaginator)
3. item: `AioPageIterator[ValidatePolicyResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ValidatePolicyPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    policyDocument: str,
    policyType: PolicyTypeType,  # (1)
    locale: LocaleType = ...,  # (2)
    validatePolicyResourceType: ValidatePolicyResourceTypeType = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[ValidatePolicyResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype)
2. See [:material-code-brackets: LocaleType](./literals.md#localetype)
3. See [:material-code-brackets: ValidatePolicyResourceTypeType](./literals.md#validatepolicyresourcetypetype)
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[ValidatePolicyResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ValidatePolicyRequestPaginateTypeDef = {  # (1)
    "policyDocument": ...,
    "policyType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ValidatePolicyRequestPaginateTypeDef](./type_defs.md#validatepolicyrequestpaginatetypedef)
