<a id="paginators-for-aiobotocore-securityhub-module"></a>

# Paginators for aiobotocore SecurityHub module

> [Index](..) > [SecurityHub](.) > Paginators

Auto-generated documentation for
[SecurityHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
type annotations stubs module
[types-aiobotocore-securityhub](https://pypi.org/project/types-aiobotocore-securityhub/).

- [Paginators for aiobotocore SecurityHub module](#paginators-for-aiobotocore-securityhub-module)
  - [DescribeActionTargetsPaginator](#describeactiontargetspaginator)
  - [DescribeProductsPaginator](#describeproductspaginator)
  - [DescribeStandardsPaginator](#describestandardspaginator)
  - [DescribeStandardsControlsPaginator](#describestandardscontrolspaginator)
  - [GetEnabledStandardsPaginator](#getenabledstandardspaginator)
  - [GetFindingsPaginator](#getfindingspaginator)
  - [GetInsightsPaginator](#getinsightspaginator)
  - [ListEnabledProductsForImportPaginator](#listenabledproductsforimportpaginator)
  - [ListFindingAggregatorsPaginator](#listfindingaggregatorspaginator)
  - [ListInvitationsPaginator](#listinvitationspaginator)
  - [ListMembersPaginator](#listmemberspaginator)
  - [ListOrganizationAdminAccountsPaginator](#listorganizationadminaccountspaginator)

<a id="describeactiontargetspaginator"></a>

## DescribeActionTargetsPaginator

Type annotations for
`session.create_client("securityhub").get_paginator("describe_action_targets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_securityhub.paginator import DescribeActionTargetsPaginator

session = get_session()
async with session.create_client("securityhub") as client:
    client: SecurityHubClient
    paginator: DescribeActionTargetsPaginator = client.get_paginator("describe_action_targets")
```

Boto3 documentation:
[SecurityHub.Paginator.DescribeActionTargets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeActionTargets)

Arguments for `DescribeActionTargetsPaginator.paginate` method:

- `ActionTargetArns`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeActionTargetsPaginator.paginate` returns
`AsyncIterable`\[[DescribeActionTargetsResponseTypeDef](./type_defs.md#describeactiontargetsresponsetypedef)\].

<a id="describeproductspaginator"></a>

## DescribeProductsPaginator

Type annotations for
`session.create_client("securityhub").get_paginator("describe_products")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_securityhub.paginator import DescribeProductsPaginator

session = get_session()
async with session.create_client("securityhub") as client:
    client: SecurityHubClient
    paginator: DescribeProductsPaginator = client.get_paginator("describe_products")
```

Boto3 documentation:
[SecurityHub.Paginator.DescribeProducts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeProducts)

Arguments for `DescribeProductsPaginator.paginate` method:

- `ProductArn`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeProductsPaginator.paginate` returns
`AsyncIterable`\[[DescribeProductsResponseTypeDef](./type_defs.md#describeproductsresponsetypedef)\].

<a id="describestandardspaginator"></a>

## DescribeStandardsPaginator

Type annotations for
`session.create_client("securityhub").get_paginator("describe_standards")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_securityhub.paginator import DescribeStandardsPaginator

session = get_session()
async with session.create_client("securityhub") as client:
    client: SecurityHubClient
    paginator: DescribeStandardsPaginator = client.get_paginator("describe_standards")
```

Boto3 documentation:
[SecurityHub.Paginator.DescribeStandards](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandards)

Arguments for `DescribeStandardsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeStandardsPaginator.paginate` returns
`AsyncIterable`\[[DescribeStandardsResponseTypeDef](./type_defs.md#describestandardsresponsetypedef)\].

<a id="describestandardscontrolspaginator"></a>

## DescribeStandardsControlsPaginator

Type annotations for
`session.create_client("securityhub").get_paginator("describe_standards_controls")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_securityhub.paginator import DescribeStandardsControlsPaginator

session = get_session()
async with session.create_client("securityhub") as client:
    client: SecurityHubClient
    paginator: DescribeStandardsControlsPaginator = client.get_paginator("describe_standards_controls")
```

Boto3 documentation:
[SecurityHub.Paginator.DescribeStandardsControls](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.DescribeStandardsControls)

Arguments for `DescribeStandardsControlsPaginator.paginate` method:

- `StandardsSubscriptionArn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeStandardsControlsPaginator.paginate` returns
`AsyncIterable`\[[DescribeStandardsControlsResponseTypeDef](./type_defs.md#describestandardscontrolsresponsetypedef)\].

<a id="getenabledstandardspaginator"></a>

## GetEnabledStandardsPaginator

Type annotations for
`session.create_client("securityhub").get_paginator("get_enabled_standards")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_securityhub.paginator import GetEnabledStandardsPaginator

session = get_session()
async with session.create_client("securityhub") as client:
    client: SecurityHubClient
    paginator: GetEnabledStandardsPaginator = client.get_paginator("get_enabled_standards")
```

Boto3 documentation:
[SecurityHub.Paginator.GetEnabledStandards](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetEnabledStandards)

Arguments for `GetEnabledStandardsPaginator.paginate` method:

- `StandardsSubscriptionArns`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetEnabledStandardsPaginator.paginate` returns
`AsyncIterable`\[[GetEnabledStandardsResponseTypeDef](./type_defs.md#getenabledstandardsresponsetypedef)\].

<a id="getfindingspaginator"></a>

## GetFindingsPaginator

Type annotations for
`session.create_client("securityhub").get_paginator("get_findings")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_securityhub.paginator import GetFindingsPaginator

session = get_session()
async with session.create_client("securityhub") as client:
    client: SecurityHubClient
    paginator: GetFindingsPaginator = client.get_paginator("get_findings")
```

Boto3 documentation:
[SecurityHub.Paginator.GetFindings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetFindings)

Arguments for `GetFindingsPaginator.paginate` method:

- `Filters`:
  [AwsSecurityFindingFiltersTypeDef](./type_defs.md#awssecurityfindingfilterstypedef)
- `SortCriteria`:
  `Sequence`\[[SortCriterionTypeDef](./type_defs.md#sortcriteriontypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetFindingsPaginator.paginate` returns
`AsyncIterable`\[[GetFindingsResponseTypeDef](./type_defs.md#getfindingsresponsetypedef)\].

<a id="getinsightspaginator"></a>

## GetInsightsPaginator

Type annotations for
`session.create_client("securityhub").get_paginator("get_insights")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_securityhub.paginator import GetInsightsPaginator

session = get_session()
async with session.create_client("securityhub") as client:
    client: SecurityHubClient
    paginator: GetInsightsPaginator = client.get_paginator("get_insights")
```

Boto3 documentation:
[SecurityHub.Paginator.GetInsights](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.GetInsights)

Arguments for `GetInsightsPaginator.paginate` method:

- `InsightArns`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetInsightsPaginator.paginate` returns
`AsyncIterable`\[[GetInsightsResponseTypeDef](./type_defs.md#getinsightsresponsetypedef)\].

<a id="listenabledproductsforimportpaginator"></a>

## ListEnabledProductsForImportPaginator

Type annotations for
`session.create_client("securityhub").get_paginator("list_enabled_products_for_import")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_securityhub.paginator import ListEnabledProductsForImportPaginator

session = get_session()
async with session.create_client("securityhub") as client:
    client: SecurityHubClient
    paginator: ListEnabledProductsForImportPaginator = client.get_paginator("list_enabled_products_for_import")
```

Boto3 documentation:
[SecurityHub.Paginator.ListEnabledProductsForImport](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListEnabledProductsForImport)

Arguments for `ListEnabledProductsForImportPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListEnabledProductsForImportPaginator.paginate` returns
`AsyncIterable`\[[ListEnabledProductsForImportResponseTypeDef](./type_defs.md#listenabledproductsforimportresponsetypedef)\].

<a id="listfindingaggregatorspaginator"></a>

## ListFindingAggregatorsPaginator

Type annotations for
`session.create_client("securityhub").get_paginator("list_finding_aggregators")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_securityhub.paginator import ListFindingAggregatorsPaginator

session = get_session()
async with session.create_client("securityhub") as client:
    client: SecurityHubClient
    paginator: ListFindingAggregatorsPaginator = client.get_paginator("list_finding_aggregators")
```

Boto3 documentation:
[SecurityHub.Paginator.ListFindingAggregators](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListFindingAggregators)

Arguments for `ListFindingAggregatorsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListFindingAggregatorsPaginator.paginate` returns
`AsyncIterable`\[[ListFindingAggregatorsResponseTypeDef](./type_defs.md#listfindingaggregatorsresponsetypedef)\].

<a id="listinvitationspaginator"></a>

## ListInvitationsPaginator

Type annotations for
`session.create_client("securityhub").get_paginator("list_invitations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_securityhub.paginator import ListInvitationsPaginator

session = get_session()
async with session.create_client("securityhub") as client:
    client: SecurityHubClient
    paginator: ListInvitationsPaginator = client.get_paginator("list_invitations")
```

Boto3 documentation:
[SecurityHub.Paginator.ListInvitations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListInvitations)

Arguments for `ListInvitationsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListInvitationsPaginator.paginate` returns
`AsyncIterable`\[[ListInvitationsResponseTypeDef](./type_defs.md#listinvitationsresponsetypedef)\].

<a id="listmemberspaginator"></a>

## ListMembersPaginator

Type annotations for
`session.create_client("securityhub").get_paginator("list_members")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_securityhub.paginator import ListMembersPaginator

session = get_session()
async with session.create_client("securityhub") as client:
    client: SecurityHubClient
    paginator: ListMembersPaginator = client.get_paginator("list_members")
```

Boto3 documentation:
[SecurityHub.Paginator.ListMembers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListMembers)

Arguments for `ListMembersPaginator.paginate` method:

- `OnlyAssociated`: `bool`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListMembersPaginator.paginate` returns
`AsyncIterable`\[[ListMembersResponseTypeDef](./type_defs.md#listmembersresponsetypedef)\].

<a id="listorganizationadminaccountspaginator"></a>

## ListOrganizationAdminAccountsPaginator

Type annotations for
`session.create_client("securityhub").get_paginator("list_organization_admin_accounts")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_securityhub.paginator import ListOrganizationAdminAccountsPaginator

session = get_session()
async with session.create_client("securityhub") as client:
    client: SecurityHubClient
    paginator: ListOrganizationAdminAccountsPaginator = client.get_paginator("list_organization_admin_accounts")
```

Boto3 documentation:
[SecurityHub.Paginator.ListOrganizationAdminAccounts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub.Paginator.ListOrganizationAdminAccounts)

Arguments for `ListOrganizationAdminAccountsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListOrganizationAdminAccountsPaginator.paginate` returns
`AsyncIterable`\[[ListOrganizationAdminAccountsResponseTypeDef](./type_defs.md#listorganizationadminaccountsresponsetypedef)\].
