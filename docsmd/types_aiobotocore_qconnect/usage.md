# Examples

> [Index](../README.md) > [QConnect](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [QConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#qconnect)
    type annotations stubs module [types-aiobotocore-qconnect](https://pypi.org/project/types-aiobotocore-qconnect/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[qconnect]` package installed.

Write your `QConnect` code as usual,
type checking and code completion should work out of the box.



```python
# QConnectClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("qconnect") as client:  # (1)
    result = await client.activate_message_template()  # (2)
```

1. client: [QConnectClient](./client.md)
2. result: [:material-code-braces: ActivateMessageTemplateResponseTypeDef](./type_defs.md#activatemessagetemplateresponsetypedef) 



```python
# ListAIAgentVersionsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("qconnect") as client:  # (1)
    paginator = client.get_paginator("list_ai_agent_versions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [QConnectClient](./client.md)
2. paginator: [ListAIAgentVersionsPaginator](./paginators.md#listaiagentversionspaginator)
3. item: [:material-code-braces: ListAIAgentVersionsResponseTypeDef](./type_defs.md#listaiagentversionsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[qconnect]`
or a standalone `types_aiobotocore_qconnect` package, you have to explicitly specify
`client: QConnectClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# QConnectClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_qconnect.client import QConnectClient
from types_aiobotocore_qconnect.type_defs import ActivateMessageTemplateResponseTypeDef
from types_aiobotocore_qconnect.type_defs import ActivateMessageTemplateRequestTypeDef


session = get_session()

async with session.create_client("qconnect") as client:
    client: QConnectClient
    kwargs: ActivateMessageTemplateRequestTypeDef = {...}
    result: ActivateMessageTemplateResponseTypeDef = await client.activate_message_template(**kwargs)
```



```python
# ListAIAgentVersionsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_qconnect.client import QConnectClient
from types_aiobotocore_qconnect.paginator import ListAIAgentVersionsPaginator
from types_aiobotocore_qconnect.type_defs import ListAIAgentVersionsResponseTypeDef


session = get_session()

async with session.create_client("qconnect") as client:
    client: QConnectClient
    paginator: ListAIAgentVersionsPaginator = client.get_paginator("list_ai_agent_versions")
    async for item in paginator.paginate(...):
        item: ListAIAgentVersionsResponseTypeDef
        print(item)
```


