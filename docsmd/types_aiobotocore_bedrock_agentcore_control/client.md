# BedrockAgentCoreControlPlaneFrontingLayerClient

> [Index](../README.md) > [BedrockAgentCoreControlPlaneFrontingLayer](./README.md) > BedrockAgentCoreControlPlaneFrontingLayerClient

!!! note ""

    Auto-generated documentation for [BedrockAgentCoreControlPlaneFrontingLayer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control.html#bedrockagentcorecontrolplanefrontinglayer)
    type annotations stubs module [types-aiobotocore-bedrock-agentcore-control](https://pypi.org/project/types-aiobotocore-bedrock-agentcore-control/).

## BedrockAgentCoreControlPlaneFrontingLayerClient

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control.html#BedrockAgentCoreControlPlaneFrontingLayer.Client)

```python
# BedrockAgentCoreControlPlaneFrontingLayerClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_bedrock_agentcore_control.client import BedrockAgentCoreControlPlaneFrontingLayerClient

session = get_session()
async with session.create_client("bedrock-agentcore-control") as client:
    client: BedrockAgentCoreControlPlaneFrontingLayerClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("bedrock-agentcore-control").exceptions` structure.

```python
# BedrockAgentCoreControlPlaneFrontingLayerClient.exceptions usage example

async with session.create_client("bedrock-agentcore-control") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConcurrentModificationException,
        client.ConflictException,
        client.DecryptionFailure,
        client.EncryptionFailure,
        client.InternalServerException,
        client.ResourceLimitExceededException,
        client.ResourceNotFoundException,
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
# BedrockAgentCoreControlPlaneFrontingLayerClient usage type checking example

from types_aiobotocore_bedrock_agentcore_control.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/generate_presigned_url.html)

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


### create\_agent\_runtime

Creates an Amazon Secure Agent.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").create_agent_runtime` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/create_agent_runtime.html)

```python
# create_agent_runtime method definition

await def create_agent_runtime(
    self,
    *,
    agentRuntimeName: str,
    agentRuntimeArtifact: AgentArtifactTypeDef,  # (1)
    roleArn: str,
    networkConfiguration: NetworkConfigurationTypeDef,  # (2)
    description: str = ...,
    protocolConfiguration: ProtocolConfigurationTypeDef = ...,  # (3)
    clientToken: str = ...,
    environmentVariables: Mapping[str, str] = ...,
    authorizerConfiguration: AuthorizerConfigurationUnionTypeDef = ...,  # (4)
) -> CreateAgentRuntimeResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: AgentArtifactTypeDef](./type_defs.md#agentartifacttypedef)
2. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef)
3. See [:material-code-braces: ProtocolConfigurationTypeDef](./type_defs.md#protocolconfigurationtypedef)
4. See [:material-code-braces: AuthorizerConfigurationUnionTypeDef](#authorizerconfigurationuniontypedef)
5. See [:material-code-braces: CreateAgentRuntimeResponseTypeDef](./type_defs.md#createagentruntimeresponsetypedef)


```python
# create_agent_runtime method usage example with argument unpacking

kwargs: CreateAgentRuntimeRequestTypeDef = {  # (1)
    "agentRuntimeName": ...,
    "agentRuntimeArtifact": ...,
    "roleArn": ...,
    "networkConfiguration": ...,
}

parent.create_agent_runtime(**kwargs)
```

1. See [:material-code-braces: CreateAgentRuntimeRequestTypeDef](./type_defs.md#createagentruntimerequesttypedef)

### create\_agent\_runtime\_endpoint

Creates an Amazon Secure AgentEndpoint.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").create_agent_runtime_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/create_agent_runtime_endpoint.html)

```python
# create_agent_runtime_endpoint method definition

await def create_agent_runtime_endpoint(
    self,
    *,
    agentRuntimeId: str,
    name: str,
    agentRuntimeVersion: str = ...,
    description: str = ...,
    clientToken: str = ...,
) -> CreateAgentRuntimeEndpointResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateAgentRuntimeEndpointResponseTypeDef](./type_defs.md#createagentruntimeendpointresponsetypedef)


```python
# create_agent_runtime_endpoint method usage example with argument unpacking

kwargs: CreateAgentRuntimeEndpointRequestTypeDef = {  # (1)
    "agentRuntimeId": ...,
    "name": ...,
}

parent.create_agent_runtime_endpoint(**kwargs)
```

1. See [:material-code-braces: CreateAgentRuntimeEndpointRequestTypeDef](./type_defs.md#createagentruntimeendpointrequesttypedef)

### create\_api\_key\_credential\_provider

Creates a new API key credential provider.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").create_api_key_credential_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/create_api_key_credential_provider.html)

```python
# create_api_key_credential_provider method definition

await def create_api_key_credential_provider(
    self,
    *,
    name: str,
    apiKey: str,
) -> CreateApiKeyCredentialProviderResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateApiKeyCredentialProviderResponseTypeDef](./type_defs.md#createapikeycredentialproviderresponsetypedef)


```python
# create_api_key_credential_provider method usage example with argument unpacking

kwargs: CreateApiKeyCredentialProviderRequestTypeDef = {  # (1)
    "name": ...,
    "apiKey": ...,
}

parent.create_api_key_credential_provider(**kwargs)
```

1. See [:material-code-braces: CreateApiKeyCredentialProviderRequestTypeDef](./type_defs.md#createapikeycredentialproviderrequesttypedef)

### create\_browser

Creates a custom browser.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").create_browser` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/create_browser.html)

```python
# create_browser method definition

await def create_browser(
    self,
    *,
    name: str,
    networkConfiguration: BrowserNetworkConfigurationTypeDef,  # (1)
    description: str = ...,
    executionRoleArn: str = ...,
    recording: RecordingConfigTypeDef = ...,  # (2)
    clientToken: str = ...,
) -> CreateBrowserResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: BrowserNetworkConfigurationTypeDef](./type_defs.md#browsernetworkconfigurationtypedef)
2. See [:material-code-braces: RecordingConfigTypeDef](./type_defs.md#recordingconfigtypedef)
3. See [:material-code-braces: CreateBrowserResponseTypeDef](./type_defs.md#createbrowserresponsetypedef)


```python
# create_browser method usage example with argument unpacking

kwargs: CreateBrowserRequestTypeDef = {  # (1)
    "name": ...,
    "networkConfiguration": ...,
}

parent.create_browser(**kwargs)
```

1. See [:material-code-braces: CreateBrowserRequestTypeDef](./type_defs.md#createbrowserrequesttypedef)

### create\_code\_interpreter

Creates a custom code interpreter.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").create_code_interpreter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/create_code_interpreter.html)

```python
# create_code_interpreter method definition

await def create_code_interpreter(
    self,
    *,
    name: str,
    networkConfiguration: CodeInterpreterNetworkConfigurationTypeDef,  # (1)
    description: str = ...,
    executionRoleArn: str = ...,
    clientToken: str = ...,
) -> CreateCodeInterpreterResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CodeInterpreterNetworkConfigurationTypeDef](./type_defs.md#codeinterpreternetworkconfigurationtypedef)
2. See [:material-code-braces: CreateCodeInterpreterResponseTypeDef](./type_defs.md#createcodeinterpreterresponsetypedef)


```python
# create_code_interpreter method usage example with argument unpacking

kwargs: CreateCodeInterpreterRequestTypeDef = {  # (1)
    "name": ...,
    "networkConfiguration": ...,
}

parent.create_code_interpreter(**kwargs)
```

1. See [:material-code-braces: CreateCodeInterpreterRequestTypeDef](./type_defs.md#createcodeinterpreterrequesttypedef)

### create\_gateway

Creates a gateway for Amazon Bedrock Agent.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").create_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/create_gateway.html)

```python
# create_gateway method definition

await def create_gateway(
    self,
    *,
    name: str,
    roleArn: str,
    protocolType: GatewayProtocolTypeType,  # (1)
    authorizerType: AuthorizerTypeType,  # (2)
    authorizerConfiguration: AuthorizerConfigurationUnionTypeDef,  # (3)
    description: str = ...,
    clientToken: str = ...,
    protocolConfiguration: GatewayProtocolConfigurationUnionTypeDef = ...,  # (4)
    kmsKeyArn: str = ...,
    exceptionLevel: ExceptionLevelType = ...,  # (5)
) -> CreateGatewayResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: GatewayProtocolTypeType](./literals.md#gatewayprotocoltypetype)
2. See [:material-code-brackets: AuthorizerTypeType](./literals.md#authorizertypetype)
3. See [:material-code-braces: AuthorizerConfigurationUnionTypeDef](#authorizerconfigurationuniontypedef)
4. See [:material-code-braces: GatewayProtocolConfigurationUnionTypeDef](#gatewayprotocolconfigurationuniontypedef)
5. See [:material-code-brackets: ExceptionLevelType](./literals.md#exceptionleveltype)
6. See [:material-code-braces: CreateGatewayResponseTypeDef](./type_defs.md#creategatewayresponsetypedef)


```python
# create_gateway method usage example with argument unpacking

kwargs: CreateGatewayRequestTypeDef = {  # (1)
    "name": ...,
    "roleArn": ...,
    "protocolType": ...,
    "authorizerType": ...,
    "authorizerConfiguration": ...,
}

parent.create_gateway(**kwargs)
```

1. See [:material-code-braces: CreateGatewayRequestTypeDef](./type_defs.md#creategatewayrequesttypedef)

### create\_gateway\_target

Creates a target for a gateway.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").create_gateway_target` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/create_gateway_target.html)

```python
# create_gateway_target method definition

await def create_gateway_target(
    self,
    *,
    gatewayIdentifier: str,
    name: str,
    targetConfiguration: TargetConfigurationUnionTypeDef,  # (1)
    credentialProviderConfigurations: Sequence[CredentialProviderConfigurationUnionTypeDef],  # (2)
    description: str = ...,
    clientToken: str = ...,
) -> CreateGatewayTargetResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TargetConfigurationUnionTypeDef](#targetconfigurationuniontypedef)
2. See `Sequence[CredentialProviderConfigurationUnionTypeDef]`
3. See [:material-code-braces: CreateGatewayTargetResponseTypeDef](./type_defs.md#creategatewaytargetresponsetypedef)


```python
# create_gateway_target method usage example with argument unpacking

kwargs: CreateGatewayTargetRequestTypeDef = {  # (1)
    "gatewayIdentifier": ...,
    "name": ...,
    "targetConfiguration": ...,
    "credentialProviderConfigurations": ...,
}

parent.create_gateway_target(**kwargs)
```

1. See [:material-code-braces: CreateGatewayTargetRequestTypeDef](./type_defs.md#creategatewaytargetrequesttypedef)

### create\_memory

Creates a new memory.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").create_memory` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/create_memory.html)

```python
# create_memory method definition

await def create_memory(
    self,
    *,
    name: str,
    eventExpiryDuration: int,
    clientToken: str = ...,
    description: str = ...,
    encryptionKeyArn: str = ...,
    memoryExecutionRoleArn: str = ...,
    memoryStrategies: Sequence[MemoryStrategyInputTypeDef] = ...,  # (1)
) -> CreateMemoryOutputTypeDef:  # (2)
    ...
```

1. See `Sequence[MemoryStrategyInputTypeDef]`
2. See [:material-code-braces: CreateMemoryOutputTypeDef](./type_defs.md#creatememoryoutputtypedef)


```python
# create_memory method usage example with argument unpacking

kwargs: CreateMemoryInputTypeDef = {  # (1)
    "name": ...,
    "eventExpiryDuration": ...,
}

parent.create_memory(**kwargs)
```

1. See [:material-code-braces: CreateMemoryInputTypeDef](./type_defs.md#creatememoryinputtypedef)

### create\_oauth2\_credential\_provider

Creates a new OAuth2 credential provider.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").create_oauth2_credential_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/create_oauth2_credential_provider.html)

```python
# create_oauth2_credential_provider method definition

await def create_oauth2_credential_provider(
    self,
    *,
    name: str,
    credentialProviderVendor: CredentialProviderVendorTypeType,  # (1)
    oauth2ProviderConfigInput: Oauth2ProviderConfigInputTypeDef,  # (2)
) -> CreateOauth2CredentialProviderResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: CredentialProviderVendorTypeType](./literals.md#credentialprovidervendortypetype)
2. See [:material-code-braces: Oauth2ProviderConfigInputTypeDef](./type_defs.md#oauth2providerconfiginputtypedef)
3. See [:material-code-braces: CreateOauth2CredentialProviderResponseTypeDef](./type_defs.md#createoauth2credentialproviderresponsetypedef)


```python
# create_oauth2_credential_provider method usage example with argument unpacking

kwargs: CreateOauth2CredentialProviderRequestTypeDef = {  # (1)
    "name": ...,
    "credentialProviderVendor": ...,
    "oauth2ProviderConfigInput": ...,
}

parent.create_oauth2_credential_provider(**kwargs)
```

1. See [:material-code-braces: CreateOauth2CredentialProviderRequestTypeDef](./type_defs.md#createoauth2credentialproviderrequesttypedef)

### create\_workload\_identity

Creates a new workload identity.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").create_workload_identity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/create_workload_identity.html)

```python
# create_workload_identity method definition

await def create_workload_identity(
    self,
    *,
    name: str,
    allowedResourceOauth2ReturnUrls: Sequence[str] = ...,
) -> CreateWorkloadIdentityResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateWorkloadIdentityResponseTypeDef](./type_defs.md#createworkloadidentityresponsetypedef)


```python
# create_workload_identity method usage example with argument unpacking

kwargs: CreateWorkloadIdentityRequestTypeDef = {  # (1)
    "name": ...,
}

parent.create_workload_identity(**kwargs)
```

1. See [:material-code-braces: CreateWorkloadIdentityRequestTypeDef](./type_defs.md#createworkloadidentityrequesttypedef)

### delete\_agent\_runtime

Deletes an Amazon Secure Agent.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").delete_agent_runtime` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/delete_agent_runtime.html)

```python
# delete_agent_runtime method definition

await def delete_agent_runtime(
    self,
    *,
    agentRuntimeId: str,
) -> DeleteAgentRuntimeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteAgentRuntimeResponseTypeDef](./type_defs.md#deleteagentruntimeresponsetypedef)


```python
# delete_agent_runtime method usage example with argument unpacking

kwargs: DeleteAgentRuntimeRequestTypeDef = {  # (1)
    "agentRuntimeId": ...,
}

parent.delete_agent_runtime(**kwargs)
```

1. See [:material-code-braces: DeleteAgentRuntimeRequestTypeDef](./type_defs.md#deleteagentruntimerequesttypedef)

### delete\_agent\_runtime\_endpoint

Deletes an Amazon Secure AgentEndpoint.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").delete_agent_runtime_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/delete_agent_runtime_endpoint.html)

```python
# delete_agent_runtime_endpoint method definition

await def delete_agent_runtime_endpoint(
    self,
    *,
    agentRuntimeId: str,
    endpointName: str,
    clientToken: str = ...,
) -> DeleteAgentRuntimeEndpointResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteAgentRuntimeEndpointResponseTypeDef](./type_defs.md#deleteagentruntimeendpointresponsetypedef)


```python
# delete_agent_runtime_endpoint method usage example with argument unpacking

kwargs: DeleteAgentRuntimeEndpointRequestTypeDef = {  # (1)
    "agentRuntimeId": ...,
    "endpointName": ...,
}

parent.delete_agent_runtime_endpoint(**kwargs)
```

1. See [:material-code-braces: DeleteAgentRuntimeEndpointRequestTypeDef](./type_defs.md#deleteagentruntimeendpointrequesttypedef)

### delete\_api\_key\_credential\_provider

Deletes an API key credential provider.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").delete_api_key_credential_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/delete_api_key_credential_provider.html)

```python
# delete_api_key_credential_provider method definition

await def delete_api_key_credential_provider(
    self,
    *,
    name: str,
) -> Dict[str, Any]:
    ...
```

```python
# delete_api_key_credential_provider method usage example with argument unpacking

kwargs: DeleteApiKeyCredentialProviderRequestTypeDef = {  # (1)
    "name": ...,
}

parent.delete_api_key_credential_provider(**kwargs)
```

1. See [:material-code-braces: DeleteApiKeyCredentialProviderRequestTypeDef](./type_defs.md#deleteapikeycredentialproviderrequesttypedef)

### delete\_browser

Deletes a custom browser.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").delete_browser` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/delete_browser.html)

```python
# delete_browser method definition

await def delete_browser(
    self,
    *,
    browserId: str,
    clientToken: str = ...,
) -> DeleteBrowserResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteBrowserResponseTypeDef](./type_defs.md#deletebrowserresponsetypedef)


```python
# delete_browser method usage example with argument unpacking

kwargs: DeleteBrowserRequestTypeDef = {  # (1)
    "browserId": ...,
}

parent.delete_browser(**kwargs)
```

1. See [:material-code-braces: DeleteBrowserRequestTypeDef](./type_defs.md#deletebrowserrequesttypedef)

### delete\_code\_interpreter

Deletes a custom code interpreter.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").delete_code_interpreter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/delete_code_interpreter.html)

```python
# delete_code_interpreter method definition

await def delete_code_interpreter(
    self,
    *,
    codeInterpreterId: str,
    clientToken: str = ...,
) -> DeleteCodeInterpreterResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteCodeInterpreterResponseTypeDef](./type_defs.md#deletecodeinterpreterresponsetypedef)


```python
# delete_code_interpreter method usage example with argument unpacking

kwargs: DeleteCodeInterpreterRequestTypeDef = {  # (1)
    "codeInterpreterId": ...,
}

parent.delete_code_interpreter(**kwargs)
```

1. See [:material-code-braces: DeleteCodeInterpreterRequestTypeDef](./type_defs.md#deletecodeinterpreterrequesttypedef)

### delete\_gateway

Deletes a Gateway.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").delete_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/delete_gateway.html)

```python
# delete_gateway method definition

await def delete_gateway(
    self,
    *,
    gatewayIdentifier: str,
) -> DeleteGatewayResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteGatewayResponseTypeDef](./type_defs.md#deletegatewayresponsetypedef)


```python
# delete_gateway method usage example with argument unpacking

kwargs: DeleteGatewayRequestTypeDef = {  # (1)
    "gatewayIdentifier": ...,
}

parent.delete_gateway(**kwargs)
```

1. See [:material-code-braces: DeleteGatewayRequestTypeDef](./type_defs.md#deletegatewayrequesttypedef)

### delete\_gateway\_target

Deletes a Gateway Target.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").delete_gateway_target` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/delete_gateway_target.html)

```python
# delete_gateway_target method definition

await def delete_gateway_target(
    self,
    *,
    gatewayIdentifier: str,
    targetId: str,
) -> DeleteGatewayTargetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteGatewayTargetResponseTypeDef](./type_defs.md#deletegatewaytargetresponsetypedef)


```python
# delete_gateway_target method usage example with argument unpacking

kwargs: DeleteGatewayTargetRequestTypeDef = {  # (1)
    "gatewayIdentifier": ...,
    "targetId": ...,
}

parent.delete_gateway_target(**kwargs)
```

1. See [:material-code-braces: DeleteGatewayTargetRequestTypeDef](./type_defs.md#deletegatewaytargetrequesttypedef)

### delete\_memory

Deletes a memory.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").delete_memory` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/delete_memory.html)

```python
# delete_memory method definition

await def delete_memory(
    self,
    *,
    memoryId: str,
    clientToken: str = ...,
) -> DeleteMemoryOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteMemoryOutputTypeDef](./type_defs.md#deletememoryoutputtypedef)


```python
# delete_memory method usage example with argument unpacking

kwargs: DeleteMemoryInputTypeDef = {  # (1)
    "memoryId": ...,
}

parent.delete_memory(**kwargs)
```

1. See [:material-code-braces: DeleteMemoryInputTypeDef](./type_defs.md#deletememoryinputtypedef)

### delete\_oauth2\_credential\_provider

Deletes an OAuth2 credential provider.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").delete_oauth2_credential_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/delete_oauth2_credential_provider.html)

```python
# delete_oauth2_credential_provider method definition

await def delete_oauth2_credential_provider(
    self,
    *,
    name: str,
) -> Dict[str, Any]:
    ...
```

```python
# delete_oauth2_credential_provider method usage example with argument unpacking

kwargs: DeleteOauth2CredentialProviderRequestTypeDef = {  # (1)
    "name": ...,
}

parent.delete_oauth2_credential_provider(**kwargs)
```

1. See [:material-code-braces: DeleteOauth2CredentialProviderRequestTypeDef](./type_defs.md#deleteoauth2credentialproviderrequesttypedef)

### delete\_workload\_identity

Deletes a workload identity.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").delete_workload_identity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/delete_workload_identity.html)

```python
# delete_workload_identity method definition

await def delete_workload_identity(
    self,
    *,
    name: str,
) -> Dict[str, Any]:
    ...
```

```python
# delete_workload_identity method usage example with argument unpacking

kwargs: DeleteWorkloadIdentityRequestTypeDef = {  # (1)
    "name": ...,
}

parent.delete_workload_identity(**kwargs)
```

1. See [:material-code-braces: DeleteWorkloadIdentityRequestTypeDef](./type_defs.md#deleteworkloadidentityrequesttypedef)

### get\_agent\_runtime

Gets an Amazon Secure Agent.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").get_agent_runtime` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/get_agent_runtime.html)

```python
# get_agent_runtime method definition

await def get_agent_runtime(
    self,
    *,
    agentRuntimeId: str,
    agentRuntimeVersion: str = ...,
) -> GetAgentRuntimeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAgentRuntimeResponseTypeDef](./type_defs.md#getagentruntimeresponsetypedef)


```python
# get_agent_runtime method usage example with argument unpacking

kwargs: GetAgentRuntimeRequestTypeDef = {  # (1)
    "agentRuntimeId": ...,
}

parent.get_agent_runtime(**kwargs)
```

1. See [:material-code-braces: GetAgentRuntimeRequestTypeDef](./type_defs.md#getagentruntimerequesttypedef)

### get\_agent\_runtime\_endpoint

Gets information about an Amazon Secure AgentEndpoint.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").get_agent_runtime_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/get_agent_runtime_endpoint.html)

```python
# get_agent_runtime_endpoint method definition

await def get_agent_runtime_endpoint(
    self,
    *,
    agentRuntimeId: str,
    endpointName: str,
) -> GetAgentRuntimeEndpointResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAgentRuntimeEndpointResponseTypeDef](./type_defs.md#getagentruntimeendpointresponsetypedef)


```python
# get_agent_runtime_endpoint method usage example with argument unpacking

kwargs: GetAgentRuntimeEndpointRequestTypeDef = {  # (1)
    "agentRuntimeId": ...,
    "endpointName": ...,
}

parent.get_agent_runtime_endpoint(**kwargs)
```

1. See [:material-code-braces: GetAgentRuntimeEndpointRequestTypeDef](./type_defs.md#getagentruntimeendpointrequesttypedef)

### get\_api\_key\_credential\_provider

Retrieves information about an API key credential provider.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").get_api_key_credential_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/get_api_key_credential_provider.html)

```python
# get_api_key_credential_provider method definition

await def get_api_key_credential_provider(
    self,
    *,
    name: str,
) -> GetApiKeyCredentialProviderResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetApiKeyCredentialProviderResponseTypeDef](./type_defs.md#getapikeycredentialproviderresponsetypedef)


```python
# get_api_key_credential_provider method usage example with argument unpacking

kwargs: GetApiKeyCredentialProviderRequestTypeDef = {  # (1)
    "name": ...,
}

parent.get_api_key_credential_provider(**kwargs)
```

1. See [:material-code-braces: GetApiKeyCredentialProviderRequestTypeDef](./type_defs.md#getapikeycredentialproviderrequesttypedef)

### get\_browser

Gets information about a custom browser.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").get_browser` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/get_browser.html)

```python
# get_browser method definition

await def get_browser(
    self,
    *,
    browserId: str,
) -> GetBrowserResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetBrowserResponseTypeDef](./type_defs.md#getbrowserresponsetypedef)


```python
# get_browser method usage example with argument unpacking

kwargs: GetBrowserRequestTypeDef = {  # (1)
    "browserId": ...,
}

parent.get_browser(**kwargs)
```

1. See [:material-code-braces: GetBrowserRequestTypeDef](./type_defs.md#getbrowserrequesttypedef)

### get\_code\_interpreter

Gets information about a custom code interpreter.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").get_code_interpreter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/get_code_interpreter.html)

```python
# get_code_interpreter method definition

await def get_code_interpreter(
    self,
    *,
    codeInterpreterId: str,
) -> GetCodeInterpreterResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCodeInterpreterResponseTypeDef](./type_defs.md#getcodeinterpreterresponsetypedef)


```python
# get_code_interpreter method usage example with argument unpacking

kwargs: GetCodeInterpreterRequestTypeDef = {  # (1)
    "codeInterpreterId": ...,
}

parent.get_code_interpreter(**kwargs)
```

1. See [:material-code-braces: GetCodeInterpreterRequestTypeDef](./type_defs.md#getcodeinterpreterrequesttypedef)

### get\_gateway

Retrieves information about a specific Gateway.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").get_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/get_gateway.html)

```python
# get_gateway method definition

await def get_gateway(
    self,
    *,
    gatewayIdentifier: str,
) -> GetGatewayResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetGatewayResponseTypeDef](./type_defs.md#getgatewayresponsetypedef)


```python
# get_gateway method usage example with argument unpacking

kwargs: GetGatewayRequestTypeDef = {  # (1)
    "gatewayIdentifier": ...,
}

parent.get_gateway(**kwargs)
```

1. See [:material-code-braces: GetGatewayRequestTypeDef](./type_defs.md#getgatewayrequesttypedef)

### get\_gateway\_target

Retrieves information about a specific Gateway Target.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").get_gateway_target` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/get_gateway_target.html)

```python
# get_gateway_target method definition

await def get_gateway_target(
    self,
    *,
    gatewayIdentifier: str,
    targetId: str,
) -> GetGatewayTargetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetGatewayTargetResponseTypeDef](./type_defs.md#getgatewaytargetresponsetypedef)


```python
# get_gateway_target method usage example with argument unpacking

kwargs: GetGatewayTargetRequestTypeDef = {  # (1)
    "gatewayIdentifier": ...,
    "targetId": ...,
}

parent.get_gateway_target(**kwargs)
```

1. See [:material-code-braces: GetGatewayTargetRequestTypeDef](./type_defs.md#getgatewaytargetrequesttypedef)

### get\_memory

Retrieve an existing memory.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").get_memory` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/get_memory.html)

```python
# get_memory method definition

await def get_memory(
    self,
    *,
    memoryId: str,
) -> GetMemoryOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMemoryOutputTypeDef](./type_defs.md#getmemoryoutputtypedef)


```python
# get_memory method usage example with argument unpacking

kwargs: GetMemoryInputTypeDef = {  # (1)
    "memoryId": ...,
}

parent.get_memory(**kwargs)
```

1. See [:material-code-braces: GetMemoryInputTypeDef](./type_defs.md#getmemoryinputtypedef)

### get\_oauth2\_credential\_provider

Retrieves information about an OAuth2 credential provider.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").get_oauth2_credential_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/get_oauth2_credential_provider.html)

```python
# get_oauth2_credential_provider method definition

await def get_oauth2_credential_provider(
    self,
    *,
    name: str,
) -> GetOauth2CredentialProviderResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOauth2CredentialProviderResponseTypeDef](./type_defs.md#getoauth2credentialproviderresponsetypedef)


```python
# get_oauth2_credential_provider method usage example with argument unpacking

kwargs: GetOauth2CredentialProviderRequestTypeDef = {  # (1)
    "name": ...,
}

parent.get_oauth2_credential_provider(**kwargs)
```

1. See [:material-code-braces: GetOauth2CredentialProviderRequestTypeDef](./type_defs.md#getoauth2credentialproviderrequesttypedef)

### get\_token\_vault

Retrieves information about a token vault.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").get_token_vault` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/get_token_vault.html)

```python
# get_token_vault method definition

await def get_token_vault(
    self,
    *,
    tokenVaultId: str = ...,
) -> GetTokenVaultResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTokenVaultResponseTypeDef](./type_defs.md#gettokenvaultresponsetypedef)


```python
# get_token_vault method usage example with argument unpacking

kwargs: GetTokenVaultRequestTypeDef = {  # (1)
    "tokenVaultId": ...,
}

parent.get_token_vault(**kwargs)
```

1. See [:material-code-braces: GetTokenVaultRequestTypeDef](./type_defs.md#gettokenvaultrequesttypedef)

### get\_workload\_identity

Retrieves information about a workload identity.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").get_workload_identity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/get_workload_identity.html)

```python
# get_workload_identity method definition

await def get_workload_identity(
    self,
    *,
    name: str,
) -> GetWorkloadIdentityResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWorkloadIdentityResponseTypeDef](./type_defs.md#getworkloadidentityresponsetypedef)


```python
# get_workload_identity method usage example with argument unpacking

kwargs: GetWorkloadIdentityRequestTypeDef = {  # (1)
    "name": ...,
}

parent.get_workload_identity(**kwargs)
```

1. See [:material-code-braces: GetWorkloadIdentityRequestTypeDef](./type_defs.md#getworkloadidentityrequesttypedef)

### list\_agent\_runtime\_endpoints

Lists all endpoints for a specific Amazon Secure Agent.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").list_agent_runtime_endpoints` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/list_agent_runtime_endpoints.html)

```python
# list_agent_runtime_endpoints method definition

await def list_agent_runtime_endpoints(
    self,
    *,
    agentRuntimeId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAgentRuntimeEndpointsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAgentRuntimeEndpointsResponseTypeDef](./type_defs.md#listagentruntimeendpointsresponsetypedef)


```python
# list_agent_runtime_endpoints method usage example with argument unpacking

kwargs: ListAgentRuntimeEndpointsRequestTypeDef = {  # (1)
    "agentRuntimeId": ...,
}

parent.list_agent_runtime_endpoints(**kwargs)
```

1. See [:material-code-braces: ListAgentRuntimeEndpointsRequestTypeDef](./type_defs.md#listagentruntimeendpointsrequesttypedef)

### list\_agent\_runtime\_versions

Lists all versions of a specific Amazon Secure Agent.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").list_agent_runtime_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/list_agent_runtime_versions.html)

```python
# list_agent_runtime_versions method definition

await def list_agent_runtime_versions(
    self,
    *,
    agentRuntimeId: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAgentRuntimeVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAgentRuntimeVersionsResponseTypeDef](./type_defs.md#listagentruntimeversionsresponsetypedef)


```python
# list_agent_runtime_versions method usage example with argument unpacking

kwargs: ListAgentRuntimeVersionsRequestTypeDef = {  # (1)
    "agentRuntimeId": ...,
}

parent.list_agent_runtime_versions(**kwargs)
```

1. See [:material-code-braces: ListAgentRuntimeVersionsRequestTypeDef](./type_defs.md#listagentruntimeversionsrequesttypedef)

### list\_agent\_runtimes

Lists all Amazon Secure Agents in your account.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").list_agent_runtimes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/list_agent_runtimes.html)

```python
# list_agent_runtimes method definition

await def list_agent_runtimes(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAgentRuntimesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAgentRuntimesResponseTypeDef](./type_defs.md#listagentruntimesresponsetypedef)


```python
# list_agent_runtimes method usage example with argument unpacking

kwargs: ListAgentRuntimesRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_agent_runtimes(**kwargs)
```

1. See [:material-code-braces: ListAgentRuntimesRequestTypeDef](./type_defs.md#listagentruntimesrequesttypedef)

### list\_api\_key\_credential\_providers

Lists all API key credential providers in your account.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").list_api_key_credential_providers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/list_api_key_credential_providers.html)

```python
# list_api_key_credential_providers method definition

await def list_api_key_credential_providers(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListApiKeyCredentialProvidersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListApiKeyCredentialProvidersResponseTypeDef](./type_defs.md#listapikeycredentialprovidersresponsetypedef)


```python
# list_api_key_credential_providers method usage example with argument unpacking

kwargs: ListApiKeyCredentialProvidersRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_api_key_credential_providers(**kwargs)
```

1. See [:material-code-braces: ListApiKeyCredentialProvidersRequestTypeDef](./type_defs.md#listapikeycredentialprovidersrequesttypedef)

### list\_browsers

Lists all custom browsers in your account.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").list_browsers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/list_browsers.html)

```python
# list_browsers method definition

await def list_browsers(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    type: ResourceTypeType = ...,  # (1)
) -> ListBrowsersResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype)
2. See [:material-code-braces: ListBrowsersResponseTypeDef](./type_defs.md#listbrowsersresponsetypedef)


```python
# list_browsers method usage example with argument unpacking

kwargs: ListBrowsersRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_browsers(**kwargs)
```

1. See [:material-code-braces: ListBrowsersRequestTypeDef](./type_defs.md#listbrowsersrequesttypedef)

### list\_code\_interpreters

Lists all custom code interpreters in your account.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").list_code_interpreters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/list_code_interpreters.html)

```python
# list_code_interpreters method definition

await def list_code_interpreters(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    type: ResourceTypeType = ...,  # (1)
) -> ListCodeInterpretersResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype)
2. See [:material-code-braces: ListCodeInterpretersResponseTypeDef](./type_defs.md#listcodeinterpretersresponsetypedef)


```python
# list_code_interpreters method usage example with argument unpacking

kwargs: ListCodeInterpretersRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_code_interpreters(**kwargs)
```

1. See [:material-code-braces: ListCodeInterpretersRequestTypeDef](./type_defs.md#listcodeinterpretersrequesttypedef)

### list\_gateway\_targets

Lists all targets for a specific Gateway.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").list_gateway_targets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/list_gateway_targets.html)

```python
# list_gateway_targets method definition

await def list_gateway_targets(
    self,
    *,
    gatewayIdentifier: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListGatewayTargetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGatewayTargetsResponseTypeDef](./type_defs.md#listgatewaytargetsresponsetypedef)


```python
# list_gateway_targets method usage example with argument unpacking

kwargs: ListGatewayTargetsRequestTypeDef = {  # (1)
    "gatewayIdentifier": ...,
}

parent.list_gateway_targets(**kwargs)
```

1. See [:material-code-braces: ListGatewayTargetsRequestTypeDef](./type_defs.md#listgatewaytargetsrequesttypedef)

### list\_gateways

Lists all Gateways in the account.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").list_gateways` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/list_gateways.html)

```python
# list_gateways method definition

await def list_gateways(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListGatewaysResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGatewaysResponseTypeDef](./type_defs.md#listgatewaysresponsetypedef)


```python
# list_gateways method usage example with argument unpacking

kwargs: ListGatewaysRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_gateways(**kwargs)
```

1. See [:material-code-braces: ListGatewaysRequestTypeDef](./type_defs.md#listgatewaysrequesttypedef)

### list\_memories

Lists the memory present.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").list_memories` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/list_memories.html)

```python
# list_memories method definition

await def list_memories(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListMemoriesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMemoriesOutputTypeDef](./type_defs.md#listmemoriesoutputtypedef)


```python
# list_memories method usage example with argument unpacking

kwargs: ListMemoriesInputTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_memories(**kwargs)
```

1. See [:material-code-braces: ListMemoriesInputTypeDef](./type_defs.md#listmemoriesinputtypedef)

### list\_oauth2\_credential\_providers

Lists all OAuth2 credential providers in your account.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").list_oauth2_credential_providers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/list_oauth2_credential_providers.html)

```python
# list_oauth2_credential_providers method definition

await def list_oauth2_credential_providers(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListOauth2CredentialProvidersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListOauth2CredentialProvidersResponseTypeDef](./type_defs.md#listoauth2credentialprovidersresponsetypedef)


```python
# list_oauth2_credential_providers method usage example with argument unpacking

kwargs: ListOauth2CredentialProvidersRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_oauth2_credential_providers(**kwargs)
```

1. See [:material-code-braces: ListOauth2CredentialProvidersRequestTypeDef](./type_defs.md#listoauth2credentialprovidersrequesttypedef)

### list\_workload\_identities

Lists all workload identities in your account.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").list_workload_identities` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/list_workload_identities.html)

```python
# list_workload_identities method definition

await def list_workload_identities(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListWorkloadIdentitiesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListWorkloadIdentitiesResponseTypeDef](./type_defs.md#listworkloadidentitiesresponsetypedef)


```python
# list_workload_identities method usage example with argument unpacking

kwargs: ListWorkloadIdentitiesRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_workload_identities(**kwargs)
```

1. See [:material-code-braces: ListWorkloadIdentitiesRequestTypeDef](./type_defs.md#listworkloadidentitiesrequesttypedef)

### set\_token\_vault\_cmk

Sets the customer master key (CMK) for a token vault.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").set_token_vault_cmk` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/set_token_vault_cmk.html)

```python
# set_token_vault_cmk method definition

await def set_token_vault_cmk(
    self,
    *,
    kmsConfiguration: KmsConfigurationTypeDef,  # (1)
    tokenVaultId: str = ...,
) -> SetTokenVaultCMKResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: KmsConfigurationTypeDef](./type_defs.md#kmsconfigurationtypedef)
2. See [:material-code-braces: SetTokenVaultCMKResponseTypeDef](./type_defs.md#settokenvaultcmkresponsetypedef)


```python
# set_token_vault_cmk method usage example with argument unpacking

kwargs: SetTokenVaultCMKRequestTypeDef = {  # (1)
    "kmsConfiguration": ...,
}

parent.set_token_vault_cmk(**kwargs)
```

1. See [:material-code-braces: SetTokenVaultCMKRequestTypeDef](./type_defs.md#settokenvaultcmkrequesttypedef)

### update\_agent\_runtime

Updates an existing Amazon Secure Agent.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").update_agent_runtime` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/update_agent_runtime.html)

```python
# update_agent_runtime method definition

await def update_agent_runtime(
    self,
    *,
    agentRuntimeId: str,
    agentRuntimeArtifact: AgentArtifactTypeDef,  # (1)
    roleArn: str,
    networkConfiguration: NetworkConfigurationTypeDef,  # (2)
    description: str = ...,
    protocolConfiguration: ProtocolConfigurationTypeDef = ...,  # (3)
    clientToken: str = ...,
    environmentVariables: Mapping[str, str] = ...,
    authorizerConfiguration: AuthorizerConfigurationUnionTypeDef = ...,  # (4)
) -> UpdateAgentRuntimeResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: AgentArtifactTypeDef](./type_defs.md#agentartifacttypedef)
2. See [:material-code-braces: NetworkConfigurationTypeDef](./type_defs.md#networkconfigurationtypedef)
3. See [:material-code-braces: ProtocolConfigurationTypeDef](./type_defs.md#protocolconfigurationtypedef)
4. See [:material-code-braces: AuthorizerConfigurationUnionTypeDef](#authorizerconfigurationuniontypedef)
5. See [:material-code-braces: UpdateAgentRuntimeResponseTypeDef](./type_defs.md#updateagentruntimeresponsetypedef)


```python
# update_agent_runtime method usage example with argument unpacking

kwargs: UpdateAgentRuntimeRequestTypeDef = {  # (1)
    "agentRuntimeId": ...,
    "agentRuntimeArtifact": ...,
    "roleArn": ...,
    "networkConfiguration": ...,
}

parent.update_agent_runtime(**kwargs)
```

1. See [:material-code-braces: UpdateAgentRuntimeRequestTypeDef](./type_defs.md#updateagentruntimerequesttypedef)

### update\_agent\_runtime\_endpoint

Updates an existing Amazon Secure AgentEndpoint.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").update_agent_runtime_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/update_agent_runtime_endpoint.html)

```python
# update_agent_runtime_endpoint method definition

await def update_agent_runtime_endpoint(
    self,
    *,
    agentRuntimeId: str,
    endpointName: str,
    agentRuntimeVersion: str = ...,
    description: str = ...,
    clientToken: str = ...,
) -> UpdateAgentRuntimeEndpointResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateAgentRuntimeEndpointResponseTypeDef](./type_defs.md#updateagentruntimeendpointresponsetypedef)


```python
# update_agent_runtime_endpoint method usage example with argument unpacking

kwargs: UpdateAgentRuntimeEndpointRequestTypeDef = {  # (1)
    "agentRuntimeId": ...,
    "endpointName": ...,
}

parent.update_agent_runtime_endpoint(**kwargs)
```

1. See [:material-code-braces: UpdateAgentRuntimeEndpointRequestTypeDef](./type_defs.md#updateagentruntimeendpointrequesttypedef)

### update\_api\_key\_credential\_provider

Updates an existing API key credential provider.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").update_api_key_credential_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/update_api_key_credential_provider.html)

```python
# update_api_key_credential_provider method definition

await def update_api_key_credential_provider(
    self,
    *,
    name: str,
    apiKey: str,
) -> UpdateApiKeyCredentialProviderResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateApiKeyCredentialProviderResponseTypeDef](./type_defs.md#updateapikeycredentialproviderresponsetypedef)


```python
# update_api_key_credential_provider method usage example with argument unpacking

kwargs: UpdateApiKeyCredentialProviderRequestTypeDef = {  # (1)
    "name": ...,
    "apiKey": ...,
}

parent.update_api_key_credential_provider(**kwargs)
```

1. See [:material-code-braces: UpdateApiKeyCredentialProviderRequestTypeDef](./type_defs.md#updateapikeycredentialproviderrequesttypedef)

### update\_gateway

Updates an existing Gateway.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").update_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/update_gateway.html)

```python
# update_gateway method definition

await def update_gateway(
    self,
    *,
    gatewayIdentifier: str,
    name: str,
    roleArn: str,
    protocolType: GatewayProtocolTypeType,  # (1)
    authorizerType: AuthorizerTypeType,  # (2)
    authorizerConfiguration: AuthorizerConfigurationUnionTypeDef,  # (3)
    description: str = ...,
    protocolConfiguration: GatewayProtocolConfigurationUnionTypeDef = ...,  # (4)
    kmsKeyArn: str = ...,
    exceptionLevel: ExceptionLevelType = ...,  # (5)
) -> UpdateGatewayResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: GatewayProtocolTypeType](./literals.md#gatewayprotocoltypetype)
2. See [:material-code-brackets: AuthorizerTypeType](./literals.md#authorizertypetype)
3. See [:material-code-braces: AuthorizerConfigurationUnionTypeDef](#authorizerconfigurationuniontypedef)
4. See [:material-code-braces: GatewayProtocolConfigurationUnionTypeDef](#gatewayprotocolconfigurationuniontypedef)
5. See [:material-code-brackets: ExceptionLevelType](./literals.md#exceptionleveltype)
6. See [:material-code-braces: UpdateGatewayResponseTypeDef](./type_defs.md#updategatewayresponsetypedef)


```python
# update_gateway method usage example with argument unpacking

kwargs: UpdateGatewayRequestTypeDef = {  # (1)
    "gatewayIdentifier": ...,
    "name": ...,
    "roleArn": ...,
    "protocolType": ...,
    "authorizerType": ...,
    "authorizerConfiguration": ...,
}

parent.update_gateway(**kwargs)
```

1. See [:material-code-braces: UpdateGatewayRequestTypeDef](./type_defs.md#updategatewayrequesttypedef)

### update\_gateway\_target

Updates an existing Gateway Target.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").update_gateway_target` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/update_gateway_target.html)

```python
# update_gateway_target method definition

await def update_gateway_target(
    self,
    *,
    gatewayIdentifier: str,
    targetId: str,
    name: str,
    targetConfiguration: TargetConfigurationUnionTypeDef,  # (1)
    credentialProviderConfigurations: Sequence[CredentialProviderConfigurationUnionTypeDef],  # (2)
    description: str = ...,
) -> UpdateGatewayTargetResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TargetConfigurationUnionTypeDef](#targetconfigurationuniontypedef)
2. See `Sequence[CredentialProviderConfigurationUnionTypeDef]`
3. See [:material-code-braces: UpdateGatewayTargetResponseTypeDef](./type_defs.md#updategatewaytargetresponsetypedef)


```python
# update_gateway_target method usage example with argument unpacking

kwargs: UpdateGatewayTargetRequestTypeDef = {  # (1)
    "gatewayIdentifier": ...,
    "targetId": ...,
    "name": ...,
    "targetConfiguration": ...,
    "credentialProviderConfigurations": ...,
}

parent.update_gateway_target(**kwargs)
```

1. See [:material-code-braces: UpdateGatewayTargetRequestTypeDef](./type_defs.md#updategatewaytargetrequesttypedef)

### update\_memory

Update memory.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").update_memory` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/update_memory.html)

```python
# update_memory method definition

await def update_memory(
    self,
    *,
    memoryId: str,
    clientToken: str = ...,
    description: str = ...,
    eventExpiryDuration: int = ...,
    memoryExecutionRoleArn: str = ...,
    memoryStrategies: ModifyMemoryStrategiesTypeDef = ...,  # (1)
) -> UpdateMemoryOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ModifyMemoryStrategiesTypeDef](./type_defs.md#modifymemorystrategiestypedef)
2. See [:material-code-braces: UpdateMemoryOutputTypeDef](./type_defs.md#updatememoryoutputtypedef)


```python
# update_memory method usage example with argument unpacking

kwargs: UpdateMemoryInputTypeDef = {  # (1)
    "memoryId": ...,
}

parent.update_memory(**kwargs)
```

1. See [:material-code-braces: UpdateMemoryInputTypeDef](./type_defs.md#updatememoryinputtypedef)

### update\_oauth2\_credential\_provider

Updates an existing OAuth2 credential provider.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").update_oauth2_credential_provider` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/update_oauth2_credential_provider.html)

```python
# update_oauth2_credential_provider method definition

await def update_oauth2_credential_provider(
    self,
    *,
    name: str,
    credentialProviderVendor: CredentialProviderVendorTypeType,  # (1)
    oauth2ProviderConfigInput: Oauth2ProviderConfigInputTypeDef,  # (2)
) -> UpdateOauth2CredentialProviderResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: CredentialProviderVendorTypeType](./literals.md#credentialprovidervendortypetype)
2. See [:material-code-braces: Oauth2ProviderConfigInputTypeDef](./type_defs.md#oauth2providerconfiginputtypedef)
3. See [:material-code-braces: UpdateOauth2CredentialProviderResponseTypeDef](./type_defs.md#updateoauth2credentialproviderresponsetypedef)


```python
# update_oauth2_credential_provider method usage example with argument unpacking

kwargs: UpdateOauth2CredentialProviderRequestTypeDef = {  # (1)
    "name": ...,
    "credentialProviderVendor": ...,
    "oauth2ProviderConfigInput": ...,
}

parent.update_oauth2_credential_provider(**kwargs)
```

1. See [:material-code-braces: UpdateOauth2CredentialProviderRequestTypeDef](./type_defs.md#updateoauth2credentialproviderrequesttypedef)

### update\_workload\_identity

Updates an existing workload identity.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").update_workload_identity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/update_workload_identity.html)

```python
# update_workload_identity method definition

await def update_workload_identity(
    self,
    *,
    name: str,
    allowedResourceOauth2ReturnUrls: Sequence[str] = ...,
) -> UpdateWorkloadIdentityResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateWorkloadIdentityResponseTypeDef](./type_defs.md#updateworkloadidentityresponsetypedef)


```python
# update_workload_identity method usage example with argument unpacking

kwargs: UpdateWorkloadIdentityRequestTypeDef = {  # (1)
    "name": ...,
}

parent.update_workload_identity(**kwargs)
```

1. See [:material-code-braces: UpdateWorkloadIdentityRequestTypeDef](./type_defs.md#updateworkloadidentityrequesttypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control.html#BedrockAgentCoreControlPlaneFrontingLayer.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control.html#BedrockAgentCoreControlPlaneFrontingLayer.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Type[BaseException] | None,
    exc_val: BaseException | None,
    exc_tb: types.TracebackType | None,
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").get_paginator` method with overloads.

- `client.get_paginator("list_agent_runtime_endpoints")` -> [ListAgentRuntimeEndpointsPaginator](./paginators.md#listagentruntimeendpointspaginator)
- `client.get_paginator("list_agent_runtime_versions")` -> [ListAgentRuntimeVersionsPaginator](./paginators.md#listagentruntimeversionspaginator)
- `client.get_paginator("list_agent_runtimes")` -> [ListAgentRuntimesPaginator](./paginators.md#listagentruntimespaginator)
- `client.get_paginator("list_api_key_credential_providers")` -> [ListApiKeyCredentialProvidersPaginator](./paginators.md#listapikeycredentialproviderspaginator)
- `client.get_paginator("list_browsers")` -> [ListBrowsersPaginator](./paginators.md#listbrowserspaginator)
- `client.get_paginator("list_code_interpreters")` -> [ListCodeInterpretersPaginator](./paginators.md#listcodeinterpreterspaginator)
- `client.get_paginator("list_gateway_targets")` -> [ListGatewayTargetsPaginator](./paginators.md#listgatewaytargetspaginator)
- `client.get_paginator("list_gateways")` -> [ListGatewaysPaginator](./paginators.md#listgatewayspaginator)
- `client.get_paginator("list_memories")` -> [ListMemoriesPaginator](./paginators.md#listmemoriespaginator)
- `client.get_paginator("list_oauth2_credential_providers")` -> [ListOauth2CredentialProvidersPaginator](./paginators.md#listoauth2credentialproviderspaginator)
- `client.get_paginator("list_workload_identities")` -> [ListWorkloadIdentitiesPaginator](./paginators.md#listworkloadidentitiespaginator)




### get_waiter

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").get_waiter` method with overloads.

- `client.get_waiter("memory_created")` -> [MemoryCreatedWaiter](./waiters.md#memorycreatedwaiter)

