<a id="examples-for-aiobotocore-iam-module"></a>

# Examples for aiobotocore IAM module

> [Index](../README.md) > [IAM](./README.md) > Examples

- [Examples for aiobotocore IAM module](#examples-for-aiobotocore-iam-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[iam]` package installed.

Write your `IAM` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type IAMClient
# and provides type checking and code completion
async with session.create_client("iam") as client:
    
    # result has type None
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_client_id_to_open_id_connect_provider()
    

    
    # paginator has type GetAccountAuthorizationDetailsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("get_account_authorization_details")
    async for item in paginator.paginate(...):
        # item has type GetAccountAuthorizationDetailsResponseTypeDef
        print(item)
    

    
    # waiter has type InstanceProfileExistsWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("instance_profile_exists")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[iam]` or a standalone `types_aiobotocore_iam`
package, you have to explicitly specify `client: IAMClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_iam.client import IAMClient
from types_aiobotocore_iam.type_defs import None
from types_aiobotocore_iam.paginator import GetAccountAuthorizationDetailsPaginator
from types_aiobotocore_iam.waiter import InstanceProfileExistsWaiter
from types_aiobotocore_iam.literals import PaginatorName
from types_aiobotocore_iam.literals import WaiterName


session = get_session()

async with session.create_client("iam") as client:
    client: IAMClient

    
    result: None = client.add_client_id_to_open_id_connect_provider()
    

    
    paginator_name: PaginatorName = "get_account_authorization_details"
    paginator: GetAccountAuthorizationDetailsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: GetAccountAuthorizationDetailsResponseTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "instance_profile_exists"
    waiter: InstanceProfileExistsWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
