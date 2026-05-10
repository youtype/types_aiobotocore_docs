# DevOpsAgentServiceClient

> [Index](../README.md) > [DevOpsAgentService](./README.md) > DevOpsAgentServiceClient

!!! note ""

    Auto-generated documentation for [DevOpsAgentService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent.html#devopsagentservice)
    type annotations stubs module [types-aiobotocore-devops-agent](https://pypi.org/project/types-aiobotocore-devops-agent/).

## DevOpsAgentServiceClient

Type annotations and code completion for `#!python session.create_client("devops-agent")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent.html#DevOpsAgentService.Client)

```python
# DevOpsAgentServiceClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_devops_agent.client import DevOpsAgentServiceClient

session = get_session()
async with session.create_client("devops-agent") as client:
    client: DevOpsAgentServiceClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("devops-agent").exceptions` structure.

```python
# DevOpsAgentServiceClient.exceptions usage example

async with session.create_client("devops-agent") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.ContentSizeExceededException,
        client.IdentityCenterServiceException,
        client.InternalServerException,
        client.InvalidParameterException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# DevOpsAgentServiceClient usage type checking example

from types_aiobotocore_devops_agent.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("devops-agent").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("devops-agent").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/generate_presigned_url.html)

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


### associate\_service

Adds a specific service association to an AgentSpace.

Type annotations and code completion for `#!python session.create_client("devops-agent").associate_service` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/associate_service.html)

```python
# associate_service method definition

await def associate_service(
    self,
    *,
    agentSpaceId: str,
    serviceId: str,
    configuration: ServiceConfigurationUnionTypeDef,  # (1)
) -> AssociateServiceOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ServiceConfigurationUnionTypeDef](#serviceconfigurationuniontypedef)
2. See [:material-code-braces: AssociateServiceOutputTypeDef](./type_defs.md#associateserviceoutputtypedef)


```python
# associate_service method usage example with argument unpacking

kwargs: AssociateServiceInputTypeDef = {  # (1)
    "agentSpaceId": ...,
    "serviceId": ...,
    "configuration": ...,
}

parent.associate_service(**kwargs)
```

1. See [:material-code-braces: AssociateServiceInputTypeDef](./type_defs.md#associateserviceinputtypedef)

### create\_agent\_space

Creates a new AgentSpace with the specified name and description.

Type annotations and code completion for `#!python session.create_client("devops-agent").create_agent_space` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/create_agent_space.html)

```python
# create_agent_space method definition

await def create_agent_space(
    self,
    *,
    name: str,
    description: str = ...,
    locale: str = ...,
    kmsKeyArn: str = ...,
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateAgentSpaceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateAgentSpaceOutputTypeDef](./type_defs.md#createagentspaceoutputtypedef)


```python
# create_agent_space method usage example with argument unpacking

kwargs: CreateAgentSpaceInputTypeDef = {  # (1)
    "name": ...,
}

parent.create_agent_space(**kwargs)
```

1. See [:material-code-braces: CreateAgentSpaceInputTypeDef](./type_defs.md#createagentspaceinputtypedef)

### create\_backlog\_task

Creates a new backlog task in the specified agent space.

Type annotations and code completion for `#!python session.create_client("devops-agent").create_backlog_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/create_backlog_task.html)

```python
# create_backlog_task method definition

await def create_backlog_task(
    self,
    *,
    agentSpaceId: str,
    taskType: TaskTypeType,  # (1)
    title: str,
    priority: PriorityType,  # (2)
    reference: ReferenceInputTypeDef = ...,  # (3)
    description: str = ...,
    clientToken: str = ...,
) -> CreateBacklogTaskResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: TaskTypeType](./literals.md#tasktypetype)
2. See [:material-code-brackets: PriorityType](./literals.md#prioritytype)
3. See [:material-code-braces: ReferenceInputTypeDef](./type_defs.md#referenceinputtypedef)
4. See [:material-code-braces: CreateBacklogTaskResponseTypeDef](./type_defs.md#createbacklogtaskresponsetypedef)


```python
# create_backlog_task method usage example with argument unpacking

kwargs: CreateBacklogTaskRequestTypeDef = {  # (1)
    "agentSpaceId": ...,
    "taskType": ...,
    "title": ...,
    "priority": ...,
}

parent.create_backlog_task(**kwargs)
```

1. See [:material-code-braces: CreateBacklogTaskRequestTypeDef](./type_defs.md#createbacklogtaskrequesttypedef)

### create\_chat

Creates a new chat execution in the specified agent space.

Type annotations and code completion for `#!python session.create_client("devops-agent").create_chat` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/create_chat.html)

```python
# create_chat method definition

await def create_chat(
    self,
    *,
    agentSpaceId: str,
    userId: str = ...,
    userType: UserTypeType = ...,  # (1)
) -> CreateChatResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype)
2. See [:material-code-braces: CreateChatResponseTypeDef](./type_defs.md#createchatresponsetypedef)


```python
# create_chat method usage example with argument unpacking

kwargs: CreateChatRequestTypeDef = {  # (1)
    "agentSpaceId": ...,
}

parent.create_chat(**kwargs)
```

1. See [:material-code-braces: CreateChatRequestTypeDef](./type_defs.md#createchatrequesttypedef)

### create\_private\_connection

Creates a Private Connection to a target resource.

Type annotations and code completion for `#!python session.create_client("devops-agent").create_private_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/create_private_connection.html)

```python
# create_private_connection method definition

await def create_private_connection(
    self,
    *,
    name: str,
    mode: PrivateConnectionModeTypeDef,  # (1)
    tags: Mapping[str, str] = ...,
) -> CreatePrivateConnectionOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PrivateConnectionModeTypeDef](./type_defs.md#privateconnectionmodetypedef)
2. See [:material-code-braces: CreatePrivateConnectionOutputTypeDef](./type_defs.md#createprivateconnectionoutputtypedef)


```python
# create_private_connection method usage example with argument unpacking

kwargs: CreatePrivateConnectionInputTypeDef = {  # (1)
    "name": ...,
    "mode": ...,
}

parent.create_private_connection(**kwargs)
```

1. See [:material-code-braces: CreatePrivateConnectionInputTypeDef](./type_defs.md#createprivateconnectioninputtypedef)

### delete\_agent\_space

Deletes an AgentSpace.

Type annotations and code completion for `#!python session.create_client("devops-agent").delete_agent_space` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/delete_agent_space.html)

```python
# delete_agent_space method definition

await def delete_agent_space(
    self,
    *,
    agentSpaceId: str,
) -> dict[str, Any]:
    ...
```

```python
# delete_agent_space method usage example with argument unpacking

kwargs: DeleteAgentSpaceInputTypeDef = {  # (1)
    "agentSpaceId": ...,
}

parent.delete_agent_space(**kwargs)
```

1. See [:material-code-braces: DeleteAgentSpaceInputTypeDef](./type_defs.md#deleteagentspaceinputtypedef)

### delete\_private\_connection

Deletes a Private Connection.

Type annotations and code completion for `#!python session.create_client("devops-agent").delete_private_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/delete_private_connection.html)

```python
# delete_private_connection method definition

await def delete_private_connection(
    self,
    *,
    name: str,
) -> DeletePrivateConnectionOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeletePrivateConnectionOutputTypeDef](./type_defs.md#deleteprivateconnectionoutputtypedef)


```python
# delete_private_connection method usage example with argument unpacking

kwargs: DeletePrivateConnectionInputTypeDef = {  # (1)
    "name": ...,
}

parent.delete_private_connection(**kwargs)
```

1. See [:material-code-braces: DeletePrivateConnectionInputTypeDef](./type_defs.md#deleteprivateconnectioninputtypedef)

### deregister\_service

Deregister a service.

Type annotations and code completion for `#!python session.create_client("devops-agent").deregister_service` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/deregister_service.html)

```python
# deregister_service method definition

await def deregister_service(
    self,
    *,
    serviceId: str,
) -> dict[str, Any]:
    ...
```

```python
# deregister_service method usage example with argument unpacking

kwargs: DeregisterServiceInputTypeDef = {  # (1)
    "serviceId": ...,
}

parent.deregister_service(**kwargs)
```

1. See [:material-code-braces: DeregisterServiceInputTypeDef](./type_defs.md#deregisterserviceinputtypedef)

### describe\_private\_connection

Retrieves details of an existing Private Connection.

Type annotations and code completion for `#!python session.create_client("devops-agent").describe_private_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/describe_private_connection.html)

```python
# describe_private_connection method definition

await def describe_private_connection(
    self,
    *,
    name: str,
) -> DescribePrivateConnectionOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribePrivateConnectionOutputTypeDef](./type_defs.md#describeprivateconnectionoutputtypedef)


```python
# describe_private_connection method usage example with argument unpacking

kwargs: DescribePrivateConnectionInputTypeDef = {  # (1)
    "name": ...,
}

parent.describe_private_connection(**kwargs)
```

1. See [:material-code-braces: DescribePrivateConnectionInputTypeDef](./type_defs.md#describeprivateconnectioninputtypedef)

### disable\_operator\_app

Disable the Operator App for the specified AgentSpace.

Type annotations and code completion for `#!python session.create_client("devops-agent").disable_operator_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/disable_operator_app.html)

```python
# disable_operator_app method definition

await def disable_operator_app(
    self,
    *,
    agentSpaceId: str,
    authFlow: AuthFlowType = ...,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AuthFlowType](./literals.md#authflowtype)
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# disable_operator_app method usage example with argument unpacking

kwargs: DisableOperatorAppInputTypeDef = {  # (1)
    "agentSpaceId": ...,
}

parent.disable_operator_app(**kwargs)
```

1. See [:material-code-braces: DisableOperatorAppInputTypeDef](./type_defs.md#disableoperatorappinputtypedef)

### disassociate\_service

Deletes a specific service association from an AgentSpace.

Type annotations and code completion for `#!python session.create_client("devops-agent").disassociate_service` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/disassociate_service.html)

```python
# disassociate_service method definition

await def disassociate_service(
    self,
    *,
    agentSpaceId: str,
    associationId: str,
) -> dict[str, Any]:
    ...
```

```python
# disassociate_service method usage example with argument unpacking

kwargs: DisassociateServiceInputTypeDef = {  # (1)
    "agentSpaceId": ...,
    "associationId": ...,
}

parent.disassociate_service(**kwargs)
```

1. See [:material-code-braces: DisassociateServiceInputTypeDef](./type_defs.md#disassociateserviceinputtypedef)

### enable\_operator\_app

Enable the Operator App to access the given AgentSpace.

Type annotations and code completion for `#!python session.create_client("devops-agent").enable_operator_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/enable_operator_app.html)

```python
# enable_operator_app method definition

await def enable_operator_app(
    self,
    *,
    agentSpaceId: str,
    authFlow: AuthFlowType,  # (1)
    operatorAppRoleArn: str,
    idcInstanceArn: str = ...,
    issuerUrl: str = ...,
    idpClientId: str = ...,
    idpClientSecret: str = ...,
    provider: str = ...,
) -> EnableOperatorAppOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AuthFlowType](./literals.md#authflowtype)
2. See [:material-code-braces: EnableOperatorAppOutputTypeDef](./type_defs.md#enableoperatorappoutputtypedef)


```python
# enable_operator_app method usage example with argument unpacking

kwargs: EnableOperatorAppInputTypeDef = {  # (1)
    "agentSpaceId": ...,
    "authFlow": ...,
    "operatorAppRoleArn": ...,
}

parent.enable_operator_app(**kwargs)
```

1. See [:material-code-braces: EnableOperatorAppInputTypeDef](./type_defs.md#enableoperatorappinputtypedef)

### get\_account\_usage

Retrieves monthly account usage metrics and limits for the AWS account.

Type annotations and code completion for `#!python session.create_client("devops-agent").get_account_usage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/get_account_usage.html)

```python
# get_account_usage method definition

await def get_account_usage(
    self,
) -> GetAccountUsageOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccountUsageOutputTypeDef](./type_defs.md#getaccountusageoutputtypedef)



### get\_agent\_space

Retrieves detailed information about a specific AgentSpace.

Type annotations and code completion for `#!python session.create_client("devops-agent").get_agent_space` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/get_agent_space.html)

```python
# get_agent_space method definition

await def get_agent_space(
    self,
    *,
    agentSpaceId: str,
) -> GetAgentSpaceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAgentSpaceOutputTypeDef](./type_defs.md#getagentspaceoutputtypedef)


```python
# get_agent_space method usage example with argument unpacking

kwargs: GetAgentSpaceInputTypeDef = {  # (1)
    "agentSpaceId": ...,
}

parent.get_agent_space(**kwargs)
```

1. See [:material-code-braces: GetAgentSpaceInputTypeDef](./type_defs.md#getagentspaceinputtypedef)

### get\_association

Retrieves given associations configured for a specific AgentSpace.

Type annotations and code completion for `#!python session.create_client("devops-agent").get_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/get_association.html)

```python
# get_association method definition

await def get_association(
    self,
    *,
    agentSpaceId: str,
    associationId: str,
) -> GetAssociationOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAssociationOutputTypeDef](./type_defs.md#getassociationoutputtypedef)


```python
# get_association method usage example with argument unpacking

kwargs: GetAssociationInputTypeDef = {  # (1)
    "agentSpaceId": ...,
    "associationId": ...,
}

parent.get_association(**kwargs)
```

1. See [:material-code-braces: GetAssociationInputTypeDef](./type_defs.md#getassociationinputtypedef)

### get\_backlog\_task

Gets a backlog task for the specified agent space and task id.

Type annotations and code completion for `#!python session.create_client("devops-agent").get_backlog_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/get_backlog_task.html)

```python
# get_backlog_task method definition

await def get_backlog_task(
    self,
    *,
    agentSpaceId: str,
    taskId: str,
) -> GetBacklogTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetBacklogTaskResponseTypeDef](./type_defs.md#getbacklogtaskresponsetypedef)


```python
# get_backlog_task method usage example with argument unpacking

kwargs: GetBacklogTaskRequestTypeDef = {  # (1)
    "agentSpaceId": ...,
    "taskId": ...,
}

parent.get_backlog_task(**kwargs)
```

1. See [:material-code-braces: GetBacklogTaskRequestTypeDef](./type_defs.md#getbacklogtaskrequesttypedef)

### get\_operator\_app

Get the full auth configuration of operator including any enabled auth flow.

Type annotations and code completion for `#!python session.create_client("devops-agent").get_operator_app` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/get_operator_app.html)

```python
# get_operator_app method definition

await def get_operator_app(
    self,
    *,
    agentSpaceId: str,
) -> GetOperatorAppOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOperatorAppOutputTypeDef](./type_defs.md#getoperatorappoutputtypedef)


```python
# get_operator_app method usage example with argument unpacking

kwargs: GetOperatorAppInputTypeDef = {  # (1)
    "agentSpaceId": ...,
}

parent.get_operator_app(**kwargs)
```

1. See [:material-code-braces: GetOperatorAppInputTypeDef](./type_defs.md#getoperatorappinputtypedef)

### get\_recommendation

Retrieves a specific recommendation by its ID.

Type annotations and code completion for `#!python session.create_client("devops-agent").get_recommendation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/get_recommendation.html)

```python
# get_recommendation method definition

await def get_recommendation(
    self,
    *,
    agentSpaceId: str,
    recommendationId: str,
    recommendationVersion: int = ...,
) -> GetRecommendationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRecommendationResponseTypeDef](./type_defs.md#getrecommendationresponsetypedef)


```python
# get_recommendation method usage example with argument unpacking

kwargs: GetRecommendationRequestTypeDef = {  # (1)
    "agentSpaceId": ...,
    "recommendationId": ...,
}

parent.get_recommendation(**kwargs)
```

1. See [:material-code-braces: GetRecommendationRequestTypeDef](./type_defs.md#getrecommendationrequesttypedef)

### get\_service

Retrieves given service by it's unique identifier.

Type annotations and code completion for `#!python session.create_client("devops-agent").get_service` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/get_service.html)

```python
# get_service method definition

await def get_service(
    self,
    *,
    serviceId: str,
) -> GetServiceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetServiceOutputTypeDef](./type_defs.md#getserviceoutputtypedef)


```python
# get_service method usage example with argument unpacking

kwargs: GetServiceInputTypeDef = {  # (1)
    "serviceId": ...,
}

parent.get_service(**kwargs)
```

1. See [:material-code-braces: GetServiceInputTypeDef](./type_defs.md#getserviceinputtypedef)

### list\_agent\_spaces

Lists all AgentSpaces with optional pagination.

Type annotations and code completion for `#!python session.create_client("devops-agent").list_agent_spaces` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/list_agent_spaces.html)

```python
# list_agent_spaces method definition

await def list_agent_spaces(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAgentSpacesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAgentSpacesOutputTypeDef](./type_defs.md#listagentspacesoutputtypedef)


```python
# list_agent_spaces method usage example with argument unpacking

kwargs: ListAgentSpacesInputTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_agent_spaces(**kwargs)
```

1. See [:material-code-braces: ListAgentSpacesInputTypeDef](./type_defs.md#listagentspacesinputtypedef)

### list\_associations

List all associations for given AgentSpace.

Type annotations and code completion for `#!python session.create_client("devops-agent").list_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/list_associations.html)

```python
# list_associations method definition

await def list_associations(
    self,
    *,
    agentSpaceId: str,
    maxResults: int = ...,
    nextToken: str = ...,
    filterServiceTypes: str = ...,
) -> ListAssociationsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAssociationsOutputTypeDef](./type_defs.md#listassociationsoutputtypedef)


```python
# list_associations method usage example with argument unpacking

kwargs: ListAssociationsInputTypeDef = {  # (1)
    "agentSpaceId": ...,
}

parent.list_associations(**kwargs)
```

1. See [:material-code-braces: ListAssociationsInputTypeDef](./type_defs.md#listassociationsinputtypedef)

### list\_backlog\_tasks

Lists backlog tasks in the specified agent space with optional filtering and
sorting.

Type annotations and code completion for `#!python session.create_client("devops-agent").list_backlog_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/list_backlog_tasks.html)

```python
# list_backlog_tasks method definition

await def list_backlog_tasks(
    self,
    *,
    agentSpaceId: str,
    filter: TaskFilterTypeDef = ...,  # (1)
    limit: int = ...,
    nextToken: str = ...,
    sortField: TaskSortFieldType = ...,  # (2)
    order: TaskSortOrderType = ...,  # (3)
) -> ListBacklogTasksResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: TaskFilterTypeDef](./type_defs.md#taskfiltertypedef)
2. See [:material-code-brackets: TaskSortFieldType](./literals.md#tasksortfieldtype)
3. See [:material-code-brackets: TaskSortOrderType](./literals.md#tasksortordertype)
4. See [:material-code-braces: ListBacklogTasksResponseTypeDef](./type_defs.md#listbacklogtasksresponsetypedef)


```python
# list_backlog_tasks method usage example with argument unpacking

kwargs: ListBacklogTasksRequestTypeDef = {  # (1)
    "agentSpaceId": ...,
}

parent.list_backlog_tasks(**kwargs)
```

1. See [:material-code-braces: ListBacklogTasksRequestTypeDef](./type_defs.md#listbacklogtasksrequesttypedef)

### list\_chats

Retrieves a paginated list of the user's recent chat executions.

Type annotations and code completion for `#!python session.create_client("devops-agent").list_chats` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/list_chats.html)

```python
# list_chats method definition

await def list_chats(
    self,
    *,
    agentSpaceId: str,
    userId: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListChatsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListChatsResponseTypeDef](./type_defs.md#listchatsresponsetypedef)


```python
# list_chats method usage example with argument unpacking

kwargs: ListChatsRequestTypeDef = {  # (1)
    "agentSpaceId": ...,
}

parent.list_chats(**kwargs)
```

1. See [:material-code-braces: ListChatsRequestTypeDef](./type_defs.md#listchatsrequesttypedef)

### list\_executions

List executions.

Type annotations and code completion for `#!python session.create_client("devops-agent").list_executions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/list_executions.html)

```python
# list_executions method definition

await def list_executions(
    self,
    *,
    agentSpaceId: str,
    taskId: str,
    limit: int = ...,
    nextToken: str = ...,
) -> ListExecutionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListExecutionsResponseTypeDef](./type_defs.md#listexecutionsresponsetypedef)


```python
# list_executions method usage example with argument unpacking

kwargs: ListExecutionsRequestTypeDef = {  # (1)
    "agentSpaceId": ...,
    "taskId": ...,
}

parent.list_executions(**kwargs)
```

1. See [:material-code-braces: ListExecutionsRequestTypeDef](./type_defs.md#listexecutionsrequesttypedef)

### list\_goals

Lists goals in the specified agent space with optional filtering.

Type annotations and code completion for `#!python session.create_client("devops-agent").list_goals` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/list_goals.html)

```python
# list_goals method definition

await def list_goals(
    self,
    *,
    agentSpaceId: str,
    status: GoalStatusType = ...,  # (1)
    goalType: GoalTypeType = ...,  # (2)
    limit: int = ...,
    nextToken: str = ...,
) -> ListGoalsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: GoalStatusType](./literals.md#goalstatustype)
2. See [:material-code-brackets: GoalTypeType](./literals.md#goaltypetype)
3. See [:material-code-braces: ListGoalsResponseTypeDef](./type_defs.md#listgoalsresponsetypedef)


```python
# list_goals method usage example with argument unpacking

kwargs: ListGoalsRequestTypeDef = {  # (1)
    "agentSpaceId": ...,
}

parent.list_goals(**kwargs)
```

1. See [:material-code-braces: ListGoalsRequestTypeDef](./type_defs.md#listgoalsrequesttypedef)

### list\_journal\_records

List journal records for a specific execution.

Type annotations and code completion for `#!python session.create_client("devops-agent").list_journal_records` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/list_journal_records.html)

```python
# list_journal_records method definition

await def list_journal_records(
    self,
    *,
    agentSpaceId: str,
    executionId: str,
    limit: int = ...,
    nextToken: str = ...,
    recordType: str = ...,
    order: OrderTypeType = ...,  # (1)
) -> ListJournalRecordsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: OrderTypeType](./literals.md#ordertypetype)
2. See [:material-code-braces: ListJournalRecordsResponseTypeDef](./type_defs.md#listjournalrecordsresponsetypedef)


```python
# list_journal_records method usage example with argument unpacking

kwargs: ListJournalRecordsRequestTypeDef = {  # (1)
    "agentSpaceId": ...,
    "executionId": ...,
}

parent.list_journal_records(**kwargs)
```

1. See [:material-code-braces: ListJournalRecordsRequestTypeDef](./type_defs.md#listjournalrecordsrequesttypedef)

### list\_pending\_messages

List pending messages for a specific execution.

Type annotations and code completion for `#!python session.create_client("devops-agent").list_pending_messages` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/list_pending_messages.html)

```python
# list_pending_messages method definition

await def list_pending_messages(
    self,
    *,
    agentSpaceId: str,
    executionId: str,
) -> ListPendingMessagesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPendingMessagesResponseTypeDef](./type_defs.md#listpendingmessagesresponsetypedef)


```python
# list_pending_messages method usage example with argument unpacking

kwargs: ListPendingMessagesRequestTypeDef = {  # (1)
    "agentSpaceId": ...,
    "executionId": ...,
}

parent.list_pending_messages(**kwargs)
```

1. See [:material-code-braces: ListPendingMessagesRequestTypeDef](./type_defs.md#listpendingmessagesrequesttypedef)

### list\_private\_connections

Lists all Private Connections in the caller's account.

Type annotations and code completion for `#!python session.create_client("devops-agent").list_private_connections` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/list_private_connections.html)

```python
# list_private_connections method definition

await def list_private_connections(
    self,
) -> ListPrivateConnectionsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPrivateConnectionsOutputTypeDef](./type_defs.md#listprivateconnectionsoutputtypedef)



### list\_recommendations

Lists recommendations for the specified agent space.

Type annotations and code completion for `#!python session.create_client("devops-agent").list_recommendations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/list_recommendations.html)

```python
# list_recommendations method definition

await def list_recommendations(
    self,
    *,
    agentSpaceId: str,
    taskId: str = ...,
    goalId: str = ...,
    status: RecommendationStatusType = ...,  # (1)
    priority: RecommendationPriorityType = ...,  # (2)
    limit: int = ...,
    nextToken: str = ...,
) -> ListRecommendationsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: RecommendationStatusType](./literals.md#recommendationstatustype)
2. See [:material-code-brackets: RecommendationPriorityType](./literals.md#recommendationprioritytype)
3. See [:material-code-braces: ListRecommendationsResponseTypeDef](./type_defs.md#listrecommendationsresponsetypedef)


```python
# list_recommendations method usage example with argument unpacking

kwargs: ListRecommendationsRequestTypeDef = {  # (1)
    "agentSpaceId": ...,
}

parent.list_recommendations(**kwargs)
```

1. See [:material-code-braces: ListRecommendationsRequestTypeDef](./type_defs.md#listrecommendationsrequesttypedef)

### list\_services

List a list of registered service on the account level.

Type annotations and code completion for `#!python session.create_client("devops-agent").list_services` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/list_services.html)

```python
# list_services method definition

await def list_services(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    filterServiceType: ServiceType = ...,  # (1)
) -> ListServicesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ServiceType](./literals.md#servicetype)
2. See [:material-code-braces: ListServicesOutputTypeDef](./type_defs.md#listservicesoutputtypedef)


```python
# list_services method usage example with argument unpacking

kwargs: ListServicesInputTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_services(**kwargs)
```

1. See [:material-code-braces: ListServicesInputTypeDef](./type_defs.md#listservicesinputtypedef)

### list\_tags\_for\_resource

Lists tags for the specified AWS DevOps Agent resource.

Type annotations and code completion for `#!python session.create_client("devops-agent").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/list_tags_for_resource.html)

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

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)

### list\_webhooks

List all webhooks for given Association.

Type annotations and code completion for `#!python session.create_client("devops-agent").list_webhooks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/list_webhooks.html)

```python
# list_webhooks method definition

await def list_webhooks(
    self,
    *,
    agentSpaceId: str,
    associationId: str,
) -> ListWebhooksOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListWebhooksOutputTypeDef](./type_defs.md#listwebhooksoutputtypedef)


```python
# list_webhooks method usage example with argument unpacking

kwargs: ListWebhooksInputTypeDef = {  # (1)
    "agentSpaceId": ...,
    "associationId": ...,
}

parent.list_webhooks(**kwargs)
```

1. See [:material-code-braces: ListWebhooksInputTypeDef](./type_defs.md#listwebhooksinputtypedef)

### register\_service

This operation registers the specified service.

Type annotations and code completion for `#!python session.create_client("devops-agent").register_service` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/register_service.html)

```python
# register_service method definition

await def register_service(
    self,
    *,
    service: PostRegisterServiceSupportedServiceType,  # (1)
    serviceDetails: ServiceDetailsTypeDef,  # (2)
    kmsKeyArn: str = ...,
    privateConnectionName: str = ...,
    name: str = ...,
    tags: Mapping[str, str] = ...,
) -> RegisterServiceOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: PostRegisterServiceSupportedServiceType](./literals.md#postregisterservicesupportedservicetype)
2. See [:material-code-braces: ServiceDetailsTypeDef](./type_defs.md#servicedetailstypedef)
3. See [:material-code-braces: RegisterServiceOutputTypeDef](./type_defs.md#registerserviceoutputtypedef)


```python
# register_service method usage example with argument unpacking

kwargs: RegisterServiceInputTypeDef = {  # (1)
    "service": ...,
    "serviceDetails": ...,
}

parent.register_service(**kwargs)
```

1. See [:material-code-braces: RegisterServiceInputTypeDef](./type_defs.md#registerserviceinputtypedef)

### send\_message

Sends a chat message and streams the response for the specified agent space
execution.

Type annotations and code completion for `#!python session.create_client("devops-agent").send_message` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/send_message.html)

```python
# send_message method definition

await def send_message(
    self,
    *,
    agentSpaceId: str,
    executionId: str,
    content: str,
    context: SendMessageContextTypeDef = ...,  # (1)
    userId: str = ...,
) -> SendMessageResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SendMessageContextTypeDef](./type_defs.md#sendmessagecontexttypedef)
2. See [:material-code-braces: SendMessageResponseTypeDef](./type_defs.md#sendmessageresponsetypedef)


```python
# send_message method usage example with argument unpacking

kwargs: SendMessageRequestTypeDef = {  # (1)
    "agentSpaceId": ...,
    "executionId": ...,
    "content": ...,
}

parent.send_message(**kwargs)
```

1. See [:material-code-braces: SendMessageRequestTypeDef](./type_defs.md#sendmessagerequesttypedef)

### tag\_resource

Adds or overwrites tags for the specified AWS DevOps Agent resource.

Type annotations and code completion for `#!python session.create_client("devops-agent").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> dict[str, Any]:
    ...
```

```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)

### untag\_resource

Removes tags from the specified AWS DevOps Agent resource.

Type annotations and code completion for `#!python session.create_client("devops-agent").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> dict[str, Any]:
    ...
```

```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)

### update\_agent\_space

Updates the information of an existing AgentSpace.

Type annotations and code completion for `#!python session.create_client("devops-agent").update_agent_space` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/update_agent_space.html)

```python
# update_agent_space method definition

await def update_agent_space(
    self,
    *,
    agentSpaceId: str,
    name: str = ...,
    description: str = ...,
    locale: str = ...,
) -> UpdateAgentSpaceOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateAgentSpaceOutputTypeDef](./type_defs.md#updateagentspaceoutputtypedef)


```python
# update_agent_space method usage example with argument unpacking

kwargs: UpdateAgentSpaceInputTypeDef = {  # (1)
    "agentSpaceId": ...,
}

parent.update_agent_space(**kwargs)
```

1. See [:material-code-braces: UpdateAgentSpaceInputTypeDef](./type_defs.md#updateagentspaceinputtypedef)

### update\_association

Partially updates the configuration of an existing service association for an
AgentSpace.

Type annotations and code completion for `#!python session.create_client("devops-agent").update_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/update_association.html)

```python
# update_association method definition

await def update_association(
    self,
    *,
    agentSpaceId: str,
    associationId: str,
    configuration: ServiceConfigurationUnionTypeDef,  # (1)
) -> UpdateAssociationOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ServiceConfigurationUnionTypeDef](#serviceconfigurationuniontypedef)
2. See [:material-code-braces: UpdateAssociationOutputTypeDef](./type_defs.md#updateassociationoutputtypedef)


```python
# update_association method usage example with argument unpacking

kwargs: UpdateAssociationInputTypeDef = {  # (1)
    "agentSpaceId": ...,
    "associationId": ...,
    "configuration": ...,
}

parent.update_association(**kwargs)
```

1. See [:material-code-braces: UpdateAssociationInputTypeDef](./type_defs.md#updateassociationinputtypedef)

### update\_backlog\_task

Update an existing backlog task.

Type annotations and code completion for `#!python session.create_client("devops-agent").update_backlog_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/update_backlog_task.html)

```python
# update_backlog_task method definition

await def update_backlog_task(
    self,
    *,
    agentSpaceId: str,
    taskId: str,
    taskStatus: TaskStatusType = ...,  # (1)
    clientToken: str = ...,
) -> UpdateBacklogTaskResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype)
2. See [:material-code-braces: UpdateBacklogTaskResponseTypeDef](./type_defs.md#updatebacklogtaskresponsetypedef)


```python
# update_backlog_task method usage example with argument unpacking

kwargs: UpdateBacklogTaskRequestTypeDef = {  # (1)
    "agentSpaceId": ...,
    "taskId": ...,
}

parent.update_backlog_task(**kwargs)
```

1. See [:material-code-braces: UpdateBacklogTaskRequestTypeDef](./type_defs.md#updatebacklogtaskrequesttypedef)

### update\_goal

Update an existing goal.

Type annotations and code completion for `#!python session.create_client("devops-agent").update_goal` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/update_goal.html)

```python
# update_goal method definition

await def update_goal(
    self,
    *,
    agentSpaceId: str,
    goalId: str,
    evaluationSchedule: GoalScheduleInputTypeDef = ...,  # (1)
    clientToken: str = ...,
) -> UpdateGoalResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: GoalScheduleInputTypeDef](./type_defs.md#goalscheduleinputtypedef)
2. See [:material-code-braces: UpdateGoalResponseTypeDef](./type_defs.md#updategoalresponsetypedef)


```python
# update_goal method usage example with argument unpacking

kwargs: UpdateGoalRequestTypeDef = {  # (1)
    "agentSpaceId": ...,
    "goalId": ...,
}

parent.update_goal(**kwargs)
```

1. See [:material-code-braces: UpdateGoalRequestTypeDef](./type_defs.md#updategoalrequesttypedef)

### update\_operator\_app\_idp\_config

Update the external Identity Provider configuration for the Operator App.

Type annotations and code completion for `#!python session.create_client("devops-agent").update_operator_app_idp_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/update_operator_app_idp_config.html)

```python
# update_operator_app_idp_config method definition

await def update_operator_app_idp_config(
    self,
    *,
    agentSpaceId: str,
    idpClientSecret: str = ...,
) -> UpdateOperatorAppIdpConfigOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateOperatorAppIdpConfigOutputTypeDef](./type_defs.md#updateoperatorappidpconfigoutputtypedef)


```python
# update_operator_app_idp_config method usage example with argument unpacking

kwargs: UpdateOperatorAppIdpConfigInputTypeDef = {  # (1)
    "agentSpaceId": ...,
}

parent.update_operator_app_idp_config(**kwargs)
```

1. See [:material-code-braces: UpdateOperatorAppIdpConfigInputTypeDef](./type_defs.md#updateoperatorappidpconfiginputtypedef)

### update\_private\_connection\_certificate

Updates the certificate associated with a Private Connection.

Type annotations and code completion for `#!python session.create_client("devops-agent").update_private_connection_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/update_private_connection_certificate.html)

```python
# update_private_connection_certificate method definition

await def update_private_connection_certificate(
    self,
    *,
    name: str,
    certificate: str,
) -> UpdatePrivateConnectionCertificateOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdatePrivateConnectionCertificateOutputTypeDef](./type_defs.md#updateprivateconnectioncertificateoutputtypedef)


```python
# update_private_connection_certificate method usage example with argument unpacking

kwargs: UpdatePrivateConnectionCertificateInputTypeDef = {  # (1)
    "name": ...,
    "certificate": ...,
}

parent.update_private_connection_certificate(**kwargs)
```

1. See [:material-code-braces: UpdatePrivateConnectionCertificateInputTypeDef](./type_defs.md#updateprivateconnectioncertificateinputtypedef)

### update\_recommendation

Updates an existing recommendation with new content, status, or metadata.

Type annotations and code completion for `#!python session.create_client("devops-agent").update_recommendation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/update_recommendation.html)

```python
# update_recommendation method definition

await def update_recommendation(
    self,
    *,
    agentSpaceId: str,
    recommendationId: str,
    status: RecommendationStatusType = ...,  # (1)
    additionalContext: str = ...,
    clientToken: str = ...,
) -> UpdateRecommendationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RecommendationStatusType](./literals.md#recommendationstatustype)
2. See [:material-code-braces: UpdateRecommendationResponseTypeDef](./type_defs.md#updaterecommendationresponsetypedef)


```python
# update_recommendation method usage example with argument unpacking

kwargs: UpdateRecommendationRequestTypeDef = {  # (1)
    "agentSpaceId": ...,
    "recommendationId": ...,
}

parent.update_recommendation(**kwargs)
```

1. See [:material-code-braces: UpdateRecommendationRequestTypeDef](./type_defs.md#updaterecommendationrequesttypedef)

### validate\_aws\_associations

Validates an aws association and set status and returns a 204 No Content
response on success.

Type annotations and code completion for `#!python session.create_client("devops-agent").validate_aws_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent/client/validate_aws_associations.html)

```python
# validate_aws_associations method definition

await def validate_aws_associations(
    self,
    *,
    agentSpaceId: str,
) -> dict[str, Any]:
    ...
```

```python
# validate_aws_associations method usage example with argument unpacking

kwargs: ValidateAwsAssociationsInputTypeDef = {  # (1)
    "agentSpaceId": ...,
}

parent.validate_aws_associations(**kwargs)
```

1. See [:material-code-braces: ValidateAwsAssociationsInputTypeDef](./type_defs.md#validateawsassociationsinputtypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("devops-agent").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent.html#DevOpsAgentService.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("devops-agent").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent.html#DevOpsAgentService.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: type[BaseException] | None,
    exc_val: BaseException | None,
    exc_tb: types.TracebackType | None,
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("devops-agent").get_paginator` method with overloads.

- `client.get_paginator("list_agent_spaces")` -> [ListAgentSpacesPaginator](./paginators.md#listagentspacespaginator)
- `client.get_paginator("list_associations")` -> [ListAssociationsPaginator](./paginators.md#listassociationspaginator)
- `client.get_paginator("list_backlog_tasks")` -> [ListBacklogTasksPaginator](./paginators.md#listbacklogtaskspaginator)
- `client.get_paginator("list_executions")` -> [ListExecutionsPaginator](./paginators.md#listexecutionspaginator)
- `client.get_paginator("list_goals")` -> [ListGoalsPaginator](./paginators.md#listgoalspaginator)
- `client.get_paginator("list_journal_records")` -> [ListJournalRecordsPaginator](./paginators.md#listjournalrecordspaginator)
- `client.get_paginator("list_services")` -> [ListServicesPaginator](./paginators.md#listservicespaginator)



