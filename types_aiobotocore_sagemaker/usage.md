<a id="examples-for-aiobotocore-sagemaker-module"></a>

# Examples for aiobotocore SageMaker module

> [Index](../README.md) > [SageMaker](./README.md) > Examples

- [Examples for aiobotocore SageMaker module](#examples-for-aiobotocore-sagemaker-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[sagemaker]` package installed.

Write your `SageMaker` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type SageMakerClient
# and provides type checking and code completion
async with session.create_client("sagemaker") as client:
    
    # result has type AddAssociationResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_association()
    

    
    # paginator has type ListActionsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_actions")
    async for item in paginator.paginate(...):
        # item has type ListActionsResponseTypeDef
        print(item)
    

    
    # waiter has type EndpointDeletedWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("endpoint_deleted")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[sagemaker]` or a standalone
`types_aiobotocore_sagemaker` package, you have to explicitly specify
`client: SageMakerClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_sagemaker.client import SageMakerClient
from types_aiobotocore_sagemaker.type_defs import AddAssociationResponseTypeDef
from types_aiobotocore_sagemaker.paginator import ListActionsPaginator
from types_aiobotocore_sagemaker.waiter import EndpointDeletedWaiter
from types_aiobotocore_sagemaker.literals import PaginatorName
from types_aiobotocore_sagemaker.literals import WaiterName


session = get_session()

async with session.create_client("sagemaker") as client:
    client: SageMakerClient

    
    result: AddAssociationResponseTypeDef = client.add_association()
    

    
    paginator_name: PaginatorName = "list_actions"
    paginator: ListActionsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListActionsResponseTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "endpoint_deleted"
    waiter: EndpointDeletedWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```
