<a id="examples-for-aiobotocore-ioteventsdata-module"></a>

# Examples for aiobotocore IoTEventsData module

> [Index](../README.md) > [IoTEventsData](./README.md) > Examples

- [Examples for aiobotocore IoTEventsData module](#examples-for-aiobotocore-ioteventsdata-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[iotevents-data]` package installed.

Write your `IoTEventsData` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type IoTEventsDataClient
# and provides type checking and code completion
async with session.create_client("iotevents-data") as client:
    
    # result has type BatchAcknowledgeAlarmResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.batch_acknowledge_alarm()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[iotevents-data]` or a standalone
`types_aiobotocore_iotevents_data` package, you have to explicitly specify
`client: IoTEventsDataClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_iotevents_data.client import IoTEventsDataClient
from types_aiobotocore_iotevents_data.type_defs import BatchAcknowledgeAlarmResponseTypeDef






session = get_session()

async with session.create_client("iotevents-data") as client:
    client: IoTEventsDataClient

    
    result: BatchAcknowledgeAlarmResponseTypeDef = client.batch_acknowledge_alarm()
    

    

    
```
