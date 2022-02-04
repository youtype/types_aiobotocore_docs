<a id="waiters-for-aiobotocore-dynamodb-module"></a>

# Waiters for aiobotocore DynamoDB module

> [Index](..) > [DynamoDB](.) > Waiters

Auto-generated documentation for
[DynamoDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
type annotations stubs module
[types-aiobotocore-dynamodb](https://pypi.org/project/types-aiobotocore-dynamodb/).

- [Waiters for aiobotocore DynamoDB module](#waiters-for-aiobotocore-dynamodb-module)
  - [TableExistsWaiter](#tableexistswaiter)
  - [TableNotExistsWaiter](#tablenotexistswaiter)

<a id="tableexistswaiter"></a>

## TableExistsWaiter

Type annotations for
`aiobotocore.create_client("dynamodb").get_waiter("table_exists")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_dynamodb.waiter import TableExistsWaiter

def get_table_exists_waiter() -> TableExistsWaiter:
    return Session().create_client("dynamodb").get_waiter("table_exists")
```

Boto3 documentation:
[DynamoDB.Waiter.table_exists](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Waiter.TableExists)

Arguments for `TableExistsWaiter.wait` method:

- `TableName`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="tablenotexistswaiter"></a>

## TableNotExistsWaiter

Type annotations for
`aiobotocore.create_client("dynamodb").get_waiter("table_not_exists")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_dynamodb.waiter import TableNotExistsWaiter

def get_table_not_exists_waiter() -> TableNotExistsWaiter:
    return Session().create_client("dynamodb").get_waiter("table_not_exists")
```

Boto3 documentation:
[DynamoDB.Waiter.table_not_exists](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Waiter.TableNotExists)

Arguments for `TableNotExistsWaiter.wait` method:

- `TableName`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
