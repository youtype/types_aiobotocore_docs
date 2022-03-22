<a id="examples-for-aiobotocore-cloudhsm-module"></a>

# Examples for aiobotocore CloudHSM module

> [Index](../README.md) > [CloudHSM](./README.md) > Examples

- [Examples for aiobotocore CloudHSM module](#examples-for-aiobotocore-cloudhsm-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[cloudhsm]` package installed.

Write your `CloudHSM` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type CloudHSMClient
# and provides type checking and code completion
async with session.create_client("cloudhsm") as client:
    
    # result has type AddTagsToResourceResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_tags_to_resource()
    

    
    # paginator has type ListHapgsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_hapgs")
    async for item in paginator.paginate(...):
        # item has type ListHapgsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[cloudhsm]` or a standalone
`types_aiobotocore_cloudhsm` package, you have to explicitly specify
`client: CloudHSMClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudhsm.client import CloudHSMClient
from types_aiobotocore_cloudhsm.type_defs import AddTagsToResourceResponseTypeDef
from types_aiobotocore_cloudhsm.paginator import ListHapgsPaginator

from types_aiobotocore_cloudhsm.literals import PaginatorName



session = get_session()

async with session.create_client("cloudhsm") as client:
    client: CloudHSMClient

    
    result: AddTagsToResourceResponseTypeDef = client.add_tags_to_resource()
    

    
    paginator_name: PaginatorName = "list_hapgs"
    paginator: ListHapgsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListHapgsResponseTypeDef
        print(item)
    

    
```
