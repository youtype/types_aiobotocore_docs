# Examples

> [Index](../README.md) > [IoT](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IoT](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#iot)
    type annotations stubs module [types-aiobotocore-iot](https://pypi.org/project/types-aiobotocore-iot/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[iot]` package installed.

Write your `IoT` code as usual,
type checking and code completion should work out of the box.



```python
# IoTClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("iot") as client:  # (1)
    result = await client.accept_certificate_transfer()  # (2)
```

1. client: [IoTClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



```python
# GetBehaviorModelTrainingSummariesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("iot") as client:  # (1)
    paginator = client.get_paginator("get_behavior_model_training_summaries")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [IoTClient](./client.md)
2. paginator: [GetBehaviorModelTrainingSummariesPaginator](./paginators.md#getbehaviormodeltrainingsummariespaginator)
3. item: [:material-code-braces: GetBehaviorModelTrainingSummariesResponseTypeDef](./type_defs.md#getbehaviormodeltrainingsummariesresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[iot]`
or a standalone `types_aiobotocore_iot` package, you have to explicitly specify
`client: IoTClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# IoTClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_iot.client import IoTClient
from types_aiobotocore_iot.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_iot.type_defs import AcceptCertificateTransferRequestTypeDef


session = get_session()

async with session.create_client("iot") as client:
    client: IoTClient
    kwargs: AcceptCertificateTransferRequestTypeDef = {...}
    result: EmptyResponseMetadataTypeDef = await client.accept_certificate_transfer(**kwargs)
```



```python
# GetBehaviorModelTrainingSummariesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_iot.client import IoTClient
from types_aiobotocore_iot.paginator import GetBehaviorModelTrainingSummariesPaginator
from types_aiobotocore_iot.type_defs import GetBehaviorModelTrainingSummariesResponseTypeDef


session = get_session()

async with session.create_client("iot") as client:
    client: IoTClient
    paginator: GetBehaviorModelTrainingSummariesPaginator = client.get_paginator("get_behavior_model_training_summaries")
    async for item in paginator.paginate(...):
        item: GetBehaviorModelTrainingSummariesResponseTypeDef
        print(item)
```


