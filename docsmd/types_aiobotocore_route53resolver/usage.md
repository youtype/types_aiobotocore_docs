# Examples

> [Index](../README.md) > [Route53Resolver](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Route53Resolver](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#route53resolver)
    type annotations stubs module [types-aiobotocore-route53resolver](https://pypi.org/project/types-aiobotocore-route53resolver/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[route53resolver]` package installed.

Write your `Route53Resolver` code as usual,
type checking and code completion should work out of the box.



```python
# Route53ResolverClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("route53resolver") as client:  # (1)
    result = await client.associate_firewall_rule_group()  # (2)
```

1. client: [Route53ResolverClient](./client.md)
2. result: [:material-code-braces: AssociateFirewallRuleGroupResponseTypeDef](./type_defs.md#associatefirewallrulegroupresponsetypedef) 



```python
# ListFirewallConfigsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("route53resolver") as client:  # (1)
    paginator = client.get_paginator("list_firewall_configs")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [Route53ResolverClient](./client.md)
2. paginator: [ListFirewallConfigsPaginator](./paginators.md#listfirewallconfigspaginator)
3. item: [:material-code-braces: ListFirewallConfigsResponseTypeDef](./type_defs.md#listfirewallconfigsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[route53resolver]`
or a standalone `types_aiobotocore_route53resolver` package, you have to explicitly specify
`client: Route53ResolverClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# Route53ResolverClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.client import Route53ResolverClient
from types_aiobotocore_route53resolver.type_defs import AssociateFirewallRuleGroupResponseTypeDef
from types_aiobotocore_route53resolver.type_defs import AssociateFirewallRuleGroupRequestTypeDef


session = get_session()

async with session.create_client("route53resolver") as client:
    client: Route53ResolverClient
    kwargs: AssociateFirewallRuleGroupRequestTypeDef = {...}
    result: AssociateFirewallRuleGroupResponseTypeDef = await client.associate_firewall_rule_group(**kwargs)
```



```python
# ListFirewallConfigsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_route53resolver.client import Route53ResolverClient
from types_aiobotocore_route53resolver.paginator import ListFirewallConfigsPaginator
from types_aiobotocore_route53resolver.type_defs import ListFirewallConfigsResponseTypeDef


session = get_session()

async with session.create_client("route53resolver") as client:
    client: Route53ResolverClient
    paginator: ListFirewallConfigsPaginator = client.get_paginator("list_firewall_configs")
    async for item in paginator.paginate(...):
        item: ListFirewallConfigsResponseTypeDef
        print(item)
```


