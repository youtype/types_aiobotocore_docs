<a id="examples-for-aiobotocore-ram-module"></a>

# Examples for aiobotocore RAM module

> [Index](../README.md) > [RAM](./README.md) > Examples

- [Examples for aiobotocore RAM module](#examples-for-aiobotocore-ram-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[ram]` package installed.

Write your `RAM` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type RAMClient
# and provides type checking and code completion
async with session.create_client("ram") as client:
    
    # result has type AcceptResourceShareInvitationResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.accept_resource_share_invitation()
    

    
    # paginator has type GetResourcePoliciesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("get_resource_policies")
    async for item in paginator.paginate(...):
        # item has type GetResourcePoliciesResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[ram]` or a standalone `types_aiobotocore_ram`
package, you have to explicitly specify `client: RAMClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_ram.client import RAMClient
from types_aiobotocore_ram.type_defs import AcceptResourceShareInvitationResponseTypeDef
from types_aiobotocore_ram.paginator import GetResourcePoliciesPaginator

from types_aiobotocore_ram.literals import PaginatorName



session = get_session()

async with session.create_client("ram") as client:
    client: RAMClient

    
    result: AcceptResourceShareInvitationResponseTypeDef = client.accept_resource_share_invitation()
    

    
    paginator_name: PaginatorName = "get_resource_policies"
    paginator: GetResourcePoliciesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: GetResourcePoliciesResponseTypeDef
        print(item)
    

    
```
