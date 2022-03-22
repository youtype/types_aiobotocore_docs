<a id="examples-for-aiobotocore-route53resolver-module"></a>

# Examples for aiobotocore Route53Resolver module

> [Index](../README.md) > [Route53Resolver](./README.md) > Examples

- [Examples for aiobotocore Route53Resolver module](#examples-for-aiobotocore-route53resolver-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[route53resolver]` package installed.

Write your `Route53Resolver` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type Route53ResolverClient
# and provides type checking and code completion
async with session.create_client("route53resolver") as client:
    
    # result has type AssociateFirewallRuleGroupResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_firewall_rule_group()
    

    
    # paginator has type ListFirewallConfigsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_firewall_configs")
    async for item in paginator.paginate(...):
        # item has type ListFirewallConfigsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[route53resolver]` or a standalone
`types_aiobotocore_route53resolver` package, you have to explicitly specify
`client: Route53ResolverClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.client import Route53ResolverClient
from types_aiobotocore_route53resolver.type_defs import AssociateFirewallRuleGroupResponseTypeDef
from types_aiobotocore_route53resolver.paginator import ListFirewallConfigsPaginator

from types_aiobotocore_route53resolver.literals import PaginatorName



session = get_session()

async with session.create_client("route53resolver") as client:
    client: Route53ResolverClient

    
    result: AssociateFirewallRuleGroupResponseTypeDef = client.associate_firewall_rule_group()
    

    
    paginator_name: PaginatorName = "list_firewall_configs"
    paginator: ListFirewallConfigsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListFirewallConfigsResponseTypeDef
        print(item)
    

    
```
