# Paginators

> [Index](../README.md) > [Inspector2](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Inspector2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
    type annotations stubs module [types-aiobotocore-inspector2](https://pypi.org/project/types-aiobotocore-inspector2/).

## ListAccountPermissionsPaginator

Type annotations and code completion for `#!python session.create_client("inspector2").get_paginator("list_account_permissions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListAccountPermissions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import ListAccountPermissionsPaginator

session = get_session()
async with session.create_client("inspector2") as client:
    client: Inspector2Client
    paginator: ListAccountPermissionsPaginator = client.get_paginator("list_account_permissions")
```


### paginate

Type annotations and code completion for `#!python ListAccountPermissionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    service: ServiceType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListAccountPermissionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ServiceType](./literals.md#servicetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAccountPermissionsResponseTypeDef](./type_defs.md#listaccountpermissionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef = {  # (1)
    "service": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef](./type_defs.md#listaccountpermissionsrequestlistaccountpermissionspaginatetypedef) 
## ListCoveragePaginator

Type annotations and code completion for `#!python session.create_client("inspector2").get_paginator("list_coverage")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListCoverage)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import ListCoveragePaginator

session = get_session()
async with session.create_client("inspector2") as client:
    client: Inspector2Client
    paginator: ListCoveragePaginator = client.get_paginator("list_coverage")
```


### paginate

Type annotations and code completion for `#!python ListCoveragePaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    filterCriteria: CoverageFilterCriteriaTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListCoverageResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: CoverageFilterCriteriaTypeDef](./type_defs.md#coveragefiltercriteriatypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListCoverageResponseTypeDef](./type_defs.md#listcoverageresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListCoverageRequestListCoveragePaginateTypeDef = {  # (1)
    "filterCriteria": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCoverageRequestListCoveragePaginateTypeDef](./type_defs.md#listcoveragerequestlistcoveragepaginatetypedef) 
## ListCoverageStatisticsPaginator

Type annotations and code completion for `#!python session.create_client("inspector2").get_paginator("list_coverage_statistics")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListCoverageStatistics)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import ListCoverageStatisticsPaginator

session = get_session()
async with session.create_client("inspector2") as client:
    client: Inspector2Client
    paginator: ListCoverageStatisticsPaginator = client.get_paginator("list_coverage_statistics")
```


### paginate

Type annotations and code completion for `#!python ListCoverageStatisticsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    filterCriteria: CoverageFilterCriteriaTypeDef = ...,  # (1)
    groupBy: GroupKeyType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListCoverageStatisticsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: CoverageFilterCriteriaTypeDef](./type_defs.md#coveragefiltercriteriatypedef) 
2. See [:material-code-brackets: GroupKeyType](./literals.md#groupkeytype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListCoverageStatisticsResponseTypeDef](./type_defs.md#listcoveragestatisticsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef = {  # (1)
    "filterCriteria": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef](./type_defs.md#listcoveragestatisticsrequestlistcoveragestatisticspaginatetypedef) 
## ListDelegatedAdminAccountsPaginator

Type annotations and code completion for `#!python session.create_client("inspector2").get_paginator("list_delegated_admin_accounts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListDelegatedAdminAccounts)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import ListDelegatedAdminAccountsPaginator

session = get_session()
async with session.create_client("inspector2") as client:
    client: Inspector2Client
    paginator: ListDelegatedAdminAccountsPaginator = client.get_paginator("list_delegated_admin_accounts")
```


### paginate

Type annotations and code completion for `#!python ListDelegatedAdminAccountsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDelegatedAdminAccountsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDelegatedAdminAccountsResponseTypeDef](./type_defs.md#listdelegatedadminaccountsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef](./type_defs.md#listdelegatedadminaccountsrequestlistdelegatedadminaccountspaginatetypedef) 
## ListFiltersPaginator

Type annotations and code completion for `#!python session.create_client("inspector2").get_paginator("list_filters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFilters)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import ListFiltersPaginator

session = get_session()
async with session.create_client("inspector2") as client:
    client: Inspector2Client
    paginator: ListFiltersPaginator = client.get_paginator("list_filters")
```


### paginate

Type annotations and code completion for `#!python ListFiltersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    action: FilterActionType = ...,  # (1)
    arns: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListFiltersResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: FilterActionType](./literals.md#filteractiontype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListFiltersResponseTypeDef](./type_defs.md#listfiltersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListFiltersRequestListFiltersPaginateTypeDef = {  # (1)
    "action": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFiltersRequestListFiltersPaginateTypeDef](./type_defs.md#listfiltersrequestlistfilterspaginatetypedef) 
## ListFindingAggregationsPaginator

Type annotations and code completion for `#!python session.create_client("inspector2").get_paginator("list_finding_aggregations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindingAggregations)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import ListFindingAggregationsPaginator

session = get_session()
async with session.create_client("inspector2") as client:
    client: Inspector2Client
    paginator: ListFindingAggregationsPaginator = client.get_paginator("list_finding_aggregations")
```


### paginate

Type annotations and code completion for `#!python ListFindingAggregationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    aggregationType: AggregationTypeType,  # (1)
    accountIds: Sequence[StringFilterTypeDef] = ...,  # (2)
    aggregationRequest: AggregationRequestTypeDef = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AsyncIterator[ListFindingAggregationsResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: AggregationTypeType](./literals.md#aggregationtypetype) 
2. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
3. See [:material-code-braces: AggregationRequestTypeDef](./type_defs.md#aggregationrequesttypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: ListFindingAggregationsResponseTypeDef](./type_defs.md#listfindingaggregationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef = {  # (1)
    "aggregationType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef](./type_defs.md#listfindingaggregationsrequestlistfindingaggregationspaginatetypedef) 
## ListFindingsPaginator

Type annotations and code completion for `#!python session.create_client("inspector2").get_paginator("list_findings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindings)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import ListFindingsPaginator

session = get_session()
async with session.create_client("inspector2") as client:
    client: Inspector2Client
    paginator: ListFindingsPaginator = client.get_paginator("list_findings")
```


### paginate

Type annotations and code completion for `#!python ListFindingsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    filterCriteria: FilterCriteriaTypeDef = ...,  # (1)
    sortCriteria: SortCriteriaTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListFindingsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) 
2. See [:material-code-braces: SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListFindingsResponseTypeDef](./type_defs.md#listfindingsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListFindingsRequestListFindingsPaginateTypeDef = {  # (1)
    "filterCriteria": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFindingsRequestListFindingsPaginateTypeDef](./type_defs.md#listfindingsrequestlistfindingspaginatetypedef) 
## ListMembersPaginator

Type annotations and code completion for `#!python session.create_client("inspector2").get_paginator("list_members")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListMembers)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import ListMembersPaginator

session = get_session()
async with session.create_client("inspector2") as client:
    client: Inspector2Client
    paginator: ListMembersPaginator = client.get_paginator("list_members")
```


### paginate

Type annotations and code completion for `#!python ListMembersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    onlyAssociated: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListMembersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMembersResponseTypeDef](./type_defs.md#listmembersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListMembersRequestListMembersPaginateTypeDef = {  # (1)
    "onlyAssociated": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMembersRequestListMembersPaginateTypeDef](./type_defs.md#listmembersrequestlistmemberspaginatetypedef) 
## ListUsageTotalsPaginator

Type annotations and code completion for `#!python session.create_client("inspector2").get_paginator("list_usage_totals")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListUsageTotals)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import ListUsageTotalsPaginator

session = get_session()
async with session.create_client("inspector2") as client:
    client: Inspector2Client
    paginator: ListUsageTotalsPaginator = client.get_paginator("list_usage_totals")
```


### paginate

Type annotations and code completion for `#!python ListUsageTotalsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    accountIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListUsageTotalsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListUsageTotalsResponseTypeDef](./type_defs.md#listusagetotalsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListUsageTotalsRequestListUsageTotalsPaginateTypeDef = {  # (1)
    "accountIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUsageTotalsRequestListUsageTotalsPaginateTypeDef](./type_defs.md#listusagetotalsrequestlistusagetotalspaginatetypedef) 
