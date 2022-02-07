<a id="paginators-for-aiobotocore-guardduty-module"></a>

# Paginators for aiobotocore GuardDuty module

> [Index](..) > [GuardDuty](.) > Paginators

Auto-generated documentation for
[GuardDuty](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
type annotations stubs module
[types-aiobotocore-guardduty](https://pypi.org/project/types-aiobotocore-guardduty/).

- [Paginators for aiobotocore GuardDuty module](#paginators-for-aiobotocore-guardduty-module)
  - [ListDetectorsPaginator](#listdetectorspaginator)
  - [ListFiltersPaginator](#listfilterspaginator)
  - [ListFindingsPaginator](#listfindingspaginator)
  - [ListIPSetsPaginator](#listipsetspaginator)
  - [ListInvitationsPaginator](#listinvitationspaginator)
  - [ListMembersPaginator](#listmemberspaginator)
  - [ListOrganizationAdminAccountsPaginator](#listorganizationadminaccountspaginator)
  - [ListThreatIntelSetsPaginator](#listthreatintelsetspaginator)

<a id="listdetectorspaginator"></a>

## ListDetectorsPaginator

Type annotations for
`session.create_client("guardduty").get_paginator("list_detectors")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_guardduty.paginator import ListDetectorsPaginator

session = get_session()
async with session.create_client("guardduty") as client:
    client: GuardDutyClient
    paginator: ListDetectorsPaginator = client.get_paginator("list_detectors")
```

Boto3 documentation:
[GuardDuty.Paginator.ListDetectors](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListDetectors)

Arguments for `ListDetectorsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDetectorsPaginator.paginate` returns
`_PageIterator`\[[ListDetectorsResponseTypeDef](./type_defs.md#listdetectorsresponsetypedef)\].

<a id="listfilterspaginator"></a>

## ListFiltersPaginator

Type annotations for
`session.create_client("guardduty").get_paginator("list_filters")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_guardduty.paginator import ListFiltersPaginator

session = get_session()
async with session.create_client("guardduty") as client:
    client: GuardDutyClient
    paginator: ListFiltersPaginator = client.get_paginator("list_filters")
```

Boto3 documentation:
[GuardDuty.Paginator.ListFilters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFilters)

Arguments for `ListFiltersPaginator.paginate` method:

- `DetectorId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListFiltersPaginator.paginate` returns
`_PageIterator`\[[ListFiltersResponseTypeDef](./type_defs.md#listfiltersresponsetypedef)\].

<a id="listfindingspaginator"></a>

## ListFindingsPaginator

Type annotations for
`session.create_client("guardduty").get_paginator("list_findings")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_guardduty.paginator import ListFindingsPaginator

session = get_session()
async with session.create_client("guardduty") as client:
    client: GuardDutyClient
    paginator: ListFindingsPaginator = client.get_paginator("list_findings")
```

Boto3 documentation:
[GuardDuty.Paginator.ListFindings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFindings)

Arguments for `ListFindingsPaginator.paginate` method:

- `DetectorId`: `str` *(required)*
- `FindingCriteria`:
  [FindingCriteriaTypeDef](./type_defs.md#findingcriteriatypedef)
- `SortCriteria`: [SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListFindingsPaginator.paginate` returns
`_PageIterator`\[[ListFindingsResponseTypeDef](./type_defs.md#listfindingsresponsetypedef)\].

<a id="listipsetspaginator"></a>

## ListIPSetsPaginator

Type annotations for
`session.create_client("guardduty").get_paginator("list_ip_sets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_guardduty.paginator import ListIPSetsPaginator

session = get_session()
async with session.create_client("guardduty") as client:
    client: GuardDutyClient
    paginator: ListIPSetsPaginator = client.get_paginator("list_ip_sets")
```

Boto3 documentation:
[GuardDuty.Paginator.ListIPSets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListIPSets)

Arguments for `ListIPSetsPaginator.paginate` method:

- `DetectorId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListIPSetsPaginator.paginate` returns
`_PageIterator`\[[ListIPSetsResponseTypeDef](./type_defs.md#listipsetsresponsetypedef)\].

<a id="listinvitationspaginator"></a>

## ListInvitationsPaginator

Type annotations for
`session.create_client("guardduty").get_paginator("list_invitations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_guardduty.paginator import ListInvitationsPaginator

session = get_session()
async with session.create_client("guardduty") as client:
    client: GuardDutyClient
    paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")
```

Boto3 documentation:
[GuardDuty.Paginator.ListInvitations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListInvitations)

Arguments for `ListInvitationsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListInvitationsPaginator.paginate` returns
`_PageIterator`\[[ListInvitationsResponseTypeDef](./type_defs.md#listinvitationsresponsetypedef)\].

<a id="listmemberspaginator"></a>

## ListMembersPaginator

Type annotations for
`session.create_client("guardduty").get_paginator("list_members")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_guardduty.paginator import ListMembersPaginator

session = get_session()
async with session.create_client("guardduty") as client:
    client: GuardDutyClient
    paginator: ListMembersPaginator = client.get_paginator("list_members")
```

Boto3 documentation:
[GuardDuty.Paginator.ListMembers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListMembers)

Arguments for `ListMembersPaginator.paginate` method:

- `DetectorId`: `str` *(required)*
- `OnlyAssociated`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListMembersPaginator.paginate` returns
`_PageIterator`\[[ListMembersResponseTypeDef](./type_defs.md#listmembersresponsetypedef)\].

<a id="listorganizationadminaccountspaginator"></a>

## ListOrganizationAdminAccountsPaginator

Type annotations for
`session.create_client("guardduty").get_paginator("list_organization_admin_accounts")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_guardduty.paginator import ListOrganizationAdminAccountsPaginator

session = get_session()
async with session.create_client("guardduty") as client:
    client: GuardDutyClient
    paginator: ListOrganizationAdminAccountsPaginator = client.get_paginator("list_organization_admin_accounts")
```

Boto3 documentation:
[GuardDuty.Paginator.ListOrganizationAdminAccounts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListOrganizationAdminAccounts)

Arguments for `ListOrganizationAdminAccountsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListOrganizationAdminAccountsPaginator.paginate` returns
`_PageIterator`\[[ListOrganizationAdminAccountsResponseTypeDef](./type_defs.md#listorganizationadminaccountsresponsetypedef)\].

<a id="listthreatintelsetspaginator"></a>

## ListThreatIntelSetsPaginator

Type annotations for
`session.create_client("guardduty").get_paginator("list_threat_intel_sets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_guardduty.paginator import ListThreatIntelSetsPaginator

session = get_session()
async with session.create_client("guardduty") as client:
    client: GuardDutyClient
    paginator: ListThreatIntelSetsPaginator = client.get_paginator("list_threat_intel_sets")
```

Boto3 documentation:
[GuardDuty.Paginator.ListThreatIntelSets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListThreatIntelSets)

Arguments for `ListThreatIntelSetsPaginator.paginate` method:

- `DetectorId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListThreatIntelSetsPaginator.paginate` returns
`_PageIterator`\[[ListThreatIntelSetsResponseTypeDef](./type_defs.md#listthreatintelsetsresponsetypedef)\].
