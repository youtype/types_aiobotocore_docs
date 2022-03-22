<a id="paginators-for-aiobotocore-route53resolver-module"></a>

# Paginators for aiobotocore Route53Resolver module

> [Index](../README.md) > [Route53Resolver](./README.md) > Paginators

Auto-generated documentation for
[Route53Resolver](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver)
type annotations stubs module
[types-aiobotocore-route53resolver](https://pypi.org/project/types-aiobotocore-route53resolver/).

- [Paginators for aiobotocore Route53Resolver module](#paginators-for-aiobotocore-route53resolver-module)
  - [ListFirewallConfigsPaginator](#listfirewallconfigspaginator)
  - [ListFirewallDomainListsPaginator](#listfirewalldomainlistspaginator)
  - [ListFirewallDomainsPaginator](#listfirewalldomainspaginator)
  - [ListFirewallRuleGroupAssociationsPaginator](#listfirewallrulegroupassociationspaginator)
  - [ListFirewallRuleGroupsPaginator](#listfirewallrulegroupspaginator)
  - [ListFirewallRulesPaginator](#listfirewallrulespaginator)
  - [ListResolverConfigsPaginator](#listresolverconfigspaginator)
  - [ListResolverDnssecConfigsPaginator](#listresolverdnssecconfigspaginator)
  - [ListResolverEndpointIpAddressesPaginator](#listresolverendpointipaddressespaginator)
  - [ListResolverEndpointsPaginator](#listresolverendpointspaginator)
  - [ListResolverQueryLogConfigAssociationsPaginator](#listresolverquerylogconfigassociationspaginator)
  - [ListResolverQueryLogConfigsPaginator](#listresolverquerylogconfigspaginator)
  - [ListResolverRuleAssociationsPaginator](#listresolverruleassociationspaginator)
  - [ListResolverRulesPaginator](#listresolverrulespaginator)
  - [ListTagsForResourcePaginator](#listtagsforresourcepaginator)

<a id="listfirewallconfigspaginator"></a>

## ListFirewallConfigsPaginator

Type annotations for
`session.create_client("route53resolver").get_paginator("list_firewall_configs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.paginator import ListFirewallConfigsPaginator

session = get_session()
async with session.create_client("route53resolver") as client:
    client: Route53ResolverClient
    paginator: ListFirewallConfigsPaginator = client.get_paginator("list_firewall_configs")
```

Boto3 documentation:
[Route53Resolver.Paginator.ListFirewallConfigs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallConfigs)

Arguments for `ListFirewallConfigsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListFirewallConfigsPaginator.paginate` returns
`AsyncIterator`\[[ListFirewallConfigsResponseTypeDef](./type_defs.md#listfirewallconfigsresponsetypedef)\].

<a id="listfirewalldomainlistspaginator"></a>

## ListFirewallDomainListsPaginator

Type annotations for
`session.create_client("route53resolver").get_paginator("list_firewall_domain_lists")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.paginator import ListFirewallDomainListsPaginator

session = get_session()
async with session.create_client("route53resolver") as client:
    client: Route53ResolverClient
    paginator: ListFirewallDomainListsPaginator = client.get_paginator("list_firewall_domain_lists")
```

Boto3 documentation:
[Route53Resolver.Paginator.ListFirewallDomainLists](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallDomainLists)

Arguments for `ListFirewallDomainListsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListFirewallDomainListsPaginator.paginate` returns
`AsyncIterator`\[[ListFirewallDomainListsResponseTypeDef](./type_defs.md#listfirewalldomainlistsresponsetypedef)\].

<a id="listfirewalldomainspaginator"></a>

## ListFirewallDomainsPaginator

Type annotations for
`session.create_client("route53resolver").get_paginator("list_firewall_domains")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.paginator import ListFirewallDomainsPaginator

session = get_session()
async with session.create_client("route53resolver") as client:
    client: Route53ResolverClient
    paginator: ListFirewallDomainsPaginator = client.get_paginator("list_firewall_domains")
```

Boto3 documentation:
[Route53Resolver.Paginator.ListFirewallDomains](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallDomains)

Arguments for `ListFirewallDomainsPaginator.paginate` method:

- `FirewallDomainListId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListFirewallDomainsPaginator.paginate` returns
`AsyncIterator`\[[ListFirewallDomainsResponseTypeDef](./type_defs.md#listfirewalldomainsresponsetypedef)\].

<a id="listfirewallrulegroupassociationspaginator"></a>

## ListFirewallRuleGroupAssociationsPaginator

Type annotations for
`session.create_client("route53resolver").get_paginator("list_firewall_rule_group_associations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.paginator import ListFirewallRuleGroupAssociationsPaginator

session = get_session()
async with session.create_client("route53resolver") as client:
    client: Route53ResolverClient
    paginator: ListFirewallRuleGroupAssociationsPaginator = client.get_paginator("list_firewall_rule_group_associations")
```

Boto3 documentation:
[Route53Resolver.Paginator.ListFirewallRuleGroupAssociations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallRuleGroupAssociations)

Arguments for `ListFirewallRuleGroupAssociationsPaginator.paginate` method:

- `FirewallRuleGroupId`: `str`
- `VpcId`: `str`
- `Priority`: `int`
- `Status`:
  [FirewallRuleGroupAssociationStatusType](./literals.md#firewallrulegroupassociationstatustype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListFirewallRuleGroupAssociationsPaginator.paginate` returns
`AsyncIterator`\[[ListFirewallRuleGroupAssociationsResponseTypeDef](./type_defs.md#listfirewallrulegroupassociationsresponsetypedef)\].

<a id="listfirewallrulegroupspaginator"></a>

## ListFirewallRuleGroupsPaginator

Type annotations for
`session.create_client("route53resolver").get_paginator("list_firewall_rule_groups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.paginator import ListFirewallRuleGroupsPaginator

session = get_session()
async with session.create_client("route53resolver") as client:
    client: Route53ResolverClient
    paginator: ListFirewallRuleGroupsPaginator = client.get_paginator("list_firewall_rule_groups")
```

Boto3 documentation:
[Route53Resolver.Paginator.ListFirewallRuleGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallRuleGroups)

Arguments for `ListFirewallRuleGroupsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListFirewallRuleGroupsPaginator.paginate` returns
`AsyncIterator`\[[ListFirewallRuleGroupsResponseTypeDef](./type_defs.md#listfirewallrulegroupsresponsetypedef)\].

<a id="listfirewallrulespaginator"></a>

## ListFirewallRulesPaginator

Type annotations for
`session.create_client("route53resolver").get_paginator("list_firewall_rules")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.paginator import ListFirewallRulesPaginator

session = get_session()
async with session.create_client("route53resolver") as client:
    client: Route53ResolverClient
    paginator: ListFirewallRulesPaginator = client.get_paginator("list_firewall_rules")
```

Boto3 documentation:
[Route53Resolver.Paginator.ListFirewallRules](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListFirewallRules)

Arguments for `ListFirewallRulesPaginator.paginate` method:

- `FirewallRuleGroupId`: `str` *(required)*
- `Priority`: `int`
- `Action`: [ActionType](./literals.md#actiontype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListFirewallRulesPaginator.paginate` returns
`AsyncIterator`\[[ListFirewallRulesResponseTypeDef](./type_defs.md#listfirewallrulesresponsetypedef)\].

<a id="listresolverconfigspaginator"></a>

## ListResolverConfigsPaginator

Type annotations for
`session.create_client("route53resolver").get_paginator("list_resolver_configs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.paginator import ListResolverConfigsPaginator

session = get_session()
async with session.create_client("route53resolver") as client:
    client: Route53ResolverClient
    paginator: ListResolverConfigsPaginator = client.get_paginator("list_resolver_configs")
```

Boto3 documentation:
[Route53Resolver.Paginator.ListResolverConfigs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverConfigs)

Arguments for `ListResolverConfigsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListResolverConfigsPaginator.paginate` returns
`AsyncIterator`\[[ListResolverConfigsResponseTypeDef](./type_defs.md#listresolverconfigsresponsetypedef)\].

<a id="listresolverdnssecconfigspaginator"></a>

## ListResolverDnssecConfigsPaginator

Type annotations for
`session.create_client("route53resolver").get_paginator("list_resolver_dnssec_configs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.paginator import ListResolverDnssecConfigsPaginator

session = get_session()
async with session.create_client("route53resolver") as client:
    client: Route53ResolverClient
    paginator: ListResolverDnssecConfigsPaginator = client.get_paginator("list_resolver_dnssec_configs")
```

Boto3 documentation:
[Route53Resolver.Paginator.ListResolverDnssecConfigs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverDnssecConfigs)

Arguments for `ListResolverDnssecConfigsPaginator.paginate` method:

- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListResolverDnssecConfigsPaginator.paginate` returns
`AsyncIterator`\[[ListResolverDnssecConfigsResponseTypeDef](./type_defs.md#listresolverdnssecconfigsresponsetypedef)\].

<a id="listresolverendpointipaddressespaginator"></a>

## ListResolverEndpointIpAddressesPaginator

Type annotations for
`session.create_client("route53resolver").get_paginator("list_resolver_endpoint_ip_addresses")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.paginator import ListResolverEndpointIpAddressesPaginator

session = get_session()
async with session.create_client("route53resolver") as client:
    client: Route53ResolverClient
    paginator: ListResolverEndpointIpAddressesPaginator = client.get_paginator("list_resolver_endpoint_ip_addresses")
```

Boto3 documentation:
[Route53Resolver.Paginator.ListResolverEndpointIpAddresses](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverEndpointIpAddresses)

Arguments for `ListResolverEndpointIpAddressesPaginator.paginate` method:

- `ResolverEndpointId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListResolverEndpointIpAddressesPaginator.paginate` returns
`AsyncIterator`\[[ListResolverEndpointIpAddressesResponseTypeDef](./type_defs.md#listresolverendpointipaddressesresponsetypedef)\].

<a id="listresolverendpointspaginator"></a>

## ListResolverEndpointsPaginator

Type annotations for
`session.create_client("route53resolver").get_paginator("list_resolver_endpoints")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.paginator import ListResolverEndpointsPaginator

session = get_session()
async with session.create_client("route53resolver") as client:
    client: Route53ResolverClient
    paginator: ListResolverEndpointsPaginator = client.get_paginator("list_resolver_endpoints")
```

Boto3 documentation:
[Route53Resolver.Paginator.ListResolverEndpoints](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverEndpoints)

Arguments for `ListResolverEndpointsPaginator.paginate` method:

- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListResolverEndpointsPaginator.paginate` returns
`AsyncIterator`\[[ListResolverEndpointsResponseTypeDef](./type_defs.md#listresolverendpointsresponsetypedef)\].

<a id="listresolverquerylogconfigassociationspaginator"></a>

## ListResolverQueryLogConfigAssociationsPaginator

Type annotations for
`session.create_client("route53resolver").get_paginator("list_resolver_query_log_config_associations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.paginator import ListResolverQueryLogConfigAssociationsPaginator

session = get_session()
async with session.create_client("route53resolver") as client:
    client: Route53ResolverClient
    paginator: ListResolverQueryLogConfigAssociationsPaginator = client.get_paginator("list_resolver_query_log_config_associations")
```

Boto3 documentation:
[Route53Resolver.Paginator.ListResolverQueryLogConfigAssociations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverQueryLogConfigAssociations)

Arguments for `ListResolverQueryLogConfigAssociationsPaginator.paginate`
method:

- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `SortBy`: `str`
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListResolverQueryLogConfigAssociationsPaginator.paginate` returns
`AsyncIterator`\[[ListResolverQueryLogConfigAssociationsResponseTypeDef](./type_defs.md#listresolverquerylogconfigassociationsresponsetypedef)\].

<a id="listresolverquerylogconfigspaginator"></a>

## ListResolverQueryLogConfigsPaginator

Type annotations for
`session.create_client("route53resolver").get_paginator("list_resolver_query_log_configs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.paginator import ListResolverQueryLogConfigsPaginator

session = get_session()
async with session.create_client("route53resolver") as client:
    client: Route53ResolverClient
    paginator: ListResolverQueryLogConfigsPaginator = client.get_paginator("list_resolver_query_log_configs")
```

Boto3 documentation:
[Route53Resolver.Paginator.ListResolverQueryLogConfigs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverQueryLogConfigs)

Arguments for `ListResolverQueryLogConfigsPaginator.paginate` method:

- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `SortBy`: `str`
- `SortOrder`: [SortOrderType](./literals.md#sortordertype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListResolverQueryLogConfigsPaginator.paginate` returns
`AsyncIterator`\[[ListResolverQueryLogConfigsResponseTypeDef](./type_defs.md#listresolverquerylogconfigsresponsetypedef)\].

<a id="listresolverruleassociationspaginator"></a>

## ListResolverRuleAssociationsPaginator

Type annotations for
`session.create_client("route53resolver").get_paginator("list_resolver_rule_associations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.paginator import ListResolverRuleAssociationsPaginator

session = get_session()
async with session.create_client("route53resolver") as client:
    client: Route53ResolverClient
    paginator: ListResolverRuleAssociationsPaginator = client.get_paginator("list_resolver_rule_associations")
```

Boto3 documentation:
[Route53Resolver.Paginator.ListResolverRuleAssociations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverRuleAssociations)

Arguments for `ListResolverRuleAssociationsPaginator.paginate` method:

- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListResolverRuleAssociationsPaginator.paginate` returns
`AsyncIterator`\[[ListResolverRuleAssociationsResponseTypeDef](./type_defs.md#listresolverruleassociationsresponsetypedef)\].

<a id="listresolverrulespaginator"></a>

## ListResolverRulesPaginator

Type annotations for
`session.create_client("route53resolver").get_paginator("list_resolver_rules")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.paginator import ListResolverRulesPaginator

session = get_session()
async with session.create_client("route53resolver") as client:
    client: Route53ResolverClient
    paginator: ListResolverRulesPaginator = client.get_paginator("list_resolver_rules")
```

Boto3 documentation:
[Route53Resolver.Paginator.ListResolverRules](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListResolverRules)

Arguments for `ListResolverRulesPaginator.paginate` method:

- `Filters`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListResolverRulesPaginator.paginate` returns
`AsyncIterator`\[[ListResolverRulesResponseTypeDef](./type_defs.md#listresolverrulesresponsetypedef)\].

<a id="listtagsforresourcepaginator"></a>

## ListTagsForResourcePaginator

Type annotations for
`session.create_client("route53resolver").get_paginator("list_tags_for_resource")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("route53resolver") as client:
    client: Route53ResolverClient
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
```

Boto3 documentation:
[Route53Resolver.Paginator.ListTagsForResource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#Route53Resolver.Paginator.ListTagsForResource)

Arguments for `ListTagsForResourcePaginator.paginate` method:

- `ResourceArn`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTagsForResourcePaginator.paginate` returns
`AsyncIterator`\[[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)\].
