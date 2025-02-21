# Examples

> [Index](../README.md) > [EMRServerless](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [EMRServerless](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#emrserverless)
    type annotations stubs module [types-aiobotocore-emr-serverless](https://pypi.org/project/types-aiobotocore-emr-serverless/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[emr-serverless]` package installed.

Write your `EMRServerless` code as usual,
type checking and code completion should work out of the box.



```python
# EMRServerlessClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("emr-serverless") as client:  # (1)
    result = await client.cancel_job_run()  # (2)
```

1. client: [EMRServerlessClient](./client.md)
2. result: [:material-code-braces: CancelJobRunResponseTypeDef](./type_defs.md#canceljobrunresponsetypedef) 



```python
# ListApplicationsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("emr-serverless") as client:  # (1)
    paginator = client.get_paginator("list_applications")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [EMRServerlessClient](./client.md)
2. paginator: [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
3. item: [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[emr-serverless]`
or a standalone `types_aiobotocore_emr_serverless` package, you have to explicitly specify
`client: EMRServerlessClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# EMRServerlessClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_emr_serverless.client import EMRServerlessClient
from types_aiobotocore_emr_serverless.type_defs import CancelJobRunResponseTypeDef
from types_aiobotocore_emr_serverless.type_defs import CancelJobRunRequestTypeDef


session = get_session()

async with session.create_client("emr-serverless") as client:
    client: EMRServerlessClient
    kwargs: CancelJobRunRequestTypeDef = {...}
    result: CancelJobRunResponseTypeDef = await client.cancel_job_run(**kwargs)
```



```python
# ListApplicationsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_emr_serverless.client import EMRServerlessClient
from types_aiobotocore_emr_serverless.paginator import ListApplicationsPaginator
from types_aiobotocore_emr_serverless.type_defs import ListApplicationsResponseTypeDef


session = get_session()

async with session.create_client("emr-serverless") as client:
    client: EMRServerlessClient
    paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
    async for item in paginator.paginate(...):
        item: ListApplicationsResponseTypeDef
        print(item)
```


