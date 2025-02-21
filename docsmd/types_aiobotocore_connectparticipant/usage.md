# Examples

> [Index](../README.md) > [ConnectParticipant](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ConnectParticipant](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#connectparticipant)
    type annotations stubs module [types-aiobotocore-connectparticipant](https://pypi.org/project/types-aiobotocore-connectparticipant/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[connectparticipant]` package installed.

Write your `ConnectParticipant` code as usual,
type checking and code completion should work out of the box.



```python
# ConnectParticipantClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("connectparticipant") as client:  # (1)
    result = await client.create_participant_connection()  # (2)
```

1. client: [ConnectParticipantClient](./client.md)
2. result: [:material-code-braces: CreateParticipantConnectionResponseTypeDef](./type_defs.md#createparticipantconnectionresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[connectparticipant]`
or a standalone `types_aiobotocore_connectparticipant` package, you have to explicitly specify
`client: ConnectParticipantClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ConnectParticipantClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_connectparticipant.client import ConnectParticipantClient
from types_aiobotocore_connectparticipant.type_defs import CreateParticipantConnectionResponseTypeDef
from types_aiobotocore_connectparticipant.type_defs import CreateParticipantConnectionRequestTypeDef


session = get_session()

async with session.create_client("connectparticipant") as client:
    client: ConnectParticipantClient
    kwargs: CreateParticipantConnectionRequestTypeDef = {...}
    result: CreateParticipantConnectionResponseTypeDef = await client.create_participant_connection(**kwargs)
```




