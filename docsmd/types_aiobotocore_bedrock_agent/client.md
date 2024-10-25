# AgentsforBedrockClient

> [Index](../README.md) > [AgentsforBedrock](./README.md) > AgentsforBedrockClient

!!! note ""

    Auto-generated documentation for [AgentsforBedrock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
    type annotations stubs module [types-aiobotocore-bedrock-agent](https://pypi.org/project/types-aiobotocore-bedrock-agent/).

## AgentsforBedrockClient

Type annotations and code completion for `#!python session.create_client("bedrock-agent")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client)

```python
# AgentsforBedrockClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_bedrock_agent.client import AgentsforBedrockClient

session = get_session()
async with session.create_client("bedrock-agent") as client:
    client: AgentsforBedrockClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("bedrock-agent").exceptions` structure.

```python
# AgentsforBedrockClient.exceptions usage example

async with session.create_client("bedrock-agent") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# AgentsforBedrockClient usage type checking example

from types_aiobotocore_bedrock_agent.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### associate\_agent\_knowledge\_base

Associates a knowledge base with an agent.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").associate_agent_knowledge_base` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.associate_agent_knowledge_base)

```python
# associate_agent_knowledge_base method definition

await def associate_agent_knowledge_base(
    self,
    *,
    agentId: str,
    agentVersion: str,
    description: str,
    knowledgeBaseId: str,
    knowledgeBaseState: KnowledgeBaseStateType = ...,  # (1)
) -> AssociateAgentKnowledgeBaseResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: KnowledgeBaseStateType](./literals.md#knowledgebasestatetype) 
2. See [:material-code-braces: AssociateAgentKnowledgeBaseResponseTypeDef](./type_defs.md#associateagentknowledgebaseresponsetypedef) 


```python
# associate_agent_knowledge_base method usage example with argument unpacking

kwargs: AssociateAgentKnowledgeBaseRequestRequestTypeDef = {  # (1)
    "agentId": ...,
    "agentVersion": ...,
    "description": ...,
    "knowledgeBaseId": ...,
}

parent.associate_agent_knowledge_base(**kwargs)
```

1. See [:material-code-braces: AssociateAgentKnowledgeBaseRequestRequestTypeDef](./type_defs.md#associateagentknowledgebaserequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("bedrock-agent").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_agent

Creates an agent that orchestrates interactions between foundation models, data
sources, software applications, user conversations, and APIs to carry out tasks
to help
customers.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").create_agent` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.create_agent)

```python
# create_agent method definition

await def create_agent(
    self,
    *,
    agentName: str,
    agentResourceRoleArn: str = ...,
    clientToken: str = ...,
    customerEncryptionKeyArn: str = ...,
    description: str = ...,
    foundationModel: str = ...,
    guardrailConfiguration: GuardrailConfigurationTypeDef = ...,  # (1)
    idleSessionTTLInSeconds: int = ...,
    instruction: str = ...,
    memoryConfiguration: MemoryConfigurationTypeDef = ...,  # (2)
    promptOverrideConfiguration: PromptOverrideConfigurationTypeDef = ...,  # (3)
    tags: Mapping[str, str] = ...,
) -> CreateAgentResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef) 
2. See [:material-code-braces: MemoryConfigurationTypeDef](./type_defs.md#memoryconfigurationtypedef) 
3. See [:material-code-braces: PromptOverrideConfigurationTypeDef](./type_defs.md#promptoverrideconfigurationtypedef) 
4. See [:material-code-braces: CreateAgentResponseTypeDef](./type_defs.md#createagentresponsetypedef) 


```python
# create_agent method usage example with argument unpacking

kwargs: CreateAgentRequestRequestTypeDef = {  # (1)
    "agentName": ...,
}

parent.create_agent(**kwargs)
```

1. See [:material-code-braces: CreateAgentRequestRequestTypeDef](./type_defs.md#createagentrequestrequesttypedef) 

### create\_agent\_action\_group

Creates an action group for an agent.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").create_agent_action_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.create_agent_action_group)

```python
# create_agent_action_group method definition

await def create_agent_action_group(
    self,
    *,
    actionGroupName: str,
    agentId: str,
    agentVersion: str,
    actionGroupExecutor: ActionGroupExecutorTypeDef = ...,  # (1)
    actionGroupState: ActionGroupStateType = ...,  # (2)
    apiSchema: APISchemaTypeDef = ...,  # (3)
    clientToken: str = ...,
    description: str = ...,
    functionSchema: FunctionSchemaTypeDef = ...,  # (4)
    parentActionGroupSignature: ActionGroupSignatureType = ...,  # (5)
) -> CreateAgentActionGroupResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: ActionGroupExecutorTypeDef](./type_defs.md#actiongroupexecutortypedef) 
2. See [:material-code-brackets: ActionGroupStateType](./literals.md#actiongroupstatetype) 
3. See [:material-code-braces: APISchemaTypeDef](./type_defs.md#apischematypedef) 
4. See [:material-code-braces: FunctionSchemaTypeDef](./type_defs.md#functionschematypedef) 
5. See [:material-code-brackets: ActionGroupSignatureType](./literals.md#actiongroupsignaturetype) 
6. See [:material-code-braces: CreateAgentActionGroupResponseTypeDef](./type_defs.md#createagentactiongroupresponsetypedef) 


```python
# create_agent_action_group method usage example with argument unpacking

kwargs: CreateAgentActionGroupRequestRequestTypeDef = {  # (1)
    "actionGroupName": ...,
    "agentId": ...,
    "agentVersion": ...,
}

parent.create_agent_action_group(**kwargs)
```

1. See [:material-code-braces: CreateAgentActionGroupRequestRequestTypeDef](./type_defs.md#createagentactiongrouprequestrequesttypedef) 

### create\_agent\_alias

Creates an alias of an agent that can be used to deploy the agent.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").create_agent_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.create_agent_alias)

```python
# create_agent_alias method definition

await def create_agent_alias(
    self,
    *,
    agentAliasName: str,
    agentId: str,
    clientToken: str = ...,
    description: str = ...,
    routingConfiguration: Sequence[AgentAliasRoutingConfigurationListItemTypeDef] = ...,  # (1)
    tags: Mapping[str, str] = ...,
) -> CreateAgentAliasResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AgentAliasRoutingConfigurationListItemTypeDef](./type_defs.md#agentaliasroutingconfigurationlistitemtypedef) 
2. See [:material-code-braces: CreateAgentAliasResponseTypeDef](./type_defs.md#createagentaliasresponsetypedef) 


```python
# create_agent_alias method usage example with argument unpacking

kwargs: CreateAgentAliasRequestRequestTypeDef = {  # (1)
    "agentAliasName": ...,
    "agentId": ...,
}

parent.create_agent_alias(**kwargs)
```

1. See [:material-code-braces: CreateAgentAliasRequestRequestTypeDef](./type_defs.md#createagentaliasrequestrequesttypedef) 

### create\_data\_source

Creates a data source connector for a knowledge base.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").create_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.create_data_source)

```python
# create_data_source method definition

await def create_data_source(
    self,
    *,
    dataSourceConfiguration: DataSourceConfigurationTypeDef,  # (1)
    knowledgeBaseId: str,
    name: str,
    clientToken: str = ...,
    dataDeletionPolicy: DataDeletionPolicyType = ...,  # (2)
    description: str = ...,
    serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,  # (3)
    vectorIngestionConfiguration: VectorIngestionConfigurationTypeDef = ...,  # (4)
) -> CreateDataSourceResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: DataSourceConfigurationTypeDef](./type_defs.md#datasourceconfigurationtypedef) 
2. See [:material-code-brackets: DataDeletionPolicyType](./literals.md#datadeletionpolicytype) 
3. See [:material-code-braces: ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef) 
4. See [:material-code-braces: VectorIngestionConfigurationTypeDef](./type_defs.md#vectoringestionconfigurationtypedef) 
5. See [:material-code-braces: CreateDataSourceResponseTypeDef](./type_defs.md#createdatasourceresponsetypedef) 


```python
# create_data_source method usage example with argument unpacking

kwargs: CreateDataSourceRequestRequestTypeDef = {  # (1)
    "dataSourceConfiguration": ...,
    "knowledgeBaseId": ...,
    "name": ...,
}

parent.create_data_source(**kwargs)
```

1. See [:material-code-braces: CreateDataSourceRequestRequestTypeDef](./type_defs.md#createdatasourcerequestrequesttypedef) 

### create\_flow

Creates a prompt flow that you can use to send an input through various steps
to yield an
output.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").create_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.create_flow)

```python
# create_flow method definition

await def create_flow(
    self,
    *,
    executionRoleArn: str,
    name: str,
    clientToken: str = ...,
    customerEncryptionKeyArn: str = ...,
    definition: FlowDefinitionTypeDef = ...,  # (1)
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateFlowResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FlowDefinitionTypeDef](./type_defs.md#flowdefinitiontypedef) 
2. See [:material-code-braces: CreateFlowResponseTypeDef](./type_defs.md#createflowresponsetypedef) 


```python
# create_flow method usage example with argument unpacking

kwargs: CreateFlowRequestRequestTypeDef = {  # (1)
    "executionRoleArn": ...,
    "name": ...,
}

parent.create_flow(**kwargs)
```

1. See [:material-code-braces: CreateFlowRequestRequestTypeDef](./type_defs.md#createflowrequestrequesttypedef) 

### create\_flow\_alias

Creates an alias of a flow for deployment.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").create_flow_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.create_flow_alias)

```python
# create_flow_alias method definition

await def create_flow_alias(
    self,
    *,
    flowIdentifier: str,
    name: str,
    routingConfiguration: Sequence[FlowAliasRoutingConfigurationListItemTypeDef],  # (1)
    clientToken: str = ...,
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateFlowAliasResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FlowAliasRoutingConfigurationListItemTypeDef](./type_defs.md#flowaliasroutingconfigurationlistitemtypedef) 
2. See [:material-code-braces: CreateFlowAliasResponseTypeDef](./type_defs.md#createflowaliasresponsetypedef) 


```python
# create_flow_alias method usage example with argument unpacking

kwargs: CreateFlowAliasRequestRequestTypeDef = {  # (1)
    "flowIdentifier": ...,
    "name": ...,
    "routingConfiguration": ...,
}

parent.create_flow_alias(**kwargs)
```

1. See [:material-code-braces: CreateFlowAliasRequestRequestTypeDef](./type_defs.md#createflowaliasrequestrequesttypedef) 

### create\_flow\_version

Creates a version of the flow that you can deploy.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").create_flow_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.create_flow_version)

```python
# create_flow_version method definition

await def create_flow_version(
    self,
    *,
    flowIdentifier: str,
    clientToken: str = ...,
    description: str = ...,
) -> CreateFlowVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateFlowVersionResponseTypeDef](./type_defs.md#createflowversionresponsetypedef) 


```python
# create_flow_version method usage example with argument unpacking

kwargs: CreateFlowVersionRequestRequestTypeDef = {  # (1)
    "flowIdentifier": ...,
}

parent.create_flow_version(**kwargs)
```

1. See [:material-code-braces: CreateFlowVersionRequestRequestTypeDef](./type_defs.md#createflowversionrequestrequesttypedef) 

### create\_knowledge\_base

Creates a knowledge base.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").create_knowledge_base` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.create_knowledge_base)

```python
# create_knowledge_base method definition

await def create_knowledge_base(
    self,
    *,
    knowledgeBaseConfiguration: KnowledgeBaseConfigurationTypeDef,  # (1)
    name: str,
    roleArn: str,
    storageConfiguration: StorageConfigurationTypeDef,  # (2)
    clientToken: str = ...,
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateKnowledgeBaseResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: KnowledgeBaseConfigurationTypeDef](./type_defs.md#knowledgebaseconfigurationtypedef) 
2. See [:material-code-braces: StorageConfigurationTypeDef](./type_defs.md#storageconfigurationtypedef) 
3. See [:material-code-braces: CreateKnowledgeBaseResponseTypeDef](./type_defs.md#createknowledgebaseresponsetypedef) 


```python
# create_knowledge_base method usage example with argument unpacking

kwargs: CreateKnowledgeBaseRequestRequestTypeDef = {  # (1)
    "knowledgeBaseConfiguration": ...,
    "name": ...,
    "roleArn": ...,
    "storageConfiguration": ...,
}

parent.create_knowledge_base(**kwargs)
```

1. See [:material-code-braces: CreateKnowledgeBaseRequestRequestTypeDef](./type_defs.md#createknowledgebaserequestrequesttypedef) 

### create\_prompt

Creates a prompt in your prompt library that you can add to a flow.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").create_prompt` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.create_prompt)

```python
# create_prompt method definition

await def create_prompt(
    self,
    *,
    name: str,
    clientToken: str = ...,
    customerEncryptionKeyArn: str = ...,
    defaultVariant: str = ...,
    description: str = ...,
    tags: Mapping[str, str] = ...,
    variants: Sequence[PromptVariantUnionTypeDef] = ...,  # (1)
) -> CreatePromptResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PromptVariantTypeDef](./type_defs.md#promptvarianttypedef) [:material-code-braces: PromptVariantOutputTypeDef](./type_defs.md#promptvariantoutputtypedef) 
2. See [:material-code-braces: CreatePromptResponseTypeDef](./type_defs.md#createpromptresponsetypedef) 


```python
# create_prompt method usage example with argument unpacking

kwargs: CreatePromptRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.create_prompt(**kwargs)
```

1. See [:material-code-braces: CreatePromptRequestRequestTypeDef](./type_defs.md#createpromptrequestrequesttypedef) 

### create\_prompt\_version

Creates a static snapshot of your prompt that can be deployed to production.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").create_prompt_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.create_prompt_version)

```python
# create_prompt_version method definition

await def create_prompt_version(
    self,
    *,
    promptIdentifier: str,
    clientToken: str = ...,
    description: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreatePromptVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreatePromptVersionResponseTypeDef](./type_defs.md#createpromptversionresponsetypedef) 


```python
# create_prompt_version method usage example with argument unpacking

kwargs: CreatePromptVersionRequestRequestTypeDef = {  # (1)
    "promptIdentifier": ...,
}

parent.create_prompt_version(**kwargs)
```

1. See [:material-code-braces: CreatePromptVersionRequestRequestTypeDef](./type_defs.md#createpromptversionrequestrequesttypedef) 

### delete\_agent

Deletes an agent.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").delete_agent` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.delete_agent)

```python
# delete_agent method definition

await def delete_agent(
    self,
    *,
    agentId: str,
    skipResourceInUseCheck: bool = ...,
) -> DeleteAgentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteAgentResponseTypeDef](./type_defs.md#deleteagentresponsetypedef) 


```python
# delete_agent method usage example with argument unpacking

kwargs: DeleteAgentRequestRequestTypeDef = {  # (1)
    "agentId": ...,
}

parent.delete_agent(**kwargs)
```

1. See [:material-code-braces: DeleteAgentRequestRequestTypeDef](./type_defs.md#deleteagentrequestrequesttypedef) 

### delete\_agent\_action\_group

Deletes an action group in an agent.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").delete_agent_action_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.delete_agent_action_group)

```python
# delete_agent_action_group method definition

await def delete_agent_action_group(
    self,
    *,
    actionGroupId: str,
    agentId: str,
    agentVersion: str,
    skipResourceInUseCheck: bool = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_agent_action_group method usage example with argument unpacking

kwargs: DeleteAgentActionGroupRequestRequestTypeDef = {  # (1)
    "actionGroupId": ...,
    "agentId": ...,
    "agentVersion": ...,
}

parent.delete_agent_action_group(**kwargs)
```

1. See [:material-code-braces: DeleteAgentActionGroupRequestRequestTypeDef](./type_defs.md#deleteagentactiongrouprequestrequesttypedef) 

### delete\_agent\_alias

Deletes an alias of an agent.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").delete_agent_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.delete_agent_alias)

```python
# delete_agent_alias method definition

await def delete_agent_alias(
    self,
    *,
    agentAliasId: str,
    agentId: str,
) -> DeleteAgentAliasResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteAgentAliasResponseTypeDef](./type_defs.md#deleteagentaliasresponsetypedef) 


```python
# delete_agent_alias method usage example with argument unpacking

kwargs: DeleteAgentAliasRequestRequestTypeDef = {  # (1)
    "agentAliasId": ...,
    "agentId": ...,
}

parent.delete_agent_alias(**kwargs)
```

1. See [:material-code-braces: DeleteAgentAliasRequestRequestTypeDef](./type_defs.md#deleteagentaliasrequestrequesttypedef) 

### delete\_agent\_version

Deletes a version of an agent.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").delete_agent_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.delete_agent_version)

```python
# delete_agent_version method definition

await def delete_agent_version(
    self,
    *,
    agentId: str,
    agentVersion: str,
    skipResourceInUseCheck: bool = ...,
) -> DeleteAgentVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteAgentVersionResponseTypeDef](./type_defs.md#deleteagentversionresponsetypedef) 


```python
# delete_agent_version method usage example with argument unpacking

kwargs: DeleteAgentVersionRequestRequestTypeDef = {  # (1)
    "agentId": ...,
    "agentVersion": ...,
}

parent.delete_agent_version(**kwargs)
```

1. See [:material-code-braces: DeleteAgentVersionRequestRequestTypeDef](./type_defs.md#deleteagentversionrequestrequesttypedef) 

### delete\_data\_source

Deletes a data source from a knowledge base.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").delete_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.delete_data_source)

```python
# delete_data_source method definition

await def delete_data_source(
    self,
    *,
    dataSourceId: str,
    knowledgeBaseId: str,
) -> DeleteDataSourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteDataSourceResponseTypeDef](./type_defs.md#deletedatasourceresponsetypedef) 


```python
# delete_data_source method usage example with argument unpacking

kwargs: DeleteDataSourceRequestRequestTypeDef = {  # (1)
    "dataSourceId": ...,
    "knowledgeBaseId": ...,
}

parent.delete_data_source(**kwargs)
```

1. See [:material-code-braces: DeleteDataSourceRequestRequestTypeDef](./type_defs.md#deletedatasourcerequestrequesttypedef) 

### delete\_flow

Deletes a flow.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").delete_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.delete_flow)

```python
# delete_flow method definition

await def delete_flow(
    self,
    *,
    flowIdentifier: str,
    skipResourceInUseCheck: bool = ...,
) -> DeleteFlowResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteFlowResponseTypeDef](./type_defs.md#deleteflowresponsetypedef) 


```python
# delete_flow method usage example with argument unpacking

kwargs: DeleteFlowRequestRequestTypeDef = {  # (1)
    "flowIdentifier": ...,
}

parent.delete_flow(**kwargs)
```

1. See [:material-code-braces: DeleteFlowRequestRequestTypeDef](./type_defs.md#deleteflowrequestrequesttypedef) 

### delete\_flow\_alias

Deletes an alias of a flow.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").delete_flow_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.delete_flow_alias)

```python
# delete_flow_alias method definition

await def delete_flow_alias(
    self,
    *,
    aliasIdentifier: str,
    flowIdentifier: str,
) -> DeleteFlowAliasResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteFlowAliasResponseTypeDef](./type_defs.md#deleteflowaliasresponsetypedef) 


```python
# delete_flow_alias method usage example with argument unpacking

kwargs: DeleteFlowAliasRequestRequestTypeDef = {  # (1)
    "aliasIdentifier": ...,
    "flowIdentifier": ...,
}

parent.delete_flow_alias(**kwargs)
```

1. See [:material-code-braces: DeleteFlowAliasRequestRequestTypeDef](./type_defs.md#deleteflowaliasrequestrequesttypedef) 

### delete\_flow\_version

Deletes a version of a flow.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").delete_flow_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.delete_flow_version)

```python
# delete_flow_version method definition

await def delete_flow_version(
    self,
    *,
    flowIdentifier: str,
    flowVersion: str,
    skipResourceInUseCheck: bool = ...,
) -> DeleteFlowVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteFlowVersionResponseTypeDef](./type_defs.md#deleteflowversionresponsetypedef) 


```python
# delete_flow_version method usage example with argument unpacking

kwargs: DeleteFlowVersionRequestRequestTypeDef = {  # (1)
    "flowIdentifier": ...,
    "flowVersion": ...,
}

parent.delete_flow_version(**kwargs)
```

1. See [:material-code-braces: DeleteFlowVersionRequestRequestTypeDef](./type_defs.md#deleteflowversionrequestrequesttypedef) 

### delete\_knowledge\_base

Deletes a knowledge base.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").delete_knowledge_base` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.delete_knowledge_base)

```python
# delete_knowledge_base method definition

await def delete_knowledge_base(
    self,
    *,
    knowledgeBaseId: str,
) -> DeleteKnowledgeBaseResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteKnowledgeBaseResponseTypeDef](./type_defs.md#deleteknowledgebaseresponsetypedef) 


```python
# delete_knowledge_base method usage example with argument unpacking

kwargs: DeleteKnowledgeBaseRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
}

parent.delete_knowledge_base(**kwargs)
```

1. See [:material-code-braces: DeleteKnowledgeBaseRequestRequestTypeDef](./type_defs.md#deleteknowledgebaserequestrequesttypedef) 

### delete\_prompt

Deletes a prompt or a version of it, depending on whether you include the
`promptVersion` field or
not.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").delete_prompt` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.delete_prompt)

```python
# delete_prompt method definition

await def delete_prompt(
    self,
    *,
    promptIdentifier: str,
    promptVersion: str = ...,
) -> DeletePromptResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeletePromptResponseTypeDef](./type_defs.md#deletepromptresponsetypedef) 


```python
# delete_prompt method usage example with argument unpacking

kwargs: DeletePromptRequestRequestTypeDef = {  # (1)
    "promptIdentifier": ...,
}

parent.delete_prompt(**kwargs)
```

1. See [:material-code-braces: DeletePromptRequestRequestTypeDef](./type_defs.md#deletepromptrequestrequesttypedef) 

### disassociate\_agent\_knowledge\_base

Disassociates a knowledge base from an agent.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").disassociate_agent_knowledge_base` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.disassociate_agent_knowledge_base)

```python
# disassociate_agent_knowledge_base method definition

await def disassociate_agent_knowledge_base(
    self,
    *,
    agentId: str,
    agentVersion: str,
    knowledgeBaseId: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_agent_knowledge_base method usage example with argument unpacking

kwargs: DisassociateAgentKnowledgeBaseRequestRequestTypeDef = {  # (1)
    "agentId": ...,
    "agentVersion": ...,
    "knowledgeBaseId": ...,
}

parent.disassociate_agent_knowledge_base(**kwargs)
```

1. See [:material-code-braces: DisassociateAgentKnowledgeBaseRequestRequestTypeDef](./type_defs.md#disassociateagentknowledgebaserequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.generate_presigned_url)

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


### get\_agent

Gets information about an agent.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").get_agent` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.get_agent)

```python
# get_agent method definition

await def get_agent(
    self,
    *,
    agentId: str,
) -> GetAgentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAgentResponseTypeDef](./type_defs.md#getagentresponsetypedef) 


```python
# get_agent method usage example with argument unpacking

kwargs: GetAgentRequestRequestTypeDef = {  # (1)
    "agentId": ...,
}

parent.get_agent(**kwargs)
```

1. See [:material-code-braces: GetAgentRequestRequestTypeDef](./type_defs.md#getagentrequestrequesttypedef) 

### get\_agent\_action\_group

Gets information about an action group for an agent.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").get_agent_action_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.get_agent_action_group)

```python
# get_agent_action_group method definition

await def get_agent_action_group(
    self,
    *,
    actionGroupId: str,
    agentId: str,
    agentVersion: str,
) -> GetAgentActionGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAgentActionGroupResponseTypeDef](./type_defs.md#getagentactiongroupresponsetypedef) 


```python
# get_agent_action_group method usage example with argument unpacking

kwargs: GetAgentActionGroupRequestRequestTypeDef = {  # (1)
    "actionGroupId": ...,
    "agentId": ...,
    "agentVersion": ...,
}

parent.get_agent_action_group(**kwargs)
```

1. See [:material-code-braces: GetAgentActionGroupRequestRequestTypeDef](./type_defs.md#getagentactiongrouprequestrequesttypedef) 

### get\_agent\_alias

Gets information about an alias of an agent.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").get_agent_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.get_agent_alias)

```python
# get_agent_alias method definition

await def get_agent_alias(
    self,
    *,
    agentAliasId: str,
    agentId: str,
) -> GetAgentAliasResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAgentAliasResponseTypeDef](./type_defs.md#getagentaliasresponsetypedef) 


```python
# get_agent_alias method usage example with argument unpacking

kwargs: GetAgentAliasRequestRequestTypeDef = {  # (1)
    "agentAliasId": ...,
    "agentId": ...,
}

parent.get_agent_alias(**kwargs)
```

1. See [:material-code-braces: GetAgentAliasRequestRequestTypeDef](./type_defs.md#getagentaliasrequestrequesttypedef) 

### get\_agent\_knowledge\_base

Gets information about a knowledge base associated with an agent.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").get_agent_knowledge_base` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.get_agent_knowledge_base)

```python
# get_agent_knowledge_base method definition

await def get_agent_knowledge_base(
    self,
    *,
    agentId: str,
    agentVersion: str,
    knowledgeBaseId: str,
) -> GetAgentKnowledgeBaseResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAgentKnowledgeBaseResponseTypeDef](./type_defs.md#getagentknowledgebaseresponsetypedef) 


```python
# get_agent_knowledge_base method usage example with argument unpacking

kwargs: GetAgentKnowledgeBaseRequestRequestTypeDef = {  # (1)
    "agentId": ...,
    "agentVersion": ...,
    "knowledgeBaseId": ...,
}

parent.get_agent_knowledge_base(**kwargs)
```

1. See [:material-code-braces: GetAgentKnowledgeBaseRequestRequestTypeDef](./type_defs.md#getagentknowledgebaserequestrequesttypedef) 

### get\_agent\_version

Gets details about a version of an agent.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").get_agent_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.get_agent_version)

```python
# get_agent_version method definition

await def get_agent_version(
    self,
    *,
    agentId: str,
    agentVersion: str,
) -> GetAgentVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAgentVersionResponseTypeDef](./type_defs.md#getagentversionresponsetypedef) 


```python
# get_agent_version method usage example with argument unpacking

kwargs: GetAgentVersionRequestRequestTypeDef = {  # (1)
    "agentId": ...,
    "agentVersion": ...,
}

parent.get_agent_version(**kwargs)
```

1. See [:material-code-braces: GetAgentVersionRequestRequestTypeDef](./type_defs.md#getagentversionrequestrequesttypedef) 

### get\_data\_source

Gets information about a data source.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").get_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.get_data_source)

```python
# get_data_source method definition

await def get_data_source(
    self,
    *,
    dataSourceId: str,
    knowledgeBaseId: str,
) -> GetDataSourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataSourceResponseTypeDef](./type_defs.md#getdatasourceresponsetypedef) 


```python
# get_data_source method usage example with argument unpacking

kwargs: GetDataSourceRequestRequestTypeDef = {  # (1)
    "dataSourceId": ...,
    "knowledgeBaseId": ...,
}

parent.get_data_source(**kwargs)
```

1. See [:material-code-braces: GetDataSourceRequestRequestTypeDef](./type_defs.md#getdatasourcerequestrequesttypedef) 

### get\_flow

Retrieves information about a flow.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").get_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.get_flow)

```python
# get_flow method definition

await def get_flow(
    self,
    *,
    flowIdentifier: str,
) -> GetFlowResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFlowResponseTypeDef](./type_defs.md#getflowresponsetypedef) 


```python
# get_flow method usage example with argument unpacking

kwargs: GetFlowRequestRequestTypeDef = {  # (1)
    "flowIdentifier": ...,
}

parent.get_flow(**kwargs)
```

1. See [:material-code-braces: GetFlowRequestRequestTypeDef](./type_defs.md#getflowrequestrequesttypedef) 

### get\_flow\_alias

Retrieves information about a flow.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").get_flow_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.get_flow_alias)

```python
# get_flow_alias method definition

await def get_flow_alias(
    self,
    *,
    aliasIdentifier: str,
    flowIdentifier: str,
) -> GetFlowAliasResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFlowAliasResponseTypeDef](./type_defs.md#getflowaliasresponsetypedef) 


```python
# get_flow_alias method usage example with argument unpacking

kwargs: GetFlowAliasRequestRequestTypeDef = {  # (1)
    "aliasIdentifier": ...,
    "flowIdentifier": ...,
}

parent.get_flow_alias(**kwargs)
```

1. See [:material-code-braces: GetFlowAliasRequestRequestTypeDef](./type_defs.md#getflowaliasrequestrequesttypedef) 

### get\_flow\_version

Retrieves information about a version of a flow.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").get_flow_version` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.get_flow_version)

```python
# get_flow_version method definition

await def get_flow_version(
    self,
    *,
    flowIdentifier: str,
    flowVersion: str,
) -> GetFlowVersionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFlowVersionResponseTypeDef](./type_defs.md#getflowversionresponsetypedef) 


```python
# get_flow_version method usage example with argument unpacking

kwargs: GetFlowVersionRequestRequestTypeDef = {  # (1)
    "flowIdentifier": ...,
    "flowVersion": ...,
}

parent.get_flow_version(**kwargs)
```

1. See [:material-code-braces: GetFlowVersionRequestRequestTypeDef](./type_defs.md#getflowversionrequestrequesttypedef) 

### get\_ingestion\_job

Gets information about a data ingestion job.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").get_ingestion_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.get_ingestion_job)

```python
# get_ingestion_job method definition

await def get_ingestion_job(
    self,
    *,
    dataSourceId: str,
    ingestionJobId: str,
    knowledgeBaseId: str,
) -> GetIngestionJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetIngestionJobResponseTypeDef](./type_defs.md#getingestionjobresponsetypedef) 


```python
# get_ingestion_job method usage example with argument unpacking

kwargs: GetIngestionJobRequestRequestTypeDef = {  # (1)
    "dataSourceId": ...,
    "ingestionJobId": ...,
    "knowledgeBaseId": ...,
}

parent.get_ingestion_job(**kwargs)
```

1. See [:material-code-braces: GetIngestionJobRequestRequestTypeDef](./type_defs.md#getingestionjobrequestrequesttypedef) 

### get\_knowledge\_base

Gets information about a knoweldge base.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").get_knowledge_base` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.get_knowledge_base)

```python
# get_knowledge_base method definition

await def get_knowledge_base(
    self,
    *,
    knowledgeBaseId: str,
) -> GetKnowledgeBaseResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetKnowledgeBaseResponseTypeDef](./type_defs.md#getknowledgebaseresponsetypedef) 


```python
# get_knowledge_base method usage example with argument unpacking

kwargs: GetKnowledgeBaseRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
}

parent.get_knowledge_base(**kwargs)
```

1. See [:material-code-braces: GetKnowledgeBaseRequestRequestTypeDef](./type_defs.md#getknowledgebaserequestrequesttypedef) 

### get\_prompt

Retrieves information about the working draft ( `DRAFT` version) of a prompt or
a version of it, depending on whether you include the `promptVersion` field or
not.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").get_prompt` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.get_prompt)

```python
# get_prompt method definition

await def get_prompt(
    self,
    *,
    promptIdentifier: str,
    promptVersion: str = ...,
) -> GetPromptResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPromptResponseTypeDef](./type_defs.md#getpromptresponsetypedef) 


```python
# get_prompt method usage example with argument unpacking

kwargs: GetPromptRequestRequestTypeDef = {  # (1)
    "promptIdentifier": ...,
}

parent.get_prompt(**kwargs)
```

1. See [:material-code-braces: GetPromptRequestRequestTypeDef](./type_defs.md#getpromptrequestrequesttypedef) 

### list\_agent\_action\_groups

Lists the action groups for an agent and information about each one.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").list_agent_action_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.list_agent_action_groups)

```python
# list_agent_action_groups method definition

await def list_agent_action_groups(
    self,
    *,
    agentId: str,
    agentVersion: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAgentActionGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAgentActionGroupsResponseTypeDef](./type_defs.md#listagentactiongroupsresponsetypedef) 


```python
# list_agent_action_groups method usage example with argument unpacking

kwargs: ListAgentActionGroupsRequestRequestTypeDef = {  # (1)
    "agentId": ...,
    "agentVersion": ...,
}

parent.list_agent_action_groups(**kwargs)
```

1. See [:material-code-braces: ListAgentActionGroupsRequestRequestTypeDef](./type_defs.md#listagentactiongroupsrequestrequesttypedef) 

### list\_agent\_aliases

Lists the aliases of an agent and information about each one.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").list_agent_aliases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.list_agent_aliases)

```python
# list_agent_aliases method definition

await def list_agent_aliases(
    self,
    *,
    agentId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAgentAliasesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAgentAliasesResponseTypeDef](./type_defs.md#listagentaliasesresponsetypedef) 


```python
# list_agent_aliases method usage example with argument unpacking

kwargs: ListAgentAliasesRequestRequestTypeDef = {  # (1)
    "agentId": ...,
}

parent.list_agent_aliases(**kwargs)
```

1. See [:material-code-braces: ListAgentAliasesRequestRequestTypeDef](./type_defs.md#listagentaliasesrequestrequesttypedef) 

### list\_agent\_knowledge\_bases

Lists knowledge bases associated with an agent and information about each one.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").list_agent_knowledge_bases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.list_agent_knowledge_bases)

```python
# list_agent_knowledge_bases method definition

await def list_agent_knowledge_bases(
    self,
    *,
    agentId: str,
    agentVersion: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAgentKnowledgeBasesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAgentKnowledgeBasesResponseTypeDef](./type_defs.md#listagentknowledgebasesresponsetypedef) 


```python
# list_agent_knowledge_bases method usage example with argument unpacking

kwargs: ListAgentKnowledgeBasesRequestRequestTypeDef = {  # (1)
    "agentId": ...,
    "agentVersion": ...,
}

parent.list_agent_knowledge_bases(**kwargs)
```

1. See [:material-code-braces: ListAgentKnowledgeBasesRequestRequestTypeDef](./type_defs.md#listagentknowledgebasesrequestrequesttypedef) 

### list\_agent\_versions

Lists the versions of an agent and information about each version.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").list_agent_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.list_agent_versions)

```python
# list_agent_versions method definition

await def list_agent_versions(
    self,
    *,
    agentId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAgentVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAgentVersionsResponseTypeDef](./type_defs.md#listagentversionsresponsetypedef) 


```python
# list_agent_versions method usage example with argument unpacking

kwargs: ListAgentVersionsRequestRequestTypeDef = {  # (1)
    "agentId": ...,
}

parent.list_agent_versions(**kwargs)
```

1. See [:material-code-braces: ListAgentVersionsRequestRequestTypeDef](./type_defs.md#listagentversionsrequestrequesttypedef) 

### list\_agents

Lists the agents belonging to an account and information about each agent.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").list_agents` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.list_agents)

```python
# list_agents method definition

await def list_agents(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAgentsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAgentsResponseTypeDef](./type_defs.md#listagentsresponsetypedef) 


```python
# list_agents method usage example with argument unpacking

kwargs: ListAgentsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_agents(**kwargs)
```

1. See [:material-code-braces: ListAgentsRequestRequestTypeDef](./type_defs.md#listagentsrequestrequesttypedef) 

### list\_data\_sources

Lists the data sources in a knowledge base and information about each one.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").list_data_sources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.list_data_sources)

```python
# list_data_sources method definition

await def list_data_sources(
    self,
    *,
    knowledgeBaseId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListDataSourcesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDataSourcesResponseTypeDef](./type_defs.md#listdatasourcesresponsetypedef) 


```python
# list_data_sources method usage example with argument unpacking

kwargs: ListDataSourcesRequestRequestTypeDef = {  # (1)
    "knowledgeBaseId": ...,
}

parent.list_data_sources(**kwargs)
```

1. See [:material-code-braces: ListDataSourcesRequestRequestTypeDef](./type_defs.md#listdatasourcesrequestrequesttypedef) 

### list\_flow\_aliases

Returns a list of aliases for a flow.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").list_flow_aliases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.list_flow_aliases)

```python
# list_flow_aliases method definition

await def list_flow_aliases(
    self,
    *,
    flowIdentifier: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListFlowAliasesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFlowAliasesResponseTypeDef](./type_defs.md#listflowaliasesresponsetypedef) 


```python
# list_flow_aliases method usage example with argument unpacking

kwargs: ListFlowAliasesRequestRequestTypeDef = {  # (1)
    "flowIdentifier": ...,
}

parent.list_flow_aliases(**kwargs)
```

1. See [:material-code-braces: ListFlowAliasesRequestRequestTypeDef](./type_defs.md#listflowaliasesrequestrequesttypedef) 

### list\_flow\_versions

Returns a list of information about each flow.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").list_flow_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.list_flow_versions)

```python
# list_flow_versions method definition

await def list_flow_versions(
    self,
    *,
    flowIdentifier: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListFlowVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFlowVersionsResponseTypeDef](./type_defs.md#listflowversionsresponsetypedef) 


```python
# list_flow_versions method usage example with argument unpacking

kwargs: ListFlowVersionsRequestRequestTypeDef = {  # (1)
    "flowIdentifier": ...,
}

parent.list_flow_versions(**kwargs)
```

1. See [:material-code-braces: ListFlowVersionsRequestRequestTypeDef](./type_defs.md#listflowversionsrequestrequesttypedef) 

### list\_flows

Returns a list of flows and information about each flow.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").list_flows` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.list_flows)

```python
# list_flows method definition

await def list_flows(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListFlowsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFlowsResponseTypeDef](./type_defs.md#listflowsresponsetypedef) 


```python
# list_flows method usage example with argument unpacking

kwargs: ListFlowsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_flows(**kwargs)
```

1. See [:material-code-braces: ListFlowsRequestRequestTypeDef](./type_defs.md#listflowsrequestrequesttypedef) 

### list\_ingestion\_jobs

Lists the data ingestion jobs for a data source.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").list_ingestion_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.list_ingestion_jobs)

```python
# list_ingestion_jobs method definition

await def list_ingestion_jobs(
    self,
    *,
    dataSourceId: str,
    knowledgeBaseId: str,
    filters: Sequence[IngestionJobFilterTypeDef] = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
    sortBy: IngestionJobSortByTypeDef = ...,  # (2)
) -> ListIngestionJobsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: IngestionJobFilterTypeDef](./type_defs.md#ingestionjobfiltertypedef) 
2. See [:material-code-braces: IngestionJobSortByTypeDef](./type_defs.md#ingestionjobsortbytypedef) 
3. See [:material-code-braces: ListIngestionJobsResponseTypeDef](./type_defs.md#listingestionjobsresponsetypedef) 


```python
# list_ingestion_jobs method usage example with argument unpacking

kwargs: ListIngestionJobsRequestRequestTypeDef = {  # (1)
    "dataSourceId": ...,
    "knowledgeBaseId": ...,
}

parent.list_ingestion_jobs(**kwargs)
```

1. See [:material-code-braces: ListIngestionJobsRequestRequestTypeDef](./type_defs.md#listingestionjobsrequestrequesttypedef) 

### list\_knowledge\_bases

Lists the knowledge bases in an account.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").list_knowledge_bases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.list_knowledge_bases)

```python
# list_knowledge_bases method definition

await def list_knowledge_bases(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListKnowledgeBasesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListKnowledgeBasesResponseTypeDef](./type_defs.md#listknowledgebasesresponsetypedef) 


```python
# list_knowledge_bases method usage example with argument unpacking

kwargs: ListKnowledgeBasesRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_knowledge_bases(**kwargs)
```

1. See [:material-code-braces: ListKnowledgeBasesRequestRequestTypeDef](./type_defs.md#listknowledgebasesrequestrequesttypedef) 

### list\_prompts

Returns either information about the working draft ( `DRAFT` version) of each
prompt in an account, or information about of all versions of a prompt,
depending on whether you include the `promptIdentifier` field or
not.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").list_prompts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.list_prompts)

```python
# list_prompts method definition

await def list_prompts(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    promptIdentifier: str = ...,
) -> ListPromptsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPromptsResponseTypeDef](./type_defs.md#listpromptsresponsetypedef) 


```python
# list_prompts method usage example with argument unpacking

kwargs: ListPromptsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_prompts(**kwargs)
```

1. See [:material-code-braces: ListPromptsRequestRequestTypeDef](./type_defs.md#listpromptsrequestrequesttypedef) 

### list\_tags\_for\_resource

List all the tags for the resource you specify.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### prepare\_agent

Creates a `DRAFT` version of the agent that can be used for internal testing.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").prepare_agent` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.prepare_agent)

```python
# prepare_agent method definition

await def prepare_agent(
    self,
    *,
    agentId: str,
) -> PrepareAgentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PrepareAgentResponseTypeDef](./type_defs.md#prepareagentresponsetypedef) 


```python
# prepare_agent method usage example with argument unpacking

kwargs: PrepareAgentRequestRequestTypeDef = {  # (1)
    "agentId": ...,
}

parent.prepare_agent(**kwargs)
```

1. See [:material-code-braces: PrepareAgentRequestRequestTypeDef](./type_defs.md#prepareagentrequestrequesttypedef) 

### prepare\_flow

Prepares the `DRAFT` version of a flow so that it can be invoked.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").prepare_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.prepare_flow)

```python
# prepare_flow method definition

await def prepare_flow(
    self,
    *,
    flowIdentifier: str,
) -> PrepareFlowResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PrepareFlowResponseTypeDef](./type_defs.md#prepareflowresponsetypedef) 


```python
# prepare_flow method usage example with argument unpacking

kwargs: PrepareFlowRequestRequestTypeDef = {  # (1)
    "flowIdentifier": ...,
}

parent.prepare_flow(**kwargs)
```

1. See [:material-code-braces: PrepareFlowRequestRequestTypeDef](./type_defs.md#prepareflowrequestrequesttypedef) 

### start\_ingestion\_job

Begins a data ingestion job.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").start_ingestion_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.start_ingestion_job)

```python
# start_ingestion_job method definition

await def start_ingestion_job(
    self,
    *,
    dataSourceId: str,
    knowledgeBaseId: str,
    clientToken: str = ...,
    description: str = ...,
) -> StartIngestionJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartIngestionJobResponseTypeDef](./type_defs.md#startingestionjobresponsetypedef) 


```python
# start_ingestion_job method usage example with argument unpacking

kwargs: StartIngestionJobRequestRequestTypeDef = {  # (1)
    "dataSourceId": ...,
    "knowledgeBaseId": ...,
}

parent.start_ingestion_job(**kwargs)
```

1. See [:material-code-braces: StartIngestionJobRequestRequestTypeDef](./type_defs.md#startingestionjobrequestrequesttypedef) 

### stop\_ingestion\_job

Stops a currently running data ingestion job.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").stop_ingestion_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.stop_ingestion_job)

```python
# stop_ingestion_job method definition

await def stop_ingestion_job(
    self,
    *,
    dataSourceId: str,
    ingestionJobId: str,
    knowledgeBaseId: str,
) -> StopIngestionJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopIngestionJobResponseTypeDef](./type_defs.md#stopingestionjobresponsetypedef) 


```python
# stop_ingestion_job method usage example with argument unpacking

kwargs: StopIngestionJobRequestRequestTypeDef = {  # (1)
    "dataSourceId": ...,
    "ingestionJobId": ...,
    "knowledgeBaseId": ...,
}

parent.stop_ingestion_job(**kwargs)
```

1. See [:material-code-braces: StopIngestionJobRequestRequestTypeDef](./type_defs.md#stopingestionjobrequestrequesttypedef) 

### tag\_resource

Associate tags with a resource.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Remove tags from a resource.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_agent

Updates the configuration of an agent.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").update_agent` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_agent)

```python
# update_agent method definition

await def update_agent(
    self,
    *,
    agentId: str,
    agentName: str,
    agentResourceRoleArn: str,
    foundationModel: str,
    customerEncryptionKeyArn: str = ...,
    description: str = ...,
    guardrailConfiguration: GuardrailConfigurationTypeDef = ...,  # (1)
    idleSessionTTLInSeconds: int = ...,
    instruction: str = ...,
    memoryConfiguration: MemoryConfigurationTypeDef = ...,  # (2)
    promptOverrideConfiguration: PromptOverrideConfigurationTypeDef = ...,  # (3)
) -> UpdateAgentResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef) 
2. See [:material-code-braces: MemoryConfigurationTypeDef](./type_defs.md#memoryconfigurationtypedef) 
3. See [:material-code-braces: PromptOverrideConfigurationTypeDef](./type_defs.md#promptoverrideconfigurationtypedef) 
4. See [:material-code-braces: UpdateAgentResponseTypeDef](./type_defs.md#updateagentresponsetypedef) 


```python
# update_agent method usage example with argument unpacking

kwargs: UpdateAgentRequestRequestTypeDef = {  # (1)
    "agentId": ...,
    "agentName": ...,
    "agentResourceRoleArn": ...,
    "foundationModel": ...,
}

parent.update_agent(**kwargs)
```

1. See [:material-code-braces: UpdateAgentRequestRequestTypeDef](./type_defs.md#updateagentrequestrequesttypedef) 

### update\_agent\_action\_group

Updates the configuration for an action group for an agent.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").update_agent_action_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_agent_action_group)

```python
# update_agent_action_group method definition

await def update_agent_action_group(
    self,
    *,
    actionGroupId: str,
    actionGroupName: str,
    agentId: str,
    agentVersion: str,
    actionGroupExecutor: ActionGroupExecutorTypeDef = ...,  # (1)
    actionGroupState: ActionGroupStateType = ...,  # (2)
    apiSchema: APISchemaTypeDef = ...,  # (3)
    description: str = ...,
    functionSchema: FunctionSchemaTypeDef = ...,  # (4)
    parentActionGroupSignature: ActionGroupSignatureType = ...,  # (5)
) -> UpdateAgentActionGroupResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: ActionGroupExecutorTypeDef](./type_defs.md#actiongroupexecutortypedef) 
2. See [:material-code-brackets: ActionGroupStateType](./literals.md#actiongroupstatetype) 
3. See [:material-code-braces: APISchemaTypeDef](./type_defs.md#apischematypedef) 
4. See [:material-code-braces: FunctionSchemaTypeDef](./type_defs.md#functionschematypedef) 
5. See [:material-code-brackets: ActionGroupSignatureType](./literals.md#actiongroupsignaturetype) 
6. See [:material-code-braces: UpdateAgentActionGroupResponseTypeDef](./type_defs.md#updateagentactiongroupresponsetypedef) 


```python
# update_agent_action_group method usage example with argument unpacking

kwargs: UpdateAgentActionGroupRequestRequestTypeDef = {  # (1)
    "actionGroupId": ...,
    "actionGroupName": ...,
    "agentId": ...,
    "agentVersion": ...,
}

parent.update_agent_action_group(**kwargs)
```

1. See [:material-code-braces: UpdateAgentActionGroupRequestRequestTypeDef](./type_defs.md#updateagentactiongrouprequestrequesttypedef) 

### update\_agent\_alias

Updates configurations for an alias of an agent.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").update_agent_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_agent_alias)

```python
# update_agent_alias method definition

await def update_agent_alias(
    self,
    *,
    agentAliasId: str,
    agentAliasName: str,
    agentId: str,
    description: str = ...,
    routingConfiguration: Sequence[AgentAliasRoutingConfigurationListItemTypeDef] = ...,  # (1)
) -> UpdateAgentAliasResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AgentAliasRoutingConfigurationListItemTypeDef](./type_defs.md#agentaliasroutingconfigurationlistitemtypedef) 
2. See [:material-code-braces: UpdateAgentAliasResponseTypeDef](./type_defs.md#updateagentaliasresponsetypedef) 


```python
# update_agent_alias method usage example with argument unpacking

kwargs: UpdateAgentAliasRequestRequestTypeDef = {  # (1)
    "agentAliasId": ...,
    "agentAliasName": ...,
    "agentId": ...,
}

parent.update_agent_alias(**kwargs)
```

1. See [:material-code-braces: UpdateAgentAliasRequestRequestTypeDef](./type_defs.md#updateagentaliasrequestrequesttypedef) 

### update\_agent\_knowledge\_base

Updates the configuration for a knowledge base that has been associated with an
agent.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").update_agent_knowledge_base` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_agent_knowledge_base)

```python
# update_agent_knowledge_base method definition

await def update_agent_knowledge_base(
    self,
    *,
    agentId: str,
    agentVersion: str,
    knowledgeBaseId: str,
    description: str = ...,
    knowledgeBaseState: KnowledgeBaseStateType = ...,  # (1)
) -> UpdateAgentKnowledgeBaseResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: KnowledgeBaseStateType](./literals.md#knowledgebasestatetype) 
2. See [:material-code-braces: UpdateAgentKnowledgeBaseResponseTypeDef](./type_defs.md#updateagentknowledgebaseresponsetypedef) 


```python
# update_agent_knowledge_base method usage example with argument unpacking

kwargs: UpdateAgentKnowledgeBaseRequestRequestTypeDef = {  # (1)
    "agentId": ...,
    "agentVersion": ...,
    "knowledgeBaseId": ...,
}

parent.update_agent_knowledge_base(**kwargs)
```

1. See [:material-code-braces: UpdateAgentKnowledgeBaseRequestRequestTypeDef](./type_defs.md#updateagentknowledgebaserequestrequesttypedef) 

### update\_data\_source

Updates the configurations for a data source connector.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").update_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_data_source)

```python
# update_data_source method definition

await def update_data_source(
    self,
    *,
    dataSourceConfiguration: DataSourceConfigurationTypeDef,  # (1)
    dataSourceId: str,
    knowledgeBaseId: str,
    name: str,
    dataDeletionPolicy: DataDeletionPolicyType = ...,  # (2)
    description: str = ...,
    serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,  # (3)
    vectorIngestionConfiguration: VectorIngestionConfigurationTypeDef = ...,  # (4)
) -> UpdateDataSourceResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: DataSourceConfigurationTypeDef](./type_defs.md#datasourceconfigurationtypedef) 
2. See [:material-code-brackets: DataDeletionPolicyType](./literals.md#datadeletionpolicytype) 
3. See [:material-code-braces: ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef) 
4. See [:material-code-braces: VectorIngestionConfigurationTypeDef](./type_defs.md#vectoringestionconfigurationtypedef) 
5. See [:material-code-braces: UpdateDataSourceResponseTypeDef](./type_defs.md#updatedatasourceresponsetypedef) 


```python
# update_data_source method usage example with argument unpacking

kwargs: UpdateDataSourceRequestRequestTypeDef = {  # (1)
    "dataSourceConfiguration": ...,
    "dataSourceId": ...,
    "knowledgeBaseId": ...,
    "name": ...,
}

parent.update_data_source(**kwargs)
```

1. See [:material-code-braces: UpdateDataSourceRequestRequestTypeDef](./type_defs.md#updatedatasourcerequestrequesttypedef) 

### update\_flow

Modifies a flow.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").update_flow` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_flow)

```python
# update_flow method definition

await def update_flow(
    self,
    *,
    executionRoleArn: str,
    flowIdentifier: str,
    name: str,
    customerEncryptionKeyArn: str = ...,
    definition: FlowDefinitionTypeDef = ...,  # (1)
    description: str = ...,
) -> UpdateFlowResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FlowDefinitionTypeDef](./type_defs.md#flowdefinitiontypedef) 
2. See [:material-code-braces: UpdateFlowResponseTypeDef](./type_defs.md#updateflowresponsetypedef) 


```python
# update_flow method usage example with argument unpacking

kwargs: UpdateFlowRequestRequestTypeDef = {  # (1)
    "executionRoleArn": ...,
    "flowIdentifier": ...,
    "name": ...,
}

parent.update_flow(**kwargs)
```

1. See [:material-code-braces: UpdateFlowRequestRequestTypeDef](./type_defs.md#updateflowrequestrequesttypedef) 

### update\_flow\_alias

Modifies the alias of a flow.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").update_flow_alias` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_flow_alias)

```python
# update_flow_alias method definition

await def update_flow_alias(
    self,
    *,
    aliasIdentifier: str,
    flowIdentifier: str,
    name: str,
    routingConfiguration: Sequence[FlowAliasRoutingConfigurationListItemTypeDef],  # (1)
    description: str = ...,
) -> UpdateFlowAliasResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FlowAliasRoutingConfigurationListItemTypeDef](./type_defs.md#flowaliasroutingconfigurationlistitemtypedef) 
2. See [:material-code-braces: UpdateFlowAliasResponseTypeDef](./type_defs.md#updateflowaliasresponsetypedef) 


```python
# update_flow_alias method usage example with argument unpacking

kwargs: UpdateFlowAliasRequestRequestTypeDef = {  # (1)
    "aliasIdentifier": ...,
    "flowIdentifier": ...,
    "name": ...,
    "routingConfiguration": ...,
}

parent.update_flow_alias(**kwargs)
```

1. See [:material-code-braces: UpdateFlowAliasRequestRequestTypeDef](./type_defs.md#updateflowaliasrequestrequesttypedef) 

### update\_knowledge\_base

Updates the configuration of a knowledge base with the fields that you specify.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").update_knowledge_base` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_knowledge_base)

```python
# update_knowledge_base method definition

await def update_knowledge_base(
    self,
    *,
    knowledgeBaseConfiguration: KnowledgeBaseConfigurationTypeDef,  # (1)
    knowledgeBaseId: str,
    name: str,
    roleArn: str,
    storageConfiguration: StorageConfigurationTypeDef,  # (2)
    description: str = ...,
) -> UpdateKnowledgeBaseResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: KnowledgeBaseConfigurationTypeDef](./type_defs.md#knowledgebaseconfigurationtypedef) 
2. See [:material-code-braces: StorageConfigurationTypeDef](./type_defs.md#storageconfigurationtypedef) 
3. See [:material-code-braces: UpdateKnowledgeBaseResponseTypeDef](./type_defs.md#updateknowledgebaseresponsetypedef) 


```python
# update_knowledge_base method usage example with argument unpacking

kwargs: UpdateKnowledgeBaseRequestRequestTypeDef = {  # (1)
    "knowledgeBaseConfiguration": ...,
    "knowledgeBaseId": ...,
    "name": ...,
    "roleArn": ...,
    "storageConfiguration": ...,
}

parent.update_knowledge_base(**kwargs)
```

1. See [:material-code-braces: UpdateKnowledgeBaseRequestRequestTypeDef](./type_defs.md#updateknowledgebaserequestrequesttypedef) 

### update\_prompt

Modifies a prompt in your prompt library.

Type annotations and code completion for `#!python session.create_client("bedrock-agent").update_prompt` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.update_prompt)

```python
# update_prompt method definition

await def update_prompt(
    self,
    *,
    name: str,
    promptIdentifier: str,
    customerEncryptionKeyArn: str = ...,
    defaultVariant: str = ...,
    description: str = ...,
    variants: Sequence[PromptVariantTypeDef] = ...,  # (1)
) -> UpdatePromptResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PromptVariantTypeDef](./type_defs.md#promptvarianttypedef) 
2. See [:material-code-braces: UpdatePromptResponseTypeDef](./type_defs.md#updatepromptresponsetypedef) 


```python
# update_prompt method usage example with argument unpacking

kwargs: UpdatePromptRequestRequestTypeDef = {  # (1)
    "name": ...,
    "promptIdentifier": ...,
}

parent.update_prompt(**kwargs)
```

1. See [:material-code-braces: UpdatePromptRequestRequestTypeDef](./type_defs.md#updatepromptrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("bedrock-agent").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "AgentsforBedrockClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("bedrock-agent").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("bedrock-agent").get_paginator` method with overloads.

- `client.get_paginator("list_agent_action_groups")` -> [ListAgentActionGroupsPaginator](./paginators.md#listagentactiongroupspaginator)
- `client.get_paginator("list_agent_aliases")` -> [ListAgentAliasesPaginator](./paginators.md#listagentaliasespaginator)
- `client.get_paginator("list_agent_knowledge_bases")` -> [ListAgentKnowledgeBasesPaginator](./paginators.md#listagentknowledgebasespaginator)
- `client.get_paginator("list_agent_versions")` -> [ListAgentVersionsPaginator](./paginators.md#listagentversionspaginator)
- `client.get_paginator("list_agents")` -> [ListAgentsPaginator](./paginators.md#listagentspaginator)
- `client.get_paginator("list_data_sources")` -> [ListDataSourcesPaginator](./paginators.md#listdatasourcespaginator)
- `client.get_paginator("list_flow_aliases")` -> [ListFlowAliasesPaginator](./paginators.md#listflowaliasespaginator)
- `client.get_paginator("list_flow_versions")` -> [ListFlowVersionsPaginator](./paginators.md#listflowversionspaginator)
- `client.get_paginator("list_flows")` -> [ListFlowsPaginator](./paginators.md#listflowspaginator)
- `client.get_paginator("list_ingestion_jobs")` -> [ListIngestionJobsPaginator](./paginators.md#listingestionjobspaginator)
- `client.get_paginator("list_knowledge_bases")` -> [ListKnowledgeBasesPaginator](./paginators.md#listknowledgebasespaginator)
- `client.get_paginator("list_prompts")` -> [ListPromptsPaginator](./paginators.md#listpromptspaginator)



