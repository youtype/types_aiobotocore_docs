<a id="examples-for-aiobotocore-glue-module"></a>

# Examples for aiobotocore Glue module

> [Index](../README.md) > [Glue](./README.md) > Examples

- [Examples for aiobotocore Glue module](#examples-for-aiobotocore-glue-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[glue]` package installed.

Write your `Glue` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type GlueClient
# and provides type checking and code completion
async with session.create_client("glue") as client:
    
    # result has type BatchCreatePartitionResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.batch_create_partition()
    

    
    # paginator has type GetClassifiersPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("get_classifiers")
    async for item in paginator.paginate(...):
        # item has type GetClassifiersResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[glue]` or a standalone `types_aiobotocore_glue`
package, you have to explicitly specify `client: GlueClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_glue.client import GlueClient
from types_aiobotocore_glue.type_defs import BatchCreatePartitionResponseTypeDef
from types_aiobotocore_glue.paginator import GetClassifiersPaginator

from types_aiobotocore_glue.literals import PaginatorName



session = get_session()

async with session.create_client("glue") as client:
    client: GlueClient

    
    result: BatchCreatePartitionResponseTypeDef = client.batch_create_partition()
    

    
    paginator_name: PaginatorName = "get_classifiers"
    paginator: GetClassifiersPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: GetClassifiersResponseTypeDef
        print(item)
    

    
```
