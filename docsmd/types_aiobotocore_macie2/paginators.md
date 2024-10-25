# Paginators

> [Index](../README.md) > [Macie2](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Macie2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
    type annotations stubs module [types-aiobotocore-macie2](https://pypi.org/project/types-aiobotocore-macie2/).

## DescribeBucketsPaginator

Type annotations and code completion for `#!python session.create_client("macie2").get_paginator("describe_buckets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.DescribeBuckets)

```python
# DescribeBucketsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_macie2.paginator import DescribeBucketsPaginator

session = get_session()
async with session.create_client("macie2") as client:  # (1)
    paginator: DescribeBucketsPaginator = client.get_paginator("describe_buckets")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeBucketsResponseTypeDef
        print(item)  # (3)
```

1. client: [Macie2Client](./client.md)
2. paginator: [DescribeBucketsPaginator](./paginators.md#describebucketspaginator)
3. item: [:material-code-braces: DescribeBucketsResponseTypeDef](./type_defs.md#describebucketsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeBucketsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    criteria: Mapping[str, BucketCriteriaAdditionalPropertiesTypeDef] = ...,  # (1)
    sortCriteria: BucketSortCriteriaTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[DescribeBucketsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: BucketCriteriaAdditionalPropertiesTypeDef](./type_defs.md#bucketcriteriaadditionalpropertiestypedef) 
2. See [:material-code-braces: BucketSortCriteriaTypeDef](./type_defs.md#bucketsortcriteriatypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: DescribeBucketsResponseTypeDef](./type_defs.md#describebucketsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeBucketsRequestDescribeBucketsPaginateTypeDef = {  # (1)
    "criteria": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeBucketsRequestDescribeBucketsPaginateTypeDef](./type_defs.md#describebucketsrequestdescribebucketspaginatetypedef) 
## GetUsageStatisticsPaginator

Type annotations and code completion for `#!python session.create_client("macie2").get_paginator("get_usage_statistics")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.GetUsageStatistics)

```python
# GetUsageStatisticsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_macie2.paginator import GetUsageStatisticsPaginator

session = get_session()
async with session.create_client("macie2") as client:  # (1)
    paginator: GetUsageStatisticsPaginator = client.get_paginator("get_usage_statistics")  # (2)
    async for item in paginator.paginate(...):
        item: GetUsageStatisticsResponseTypeDef
        print(item)  # (3)
```

1. client: [Macie2Client](./client.md)
2. paginator: [GetUsageStatisticsPaginator](./paginators.md#getusagestatisticspaginator)
3. item: [:material-code-braces: GetUsageStatisticsResponseTypeDef](./type_defs.md#getusagestatisticsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetUsageStatisticsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filterBy: Sequence[UsageStatisticsFilterTypeDef] = ...,  # (1)
    sortBy: UsageStatisticsSortByTypeDef = ...,  # (2)
    timeRange: TimeRangeType = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AsyncIterator[GetUsageStatisticsResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-braces: UsageStatisticsFilterTypeDef](./type_defs.md#usagestatisticsfiltertypedef) 
2. See [:material-code-braces: UsageStatisticsSortByTypeDef](./type_defs.md#usagestatisticssortbytypedef) 
3. See [:material-code-brackets: TimeRangeType](./literals.md#timerangetype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: GetUsageStatisticsResponseTypeDef](./type_defs.md#getusagestatisticsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef = {  # (1)
    "filterBy": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef](./type_defs.md#getusagestatisticsrequestgetusagestatisticspaginatetypedef) 
## ListAllowListsPaginator

Type annotations and code completion for `#!python session.create_client("macie2").get_paginator("list_allow_lists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListAllowLists)

```python
# ListAllowListsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_macie2.paginator import ListAllowListsPaginator

session = get_session()
async with session.create_client("macie2") as client:  # (1)
    paginator: ListAllowListsPaginator = client.get_paginator("list_allow_lists")  # (2)
    async for item in paginator.paginate(...):
        item: ListAllowListsResponseTypeDef
        print(item)  # (3)
```

1. client: [Macie2Client](./client.md)
2. paginator: [ListAllowListsPaginator](./paginators.md#listallowlistspaginator)
3. item: [:material-code-braces: ListAllowListsResponseTypeDef](./type_defs.md#listallowlistsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAllowListsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAllowListsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAllowListsResponseTypeDef](./type_defs.md#listallowlistsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAllowListsRequestListAllowListsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAllowListsRequestListAllowListsPaginateTypeDef](./type_defs.md#listallowlistsrequestlistallowlistspaginatetypedef) 
## ListAutomatedDiscoveryAccountsPaginator

Type annotations and code completion for `#!python session.create_client("macie2").get_paginator("list_automated_discovery_accounts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListAutomatedDiscoveryAccounts)

```python
# ListAutomatedDiscoveryAccountsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_macie2.paginator import ListAutomatedDiscoveryAccountsPaginator

session = get_session()
async with session.create_client("macie2") as client:  # (1)
    paginator: ListAutomatedDiscoveryAccountsPaginator = client.get_paginator("list_automated_discovery_accounts")  # (2)
    async for item in paginator.paginate(...):
        item: ListAutomatedDiscoveryAccountsResponseTypeDef
        print(item)  # (3)
```

1. client: [Macie2Client](./client.md)
2. paginator: [ListAutomatedDiscoveryAccountsPaginator](./paginators.md#listautomateddiscoveryaccountspaginator)
3. item: [:material-code-braces: ListAutomatedDiscoveryAccountsResponseTypeDef](./type_defs.md#listautomateddiscoveryaccountsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAutomatedDiscoveryAccountsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    accountIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAutomatedDiscoveryAccountsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAutomatedDiscoveryAccountsResponseTypeDef](./type_defs.md#listautomateddiscoveryaccountsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAutomatedDiscoveryAccountsRequestListAutomatedDiscoveryAccountsPaginateTypeDef = {  # (1)
    "accountIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAutomatedDiscoveryAccountsRequestListAutomatedDiscoveryAccountsPaginateTypeDef](./type_defs.md#listautomateddiscoveryaccountsrequestlistautomateddiscoveryaccountspaginatetypedef) 
## ListClassificationJobsPaginator

Type annotations and code completion for `#!python session.create_client("macie2").get_paginator("list_classification_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListClassificationJobs)

```python
# ListClassificationJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_macie2.paginator import ListClassificationJobsPaginator

session = get_session()
async with session.create_client("macie2") as client:  # (1)
    paginator: ListClassificationJobsPaginator = client.get_paginator("list_classification_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListClassificationJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [Macie2Client](./client.md)
2. paginator: [ListClassificationJobsPaginator](./paginators.md#listclassificationjobspaginator)
3. item: [:material-code-braces: ListClassificationJobsResponseTypeDef](./type_defs.md#listclassificationjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListClassificationJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filterCriteria: ListJobsFilterCriteriaTypeDef = ...,  # (1)
    sortCriteria: ListJobsSortCriteriaTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListClassificationJobsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: ListJobsFilterCriteriaTypeDef](./type_defs.md#listjobsfiltercriteriatypedef) 
2. See [:material-code-braces: ListJobsSortCriteriaTypeDef](./type_defs.md#listjobssortcriteriatypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListClassificationJobsResponseTypeDef](./type_defs.md#listclassificationjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListClassificationJobsRequestListClassificationJobsPaginateTypeDef = {  # (1)
    "filterCriteria": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListClassificationJobsRequestListClassificationJobsPaginateTypeDef](./type_defs.md#listclassificationjobsrequestlistclassificationjobspaginatetypedef) 
## ListClassificationScopesPaginator

Type annotations and code completion for `#!python session.create_client("macie2").get_paginator("list_classification_scopes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListClassificationScopes)

```python
# ListClassificationScopesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_macie2.paginator import ListClassificationScopesPaginator

session = get_session()
async with session.create_client("macie2") as client:  # (1)
    paginator: ListClassificationScopesPaginator = client.get_paginator("list_classification_scopes")  # (2)
    async for item in paginator.paginate(...):
        item: ListClassificationScopesResponseTypeDef
        print(item)  # (3)
```

1. client: [Macie2Client](./client.md)
2. paginator: [ListClassificationScopesPaginator](./paginators.md#listclassificationscopespaginator)
3. item: [:material-code-braces: ListClassificationScopesResponseTypeDef](./type_defs.md#listclassificationscopesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListClassificationScopesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    name: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListClassificationScopesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListClassificationScopesResponseTypeDef](./type_defs.md#listclassificationscopesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListClassificationScopesRequestListClassificationScopesPaginateTypeDef = {  # (1)
    "name": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListClassificationScopesRequestListClassificationScopesPaginateTypeDef](./type_defs.md#listclassificationscopesrequestlistclassificationscopespaginatetypedef) 
## ListCustomDataIdentifiersPaginator

Type annotations and code completion for `#!python session.create_client("macie2").get_paginator("list_custom_data_identifiers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListCustomDataIdentifiers)

```python
# ListCustomDataIdentifiersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_macie2.paginator import ListCustomDataIdentifiersPaginator

session = get_session()
async with session.create_client("macie2") as client:  # (1)
    paginator: ListCustomDataIdentifiersPaginator = client.get_paginator("list_custom_data_identifiers")  # (2)
    async for item in paginator.paginate(...):
        item: ListCustomDataIdentifiersResponseTypeDef
        print(item)  # (3)
```

1. client: [Macie2Client](./client.md)
2. paginator: [ListCustomDataIdentifiersPaginator](./paginators.md#listcustomdataidentifierspaginator)
3. item: [:material-code-braces: ListCustomDataIdentifiersResponseTypeDef](./type_defs.md#listcustomdataidentifiersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCustomDataIdentifiersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListCustomDataIdentifiersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCustomDataIdentifiersResponseTypeDef](./type_defs.md#listcustomdataidentifiersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef](./type_defs.md#listcustomdataidentifiersrequestlistcustomdataidentifierspaginatetypedef) 
## ListFindingsPaginator

Type annotations and code completion for `#!python session.create_client("macie2").get_paginator("list_findings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListFindings)

```python
# ListFindingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_macie2.paginator import ListFindingsPaginator

session = get_session()
async with session.create_client("macie2") as client:  # (1)
    paginator: ListFindingsPaginator = client.get_paginator("list_findings")  # (2)
    async for item in paginator.paginate(...):
        item: ListFindingsResponseTypeDef
        print(item)  # (3)
```

1. client: [Macie2Client](./client.md)
2. paginator: [ListFindingsPaginator](./paginators.md#listfindingspaginator)
3. item: [:material-code-braces: ListFindingsResponseTypeDef](./type_defs.md#listfindingsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFindingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    findingCriteria: FindingCriteriaTypeDef = ...,  # (1)
    sortCriteria: SortCriteriaTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListFindingsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: FindingCriteriaTypeDef](./type_defs.md#findingcriteriatypedef) 
2. See [:material-code-braces: SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListFindingsResponseTypeDef](./type_defs.md#listfindingsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFindingsRequestListFindingsPaginateTypeDef = {  # (1)
    "findingCriteria": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFindingsRequestListFindingsPaginateTypeDef](./type_defs.md#listfindingsrequestlistfindingspaginatetypedef) 
## ListFindingsFiltersPaginator

Type annotations and code completion for `#!python session.create_client("macie2").get_paginator("list_findings_filters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListFindingsFilters)

```python
# ListFindingsFiltersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_macie2.paginator import ListFindingsFiltersPaginator

session = get_session()
async with session.create_client("macie2") as client:  # (1)
    paginator: ListFindingsFiltersPaginator = client.get_paginator("list_findings_filters")  # (2)
    async for item in paginator.paginate(...):
        item: ListFindingsFiltersResponseTypeDef
        print(item)  # (3)
```

1. client: [Macie2Client](./client.md)
2. paginator: [ListFindingsFiltersPaginator](./paginators.md#listfindingsfilterspaginator)
3. item: [:material-code-braces: ListFindingsFiltersResponseTypeDef](./type_defs.md#listfindingsfiltersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFindingsFiltersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListFindingsFiltersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFindingsFiltersResponseTypeDef](./type_defs.md#listfindingsfiltersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef](./type_defs.md#listfindingsfiltersrequestlistfindingsfilterspaginatetypedef) 
## ListInvitationsPaginator

Type annotations and code completion for `#!python session.create_client("macie2").get_paginator("list_invitations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListInvitations)

```python
# ListInvitationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_macie2.paginator import ListInvitationsPaginator

session = get_session()
async with session.create_client("macie2") as client:  # (1)
    paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")  # (2)
    async for item in paginator.paginate(...):
        item: ListInvitationsResponseTypeDef
        print(item)  # (3)
```

1. client: [Macie2Client](./client.md)
2. paginator: [ListInvitationsPaginator](./paginators.md#listinvitationspaginator)
3. item: [:material-code-braces: ListInvitationsResponseTypeDef](./type_defs.md#listinvitationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListInvitationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListInvitationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListInvitationsResponseTypeDef](./type_defs.md#listinvitationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListInvitationsRequestListInvitationsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInvitationsRequestListInvitationsPaginateTypeDef](./type_defs.md#listinvitationsrequestlistinvitationspaginatetypedef) 
## ListManagedDataIdentifiersPaginator

Type annotations and code completion for `#!python session.create_client("macie2").get_paginator("list_managed_data_identifiers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListManagedDataIdentifiers)

```python
# ListManagedDataIdentifiersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_macie2.paginator import ListManagedDataIdentifiersPaginator

session = get_session()
async with session.create_client("macie2") as client:  # (1)
    paginator: ListManagedDataIdentifiersPaginator = client.get_paginator("list_managed_data_identifiers")  # (2)
    async for item in paginator.paginate(...):
        item: ListManagedDataIdentifiersResponseTypeDef
        print(item)  # (3)
```

1. client: [Macie2Client](./client.md)
2. paginator: [ListManagedDataIdentifiersPaginator](./paginators.md#listmanageddataidentifierspaginator)
3. item: [:material-code-braces: ListManagedDataIdentifiersResponseTypeDef](./type_defs.md#listmanageddataidentifiersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListManagedDataIdentifiersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListManagedDataIdentifiersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListManagedDataIdentifiersResponseTypeDef](./type_defs.md#listmanageddataidentifiersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef](./type_defs.md#listmanageddataidentifiersrequestlistmanageddataidentifierspaginatetypedef) 
## ListMembersPaginator

Type annotations and code completion for `#!python session.create_client("macie2").get_paginator("list_members")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListMembers)

```python
# ListMembersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_macie2.paginator import ListMembersPaginator

session = get_session()
async with session.create_client("macie2") as client:  # (1)
    paginator: ListMembersPaginator = client.get_paginator("list_members")  # (2)
    async for item in paginator.paginate(...):
        item: ListMembersResponseTypeDef
        print(item)  # (3)
```

1. client: [Macie2Client](./client.md)
2. paginator: [ListMembersPaginator](./paginators.md#listmemberspaginator)
3. item: [:material-code-braces: ListMembersResponseTypeDef](./type_defs.md#listmembersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListMembersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    onlyAssociated: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListMembersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMembersResponseTypeDef](./type_defs.md#listmembersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMembersRequestListMembersPaginateTypeDef = {  # (1)
    "onlyAssociated": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMembersRequestListMembersPaginateTypeDef](./type_defs.md#listmembersrequestlistmemberspaginatetypedef) 
## ListOrganizationAdminAccountsPaginator

Type annotations and code completion for `#!python session.create_client("macie2").get_paginator("list_organization_admin_accounts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListOrganizationAdminAccounts)

```python
# ListOrganizationAdminAccountsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_macie2.paginator import ListOrganizationAdminAccountsPaginator

session = get_session()
async with session.create_client("macie2") as client:  # (1)
    paginator: ListOrganizationAdminAccountsPaginator = client.get_paginator("list_organization_admin_accounts")  # (2)
    async for item in paginator.paginate(...):
        item: ListOrganizationAdminAccountsResponseTypeDef
        print(item)  # (3)
```

1. client: [Macie2Client](./client.md)
2. paginator: [ListOrganizationAdminAccountsPaginator](./paginators.md#listorganizationadminaccountspaginator)
3. item: [:material-code-braces: ListOrganizationAdminAccountsResponseTypeDef](./type_defs.md#listorganizationadminaccountsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListOrganizationAdminAccountsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListOrganizationAdminAccountsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListOrganizationAdminAccountsResponseTypeDef](./type_defs.md#listorganizationadminaccountsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef](./type_defs.md#listorganizationadminaccountsrequestlistorganizationadminaccountspaginatetypedef) 
## ListResourceProfileArtifactsPaginator

Type annotations and code completion for `#!python session.create_client("macie2").get_paginator("list_resource_profile_artifacts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListResourceProfileArtifacts)

```python
# ListResourceProfileArtifactsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_macie2.paginator import ListResourceProfileArtifactsPaginator

session = get_session()
async with session.create_client("macie2") as client:  # (1)
    paginator: ListResourceProfileArtifactsPaginator = client.get_paginator("list_resource_profile_artifacts")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourceProfileArtifactsResponseTypeDef
        print(item)  # (3)
```

1. client: [Macie2Client](./client.md)
2. paginator: [ListResourceProfileArtifactsPaginator](./paginators.md#listresourceprofileartifactspaginator)
3. item: [:material-code-braces: ListResourceProfileArtifactsResponseTypeDef](./type_defs.md#listresourceprofileartifactsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListResourceProfileArtifactsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    resourceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListResourceProfileArtifactsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListResourceProfileArtifactsResponseTypeDef](./type_defs.md#listresourceprofileartifactsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef](./type_defs.md#listresourceprofileartifactsrequestlistresourceprofileartifactspaginatetypedef) 
## ListResourceProfileDetectionsPaginator

Type annotations and code completion for `#!python session.create_client("macie2").get_paginator("list_resource_profile_detections")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListResourceProfileDetections)

```python
# ListResourceProfileDetectionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_macie2.paginator import ListResourceProfileDetectionsPaginator

session = get_session()
async with session.create_client("macie2") as client:  # (1)
    paginator: ListResourceProfileDetectionsPaginator = client.get_paginator("list_resource_profile_detections")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourceProfileDetectionsResponseTypeDef
        print(item)  # (3)
```

1. client: [Macie2Client](./client.md)
2. paginator: [ListResourceProfileDetectionsPaginator](./paginators.md#listresourceprofiledetectionspaginator)
3. item: [:material-code-braces: ListResourceProfileDetectionsResponseTypeDef](./type_defs.md#listresourceprofiledetectionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListResourceProfileDetectionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    resourceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListResourceProfileDetectionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListResourceProfileDetectionsResponseTypeDef](./type_defs.md#listresourceprofiledetectionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef](./type_defs.md#listresourceprofiledetectionsrequestlistresourceprofiledetectionspaginatetypedef) 
## ListSensitivityInspectionTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("macie2").get_paginator("list_sensitivity_inspection_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListSensitivityInspectionTemplates)

```python
# ListSensitivityInspectionTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_macie2.paginator import ListSensitivityInspectionTemplatesPaginator

session = get_session()
async with session.create_client("macie2") as client:  # (1)
    paginator: ListSensitivityInspectionTemplatesPaginator = client.get_paginator("list_sensitivity_inspection_templates")  # (2)
    async for item in paginator.paginate(...):
        item: ListSensitivityInspectionTemplatesResponseTypeDef
        print(item)  # (3)
```

1. client: [Macie2Client](./client.md)
2. paginator: [ListSensitivityInspectionTemplatesPaginator](./paginators.md#listsensitivityinspectiontemplatespaginator)
3. item: [:material-code-braces: ListSensitivityInspectionTemplatesResponseTypeDef](./type_defs.md#listsensitivityinspectiontemplatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSensitivityInspectionTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSensitivityInspectionTemplatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSensitivityInspectionTemplatesResponseTypeDef](./type_defs.md#listsensitivityinspectiontemplatesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef](./type_defs.md#listsensitivityinspectiontemplatesrequestlistsensitivityinspectiontemplatespaginatetypedef) 
## SearchResourcesPaginator

Type annotations and code completion for `#!python session.create_client("macie2").get_paginator("search_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.SearchResources)

```python
# SearchResourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_macie2.paginator import SearchResourcesPaginator

session = get_session()
async with session.create_client("macie2") as client:  # (1)
    paginator: SearchResourcesPaginator = client.get_paginator("search_resources")  # (2)
    async for item in paginator.paginate(...):
        item: SearchResourcesResponseTypeDef
        print(item)  # (3)
```

1. client: [Macie2Client](./client.md)
2. paginator: [SearchResourcesPaginator](./paginators.md#searchresourcespaginator)
3. item: [:material-code-braces: SearchResourcesResponseTypeDef](./type_defs.md#searchresourcesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SearchResourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    bucketCriteria: SearchResourcesBucketCriteriaTypeDef = ...,  # (1)
    sortCriteria: SearchResourcesSortCriteriaTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[SearchResourcesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: SearchResourcesBucketCriteriaTypeDef](./type_defs.md#searchresourcesbucketcriteriatypedef) 
2. See [:material-code-braces: SearchResourcesSortCriteriaTypeDef](./type_defs.md#searchresourcessortcriteriatypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: SearchResourcesResponseTypeDef](./type_defs.md#searchresourcesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: SearchResourcesRequestSearchResourcesPaginateTypeDef = {  # (1)
    "bucketCriteria": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchResourcesRequestSearchResourcesPaginateTypeDef](./type_defs.md#searchresourcesrequestsearchresourcespaginatetypedef) 
