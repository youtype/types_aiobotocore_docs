# Examples

> [Index](../README.md) > [SecurityAgent](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SecurityAgent](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityagent.html#securityagent)
    type annotations stubs module [types-aiobotocore-securityagent](https://pypi.org/project/types-aiobotocore-securityagent/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[securityagent]` package installed.

Write your `SecurityAgent` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# SecurityAgentClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("securityagent") as client:  # (1)
    result = await client.add_artifact()  # (2)
```

1. client: [SecurityAgentClient](./client.md)
2. result: [:material-code-braces: AddArtifactOutputTypeDef](./type_defs.md#addartifactoutputtypedef)



#### Paginator usage example

```python
# ListAgentSpacesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("securityagent") as client:  # (1)
    paginator = client.get_paginator("list_agent_spaces")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SecurityAgentClient](./client.md)
2. paginator: [ListAgentSpacesPaginator](./paginators.md#listagentspacespaginator)
3. item: [:material-code-braces: ListAgentSpacesOutputTypeDef](./type_defs.md#listagentspacesoutputtypedef)




### Explicit type annotations

With `types-aiobotocore-lite[securityagent]`
or a standalone `types_aiobotocore_securityagent` package, you have to explicitly specify
`client: SecurityAgentClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# SecurityAgentClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_securityagent.client import SecurityAgentClient
from types_aiobotocore_securityagent.type_defs import AddArtifactOutputTypeDef
from types_aiobotocore_securityagent.type_defs import AddArtifactInputTypeDef


session = get_session()

async with session.create_client("securityagent") as client:
    client: SecurityAgentClient
    kwargs: AddArtifactInputTypeDef = {...}
    result: AddArtifactOutputTypeDef = await client.add_artifact(**kwargs)
```



#### Paginator usage example

```python
# ListAgentSpacesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_securityagent.client import SecurityAgentClient
from types_aiobotocore_securityagent.paginator import ListAgentSpacesPaginator
from types_aiobotocore_securityagent.type_defs import ListAgentSpacesOutputTypeDef


session = get_session()

async with session.create_client("securityagent") as client:
    client: SecurityAgentClient
    paginator: ListAgentSpacesPaginator = client.get_paginator("list_agent_spaces")
    async for item in paginator.paginate(...):
        item: ListAgentSpacesOutputTypeDef
        print(item)
```


