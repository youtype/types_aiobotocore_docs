# Paginators

> [Index](../README.md) > [Route53RecoveryCluster](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Route53RecoveryCluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#route53recoverycluster)
    type annotations stubs module [types-aiobotocore-route53-recovery-cluster](https://pypi.org/project/types-aiobotocore-route53-recovery-cluster/).

## ListRoutingControlsPaginator

Type annotations and code completion for `#!python session.create_client("route53-recovery-cluster").get_paginator("list_routing_controls")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster/paginator/ListRoutingControls.html#Route53RecoveryCluster.Paginator.ListRoutingControls)

```python
# ListRoutingControlsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53_recovery_cluster.paginator import ListRoutingControlsPaginator

session = get_session()
async with session.create_client("route53-recovery-cluster") as client:  # (1)
    paginator: ListRoutingControlsPaginator = client.get_paginator("list_routing_controls")  # (2)
    async for item in paginator.paginate(...):
        item: ListRoutingControlsResponseTypeDef
        print(item)  # (3)
```

1. client: [Route53RecoveryClusterClient](./client.md)
2. paginator: [ListRoutingControlsPaginator](./paginators.md#listroutingcontrolspaginator)
3. item: [:material-code-braces: ListRoutingControlsResponseTypeDef](./type_defs.md#listroutingcontrolsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRoutingControlsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ControlPanelArn: str = ...,
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
