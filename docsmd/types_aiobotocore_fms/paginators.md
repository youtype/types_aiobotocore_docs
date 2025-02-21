# Paginators

> [Index](../README.md) > [FMS](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [FMS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#fms)
    type annotations stubs module [types-aiobotocore-fms](https://pypi.org/project/types-aiobotocore-fms/).

## ListAdminAccountsForOrganizationPaginator

Type annotations and code completion for `#!python session.create_client("fms").get_paginator("list_admin_accounts_for_organization")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms/paginator/ListAdminAccountsForOrganization.html#FMS.Paginator.ListAdminAccountsForOrganization)

```python
# ListAdminAccountsForOrganizationPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_fms.paginator import ListAdminAccountsForOrganizationPaginator

session = get_session()
async with session.create_client("fms") as client:  # (1)
    paginator: ListAdminAccountsForOrganizationPaginator = client.get_paginator("list_admin_accounts_for_organization")  # (2)
    async for item in paginator.paginate(...):
        item: ListAdminAccountsForOrganizationResponseTypeDef
        print(item)  # (3)
```

1. client: [FMSClient](./client.md)
2. paginator: [ListAdminAccountsForOrganizationPaginator](./paginators.md#listadminaccountsfororganizationpaginator)
3. item: [:material-code-braces: ListAdminAccountsForOrganizationResponseTypeDef](./type_defs.md#listadminaccountsfororganizationresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAdminAccountsForOrganizationPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAdminAccountsForOrganizationResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAdminAccountsForOrganizationResponseTypeDef](./type_defs.md#listadminaccountsfororganizationresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAdminAccountsForOrganizationRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAdminAccountsForOrganizationRequestPaginateTypeDef](./type_defs.md#listadminaccountsfororganizationrequestpaginatetypedef) 
## ListAdminsManagingAccountPaginator

Type annotations and code completion for `#!python session.create_client("fms").get_paginator("list_admins_managing_account")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms/paginator/ListAdminsManagingAccount.html#FMS.Paginator.ListAdminsManagingAccount)

```python
# ListAdminsManagingAccountPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_fms.paginator import ListAdminsManagingAccountPaginator

session = get_session()
async with session.create_client("fms") as client:  # (1)
    paginator: ListAdminsManagingAccountPaginator = client.get_paginator("list_admins_managing_account")  # (2)
    async for item in paginator.paginate(...):
        item: ListAdminsManagingAccountResponseTypeDef
        print(item)  # (3)
```

1. client: [FMSClient](./client.md)
2. paginator: [ListAdminsManagingAccountPaginator](./paginators.md#listadminsmanagingaccountpaginator)
3. item: [:material-code-braces: ListAdminsManagingAccountResponseTypeDef](./type_defs.md#listadminsmanagingaccountresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAdminsManagingAccountPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAdminsManagingAccountResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAdminsManagingAccountResponseTypeDef](./type_defs.md#listadminsmanagingaccountresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAdminsManagingAccountRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAdminsManagingAccountRequestPaginateTypeDef](./type_defs.md#listadminsmanagingaccountrequestpaginatetypedef) 
## ListAppsListsPaginator

Type annotations and code completion for `#!python session.create_client("fms").get_paginator("list_apps_lists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms/paginator/ListAppsLists.html#FMS.Paginator.ListAppsLists)

```python
# ListAppsListsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_fms.paginator import ListAppsListsPaginator

session = get_session()
async with session.create_client("fms") as client:  # (1)
    paginator: ListAppsListsPaginator = client.get_paginator("list_apps_lists")  # (2)
    async for item in paginator.paginate(...):
        item: ListAppsListsResponseTypeDef
        print(item)  # (3)
```

1. client: [FMSClient](./client.md)
2. paginator: [ListAppsListsPaginator](./paginators.md#listappslistspaginator)
3. item: [:material-code-braces: ListAppsListsResponseTypeDef](./type_defs.md#listappslistsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAppsListsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DefaultLists: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAppsListsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAppsListsResponseTypeDef](./type_defs.md#listappslistsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAppsListsRequestPaginateTypeDef = {  # (1)
    "DefaultLists": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAppsListsRequestPaginateTypeDef](./type_defs.md#listappslistsrequestpaginatetypedef) 
## ListComplianceStatusPaginator

Type annotations and code completion for `#!python session.create_client("fms").get_paginator("list_compliance_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms/paginator/ListComplianceStatus.html#FMS.Paginator.ListComplianceStatus)

```python
# ListComplianceStatusPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_fms.paginator import ListComplianceStatusPaginator

session = get_session()
async with session.create_client("fms") as client:  # (1)
    paginator: ListComplianceStatusPaginator = client.get_paginator("list_compliance_status")  # (2)
    async for item in paginator.paginate(...):
        item: ListComplianceStatusResponseTypeDef
        print(item)  # (3)
```

1. client: [FMSClient](./client.md)
2. paginator: [ListComplianceStatusPaginator](./paginators.md#listcompliancestatuspaginator)
3. item: [:material-code-braces: ListComplianceStatusResponseTypeDef](./type_defs.md#listcompliancestatusresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListComplianceStatusPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PolicyId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListComplianceStatusResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListComplianceStatusResponseTypeDef](./type_defs.md#listcompliancestatusresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListComplianceStatusRequestPaginateTypeDef = {  # (1)
    "PolicyId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListComplianceStatusRequestPaginateTypeDef](./type_defs.md#listcompliancestatusrequestpaginatetypedef) 
## ListMemberAccountsPaginator

Type annotations and code completion for `#!python session.create_client("fms").get_paginator("list_member_accounts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms/paginator/ListMemberAccounts.html#FMS.Paginator.ListMemberAccounts)

```python
# ListMemberAccountsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_fms.paginator import ListMemberAccountsPaginator

session = get_session()
async with session.create_client("fms") as client:  # (1)
    paginator: ListMemberAccountsPaginator = client.get_paginator("list_member_accounts")  # (2)
    async for item in paginator.paginate(...):
        item: ListMemberAccountsResponseTypeDef
        print(item)  # (3)
```

1. client: [FMSClient](./client.md)
2. paginator: [ListMemberAccountsPaginator](./paginators.md#listmemberaccountspaginator)
3. item: [:material-code-braces: ListMemberAccountsResponseTypeDef](./type_defs.md#listmemberaccountsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListMemberAccountsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListMemberAccountsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMemberAccountsResponseTypeDef](./type_defs.md#listmemberaccountsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListMemberAccountsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMemberAccountsRequestPaginateTypeDef](./type_defs.md#listmemberaccountsrequestpaginatetypedef) 
## ListPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("fms").get_paginator("list_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms/paginator/ListPolicies.html#FMS.Paginator.ListPolicies)

```python
# ListPoliciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_fms.paginator import ListPoliciesPaginator

session = get_session()
async with session.create_client("fms") as client:  # (1)
    paginator: ListPoliciesPaginator = client.get_paginator("list_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListPoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [FMSClient](./client.md)
2. paginator: [ListPoliciesPaginator](./paginators.md#listpoliciespaginator)
3. item: [:material-code-braces: ListPoliciesResponseTypeDef](./type_defs.md#listpoliciesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListPoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPoliciesResponseTypeDef](./type_defs.md#listpoliciesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPoliciesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPoliciesRequestPaginateTypeDef](./type_defs.md#listpoliciesrequestpaginatetypedef) 
## ListProtocolsListsPaginator

Type annotations and code completion for `#!python session.create_client("fms").get_paginator("list_protocols_lists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms/paginator/ListProtocolsLists.html#FMS.Paginator.ListProtocolsLists)

```python
# ListProtocolsListsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_fms.paginator import ListProtocolsListsPaginator

session = get_session()
async with session.create_client("fms") as client:  # (1)
    paginator: ListProtocolsListsPaginator = client.get_paginator("list_protocols_lists")  # (2)
    async for item in paginator.paginate(...):
        item: ListProtocolsListsResponseTypeDef
        print(item)  # (3)
```

1. client: [FMSClient](./client.md)
2. paginator: [ListProtocolsListsPaginator](./paginators.md#listprotocolslistspaginator)
3. item: [:material-code-braces: ListProtocolsListsResponseTypeDef](./type_defs.md#listprotocolslistsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListProtocolsListsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DefaultLists: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListProtocolsListsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListProtocolsListsResponseTypeDef](./type_defs.md#listprotocolslistsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListProtocolsListsRequestPaginateTypeDef = {  # (1)
    "DefaultLists": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProtocolsListsRequestPaginateTypeDef](./type_defs.md#listprotocolslistsrequestpaginatetypedef) 
## ListThirdPartyFirewallFirewallPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("fms").get_paginator("list_third_party_firewall_firewall_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms/paginator/ListThirdPartyFirewallFirewallPolicies.html#FMS.Paginator.ListThirdPartyFirewallFirewallPolicies)

```python
# ListThirdPartyFirewallFirewallPoliciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_fms.paginator import ListThirdPartyFirewallFirewallPoliciesPaginator

session = get_session()
async with session.create_client("fms") as client:  # (1)
    paginator: ListThirdPartyFirewallFirewallPoliciesPaginator = client.get_paginator("list_third_party_firewall_firewall_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListThirdPartyFirewallFirewallPoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [FMSClient](./client.md)
2. paginator: [ListThirdPartyFirewallFirewallPoliciesPaginator](./paginators.md#listthirdpartyfirewallfirewallpoliciespaginator)
3. item: [:material-code-braces: ListThirdPartyFirewallFirewallPoliciesResponseTypeDef](./type_defs.md#listthirdpartyfirewallfirewallpoliciesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListThirdPartyFirewallFirewallPoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ThirdPartyFirewall: ThirdPartyFirewallType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListThirdPartyFirewallFirewallPoliciesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ThirdPartyFirewallType](./literals.md#thirdpartyfirewalltype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListThirdPartyFirewallFirewallPoliciesResponseTypeDef](./type_defs.md#listthirdpartyfirewallfirewallpoliciesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListThirdPartyFirewallFirewallPoliciesRequestPaginateTypeDef = {  # (1)
    "ThirdPartyFirewall": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListThirdPartyFirewallFirewallPoliciesRequestPaginateTypeDef](./type_defs.md#listthirdpartyfirewallfirewallpoliciesrequestpaginatetypedef) 
