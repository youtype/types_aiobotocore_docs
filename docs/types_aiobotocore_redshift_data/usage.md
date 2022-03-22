<a id="examples-for-aiobotocore-redshiftdataapiservice-module"></a>

# Examples for aiobotocore RedshiftDataAPIService module

> [Index](../README.md) > [RedshiftDataAPIService](./README.md) > Examples

- [Examples for aiobotocore RedshiftDataAPIService module](#examples-for-aiobotocore-redshiftdataapiservice-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[redshift-data]` package installed.

Write your `RedshiftDataAPIService` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type RedshiftDataAPIServiceClient
# and provides type checking and code completion
async with session.create_client("redshift-data") as client:
    
    # result has type BatchExecuteStatementOutputTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.batch_execute_statement()
    

    
    # paginator has type DescribeTablePaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_table")
    async for item in paginator.paginate(...):
        # item has type DescribeTableResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[redshift-data]` or a standalone
`types_aiobotocore_redshift_data` package, you have to explicitly specify
`client: RedshiftDataAPIServiceClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_redshift_data.client import RedshiftDataAPIServiceClient
from types_aiobotocore_redshift_data.type_defs import BatchExecuteStatementOutputTypeDef
from types_aiobotocore_redshift_data.paginator import DescribeTablePaginator

from types_aiobotocore_redshift_data.literals import PaginatorName



session = get_session()

async with session.create_client("redshift-data") as client:
    client: RedshiftDataAPIServiceClient

    
    result: BatchExecuteStatementOutputTypeDef = client.batch_execute_statement()
    

    
    paginator_name: PaginatorName = "describe_table"
    paginator: DescribeTablePaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeTableResponseTypeDef
        print(item)
    

    
```
