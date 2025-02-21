# Paginators

> [Index](../README.md) > [Route53Resolver](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Route53Resolver](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#route53resolver)
    type annotations stubs module [types-aiobotocore-route53resolver](https://pypi.org/project/types-aiobotocore-route53resolver/).

## ListFirewallConfigsPaginator

Type annotations and code completion for `#!python session.create_client("route53resolver").get_paginator("list_firewall_configs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver/paginator/ListFirewallConfigs.html#Route53Resolver.Paginator.ListFirewallConfigs)

```python
# ListFirewallConfigsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.paginator import ListFirewallConfigsPaginator

session = get_session()
async with session.create_client("route53resolver") as client:  # (1)
    paginator: ListFirewallConfigsPaginator = client.get_paginator("list_firewall_configs")  # (2)
    async for item in paginator.paginate(...):
        item: ListFirewallConfigsResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53ResolverClient](./client.md)
2. paginator: [ListFirewallConfigsPaginator](./paginators.md#listfirewallconfigspaginator)
3. item: [:material-code-braces: ListFirewallConfigsResponseTypeDef](./type_defs.md#listfirewallconfigsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFirewallConfigsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListFirewallConfigsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFirewallConfigsResponseTypeDef](./type_defs.md#listfirewallconfigsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFirewallConfigsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFirewallConfigsRequestPaginateTypeDef](./type_defs.md#listfirewallconfigsrequestpaginatetypedef) 
## ListFirewallDomainListsPaginator

Type annotations and code completion for `#!python session.create_client("route53resolver").get_paginator("list_firewall_domain_lists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver/paginator/ListFirewallDomainLists.html#Route53Resolver.Paginator.ListFirewallDomainLists)

```python
# ListFirewallDomainListsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.paginator import ListFirewallDomainListsPaginator

session = get_session()
async with session.create_client("route53resolver") as client:  # (1)
    paginator: ListFirewallDomainListsPaginator = client.get_paginator("list_firewall_domain_lists")  # (2)
    async for item in paginator.paginate(...):
        item: ListFirewallDomainListsResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53ResolverClient](./client.md)
2. paginator: [ListFirewallDomainListsPaginator](./paginators.md#listfirewalldomainlistspaginator)
3. item: [:material-code-braces: ListFirewallDomainListsResponseTypeDef](./type_defs.md#listfirewalldomainlistsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFirewallDomainListsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListFirewallDomainListsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFirewallDomainListsResponseTypeDef](./type_defs.md#listfirewalldomainlistsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFirewallDomainListsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFirewallDomainListsRequestPaginateTypeDef](./type_defs.md#listfirewalldomainlistsrequestpaginatetypedef) 
## ListFirewallDomainsPaginator

Type annotations and code completion for `#!python session.create_client("route53resolver").get_paginator("list_firewall_domains")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver/paginator/ListFirewallDomains.html#Route53Resolver.Paginator.ListFirewallDomains)

```python
# ListFirewallDomainsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.paginator import ListFirewallDomainsPaginator

session = get_session()
async with session.create_client("route53resolver") as client:  # (1)
    paginator: ListFirewallDomainsPaginator = client.get_paginator("list_firewall_domains")  # (2)
    async for item in paginator.paginate(...):
        item: ListFirewallDomainsResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53ResolverClient](./client.md)
2. paginator: [ListFirewallDomainsPaginator](./paginators.md#listfirewalldomainspaginator)
3. item: [:material-code-braces: ListFirewallDomainsResponseTypeDef](./type_defs.md#listfirewalldomainsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFirewallDomainsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FirewallDomainListId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListFirewallDomainsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFirewallDomainsResponseTypeDef](./type_defs.md#listfirewalldomainsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFirewallDomainsRequestPaginateTypeDef = {  # (1)
    "FirewallDomainListId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFirewallDomainsRequestPaginateTypeDef](./type_defs.md#listfirewalldomainsrequestpaginatetypedef) 
## ListFirewallRuleGroupAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("route53resolver").get_paginator("list_firewall_rule_group_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver/paginator/ListFirewallRuleGroupAssociations.html#Route53Resolver.Paginator.ListFirewallRuleGroupAssociations)

```python
# ListFirewallRuleGroupAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.paginator import ListFirewallRuleGroupAssociationsPaginator

session = get_session()
async with session.create_client("route53resolver") as client:  # (1)
    paginator: ListFirewallRuleGroupAssociationsPaginator = client.get_paginator("list_firewall_rule_group_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListFirewallRuleGroupAssociationsResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53ResolverClient](./client.md)
2. paginator: [ListFirewallRuleGroupAssociationsPaginator](./paginators.md#listfirewallrulegroupassociationspaginator)
3. item: [:material-code-braces: ListFirewallRuleGroupAssociationsResponseTypeDef](./type_defs.md#listfirewallrulegroupassociationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFirewallRuleGroupAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FirewallRuleGroupId: str = ...,
    VpcId: str = ...,
    Priority: int = ...,
    Status: FirewallRuleGroupAssociationStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListFirewallRuleGroupAssociationsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: FirewallRuleGroupAssociationStatusType](./literals.md#firewallrulegroupassociationstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListFirewallRuleGroupAssociationsResponseTypeDef](./type_defs.md#listfirewallrulegroupassociationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFirewallRuleGroupAssociationsRequestPaginateTypeDef = {  # (1)
    "FirewallRuleGroupId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFirewallRuleGroupAssociationsRequestPaginateTypeDef](./type_defs.md#listfirewallrulegroupassociationsrequestpaginatetypedef) 
## ListFirewallRuleGroupsPaginator

Type annotations and code completion for `#!python session.create_client("route53resolver").get_paginator("list_firewall_rule_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver/paginator/ListFirewallRuleGroups.html#Route53Resolver.Paginator.ListFirewallRuleGroups)

```python
# ListFirewallRuleGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.paginator import ListFirewallRuleGroupsPaginator

session = get_session()
async with session.create_client("route53resolver") as client:  # (1)
    paginator: ListFirewallRuleGroupsPaginator = client.get_paginator("list_firewall_rule_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListFirewallRuleGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53ResolverClient](./client.md)
2. paginator: [ListFirewallRuleGroupsPaginator](./paginators.md#listfirewallrulegroupspaginator)
3. item: [:material-code-braces: ListFirewallRuleGroupsResponseTypeDef](./type_defs.md#listfirewallrulegroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFirewallRuleGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListFirewallRuleGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFirewallRuleGroupsResponseTypeDef](./type_defs.md#listfirewallrulegroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFirewallRuleGroupsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFirewallRuleGroupsRequestPaginateTypeDef](./type_defs.md#listfirewallrulegroupsrequestpaginatetypedef) 
## ListFirewallRulesPaginator

Type annotations and code completion for `#!python session.create_client("route53resolver").get_paginator("list_firewall_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver/paginator/ListFirewallRules.html#Route53Resolver.Paginator.ListFirewallRules)

```python
# ListFirewallRulesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.paginator import ListFirewallRulesPaginator

session = get_session()
async with session.create_client("route53resolver") as client:  # (1)
    paginator: ListFirewallRulesPaginator = client.get_paginator("list_firewall_rules")  # (2)
    async for item in paginator.paginate(...):
        item: ListFirewallRulesResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53ResolverClient](./client.md)
2. paginator: [ListFirewallRulesPaginator](./paginators.md#listfirewallrulespaginator)
3. item: [:material-code-braces: ListFirewallRulesResponseTypeDef](./type_defs.md#listfirewallrulesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFirewallRulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FirewallRuleGroupId: str,
    Priority: int = ...,
    Action: ActionType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListFirewallRulesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ActionType](./literals.md#actiontype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListFirewallRulesResponseTypeDef](./type_defs.md#listfirewallrulesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFirewallRulesRequestPaginateTypeDef = {  # (1)
    "FirewallRuleGroupId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFirewallRulesRequestPaginateTypeDef](./type_defs.md#listfirewallrulesrequestpaginatetypedef) 
## ListOutpostResolversPaginator

Type annotations and code completion for `#!python session.create_client("route53resolver").get_paginator("list_outpost_resolvers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver/paginator/ListOutpostResolvers.html#Route53Resolver.Paginator.ListOutpostResolvers)

```python
# ListOutpostResolversPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.paginator import ListOutpostResolversPaginator

session = get_session()
async with session.create_client("route53resolver") as client:  # (1)
    paginator: ListOutpostResolversPaginator = client.get_paginator("list_outpost_resolvers")  # (2)
    async for item in paginator.paginate(...):
        item: ListOutpostResolversResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53ResolverClient](./client.md)
2. paginator: [ListOutpostResolversPaginator](./paginators.md#listoutpostresolverspaginator)
3. item: [:material-code-braces: ListOutpostResolversResponseTypeDef](./type_defs.md#listoutpostresolversresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListOutpostResolversPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OutpostArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListOutpostResolversResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListOutpostResolversResponseTypeDef](./type_defs.md#listoutpostresolversresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListOutpostResolversRequestPaginateTypeDef = {  # (1)
    "OutpostArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListOutpostResolversRequestPaginateTypeDef](./type_defs.md#listoutpostresolversrequestpaginatetypedef) 
## ListResolverConfigsPaginator

Type annotations and code completion for `#!python session.create_client("route53resolver").get_paginator("list_resolver_configs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver/paginator/ListResolverConfigs.html#Route53Resolver.Paginator.ListResolverConfigs)

```python
# ListResolverConfigsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.paginator import ListResolverConfigsPaginator

session = get_session()
async with session.create_client("route53resolver") as client:  # (1)
    paginator: ListResolverConfigsPaginator = client.get_paginator("list_resolver_configs")  # (2)
    async for item in paginator.paginate(...):
        item: ListResolverConfigsResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53ResolverClient](./client.md)
2. paginator: [ListResolverConfigsPaginator](./paginators.md#listresolverconfigspaginator)
3. item: [:material-code-braces: ListResolverConfigsResponseTypeDef](./type_defs.md#listresolverconfigsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListResolverConfigsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListResolverConfigsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListResolverConfigsResponseTypeDef](./type_defs.md#listresolverconfigsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListResolverConfigsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResolverConfigsRequestPaginateTypeDef](./type_defs.md#listresolverconfigsrequestpaginatetypedef) 
## ListResolverDnssecConfigsPaginator

Type annotations and code completion for `#!python session.create_client("route53resolver").get_paginator("list_resolver_dnssec_configs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver/paginator/ListResolverDnssecConfigs.html#Route53Resolver.Paginator.ListResolverDnssecConfigs)

```python
# ListResolverDnssecConfigsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.paginator import ListResolverDnssecConfigsPaginator

session = get_session()
async with session.create_client("route53resolver") as client:  # (1)
    paginator: ListResolverDnssecConfigsPaginator = client.get_paginator("list_resolver_dnssec_configs")  # (2)
    async for item in paginator.paginate(...):
        item: ListResolverDnssecConfigsResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53ResolverClient](./client.md)
2. paginator: [ListResolverDnssecConfigsPaginator](./paginators.md#listresolverdnssecconfigspaginator)
3. item: [:material-code-braces: ListResolverDnssecConfigsResponseTypeDef](./type_defs.md#listresolverdnssecconfigsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListResolverDnssecConfigsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListResolverDnssecConfigsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListResolverDnssecConfigsResponseTypeDef](./type_defs.md#listresolverdnssecconfigsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListResolverDnssecConfigsRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResolverDnssecConfigsRequestPaginateTypeDef](./type_defs.md#listresolverdnssecconfigsrequestpaginatetypedef) 
## ListResolverEndpointIpAddressesPaginator

Type annotations and code completion for `#!python session.create_client("route53resolver").get_paginator("list_resolver_endpoint_ip_addresses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver/paginator/ListResolverEndpointIpAddresses.html#Route53Resolver.Paginator.ListResolverEndpointIpAddresses)

```python
# ListResolverEndpointIpAddressesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.paginator import ListResolverEndpointIpAddressesPaginator

session = get_session()
async with session.create_client("route53resolver") as client:  # (1)
    paginator: ListResolverEndpointIpAddressesPaginator = client.get_paginator("list_resolver_endpoint_ip_addresses")  # (2)
    async for item in paginator.paginate(...):
        item: ListResolverEndpointIpAddressesResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53ResolverClient](./client.md)
2. paginator: [ListResolverEndpointIpAddressesPaginator](./paginators.md#listresolverendpointipaddressespaginator)
3. item: [:material-code-braces: ListResolverEndpointIpAddressesResponseTypeDef](./type_defs.md#listresolverendpointipaddressesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListResolverEndpointIpAddressesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResolverEndpointId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListResolverEndpointIpAddressesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListResolverEndpointIpAddressesResponseTypeDef](./type_defs.md#listresolverendpointipaddressesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListResolverEndpointIpAddressesRequestPaginateTypeDef = {  # (1)
    "ResolverEndpointId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResolverEndpointIpAddressesRequestPaginateTypeDef](./type_defs.md#listresolverendpointipaddressesrequestpaginatetypedef) 
## ListResolverEndpointsPaginator

Type annotations and code completion for `#!python session.create_client("route53resolver").get_paginator("list_resolver_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver/paginator/ListResolverEndpoints.html#Route53Resolver.Paginator.ListResolverEndpoints)

```python
# ListResolverEndpointsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.paginator import ListResolverEndpointsPaginator

session = get_session()
async with session.create_client("route53resolver") as client:  # (1)
    paginator: ListResolverEndpointsPaginator = client.get_paginator("list_resolver_endpoints")  # (2)
    async for item in paginator.paginate(...):
        item: ListResolverEndpointsResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53ResolverClient](./client.md)
2. paginator: [ListResolverEndpointsPaginator](./paginators.md#listresolverendpointspaginator)
3. item: [:material-code-braces: ListResolverEndpointsResponseTypeDef](./type_defs.md#listresolverendpointsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListResolverEndpointsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListResolverEndpointsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListResolverEndpointsResponseTypeDef](./type_defs.md#listresolverendpointsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListResolverEndpointsRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResolverEndpointsRequestPaginateTypeDef](./type_defs.md#listresolverendpointsrequestpaginatetypedef) 
## ListResolverQueryLogConfigAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("route53resolver").get_paginator("list_resolver_query_log_config_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver/paginator/ListResolverQueryLogConfigAssociations.html#Route53Resolver.Paginator.ListResolverQueryLogConfigAssociations)

```python
# ListResolverQueryLogConfigAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.paginator import ListResolverQueryLogConfigAssociationsPaginator

session = get_session()
async with session.create_client("route53resolver") as client:  # (1)
    paginator: ListResolverQueryLogConfigAssociationsPaginator = client.get_paginator("list_resolver_query_log_config_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListResolverQueryLogConfigAssociationsResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53ResolverClient](./client.md)
2. paginator: [ListResolverQueryLogConfigAssociationsPaginator](./paginators.md#listresolverquerylogconfigassociationspaginator)
3. item: [:material-code-braces: ListResolverQueryLogConfigAssociationsResponseTypeDef](./type_defs.md#listresolverquerylogconfigassociationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListResolverQueryLogConfigAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    SortBy: str = ...,
    SortOrder: SortOrderType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListResolverQueryLogConfigAssociationsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListResolverQueryLogConfigAssociationsResponseTypeDef](./type_defs.md#listresolverquerylogconfigassociationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListResolverQueryLogConfigAssociationsRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResolverQueryLogConfigAssociationsRequestPaginateTypeDef](./type_defs.md#listresolverquerylogconfigassociationsrequestpaginatetypedef) 
## ListResolverQueryLogConfigsPaginator

Type annotations and code completion for `#!python session.create_client("route53resolver").get_paginator("list_resolver_query_log_configs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver/paginator/ListResolverQueryLogConfigs.html#Route53Resolver.Paginator.ListResolverQueryLogConfigs)

```python
# ListResolverQueryLogConfigsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.paginator import ListResolverQueryLogConfigsPaginator

session = get_session()
async with session.create_client("route53resolver") as client:  # (1)
    paginator: ListResolverQueryLogConfigsPaginator = client.get_paginator("list_resolver_query_log_configs")  # (2)
    async for item in paginator.paginate(...):
        item: ListResolverQueryLogConfigsResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53ResolverClient](./client.md)
2. paginator: [ListResolverQueryLogConfigsPaginator](./paginators.md#listresolverquerylogconfigspaginator)
3. item: [:material-code-braces: ListResolverQueryLogConfigsResponseTypeDef](./type_defs.md#listresolverquerylogconfigsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListResolverQueryLogConfigsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    SortBy: str = ...,
    SortOrder: SortOrderType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListResolverQueryLogConfigsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListResolverQueryLogConfigsResponseTypeDef](./type_defs.md#listresolverquerylogconfigsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListResolverQueryLogConfigsRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResolverQueryLogConfigsRequestPaginateTypeDef](./type_defs.md#listresolverquerylogconfigsrequestpaginatetypedef) 
## ListResolverRuleAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("route53resolver").get_paginator("list_resolver_rule_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver/paginator/ListResolverRuleAssociations.html#Route53Resolver.Paginator.ListResolverRuleAssociations)

```python
# ListResolverRuleAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.paginator import ListResolverRuleAssociationsPaginator

session = get_session()
async with session.create_client("route53resolver") as client:  # (1)
    paginator: ListResolverRuleAssociationsPaginator = client.get_paginator("list_resolver_rule_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListResolverRuleAssociationsResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53ResolverClient](./client.md)
2. paginator: [ListResolverRuleAssociationsPaginator](./paginators.md#listresolverruleassociationspaginator)
3. item: [:material-code-braces: ListResolverRuleAssociationsResponseTypeDef](./type_defs.md#listresolverruleassociationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListResolverRuleAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListResolverRuleAssociationsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListResolverRuleAssociationsResponseTypeDef](./type_defs.md#listresolverruleassociationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListResolverRuleAssociationsRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResolverRuleAssociationsRequestPaginateTypeDef](./type_defs.md#listresolverruleassociationsrequestpaginatetypedef) 
## ListResolverRulesPaginator

Type annotations and code completion for `#!python session.create_client("route53resolver").get_paginator("list_resolver_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver/paginator/ListResolverRules.html#Route53Resolver.Paginator.ListResolverRules)

```python
# ListResolverRulesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.paginator import ListResolverRulesPaginator

session = get_session()
async with session.create_client("route53resolver") as client:  # (1)
    paginator: ListResolverRulesPaginator = client.get_paginator("list_resolver_rules")  # (2)
    async for item in paginator.paginate(...):
        item: ListResolverRulesResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53ResolverClient](./client.md)
2. paginator: [ListResolverRulesPaginator](./paginators.md#listresolverrulespaginator)
3. item: [:material-code-braces: ListResolverRulesResponseTypeDef](./type_defs.md#listresolverrulesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListResolverRulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListResolverRulesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListResolverRulesResponseTypeDef](./type_defs.md#listresolverrulesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListResolverRulesRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResolverRulesRequestPaginateTypeDef](./type_defs.md#listresolverrulesrequestpaginatetypedef) 
## ListTagsForResourcePaginator

Type annotations and code completion for `#!python session.create_client("route53resolver").get_paginator("list_tags_for_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver/paginator/ListTagsForResource.html#Route53Resolver.Paginator.ListTagsForResource)

```python
# ListTagsForResourcePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("route53resolver") as client:  # (1)
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")  # (2)
    async for item in paginator.paginate(...):
        item: ListTagsForResourceResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53ResolverClient](./client.md)
2. paginator: [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
3. item: [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTagsForResourcePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTagsForResourceResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTagsForResourceRequestPaginateTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestPaginateTypeDef](./type_defs.md#listtagsforresourcerequestpaginatetypedef) 
