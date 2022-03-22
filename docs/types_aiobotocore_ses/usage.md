<a id="examples-for-aiobotocore-ses-module"></a>

# Examples for aiobotocore SES module

> [Index](../README.md) > [SES](./README.md) > Examples

- [Examples for aiobotocore SES module](#examples-for-aiobotocore-ses-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[ses]` package installed.

Write your `SES` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type SESClient
# and provides type checking and code completion
async with session.create_client("ses") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListConfigurationSetsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_configuration_sets")
    async for item in paginator.paginate(...):
        # item has type ListConfigurationSetsResponseTypeDef
        print(item)
    

    
    # waiter has type IdentityExistsWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("identity_exists")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[ses]` or a standalone `types_aiobotocore_ses`
package, you have to explicitly specify `client: SESClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_ses.client import SESClient
from types_aiobotocore_ses.type_defs import bool
from types_aiobotocore_ses.paginator import ListConfigurationSetsPaginator
from types_aiobotocore_ses.waiter import IdentityExistsWaiter
from types_aiobotocore_ses.literals import PaginatorName
from types_aiobotocore_ses.literals import WaiterName


session = get_session()

async with session.create_client("ses") as client:
    client: SESClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_configuration_sets"
    paginator: ListConfigurationSetsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListConfigurationSetsResponseTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "identity_exists"
    waiter: IdentityExistsWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
