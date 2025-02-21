# Examples

> [Index](../README.md) > [EKS](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [EKS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#eks)
    type annotations stubs module [types-aiobotocore-eks](https://pypi.org/project/types-aiobotocore-eks/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[eks]` package installed.

Write your `EKS` code as usual,
type checking and code completion should work out of the box.



```python
# EKSClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("eks") as client:  # (1)
    result = await client.associate_access_policy()  # (2)
```

1. client: [EKSClient](./client.md)
2. result: [:material-code-braces: AssociateAccessPolicyResponseTypeDef](./type_defs.md#associateaccesspolicyresponsetypedef) 



```python
# DescribeAddonVersionsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("eks") as client:  # (1)
    paginator = client.get_paginator("describe_addon_versions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [EKSClient](./client.md)
2. paginator: [DescribeAddonVersionsPaginator](./paginators.md#describeaddonversionspaginator)
3. item: [:material-code-braces: DescribeAddonVersionsResponseTypeDef](./type_defs.md#describeaddonversionsresponsetypedef) 



```python
# AddonActiveWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("eks") as client:  # (1)
    waiter = client.get_waiter("addon_active")  # (2)
    await waiter.wait()
```

1. client: [EKSClient](./client.md)
2. waiter: [AddonActiveWaiter](./waiters.md#addonactivewaiter)


### Explicit type annotations

With `types-aiobotocore-lite[eks]`
or a standalone `types_aiobotocore_eks` package, you have to explicitly specify
`client: EKSClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# EKSClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_eks.client import EKSClient
from types_aiobotocore_eks.type_defs import AssociateAccessPolicyResponseTypeDef
from types_aiobotocore_eks.type_defs import AssociateAccessPolicyRequestTypeDef


session = get_session()

async with session.create_client("eks") as client:
    client: EKSClient
    kwargs: AssociateAccessPolicyRequestTypeDef = {...}
    result: AssociateAccessPolicyResponseTypeDef = await client.associate_access_policy(**kwargs)
```



```python
# DescribeAddonVersionsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_eks.client import EKSClient
from types_aiobotocore_eks.paginator import DescribeAddonVersionsPaginator
from types_aiobotocore_eks.type_defs import DescribeAddonVersionsResponseTypeDef


session = get_session()

async with session.create_client("eks") as client:
    client: EKSClient
    paginator: DescribeAddonVersionsPaginator = client.get_paginator("describe_addon_versions")
    async for item in paginator.paginate(...):
        item: DescribeAddonVersionsResponseTypeDef
        print(item)
```



```python
# AddonActiveWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_eks.client import EKSClient
from types_aiobotocore_eks.waiter import AddonActiveWaiter


session = get_session()

async with session.create_client("eks") as client:
    client: EKSClient
    waiter: AddonActiveWaiter = client.get_waiter("addon_active")
    await waiter.wait()
```
