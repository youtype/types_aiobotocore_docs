# Paginators

> [Index](../README.md) > [NetworkFirewall](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [NetworkFirewall](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall)
    type annotations stubs module [types-aiobotocore-network-firewall](https://pypi.org/project/types-aiobotocore-network-firewall/).

## ListFirewallPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("network-firewall").get_paginator("list_firewall_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListFirewallPolicies)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_network_firewall.paginator import ListFirewallPoliciesPaginator

session = get_session()
async with session.create_client("network-firewall") as client:
    client: NetworkFirewallClient
    paginator: ListFirewallPoliciesPaginator = client.get_paginator("list_firewall_policies")
```


### paginate

Type annotations and code completion for `#!python ListFirewallPoliciesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListFirewallPoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFirewallPoliciesResponseTypeDef](./type_defs.md#listfirewallpoliciesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFirewallPoliciesRequestListFirewallPoliciesPaginateTypeDef](./type_defs.md#listfirewallpoliciesrequestlistfirewallpoliciespaginatetypedef) 
## ListFirewallsPaginator

Type annotations and code completion for `#!python session.create_client("network-firewall").get_paginator("list_firewalls")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListFirewalls)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_network_firewall.paginator import ListFirewallsPaginator

session = get_session()
async with session.create_client("network-firewall") as client:
    client: NetworkFirewallClient
    paginator: ListFirewallsPaginator = client.get_paginator("list_firewalls")
```


### paginate

Type annotations and code completion for `#!python ListFirewallsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    VpcIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListFirewallsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFirewallsResponseTypeDef](./type_defs.md#listfirewallsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListFirewallsRequestListFirewallsPaginateTypeDef = {  # (1)
    "VpcIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFirewallsRequestListFirewallsPaginateTypeDef](./type_defs.md#listfirewallsrequestlistfirewallspaginatetypedef) 
## ListRuleGroupsPaginator

Type annotations and code completion for `#!python session.create_client("network-firewall").get_paginator("list_rule_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListRuleGroups)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_network_firewall.paginator import ListRuleGroupsPaginator

session = get_session()
async with session.create_client("network-firewall") as client:
    client: NetworkFirewallClient
    paginator: ListRuleGroupsPaginator = client.get_paginator("list_rule_groups")
```


### paginate

Type annotations and code completion for `#!python ListRuleGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Scope: ResourceManagedStatusType = ...,  # (1)
    ManagedType: ResourceManagedTypeType = ...,  # (2)
    Type: RuleGroupTypeType = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AsyncIterator[ListRuleGroupsResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: ResourceManagedStatusType](./literals.md#resourcemanagedstatustype) 
2. See [:material-code-brackets: ResourceManagedTypeType](./literals.md#resourcemanagedtypetype) 
3. See [:material-code-brackets: RuleGroupTypeType](./literals.md#rulegrouptypetype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: ListRuleGroupsResponseTypeDef](./type_defs.md#listrulegroupsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListRuleGroupsRequestListRuleGroupsPaginateTypeDef = {  # (1)
    "Scope": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRuleGroupsRequestListRuleGroupsPaginateTypeDef](./type_defs.md#listrulegroupsrequestlistrulegroupspaginatetypedef) 
## ListTagsForResourcePaginator

Type annotations and code completion for `#!python session.create_client("network-firewall").get_paginator("list_tags_for_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#NetworkFirewall.Paginator.ListTagsForResource)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_network_firewall.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("network-firewall") as client:
    client: NetworkFirewallClient
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
```


### paginate

Type annotations and code completion for `#!python ListTagsForResourcePaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ResourceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTagsForResourceResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTagsForResourceRequestListTagsForResourcePaginateTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestListTagsForResourcePaginateTypeDef](./type_defs.md#listtagsforresourcerequestlisttagsforresourcepaginatetypedef) 
