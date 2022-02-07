<a id="waiters-for-aiobotocore-opsworkscm-module"></a>

# Waiters for aiobotocore OpsWorksCM module

> [Index](..) > [OpsWorksCM](.) > Waiters

Auto-generated documentation for
[OpsWorksCM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
type annotations stubs module
[types-aiobotocore-opsworkscm](https://pypi.org/project/types-aiobotocore-opsworkscm/).

- [Waiters for aiobotocore OpsWorksCM module](#waiters-for-aiobotocore-opsworkscm-module)
  - [NodeAssociatedWaiter](#nodeassociatedwaiter)

<a id="nodeassociatedwaiter"></a>

## NodeAssociatedWaiter

Type annotations for
`session.create_client("opsworkscm").get_waiter("node_associated")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_opsworkscm.waiter import NodeAssociatedWaiter

def get_node_associated_waiter() -> NodeAssociatedWaiter:
    return Session().client("opsworkscm").get_waiter("node_associated")
```

Boto3 documentation:
[OpsWorksCM.Waiter.node_associated](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Waiter.NodeAssociated)

Arguments for `NodeAssociatedWaiter.wait` method:

- `NodeAssociationStatusToken`: `str` *(required)*
- `ServerName`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
