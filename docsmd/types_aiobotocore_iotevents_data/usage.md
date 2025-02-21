# Examples

> [Index](../README.md) > [IoTEventsData](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IoTEventsData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#ioteventsdata)
    type annotations stubs module [types-aiobotocore-iotevents-data](https://pypi.org/project/types-aiobotocore-iotevents-data/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[iotevents-data]` package installed.

Write your `IoTEventsData` code as usual,
type checking and code completion should work out of the box.



```python
# IoTEventsDataClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("iotevents-data") as client:  # (1)
    result = await client.batch_acknowledge_alarm()  # (2)
```

1. client: [IoTEventsDataClient](./client.md)
2. result: [:material-code-braces: BatchAcknowledgeAlarmResponseTypeDef](./type_defs.md#batchacknowledgealarmresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[iotevents-data]`
or a standalone `types_aiobotocore_iotevents_data` package, you have to explicitly specify
`client: IoTEventsDataClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# IoTEventsDataClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_iotevents_data.client import IoTEventsDataClient
from types_aiobotocore_iotevents_data.type_defs import BatchAcknowledgeAlarmResponseTypeDef
from types_aiobotocore_iotevents_data.type_defs import BatchAcknowledgeAlarmRequestTypeDef


session = get_session()

async with session.create_client("iotevents-data") as client:
    client: IoTEventsDataClient
    kwargs: BatchAcknowledgeAlarmRequestTypeDef = {...}
    result: BatchAcknowledgeAlarmResponseTypeDef = await client.batch_acknowledge_alarm(**kwargs)
```




