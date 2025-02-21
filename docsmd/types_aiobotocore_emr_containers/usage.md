# Examples

> [Index](../README.md) > [EMRContainers](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [EMRContainers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#emrcontainers)
    type annotations stubs module [types-aiobotocore-emr-containers](https://pypi.org/project/types-aiobotocore-emr-containers/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[emr-containers]` package installed.

Write your `EMRContainers` code as usual,
type checking and code completion should work out of the box.



```python
# EMRContainersClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("emr-containers") as client:  # (1)
    result = await client.cancel_job_run()  # (2)
```

1. client: [EMRContainersClient](./client.md)
2. result: [:material-code-braces: CancelJobRunResponseTypeDef](./type_defs.md#canceljobrunresponsetypedef) 



```python
# ListJobRunsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("emr-containers") as client:  # (1)
    paginator = client.get_paginator("list_job_runs")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [EMRContainersClient](./client.md)
2. paginator: [ListJobRunsPaginator](./paginators.md#listjobrunspaginator)
3. item: [:material-code-braces: ListJobRunsResponsePaginatorTypeDef](./type_defs.md#listjobrunsresponsepaginatortypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[emr-containers]`
or a standalone `types_aiobotocore_emr_containers` package, you have to explicitly specify
`client: EMRContainersClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# EMRContainersClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_emr_containers.client import EMRContainersClient
from types_aiobotocore_emr_containers.type_defs import CancelJobRunResponseTypeDef
from types_aiobotocore_emr_containers.type_defs import CancelJobRunRequestTypeDef


session = get_session()

async with session.create_client("emr-containers") as client:
    client: EMRContainersClient
    kwargs: CancelJobRunRequestTypeDef = {...}
    result: CancelJobRunResponseTypeDef = await client.cancel_job_run(**kwargs)
```



```python
# ListJobRunsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_emr_containers.client import EMRContainersClient
from types_aiobotocore_emr_containers.paginator import ListJobRunsPaginator
from types_aiobotocore_emr_containers.type_defs import ListJobRunsResponsePaginatorTypeDef


session = get_session()

async with session.create_client("emr-containers") as client:
    client: EMRContainersClient
    paginator: ListJobRunsPaginator = client.get_paginator("list_job_runs")
    async for item in paginator.paginate(...):
        item: ListJobRunsResponsePaginatorTypeDef
        print(item)
```


