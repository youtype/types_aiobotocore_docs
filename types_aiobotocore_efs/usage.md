<a id="examples-for-aiobotocore-efs-module"></a>

# Examples for aiobotocore EFS module

> [Index](../README.md) > [EFS](./README.md) > Examples

- [Examples for aiobotocore EFS module](#examples-for-aiobotocore-efs-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[efs]` package installed.

Write your `EFS` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type EFSClient
# and provides type checking and code completion
async with session.create_client("efs") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type DescribeFileSystemsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_file_systems")
    async for item in paginator.paginate(...):
        # item has type DescribeFileSystemsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[efs]` or a standalone `types_aiobotocore_efs`
package, you have to explicitly specify `client: EFSClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_efs.client import EFSClient
from types_aiobotocore_efs.type_defs import bool
from types_aiobotocore_efs.paginator import DescribeFileSystemsPaginator

from types_aiobotocore_efs.literals import PaginatorName



session = get_session()

async with session.create_client("efs") as client:
    client: EFSClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "describe_file_systems"
    paginator: DescribeFileSystemsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeFileSystemsResponseTypeDef
        print(item)
    

    
```
