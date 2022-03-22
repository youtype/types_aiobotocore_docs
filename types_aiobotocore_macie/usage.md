<a id="examples-for-aiobotocore-macie-module"></a>

# Examples for aiobotocore Macie module

> [Index](../README.md) > [Macie](./README.md) > Examples

- [Examples for aiobotocore Macie module](#examples-for-aiobotocore-macie-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[macie]` package installed.

Write your `Macie` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type MacieClient
# and provides type checking and code completion
async with session.create_client("macie") as client:
    
    # result has type None
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_member_account()
    

    
    # paginator has type ListMemberAccountsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_member_accounts")
    async for item in paginator.paginate(...):
        # item has type ListMemberAccountsResultTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[macie]` or a standalone `types_aiobotocore_macie`
package, you have to explicitly specify `client: MacieClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_macie.client import MacieClient
from types_aiobotocore_macie.type_defs import None
from types_aiobotocore_macie.paginator import ListMemberAccountsPaginator

from types_aiobotocore_macie.literals import PaginatorName



session = get_session()

async with session.create_client("macie") as client:
    client: MacieClient

    
    result: None = client.associate_member_account()
    

    
    paginator_name: PaginatorName = "list_member_accounts"
    paginator: ListMemberAccountsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListMemberAccountsResultTypeDef
        print(item)
    

    
```
