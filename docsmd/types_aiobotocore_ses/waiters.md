# Waiters

> [Index](../README.md) > [SES](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [SES](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
    type annotations stubs module [types-aiobotocore-ses](https://pypi.org/project/types-aiobotocore-ses/).

## IdentityExistsWaiter

Type annotations and code completion for `#!python session.create_client("ses").get_waiter("identity_exists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Waiter.IdentityExists)

```python title="Usage example"
from aiobotocore.session import Session

from types_aiobotocore_ses.waiter import IdentityExistsWaiter

def get_identity_exists_waiter() -> IdentityExistsWaiter:
    return Session().client("ses").get_waiter("identity_exists")
```


### wait

Type annotations and code completion for `#!python IdentityExistsWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    Identities: Sequence[str],
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: GetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef = {  # (1)
    "Identities": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef](./type_defs.md#getidentityverificationattributesrequestidentityexistswaittypedef) 
