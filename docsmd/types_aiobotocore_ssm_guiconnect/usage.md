# Examples

> [Index](../README.md) > [SSMGUIConnect](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SSMGUIConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-guiconnect.html#ssmguiconnect)
    type annotations stubs module [types-aiobotocore-ssm-guiconnect](https://pypi.org/project/types-aiobotocore-ssm-guiconnect/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[ssm-guiconnect]` package installed.

Write your `SSMGUIConnect` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# SSMGUIConnectClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ssm-guiconnect") as client:  # (1)
    result = await client.delete_connection_recording_preferences()  # (2)
```

1. client: [SSMGUIConnectClient](./client.md)
2. result: [:material-code-braces: DeleteConnectionRecordingPreferencesResponseTypeDef](./type_defs.md#deleteconnectionrecordingpreferencesresponsetypedef)






### Explicit type annotations

With `types-aiobotocore-lite[ssm-guiconnect]`
or a standalone `types_aiobotocore_ssm_guiconnect` package, you have to explicitly specify
`client: SSMGUIConnectClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# SSMGUIConnectClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ssm_guiconnect.client import SSMGUIConnectClient
from types_aiobotocore_ssm_guiconnect.type_defs import DeleteConnectionRecordingPreferencesResponseTypeDef
from types_aiobotocore_ssm_guiconnect.type_defs import DeleteConnectionRecordingPreferencesRequestTypeDef


session = get_session()

async with session.create_client("ssm-guiconnect") as client:
    client: SSMGUIConnectClient
    kwargs: DeleteConnectionRecordingPreferencesRequestTypeDef = {...}
    result: DeleteConnectionRecordingPreferencesResponseTypeDef = await client.delete_connection_recording_preferences(**kwargs)
```




