# Examples

> [Index](../README.md) > [SecurityLake](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SecurityLake](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#securitylake)
    type annotations stubs module [types-aiobotocore-securitylake](https://pypi.org/project/types-aiobotocore-securitylake/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[securitylake]` package installed.

Write your `SecurityLake` code as usual,
type checking and code completion should work out of the box.



```python
# SecurityLakeClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("securitylake") as client:  # (1)
    result = await client.create_aws_log_source()  # (2)
```

1. client: [SecurityLakeClient](./client.md)
2. result: [:material-code-braces: CreateAwsLogSourceResponseTypeDef](./type_defs.md#createawslogsourceresponsetypedef) 



```python
# GetDataLakeSourcesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("securitylake") as client:  # (1)
    paginator = client.get_paginator("get_data_lake_sources")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SecurityLakeClient](./client.md)
2. paginator: [GetDataLakeSourcesPaginator](./paginators.md#getdatalakesourcespaginator)
3. item: [:material-code-braces: GetDataLakeSourcesResponseTypeDef](./type_defs.md#getdatalakesourcesresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[securitylake]`
or a standalone `types_aiobotocore_securitylake` package, you have to explicitly specify
`client: SecurityLakeClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# SecurityLakeClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_securitylake.client import SecurityLakeClient
from types_aiobotocore_securitylake.type_defs import CreateAwsLogSourceResponseTypeDef
from types_aiobotocore_securitylake.type_defs import CreateAwsLogSourceRequestTypeDef


session = get_session()

async with session.create_client("securitylake") as client:
    client: SecurityLakeClient
    kwargs: CreateAwsLogSourceRequestTypeDef = {...}
    result: CreateAwsLogSourceResponseTypeDef = await client.create_aws_log_source(**kwargs)
```



```python
# GetDataLakeSourcesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_securitylake.client import SecurityLakeClient
from types_aiobotocore_securitylake.paginator import GetDataLakeSourcesPaginator
from types_aiobotocore_securitylake.type_defs import GetDataLakeSourcesResponseTypeDef


session = get_session()

async with session.create_client("securitylake") as client:
    client: SecurityLakeClient
    paginator: GetDataLakeSourcesPaginator = client.get_paginator("get_data_lake_sources")
    async for item in paginator.paginate(...):
        item: GetDataLakeSourcesResponseTypeDef
        print(item)
```


