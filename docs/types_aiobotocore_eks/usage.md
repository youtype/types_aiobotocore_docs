<a id="examples-for-aiobotocore-eks-module"></a>

# Examples for aiobotocore EKS module

> [Index](../README.md) > [EKS](./README.md) > Examples

- [Examples for aiobotocore EKS module](#examples-for-aiobotocore-eks-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[eks]` package installed.

Write your `EKS` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type EKSClient
# and provides type checking and code completion
async with session.create_client("eks") as client:
    
    # result has type AssociateEncryptionConfigResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_encryption_config()
    

    
    # paginator has type DescribeAddonVersionsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_addon_versions")
    async for item in paginator.paginate(...):
        # item has type DescribeAddonVersionsResponseTypeDef
        print(item)
    

    
    # waiter has type AddonActiveWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("addon_active")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[eks]` or a standalone `types_aiobotocore_eks`
package, you have to explicitly specify `client: EKSClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_eks.client import EKSClient
from types_aiobotocore_eks.type_defs import AssociateEncryptionConfigResponseTypeDef
from types_aiobotocore_eks.paginator import DescribeAddonVersionsPaginator
from types_aiobotocore_eks.waiter import AddonActiveWaiter
from types_aiobotocore_eks.literals import PaginatorName
from types_aiobotocore_eks.literals import WaiterName


session = get_session()

async with session.create_client("eks") as client:
    client: EKSClient

    
    result: AssociateEncryptionConfigResponseTypeDef = client.associate_encryption_config()
    

    
    paginator_name: PaginatorName = "describe_addon_versions"
    paginator: DescribeAddonVersionsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeAddonVersionsResponseTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "addon_active"
    waiter: AddonActiveWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
