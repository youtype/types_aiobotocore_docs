# Examples

> [Index](../README.md) > [RDSDataService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [RDSDataService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#rdsdataservice)
    type annotations stubs module [types-aiobotocore-rds-data](https://pypi.org/project/types-aiobotocore-rds-data/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[rds-data]` package installed.

Write your `RDSDataService` code as usual,
type checking and code completion should work out of the box.



```python
# RDSDataServiceClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("rds-data") as client:  # (1)
    result = await client.batch_execute_statement()  # (2)
```

1. client: [RDSDataServiceClient](./client.md)
2. result: [:material-code-braces: BatchExecuteStatementResponseTypeDef](./type_defs.md#batchexecutestatementresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[rds-data]`
or a standalone `types_aiobotocore_rds_data` package, you have to explicitly specify
`client: RDSDataServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# RDSDataServiceClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_rds_data.client import RDSDataServiceClient
from types_aiobotocore_rds_data.type_defs import BatchExecuteStatementResponseTypeDef
from types_aiobotocore_rds_data.type_defs import BatchExecuteStatementRequestTypeDef


session = get_session()

async with session.create_client("rds-data") as client:
    client: RDSDataServiceClient
    kwargs: BatchExecuteStatementRequestTypeDef = {...}
    result: BatchExecuteStatementResponseTypeDef = await client.batch_execute_statement(**kwargs)
```




