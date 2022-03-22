<a id="waiters-for-aiobotocore-ses-module"></a>

# Waiters for aiobotocore SES module

> [Index](../README.md) > [SES](./README.md) > Waiters

Auto-generated documentation for
[SES](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
type annotations stubs module
[types-aiobotocore-ses](https://pypi.org/project/types-aiobotocore-ses/).

- [Waiters for aiobotocore SES module](#waiters-for-aiobotocore-ses-module)
  - [IdentityExistsWaiter](#identityexistswaiter)

<a id="identityexistswaiter"></a>

## IdentityExistsWaiter

Type annotations for
`session.create_client("ses").get_waiter("identity_exists")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_ses.waiter import IdentityExistsWaiter

def get_identity_exists_waiter() -> IdentityExistsWaiter:
    return Session().client("ses").get_waiter("identity_exists")
```

Boto3 documentation:
[SES.Waiter.identity_exists](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Waiter.IdentityExists)

Arguments for `IdentityExistsWaiter.wait` method:

- `Identities`: `Sequence`\[`str`\] *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
