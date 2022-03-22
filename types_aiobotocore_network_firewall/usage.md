<a id="examples-for-aiobotocore-networkfirewall-module"></a>

# Examples for aiobotocore NetworkFirewall module

> [Index](../README.md) > [NetworkFirewall](./README.md) > Examples

- [Examples for aiobotocore NetworkFirewall module](#examples-for-aiobotocore-networkfirewall-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[network-firewall]` package installed.

Write your `NetworkFirewall` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type NetworkFirewallClient
# and provides type checking and code completion
async with session.create_client("network-firewall") as client:
    
    # result has type AssociateFirewallPolicyResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_firewall_policy()
    

    
    # paginator has type ListFirewallPoliciesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_firewall_policies")
    async for item in paginator.paginate(...):
        # item has type ListFirewallPoliciesResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[network-firewall]` or a standalone
`types_aiobotocore_network_firewall` package, you have to explicitly specify
`client: NetworkFirewallClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_network_firewall.client import NetworkFirewallClient
from types_aiobotocore_network_firewall.type_defs import AssociateFirewallPolicyResponseTypeDef
from types_aiobotocore_network_firewall.paginator import ListFirewallPoliciesPaginator

from types_aiobotocore_network_firewall.literals import PaginatorName



session = get_session()

async with session.create_client("network-firewall") as client:
    client: NetworkFirewallClient

    
    result: AssociateFirewallPolicyResponseTypeDef = client.associate_firewall_policy()
    

    
    paginator_name: PaginatorName = "list_firewall_policies"
    paginator: ListFirewallPoliciesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListFirewallPoliciesResponseTypeDef
        print(item)
    

    
```
