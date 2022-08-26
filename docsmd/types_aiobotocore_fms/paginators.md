# Paginators

> [Index](../README.md) > [FMS](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [FMS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
    type annotations stubs module [types-aiobotocore-fms](https://pypi.org/project/types-aiobotocore-fms/).

## ListAppsListsPaginator

Type annotations and code completion for `#!python session.create_client("fms").get_paginator("list_apps_lists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAppsLists)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    DefaultLists: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAppsListsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAppsListsResponseTypeDef](./type_defs.md#listappslistsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAppsListsRequestListAppsListsPaginateTypeDef = {  # (1)
    "DefaultLists": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAppsListsRequestListAppsListsPaginateTypeDef](./type_defs.md#listappslistsrequestlistappslistspaginatetypedef) 
## ListComplianceStatusPaginator

Type annotations and code completion for `#!python session.create_client("fms").get_paginator("list_compliance_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListComplianceStatus)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    PolicyId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListComplianceStatusResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListComplianceStatusResponseTypeDef](./type_defs.md#listcompliancestatusresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListComplianceStatusRequestListComplianceStatusPaginateTypeDef = {  # (1)
    "PolicyId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListComplianceStatusRequestListComplianceStatusPaginateTypeDef](./type_defs.md#listcompliancestatusrequestlistcompliancestatuspaginatetypedef) 
## ListMemberAccountsPaginator

Type annotations and code completion for `#!python session.create_client("fms").get_paginator("list_member_accounts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListMemberAccounts)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListMemberAccountsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListMemberAccountsResponseTypeDef](./type_defs.md#listmemberaccountsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListMemberAccountsRequestListMemberAccountsPaginateTypeDef](./type_defs.md#listmemberaccountsrequestlistmemberaccountspaginatetypedef) 
## ListPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("fms").get_paginator("list_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListPolicies)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPoliciesResponseTypeDef](./type_defs.md#listpoliciesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListPoliciesRequestListPoliciesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPoliciesRequestListPoliciesPaginateTypeDef](./type_defs.md#listpoliciesrequestlistpoliciespaginatetypedef) 
## ListProtocolsListsPaginator

Type annotations and code completion for `#!python session.create_client("fms").get_paginator("list_protocols_lists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListProtocolsLists)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    DefaultLists: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListProtocolsListsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListProtocolsListsResponseTypeDef](./type_defs.md#listprotocolslistsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListProtocolsListsRequestListProtocolsListsPaginateTypeDef = {  # (1)
    "DefaultLists": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProtocolsListsRequestListProtocolsListsPaginateTypeDef](./type_defs.md#listprotocolslistsrequestlistprotocolslistspaginatetypedef) 
## ListThirdPartyFirewallFirewallPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("fms").get_paginator("list_third_party_firewall_firewall_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListThirdPartyFirewallFirewallPolicies)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    ThirdPartyFirewall: ThirdPartyFirewallType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListThirdPartyFirewallFirewallPoliciesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ThirdPartyFirewallType](./literals.md#thirdpartyfirewalltype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListThirdPartyFirewallFirewallPoliciesResponseTypeDef](./type_defs.md#listthirdpartyfirewallfirewallpoliciesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef = {  # (1)
    "ThirdPartyFirewall": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef](./type_defs.md#listthirdpartyfirewallfirewallpoliciesrequestlistthirdpartyfirewallfirewallpoliciespaginatetypedef) 
