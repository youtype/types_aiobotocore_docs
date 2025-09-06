# Paginators

> [Index](../README.md) > [Inspector2](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Inspector2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#inspector2)
    type annotations stubs module [types-aiobotocore-inspector2](https://pypi.org/project/types-aiobotocore-inspector2/).

## GetCisScanResultDetailsPaginator

Type annotations and code completion for `#!python session.create_client("inspector2").get_paginator("get_cis_scan_result_details")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2/paginator/GetCisScanResultDetails.html#Inspector2.Paginator.GetCisScanResultDetails)

```python
# GetCisScanResultDetailsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import GetCisScanResultDetailsPaginator

session = get_session()
async with session.create_client("inspector2") as client:  # (1)
    paginator: GetCisScanResultDetailsPaginator = client.get_paginator("get_cis_scan_result_details")  # (2)
    async for item in paginator.paginate(...):
        item: GetCisScanResultDetailsResponseTypeDef
        print(item)  # (3)
```

1. client: [Inspector2Client](./client.md)
2. paginator: [GetCisScanResultDetailsPaginator](./paginators.md#getcisscanresultdetailspaginator)
3. item: `AioPageIterator[GetCisScanResultDetailsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetCisScanResultDetailsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    scanArn: str,
    targetResourceId: str,
    accountId: str,
    filterCriteria: CisScanResultDetailsFilterCriteriaTypeDef = ...,  # (1)
    sortBy: CisScanResultDetailsSortByType = ...,  # (2)
    sortOrder: CisSortOrderType = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[GetCisScanResultDetailsResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-braces: CisScanResultDetailsFilterCriteriaTypeDef](./type_defs.md#cisscanresultdetailsfiltercriteriatypedef)
2. See [:material-code-brackets: CisScanResultDetailsSortByType](./literals.md#cisscanresultdetailssortbytype)
3. See [:material-code-brackets: CisSortOrderType](./literals.md#cissortordertype)
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[GetCisScanResultDetailsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetCisScanResultDetailsRequestPaginateTypeDef = {  # (1)
    "scanArn": ...,
    "targetResourceId": ...,
    "accountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetCisScanResultDetailsRequestPaginateTypeDef](./type_defs.md#getcisscanresultdetailsrequestpaginatetypedef)
## GetClustersForImagePaginator

Type annotations and code completion for `#!python session.create_client("inspector2").get_paginator("get_clusters_for_image")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2/paginator/GetClustersForImage.html#Inspector2.Paginator.GetClustersForImage)

```python
# GetClustersForImagePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import GetClustersForImagePaginator

session = get_session()
async with session.create_client("inspector2") as client:  # (1)
    paginator: GetClustersForImagePaginator = client.get_paginator("get_clusters_for_image")  # (2)
    async for item in paginator.paginate(...):
        item: GetClustersForImageResponseTypeDef
        print(item)  # (3)
```

1. client: [Inspector2Client](./client.md)
2. paginator: [GetClustersForImagePaginator](./paginators.md#getclustersforimagepaginator)
3. item: `AioPageIterator[GetClustersForImageResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetClustersForImagePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filter: ClusterForImageFilterCriteriaTypeDef,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[GetClustersForImageResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ClusterForImageFilterCriteriaTypeDef](./type_defs.md#clusterforimagefiltercriteriatypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[GetClustersForImageResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetClustersForImageRequestPaginateTypeDef = {  # (1)
    "filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetClustersForImageRequestPaginateTypeDef](./type_defs.md#getclustersforimagerequestpaginatetypedef)
## ListAccountPermissionsPaginator

Type annotations and code completion for `#!python session.create_client("inspector2").get_paginator("list_account_permissions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2/paginator/ListAccountPermissions.html#Inspector2.Paginator.ListAccountPermissions)

```python
# ListAccountPermissionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import ListAccountPermissionsPaginator

session = get_session()
async with session.create_client("inspector2") as client:  # (1)
    paginator: ListAccountPermissionsPaginator = client.get_paginator("list_account_permissions")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccountPermissionsResponseTypeDef
        print(item)  # (3)
```

1. client: [Inspector2Client](./client.md)
2. paginator: [ListAccountPermissionsPaginator](./paginators.md#listaccountpermissionspaginator)
3. item: `AioPageIterator[ListAccountPermissionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAccountPermissionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    service: ServiceType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListAccountPermissionsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ServiceType](./literals.md#servicetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListAccountPermissionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAccountPermissionsRequestPaginateTypeDef = {  # (1)
    "service": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccountPermissionsRequestPaginateTypeDef](./type_defs.md#listaccountpermissionsrequestpaginatetypedef)
## ListCisScanConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("inspector2").get_paginator("list_cis_scan_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2/paginator/ListCisScanConfigurations.html#Inspector2.Paginator.ListCisScanConfigurations)

```python
# ListCisScanConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import ListCisScanConfigurationsPaginator

session = get_session()
async with session.create_client("inspector2") as client:  # (1)
    paginator: ListCisScanConfigurationsPaginator = client.get_paginator("list_cis_scan_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListCisScanConfigurationsResponseTypeDef
        print(item)  # (3)
```

1. client: [Inspector2Client](./client.md)
2. paginator: [ListCisScanConfigurationsPaginator](./paginators.md#listcisscanconfigurationspaginator)
3. item: `AioPageIterator[ListCisScanConfigurationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCisScanConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filterCriteria: ListCisScanConfigurationsFilterCriteriaTypeDef = ...,  # (1)
    sortBy: CisScanConfigurationsSortByType = ...,  # (2)
    sortOrder: CisSortOrderType = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[ListCisScanConfigurationsResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-braces: ListCisScanConfigurationsFilterCriteriaTypeDef](./type_defs.md#listcisscanconfigurationsfiltercriteriatypedef)
2. See [:material-code-brackets: CisScanConfigurationsSortByType](./literals.md#cisscanconfigurationssortbytype)
3. See [:material-code-brackets: CisSortOrderType](./literals.md#cissortordertype)
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[ListCisScanConfigurationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCisScanConfigurationsRequestPaginateTypeDef = {  # (1)
    "filterCriteria": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCisScanConfigurationsRequestPaginateTypeDef](./type_defs.md#listcisscanconfigurationsrequestpaginatetypedef)
## ListCisScanResultsAggregatedByChecksPaginator

Type annotations and code completion for `#!python session.create_client("inspector2").get_paginator("list_cis_scan_results_aggregated_by_checks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2/paginator/ListCisScanResultsAggregatedByChecks.html#Inspector2.Paginator.ListCisScanResultsAggregatedByChecks)

```python
# ListCisScanResultsAggregatedByChecksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import ListCisScanResultsAggregatedByChecksPaginator

session = get_session()
async with session.create_client("inspector2") as client:  # (1)
    paginator: ListCisScanResultsAggregatedByChecksPaginator = client.get_paginator("list_cis_scan_results_aggregated_by_checks")  # (2)
    async for item in paginator.paginate(...):
        item: ListCisScanResultsAggregatedByChecksResponseTypeDef
        print(item)  # (3)
```

1. client: [Inspector2Client](./client.md)
2. paginator: [ListCisScanResultsAggregatedByChecksPaginator](./paginators.md#listcisscanresultsaggregatedbycheckspaginator)
3. item: `AioPageIterator[ListCisScanResultsAggregatedByChecksResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCisScanResultsAggregatedByChecksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    scanArn: str,
    filterCriteria: CisScanResultsAggregatedByChecksFilterCriteriaTypeDef = ...,  # (1)
    sortBy: CisScanResultsAggregatedByChecksSortByType = ...,  # (2)
    sortOrder: CisSortOrderType = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[ListCisScanResultsAggregatedByChecksResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-braces: CisScanResultsAggregatedByChecksFilterCriteriaTypeDef](./type_defs.md#cisscanresultsaggregatedbychecksfiltercriteriatypedef)
2. See [:material-code-brackets: CisScanResultsAggregatedByChecksSortByType](./literals.md#cisscanresultsaggregatedbycheckssortbytype)
3. See [:material-code-brackets: CisSortOrderType](./literals.md#cissortordertype)
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[ListCisScanResultsAggregatedByChecksResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCisScanResultsAggregatedByChecksRequestPaginateTypeDef = {  # (1)
    "scanArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCisScanResultsAggregatedByChecksRequestPaginateTypeDef](./type_defs.md#listcisscanresultsaggregatedbychecksrequestpaginatetypedef)
## ListCisScanResultsAggregatedByTargetResourcePaginator

Type annotations and code completion for `#!python session.create_client("inspector2").get_paginator("list_cis_scan_results_aggregated_by_target_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2/paginator/ListCisScanResultsAggregatedByTargetResource.html#Inspector2.Paginator.ListCisScanResultsAggregatedByTargetResource)

```python
# ListCisScanResultsAggregatedByTargetResourcePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import ListCisScanResultsAggregatedByTargetResourcePaginator

session = get_session()
async with session.create_client("inspector2") as client:  # (1)
    paginator: ListCisScanResultsAggregatedByTargetResourcePaginator = client.get_paginator("list_cis_scan_results_aggregated_by_target_resource")  # (2)
    async for item in paginator.paginate(...):
        item: ListCisScanResultsAggregatedByTargetResourceResponseTypeDef
        print(item)  # (3)
```

1. client: [Inspector2Client](./client.md)
2. paginator: [ListCisScanResultsAggregatedByTargetResourcePaginator](./paginators.md#listcisscanresultsaggregatedbytargetresourcepaginator)
3. item: `AioPageIterator[ListCisScanResultsAggregatedByTargetResourceResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCisScanResultsAggregatedByTargetResourcePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    scanArn: str,
    filterCriteria: CisScanResultsAggregatedByTargetResourceFilterCriteriaTypeDef = ...,  # (1)
    sortBy: CisScanResultsAggregatedByTargetResourceSortByType = ...,  # (2)
    sortOrder: CisSortOrderType = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[ListCisScanResultsAggregatedByTargetResourceResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-braces: CisScanResultsAggregatedByTargetResourceFilterCriteriaTypeDef](./type_defs.md#cisscanresultsaggregatedbytargetresourcefiltercriteriatypedef)
2. See [:material-code-brackets: CisScanResultsAggregatedByTargetResourceSortByType](./literals.md#cisscanresultsaggregatedbytargetresourcesortbytype)
3. See [:material-code-brackets: CisSortOrderType](./literals.md#cissortordertype)
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[ListCisScanResultsAggregatedByTargetResourceResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCisScanResultsAggregatedByTargetResourceRequestPaginateTypeDef = {  # (1)
    "scanArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCisScanResultsAggregatedByTargetResourceRequestPaginateTypeDef](./type_defs.md#listcisscanresultsaggregatedbytargetresourcerequestpaginatetypedef)
## ListCisScansPaginator

Type annotations and code completion for `#!python session.create_client("inspector2").get_paginator("list_cis_scans")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2/paginator/ListCisScans.html#Inspector2.Paginator.ListCisScans)

```python
# ListCisScansPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import ListCisScansPaginator

session = get_session()
async with session.create_client("inspector2") as client:  # (1)
    paginator: ListCisScansPaginator = client.get_paginator("list_cis_scans")  # (2)
    async for item in paginator.paginate(...):
        item: ListCisScansResponseTypeDef
        print(item)  # (3)
```

1. client: [Inspector2Client](./client.md)
2. paginator: [ListCisScansPaginator](./paginators.md#listcisscanspaginator)
3. item: `AioPageIterator[ListCisScansResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCisScansPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filterCriteria: ListCisScansFilterCriteriaTypeDef = ...,  # (1)
    detailLevel: ListCisScansDetailLevelType = ...,  # (2)
    sortBy: ListCisScansSortByType = ...,  # (3)
    sortOrder: CisSortOrderType = ...,  # (4)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (5)
) -> aiobotocore.paginate.AioPageIterator[ListCisScansResponseTypeDef]:  # (6)
    ...
```

1. See [:material-code-braces: ListCisScansFilterCriteriaTypeDef](./type_defs.md#listcisscansfiltercriteriatypedef)
2. See [:material-code-brackets: ListCisScansDetailLevelType](./literals.md#listcisscansdetailleveltype)
3. See [:material-code-brackets: ListCisScansSortByType](./literals.md#listcisscanssortbytype)
4. See [:material-code-brackets: CisSortOrderType](./literals.md#cissortordertype)
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
6. See `AioPageIterator[ListCisScansResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCisScansRequestPaginateTypeDef = {  # (1)
    "filterCriteria": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCisScansRequestPaginateTypeDef](./type_defs.md#listcisscansrequestpaginatetypedef)
## ListCoveragePaginator

Type annotations and code completion for `#!python session.create_client("inspector2").get_paginator("list_coverage")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2/paginator/ListCoverage.html#Inspector2.Paginator.ListCoverage)

```python
# ListCoveragePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import ListCoveragePaginator

session = get_session()
async with session.create_client("inspector2") as client:  # (1)
    paginator: ListCoveragePaginator = client.get_paginator("list_coverage")  # (2)
    async for item in paginator.paginate(...):
        item: ListCoverageResponseTypeDef
        print(item)  # (3)
```

1. client: [Inspector2Client](./client.md)
2. paginator: [ListCoveragePaginator](./paginators.md#listcoveragepaginator)
3. item: `AioPageIterator[ListCoverageResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCoveragePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filterCriteria: CoverageFilterCriteriaTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListCoverageResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: CoverageFilterCriteriaTypeDef](./type_defs.md#coveragefiltercriteriatypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListCoverageResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCoverageRequestPaginateTypeDef = {  # (1)
    "filterCriteria": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCoverageRequestPaginateTypeDef](./type_defs.md#listcoveragerequestpaginatetypedef)
## ListCoverageStatisticsPaginator

Type annotations and code completion for `#!python session.create_client("inspector2").get_paginator("list_coverage_statistics")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2/paginator/ListCoverageStatistics.html#Inspector2.Paginator.ListCoverageStatistics)

```python
# ListCoverageStatisticsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import ListCoverageStatisticsPaginator

session = get_session()
async with session.create_client("inspector2") as client:  # (1)
    paginator: ListCoverageStatisticsPaginator = client.get_paginator("list_coverage_statistics")  # (2)
    async for item in paginator.paginate(...):
        item: ListCoverageStatisticsResponseTypeDef
        print(item)  # (3)
```

1. client: [Inspector2Client](./client.md)
2. paginator: [ListCoverageStatisticsPaginator](./paginators.md#listcoveragestatisticspaginator)
3. item: `AioPageIterator[ListCoverageStatisticsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCoverageStatisticsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filterCriteria: CoverageFilterCriteriaTypeDef = ...,  # (1)
    groupBy: GroupKeyType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListCoverageStatisticsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: CoverageFilterCriteriaTypeDef](./type_defs.md#coveragefiltercriteriatypedef)
2. See [:material-code-brackets: GroupKeyType](./literals.md#groupkeytype)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListCoverageStatisticsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCoverageStatisticsRequestPaginateTypeDef = {  # (1)
    "filterCriteria": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCoverageStatisticsRequestPaginateTypeDef](./type_defs.md#listcoveragestatisticsrequestpaginatetypedef)
## ListDelegatedAdminAccountsPaginator

Type annotations and code completion for `#!python session.create_client("inspector2").get_paginator("list_delegated_admin_accounts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2/paginator/ListDelegatedAdminAccounts.html#Inspector2.Paginator.ListDelegatedAdminAccounts)

```python
# ListDelegatedAdminAccountsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import ListDelegatedAdminAccountsPaginator

session = get_session()
async with session.create_client("inspector2") as client:  # (1)
    paginator: ListDelegatedAdminAccountsPaginator = client.get_paginator("list_delegated_admin_accounts")  # (2)
    async for item in paginator.paginate(...):
        item: ListDelegatedAdminAccountsResponseTypeDef
        print(item)  # (3)
```

1. client: [Inspector2Client](./client.md)
2. paginator: [ListDelegatedAdminAccountsPaginator](./paginators.md#listdelegatedadminaccountspaginator)
3. item: `AioPageIterator[ListDelegatedAdminAccountsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDelegatedAdminAccountsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDelegatedAdminAccountsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDelegatedAdminAccountsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDelegatedAdminAccountsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDelegatedAdminAccountsRequestPaginateTypeDef](./type_defs.md#listdelegatedadminaccountsrequestpaginatetypedef)
## ListFiltersPaginator

Type annotations and code completion for `#!python session.create_client("inspector2").get_paginator("list_filters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2/paginator/ListFilters.html#Inspector2.Paginator.ListFilters)

```python
# ListFiltersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import ListFiltersPaginator

session = get_session()
async with session.create_client("inspector2") as client:  # (1)
    paginator: ListFiltersPaginator = client.get_paginator("list_filters")  # (2)
    async for item in paginator.paginate(...):
        item: ListFiltersResponseTypeDef
        print(item)  # (3)
```

1. client: [Inspector2Client](./client.md)
2. paginator: [ListFiltersPaginator](./paginators.md#listfilterspaginator)
3. item: `AioPageIterator[ListFiltersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFiltersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    arns: Sequence[str] = ...,
    action: FilterActionType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListFiltersResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: FilterActionType](./literals.md#filteractiontype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListFiltersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFiltersRequestPaginateTypeDef = {  # (1)
    "arns": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFiltersRequestPaginateTypeDef](./type_defs.md#listfiltersrequestpaginatetypedef)
## ListFindingAggregationsPaginator

Type annotations and code completion for `#!python session.create_client("inspector2").get_paginator("list_finding_aggregations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2/paginator/ListFindingAggregations.html#Inspector2.Paginator.ListFindingAggregations)

```python
# ListFindingAggregationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import ListFindingAggregationsPaginator

session = get_session()
async with session.create_client("inspector2") as client:  # (1)
    paginator: ListFindingAggregationsPaginator = client.get_paginator("list_finding_aggregations")  # (2)
    async for item in paginator.paginate(...):
        item: ListFindingAggregationsResponseTypeDef
        print(item)  # (3)
```

1. client: [Inspector2Client](./client.md)
2. paginator: [ListFindingAggregationsPaginator](./paginators.md#listfindingaggregationspaginator)
3. item: `AioPageIterator[ListFindingAggregationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFindingAggregationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    aggregationType: AggregationTypeType,  # (1)
    accountIds: Sequence[StringFilterTypeDef] = ...,  # (2)
    aggregationRequest: AggregationRequestTypeDef = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[ListFindingAggregationsResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: AggregationTypeType](./literals.md#aggregationtypetype)
2. See `Sequence[StringFilterTypeDef]`
3. See [:material-code-braces: AggregationRequestTypeDef](./type_defs.md#aggregationrequesttypedef)
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[ListFindingAggregationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFindingAggregationsRequestPaginateTypeDef = {  # (1)
    "aggregationType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFindingAggregationsRequestPaginateTypeDef](./type_defs.md#listfindingaggregationsrequestpaginatetypedef)
## ListFindingsPaginator

Type annotations and code completion for `#!python session.create_client("inspector2").get_paginator("list_findings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2/paginator/ListFindings.html#Inspector2.Paginator.ListFindings)

```python
# ListFindingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import ListFindingsPaginator

session = get_session()
async with session.create_client("inspector2") as client:  # (1)
    paginator: ListFindingsPaginator = client.get_paginator("list_findings")  # (2)
    async for item in paginator.paginate(...):
        item: ListFindingsResponseTypeDef
        print(item)  # (3)
```

1. client: [Inspector2Client](./client.md)
2. paginator: [ListFindingsPaginator](./paginators.md#listfindingspaginator)
3. item: `AioPageIterator[ListFindingsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFindingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filterCriteria: FilterCriteriaUnionTypeDef = ...,  # (1)
    sortCriteria: SortCriteriaTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListFindingsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: FilterCriteriaUnionTypeDef](#filtercriteriauniontypedef)
2. See [:material-code-braces: SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListFindingsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFindingsRequestPaginateTypeDef = {  # (1)
    "filterCriteria": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFindingsRequestPaginateTypeDef](./type_defs.md#listfindingsrequestpaginatetypedef)
## ListMembersPaginator

Type annotations and code completion for `#!python session.create_client("inspector2").get_paginator("list_members")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2/paginator/ListMembers.html#Inspector2.Paginator.ListMembers)

```python
# ListMembersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import ListMembersPaginator

session = get_session()
async with session.create_client("inspector2") as client:  # (1)
    paginator: ListMembersPaginator = client.get_paginator("list_members")  # (2)
    async for item in paginator.paginate(...):
        item: ListMembersResponseTypeDef
        print(item)  # (3)
```

1. client: [Inspector2Client](./client.md)
2. paginator: [ListMembersPaginator](./paginators.md#listmemberspaginator)
3. item: `AioPageIterator[ListMembersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListMembersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    onlyAssociated: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListMembersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListMembersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListMembersRequestPaginateTypeDef = {  # (1)
    "onlyAssociated": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMembersRequestPaginateTypeDef](./type_defs.md#listmembersrequestpaginatetypedef)
## ListUsageTotalsPaginator

Type annotations and code completion for `#!python session.create_client("inspector2").get_paginator("list_usage_totals")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2/paginator/ListUsageTotals.html#Inspector2.Paginator.ListUsageTotals)

```python
# ListUsageTotalsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import ListUsageTotalsPaginator

session = get_session()
async with session.create_client("inspector2") as client:  # (1)
    paginator: ListUsageTotalsPaginator = client.get_paginator("list_usage_totals")  # (2)
    async for item in paginator.paginate(...):
        item: ListUsageTotalsResponseTypeDef
        print(item)  # (3)
```

1. client: [Inspector2Client](./client.md)
2. paginator: [ListUsageTotalsPaginator](./paginators.md#listusagetotalspaginator)
3. item: `AioPageIterator[ListUsageTotalsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListUsageTotalsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    accountIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListUsageTotalsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListUsageTotalsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListUsageTotalsRequestPaginateTypeDef = {  # (1)
    "accountIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUsageTotalsRequestPaginateTypeDef](./type_defs.md#listusagetotalsrequestpaginatetypedef)
## SearchVulnerabilitiesPaginator

Type annotations and code completion for `#!python session.create_client("inspector2").get_paginator("search_vulnerabilities")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2/paginator/SearchVulnerabilities.html#Inspector2.Paginator.SearchVulnerabilities)

```python
# SearchVulnerabilitiesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_inspector2.paginator import SearchVulnerabilitiesPaginator

session = get_session()
async with session.create_client("inspector2") as client:  # (1)
    paginator: SearchVulnerabilitiesPaginator = client.get_paginator("search_vulnerabilities")  # (2)
    async for item in paginator.paginate(...):
        item: SearchVulnerabilitiesResponseTypeDef
        print(item)  # (3)
```

1. client: [Inspector2Client](./client.md)
2. paginator: [SearchVulnerabilitiesPaginator](./paginators.md#searchvulnerabilitiespaginator)
3. item: `AioPageIterator[SearchVulnerabilitiesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchVulnerabilitiesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filterCriteria: SearchVulnerabilitiesFilterCriteriaTypeDef,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[SearchVulnerabilitiesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: SearchVulnerabilitiesFilterCriteriaTypeDef](./type_defs.md#searchvulnerabilitiesfiltercriteriatypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[SearchVulnerabilitiesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchVulnerabilitiesRequestPaginateTypeDef = {  # (1)
    "filterCriteria": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchVulnerabilitiesRequestPaginateTypeDef](./type_defs.md#searchvulnerabilitiesrequestpaginatetypedef)
