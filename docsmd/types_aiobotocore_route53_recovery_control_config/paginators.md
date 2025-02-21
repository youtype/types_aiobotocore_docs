# Paginators

> [Index](../README.md) > [Route53RecoveryControlConfig](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Route53RecoveryControlConfig](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#route53recoverycontrolconfig)
    type annotations stubs module [types-aiobotocore-route53-recovery-control-config](https://pypi.org/project/types-aiobotocore-route53-recovery-control-config/).

## ListAssociatedRoute53HealthChecksPaginator

Type annotations and code completion for `#!python session.create_client("route53-recovery-control-config").get_paginator("list_associated_route53_health_checks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config/paginator/ListAssociatedRoute53HealthChecks.html#Route53RecoveryControlConfig.Paginator.ListAssociatedRoute53HealthChecks)

```python
# ListAssociatedRoute53HealthChecksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53_recovery_control_config.paginator import ListAssociatedRoute53HealthChecksPaginator

session = get_session()
async with session.create_client("route53-recovery-control-config") as client:  # (1)
    paginator: ListAssociatedRoute53HealthChecksPaginator = client.get_paginator("list_associated_route53_health_checks")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssociatedRoute53HealthChecksResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53RecoveryControlConfigClient](./client.md)
2. paginator: [ListAssociatedRoute53HealthChecksPaginator](./paginators.md#listassociatedroute53healthcheckspaginator)
3. item: [:material-code-braces: ListAssociatedRoute53HealthChecksResponseTypeDef](./type_defs.md#listassociatedroute53healthchecksresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAssociatedRoute53HealthChecksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    RoutingControlArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAssociatedRoute53HealthChecksResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAssociatedRoute53HealthChecksResponseTypeDef](./type_defs.md#listassociatedroute53healthchecksresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAssociatedRoute53HealthChecksRequestPaginateTypeDef = {  # (1)
    "RoutingControlArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssociatedRoute53HealthChecksRequestPaginateTypeDef](./type_defs.md#listassociatedroute53healthchecksrequestpaginatetypedef) 
## ListClustersPaginator

Type annotations and code completion for `#!python session.create_client("route53-recovery-control-config").get_paginator("list_clusters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config/paginator/ListClusters.html#Route53RecoveryControlConfig.Paginator.ListClusters)

```python
# ListClustersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53_recovery_control_config.paginator import ListClustersPaginator

session = get_session()
async with session.create_client("route53-recovery-control-config") as client:  # (1)
    paginator: ListClustersPaginator = client.get_paginator("list_clusters")  # (2)
    async for item in paginator.paginate(...):
        item: ListClustersResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53RecoveryControlConfigClient](./client.md)
2. paginator: [ListClustersPaginator](./paginators.md#listclusterspaginator)
3. item: [:material-code-braces: ListClustersResponseTypeDef](./type_defs.md#listclustersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListClustersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListClustersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListClustersResponseTypeDef](./type_defs.md#listclustersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListClustersRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListClustersRequestPaginateTypeDef](./type_defs.md#listclustersrequestpaginatetypedef) 
## ListControlPanelsPaginator

Type annotations and code completion for `#!python session.create_client("route53-recovery-control-config").get_paginator("list_control_panels")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config/paginator/ListControlPanels.html#Route53RecoveryControlConfig.Paginator.ListControlPanels)

```python
# ListControlPanelsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53_recovery_control_config.paginator import ListControlPanelsPaginator

session = get_session()
async with session.create_client("route53-recovery-control-config") as client:  # (1)
    paginator: ListControlPanelsPaginator = client.get_paginator("list_control_panels")  # (2)
    async for item in paginator.paginate(...):
        item: ListControlPanelsResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53RecoveryControlConfigClient](./client.md)
2. paginator: [ListControlPanelsPaginator](./paginators.md#listcontrolpanelspaginator)
3. item: [:material-code-braces: ListControlPanelsResponseTypeDef](./type_defs.md#listcontrolpanelsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListControlPanelsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClusterArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListControlPanelsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListControlPanelsResponseTypeDef](./type_defs.md#listcontrolpanelsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListControlPanelsRequestPaginateTypeDef = {  # (1)
    "ClusterArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListControlPanelsRequestPaginateTypeDef](./type_defs.md#listcontrolpanelsrequestpaginatetypedef) 
## ListRoutingControlsPaginator

Type annotations and code completion for `#!python session.create_client("route53-recovery-control-config").get_paginator("list_routing_controls")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config/paginator/ListRoutingControls.html#Route53RecoveryControlConfig.Paginator.ListRoutingControls)

```python
# ListRoutingControlsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53_recovery_control_config.paginator import ListRoutingControlsPaginator

session = get_session()
async with session.create_client("route53-recovery-control-config") as client:  # (1)
    paginator: ListRoutingControlsPaginator = client.get_paginator("list_routing_controls")  # (2)
    async for item in paginator.paginate(...):
        item: ListRoutingControlsResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53RecoveryControlConfigClient](./client.md)
2. paginator: [ListRoutingControlsPaginator](./paginators.md#listroutingcontrolspaginator)
3. item: [:material-code-braces: ListRoutingControlsResponseTypeDef](./type_defs.md#listroutingcontrolsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRoutingControlsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ControlPanelArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListRoutingControlsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRoutingControlsResponseTypeDef](./type_defs.md#listroutingcontrolsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRoutingControlsRequestPaginateTypeDef = {  # (1)
    "ControlPanelArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRoutingControlsRequestPaginateTypeDef](./type_defs.md#listroutingcontrolsrequestpaginatetypedef) 
## ListSafetyRulesPaginator

Type annotations and code completion for `#!python session.create_client("route53-recovery-control-config").get_paginator("list_safety_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config/paginator/ListSafetyRules.html#Route53RecoveryControlConfig.Paginator.ListSafetyRules)

```python
# ListSafetyRulesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53_recovery_control_config.paginator import ListSafetyRulesPaginator

session = get_session()
async with session.create_client("route53-recovery-control-config") as client:  # (1)
    paginator: ListSafetyRulesPaginator = client.get_paginator("list_safety_rules")  # (2)
    async for item in paginator.paginate(...):
        item: ListSafetyRulesResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53RecoveryControlConfigClient](./client.md)
2. paginator: [ListSafetyRulesPaginator](./paginators.md#listsafetyrulespaginator)
3. item: [:material-code-braces: ListSafetyRulesResponseTypeDef](./type_defs.md#listsafetyrulesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSafetyRulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ControlPanelArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSafetyRulesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSafetyRulesResponseTypeDef](./type_defs.md#listsafetyrulesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSafetyRulesRequestPaginateTypeDef = {  # (1)
    "ControlPanelArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSafetyRulesRequestPaginateTypeDef](./type_defs.md#listsafetyrulesrequestpaginatetypedef) 
