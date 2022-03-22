<a id="examples-for-aiobotocore-cloudhsmv2-module"></a>

# Examples for aiobotocore CloudHSMV2 module

> [Index](../README.md) > [CloudHSMV2](./README.md) > Examples

- [Examples for aiobotocore CloudHSMV2 module](#examples-for-aiobotocore-cloudhsmv2-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[cloudhsmv2]` package installed.

Write your `CloudHSMV2` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type CloudHSMV2Client
# and provides type checking and code completion
async with session.create_client("cloudhsmv2") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type DescribeBackupsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_backups")
    async for item in paginator.paginate(...):
        # item has type DescribeBackupsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[cloudhsmv2]` or a standalone
`types_aiobotocore_cloudhsmv2` package, you have to explicitly specify
`client: CloudHSMV2Client` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_cloudhsmv2.client import CloudHSMV2Client
from types_aiobotocore_cloudhsmv2.type_defs import bool
from types_aiobotocore_cloudhsmv2.paginator import DescribeBackupsPaginator

from types_aiobotocore_cloudhsmv2.literals import PaginatorName



session = get_session()

async with session.create_client("cloudhsmv2") as client:
    client: CloudHSMV2Client

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "describe_backups"
    paginator: DescribeBackupsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeBackupsResponseTypeDef
        print(item)
    

    
```
