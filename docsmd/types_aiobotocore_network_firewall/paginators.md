# Paginators

> [Index](../README.md) > [NetworkFirewall](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [NetworkFirewall](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#networkfirewall)
    type annotations stubs module [types-aiobotocore-network-firewall](https://pypi.org/project/types-aiobotocore-network-firewall/).

## GetAnalysisReportResultsPaginator

Type annotations and code completion for `#!python session.create_client("network-firewall").get_paginator("get_analysis_report_results")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall/paginator/GetAnalysisReportResults.html#NetworkFirewall.Paginator.GetAnalysisReportResults)

```python
# GetAnalysisReportResultsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_network_firewall.paginator import GetAnalysisReportResultsPaginator

session = get_session()
async with session.create_client("network-firewall") as client:  # (1)
    paginator: GetAnalysisReportResultsPaginator = client.get_paginator("get_analysis_report_results")  # (2)
    async for item in paginator.paginate(...):
        item: GetAnalysisReportResultsResponseTypeDef
        print(item)  # (3)
```

1. client: [NetworkFirewallClient](./client.md)
2. paginator: [GetAnalysisReportResultsPaginator](./paginators.md#getanalysisreportresultspaginator)
3. item: `AioPageIterator[GetAnalysisReportResultsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetAnalysisReportResultsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AnalysisReportId: str,
    FirewallName: str = ...,
    FirewallArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetAnalysisReportResultsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetAnalysisReportResultsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetAnalysisReportResultsRequestPaginateTypeDef = {  # (1)
    "AnalysisReportId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetAnalysisReportResultsRequestPaginateTypeDef](./type_defs.md#getanalysisreportresultsrequestpaginatetypedef)
## ListAnalysisReportsPaginator

Type annotations and code completion for `#!python session.create_client("network-firewall").get_paginator("list_analysis_reports")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall/paginator/ListAnalysisReports.html#NetworkFirewall.Paginator.ListAnalysisReports)

```python
# ListAnalysisReportsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_network_firewall.paginator import ListAnalysisReportsPaginator

session = get_session()
async with session.create_client("network-firewall") as client:  # (1)
    paginator: ListAnalysisReportsPaginator = client.get_paginator("list_analysis_reports")  # (2)
    async for item in paginator.paginate(...):
        item: ListAnalysisReportsResponseTypeDef
        print(item)  # (3)
```

1. client: [NetworkFirewallClient](./client.md)
2. paginator: [ListAnalysisReportsPaginator](./paginators.md#listanalysisreportspaginator)
3. item: `AioPageIterator[ListAnalysisReportsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListAnalysisReportsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FirewallName: str = ...,
    FirewallArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListAnalysisReportsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListAnalysisReportsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListAnalysisReportsRequestPaginateTypeDef = {  # (1)
    "FirewallName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAnalysisReportsRequestPaginateTypeDef](./type_defs.md#listanalysisreportsrequestpaginatetypedef)
## ListFirewallPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("network-firewall").get_paginator("list_firewall_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall/paginator/ListFirewallPolicies.html#NetworkFirewall.Paginator.ListFirewallPolicies)

```python
# ListFirewallPoliciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_network_firewall.paginator import ListFirewallPoliciesPaginator

session = get_session()
async with session.create_client("network-firewall") as client:  # (1)
    paginator: ListFirewallPoliciesPaginator = client.get_paginator("list_firewall_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListFirewallPoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [NetworkFirewallClient](./client.md)
2. paginator: [ListFirewallPoliciesPaginator](./paginators.md#listfirewallpoliciespaginator)
3. item: `AioPageIterator[ListFirewallPoliciesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFirewallPoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListFirewallPoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListFirewallPoliciesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFirewallPoliciesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFirewallPoliciesRequestPaginateTypeDef](./type_defs.md#listfirewallpoliciesrequestpaginatetypedef)
## ListFirewallsPaginator

Type annotations and code completion for `#!python session.create_client("network-firewall").get_paginator("list_firewalls")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall/paginator/ListFirewalls.html#NetworkFirewall.Paginator.ListFirewalls)

```python
# ListFirewallsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_network_firewall.paginator import ListFirewallsPaginator

session = get_session()
async with session.create_client("network-firewall") as client:  # (1)
    paginator: ListFirewallsPaginator = client.get_paginator("list_firewalls")  # (2)
    async for item in paginator.paginate(...):
        item: ListFirewallsResponseTypeDef
        print(item)  # (3)
```

1. client: [NetworkFirewallClient](./client.md)
2. paginator: [ListFirewallsPaginator](./paginators.md#listfirewallspaginator)
3. item: `AioPageIterator[ListFirewallsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFirewallsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    VpcIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListFirewallsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListFirewallsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFirewallsRequestPaginateTypeDef = {  # (1)
    "VpcIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFirewallsRequestPaginateTypeDef](./type_defs.md#listfirewallsrequestpaginatetypedef)
## ListFlowOperationResultsPaginator

Type annotations and code completion for `#!python session.create_client("network-firewall").get_paginator("list_flow_operation_results")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall/paginator/ListFlowOperationResults.html#NetworkFirewall.Paginator.ListFlowOperationResults)

```python
# ListFlowOperationResultsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_network_firewall.paginator import ListFlowOperationResultsPaginator

session = get_session()
async with session.create_client("network-firewall") as client:  # (1)
    paginator: ListFlowOperationResultsPaginator = client.get_paginator("list_flow_operation_results")  # (2)
    async for item in paginator.paginate(...):
        item: ListFlowOperationResultsResponseTypeDef
        print(item)  # (3)
```

1. client: [NetworkFirewallClient](./client.md)
2. paginator: [ListFlowOperationResultsPaginator](./paginators.md#listflowoperationresultspaginator)
3. item: `AioPageIterator[ListFlowOperationResultsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFlowOperationResultsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FirewallArn: str,
    FlowOperationId: str,
    AvailabilityZone: str = ...,
    VpcEndpointId: str = ...,
    VpcEndpointAssociationArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListFlowOperationResultsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListFlowOperationResultsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFlowOperationResultsRequestPaginateTypeDef = {  # (1)
    "FirewallArn": ...,
    "FlowOperationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFlowOperationResultsRequestPaginateTypeDef](./type_defs.md#listflowoperationresultsrequestpaginatetypedef)
## ListFlowOperationsPaginator

Type annotations and code completion for `#!python session.create_client("network-firewall").get_paginator("list_flow_operations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall/paginator/ListFlowOperations.html#NetworkFirewall.Paginator.ListFlowOperations)

```python
# ListFlowOperationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_network_firewall.paginator import ListFlowOperationsPaginator

session = get_session()
async with session.create_client("network-firewall") as client:  # (1)
    paginator: ListFlowOperationsPaginator = client.get_paginator("list_flow_operations")  # (2)
    async for item in paginator.paginate(...):
        item: ListFlowOperationsResponseTypeDef
        print(item)  # (3)
```

1. client: [NetworkFirewallClient](./client.md)
2. paginator: [ListFlowOperationsPaginator](./paginators.md#listflowoperationspaginator)
3. item: `AioPageIterator[ListFlowOperationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFlowOperationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FirewallArn: str,
    AvailabilityZone: str = ...,
    VpcEndpointAssociationArn: str = ...,
    VpcEndpointId: str = ...,
    FlowOperationType: FlowOperationTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListFlowOperationsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: FlowOperationTypeType](./literals.md#flowoperationtypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListFlowOperationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFlowOperationsRequestPaginateTypeDef = {  # (1)
    "FirewallArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFlowOperationsRequestPaginateTypeDef](./type_defs.md#listflowoperationsrequestpaginatetypedef)
## ListProxiesPaginator

Type annotations and code completion for `#!python session.create_client("network-firewall").get_paginator("list_proxies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall/paginator/ListProxies.html#NetworkFirewall.Paginator.ListProxies)

```python
# ListProxiesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_network_firewall.paginator import ListProxiesPaginator

session = get_session()
async with session.create_client("network-firewall") as client:  # (1)
    paginator: ListProxiesPaginator = client.get_paginator("list_proxies")  # (2)
    async for item in paginator.paginate(...):
        item: ListProxiesResponseTypeDef
        print(item)  # (3)
```

1. client: [NetworkFirewallClient](./client.md)
2. paginator: [ListProxiesPaginator](./paginators.md#listproxiespaginator)
3. item: `AioPageIterator[ListProxiesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListProxiesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListProxiesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListProxiesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListProxiesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProxiesRequestPaginateTypeDef](./type_defs.md#listproxiesrequestpaginatetypedef)
## ListProxyConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("network-firewall").get_paginator("list_proxy_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall/paginator/ListProxyConfigurations.html#NetworkFirewall.Paginator.ListProxyConfigurations)

```python
# ListProxyConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_network_firewall.paginator import ListProxyConfigurationsPaginator

session = get_session()
async with session.create_client("network-firewall") as client:  # (1)
    paginator: ListProxyConfigurationsPaginator = client.get_paginator("list_proxy_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListProxyConfigurationsResponseTypeDef
        print(item)  # (3)
```

1. client: [NetworkFirewallClient](./client.md)
2. paginator: [ListProxyConfigurationsPaginator](./paginators.md#listproxyconfigurationspaginator)
3. item: `AioPageIterator[ListProxyConfigurationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListProxyConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListProxyConfigurationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListProxyConfigurationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListProxyConfigurationsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProxyConfigurationsRequestPaginateTypeDef](./type_defs.md#listproxyconfigurationsrequestpaginatetypedef)
## ListProxyRuleGroupsPaginator

Type annotations and code completion for `#!python session.create_client("network-firewall").get_paginator("list_proxy_rule_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall/paginator/ListProxyRuleGroups.html#NetworkFirewall.Paginator.ListProxyRuleGroups)

```python
# ListProxyRuleGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_network_firewall.paginator import ListProxyRuleGroupsPaginator

session = get_session()
async with session.create_client("network-firewall") as client:  # (1)
    paginator: ListProxyRuleGroupsPaginator = client.get_paginator("list_proxy_rule_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListProxyRuleGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [NetworkFirewallClient](./client.md)
2. paginator: [ListProxyRuleGroupsPaginator](./paginators.md#listproxyrulegroupspaginator)
3. item: `AioPageIterator[ListProxyRuleGroupsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListProxyRuleGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListProxyRuleGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListProxyRuleGroupsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListProxyRuleGroupsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProxyRuleGroupsRequestPaginateTypeDef](./type_defs.md#listproxyrulegroupsrequestpaginatetypedef)
## ListRuleGroupsPaginator

Type annotations and code completion for `#!python session.create_client("network-firewall").get_paginator("list_rule_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall/paginator/ListRuleGroups.html#NetworkFirewall.Paginator.ListRuleGroups)

```python
# ListRuleGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_network_firewall.paginator import ListRuleGroupsPaginator

session = get_session()
async with session.create_client("network-firewall") as client:  # (1)
    paginator: ListRuleGroupsPaginator = client.get_paginator("list_rule_groups")  # (2)
    async for item in paginator.paginate(...):
        item: ListRuleGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [NetworkFirewallClient](./client.md)
2. paginator: [ListRuleGroupsPaginator](./paginators.md#listrulegroupspaginator)
3. item: `AioPageIterator[ListRuleGroupsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRuleGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Scope: ResourceManagedStatusType = ...,  # (1)
    ManagedType: ResourceManagedTypeType = ...,  # (2)
    SubscriptionStatus: SubscriptionStatusType = ...,  # (3)
    Type: RuleGroupTypeType = ...,  # (4)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (5)
) -> aiobotocore.paginate.AioPageIterator[ListRuleGroupsResponseTypeDef]:  # (6)
    ...
```

1. See [:material-code-brackets: ResourceManagedStatusType](./literals.md#resourcemanagedstatustype)
2. See [:material-code-brackets: ResourceManagedTypeType](./literals.md#resourcemanagedtypetype)
3. See [:material-code-brackets: SubscriptionStatusType](./literals.md#subscriptionstatustype)
4. See [:material-code-brackets: RuleGroupTypeType](./literals.md#rulegrouptypetype)
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
6. See `AioPageIterator[ListRuleGroupsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRuleGroupsRequestPaginateTypeDef = {  # (1)
    "Scope": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRuleGroupsRequestPaginateTypeDef](./type_defs.md#listrulegroupsrequestpaginatetypedef)
## ListTLSInspectionConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("network-firewall").get_paginator("list_tls_inspection_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall/paginator/ListTLSInspectionConfigurations.html#NetworkFirewall.Paginator.ListTLSInspectionConfigurations)

```python
# ListTLSInspectionConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_network_firewall.paginator import ListTLSInspectionConfigurationsPaginator

session = get_session()
async with session.create_client("network-firewall") as client:  # (1)
    paginator: ListTLSInspectionConfigurationsPaginator = client.get_paginator("list_tls_inspection_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: ListTLSInspectionConfigurationsResponseTypeDef
        print(item)  # (3)
```

1. client: [NetworkFirewallClient](./client.md)
2. paginator: [ListTLSInspectionConfigurationsPaginator](./paginators.md#listtlsinspectionconfigurationspaginator)
3. item: `AioPageIterator[ListTLSInspectionConfigurationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTLSInspectionConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTLSInspectionConfigurationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTLSInspectionConfigurationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTLSInspectionConfigurationsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTLSInspectionConfigurationsRequestPaginateTypeDef](./type_defs.md#listtlsinspectionconfigurationsrequestpaginatetypedef)
## ListTagsForResourcePaginator

Type annotations and code completion for `#!python session.create_client("network-firewall").get_paginator("list_tags_for_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall/paginator/ListTagsForResource.html#NetworkFirewall.Paginator.ListTagsForResource)

```python
# ListTagsForResourcePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_network_firewall.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("network-firewall") as client:  # (1)
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")  # (2)
    async for item in paginator.paginate(...):
        item: ListTagsForResourceResponseTypeDef
        print(item)  # (3)
```

1. client: [NetworkFirewallClient](./client.md)
2. paginator: [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
3. item: `AioPageIterator[ListTagsForResourceResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListTagsForResourcePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListTagsForResourceResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListTagsForResourceResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListTagsForResourceRequestPaginateTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestPaginateTypeDef](./type_defs.md#listtagsforresourcerequestpaginatetypedef)
## ListVpcEndpointAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("network-firewall").get_paginator("list_vpc_endpoint_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall/paginator/ListVpcEndpointAssociations.html#NetworkFirewall.Paginator.ListVpcEndpointAssociations)

```python
# ListVpcEndpointAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_network_firewall.paginator import ListVpcEndpointAssociationsPaginator

session = get_session()
async with session.create_client("network-firewall") as client:  # (1)
    paginator: ListVpcEndpointAssociationsPaginator = client.get_paginator("list_vpc_endpoint_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListVpcEndpointAssociationsResponseTypeDef
        print(item)  # (3)
```

1. client: [NetworkFirewallClient](./client.md)
2. paginator: [ListVpcEndpointAssociationsPaginator](./paginators.md#listvpcendpointassociationspaginator)
3. item: `AioPageIterator[ListVpcEndpointAssociationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListVpcEndpointAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FirewallArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListVpcEndpointAssociationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListVpcEndpointAssociationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListVpcEndpointAssociationsRequestPaginateTypeDef = {  # (1)
    "FirewallArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListVpcEndpointAssociationsRequestPaginateTypeDef](./type_defs.md#listvpcendpointassociationsrequestpaginatetypedef)
