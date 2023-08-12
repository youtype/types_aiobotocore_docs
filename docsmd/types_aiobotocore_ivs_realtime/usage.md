# Examples

> [Index](../README.md) > [ivsrealtime](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ivsrealtime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
    type annotations stubs module [types-aiobotocore-ivs-realtime](https://pypi.org/project/types-aiobotocore-ivs-realtime/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[ivs-realtime]` package installed.

Write your `ivsrealtime` code as usual,
type checking and code completion should work out of the box.



```python
# ivsrealtimeClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ivs-realtime") as client:  # (1)
    result = await client.create_participant_token()  # (2)
```

1. client: [ivsrealtimeClient](./client.md)
2. result: [:material-code-braces: CreateParticipantTokenResponseTypeDef](./type_defs.md#createparticipanttokenresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[ivs-realtime]`
or a standalone `types_aiobotocore_ivs_realtime` package, you have to explicitly specify
`client: ivsrealtimeClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ivsrealtimeClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ivs_realtime.client import ivsrealtimeClient
from types_aiobotocore_ivs_realtime.type_defs import CreateParticipantTokenResponseTypeDef
from types_aiobotocore_ivs_realtime.type_defs import CreateParticipantTokenRequestRequestTypeDef


session = get_session()

async with session.create_client("ivs-realtime") as client:
    client: ivsrealtimeClient
    kwargs: CreateParticipantTokenRequestRequestTypeDef = {...}
    result: CreateParticipantTokenResponseTypeDef = await client.create_participant_token(**kwargs)
```




