# Examples

> [Index](../README.md) > [IoTRoboRunner](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [IoTRoboRunner](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
    type annotations stubs module [types-aiobotocore-iot-roborunner](https://pypi.org/project/types-aiobotocore-iot-roborunner/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[iot-roborunner]` package installed.

Write your `IoTRoboRunner` code as usual,
type checking and code completion should work out of the box.



```python
# IoTRoboRunnerClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("iot-roborunner") as client:  # (1)
    result = await client.create_destination()  # (2)
```

1. client: [IoTRoboRunnerClient](./client.md)
2. result: [:material-code-braces: CreateDestinationResponseTypeDef](./type_defs.md#createdestinationresponsetypedef) 



```python
# ListDestinationsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("iot-roborunner") as client:  # (1)
    paginator = client.get_paginator("list_destinations")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [IoTRoboRunnerClient](./client.md)
2. paginator: [ListDestinationsPaginator](./paginators.md#listdestinationspaginator)
3. item: [:material-code-braces: ListDestinationsResponseTypeDef](./type_defs.md#listdestinationsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[iot-roborunner]`
or a standalone `types_aiobotocore_iot_roborunner` package, you have to explicitly specify
`client: IoTRoboRunnerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# IoTRoboRunnerClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_iot_roborunner.client import IoTRoboRunnerClient
from types_aiobotocore_iot_roborunner.type_defs import CreateDestinationResponseTypeDef
from types_aiobotocore_iot_roborunner.type_defs import CreateDestinationRequestRequestTypeDef


session = get_session()

async with session.create_client("iot-roborunner") as client:
    client: IoTRoboRunnerClient
    kwargs: CreateDestinationRequestRequestTypeDef = {...}
    result: CreateDestinationResponseTypeDef = await client.create_destination(**kwargs)
```



```python
# ListDestinationsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_iot_roborunner.client import IoTRoboRunnerClient
from types_aiobotocore_iot_roborunner.paginator import ListDestinationsPaginator
from types_aiobotocore_iot_roborunner.type_defs import ListDestinationsResponseTypeDef


session = get_session()

async with session.create_client("iot-roborunner") as client:
    client: IoTRoboRunnerClient
    paginator: ListDestinationsPaginator = client.get_paginator("list_destinations")
    async for item in paginator.paginate(...):
        item: ListDestinationsResponseTypeDef
        print(item)
```


