<a id="paginators-for-aiobotocore-organizations-module"></a>

# Paginators for aiobotocore Organizations module

> [Index](..) > [Organizations](.) > Paginators

Auto-generated documentation for
[Organizations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations)
type annotations stubs module
[types-aiobotocore-organizations](https://pypi.org/project/types-aiobotocore-organizations/).

- [Paginators for aiobotocore Organizations module](#paginators-for-aiobotocore-organizations-module)
  - [ListAWSServiceAccessForOrganizationPaginator](#listawsserviceaccessfororganizationpaginator)
  - [ListAccountsPaginator](#listaccountspaginator)
  - [ListAccountsForParentPaginator](#listaccountsforparentpaginator)
  - [ListChildrenPaginator](#listchildrenpaginator)
  - [ListCreateAccountStatusPaginator](#listcreateaccountstatuspaginator)
  - [ListDelegatedAdministratorsPaginator](#listdelegatedadministratorspaginator)
  - [ListDelegatedServicesForAccountPaginator](#listdelegatedservicesforaccountpaginator)
  - [ListHandshakesForAccountPaginator](#listhandshakesforaccountpaginator)
  - [ListHandshakesForOrganizationPaginator](#listhandshakesfororganizationpaginator)
  - [ListOrganizationalUnitsForParentPaginator](#listorganizationalunitsforparentpaginator)
  - [ListParentsPaginator](#listparentspaginator)
  - [ListPoliciesPaginator](#listpoliciespaginator)
  - [ListPoliciesForTargetPaginator](#listpoliciesfortargetpaginator)
  - [ListRootsPaginator](#listrootspaginator)
  - [ListTagsForResourcePaginator](#listtagsforresourcepaginator)
  - [ListTargetsForPolicyPaginator](#listtargetsforpolicypaginator)

<a id="listawsserviceaccessfororganizationpaginator"></a>

## ListAWSServiceAccessForOrganizationPaginator

Type annotations for
`session.create_client("organizations").get_paginator("list_aws_service_access_for_organization")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListAWSServiceAccessForOrganizationPaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListAWSServiceAccessForOrganizationPaginator = client.get_paginator("list_aws_service_access_for_organization")
```

Boto3 documentation:
[Organizations.Paginator.ListAWSServiceAccessForOrganization](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListAWSServiceAccessForOrganization)

Arguments for `ListAWSServiceAccessForOrganizationPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAWSServiceAccessForOrganizationPaginator.paginate` returns
`AsyncIterable`\[[ListAWSServiceAccessForOrganizationResponseTypeDef](./type_defs.md#listawsserviceaccessfororganizationresponsetypedef)\].

<a id="listaccountspaginator"></a>

## ListAccountsPaginator

Type annotations for
`session.create_client("organizations").get_paginator("list_accounts")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListAccountsPaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListAccountsPaginator = client.get_paginator("list_accounts")
```

Boto3 documentation:
[Organizations.Paginator.ListAccounts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListAccounts)

Arguments for `ListAccountsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAccountsPaginator.paginate` returns
`AsyncIterable`\[[ListAccountsResponseTypeDef](./type_defs.md#listaccountsresponsetypedef)\].

<a id="listaccountsforparentpaginator"></a>

## ListAccountsForParentPaginator

Type annotations for
`session.create_client("organizations").get_paginator("list_accounts_for_parent")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListAccountsForParentPaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListAccountsForParentPaginator = client.get_paginator("list_accounts_for_parent")
```

Boto3 documentation:
[Organizations.Paginator.ListAccountsForParent](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListAccountsForParent)

Arguments for `ListAccountsForParentPaginator.paginate` method:

- `ParentId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAccountsForParentPaginator.paginate` returns
`AsyncIterable`\[[ListAccountsForParentResponseTypeDef](./type_defs.md#listaccountsforparentresponsetypedef)\].

<a id="listchildrenpaginator"></a>

## ListChildrenPaginator

Type annotations for
`session.create_client("organizations").get_paginator("list_children")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListChildrenPaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListChildrenPaginator = client.get_paginator("list_children")
```

Boto3 documentation:
[Organizations.Paginator.ListChildren](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListChildren)

Arguments for `ListChildrenPaginator.paginate` method:

- `ParentId`: `str` *(required)*
- `ChildType`: [ChildTypeType](./literals.md#childtypetype) *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListChildrenPaginator.paginate` returns
`AsyncIterable`\[[ListChildrenResponseTypeDef](./type_defs.md#listchildrenresponsetypedef)\].

<a id="listcreateaccountstatuspaginator"></a>

## ListCreateAccountStatusPaginator

Type annotations for
`session.create_client("organizations").get_paginator("list_create_account_status")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListCreateAccountStatusPaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListCreateAccountStatusPaginator = client.get_paginator("list_create_account_status")
```

Boto3 documentation:
[Organizations.Paginator.ListCreateAccountStatus](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListCreateAccountStatus)

Arguments for `ListCreateAccountStatusPaginator.paginate` method:

- `States`:
  `Sequence`\[[CreateAccountStateType](./literals.md#createaccountstatetype)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListCreateAccountStatusPaginator.paginate` returns
`AsyncIterable`\[[ListCreateAccountStatusResponseTypeDef](./type_defs.md#listcreateaccountstatusresponsetypedef)\].

<a id="listdelegatedadministratorspaginator"></a>

## ListDelegatedAdministratorsPaginator

Type annotations for
`session.create_client("organizations").get_paginator("list_delegated_administrators")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListDelegatedAdministratorsPaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListDelegatedAdministratorsPaginator = client.get_paginator("list_delegated_administrators")
```

Boto3 documentation:
[Organizations.Paginator.ListDelegatedAdministrators](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListDelegatedAdministrators)

Arguments for `ListDelegatedAdministratorsPaginator.paginate` method:

- `ServicePrincipal`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDelegatedAdministratorsPaginator.paginate` returns
`AsyncIterable`\[[ListDelegatedAdministratorsResponseTypeDef](./type_defs.md#listdelegatedadministratorsresponsetypedef)\].

<a id="listdelegatedservicesforaccountpaginator"></a>

## ListDelegatedServicesForAccountPaginator

Type annotations for
`session.create_client("organizations").get_paginator("list_delegated_services_for_account")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListDelegatedServicesForAccountPaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListDelegatedServicesForAccountPaginator = client.get_paginator("list_delegated_services_for_account")
```

Boto3 documentation:
[Organizations.Paginator.ListDelegatedServicesForAccount](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListDelegatedServicesForAccount)

Arguments for `ListDelegatedServicesForAccountPaginator.paginate` method:

- `AccountId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListDelegatedServicesForAccountPaginator.paginate` returns
`AsyncIterable`\[[ListDelegatedServicesForAccountResponseTypeDef](./type_defs.md#listdelegatedservicesforaccountresponsetypedef)\].

<a id="listhandshakesforaccountpaginator"></a>

## ListHandshakesForAccountPaginator

Type annotations for
`session.create_client("organizations").get_paginator("list_handshakes_for_account")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListHandshakesForAccountPaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListHandshakesForAccountPaginator = client.get_paginator("list_handshakes_for_account")
```

Boto3 documentation:
[Organizations.Paginator.ListHandshakesForAccount](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListHandshakesForAccount)

Arguments for `ListHandshakesForAccountPaginator.paginate` method:

- `Filter`: [HandshakeFilterTypeDef](./type_defs.md#handshakefiltertypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListHandshakesForAccountPaginator.paginate` returns
`AsyncIterable`\[[ListHandshakesForAccountResponseTypeDef](./type_defs.md#listhandshakesforaccountresponsetypedef)\].

<a id="listhandshakesfororganizationpaginator"></a>

## ListHandshakesForOrganizationPaginator

Type annotations for
`session.create_client("organizations").get_paginator("list_handshakes_for_organization")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListHandshakesForOrganizationPaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListHandshakesForOrganizationPaginator = client.get_paginator("list_handshakes_for_organization")
```

Boto3 documentation:
[Organizations.Paginator.ListHandshakesForOrganization](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListHandshakesForOrganization)

Arguments for `ListHandshakesForOrganizationPaginator.paginate` method:

- `Filter`: [HandshakeFilterTypeDef](./type_defs.md#handshakefiltertypedef)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListHandshakesForOrganizationPaginator.paginate` returns
`AsyncIterable`\[[ListHandshakesForOrganizationResponseTypeDef](./type_defs.md#listhandshakesfororganizationresponsetypedef)\].

<a id="listorganizationalunitsforparentpaginator"></a>

## ListOrganizationalUnitsForParentPaginator

Type annotations for
`session.create_client("organizations").get_paginator("list_organizational_units_for_parent")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListOrganizationalUnitsForParentPaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListOrganizationalUnitsForParentPaginator = client.get_paginator("list_organizational_units_for_parent")
```

Boto3 documentation:
[Organizations.Paginator.ListOrganizationalUnitsForParent](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListOrganizationalUnitsForParent)

Arguments for `ListOrganizationalUnitsForParentPaginator.paginate` method:

- `ParentId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListOrganizationalUnitsForParentPaginator.paginate` returns
`AsyncIterable`\[[ListOrganizationalUnitsForParentResponseTypeDef](./type_defs.md#listorganizationalunitsforparentresponsetypedef)\].

<a id="listparentspaginator"></a>

## ListParentsPaginator

Type annotations for
`session.create_client("organizations").get_paginator("list_parents")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListParentsPaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListParentsPaginator = client.get_paginator("list_parents")
```

Boto3 documentation:
[Organizations.Paginator.ListParents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListParents)

Arguments for `ListParentsPaginator.paginate` method:

- `ChildId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListParentsPaginator.paginate` returns
`AsyncIterable`\[[ListParentsResponseTypeDef](./type_defs.md#listparentsresponsetypedef)\].

<a id="listpoliciespaginator"></a>

## ListPoliciesPaginator

Type annotations for
`session.create_client("organizations").get_paginator("list_policies")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListPoliciesPaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListPoliciesPaginator = client.get_paginator("list_policies")
```

Boto3 documentation:
[Organizations.Paginator.ListPolicies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListPolicies)

Arguments for `ListPoliciesPaginator.paginate` method:

- `Filter`: [PolicyTypeType](./literals.md#policytypetype) *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPoliciesPaginator.paginate` returns
`AsyncIterable`\[[ListPoliciesResponseTypeDef](./type_defs.md#listpoliciesresponsetypedef)\].

<a id="listpoliciesfortargetpaginator"></a>

## ListPoliciesForTargetPaginator

Type annotations for
`session.create_client("organizations").get_paginator("list_policies_for_target")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListPoliciesForTargetPaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListPoliciesForTargetPaginator = client.get_paginator("list_policies_for_target")
```

Boto3 documentation:
[Organizations.Paginator.ListPoliciesForTarget](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListPoliciesForTarget)

Arguments for `ListPoliciesForTargetPaginator.paginate` method:

- `TargetId`: `str` *(required)*
- `Filter`: [PolicyTypeType](./literals.md#policytypetype) *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPoliciesForTargetPaginator.paginate` returns
`AsyncIterable`\[[ListPoliciesForTargetResponseTypeDef](./type_defs.md#listpoliciesfortargetresponsetypedef)\].

<a id="listrootspaginator"></a>

## ListRootsPaginator

Type annotations for
`session.create_client("organizations").get_paginator("list_roots")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListRootsPaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListRootsPaginator = client.get_paginator("list_roots")
```

Boto3 documentation:
[Organizations.Paginator.ListRoots](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListRoots)

Arguments for `ListRootsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListRootsPaginator.paginate` returns
`AsyncIterable`\[[ListRootsResponseTypeDef](./type_defs.md#listrootsresponsetypedef)\].

<a id="listtagsforresourcepaginator"></a>

## ListTagsForResourcePaginator

Type annotations for
`session.create_client("organizations").get_paginator("list_tags_for_resource")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
```

Boto3 documentation:
[Organizations.Paginator.ListTagsForResource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListTagsForResource)

Arguments for `ListTagsForResourcePaginator.paginate` method:

- `ResourceId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTagsForResourcePaginator.paginate` returns
`AsyncIterable`\[[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)\].

<a id="listtargetsforpolicypaginator"></a>

## ListTargetsForPolicyPaginator

Type annotations for
`session.create_client("organizations").get_paginator("list_targets_for_policy")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListTargetsForPolicyPaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListTargetsForPolicyPaginator = client.get_paginator("list_targets_for_policy")
```

Boto3 documentation:
[Organizations.Paginator.ListTargetsForPolicy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListTargetsForPolicy)

Arguments for `ListTargetsForPolicyPaginator.paginate` method:

- `PolicyId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTargetsForPolicyPaginator.paginate` returns
`AsyncIterable`\[[ListTargetsForPolicyResponseTypeDef](./type_defs.md#listtargetsforpolicyresponsetypedef)\].
