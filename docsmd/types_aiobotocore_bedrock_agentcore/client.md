# BedrockAgentCoreClient

> [Index](../README.md) > [BedrockAgentCore](./README.md) > BedrockAgentCoreClient

!!! note ""

    Auto-generated documentation for [BedrockAgentCore](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore.html#bedrockagentcore)
    type annotations stubs module [types-aiobotocore-bedrock-agentcore](https://pypi.org/project/types-aiobotocore-bedrock-agentcore/).

## BedrockAgentCoreClient

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore.html#BedrockAgentCore.Client)

```python
# BedrockAgentCoreClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_bedrock_agentcore.client import BedrockAgentCoreClient

session = get_session()
async with session.create_client("bedrock-agentcore") as client:
    client: BedrockAgentCoreClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("bedrock-agentcore").exceptions` structure.

```python
# BedrockAgentCoreClient.exceptions usage example

async with session.create_client("bedrock-agentcore") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.DuplicateIdException,
        client.InternalServerException,
        client.InvalidInputException,
        client.ResourceNotFoundException,
        client.RuntimeClientError,
        client.ServiceException,
        client.ServiceQuotaExceededException,
        client.ThrottledException,
        client.ThrottlingException,
        client.UnauthorizedException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# BedrockAgentCoreClient usage type checking example

from types_aiobotocore_bedrock_agentcore.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/generate_presigned_url.html)

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


### batch\_create\_memory\_records

Creates multiple memory records in a single batch operation for the specified
memory with custom content.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").batch_create_memory_records` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/batch_create_memory_records.html)

```python
# batch_create_memory_records method definition

await def batch_create_memory_records(
    self,
    *,
    memoryId: str,
    records: Sequence[MemoryRecordCreateInputTypeDef],  # (1)
    clientToken: str = ...,
) -> BatchCreateMemoryRecordsOutputTypeDef:  # (2)
    ...
```

1. See `Sequence[MemoryRecordCreateInputTypeDef]`
2. See [:material-code-braces: BatchCreateMemoryRecordsOutputTypeDef](./type_defs.md#batchcreatememoryrecordsoutputtypedef)


```python
# batch_create_memory_records method usage example with argument unpacking

kwargs: BatchCreateMemoryRecordsInputTypeDef = {  # (1)
    "memoryId": ...,
    "records": ...,
}

parent.batch_create_memory_records(**kwargs)
```

1. See [:material-code-braces: BatchCreateMemoryRecordsInputTypeDef](./type_defs.md#batchcreatememoryrecordsinputtypedef)

### batch\_delete\_memory\_records

Deletes multiple memory records in a single batch operation from the specified
memory.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").batch_delete_memory_records` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/batch_delete_memory_records.html)

```python
# batch_delete_memory_records method definition

await def batch_delete_memory_records(
    self,
    *,
    memoryId: str,
    records: Sequence[MemoryRecordDeleteInputTypeDef],  # (1)
) -> BatchDeleteMemoryRecordsOutputTypeDef:  # (2)
    ...
```

1. See `Sequence[MemoryRecordDeleteInputTypeDef]`
2. See [:material-code-braces: BatchDeleteMemoryRecordsOutputTypeDef](./type_defs.md#batchdeletememoryrecordsoutputtypedef)


```python
# batch_delete_memory_records method usage example with argument unpacking

kwargs: BatchDeleteMemoryRecordsInputTypeDef = {  # (1)
    "memoryId": ...,
    "records": ...,
}

parent.batch_delete_memory_records(**kwargs)
```

1. See [:material-code-braces: BatchDeleteMemoryRecordsInputTypeDef](./type_defs.md#batchdeletememoryrecordsinputtypedef)

### batch\_update\_memory\_records

Updates multiple memory records with custom content in a single batch operation
within the specified memory.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").batch_update_memory_records` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/batch_update_memory_records.html)

```python
# batch_update_memory_records method definition

await def batch_update_memory_records(
    self,
    *,
    memoryId: str,
    records: Sequence[MemoryRecordUpdateInputTypeDef],  # (1)
) -> BatchUpdateMemoryRecordsOutputTypeDef:  # (2)
    ...
```

1. See `Sequence[MemoryRecordUpdateInputTypeDef]`
2. See [:material-code-braces: BatchUpdateMemoryRecordsOutputTypeDef](./type_defs.md#batchupdatememoryrecordsoutputtypedef)


```python
# batch_update_memory_records method usage example with argument unpacking

kwargs: BatchUpdateMemoryRecordsInputTypeDef = {  # (1)
    "memoryId": ...,
    "records": ...,
}

parent.batch_update_memory_records(**kwargs)
```

1. See [:material-code-braces: BatchUpdateMemoryRecordsInputTypeDef](./type_defs.md#batchupdatememoryrecordsinputtypedef)

### complete\_resource\_token\_auth

Confirms the user authentication session for obtaining OAuth2.0 tokens for a
resource.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").complete_resource_token_auth` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/complete_resource_token_auth.html)

```python
# complete_resource_token_auth method definition

await def complete_resource_token_auth(
    self,
    *,
    userIdentifier: UserIdentifierTypeDef,  # (1)
    sessionUri: str,
) -> dict[str, Any]:
    ...
```

1. See [:material-code-braces: UserIdentifierTypeDef](./type_defs.md#useridentifiertypedef)


```python
# complete_resource_token_auth method usage example with argument unpacking

kwargs: CompleteResourceTokenAuthRequestTypeDef = {  # (1)
    "userIdentifier": ...,
    "sessionUri": ...,
}

parent.complete_resource_token_auth(**kwargs)
```

1. See [:material-code-braces: CompleteResourceTokenAuthRequestTypeDef](./type_defs.md#completeresourcetokenauthrequesttypedef)

### create\_event

Creates an event in an AgentCore Memory resource.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").create_event` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/create_event.html)

```python
# create_event method definition

await def create_event(
    self,
    *,
    memoryId: str,
    actorId: str,
    eventTimestamp: TimestampTypeDef,
    payload: Sequence[PayloadTypeUnionTypeDef],  # (1)
    sessionId: str = ...,
    branch: BranchTypeDef = ...,  # (2)
    clientToken: str = ...,
    metadata: Mapping[str, MetadataValueTypeDef] = ...,  # (3)
) -> CreateEventOutputTypeDef:  # (4)
    ...
```

1. See `Sequence[PayloadTypeUnionTypeDef]`
2. See [:material-code-braces: BranchTypeDef](./type_defs.md#branchtypedef)
3. See `Mapping[str, MetadataValueTypeDef]`
4. See [:material-code-braces: CreateEventOutputTypeDef](./type_defs.md#createeventoutputtypedef)


```python
# create_event method usage example with argument unpacking

kwargs: CreateEventInputTypeDef = {  # (1)
    "memoryId": ...,
    "actorId": ...,
    "eventTimestamp": ...,
    "payload": ...,
}

parent.create_event(**kwargs)
```

1. See [:material-code-braces: CreateEventInputTypeDef](./type_defs.md#createeventinputtypedef)

### delete\_event

Deletes an event from an AgentCore Memory resource.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").delete_event` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/delete_event.html)

```python
# delete_event method definition

await def delete_event(
    self,
    *,
    memoryId: str,
    sessionId: str,
    eventId: str,
    actorId: str,
) -> DeleteEventOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteEventOutputTypeDef](./type_defs.md#deleteeventoutputtypedef)


```python
# delete_event method usage example with argument unpacking

kwargs: DeleteEventInputTypeDef = {  # (1)
    "memoryId": ...,
    "sessionId": ...,
    "eventId": ...,
    "actorId": ...,
}

parent.delete_event(**kwargs)
```

1. See [:material-code-braces: DeleteEventInputTypeDef](./type_defs.md#deleteeventinputtypedef)

### delete\_memory\_record

Deletes a memory record from an AgentCore Memory resource.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").delete_memory_record` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/delete_memory_record.html)

```python
# delete_memory_record method definition

await def delete_memory_record(
    self,
    *,
    memoryId: str,
    memoryRecordId: str,
) -> DeleteMemoryRecordOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteMemoryRecordOutputTypeDef](./type_defs.md#deletememoryrecordoutputtypedef)


```python
# delete_memory_record method usage example with argument unpacking

kwargs: DeleteMemoryRecordInputTypeDef = {  # (1)
    "memoryId": ...,
    "memoryRecordId": ...,
}

parent.delete_memory_record(**kwargs)
```

1. See [:material-code-braces: DeleteMemoryRecordInputTypeDef](./type_defs.md#deletememoryrecordinputtypedef)

### evaluate

Performs on-demand evaluation of agent traces using a specified evaluator.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").evaluate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/evaluate.html)

```python
# evaluate method definition

await def evaluate(
    self,
    *,
    evaluatorId: str,
    evaluationInput: EvaluationInputTypeDef,  # (1)
    evaluationTarget: EvaluationTargetTypeDef = ...,  # (2)
) -> EvaluateResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: EvaluationInputTypeDef](./type_defs.md#evaluationinputtypedef)
2. See [:material-code-braces: EvaluationTargetTypeDef](./type_defs.md#evaluationtargettypedef)
3. See [:material-code-braces: EvaluateResponseTypeDef](./type_defs.md#evaluateresponsetypedef)


```python
# evaluate method usage example with argument unpacking

kwargs: EvaluateRequestTypeDef = {  # (1)
    "evaluatorId": ...,
    "evaluationInput": ...,
}

parent.evaluate(**kwargs)
```

1. See [:material-code-braces: EvaluateRequestTypeDef](./type_defs.md#evaluaterequesttypedef)

### get\_agent\_card

Retrieves the A2A agent card associated with an AgentCore Runtime agent.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").get_agent_card` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/get_agent_card.html)

```python
# get_agent_card method definition

await def get_agent_card(
    self,
    *,
    agentRuntimeArn: str,
    runtimeSessionId: str = ...,
    qualifier: str = ...,
) -> GetAgentCardResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAgentCardResponseTypeDef](./type_defs.md#getagentcardresponsetypedef)


```python
# get_agent_card method usage example with argument unpacking

kwargs: GetAgentCardRequestTypeDef = {  # (1)
    "agentRuntimeArn": ...,
}

parent.get_agent_card(**kwargs)
```

1. See [:material-code-braces: GetAgentCardRequestTypeDef](./type_defs.md#getagentcardrequesttypedef)

### get\_browser\_session

Retrieves detailed information about a specific browser session in Amazon
Bedrock.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").get_browser_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/get_browser_session.html)

```python
# get_browser_session method definition

await def get_browser_session(
    self,
    *,
    browserIdentifier: str,
    sessionId: str,
) -> GetBrowserSessionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetBrowserSessionResponseTypeDef](./type_defs.md#getbrowsersessionresponsetypedef)


```python
# get_browser_session method usage example with argument unpacking

kwargs: GetBrowserSessionRequestTypeDef = {  # (1)
    "browserIdentifier": ...,
    "sessionId": ...,
}

parent.get_browser_session(**kwargs)
```

1. See [:material-code-braces: GetBrowserSessionRequestTypeDef](./type_defs.md#getbrowsersessionrequesttypedef)

### get\_code\_interpreter\_session

Retrieves detailed information about a specific code interpreter session in
Amazon Bedrock.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").get_code_interpreter_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/get_code_interpreter_session.html)

```python
# get_code_interpreter_session method definition

await def get_code_interpreter_session(
    self,
    *,
    codeInterpreterIdentifier: str,
    sessionId: str,
) -> GetCodeInterpreterSessionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCodeInterpreterSessionResponseTypeDef](./type_defs.md#getcodeinterpretersessionresponsetypedef)


```python
# get_code_interpreter_session method usage example with argument unpacking

kwargs: GetCodeInterpreterSessionRequestTypeDef = {  # (1)
    "codeInterpreterIdentifier": ...,
    "sessionId": ...,
}

parent.get_code_interpreter_session(**kwargs)
```

1. See [:material-code-braces: GetCodeInterpreterSessionRequestTypeDef](./type_defs.md#getcodeinterpretersessionrequesttypedef)

### get\_event

Retrieves information about a specific event in an AgentCore Memory resource.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").get_event` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/get_event.html)

```python
# get_event method definition

await def get_event(
    self,
    *,
    memoryId: str,
    sessionId: str,
    actorId: str,
    eventId: str,
) -> GetEventOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEventOutputTypeDef](./type_defs.md#geteventoutputtypedef)


```python
# get_event method usage example with argument unpacking

kwargs: GetEventInputTypeDef = {  # (1)
    "memoryId": ...,
    "sessionId": ...,
    "actorId": ...,
    "eventId": ...,
}

parent.get_event(**kwargs)
```

1. See [:material-code-braces: GetEventInputTypeDef](./type_defs.md#geteventinputtypedef)

### get\_memory\_record

Retrieves a specific memory record from an AgentCore Memory resource.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").get_memory_record` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/get_memory_record.html)

```python
# get_memory_record method definition

await def get_memory_record(
    self,
    *,
    memoryId: str,
    memoryRecordId: str,
) -> GetMemoryRecordOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMemoryRecordOutputTypeDef](./type_defs.md#getmemoryrecordoutputtypedef)


```python
# get_memory_record method usage example with argument unpacking

kwargs: GetMemoryRecordInputTypeDef = {  # (1)
    "memoryId": ...,
    "memoryRecordId": ...,
}

parent.get_memory_record(**kwargs)
```

1. See [:material-code-braces: GetMemoryRecordInputTypeDef](./type_defs.md#getmemoryrecordinputtypedef)

### get\_resource\_api\_key

Retrieves the API key associated with an API key credential provider.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").get_resource_api_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/get_resource_api_key.html)

```python
# get_resource_api_key method definition

await def get_resource_api_key(
    self,
    *,
    workloadIdentityToken: str,
    resourceCredentialProviderName: str,
) -> GetResourceApiKeyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResourceApiKeyResponseTypeDef](./type_defs.md#getresourceapikeyresponsetypedef)


```python
# get_resource_api_key method usage example with argument unpacking

kwargs: GetResourceApiKeyRequestTypeDef = {  # (1)
    "workloadIdentityToken": ...,
    "resourceCredentialProviderName": ...,
}

parent.get_resource_api_key(**kwargs)
```

1. See [:material-code-braces: GetResourceApiKeyRequestTypeDef](./type_defs.md#getresourceapikeyrequesttypedef)

### get\_resource\_oauth2\_token

Returns the OAuth 2.0 token of the provided resource.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").get_resource_oauth2_token` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/get_resource_oauth2_token.html)

```python
# get_resource_oauth2_token method definition

await def get_resource_oauth2_token(
    self,
    *,
    workloadIdentityToken: str,
    resourceCredentialProviderName: str,
    scopes: Sequence[str],
    oauth2Flow: Oauth2FlowTypeType,  # (1)
    sessionUri: str = ...,
    resourceOauth2ReturnUrl: str = ...,
    forceAuthentication: bool = ...,
    customParameters: Mapping[str, str] = ...,
    customState: str = ...,
) -> GetResourceOauth2TokenResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: Oauth2FlowTypeType](./literals.md#oauth2flowtypetype)
2. See [:material-code-braces: GetResourceOauth2TokenResponseTypeDef](./type_defs.md#getresourceoauth2tokenresponsetypedef)


```python
# get_resource_oauth2_token method usage example with argument unpacking

kwargs: GetResourceOauth2TokenRequestTypeDef = {  # (1)
    "workloadIdentityToken": ...,
    "resourceCredentialProviderName": ...,
    "scopes": ...,
    "oauth2Flow": ...,
}

parent.get_resource_oauth2_token(**kwargs)
```

1. See [:material-code-braces: GetResourceOauth2TokenRequestTypeDef](./type_defs.md#getresourceoauth2tokenrequesttypedef)

### get\_workload\_access\_token

Obtains a workload access token for agentic workloads not acting on behalf of a
user.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").get_workload_access_token` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/get_workload_access_token.html)

```python
# get_workload_access_token method definition

await def get_workload_access_token(
    self,
    *,
    workloadName: str,
) -> GetWorkloadAccessTokenResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWorkloadAccessTokenResponseTypeDef](./type_defs.md#getworkloadaccesstokenresponsetypedef)


```python
# get_workload_access_token method usage example with argument unpacking

kwargs: GetWorkloadAccessTokenRequestTypeDef = {  # (1)
    "workloadName": ...,
}

parent.get_workload_access_token(**kwargs)
```

1. See [:material-code-braces: GetWorkloadAccessTokenRequestTypeDef](./type_defs.md#getworkloadaccesstokenrequesttypedef)

### get\_workload\_access\_token\_for\_jwt

Obtains a workload access token for agentic workloads acting on behalf of a
user, using a JWT token.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").get_workload_access_token_for_jwt` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/get_workload_access_token_for_jwt.html)

```python
# get_workload_access_token_for_jwt method definition

await def get_workload_access_token_for_jwt(
    self,
    *,
    workloadName: str,
    userToken: str,
) -> GetWorkloadAccessTokenForJWTResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWorkloadAccessTokenForJWTResponseTypeDef](./type_defs.md#getworkloadaccesstokenforjwtresponsetypedef)


```python
# get_workload_access_token_for_jwt method usage example with argument unpacking

kwargs: GetWorkloadAccessTokenForJWTRequestTypeDef = {  # (1)
    "workloadName": ...,
    "userToken": ...,
}

parent.get_workload_access_token_for_jwt(**kwargs)
```

1. See [:material-code-braces: GetWorkloadAccessTokenForJWTRequestTypeDef](./type_defs.md#getworkloadaccesstokenforjwtrequesttypedef)

### get\_workload\_access\_token\_for\_user\_id

Obtains a workload access token for agentic workloads acting on behalf of a
user, using the user's ID.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").get_workload_access_token_for_user_id` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/get_workload_access_token_for_user_id.html)

```python
# get_workload_access_token_for_user_id method definition

await def get_workload_access_token_for_user_id(
    self,
    *,
    workloadName: str,
    userId: str,
) -> GetWorkloadAccessTokenForUserIdResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWorkloadAccessTokenForUserIdResponseTypeDef](./type_defs.md#getworkloadaccesstokenforuseridresponsetypedef)


```python
# get_workload_access_token_for_user_id method usage example with argument unpacking

kwargs: GetWorkloadAccessTokenForUserIdRequestTypeDef = {  # (1)
    "workloadName": ...,
    "userId": ...,
}

parent.get_workload_access_token_for_user_id(**kwargs)
```

1. See [:material-code-braces: GetWorkloadAccessTokenForUserIdRequestTypeDef](./type_defs.md#getworkloadaccesstokenforuseridrequesttypedef)

### invoke\_agent\_runtime

Sends a request to an agent or tool hosted in an Amazon Bedrock AgentCore
Runtime and receives responses in real-time.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").invoke_agent_runtime` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/invoke_agent_runtime.html)

```python
# invoke_agent_runtime method definition

await def invoke_agent_runtime(
    self,
    *,
    agentRuntimeArn: str,
    payload: BlobTypeDef,
    contentType: str = ...,
    accept: str = ...,
    mcpSessionId: str = ...,
    runtimeSessionId: str = ...,
    mcpProtocolVersion: str = ...,
    runtimeUserId: str = ...,
    traceId: str = ...,
    traceParent: str = ...,
    traceState: str = ...,
    baggage: str = ...,
    qualifier: str = ...,
    accountId: str = ...,
) -> InvokeAgentRuntimeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: InvokeAgentRuntimeResponseTypeDef](./type_defs.md#invokeagentruntimeresponsetypedef)


```python
# invoke_agent_runtime method usage example with argument unpacking

kwargs: InvokeAgentRuntimeRequestTypeDef = {  # (1)
    "agentRuntimeArn": ...,
    "payload": ...,
}

parent.invoke_agent_runtime(**kwargs)
```

1. See [:material-code-braces: InvokeAgentRuntimeRequestTypeDef](./type_defs.md#invokeagentruntimerequesttypedef)

### invoke\_code\_interpreter

Executes code within an active code interpreter session in Amazon Bedrock.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").invoke_code_interpreter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/invoke_code_interpreter.html)

```python
# invoke_code_interpreter method definition

await def invoke_code_interpreter(
    self,
    *,
    codeInterpreterIdentifier: str,
    name: ToolNameType,  # (1)
    sessionId: str = ...,
    traceId: str = ...,
    traceParent: str = ...,
    arguments: ToolArgumentsTypeDef = ...,  # (2)
) -> InvokeCodeInterpreterResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ToolNameType](./literals.md#toolnametype)
2. See [:material-code-braces: ToolArgumentsTypeDef](./type_defs.md#toolargumentstypedef)
3. See [:material-code-braces: InvokeCodeInterpreterResponseTypeDef](./type_defs.md#invokecodeinterpreterresponsetypedef)


```python
# invoke_code_interpreter method usage example with argument unpacking

kwargs: InvokeCodeInterpreterRequestTypeDef = {  # (1)
    "codeInterpreterIdentifier": ...,
    "name": ...,
}

parent.invoke_code_interpreter(**kwargs)
```

1. See [:material-code-braces: InvokeCodeInterpreterRequestTypeDef](./type_defs.md#invokecodeinterpreterrequesttypedef)

### list\_actors

Lists all actors in an AgentCore Memory resource.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").list_actors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/list_actors.html)

```python
# list_actors method definition

await def list_actors(
    self,
    *,
    memoryId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListActorsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListActorsOutputTypeDef](./type_defs.md#listactorsoutputtypedef)


```python
# list_actors method usage example with argument unpacking

kwargs: ListActorsInputTypeDef = {  # (1)
    "memoryId": ...,
}

parent.list_actors(**kwargs)
```

1. See [:material-code-braces: ListActorsInputTypeDef](./type_defs.md#listactorsinputtypedef)

### list\_browser\_sessions

Retrieves a list of browser sessions in Amazon Bedrock that match the specified
criteria.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").list_browser_sessions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/list_browser_sessions.html)

```python
# list_browser_sessions method definition

await def list_browser_sessions(
    self,
    *,
    browserIdentifier: str,
    maxResults: int = ...,
    nextToken: str = ...,
    status: BrowserSessionStatusType = ...,  # (1)
) -> ListBrowserSessionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: BrowserSessionStatusType](./literals.md#browsersessionstatustype)
2. See [:material-code-braces: ListBrowserSessionsResponseTypeDef](./type_defs.md#listbrowsersessionsresponsetypedef)


```python
# list_browser_sessions method usage example with argument unpacking

kwargs: ListBrowserSessionsRequestTypeDef = {  # (1)
    "browserIdentifier": ...,
}

parent.list_browser_sessions(**kwargs)
```

1. See [:material-code-braces: ListBrowserSessionsRequestTypeDef](./type_defs.md#listbrowsersessionsrequesttypedef)

### list\_code\_interpreter\_sessions

Retrieves a list of code interpreter sessions in Amazon Bedrock that match the
specified criteria.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").list_code_interpreter_sessions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/list_code_interpreter_sessions.html)

```python
# list_code_interpreter_sessions method definition

await def list_code_interpreter_sessions(
    self,
    *,
    codeInterpreterIdentifier: str,
    maxResults: int = ...,
    nextToken: str = ...,
    status: CodeInterpreterSessionStatusType = ...,  # (1)
) -> ListCodeInterpreterSessionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: CodeInterpreterSessionStatusType](./literals.md#codeinterpretersessionstatustype)
2. See [:material-code-braces: ListCodeInterpreterSessionsResponseTypeDef](./type_defs.md#listcodeinterpretersessionsresponsetypedef)


```python
# list_code_interpreter_sessions method usage example with argument unpacking

kwargs: ListCodeInterpreterSessionsRequestTypeDef = {  # (1)
    "codeInterpreterIdentifier": ...,
}

parent.list_code_interpreter_sessions(**kwargs)
```

1. See [:material-code-braces: ListCodeInterpreterSessionsRequestTypeDef](./type_defs.md#listcodeinterpretersessionsrequesttypedef)

### list\_events

Lists events in an AgentCore Memory resource based on specified criteria.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").list_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/list_events.html)

```python
# list_events method definition

await def list_events(
    self,
    *,
    memoryId: str,
    sessionId: str,
    actorId: str,
    includePayloads: bool = ...,
    filter: FilterInputTypeDef = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListEventsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterInputTypeDef](./type_defs.md#filterinputtypedef)
2. See [:material-code-braces: ListEventsOutputTypeDef](./type_defs.md#listeventsoutputtypedef)


```python
# list_events method usage example with argument unpacking

kwargs: ListEventsInputTypeDef = {  # (1)
    "memoryId": ...,
    "sessionId": ...,
    "actorId": ...,
}

parent.list_events(**kwargs)
```

1. See [:material-code-braces: ListEventsInputTypeDef](./type_defs.md#listeventsinputtypedef)

### list\_memory\_extraction\_jobs

Lists all long-term memory extraction jobs that are eligible to be started with
optional filtering.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").list_memory_extraction_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/list_memory_extraction_jobs.html)

```python
# list_memory_extraction_jobs method definition

await def list_memory_extraction_jobs(
    self,
    *,
    memoryId: str,
    maxResults: int = ...,
    filter: ExtractionJobFilterInputTypeDef = ...,  # (1)
    nextToken: str = ...,
) -> ListMemoryExtractionJobsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ExtractionJobFilterInputTypeDef](./type_defs.md#extractionjobfilterinputtypedef)
2. See [:material-code-braces: ListMemoryExtractionJobsOutputTypeDef](./type_defs.md#listmemoryextractionjobsoutputtypedef)


```python
# list_memory_extraction_jobs method usage example with argument unpacking

kwargs: ListMemoryExtractionJobsInputTypeDef = {  # (1)
    "memoryId": ...,
}

parent.list_memory_extraction_jobs(**kwargs)
```

1. See [:material-code-braces: ListMemoryExtractionJobsInputTypeDef](./type_defs.md#listmemoryextractionjobsinputtypedef)

### list\_memory\_records

Lists memory records in an AgentCore Memory resource based on specified
criteria.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").list_memory_records` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/list_memory_records.html)

```python
# list_memory_records method definition

await def list_memory_records(
    self,
    *,
    memoryId: str,
    namespace: str,
    memoryStrategyId: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListMemoryRecordsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMemoryRecordsOutputTypeDef](./type_defs.md#listmemoryrecordsoutputtypedef)


```python
# list_memory_records method usage example with argument unpacking

kwargs: ListMemoryRecordsInputTypeDef = {  # (1)
    "memoryId": ...,
    "namespace": ...,
}

parent.list_memory_records(**kwargs)
```

1. See [:material-code-braces: ListMemoryRecordsInputTypeDef](./type_defs.md#listmemoryrecordsinputtypedef)

### list\_sessions

Lists sessions in an AgentCore Memory resource based on specified criteria.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").list_sessions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/list_sessions.html)

```python
# list_sessions method definition

await def list_sessions(
    self,
    *,
    memoryId: str,
    actorId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListSessionsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSessionsOutputTypeDef](./type_defs.md#listsessionsoutputtypedef)


```python
# list_sessions method usage example with argument unpacking

kwargs: ListSessionsInputTypeDef = {  # (1)
    "memoryId": ...,
    "actorId": ...,
}

parent.list_sessions(**kwargs)
```

1. See [:material-code-braces: ListSessionsInputTypeDef](./type_defs.md#listsessionsinputtypedef)

### retrieve\_memory\_records

Searches for and retrieves memory records from an AgentCore Memory resource
based on specified search criteria.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").retrieve_memory_records` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/retrieve_memory_records.html)

```python
# retrieve_memory_records method definition

await def retrieve_memory_records(
    self,
    *,
    memoryId: str,
    namespace: str,
    searchCriteria: SearchCriteriaTypeDef,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> RetrieveMemoryRecordsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SearchCriteriaTypeDef](./type_defs.md#searchcriteriatypedef)
2. See [:material-code-braces: RetrieveMemoryRecordsOutputTypeDef](./type_defs.md#retrievememoryrecordsoutputtypedef)


```python
# retrieve_memory_records method usage example with argument unpacking

kwargs: RetrieveMemoryRecordsInputTypeDef = {  # (1)
    "memoryId": ...,
    "namespace": ...,
    "searchCriteria": ...,
}

parent.retrieve_memory_records(**kwargs)
```

1. See [:material-code-braces: RetrieveMemoryRecordsInputTypeDef](./type_defs.md#retrievememoryrecordsinputtypedef)

### start\_browser\_session

Creates and initializes a browser session in Amazon Bedrock.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").start_browser_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/start_browser_session.html)

```python
# start_browser_session method definition

await def start_browser_session(
    self,
    *,
    browserIdentifier: str,
    traceId: str = ...,
    traceParent: str = ...,
    name: str = ...,
    sessionTimeoutSeconds: int = ...,
    viewPort: ViewPortTypeDef = ...,  # (1)
    clientToken: str = ...,
) -> StartBrowserSessionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ViewPortTypeDef](./type_defs.md#viewporttypedef)
2. See [:material-code-braces: StartBrowserSessionResponseTypeDef](./type_defs.md#startbrowsersessionresponsetypedef)


```python
# start_browser_session method usage example with argument unpacking

kwargs: StartBrowserSessionRequestTypeDef = {  # (1)
    "browserIdentifier": ...,
}

parent.start_browser_session(**kwargs)
```

1. See [:material-code-braces: StartBrowserSessionRequestTypeDef](./type_defs.md#startbrowsersessionrequesttypedef)

### start\_code\_interpreter\_session

Creates and initializes a code interpreter session in Amazon Bedrock.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").start_code_interpreter_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/start_code_interpreter_session.html)

```python
# start_code_interpreter_session method definition

await def start_code_interpreter_session(
    self,
    *,
    codeInterpreterIdentifier: str,
    traceId: str = ...,
    traceParent: str = ...,
    name: str = ...,
    sessionTimeoutSeconds: int = ...,
    clientToken: str = ...,
) -> StartCodeInterpreterSessionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartCodeInterpreterSessionResponseTypeDef](./type_defs.md#startcodeinterpretersessionresponsetypedef)


```python
# start_code_interpreter_session method usage example with argument unpacking

kwargs: StartCodeInterpreterSessionRequestTypeDef = {  # (1)
    "codeInterpreterIdentifier": ...,
}

parent.start_code_interpreter_session(**kwargs)
```

1. See [:material-code-braces: StartCodeInterpreterSessionRequestTypeDef](./type_defs.md#startcodeinterpretersessionrequesttypedef)

### start\_memory\_extraction\_job

Starts a memory extraction job that processes events that failed extraction
previously in an AgentCore Memory resource and produces structured memory
records.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").start_memory_extraction_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/start_memory_extraction_job.html)

```python
# start_memory_extraction_job method definition

await def start_memory_extraction_job(
    self,
    *,
    memoryId: str,
    extractionJob: ExtractionJobTypeDef,  # (1)
    clientToken: str = ...,
) -> StartMemoryExtractionJobOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ExtractionJobTypeDef](./type_defs.md#extractionjobtypedef)
2. See [:material-code-braces: StartMemoryExtractionJobOutputTypeDef](./type_defs.md#startmemoryextractionjoboutputtypedef)


```python
# start_memory_extraction_job method usage example with argument unpacking

kwargs: StartMemoryExtractionJobInputTypeDef = {  # (1)
    "memoryId": ...,
    "extractionJob": ...,
}

parent.start_memory_extraction_job(**kwargs)
```

1. See [:material-code-braces: StartMemoryExtractionJobInputTypeDef](./type_defs.md#startmemoryextractionjobinputtypedef)

### stop\_browser\_session

Terminates an active browser session in Amazon Bedrock.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").stop_browser_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/stop_browser_session.html)

```python
# stop_browser_session method definition

await def stop_browser_session(
    self,
    *,
    browserIdentifier: str,
    sessionId: str,
    traceId: str = ...,
    traceParent: str = ...,
    clientToken: str = ...,
) -> StopBrowserSessionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopBrowserSessionResponseTypeDef](./type_defs.md#stopbrowsersessionresponsetypedef)


```python
# stop_browser_session method usage example with argument unpacking

kwargs: StopBrowserSessionRequestTypeDef = {  # (1)
    "browserIdentifier": ...,
    "sessionId": ...,
}

parent.stop_browser_session(**kwargs)
```

1. See [:material-code-braces: StopBrowserSessionRequestTypeDef](./type_defs.md#stopbrowsersessionrequesttypedef)

### stop\_code\_interpreter\_session

Terminates an active code interpreter session in Amazon Bedrock.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").stop_code_interpreter_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/stop_code_interpreter_session.html)

```python
# stop_code_interpreter_session method definition

await def stop_code_interpreter_session(
    self,
    *,
    codeInterpreterIdentifier: str,
    sessionId: str,
    traceId: str = ...,
    traceParent: str = ...,
    clientToken: str = ...,
) -> StopCodeInterpreterSessionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopCodeInterpreterSessionResponseTypeDef](./type_defs.md#stopcodeinterpretersessionresponsetypedef)


```python
# stop_code_interpreter_session method usage example with argument unpacking

kwargs: StopCodeInterpreterSessionRequestTypeDef = {  # (1)
    "codeInterpreterIdentifier": ...,
    "sessionId": ...,
}

parent.stop_code_interpreter_session(**kwargs)
```

1. See [:material-code-braces: StopCodeInterpreterSessionRequestTypeDef](./type_defs.md#stopcodeinterpretersessionrequesttypedef)

### stop\_runtime\_session

Stops a session that is running in an running AgentCore Runtime agent.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").stop_runtime_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/stop_runtime_session.html)

```python
# stop_runtime_session method definition

await def stop_runtime_session(
    self,
    *,
    runtimeSessionId: str,
    agentRuntimeArn: str,
    qualifier: str = ...,
    clientToken: str = ...,
) -> StopRuntimeSessionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopRuntimeSessionResponseTypeDef](./type_defs.md#stopruntimesessionresponsetypedef)


```python
# stop_runtime_session method usage example with argument unpacking

kwargs: StopRuntimeSessionRequestTypeDef = {  # (1)
    "runtimeSessionId": ...,
    "agentRuntimeArn": ...,
}

parent.stop_runtime_session(**kwargs)
```

1. See [:material-code-braces: StopRuntimeSessionRequestTypeDef](./type_defs.md#stopruntimesessionrequesttypedef)

### update\_browser\_stream

Updates a browser stream.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").update_browser_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore/client/update_browser_stream.html)

```python
# update_browser_stream method definition

await def update_browser_stream(
    self,
    *,
    browserIdentifier: str,
    sessionId: str,
    streamUpdate: StreamUpdateTypeDef,  # (1)
    clientToken: str = ...,
) -> UpdateBrowserStreamResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: StreamUpdateTypeDef](./type_defs.md#streamupdatetypedef)
2. See [:material-code-braces: UpdateBrowserStreamResponseTypeDef](./type_defs.md#updatebrowserstreamresponsetypedef)


```python
# update_browser_stream method usage example with argument unpacking

kwargs: UpdateBrowserStreamRequestTypeDef = {  # (1)
    "browserIdentifier": ...,
    "sessionId": ...,
    "streamUpdate": ...,
}

parent.update_browser_stream(**kwargs)
```

1. See [:material-code-braces: UpdateBrowserStreamRequestTypeDef](./type_defs.md#updatebrowserstreamrequesttypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore.html#BedrockAgentCore.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore.html#BedrockAgentCore.Client)

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

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore").get_paginator` method with overloads.

- `client.get_paginator("list_actors")` -> [ListActorsPaginator](./paginators.md#listactorspaginator)
- `client.get_paginator("list_events")` -> [ListEventsPaginator](./paginators.md#listeventspaginator)
- `client.get_paginator("list_memory_extraction_jobs")` -> [ListMemoryExtractionJobsPaginator](./paginators.md#listmemoryextractionjobspaginator)
- `client.get_paginator("list_memory_records")` -> [ListMemoryRecordsPaginator](./paginators.md#listmemoryrecordspaginator)
- `client.get_paginator("list_sessions")` -> [ListSessionsPaginator](./paginators.md#listsessionspaginator)
- `client.get_paginator("retrieve_memory_records")` -> [RetrieveMemoryRecordsPaginator](./paginators.md#retrievememoryrecordspaginator)



