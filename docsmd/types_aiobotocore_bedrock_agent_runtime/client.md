# AgentsforBedrockRuntimeClient

> [Index](../README.md) > [AgentsforBedrockRuntime](./README.md) > AgentsforBedrockRuntimeClient

!!! note ""

    Auto-generated documentation for [AgentsforBedrockRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#AgentsforBedrockRuntime)
    type annotations stubs module [types-aiobotocore-bedrock-agent-runtime](https://pypi.org/project/types-aiobotocore-bedrock-agent-runtime/).

## AgentsforBedrockRuntimeClient

Type annotations and code completion for `#!python session.create_client("bedrock-agent-runtime")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#AgentsforBedrockRuntime.Client)

```python
# AgentsforBedrockRuntimeClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_bedrock_agent_runtime.client import AgentsforBedrockRuntimeClient

session = get_session()
async with session.create_client("bedrock-agent-runtime") as client:
    client: AgentsforBedrockRuntimeClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("bedrock-agent-runtime").exceptions` structure.

```python
# AgentsforBedrockRuntimeClient.exceptions usage example

async with session.create_client("bedrock-agent-runtime") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.BadGatewayException,
        client.ClientError,
        client.ConflictException,
        client.DependencyFailedException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# AgentsforBedrockRuntimeClient usage type checking example

from types_aiobotocore_bedrock_agent_runtime.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("bedrock-agent-runtime").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#AgentsforBedrockRuntime.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("bedrock-agent-runtime").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#AgentsforBedrockRuntime.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### delete\_agent\_memory

Deletes memory from the specified memory identifier.

Type annotations and code completion for `#!python session.create_client("bedrock-agent-runtime").delete_agent_memory` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#AgentsforBedrockRuntime.Client.delete_agent_memory)

```python
# delete_agent_memory method definition

await def delete_agent_memory(
    self,
    *,
    agentAliasId: str,
    agentId: str,
    memoryId: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_agent_memory method usage example with argument unpacking

kwargs: DeleteAgentMemoryRequestRequestTypeDef = {  # (1)
    "agentAliasId": ...,
    "agentId": ...,
}

parent.delete_agent_memory(**kwargs)
```

1. See [:material-code-braces: DeleteAgentMemoryRequestRequestTypeDef](./type_defs.md#deleteagentmemoryrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("bedrock-agent-runtime").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#AgentsforBedrockRuntime.Client.generate_presigned_url)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### get\_agent\_memory

Gets the sessions stored in the memory of the agent.

Type annotations and code completion for `#!python session.create_client("bedrock-agent-runtime").get_agent_memory` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#AgentsforBedrockRuntime.Client.get_agent_memory)

```python
# get_agent_memory method definition

await def get_agent_memory(
    self,
    *,
    agentAliasId: str,
    agentId: str,
    memoryId: str,
    memoryType: MemoryTypeType,  # (1)
    maxItems: int = ...,
    nextToken: str = ...,
) -> GetAgentMemoryResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: MemoryTypeType](./literals.md#memorytypetype) 
2. See [:material-code-braces: GetAgentMemoryResponseTypeDef](./type_defs.md#getagentmemoryresponsetypedef) 


```python
# get_agent_memory method usage example with argument unpacking

kwargs: GetAgentMemoryRequestRequestTypeDef = {  # (1)
    "agentAliasId": ...,
    "agentId": ...,
    "memoryId": ...,
    "memoryType": ...,
}

parent.get_agent_memory(**kwargs)
```

1. See [:material-code-braces: GetAgentMemoryRequestRequestTypeDef](./type_defs.md#getagentmemoryrequestrequesttypedef) 

### invoke\_agent

.

Type annotations and code completion for `#!python session.create_client("bedrock-agent-runtime").invoke_agent` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#AgentsforBedrockRuntime.Client.invoke_agent)

```python
# invoke_agent method definition

await def invoke_agent(
    self,
    *,
    agentAliasId: str,
    agentId: str,
    sessionId: str,
    enableTrace: bool = ...,
    endSession: bool = ...,
    inputText: str = ...,
    memoryId: str = ...,
    sessionState: SessionStateTypeDef = ...,  # (1)
) -> InvokeAgentResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SessionStateTypeDef](./type_defs.md#sessionstatetypedef) 
2. See [:material-code-braces: InvokeAgentResponseTypeDef](./type_defs.md#invokeagentresponsetypedef) 


```python
# invoke_agent method usage example with argument unpacking

kwargs: InvokeAgentRequestRequestTypeDef = {  # (1)
    "agentAliasId": ...,
    "agentId": ...,
    "sessionId": ...,
}

parent.invoke_agent(**kwargs)
```

1. See [:material-code-braces: InvokeAgentRequestRequestTypeDef](./type_defs.md#invokeagentrequestrequesttypedef) 

### invoke\_flow

Invokes an alias of a flow to run the inputs that you specify and return the
output of each node as a
stream.

Type annotations and code completion for `#!python session.create_client("bedrock-agent-runtime").invoke_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#AgentsforBedrockRuntime.Client.invoke_flow)

```python
# invoke_flow method definition

await def invoke_flow(
    self,
    *,
    flowAliasIdentifier: str,
    flowIdentifier: str,
    inputs: Sequence[FlowInputTypeDef],  # (1)
) -> InvokeFlowResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FlowInputTypeDef](./type_defs.md#flowinputtypedef) 
2. See [:material-code-braces: InvokeFlowResponseTypeDef](./type_defs.md#invokeflowresponsetypedef) 


```python
# invoke_flow method usage example with argument unpacking

kwargs: InvokeFlowRequestRequestTypeDef = {  # (1)
    "flowAliasIdentifier": ...,
    "flowIdentifier": ...,
    "inputs": ...,
}

parent.invoke_flow(**kwargs)
```

1. See [:material-code-braces: InvokeFlowRequestRequestTypeDef](./type_defs.md#invokeflowrequestrequesttypedef) 

### retrieve

Queries a knowledge base and retrieves information from it.

Type annotations and code completion for `#!python session.create_client("bedrock-agent-runtime").retrieve` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#AgentsforBedrockRuntime.Client.retrieve)

```python
# retrieve method definition

await def retrieve(
    self,
    *,
    knowledgeBaseId: str,
    retrievalQuery: KnowledgeBaseQueryTypeDef,  # (1)
    nextToken: str = ...,
    retrievalConfiguration: KnowledgeBaseRetrievalConfigurationTypeDef = ...,  # (2)
) -> RetrieveResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: KnowledgeBaseQueryTypeDef](./type_defs.md#knowledgebasequerytypedef) 
2. See [:material-code-braces: KnowledgeBaseRetrievalConfigurationTypeDef](./type_defs.md#knowledgebaseretrievalconfigurationtypedef) 
3. See [:material-code-braces: RetrieveResponseTypeDef](./type_defs.md#retrieveresponsetypedef) 


```python
# retrieve method usage example with argument unpacking

kwargs: RetrieveRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
    "retrievalQuery": ...,
}

parent.retrieve(**kwargs)
```

1. See [:material-code-braces: RetrieveRequestRequestTypeDef](./type_defs.md#retrieverequestrequesttypedef) 

### retrieve\_and\_generate

Queries a knowledge base and generates responses based on the retrieved results
and using the specified foundation model or [inference
profile](https://docs.aws.amazon.com/bedrock/latest/userguide/cross-region-inference.html).

Type annotations and code completion for `#!python session.create_client("bedrock-agent-runtime").retrieve_and_generate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#AgentsforBedrockRuntime.Client.retrieve_and_generate)

```python
# retrieve_and_generate method definition

await def retrieve_and_generate(
    self,
    *,
    input: RetrieveAndGenerateInputTypeDef,  # (1)
    retrieveAndGenerateConfiguration: RetrieveAndGenerateConfigurationTypeDef = ...,  # (2)
    sessionConfiguration: RetrieveAndGenerateSessionConfigurationTypeDef = ...,  # (3)
    sessionId: str = ...,
) -> RetrieveAndGenerateResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: RetrieveAndGenerateInputTypeDef](./type_defs.md#retrieveandgenerateinputtypedef) 
2. See [:material-code-braces: RetrieveAndGenerateConfigurationTypeDef](./type_defs.md#retrieveandgenerateconfigurationtypedef) 
3. See [:material-code-braces: RetrieveAndGenerateSessionConfigurationTypeDef](./type_defs.md#retrieveandgeneratesessionconfigurationtypedef) 
4. See [:material-code-braces: RetrieveAndGenerateResponseTypeDef](./type_defs.md#retrieveandgenerateresponsetypedef) 


```python
# retrieve_and_generate method usage example with argument unpacking

kwargs: RetrieveAndGenerateRequestRequestTypeDef = {  # (1)
    "input": ...,
}

parent.retrieve_and_generate(**kwargs)
```

1. See [:material-code-braces: RetrieveAndGenerateRequestRequestTypeDef](./type_defs.md#retrieveandgeneraterequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("bedrock-agent-runtime").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#AgentsforBedrockRuntime.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "AgentsforBedrockRuntimeClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("bedrock-agent-runtime").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#AgentsforBedrockRuntime.Client.__aexit__)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("bedrock-agent-runtime").get_paginator` method with overloads.

- `client.get_paginator("get_agent_memory")` -> [GetAgentMemoryPaginator](./paginators.md#getagentmemorypaginator)
- `client.get_paginator("retrieve")` -> [RetrievePaginator](./paginators.md#retrievepaginator)



