# Waiters

> [Index](../README.md) > [DynamoDB](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [DynamoDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#dynamodb)
    type annotations stubs module [types-aiobotocore-dynamodb](https://pypi.org/project/types-aiobotocore-dynamodb/).

## TableExistsWaiter

Type annotations and code completion for `#!python session.create_client("dynamodb").get_waiter("table_exists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb/waiter/TableExists.html#DynamoDB.Waiter.TableExists)

```python
# TableExistsWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_dynamodb.waiter import TableExistsWaiter

session = get_session()
async with session.create_client("dynamodb") as client:  # (1)
    waiter: TableExistsWaiter = client.get_waiter("table_exists")  # (2)
    await waiter.wait()
```

1. client: [DynamoDBClient](./client.md)
2. waiter: [TableExistsWaiter](./waiters.md#tableexistswaiter)


### wait

Type annotations and code completion for `#!python TableExistsWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    TableName: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeTableInputWaitTypeDef = {  # (1)
    "TableName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeTableInputWaitTypeDef](./type_defs.md#describetableinputwaittypedef) 
## TableNotExistsWaiter

Type annotations and code completion for `#!python session.create_client("dynamodb").get_waiter("table_not_exists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb/waiter/TableNotExists.html#DynamoDB.Waiter.TableNotExists)

```python
# TableNotExistsWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_dynamodb.waiter import TableNotExistsWaiter

session = get_session()
async with session.create_client("dynamodb") as client:  # (1)
    waiter: TableNotExistsWaiter = client.get_waiter("table_not_exists")  # (2)
    await waiter.wait()
```

1. client: [DynamoDBClient](./client.md)
2. waiter: [TableNotExistsWaiter](./waiters.md#tablenotexistswaiter)


### wait

Type annotations and code completion for `#!python TableNotExistsWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    TableName: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: DescribeTableInputWaitExtraTypeDef = {  # (1)
    "TableName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeTableInputWaitExtraTypeDef](./type_defs.md#describetableinputwaitextratypedef) 
