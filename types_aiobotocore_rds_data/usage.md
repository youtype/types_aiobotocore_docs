<a id="examples-for-aiobotocore-rdsdataservice-module"></a>

# Examples for aiobotocore RDSDataService module

> [Index](../README.md) > [RDSDataService](./README.md) > Examples

- [Examples for aiobotocore RDSDataService module](#examples-for-aiobotocore-rdsdataservice-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[rds-data]` package installed.

Write your `RDSDataService` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type RDSDataServiceClient
# and provides type checking and code completion
async with session.create_client("rds-data") as client:
    
    # result has type BatchExecuteStatementResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.batch_execute_statement()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[rds-data]` or a standalone
`types_aiobotocore_rds_data` package, you have to explicitly specify
`client: RDSDataServiceClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_rds_data.client import RDSDataServiceClient
from types_aiobotocore_rds_data.type_defs import BatchExecuteStatementResponseTypeDef






session = get_session()

async with session.create_client("rds-data") as client:
    client: RDSDataServiceClient

    
    result: BatchExecuteStatementResponseTypeDef = client.batch_execute_statement()
    

    

    
```
