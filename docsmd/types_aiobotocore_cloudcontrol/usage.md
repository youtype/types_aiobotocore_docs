# Examples

> [Index](../README.md) > [CloudControlApi](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudControlApi](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#cloudcontrolapi)
    type annotations stubs module [types-aiobotocore-cloudcontrol](https://pypi.org/project/types-aiobotocore-cloudcontrol/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[cloudcontrol]` package installed.

Write your `CloudControlApi` code as usual,
type checking and code completion should work out of the box.



```python
# CloudControlApiClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("cloudcontrol") as client:  # (1)
    result = await client.cancel_resource_request()  # (2)
```

1. client: [CloudControlApiClient](./client.md)
2. result: [:material-code-braces: CancelResourceRequestOutputTypeDef](./type_defs.md#cancelresourcerequestoutputtypedef) 



```python
# ListResourceRequestsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("cloudcontrol") as client:  # (1)
    paginator = client.get_paginator("list_resource_requests")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CloudControlApiClient](./client.md)
2. paginator: [ListResourceRequestsPaginator](./paginators.md#listresourcerequestspaginator)
3. item: [:material-code-braces: ListResourceRequestsOutputTypeDef](./type_defs.md#listresourcerequestsoutputtypedef) 



```python
# ResourceRequestSuccessWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("cloudcontrol") as client:  # (1)
    waiter = client.get_waiter("resource_request_success")  # (2)
    await waiter.wait()
```

1. client: [CloudControlApiClient](./client.md)
2. waiter: [ResourceRequestSuccessWaiter](./waiters.md#resourcerequestsuccesswaiter)


### Explicit type annotations

With `types-aiobotocore-lite[cloudcontrol]`
or a standalone `types_aiobotocore_cloudcontrol` package, you have to explicitly specify
`client: CloudControlApiClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# CloudControlApiClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_cloudcontrol.client import CloudControlApiClient
from types_aiobotocore_cloudcontrol.type_defs import CancelResourceRequestOutputTypeDef
from types_aiobotocore_cloudcontrol.type_defs import CancelResourceRequestInputTypeDef


session = get_session()

async with session.create_client("cloudcontrol") as client:
    client: CloudControlApiClient
    kwargs: CancelResourceRequestInputTypeDef = {...}
    result: CancelResourceRequestOutputTypeDef = await client.cancel_resource_request(**kwargs)
```



```python
# ListResourceRequestsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_cloudcontrol.client import CloudControlApiClient
from types_aiobotocore_cloudcontrol.paginator import ListResourceRequestsPaginator
from types_aiobotocore_cloudcontrol.type_defs import ListResourceRequestsOutputTypeDef


session = get_session()

async with session.create_client("cloudcontrol") as client:
    client: CloudControlApiClient
    paginator: ListResourceRequestsPaginator = client.get_paginator("list_resource_requests")
    async for item in paginator.paginate(...):
        item: ListResourceRequestsOutputTypeDef
        print(item)
```



```python
# ResourceRequestSuccessWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_cloudcontrol.client import CloudControlApiClient
from types_aiobotocore_cloudcontrol.waiter import ResourceRequestSuccessWaiter


session = get_session()

async with session.create_client("cloudcontrol") as client:
    client: CloudControlApiClient
    waiter: ResourceRequestSuccessWaiter = client.get_waiter("resource_request_success")
    await waiter.wait()
```
