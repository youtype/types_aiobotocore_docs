<a id="examples-for-aiobotocore-iot-module"></a>

# Examples for aiobotocore IoT module

> [Index](../README.md) > [IoT](./README.md) > Examples

- [Examples for aiobotocore IoT module](#examples-for-aiobotocore-iot-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[iot]` package installed.

Write your `IoT` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type IoTClient
# and provides type checking and code completion
async with session.create_client("iot") as client:
    
    # result has type None
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.accept_certificate_transfer()
    

    
    # paginator has type GetBehaviorModelTrainingSummariesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("get_behavior_model_training_summaries")
    async for item in paginator.paginate(...):
        # item has type GetBehaviorModelTrainingSummariesResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[iot]` or a standalone `types_aiobotocore_iot`
package, you have to explicitly specify `client: IoTClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_iot.client import IoTClient
from types_aiobotocore_iot.type_defs import None
from types_aiobotocore_iot.paginator import GetBehaviorModelTrainingSummariesPaginator

from types_aiobotocore_iot.literals import PaginatorName



session = get_session()

async with session.create_client("iot") as client:
    client: IoTClient

    
    result: None = client.accept_certificate_transfer()
    

    
    paginator_name: PaginatorName = "get_behavior_model_training_summaries"
    paginator: GetBehaviorModelTrainingSummariesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: GetBehaviorModelTrainingSummariesResponseTypeDef
        print(item)
    

    
```
