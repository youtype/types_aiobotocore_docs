<a id="examples-for-aiobotocore-fsx-module"></a>

# Examples for aiobotocore FSx module

> [Index](../README.md) > [FSx](./README.md) > Examples

- [Examples for aiobotocore FSx module](#examples-for-aiobotocore-fsx-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[fsx]` package installed.

Write your `FSx` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type FSxClient
# and provides type checking and code completion
async with session.create_client("fsx") as client:
    
    # result has type AssociateFileSystemAliasesResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_file_system_aliases()
    

    
    # paginator has type DescribeBackupsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_backups")
    async for item in paginator.paginate(...):
        # item has type DescribeBackupsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[fsx]` or a standalone `types_aiobotocore_fsx`
package, you have to explicitly specify `client: FSxClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_fsx.client import FSxClient
from types_aiobotocore_fsx.type_defs import AssociateFileSystemAliasesResponseTypeDef
from types_aiobotocore_fsx.paginator import DescribeBackupsPaginator

from types_aiobotocore_fsx.literals import PaginatorName



session = get_session()

async with session.create_client("fsx") as client:
    client: FSxClient

    
    result: AssociateFileSystemAliasesResponseTypeDef = client.associate_file_system_aliases()
    

    
    paginator_name: PaginatorName = "describe_backups"
    paginator: DescribeBackupsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeBackupsResponseTypeDef
        print(item)
    

    
```
