<a id="examples-for-aiobotocore-dynamodb-module"></a>

# Examples for aiobotocore DynamoDB module

> [Index](../README.md) > [DynamoDB](./README.md) > Examples

- [Examples for aiobotocore DynamoDB module](#examples-for-aiobotocore-dynamodb-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[dynamodb]` package installed.

Write your `DynamoDB` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type DynamoDBClient
# and provides type checking and code completion
async with session.create_client("dynamodb") as client:
    
    # result has type BatchExecuteStatementOutputTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.batch_execute_statement()
    

    
    # paginator has type ListBackupsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_backups")
    async for item in paginator.paginate(...):
        # item has type ListBackupsOutputTypeDef
        print(item)
    

    
    # waiter has type TableExistsWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("table_exists")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[dynamodb]` or a standalone
`types_aiobotocore_dynamodb` package, you have to explicitly specify
`client: DynamoDBClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_dynamodb.client import DynamoDBClient
from types_aiobotocore_dynamodb.type_defs import BatchExecuteStatementOutputTypeDef
from types_aiobotocore_dynamodb.paginator import ListBackupsPaginator
from types_aiobotocore_dynamodb.waiter import TableExistsWaiter
from types_aiobotocore_dynamodb.literals import PaginatorName
from types_aiobotocore_dynamodb.literals import WaiterName


session = get_session()

async with session.create_client("dynamodb") as client:
    client: DynamoDBClient

    
    result: BatchExecuteStatementOutputTypeDef = client.batch_execute_statement()
    

    
    paginator_name: PaginatorName = "list_backups"
    paginator: ListBackupsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListBackupsOutputTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "table_exists"
    waiter: TableExistsWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
