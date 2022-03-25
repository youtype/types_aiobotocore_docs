<a id="paginators-for-aiobotocore-inspector2-module"></a>

# Paginators for aiobotocore Inspector2 module

> [Index](../README.md) > [Inspector2](./README.md) > Paginators

Auto-generated documentation for
[Inspector2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
type annotations stubs module
[types-aiobotocore-inspector2](https://pypi.org/project/types-aiobotocore-inspector2/).

- [Paginators for aiobotocore Inspector2 module](#paginators-for-aiobotocore-inspector2-module)
  - [ListAccountPermissionsPaginator](#listaccountpermissionspaginator)
  - [ListCoveragePaginator](#listcoveragepaginator)
  - [ListCoverageStatisticsPaginator](#listcoveragestatisticspaginator)
  - [ListDelegatedAdminAccountsPaginator](#listdelegatedadminaccountspaginator)
  - [ListFiltersPaginator](#listfilterspaginator)
  - [ListFindingAggregationsPaginator](#listfindingaggregationspaginator)
  - [ListFindingsPaginator](#listfindingspaginator)
  - [ListMembersPaginator](#listmemberspaginator)
  - [ListUsageTotalsPaginator](#listusagetotalspaginator)

<a id="listaccountpermissionspaginator"></a>

## ListAccountPermissionsPaginator

Type annotations for
`session.create_client("inspector2").get_paginator("list_account_permissions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import ListAccountPermissionsPaginator

session = get_session()
async with session.create_client("inspector2") as client:
    client: Inspector2Client
    paginator: ListAccountPermissionsPaginator = client.get_paginator("list_account_permissions")
```

Boto3 documentation:
[Inspector2.Paginator.ListAccountPermissions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListAccountPermissions)

Arguments for `ListAccountPermissionsPaginator.paginate` method:

- `service`: [ServiceType](./literals.md#servicetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAccountPermissionsPaginator.paginate` returns
`AsyncIterator`\[[ListAccountPermissionsResponseTypeDef](./type_defs.md#listaccountpermissionsresponsetypedef)\].

<a id="listcoveragepaginator"></a>

## ListCoveragePaginator

Type annotations for
`session.create_client("inspector2").get_paginator("list_coverage")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import ListCoveragePaginator

session = get_session()
async with session.create_client("inspector2") as client:
    client: Inspector2Client
    paginator: ListCoveragePaginator = client.get_paginator("list_coverage")
```

Boto3 documentation:
[Inspector2.Paginator.ListCoverage](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListCoverage)

Arguments for `ListCoveragePaginator.paginate` method:

- `filterCriteria`:
  [CoverageFilterCriteriaTypeDef](./type_defs.md#coveragefiltercriteriatypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListCoveragePaginator.paginate` returns
`AsyncIterator`\[[ListCoverageResponseTypeDef](./type_defs.md#listcoverageresponsetypedef)\].

<a id="listcoveragestatisticspaginator"></a>

## ListCoverageStatisticsPaginator

Type annotations for
`session.create_client("inspector2").get_paginator("list_coverage_statistics")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import ListCoverageStatisticsPaginator

session = get_session()
async with session.create_client("inspector2") as client:
    client: Inspector2Client
    paginator: ListCoverageStatisticsPaginator = client.get_paginator("list_coverage_statistics")
```

Boto3 documentation:
[Inspector2.Paginator.ListCoverageStatistics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListCoverageStatistics)

Arguments for `ListCoverageStatisticsPaginator.paginate` method:

- `filterCriteria`:
  [CoverageFilterCriteriaTypeDef](./type_defs.md#coveragefiltercriteriatypedef)
- `groupBy`: [GroupKeyType](./literals.md#groupkeytype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListCoverageStatisticsPaginator.paginate` returns
`AsyncIterator`\[[ListCoverageStatisticsResponseTypeDef](./type_defs.md#listcoveragestatisticsresponsetypedef)\].

<a id="listdelegatedadminaccountspaginator"></a>

## ListDelegatedAdminAccountsPaginator

Type annotations for
`session.create_client("inspector2").get_paginator("list_delegated_admin_accounts")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import ListDelegatedAdminAccountsPaginator

session = get_session()
async with session.create_client("inspector2") as client:
    client: Inspector2Client
    paginator: ListDelegatedAdminAccountsPaginator = client.get_paginator("list_delegated_admin_accounts")
```

Boto3 documentation:
[Inspector2.Paginator.ListDelegatedAdminAccounts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListDelegatedAdminAccounts)

Arguments for `ListDelegatedAdminAccountsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDelegatedAdminAccountsPaginator.paginate` returns
`AsyncIterator`\[[ListDelegatedAdminAccountsResponseTypeDef](./type_defs.md#listdelegatedadminaccountsresponsetypedef)\].

<a id="listfilterspaginator"></a>

## ListFiltersPaginator

Type annotations for
`session.create_client("inspector2").get_paginator("list_filters")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import ListFiltersPaginator

session = get_session()
async with session.create_client("inspector2") as client:
    client: Inspector2Client
    paginator: ListFiltersPaginator = client.get_paginator("list_filters")
```

Boto3 documentation:
[Inspector2.Paginator.ListFilters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFilters)

Arguments for `ListFiltersPaginator.paginate` method:

- `action`: [FilterActionType](./literals.md#filteractiontype)
- `arns`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListFiltersPaginator.paginate` returns
`AsyncIterator`\[[ListFiltersResponseTypeDef](./type_defs.md#listfiltersresponsetypedef)\].

<a id="listfindingaggregationspaginator"></a>

## ListFindingAggregationsPaginator

Type annotations for
`session.create_client("inspector2").get_paginator("list_finding_aggregations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import ListFindingAggregationsPaginator

session = get_session()
async with session.create_client("inspector2") as client:
    client: Inspector2Client
    paginator: ListFindingAggregationsPaginator = client.get_paginator("list_finding_aggregations")
```

Boto3 documentation:
[Inspector2.Paginator.ListFindingAggregations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindingAggregations)

Arguments for `ListFindingAggregationsPaginator.paginate` method:

- `aggregationType`: [AggregationTypeType](./literals.md#aggregationtypetype)
  *(required)*
- `accountIds`:
  `Sequence`\[[StringFilterTypeDef](./type_defs.md#stringfiltertypedef)\]
- `aggregationRequest`:
  [AggregationRequestTypeDef](./type_defs.md#aggregationrequesttypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListFindingAggregationsPaginator.paginate` returns
`AsyncIterator`\[[ListFindingAggregationsResponseTypeDef](./type_defs.md#listfindingaggregationsresponsetypedef)\].

<a id="listfindingspaginator"></a>

## ListFindingsPaginator

Type annotations for
`session.create_client("inspector2").get_paginator("list_findings")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import ListFindingsPaginator

session = get_session()
async with session.create_client("inspector2") as client:
    client: Inspector2Client
    paginator: ListFindingsPaginator = client.get_paginator("list_findings")
```

Boto3 documentation:
[Inspector2.Paginator.ListFindings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindings)

Arguments for `ListFindingsPaginator.paginate` method:

- `filterCriteria`:
  [FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef)
- `sortCriteria`: [SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListFindingsPaginator.paginate` returns
`AsyncIterator`\[[ListFindingsResponseTypeDef](./type_defs.md#listfindingsresponsetypedef)\].

<a id="listmemberspaginator"></a>

## ListMembersPaginator

Type annotations for
`session.create_client("inspector2").get_paginator("list_members")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import ListMembersPaginator

session = get_session()
async with session.create_client("inspector2") as client:
    client: Inspector2Client
    paginator: ListMembersPaginator = client.get_paginator("list_members")
```

Boto3 documentation:
[Inspector2.Paginator.ListMembers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListMembers)

Arguments for `ListMembersPaginator.paginate` method:

- `onlyAssociated`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListMembersPaginator.paginate` returns
`AsyncIterator`\[[ListMembersResponseTypeDef](./type_defs.md#listmembersresponsetypedef)\].

<a id="listusagetotalspaginator"></a>

## ListUsageTotalsPaginator

Type annotations for
`session.create_client("inspector2").get_paginator("list_usage_totals")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import ListUsageTotalsPaginator

session = get_session()
async with session.create_client("inspector2") as client:
    client: Inspector2Client
    paginator: ListUsageTotalsPaginator = client.get_paginator("list_usage_totals")
```

Boto3 documentation:
[Inspector2.Paginator.ListUsageTotals](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListUsageTotals)

Arguments for `ListUsageTotalsPaginator.paginate` method:

- `accountIds`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListUsageTotalsPaginator.paginate` returns
`AsyncIterator`\[[ListUsageTotalsResponseTypeDef](./type_defs.md#listusagetotalsresponsetypedef)\].