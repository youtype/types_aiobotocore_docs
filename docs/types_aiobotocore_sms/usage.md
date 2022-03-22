<a id="examples-for-aiobotocore-sms-module"></a>

# Examples for aiobotocore SMS module

> [Index](../README.md) > [SMS](./README.md) > Examples

- [Examples for aiobotocore SMS module](#examples-for-aiobotocore-sms-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[sms]` package installed.

Write your `SMS` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type SMSClient
# and provides type checking and code completion
async with session.create_client("sms") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type GetConnectorsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("get_connectors")
    async for item in paginator.paginate(...):
        # item has type GetConnectorsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[sms]` or a standalone `types_aiobotocore_sms`
package, you have to explicitly specify `client: SMSClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_sms.client import SMSClient
from types_aiobotocore_sms.type_defs import bool
from types_aiobotocore_sms.paginator import GetConnectorsPaginator

from types_aiobotocore_sms.literals import PaginatorName



session = get_session()

async with session.create_client("sms") as client:
    client: SMSClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "get_connectors"
    paginator: GetConnectorsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: GetConnectorsResponseTypeDef
        print(item)
    

    
```
