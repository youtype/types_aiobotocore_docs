<a id="paginators-for-aiobotocore-accessanalyzer-module"></a>

# Paginators for aiobotocore AccessAnalyzer module

> [Index](..) > [AccessAnalyzer](.) > Paginators

Auto-generated documentation for
[AccessAnalyzer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer)
type annotations stubs module
[types-aiobotocore-accessanalyzer](https://pypi.org/project/types-aiobotocore-accessanalyzer/).

- [Paginators for aiobotocore AccessAnalyzer module](#paginators-for-aiobotocore-accessanalyzer-module)
  - [ListAccessPreviewFindingsPaginator](#listaccesspreviewfindingspaginator)
  - [ListAccessPreviewsPaginator](#listaccesspreviewspaginator)
  - [ListAnalyzedResourcesPaginator](#listanalyzedresourcespaginator)
  - [ListAnalyzersPaginator](#listanalyzerspaginator)
  - [ListArchiveRulesPaginator](#listarchiverulespaginator)
  - [ListFindingsPaginator](#listfindingspaginator)
  - [ListPolicyGenerationsPaginator](#listpolicygenerationspaginator)
  - [ValidatePolicyPaginator](#validatepolicypaginator)

<a id="listaccesspreviewfindingspaginator"></a>

## ListAccessPreviewFindingsPaginator

Type annotations for
`session.create_client("accessanalyzer").get_paginator("list_access_preview_findings")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_accessanalyzer.paginator import ListAccessPreviewFindingsPaginator

session = get_session()
async with session.create_client("accessanalyzer") as client:
    client: AccessAnalyzerClient
    paginator: ListAccessPreviewFindingsPaginator = client.get_paginator("list_access_preview_findings")
```

Boto3 documentation:
[AccessAnalyzer.Paginator.ListAccessPreviewFindings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListAccessPreviewFindings)

Arguments for `ListAccessPreviewFindingsPaginator.paginate` method:

- `accessPreviewId`: `str` *(required)*
- `analyzerArn`: `str` *(required)*
- `filter`: `Mapping`\[`str`,
  [CriterionTypeDef](./type_defs.md#criteriontypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAccessPreviewFindingsPaginator.paginate` returns
`AsyncIterable`\[[ListAccessPreviewFindingsResponseTypeDef](./type_defs.md#listaccesspreviewfindingsresponsetypedef)\].

<a id="listaccesspreviewspaginator"></a>

## ListAccessPreviewsPaginator

Type annotations for
`session.create_client("accessanalyzer").get_paginator("list_access_previews")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_accessanalyzer.paginator import ListAccessPreviewsPaginator

session = get_session()
async with session.create_client("accessanalyzer") as client:
    client: AccessAnalyzerClient
    paginator: ListAccessPreviewsPaginator = client.get_paginator("list_access_previews")
```

Boto3 documentation:
[AccessAnalyzer.Paginator.ListAccessPreviews](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListAccessPreviews)

Arguments for `ListAccessPreviewsPaginator.paginate` method:

- `analyzerArn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAccessPreviewsPaginator.paginate` returns
`AsyncIterable`\[[ListAccessPreviewsResponseTypeDef](./type_defs.md#listaccesspreviewsresponsetypedef)\].

<a id="listanalyzedresourcespaginator"></a>

## ListAnalyzedResourcesPaginator

Type annotations for
`session.create_client("accessanalyzer").get_paginator("list_analyzed_resources")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_accessanalyzer.paginator import ListAnalyzedResourcesPaginator

session = get_session()
async with session.create_client("accessanalyzer") as client:
    client: AccessAnalyzerClient
    paginator: ListAnalyzedResourcesPaginator = client.get_paginator("list_analyzed_resources")
```

Boto3 documentation:
[AccessAnalyzer.Paginator.ListAnalyzedResources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListAnalyzedResources)

Arguments for `ListAnalyzedResourcesPaginator.paginate` method:

- `analyzerArn`: `str` *(required)*
- `resourceType`: [ResourceTypeType](./literals.md#resourcetypetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAnalyzedResourcesPaginator.paginate` returns
`AsyncIterable`\[[ListAnalyzedResourcesResponseTypeDef](./type_defs.md#listanalyzedresourcesresponsetypedef)\].

<a id="listanalyzerspaginator"></a>

## ListAnalyzersPaginator

Type annotations for
`session.create_client("accessanalyzer").get_paginator("list_analyzers")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_accessanalyzer.paginator import ListAnalyzersPaginator

session = get_session()
async with session.create_client("accessanalyzer") as client:
    client: AccessAnalyzerClient
    paginator: ListAnalyzersPaginator = client.get_paginator("list_analyzers")
```

Boto3 documentation:
[AccessAnalyzer.Paginator.ListAnalyzers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListAnalyzers)

Arguments for `ListAnalyzersPaginator.paginate` method:

- `type`: [TypeType](./literals.md#typetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAnalyzersPaginator.paginate` returns
`AsyncIterable`\[[ListAnalyzersResponseTypeDef](./type_defs.md#listanalyzersresponsetypedef)\].

<a id="listarchiverulespaginator"></a>

## ListArchiveRulesPaginator

Type annotations for
`session.create_client("accessanalyzer").get_paginator("list_archive_rules")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_accessanalyzer.paginator import ListArchiveRulesPaginator

session = get_session()
async with session.create_client("accessanalyzer") as client:
    client: AccessAnalyzerClient
    paginator: ListArchiveRulesPaginator = client.get_paginator("list_archive_rules")
```

Boto3 documentation:
[AccessAnalyzer.Paginator.ListArchiveRules](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListArchiveRules)

Arguments for `ListArchiveRulesPaginator.paginate` method:

- `analyzerName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListArchiveRulesPaginator.paginate` returns
`AsyncIterable`\[[ListArchiveRulesResponseTypeDef](./type_defs.md#listarchiverulesresponsetypedef)\].

<a id="listfindingspaginator"></a>

## ListFindingsPaginator

Type annotations for
`session.create_client("accessanalyzer").get_paginator("list_findings")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_accessanalyzer.paginator import ListFindingsPaginator

session = get_session()
async with session.create_client("accessanalyzer") as client:
    client: AccessAnalyzerClient
    paginator: ListFindingsPaginator = client.get_paginator("list_findings")
```

Boto3 documentation:
[AccessAnalyzer.Paginator.ListFindings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListFindings)

Arguments for `ListFindingsPaginator.paginate` method:

- `analyzerArn`: `str` *(required)*
- `filter`: `Mapping`\[`str`,
  [CriterionTypeDef](./type_defs.md#criteriontypedef)\]
- `sort`: [SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListFindingsPaginator.paginate` returns
`AsyncIterable`\[[ListFindingsResponseTypeDef](./type_defs.md#listfindingsresponsetypedef)\].

<a id="listpolicygenerationspaginator"></a>

## ListPolicyGenerationsPaginator

Type annotations for
`session.create_client("accessanalyzer").get_paginator("list_policy_generations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_accessanalyzer.paginator import ListPolicyGenerationsPaginator

session = get_session()
async with session.create_client("accessanalyzer") as client:
    client: AccessAnalyzerClient
    paginator: ListPolicyGenerationsPaginator = client.get_paginator("list_policy_generations")
```

Boto3 documentation:
[AccessAnalyzer.Paginator.ListPolicyGenerations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ListPolicyGenerations)

Arguments for `ListPolicyGenerationsPaginator.paginate` method:

- `principalArn`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPolicyGenerationsPaginator.paginate` returns
`AsyncIterable`\[[ListPolicyGenerationsResponseTypeDef](./type_defs.md#listpolicygenerationsresponsetypedef)\].

<a id="validatepolicypaginator"></a>

## ValidatePolicyPaginator

Type annotations for
`session.create_client("accessanalyzer").get_paginator("validate_policy")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_accessanalyzer.paginator import ValidatePolicyPaginator

session = get_session()
async with session.create_client("accessanalyzer") as client:
    client: AccessAnalyzerClient
    paginator: ValidatePolicyPaginator = client.get_paginator("validate_policy")
```

Boto3 documentation:
[AccessAnalyzer.Paginator.ValidatePolicy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#AccessAnalyzer.Paginator.ValidatePolicy)

Arguments for `ValidatePolicyPaginator.paginate` method:

- `policyDocument`: `str` *(required)*
- `policyType`: [PolicyTypeType](./literals.md#policytypetype) *(required)*
- `locale`: [LocaleType](./literals.md#localetype)
- `validatePolicyResourceType`:
  [ValidatePolicyResourceTypeType](./literals.md#validatepolicyresourcetypetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ValidatePolicyPaginator.paginate` returns
`AsyncIterable`\[[ValidatePolicyResponseTypeDef](./type_defs.md#validatepolicyresponsetypedef)\].
