# Paginators

> [Index](../README.md) > [Route53GlobalResolver](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Route53GlobalResolver](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53globalresolver.html#route53globalresolver)
    type annotations stubs module [types-aiobotocore-route53globalresolver](https://pypi.org/project/types-aiobotocore-route53globalresolver/).

## ListAccessSourcesPaginator

Type annotations and code completion for `#!python session.create_client("route53globalresolver").get_paginator("list_access_sources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53globalresolver/paginator/ListAccessSources.html#Route53GlobalResolver.Paginator.ListAccessSources)

```python
# ListAccessSourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53globalresolver.paginator import ListAccessSourcesPaginator

session = get_session()
async with session.create_client("route53globalresolver") as client:  # (1)
    paginator: ListAccessSourcesPaginator = client.get_paginator("list_access_sources")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccessSourcesOutputTypeDef
        print(item)  # (3)
```

1. client: [Route53GlobalResolverClient](./client.md)
2. paginator: [ListAccessSourcesPaginator](./paginators.md#listaccesssourcespaginator)
3. item: `AioPageIterator[ListAccessSourcesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAccessSourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Mapping[str, Sequence[str]] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAccessSourcesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAccessSourcesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAccessSourcesInputPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccessSourcesInputPaginateTypeDef](./type_defs.md#listaccesssourcesinputpaginatetypedef)
## ListAccessTokensPaginator

Type annotations and code completion for `#!python session.create_client("route53globalresolver").get_paginator("list_access_tokens")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53globalresolver/paginator/ListAccessTokens.html#Route53GlobalResolver.Paginator.ListAccessTokens)

```python
# ListAccessTokensPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53globalresolver.paginator import ListAccessTokensPaginator

session = get_session()
async with session.create_client("route53globalresolver") as client:  # (1)
    paginator: ListAccessTokensPaginator = client.get_paginator("list_access_tokens")  # (2)
    async for item in paginator.paginate(...):
        item: ListAccessTokensOutputTypeDef
        print(item)  # (3)
```

1. client: [Route53GlobalResolverClient](./client.md)
2. paginator: [ListAccessTokensPaginator](./paginators.md#listaccesstokenspaginator)
3. item: `AioPageIterator[ListAccessTokensOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAccessTokensPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    dnsViewId: str,
    filters: Mapping[str, Sequence[str]] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAccessTokensOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAccessTokensOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAccessTokensInputPaginateTypeDef = {  # (1)
    "dnsViewId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccessTokensInputPaginateTypeDef](./type_defs.md#listaccesstokensinputpaginatetypedef)
## ListDNSViewsPaginator

Type annotations and code completion for `#!python session.create_client("route53globalresolver").get_paginator("list_dns_views")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53globalresolver/paginator/ListDNSViews.html#Route53GlobalResolver.Paginator.ListDNSViews)

```python
# ListDNSViewsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53globalresolver.paginator import ListDNSViewsPaginator

session = get_session()
async with session.create_client("route53globalresolver") as client:  # (1)
    paginator: ListDNSViewsPaginator = client.get_paginator("list_dns_views")  # (2)
    async for item in paginator.paginate(...):
        item: ListDNSViewsOutputTypeDef
        print(item)  # (3)
```

1. client: [Route53GlobalResolverClient](./client.md)
2. paginator: [ListDNSViewsPaginator](./paginators.md#listdnsviewspaginator)
3. item: `AioPageIterator[ListDNSViewsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDNSViewsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    globalResolverId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDNSViewsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDNSViewsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDNSViewsInputPaginateTypeDef = {  # (1)
    "globalResolverId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDNSViewsInputPaginateTypeDef](./type_defs.md#listdnsviewsinputpaginatetypedef)
## ListFirewallDomainListsPaginator

Type annotations and code completion for `#!python session.create_client("route53globalresolver").get_paginator("list_firewall_domain_lists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53globalresolver/paginator/ListFirewallDomainLists.html#Route53GlobalResolver.Paginator.ListFirewallDomainLists)

```python
# ListFirewallDomainListsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53globalresolver.paginator import ListFirewallDomainListsPaginator

session = get_session()
async with session.create_client("route53globalresolver") as client:  # (1)
    paginator: ListFirewallDomainListsPaginator = client.get_paginator("list_firewall_domain_lists")  # (2)
    async for item in paginator.paginate(...):
        item: ListFirewallDomainListsOutputTypeDef
        print(item)  # (3)
```

1. client: [Route53GlobalResolverClient](./client.md)
2. paginator: [ListFirewallDomainListsPaginator](./paginators.md#listfirewalldomainlistspaginator)
3. item: `AioPageIterator[ListFirewallDomainListsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFirewallDomainListsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    globalResolverId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListFirewallDomainListsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListFirewallDomainListsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFirewallDomainListsInputPaginateTypeDef = {  # (1)
    "globalResolverId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFirewallDomainListsInputPaginateTypeDef](./type_defs.md#listfirewalldomainlistsinputpaginatetypedef)
## ListFirewallDomainsPaginator

Type annotations and code completion for `#!python session.create_client("route53globalresolver").get_paginator("list_firewall_domains")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53globalresolver/paginator/ListFirewallDomains.html#Route53GlobalResolver.Paginator.ListFirewallDomains)

```python
# ListFirewallDomainsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53globalresolver.paginator import ListFirewallDomainsPaginator

session = get_session()
async with session.create_client("route53globalresolver") as client:  # (1)
    paginator: ListFirewallDomainsPaginator = client.get_paginator("list_firewall_domains")  # (2)
    async for item in paginator.paginate(...):
        item: ListFirewallDomainsOutputTypeDef
        print(item)  # (3)
```

1. client: [Route53GlobalResolverClient](./client.md)
2. paginator: [ListFirewallDomainsPaginator](./paginators.md#listfirewalldomainspaginator)
3. item: `AioPageIterator[ListFirewallDomainsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFirewallDomainsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    firewallDomainListId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListFirewallDomainsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListFirewallDomainsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFirewallDomainsInputPaginateTypeDef = {  # (1)
    "firewallDomainListId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFirewallDomainsInputPaginateTypeDef](./type_defs.md#listfirewalldomainsinputpaginatetypedef)
## ListFirewallRulesPaginator

Type annotations and code completion for `#!python session.create_client("route53globalresolver").get_paginator("list_firewall_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53globalresolver/paginator/ListFirewallRules.html#Route53GlobalResolver.Paginator.ListFirewallRules)

```python
# ListFirewallRulesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53globalresolver.paginator import ListFirewallRulesPaginator

session = get_session()
async with session.create_client("route53globalresolver") as client:  # (1)
    paginator: ListFirewallRulesPaginator = client.get_paginator("list_firewall_rules")  # (2)
    async for item in paginator.paginate(...):
        item: ListFirewallRulesOutputTypeDef
        print(item)  # (3)
```

1. client: [Route53GlobalResolverClient](./client.md)
2. paginator: [ListFirewallRulesPaginator](./paginators.md#listfirewallrulespaginator)
3. item: `AioPageIterator[ListFirewallRulesOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFirewallRulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    dnsViewId: str,
    filters: Mapping[str, Sequence[str]] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListFirewallRulesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListFirewallRulesOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFirewallRulesInputPaginateTypeDef = {  # (1)
    "dnsViewId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFirewallRulesInputPaginateTypeDef](./type_defs.md#listfirewallrulesinputpaginatetypedef)
## ListGlobalResolversPaginator

Type annotations and code completion for `#!python session.create_client("route53globalresolver").get_paginator("list_global_resolvers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53globalresolver/paginator/ListGlobalResolvers.html#Route53GlobalResolver.Paginator.ListGlobalResolvers)

```python
# ListGlobalResolversPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53globalresolver.paginator import ListGlobalResolversPaginator

session = get_session()
async with session.create_client("route53globalresolver") as client:  # (1)
    paginator: ListGlobalResolversPaginator = client.get_paginator("list_global_resolvers")  # (2)
    async for item in paginator.paginate(...):
        item: ListGlobalResolversOutputTypeDef
        print(item)  # (3)
```

1. client: [Route53GlobalResolverClient](./client.md)
2. paginator: [ListGlobalResolversPaginator](./paginators.md#listglobalresolverspaginator)
3. item: `AioPageIterator[ListGlobalResolversOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListGlobalResolversPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListGlobalResolversOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListGlobalResolversOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListGlobalResolversInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGlobalResolversInputPaginateTypeDef](./type_defs.md#listglobalresolversinputpaginatetypedef)
## ListHostedZoneAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("route53globalresolver").get_paginator("list_hosted_zone_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53globalresolver/paginator/ListHostedZoneAssociations.html#Route53GlobalResolver.Paginator.ListHostedZoneAssociations)

```python
# ListHostedZoneAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53globalresolver.paginator import ListHostedZoneAssociationsPaginator

session = get_session()
async with session.create_client("route53globalresolver") as client:  # (1)
    paginator: ListHostedZoneAssociationsPaginator = client.get_paginator("list_hosted_zone_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListHostedZoneAssociationsOutputTypeDef
        print(item)  # (3)
```

1. client: [Route53GlobalResolverClient](./client.md)
2. paginator: [ListHostedZoneAssociationsPaginator](./paginators.md#listhostedzoneassociationspaginator)
3. item: `AioPageIterator[ListHostedZoneAssociationsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListHostedZoneAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    resourceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListHostedZoneAssociationsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListHostedZoneAssociationsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListHostedZoneAssociationsInputPaginateTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListHostedZoneAssociationsInputPaginateTypeDef](./type_defs.md#listhostedzoneassociationsinputpaginatetypedef)
## ListManagedFirewallDomainListsPaginator

Type annotations and code completion for `#!python session.create_client("route53globalresolver").get_paginator("list_managed_firewall_domain_lists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53globalresolver/paginator/ListManagedFirewallDomainLists.html#Route53GlobalResolver.Paginator.ListManagedFirewallDomainLists)

```python
# ListManagedFirewallDomainListsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53globalresolver.paginator import ListManagedFirewallDomainListsPaginator

session = get_session()
async with session.create_client("route53globalresolver") as client:  # (1)
    paginator: ListManagedFirewallDomainListsPaginator = client.get_paginator("list_managed_firewall_domain_lists")  # (2)
    async for item in paginator.paginate(...):
        item: ListManagedFirewallDomainListsOutputTypeDef
        print(item)  # (3)
```

1. client: [Route53GlobalResolverClient](./client.md)
2. paginator: [ListManagedFirewallDomainListsPaginator](./paginators.md#listmanagedfirewalldomainlistspaginator)
3. item: `AioPageIterator[ListManagedFirewallDomainListsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListManagedFirewallDomainListsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    managedFirewallDomainListType: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListManagedFirewallDomainListsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListManagedFirewallDomainListsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListManagedFirewallDomainListsInputPaginateTypeDef = {  # (1)
    "managedFirewallDomainListType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListManagedFirewallDomainListsInputPaginateTypeDef](./type_defs.md#listmanagedfirewalldomainlistsinputpaginatetypedef)
