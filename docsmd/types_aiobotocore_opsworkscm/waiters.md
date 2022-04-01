# Waiters

> [Index](../README.md) > [OpsWorksCM](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [OpsWorksCM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
    type annotations stubs module [types-aiobotocore-opsworkscm](https://pypi.org/project/types-aiobotocore-opsworkscm/).

## NodeAssociatedWaiter

Type annotations and code completion for `#!python session.create_client("opsworkscm").get_waiter("node_associated")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Waiter.NodeAssociated)

```python title="Usage example"
from aiobotocore.session import Session

from types_aiobotocore_opsworkscm.waiter import NodeAssociatedWaiter

def get_node_associated_waiter() -> NodeAssociatedWaiter:
    return Session().client("opsworkscm").get_waiter("node_associated")
```


### wait

Type annotations and code completion for `#!python NodeAssociatedWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    NodeAssociationStatusToken: str,
    ServerName: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef = {  # (1)
    "NodeAssociationStatusToken": ...,
    "ServerName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef](./type_defs.md#describenodeassociationstatusrequestnodeassociatedwaittypedef) 
