# Paginators

> [Index](../README.md) > [GuardDuty](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [GuardDuty](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#guardduty)
    type annotations stubs module [types-aiobotocore-guardduty](https://pypi.org/project/types-aiobotocore-guardduty/).

## DescribeMalwareScansPaginator

Type annotations and code completion for `#!python session.create_client("guardduty").get_paginator("describe_malware_scans")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty/paginator/DescribeMalwareScans.html#GuardDuty.Paginator.DescribeMalwareScans)

```python
# DescribeMalwareScansPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_guardduty.paginator import DescribeMalwareScansPaginator

session = get_session()
async with session.create_client("guardduty") as client:  # (1)
    paginator: DescribeMalwareScansPaginator = client.get_paginator("describe_malware_scans")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeMalwareScansResponseTypeDef
        print(item)  # (3)
```

1. client: [GuardDutyClient](./client.md)
2. paginator: [DescribeMalwareScansPaginator](./paginators.md#describemalwarescanspaginator)
3. item: `AioPageIterator[DescribeMalwareScansResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeMalwareScansPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DetectorId: str,
    FilterCriteria: FilterCriteriaTypeDef = ...,  # (1)
    SortCriteria: SortCriteriaTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[DescribeMalwareScansResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef)
2. See [:material-code-braces: SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[DescribeMalwareScansResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeMalwareScansRequestPaginateTypeDef = {  # (1)
    "DetectorId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeMalwareScansRequestPaginateTypeDef](./type_defs.md#describemalwarescansrequestpaginatetypedef)
## ListCoveragePaginator

Type annotations and code completion for `#!python session.create_client("guardduty").get_paginator("list_coverage")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty/paginator/ListCoverage.html#GuardDuty.Paginator.ListCoverage)

```python
# ListCoveragePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_guardduty.paginator import ListCoveragePaginator

session = get_session()
async with session.create_client("guardduty") as client:  # (1)
    paginator: ListCoveragePaginator = client.get_paginator("list_coverage")  # (2)
    async for item in paginator.paginate(...):
        item: ListCoverageResponseTypeDef
        print(item)  # (3)
```

1. client: [GuardDutyClient](./client.md)
2. paginator: [ListCoveragePaginator](./paginators.md#listcoveragepaginator)
3. item: `AioPageIterator[ListCoverageResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCoveragePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DetectorId: str,
    FilterCriteria: CoverageFilterCriteriaTypeDef = ...,  # (1)
    SortCriteria: CoverageSortCriteriaTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListCoverageResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: CoverageFilterCriteriaTypeDef](./type_defs.md#coveragefiltercriteriatypedef)
2. See [:material-code-braces: CoverageSortCriteriaTypeDef](./type_defs.md#coveragesortcriteriatypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListCoverageResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCoverageRequestPaginateTypeDef = {  # (1)
    "DetectorId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCoverageRequestPaginateTypeDef](./type_defs.md#listcoveragerequestpaginatetypedef)
## ListDetectorsPaginator

Type annotations and code completion for `#!python session.create_client("guardduty").get_paginator("list_detectors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty/paginator/ListDetectors.html#GuardDuty.Paginator.ListDetectors)

```python
# ListDetectorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_guardduty.paginator import ListDetectorsPaginator

session = get_session()
async with session.create_client("guardduty") as client:  # (1)
    paginator: ListDetectorsPaginator = client.get_paginator("list_detectors")  # (2)
    async for item in paginator.paginate(...):
        item: ListDetectorsResponseTypeDef
        print(item)  # (3)
```

1. client: [GuardDutyClient](./client.md)
2. paginator: [ListDetectorsPaginator](./paginators.md#listdetectorspaginator)
3. item: `AioPageIterator[ListDetectorsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDetectorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDetectorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDetectorsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDetectorsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDetectorsRequestPaginateTypeDef](./type_defs.md#listdetectorsrequestpaginatetypedef)
## ListFiltersPaginator

Type annotations and code completion for `#!python session.create_client("guardduty").get_paginator("list_filters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty/paginator/ListFilters.html#GuardDuty.Paginator.ListFilters)

```python
# ListFiltersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_guardduty.paginator import ListFiltersPaginator

session = get_session()
async with session.create_client("guardduty") as client:  # (1)
    paginator: ListFiltersPaginator = client.get_paginator("list_filters")  # (2)
    async for item in paginator.paginate(...):
        item: ListFiltersResponseTypeDef
        print(item)  # (3)
```

1. client: [GuardDutyClient](./client.md)
2. paginator: [ListFiltersPaginator](./paginators.md#listfilterspaginator)
3. item: `AioPageIterator[ListFiltersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFiltersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DetectorId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListFiltersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListFiltersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFiltersRequestPaginateTypeDef = {  # (1)
    "DetectorId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFiltersRequestPaginateTypeDef](./type_defs.md#listfiltersrequestpaginatetypedef)
## ListFindingsPaginator

Type annotations and code completion for `#!python session.create_client("guardduty").get_paginator("list_findings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty/paginator/ListFindings.html#GuardDuty.Paginator.ListFindings)

```python
# ListFindingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_guardduty.paginator import ListFindingsPaginator

session = get_session()
async with session.create_client("guardduty") as client:  # (1)
    paginator: ListFindingsPaginator = client.get_paginator("list_findings")  # (2)
    async for item in paginator.paginate(...):
        item: ListFindingsResponseTypeDef
        print(item)  # (3)
```

1. client: [GuardDutyClient](./client.md)
2. paginator: [ListFindingsPaginator](./paginators.md#listfindingspaginator)
3. item: `AioPageIterator[ListFindingsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFindingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DetectorId: str,
    FindingCriteria: FindingCriteriaUnionTypeDef = ...,  # (1)
    SortCriteria: SortCriteriaTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListFindingsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: FindingCriteriaUnionTypeDef](#findingcriteriauniontypedef)
2. See [:material-code-braces: SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListFindingsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFindingsRequestPaginateTypeDef = {  # (1)
    "DetectorId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFindingsRequestPaginateTypeDef](./type_defs.md#listfindingsrequestpaginatetypedef)
## ListIPSetsPaginator

Type annotations and code completion for `#!python session.create_client("guardduty").get_paginator("list_ip_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty/paginator/ListIPSets.html#GuardDuty.Paginator.ListIPSets)

```python
# ListIPSetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_guardduty.paginator import ListIPSetsPaginator

session = get_session()
async with session.create_client("guardduty") as client:  # (1)
    paginator: ListIPSetsPaginator = client.get_paginator("list_ip_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListIPSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [GuardDutyClient](./client.md)
2. paginator: [ListIPSetsPaginator](./paginators.md#listipsetspaginator)
3. item: `AioPageIterator[ListIPSetsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListIPSetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DetectorId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListIPSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListIPSetsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListIPSetsRequestPaginateTypeDef = {  # (1)
    "DetectorId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIPSetsRequestPaginateTypeDef](./type_defs.md#listipsetsrequestpaginatetypedef)
## ListInvitationsPaginator

Type annotations and code completion for `#!python session.create_client("guardduty").get_paginator("list_invitations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty/paginator/ListInvitations.html#GuardDuty.Paginator.ListInvitations)

```python
# ListInvitationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_guardduty.paginator import ListInvitationsPaginator

session = get_session()
async with session.create_client("guardduty") as client:  # (1)
    paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")  # (2)
    async for item in paginator.paginate(...):
        item: ListInvitationsResponseTypeDef
        print(item)  # (3)
```

1. client: [GuardDutyClient](./client.md)
2. paginator: [ListInvitationsPaginator](./paginators.md#listinvitationspaginator)
3. item: `AioPageIterator[ListInvitationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListInvitationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListInvitationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListInvitationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListInvitationsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInvitationsRequestPaginateTypeDef](./type_defs.md#listinvitationsrequestpaginatetypedef)
## ListMalwareScansPaginator

Type annotations and code completion for `#!python session.create_client("guardduty").get_paginator("list_malware_scans")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty/paginator/ListMalwareScans.html#GuardDuty.Paginator.ListMalwareScans)

```python
# ListMalwareScansPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_guardduty.paginator import ListMalwareScansPaginator

session = get_session()
async with session.create_client("guardduty") as client:  # (1)
    paginator: ListMalwareScansPaginator = client.get_paginator("list_malware_scans")  # (2)
    async for item in paginator.paginate(...):
        item: ListMalwareScansResponseTypeDef
        print(item)  # (3)
```

1. client: [GuardDutyClient](./client.md)
2. paginator: [ListMalwareScansPaginator](./paginators.md#listmalwarescanspaginator)
3. item: `AioPageIterator[ListMalwareScansResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListMalwareScansPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FilterCriteria: ListMalwareScansFilterCriteriaTypeDef = ...,  # (1)
    SortCriteria: SortCriteriaTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListMalwareScansResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: ListMalwareScansFilterCriteriaTypeDef](./type_defs.md#listmalwarescansfiltercriteriatypedef)
2. See [:material-code-braces: SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListMalwareScansResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListMalwareScansRequestPaginateTypeDef = {  # (1)
    "FilterCriteria": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMalwareScansRequestPaginateTypeDef](./type_defs.md#listmalwarescansrequestpaginatetypedef)
## ListMembersPaginator

Type annotations and code completion for `#!python session.create_client("guardduty").get_paginator("list_members")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty/paginator/ListMembers.html#GuardDuty.Paginator.ListMembers)

```python
# ListMembersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_guardduty.paginator import ListMembersPaginator

session = get_session()
async with session.create_client("guardduty") as client:  # (1)
    paginator: ListMembersPaginator = client.get_paginator("list_members")  # (2)
    async for item in paginator.paginate(...):
        item: ListMembersResponseTypeDef
        print(item)  # (3)
```

1. client: [GuardDutyClient](./client.md)
2. paginator: [ListMembersPaginator](./paginators.md#listmemberspaginator)
3. item: `AioPageIterator[ListMembersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListMembersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DetectorId: str,
    OnlyAssociated: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListMembersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListMembersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListMembersRequestPaginateTypeDef = {  # (1)
    "DetectorId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMembersRequestPaginateTypeDef](./type_defs.md#listmembersrequestpaginatetypedef)
## ListOrganizationAdminAccountsPaginator

Type annotations and code completion for `#!python session.create_client("guardduty").get_paginator("list_organization_admin_accounts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty/paginator/ListOrganizationAdminAccounts.html#GuardDuty.Paginator.ListOrganizationAdminAccounts)

```python
# ListOrganizationAdminAccountsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_guardduty.paginator import ListOrganizationAdminAccountsPaginator

session = get_session()
async with session.create_client("guardduty") as client:  # (1)
    paginator: ListOrganizationAdminAccountsPaginator = client.get_paginator("list_organization_admin_accounts")  # (2)
    async for item in paginator.paginate(...):
        item: ListOrganizationAdminAccountsResponseTypeDef
        print(item)  # (3)
```

1. client: [GuardDutyClient](./client.md)
2. paginator: [ListOrganizationAdminAccountsPaginator](./paginators.md#listorganizationadminaccountspaginator)
3. item: `AioPageIterator[ListOrganizationAdminAccountsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListOrganizationAdminAccountsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListOrganizationAdminAccountsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListOrganizationAdminAccountsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListOrganizationAdminAccountsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOrganizationAdminAccountsRequestPaginateTypeDef](./type_defs.md#listorganizationadminaccountsrequestpaginatetypedef)
## ListThreatEntitySetsPaginator

Type annotations and code completion for `#!python session.create_client("guardduty").get_paginator("list_threat_entity_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty/paginator/ListThreatEntitySets.html#GuardDuty.Paginator.ListThreatEntitySets)

```python
# ListThreatEntitySetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_guardduty.paginator import ListThreatEntitySetsPaginator

session = get_session()
async with session.create_client("guardduty") as client:  # (1)
    paginator: ListThreatEntitySetsPaginator = client.get_paginator("list_threat_entity_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListThreatEntitySetsResponseTypeDef
        print(item)  # (3)
```

1. client: [GuardDutyClient](./client.md)
2. paginator: [ListThreatEntitySetsPaginator](./paginators.md#listthreatentitysetspaginator)
3. item: `AioPageIterator[ListThreatEntitySetsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListThreatEntitySetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DetectorId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListThreatEntitySetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListThreatEntitySetsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListThreatEntitySetsRequestPaginateTypeDef = {  # (1)
    "DetectorId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListThreatEntitySetsRequestPaginateTypeDef](./type_defs.md#listthreatentitysetsrequestpaginatetypedef)
## ListThreatIntelSetsPaginator

Type annotations and code completion for `#!python session.create_client("guardduty").get_paginator("list_threat_intel_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty/paginator/ListThreatIntelSets.html#GuardDuty.Paginator.ListThreatIntelSets)

```python
# ListThreatIntelSetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_guardduty.paginator import ListThreatIntelSetsPaginator

session = get_session()
async with session.create_client("guardduty") as client:  # (1)
    paginator: ListThreatIntelSetsPaginator = client.get_paginator("list_threat_intel_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListThreatIntelSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [GuardDutyClient](./client.md)
2. paginator: [ListThreatIntelSetsPaginator](./paginators.md#listthreatintelsetspaginator)
3. item: `AioPageIterator[ListThreatIntelSetsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListThreatIntelSetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DetectorId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListThreatIntelSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListThreatIntelSetsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListThreatIntelSetsRequestPaginateTypeDef = {  # (1)
    "DetectorId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListThreatIntelSetsRequestPaginateTypeDef](./type_defs.md#listthreatintelsetsrequestpaginatetypedef)
## ListTrustedEntitySetsPaginator

Type annotations and code completion for `#!python session.create_client("guardduty").get_paginator("list_trusted_entity_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty/paginator/ListTrustedEntitySets.html#GuardDuty.Paginator.ListTrustedEntitySets)

```python
# ListTrustedEntitySetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_guardduty.paginator import ListTrustedEntitySetsPaginator

session = get_session()
async with session.create_client("guardduty") as client:  # (1)
    paginator: ListTrustedEntitySetsPaginator = client.get_paginator("list_trusted_entity_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListTrustedEntitySetsResponseTypeDef
        print(item)  # (3)
```

1. client: [GuardDutyClient](./client.md)
2. paginator: [ListTrustedEntitySetsPaginator](./paginators.md#listtrustedentitysetspaginator)
3. item: `AioPageIterator[ListTrustedEntitySetsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTrustedEntitySetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DetectorId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTrustedEntitySetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTrustedEntitySetsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTrustedEntitySetsRequestPaginateTypeDef = {  # (1)
    "DetectorId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTrustedEntitySetsRequestPaginateTypeDef](./type_defs.md#listtrustedentitysetsrequestpaginatetypedef)
