# Examples

> [Index](../README.md) > [FSx](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [FSx](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#fsx)
    type annotations stubs module [types-aiobotocore-fsx](https://pypi.org/project/types-aiobotocore-fsx/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[fsx]` package installed.

Write your `FSx` code as usual,
type checking and code completion should work out of the box.



```python
# FSxClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("fsx") as client:  # (1)
    result = await client.associate_file_system_aliases()  # (2)
```

1. client: [FSxClient](./client.md)
2. result: [:material-code-braces: AssociateFileSystemAliasesResponseTypeDef](./type_defs.md#associatefilesystemaliasesresponsetypedef) 



```python
# DescribeBackupsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("fsx") as client:  # (1)
    paginator = client.get_paginator("describe_backups")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [FSxClient](./client.md)
2. paginator: [DescribeBackupsPaginator](./paginators.md#describebackupspaginator)
3. item: [:material-code-braces: DescribeBackupsResponsePaginatorTypeDef](./type_defs.md#describebackupsresponsepaginatortypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[fsx]`
or a standalone `types_aiobotocore_fsx` package, you have to explicitly specify
`client: FSxClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# FSxClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_fsx.client import FSxClient
from types_aiobotocore_fsx.type_defs import AssociateFileSystemAliasesResponseTypeDef
from types_aiobotocore_fsx.type_defs import AssociateFileSystemAliasesRequestTypeDef


session = get_session()

async with session.create_client("fsx") as client:
    client: FSxClient
    kwargs: AssociateFileSystemAliasesRequestTypeDef = {...}
    result: AssociateFileSystemAliasesResponseTypeDef = await client.associate_file_system_aliases(**kwargs)
```



```python
# DescribeBackupsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_fsx.client import FSxClient
from types_aiobotocore_fsx.paginator import DescribeBackupsPaginator
from types_aiobotocore_fsx.type_defs import DescribeBackupsResponsePaginatorTypeDef


session = get_session()

async with session.create_client("fsx") as client:
    client: FSxClient
    paginator: DescribeBackupsPaginator = client.get_paginator("describe_backups")
    async for item in paginator.paginate(...):
        item: DescribeBackupsResponsePaginatorTypeDef
        print(item)
```


