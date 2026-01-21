# Examples

> [Index](../README.md) > [PrometheusService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [PrometheusService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#prometheusservice)
    type annotations stubs module [types-aiobotocore-amp](https://pypi.org/project/types-aiobotocore-amp/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[amp]` package installed.

Write your `PrometheusService` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# PrometheusServiceClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("amp") as client:  # (1)
    result = await client.create_alert_manager_definition()  # (2)
```

1. client: [PrometheusServiceClient](./client.md)
2. result: [:material-code-braces: CreateAlertManagerDefinitionResponseTypeDef](./type_defs.md#createalertmanagerdefinitionresponsetypedef)



#### Paginator usage example

```python
# ListAnomalyDetectorsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("amp") as client:  # (1)
    paginator = client.get_paginator("list_anomaly_detectors")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [PrometheusServiceClient](./client.md)
2. paginator: [ListAnomalyDetectorsPaginator](./paginators.md#listanomalydetectorspaginator)
3. item: [:material-code-braces: ListAnomalyDetectorsResponseTypeDef](./type_defs.md#listanomalydetectorsresponsetypedef)



#### Waiter usage example

```python
# AnomalyDetectorActiveWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("amp") as client:  # (1)
    waiter = client.get_waiter("anomaly_detector_active")  # (2)
    await waiter.wait(...)
```

1. client: [PrometheusServiceClient](./client.md)
2. waiter: [AnomalyDetectorActiveWaiter](./waiters.md#anomalydetectoractivewaiter)


### Explicit type annotations

With `types-aiobotocore-lite[amp]`
or a standalone `types_aiobotocore_amp` package, you have to explicitly specify
`client: PrometheusServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# PrometheusServiceClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_amp.client import PrometheusServiceClient
from types_aiobotocore_amp.type_defs import CreateAlertManagerDefinitionResponseTypeDef
from types_aiobotocore_amp.type_defs import CreateAlertManagerDefinitionRequestTypeDef


session = get_session()

async with session.create_client("amp") as client:
    client: PrometheusServiceClient
    kwargs: CreateAlertManagerDefinitionRequestTypeDef = {...}
    result: CreateAlertManagerDefinitionResponseTypeDef = await client.create_alert_manager_definition(**kwargs)
```



#### Paginator usage example

```python
# ListAnomalyDetectorsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_amp.client import PrometheusServiceClient
from types_aiobotocore_amp.paginator import ListAnomalyDetectorsPaginator
from types_aiobotocore_amp.type_defs import ListAnomalyDetectorsResponseTypeDef


session = get_session()

async with session.create_client("amp") as client:
    client: PrometheusServiceClient
    paginator: ListAnomalyDetectorsPaginator = client.get_paginator("list_anomaly_detectors")
    async for item in paginator.paginate(...):
        item: ListAnomalyDetectorsResponseTypeDef
        print(item)
```



#### Waiter usage example

```python
# AnomalyDetectorActiveWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_amp.client import PrometheusServiceClient
from types_aiobotocore_amp.waiter import AnomalyDetectorActiveWaiter


session = get_session()

async with session.create_client("amp") as client:
    client: PrometheusServiceClient
    waiter: AnomalyDetectorActiveWaiter = client.get_waiter("anomaly_detector_active")
    await waiter.wait(...)
```
