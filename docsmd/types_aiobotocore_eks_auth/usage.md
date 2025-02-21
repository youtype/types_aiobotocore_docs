# Examples

> [Index](../README.md) > [EKSAuth](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [EKSAuth](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks-auth.html#eksauth)
    type annotations stubs module [types-aiobotocore-eks-auth](https://pypi.org/project/types-aiobotocore-eks-auth/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[eks-auth]` package installed.

Write your `EKSAuth` code as usual,
type checking and code completion should work out of the box.



```python
# EKSAuthClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("eks-auth") as client:  # (1)
    result = await client.assume_role_for_pod_identity()  # (2)
```

1. client: [EKSAuthClient](./client.md)
2. result: [:material-code-braces: AssumeRoleForPodIdentityResponseTypeDef](./type_defs.md#assumeroleforpodidentityresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[eks-auth]`
or a standalone `types_aiobotocore_eks_auth` package, you have to explicitly specify
`client: EKSAuthClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# EKSAuthClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_eks_auth.client import EKSAuthClient
from types_aiobotocore_eks_auth.type_defs import AssumeRoleForPodIdentityResponseTypeDef
from types_aiobotocore_eks_auth.type_defs import AssumeRoleForPodIdentityRequestTypeDef


session = get_session()

async with session.create_client("eks-auth") as client:
    client: EKSAuthClient
    kwargs: AssumeRoleForPodIdentityRequestTypeDef = {...}
    result: AssumeRoleForPodIdentityResponseTypeDef = await client.assume_role_for_pod_identity(**kwargs)
```




