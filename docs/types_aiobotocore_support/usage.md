<a id="examples-for-aiobotocore-support-module"></a>

# Examples for aiobotocore Support module

> [Index](../README.md) > [Support](./README.md) > Examples

- [Examples for aiobotocore Support module](#examples-for-aiobotocore-support-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[support]` package installed.

Write your `Support` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type SupportClient
# and provides type checking and code completion
async with session.create_client("support") as client:
    
    # result has type AddAttachmentsToSetResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_attachments_to_set()
    

    
    # paginator has type DescribeCasesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_cases")
    async for item in paginator.paginate(...):
        # item has type DescribeCasesResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[support]` or a standalone
`types_aiobotocore_support` package, you have to explicitly specify
`client: SupportClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_support.client import SupportClient
from types_aiobotocore_support.type_defs import AddAttachmentsToSetResponseTypeDef
from types_aiobotocore_support.paginator import DescribeCasesPaginator

from types_aiobotocore_support.literals import PaginatorName



session = get_session()

async with session.create_client("support") as client:
    client: SupportClient

    
    result: AddAttachmentsToSetResponseTypeDef = client.add_attachments_to_set()
    

    
    paginator_name: PaginatorName = "describe_cases"
    paginator: DescribeCasesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeCasesResponseTypeDef
        print(item)
    

    
```
