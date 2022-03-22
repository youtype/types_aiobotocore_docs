<a id="examples-for-aiobotocore-directoryservice-module"></a>

# Examples for aiobotocore DirectoryService module

> [Index](../README.md) > [DirectoryService](./README.md) > Examples

- [Examples for aiobotocore DirectoryService module](#examples-for-aiobotocore-directoryservice-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[ds]` package installed.

Write your `DirectoryService` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type DirectoryServiceClient
# and provides type checking and code completion
async with session.create_client("ds") as client:
    
    # result has type AcceptSharedDirectoryResultTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.accept_shared_directory()
    

    
    # paginator has type DescribeDirectoriesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_directories")
    async for item in paginator.paginate(...):
        # item has type DescribeDirectoriesResultTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[ds]` or a standalone `types_aiobotocore_ds`
package, you have to explicitly specify `client: DirectoryServiceClient` type
annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_ds.client import DirectoryServiceClient
from types_aiobotocore_ds.type_defs import AcceptSharedDirectoryResultTypeDef
from types_aiobotocore_ds.paginator import DescribeDirectoriesPaginator

from types_aiobotocore_ds.literals import PaginatorName



session = get_session()

async with session.create_client("ds") as client:
    client: DirectoryServiceClient

    
    result: AcceptSharedDirectoryResultTypeDef = client.accept_shared_directory()
    

    
    paginator_name: PaginatorName = "describe_directories"
    paginator: DescribeDirectoriesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeDirectoriesResultTypeDef
        print(item)
    

    
```
