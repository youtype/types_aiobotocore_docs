# Examples

> [Index](../README.md) > [AgentsforBedrock](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AgentsforBedrock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#agentsforbedrock)
    type annotations stubs module [types-aiobotocore-bedrock-agent](https://pypi.org/project/types-aiobotocore-bedrock-agent/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[bedrock-agent]` package installed.

Write your `AgentsforBedrock` code as usual,
type checking and code completion should work out of the box.



```python
# AgentsforBedrockClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("bedrock-agent") as client:  # (1)
    result = await client.associate_agent_collaborator()  # (2)
```

1. client: [AgentsforBedrockClient](./client.md)
2. result: [:material-code-braces: AssociateAgentCollaboratorResponseTypeDef](./type_defs.md#associateagentcollaboratorresponsetypedef) 



```python
# ListAgentActionGroupsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("bedrock-agent") as client:  # (1)
    paginator = client.get_paginator("list_agent_action_groups")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [AgentsforBedrockClient](./client.md)
2. paginator: [ListAgentActionGroupsPaginator](./paginators.md#listagentactiongroupspaginator)
3. item: [:material-code-braces: ListAgentActionGroupsResponseTypeDef](./type_defs.md#listagentactiongroupsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[bedrock-agent]`
or a standalone `types_aiobotocore_bedrock_agent` package, you have to explicitly specify
`client: AgentsforBedrockClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# AgentsforBedrockClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agent.client import AgentsforBedrockClient
from types_aiobotocore_bedrock_agent.type_defs import AssociateAgentCollaboratorResponseTypeDef
from types_aiobotocore_bedrock_agent.type_defs import AssociateAgentCollaboratorRequestTypeDef


session = get_session()

async with session.create_client("bedrock-agent") as client:
    client: AgentsforBedrockClient
    kwargs: AssociateAgentCollaboratorRequestTypeDef = {...}
    result: AssociateAgentCollaboratorResponseTypeDef = await client.associate_agent_collaborator(**kwargs)
```



```python
# ListAgentActionGroupsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agent.client import AgentsforBedrockClient
from types_aiobotocore_bedrock_agent.paginator import ListAgentActionGroupsPaginator
from types_aiobotocore_bedrock_agent.type_defs import ListAgentActionGroupsResponseTypeDef


session = get_session()

async with session.create_client("bedrock-agent") as client:
    client: AgentsforBedrockClient
    paginator: ListAgentActionGroupsPaginator = client.get_paginator("list_agent_action_groups")
    async for item in paginator.paginate(...):
        item: ListAgentActionGroupsResponseTypeDef
        print(item)
```


