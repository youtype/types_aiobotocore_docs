# Paginators

> [Index](../README.md) > [Organizations](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Organizations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations)
    type annotations stubs module [types-aiobotocore-organizations](https://pypi.org/project/types-aiobotocore-organizations/).

## ListAWSServiceAccessForOrganizationPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_aws_service_access_for_organization")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListAWSServiceAccessForOrganization)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListAWSServiceAccessForOrganizationPaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListAWSServiceAccessForOrganizationPaginator = client.get_paginator("list_aws_service_access_for_organization")
```


### paginate

Type annotations and code completion for `#!python ListAWSServiceAccessForOrganizationPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAWSServiceAccessForOrganizationResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAWSServiceAccessForOrganizationResponseTypeDef](./type_defs.md#listawsserviceaccessfororganizationresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAWSServiceAccessForOrganizationRequestListAWSServiceAccessForOrganizationPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAWSServiceAccessForOrganizationRequestListAWSServiceAccessForOrganizationPaginateTypeDef](./type_defs.md#listawsserviceaccessfororganizationrequestlistawsserviceaccessfororganizationpaginatetypedef) 
## ListAccountsPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_accounts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListAccounts)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListAccountsPaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListAccountsPaginator = client.get_paginator("list_accounts")
```


### paginate

Type annotations and code completion for `#!python ListAccountsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAccountsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAccountsResponseTypeDef](./type_defs.md#listaccountsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAccountsRequestListAccountsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccountsRequestListAccountsPaginateTypeDef](./type_defs.md#listaccountsrequestlistaccountspaginatetypedef) 
## ListAccountsForParentPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_accounts_for_parent")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListAccountsForParent)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListAccountsForParentPaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListAccountsForParentPaginator = client.get_paginator("list_accounts_for_parent")
```


### paginate

Type annotations and code completion for `#!python ListAccountsForParentPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ParentId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAccountsForParentResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAccountsForParentResponseTypeDef](./type_defs.md#listaccountsforparentresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAccountsForParentRequestListAccountsForParentPaginateTypeDef = {  # (1)
    "ParentId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccountsForParentRequestListAccountsForParentPaginateTypeDef](./type_defs.md#listaccountsforparentrequestlistaccountsforparentpaginatetypedef) 
## ListChildrenPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_children")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListChildren)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListChildrenPaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListChildrenPaginator = client.get_paginator("list_children")
```


### paginate

Type annotations and code completion for `#!python ListChildrenPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ParentId: str,
    ChildType: ChildTypeType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListChildrenResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ChildTypeType](./literals.md#childtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListChildrenResponseTypeDef](./type_defs.md#listchildrenresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListChildrenRequestListChildrenPaginateTypeDef = {  # (1)
    "ParentId": ...,
    "ChildType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListChildrenRequestListChildrenPaginateTypeDef](./type_defs.md#listchildrenrequestlistchildrenpaginatetypedef) 
## ListCreateAccountStatusPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_create_account_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListCreateAccountStatus)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListCreateAccountStatusPaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListCreateAccountStatusPaginator = client.get_paginator("list_create_account_status")
```


### paginate

Type annotations and code completion for `#!python ListCreateAccountStatusPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    States: Sequence[CreateAccountStateType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListCreateAccountStatusResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: CreateAccountStateType](./literals.md#createaccountstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListCreateAccountStatusResponseTypeDef](./type_defs.md#listcreateaccountstatusresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListCreateAccountStatusRequestListCreateAccountStatusPaginateTypeDef = {  # (1)
    "States": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCreateAccountStatusRequestListCreateAccountStatusPaginateTypeDef](./type_defs.md#listcreateaccountstatusrequestlistcreateaccountstatuspaginatetypedef) 
## ListDelegatedAdministratorsPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_delegated_administrators")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListDelegatedAdministrators)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListDelegatedAdministratorsPaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListDelegatedAdministratorsPaginator = client.get_paginator("list_delegated_administrators")
```


### paginate

Type annotations and code completion for `#!python ListDelegatedAdministratorsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ServicePrincipal: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDelegatedAdministratorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDelegatedAdministratorsResponseTypeDef](./type_defs.md#listdelegatedadministratorsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDelegatedAdministratorsRequestListDelegatedAdministratorsPaginateTypeDef = {  # (1)
    "ServicePrincipal": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDelegatedAdministratorsRequestListDelegatedAdministratorsPaginateTypeDef](./type_defs.md#listdelegatedadministratorsrequestlistdelegatedadministratorspaginatetypedef) 
## ListDelegatedServicesForAccountPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_delegated_services_for_account")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListDelegatedServicesForAccount)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListDelegatedServicesForAccountPaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListDelegatedServicesForAccountPaginator = client.get_paginator("list_delegated_services_for_account")
```


### paginate

Type annotations and code completion for `#!python ListDelegatedServicesForAccountPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    AccountId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDelegatedServicesForAccountResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDelegatedServicesForAccountResponseTypeDef](./type_defs.md#listdelegatedservicesforaccountresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDelegatedServicesForAccountRequestListDelegatedServicesForAccountPaginateTypeDef = {  # (1)
    "AccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDelegatedServicesForAccountRequestListDelegatedServicesForAccountPaginateTypeDef](./type_defs.md#listdelegatedservicesforaccountrequestlistdelegatedservicesforaccountpaginatetypedef) 
## ListHandshakesForAccountPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_handshakes_for_account")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListHandshakesForAccount)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListHandshakesForAccountPaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListHandshakesForAccountPaginator = client.get_paginator("list_handshakes_for_account")
```


### paginate

Type annotations and code completion for `#!python ListHandshakesForAccountPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filter: HandshakeFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListHandshakesForAccountResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: HandshakeFilterTypeDef](./type_defs.md#handshakefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListHandshakesForAccountResponseTypeDef](./type_defs.md#listhandshakesforaccountresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListHandshakesForAccountRequestListHandshakesForAccountPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListHandshakesForAccountRequestListHandshakesForAccountPaginateTypeDef](./type_defs.md#listhandshakesforaccountrequestlisthandshakesforaccountpaginatetypedef) 
## ListHandshakesForOrganizationPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_handshakes_for_organization")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListHandshakesForOrganization)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListHandshakesForOrganizationPaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListHandshakesForOrganizationPaginator = client.get_paginator("list_handshakes_for_organization")
```


### paginate

Type annotations and code completion for `#!python ListHandshakesForOrganizationPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filter: HandshakeFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListHandshakesForOrganizationResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: HandshakeFilterTypeDef](./type_defs.md#handshakefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListHandshakesForOrganizationResponseTypeDef](./type_defs.md#listhandshakesfororganizationresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListHandshakesForOrganizationRequestListHandshakesForOrganizationPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListHandshakesForOrganizationRequestListHandshakesForOrganizationPaginateTypeDef](./type_defs.md#listhandshakesfororganizationrequestlisthandshakesfororganizationpaginatetypedef) 
## ListOrganizationalUnitsForParentPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_organizational_units_for_parent")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListOrganizationalUnitsForParent)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListOrganizationalUnitsForParentPaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListOrganizationalUnitsForParentPaginator = client.get_paginator("list_organizational_units_for_parent")
```


### paginate

Type annotations and code completion for `#!python ListOrganizationalUnitsForParentPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ParentId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListOrganizationalUnitsForParentResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListOrganizationalUnitsForParentResponseTypeDef](./type_defs.md#listorganizationalunitsforparentresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListOrganizationalUnitsForParentRequestListOrganizationalUnitsForParentPaginateTypeDef = {  # (1)
    "ParentId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOrganizationalUnitsForParentRequestListOrganizationalUnitsForParentPaginateTypeDef](./type_defs.md#listorganizationalunitsforparentrequestlistorganizationalunitsforparentpaginatetypedef) 
## ListParentsPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_parents")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListParents)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListParentsPaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListParentsPaginator = client.get_paginator("list_parents")
```


### paginate

Type annotations and code completion for `#!python ListParentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ChildId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListParentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListParentsResponseTypeDef](./type_defs.md#listparentsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListParentsRequestListParentsPaginateTypeDef = {  # (1)
    "ChildId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListParentsRequestListParentsPaginateTypeDef](./type_defs.md#listparentsrequestlistparentspaginatetypedef) 
## ListPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListPolicies)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListPoliciesPaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListPoliciesPaginator = client.get_paginator("list_policies")
```


### paginate

Type annotations and code completion for `#!python ListPoliciesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filter: PolicyTypeType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListPoliciesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListPoliciesResponseTypeDef](./type_defs.md#listpoliciesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListPoliciesRequestListPoliciesPaginateTypeDef = {  # (1)
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPoliciesRequestListPoliciesPaginateTypeDef](./type_defs.md#listpoliciesrequestlistpoliciespaginatetypedef) 
## ListPoliciesForTargetPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_policies_for_target")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListPoliciesForTarget)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListPoliciesForTargetPaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListPoliciesForTargetPaginator = client.get_paginator("list_policies_for_target")
```


### paginate

Type annotations and code completion for `#!python ListPoliciesForTargetPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TargetId: str,
    Filter: PolicyTypeType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListPoliciesForTargetResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: PolicyTypeType](./literals.md#policytypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListPoliciesForTargetResponseTypeDef](./type_defs.md#listpoliciesfortargetresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListPoliciesForTargetRequestListPoliciesForTargetPaginateTypeDef = {  # (1)
    "TargetId": ...,
    "Filter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPoliciesForTargetRequestListPoliciesForTargetPaginateTypeDef](./type_defs.md#listpoliciesfortargetrequestlistpoliciesfortargetpaginatetypedef) 
## ListRootsPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_roots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListRoots)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListRootsPaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListRootsPaginator = client.get_paginator("list_roots")
```


### paginate

Type annotations and code completion for `#!python ListRootsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListRootsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRootsResponseTypeDef](./type_defs.md#listrootsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRootsRequestListRootsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRootsRequestListRootsPaginateTypeDef](./type_defs.md#listrootsrequestlistrootspaginatetypedef) 
## ListTagsForResourcePaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_tags_for_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListTagsForResource)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
```


### paginate

Type annotations and code completion for `#!python ListTagsForResourcePaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ResourceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTagsForResourceResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTagsForResourceRequestListTagsForResourcePaginateTypeDef = {  # (1)
    "ResourceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestListTagsForResourcePaginateTypeDef](./type_defs.md#listtagsforresourcerequestlisttagsforresourcepaginatetypedef) 
## ListTargetsForPolicyPaginator

Type annotations and code completion for `#!python session.create_client("organizations").get_paginator("list_targets_for_policy")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#Organizations.Paginator.ListTargetsForPolicy)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_organizations.paginator import ListTargetsForPolicyPaginator

session = get_session()
async with session.create_client("organizations") as client:
    client: OrganizationsClient
    paginator: ListTargetsForPolicyPaginator = client.get_paginator("list_targets_for_policy")
```


### paginate

Type annotations and code completion for `#!python ListTargetsForPolicyPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PolicyId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTargetsForPolicyResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTargetsForPolicyResponseTypeDef](./type_defs.md#listtargetsforpolicyresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef = {  # (1)
    "PolicyId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef](./type_defs.md#listtargetsforpolicyrequestlisttargetsforpolicypaginatetypedef) 
