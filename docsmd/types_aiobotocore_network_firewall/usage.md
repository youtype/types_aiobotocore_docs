# Examples

> [Index](../README.md) > [NetworkFirewall](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [NetworkFirewall](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#networkfirewall)
    type annotations stubs module [types-aiobotocore-network-firewall](https://pypi.org/project/types-aiobotocore-network-firewall/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[network-firewall]` package installed.

Write your `NetworkFirewall` code as usual,
type checking and code completion should work out of the box.



```python
# NetworkFirewallClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("network-firewall") as client:  # (1)
    result = await client.associate_firewall_policy()  # (2)
```

1. client: [NetworkFirewallClient](./client.md)
2. result: [:material-code-braces: AssociateFirewallPolicyResponseTypeDef](./type_defs.md#associatefirewallpolicyresponsetypedef) 



```python
# GetAnalysisReportResultsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("network-firewall") as client:  # (1)
    paginator = client.get_paginator("get_analysis_report_results")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [NetworkFirewallClient](./client.md)
2. paginator: [GetAnalysisReportResultsPaginator](./paginators.md#getanalysisreportresultspaginator)
3. item: [:material-code-braces: GetAnalysisReportResultsResponseTypeDef](./type_defs.md#getanalysisreportresultsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[network-firewall]`
or a standalone `types_aiobotocore_network_firewall` package, you have to explicitly specify
`client: NetworkFirewallClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# NetworkFirewallClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_network_firewall.client import NetworkFirewallClient
from types_aiobotocore_network_firewall.type_defs import AssociateFirewallPolicyResponseTypeDef
from types_aiobotocore_network_firewall.type_defs import AssociateFirewallPolicyRequestTypeDef


session = get_session()

async with session.create_client("network-firewall") as client:
    client: NetworkFirewallClient
    kwargs: AssociateFirewallPolicyRequestTypeDef = {...}
    result: AssociateFirewallPolicyResponseTypeDef = await client.associate_firewall_policy(**kwargs)
```



```python
# GetAnalysisReportResultsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_network_firewall.client import NetworkFirewallClient
from types_aiobotocore_network_firewall.paginator import GetAnalysisReportResultsPaginator
from types_aiobotocore_network_firewall.type_defs import GetAnalysisReportResultsResponseTypeDef


session = get_session()

async with session.create_client("network-firewall") as client:
    client: NetworkFirewallClient
    paginator: GetAnalysisReportResultsPaginator = client.get_paginator("get_analysis_report_results")
    async for item in paginator.paginate(...):
        item: GetAnalysisReportResultsResponseTypeDef
        print(item)
```


