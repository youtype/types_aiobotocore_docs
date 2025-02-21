# Examples

> [Index](../README.md) > [IoTEvents](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IoTEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#iotevents)
    type annotations stubs module [types-aiobotocore-iotevents](https://pypi.org/project/types-aiobotocore-iotevents/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[iotevents]` package installed.

Write your `IoTEvents` code as usual,
type checking and code completion should work out of the box.



```python
# IoTEventsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("iotevents") as client:  # (1)
    result = await client.create_alarm_model()  # (2)
```

1. client: [IoTEventsClient](./client.md)
2. result: [:material-code-braces: CreateAlarmModelResponseTypeDef](./type_defs.md#createalarmmodelresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[iotevents]`
or a standalone `types_aiobotocore_iotevents` package, you have to explicitly specify
`client: IoTEventsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# IoTEventsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_iotevents.client import IoTEventsClient
from types_aiobotocore_iotevents.type_defs import CreateAlarmModelResponseTypeDef
from types_aiobotocore_iotevents.type_defs import CreateAlarmModelRequestTypeDef


session = get_session()

async with session.create_client("iotevents") as client:
    client: IoTEventsClient
    kwargs: CreateAlarmModelRequestTypeDef = {...}
    result: CreateAlarmModelResponseTypeDef = await client.create_alarm_model(**kwargs)
```




