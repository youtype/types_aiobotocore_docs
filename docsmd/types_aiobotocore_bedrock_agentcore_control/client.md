# BedrockAgentCoreControlClient

> [Index](../README.md) > [BedrockAgentCoreControl](./README.md) > BedrockAgentCoreControlClient

!!! note ""

    Auto-generated documentation for [BedrockAgentCoreControl](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control.html#bedrockagentcorecontrol)
    type annotations stubs module [types-aiobotocore-bedrock-agentcore-control](https://pypi.org/project/types-aiobotocore-bedrock-agentcore-control/).

## BedrockAgentCoreControlClient

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control.html#BedrockAgentCoreControl.Client)

```python
# BedrockAgentCoreControlClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_bedrock_agentcore_control.client import BedrockAgentCoreControlClient

session = get_session()
async with session.create_client("bedrock-agentcore-control") as client:
    client: BedrockAgentCoreControlClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("bedrock-agentcore-control").exceptions` structure.

```python
# BedrockAgentCoreControlClient.exceptions usage example

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
# BedrockAgentCoreControlClient usage type checking example

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

Creates an Amazon Bedrock AgentCore Runtime.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").create_agent_runtime` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/create_agent_runtime.html)

```python
# create_agent_runtime method definition

await def create_agent_runtime(
    self,
    *,
    agentRuntimeName: str,
    agentRuntimeArtifact: AgentRuntimeArtifactUnionTypeDef,  # (1)
    roleArn: str,
    networkConfiguration: NetworkConfigurationUnionTypeDef,  # (2)
    clientToken: str = ...,
    description: str = ...,
    authorizerConfiguration: AuthorizerConfigurationUnionTypeDef = ...,  # (3)
    requestHeaderConfiguration: RequestHeaderConfigurationUnionTypeDef = ...,  # (4)
    protocolConfiguration: ProtocolConfigurationTypeDef = ...,  # (5)
    lifecycleConfiguration: LifecycleConfigurationTypeDef = ...,  # (6)
    environmentVariables: Mapping[str, str] = ...,
    tags: Mapping[str, str] = ...,
) -> CreateAgentRuntimeResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: AgentRuntimeArtifactUnionTypeDef](#agentruntimeartifactuniontypedef)
2. See [:material-code-braces: NetworkConfigurationUnionTypeDef](#networkconfigurationuniontypedef)
3. See [:material-code-braces: AuthorizerConfigurationUnionTypeDef](#authorizerconfigurationuniontypedef)
4. See [:material-code-braces: RequestHeaderConfigurationUnionTypeDef](#requestheaderconfigurationuniontypedef)
5. See [:material-code-braces: ProtocolConfigurationTypeDef](./type_defs.md#protocolconfigurationtypedef)
6. See [:material-code-braces: LifecycleConfigurationTypeDef](./type_defs.md#lifecycleconfigurationtypedef)
7. See [:material-code-braces: CreateAgentRuntimeResponseTypeDef](./type_defs.md#createagentruntimeresponsetypedef)


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

Creates an AgentCore Runtime endpoint.

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
    tags: Mapping[str, str] = ...,
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
    tags: Mapping[str, str] = ...,
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
    networkConfiguration: BrowserNetworkConfigurationUnionTypeDef,  # (1)
    description: str = ...,
    executionRoleArn: str = ...,
    recording: RecordingConfigTypeDef = ...,  # (2)
    browserSigning: BrowserSigningConfigInputTypeDef = ...,  # (3)
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateBrowserResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: BrowserNetworkConfigurationUnionTypeDef](#browsernetworkconfigurationuniontypedef)
2. See [:material-code-braces: RecordingConfigTypeDef](./type_defs.md#recordingconfigtypedef)
3. See [:material-code-braces: BrowserSigningConfigInputTypeDef](./type_defs.md#browsersigningconfiginputtypedef)
4. See [:material-code-braces: CreateBrowserResponseTypeDef](./type_defs.md#createbrowserresponsetypedef)


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
    networkConfiguration: CodeInterpreterNetworkConfigurationUnionTypeDef,  # (1)
    description: str = ...,
    executionRoleArn: str = ...,
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateCodeInterpreterResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CodeInterpreterNetworkConfigurationUnionTypeDef](#codeinterpreternetworkconfigurationuniontypedef)
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

### create\_evaluator

Creates a custom evaluator for agent quality assessment.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").create_evaluator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/create_evaluator.html)

```python
# create_evaluator method definition

await def create_evaluator(
    self,
    *,
    evaluatorName: str,
    evaluatorConfig: EvaluatorConfigUnionTypeDef,  # (1)
    level: EvaluatorLevelType,  # (2)
    clientToken: str = ...,
    description: str = ...,
) -> CreateEvaluatorResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: EvaluatorConfigUnionTypeDef](#evaluatorconfiguniontypedef)
2. See [:material-code-brackets: EvaluatorLevelType](./literals.md#evaluatorleveltype)
3. See [:material-code-braces: CreateEvaluatorResponseTypeDef](./type_defs.md#createevaluatorresponsetypedef)


```python
# create_evaluator method usage example with argument unpacking

kwargs: CreateEvaluatorRequestTypeDef = {  # (1)
    "evaluatorName": ...,
    "evaluatorConfig": ...,
    "level": ...,
}

parent.create_evaluator(**kwargs)
```

1. See [:material-code-braces: CreateEvaluatorRequestTypeDef](./type_defs.md#createevaluatorrequesttypedef)

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
    description: str = ...,
    clientToken: str = ...,
    protocolConfiguration: GatewayProtocolConfigurationUnionTypeDef = ...,  # (3)
    authorizerConfiguration: AuthorizerConfigurationUnionTypeDef = ...,  # (4)
    kmsKeyArn: str = ...,
    interceptorConfigurations: Sequence[GatewayInterceptorConfigurationUnionTypeDef] = ...,  # (5)
    policyEngineConfiguration: GatewayPolicyEngineConfigurationTypeDef = ...,  # (6)
    exceptionLevel: ExceptionLevelType = ...,  # (7)
    tags: Mapping[str, str] = ...,
) -> CreateGatewayResponseTypeDef:  # (8)
    ...
```

1. See [:material-code-brackets: GatewayProtocolTypeType](./literals.md#gatewayprotocoltypetype)
2. See [:material-code-brackets: AuthorizerTypeType](./literals.md#authorizertypetype)
3. See [:material-code-braces: GatewayProtocolConfigurationUnionTypeDef](#gatewayprotocolconfigurationuniontypedef)
4. See [:material-code-braces: AuthorizerConfigurationUnionTypeDef](#authorizerconfigurationuniontypedef)
5. See `Sequence[GatewayInterceptorConfigurationUnionTypeDef]`
6. See [:material-code-braces: GatewayPolicyEngineConfigurationTypeDef](./type_defs.md#gatewaypolicyengineconfigurationtypedef)
7. See [:material-code-brackets: ExceptionLevelType](./literals.md#exceptionleveltype)
8. See [:material-code-braces: CreateGatewayResponseTypeDef](./type_defs.md#creategatewayresponsetypedef)


```python
# create_gateway method usage example with argument unpacking

kwargs: CreateGatewayRequestTypeDef = {  # (1)
    "name": ...,
    "roleArn": ...,
    "protocolType": ...,
    "authorizerType": ...,
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
    description: str = ...,
    clientToken: str = ...,
    credentialProviderConfigurations: Sequence[CredentialProviderConfigurationUnionTypeDef] = ...,  # (2)
    metadataConfiguration: MetadataConfigurationUnionTypeDef = ...,  # (3)
) -> CreateGatewayTargetResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: TargetConfigurationUnionTypeDef](#targetconfigurationuniontypedef)
2. See `Sequence[CredentialProviderConfigurationUnionTypeDef]`
3. See [:material-code-braces: MetadataConfigurationUnionTypeDef](#metadataconfigurationuniontypedef)
4. See [:material-code-braces: CreateGatewayTargetResponseTypeDef](./type_defs.md#creategatewaytargetresponsetypedef)


```python
# create_gateway_target method usage example with argument unpacking

kwargs: CreateGatewayTargetRequestTypeDef = {  # (1)
    "gatewayIdentifier": ...,
    "name": ...,
    "targetConfiguration": ...,
}

parent.create_gateway_target(**kwargs)
```

1. See [:material-code-braces: CreateGatewayTargetRequestTypeDef](./type_defs.md#creategatewaytargetrequesttypedef)

### create\_memory

Creates a new Amazon Bedrock AgentCore Memory resource.

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
    tags: Mapping[str, str] = ...,
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
    tags: Mapping[str, str] = ...,
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

### create\_online\_evaluation\_config

Creates an online evaluation configuration for continuous monitoring of agent
performance.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").create_online_evaluation_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/create_online_evaluation_config.html)

```python
# create_online_evaluation_config method definition

await def create_online_evaluation_config(
    self,
    *,
    onlineEvaluationConfigName: str,
    rule: RuleUnionTypeDef,  # (1)
    dataSourceConfig: DataSourceConfigUnionTypeDef,  # (2)
    evaluators: Sequence[EvaluatorReferenceTypeDef],  # (3)
    evaluationExecutionRoleArn: str,
    enableOnCreate: bool,
    clientToken: str = ...,
    description: str = ...,
) -> CreateOnlineEvaluationConfigResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: RuleUnionTypeDef](#ruleuniontypedef)
2. See [:material-code-braces: DataSourceConfigUnionTypeDef](#datasourceconfiguniontypedef)
3. See `Sequence[EvaluatorReferenceTypeDef]`
4. See [:material-code-braces: CreateOnlineEvaluationConfigResponseTypeDef](./type_defs.md#createonlineevaluationconfigresponsetypedef)


```python
# create_online_evaluation_config method usage example with argument unpacking

kwargs: CreateOnlineEvaluationConfigRequestTypeDef = {  # (1)
    "onlineEvaluationConfigName": ...,
    "rule": ...,
    "dataSourceConfig": ...,
    "evaluators": ...,
    "evaluationExecutionRoleArn": ...,
    "enableOnCreate": ...,
}

parent.create_online_evaluation_config(**kwargs)
```

1. See [:material-code-braces: CreateOnlineEvaluationConfigRequestTypeDef](./type_defs.md#createonlineevaluationconfigrequesttypedef)

### create\_policy

Creates a policy within the AgentCore Policy system.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").create_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/create_policy.html)

```python
# create_policy method definition

await def create_policy(
    self,
    *,
    name: str,
    definition: PolicyDefinitionTypeDef,  # (1)
    policyEngineId: str,
    description: str = ...,
    validationMode: PolicyValidationModeType = ...,  # (2)
    clientToken: str = ...,
) -> CreatePolicyResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: PolicyDefinitionTypeDef](./type_defs.md#policydefinitiontypedef)
2. See [:material-code-brackets: PolicyValidationModeType](./literals.md#policyvalidationmodetype)
3. See [:material-code-braces: CreatePolicyResponseTypeDef](./type_defs.md#createpolicyresponsetypedef)


```python
# create_policy method usage example with argument unpacking

kwargs: CreatePolicyRequestTypeDef = {  # (1)
    "name": ...,
    "definition": ...,
    "policyEngineId": ...,
}

parent.create_policy(**kwargs)
```

1. See [:material-code-braces: CreatePolicyRequestTypeDef](./type_defs.md#createpolicyrequesttypedef)

### create\_policy\_engine

Creates a new policy engine within the AgentCore Policy system.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").create_policy_engine` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/create_policy_engine.html)

```python
# create_policy_engine method definition

await def create_policy_engine(
    self,
    *,
    name: str,
    description: str = ...,
    clientToken: str = ...,
) -> CreatePolicyEngineResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreatePolicyEngineResponseTypeDef](./type_defs.md#createpolicyengineresponsetypedef)


```python
# create_policy_engine method usage example with argument unpacking

kwargs: CreatePolicyEngineRequestTypeDef = {  # (1)
    "name": ...,
}

parent.create_policy_engine(**kwargs)
```

1. See [:material-code-braces: CreatePolicyEngineRequestTypeDef](./type_defs.md#createpolicyenginerequesttypedef)

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
    tags: Mapping[str, str] = ...,
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

Deletes an Amazon Bedrock AgentCore Runtime.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").delete_agent_runtime` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/delete_agent_runtime.html)

```python
# delete_agent_runtime method definition

await def delete_agent_runtime(
    self,
    *,
    agentRuntimeId: str,
    clientToken: str = ...,
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

Deletes an AAgentCore Runtime endpoint.

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
) -> dict[str, Any]:
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

### delete\_evaluator

Deletes a custom evaluator.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").delete_evaluator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/delete_evaluator.html)

```python
# delete_evaluator method definition

await def delete_evaluator(
    self,
    *,
    evaluatorId: str,
) -> DeleteEvaluatorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteEvaluatorResponseTypeDef](./type_defs.md#deleteevaluatorresponsetypedef)


```python
# delete_evaluator method usage example with argument unpacking

kwargs: DeleteEvaluatorRequestTypeDef = {  # (1)
    "evaluatorId": ...,
}

parent.delete_evaluator(**kwargs)
```

1. See [:material-code-braces: DeleteEvaluatorRequestTypeDef](./type_defs.md#deleteevaluatorrequesttypedef)

### delete\_gateway

Deletes a gateway.

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

Deletes a gateway target.

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

Deletes an Amazon Bedrock AgentCore Memory resource.

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
) -> dict[str, Any]:
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

### delete\_online\_evaluation\_config

Deletes an online evaluation configuration and stops any ongoing evaluation
processes associated with it.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").delete_online_evaluation_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/delete_online_evaluation_config.html)

```python
# delete_online_evaluation_config method definition

await def delete_online_evaluation_config(
    self,
    *,
    onlineEvaluationConfigId: str,
) -> DeleteOnlineEvaluationConfigResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteOnlineEvaluationConfigResponseTypeDef](./type_defs.md#deleteonlineevaluationconfigresponsetypedef)


```python
# delete_online_evaluation_config method usage example with argument unpacking

kwargs: DeleteOnlineEvaluationConfigRequestTypeDef = {  # (1)
    "onlineEvaluationConfigId": ...,
}

parent.delete_online_evaluation_config(**kwargs)
```

1. See [:material-code-braces: DeleteOnlineEvaluationConfigRequestTypeDef](./type_defs.md#deleteonlineevaluationconfigrequesttypedef)

### delete\_policy

Deletes an existing policy from the AgentCore Policy system.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").delete_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/delete_policy.html)

```python
# delete_policy method definition

await def delete_policy(
    self,
    *,
    policyEngineId: str,
    policyId: str,
) -> DeletePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeletePolicyResponseTypeDef](./type_defs.md#deletepolicyresponsetypedef)


```python
# delete_policy method usage example with argument unpacking

kwargs: DeletePolicyRequestTypeDef = {  # (1)
    "policyEngineId": ...,
    "policyId": ...,
}

parent.delete_policy(**kwargs)
```

1. See [:material-code-braces: DeletePolicyRequestTypeDef](./type_defs.md#deletepolicyrequesttypedef)

### delete\_policy\_engine

Deletes an existing policy engine from the AgentCore Policy system.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").delete_policy_engine` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/delete_policy_engine.html)

```python
# delete_policy_engine method definition

await def delete_policy_engine(
    self,
    *,
    policyEngineId: str,
) -> DeletePolicyEngineResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeletePolicyEngineResponseTypeDef](./type_defs.md#deletepolicyengineresponsetypedef)


```python
# delete_policy_engine method usage example with argument unpacking

kwargs: DeletePolicyEngineRequestTypeDef = {  # (1)
    "policyEngineId": ...,
}

parent.delete_policy_engine(**kwargs)
```

1. See [:material-code-braces: DeletePolicyEngineRequestTypeDef](./type_defs.md#deletepolicyenginerequesttypedef)

### delete\_resource\_policy

Deletes the resource-based policy for a specified resource.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").delete_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/delete_resource_policy.html)

```python
# delete_resource_policy method definition

await def delete_resource_policy(
    self,
    *,
    resourceArn: str,
) -> dict[str, Any]:
    ...
```

```python
# delete_resource_policy method usage example with argument unpacking

kwargs: DeleteResourcePolicyRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.delete_resource_policy(**kwargs)
```

1. See [:material-code-braces: DeleteResourcePolicyRequestTypeDef](./type_defs.md#deleteresourcepolicyrequesttypedef)

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
) -> dict[str, Any]:
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

Gets an Amazon Bedrock AgentCore Runtime.

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

### get\_evaluator

Retrieves detailed information about an evaluator, including its configuration,
status, and metadata.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").get_evaluator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/get_evaluator.html)

```python
# get_evaluator method definition

await def get_evaluator(
    self,
    *,
    evaluatorId: str,
) -> GetEvaluatorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEvaluatorResponseTypeDef](./type_defs.md#getevaluatorresponsetypedef)


```python
# get_evaluator method usage example with argument unpacking

kwargs: GetEvaluatorRequestTypeDef = {  # (1)
    "evaluatorId": ...,
}

parent.get_evaluator(**kwargs)
```

1. See [:material-code-braces: GetEvaluatorRequestTypeDef](./type_defs.md#getevaluatorrequesttypedef)

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

Retrieves information about a specific gateway target.

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

Retrieve an existing Amazon Bedrock AgentCore Memory resource.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").get_memory` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/get_memory.html)

```python
# get_memory method definition

await def get_memory(
    self,
    *,
    memoryId: str,
    view: MemoryViewType = ...,  # (1)
) -> GetMemoryOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: MemoryViewType](./literals.md#memoryviewtype)
2. See [:material-code-braces: GetMemoryOutputTypeDef](./type_defs.md#getmemoryoutputtypedef)


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

### get\_online\_evaluation\_config

Retrieves detailed information about an online evaluation configuration,
including its rules, data sources, evaluators, and execution status.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").get_online_evaluation_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/get_online_evaluation_config.html)

```python
# get_online_evaluation_config method definition

await def get_online_evaluation_config(
    self,
    *,
    onlineEvaluationConfigId: str,
) -> GetOnlineEvaluationConfigResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOnlineEvaluationConfigResponseTypeDef](./type_defs.md#getonlineevaluationconfigresponsetypedef)


```python
# get_online_evaluation_config method usage example with argument unpacking

kwargs: GetOnlineEvaluationConfigRequestTypeDef = {  # (1)
    "onlineEvaluationConfigId": ...,
}

parent.get_online_evaluation_config(**kwargs)
```

1. See [:material-code-braces: GetOnlineEvaluationConfigRequestTypeDef](./type_defs.md#getonlineevaluationconfigrequesttypedef)

### get\_policy

Retrieves detailed information about a specific policy within the AgentCore
Policy system.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").get_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/get_policy.html)

```python
# get_policy method definition

await def get_policy(
    self,
    *,
    policyEngineId: str,
    policyId: str,
) -> GetPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPolicyResponseTypeDef](./type_defs.md#getpolicyresponsetypedef)


```python
# get_policy method usage example with argument unpacking

kwargs: GetPolicyRequestTypeDef = {  # (1)
    "policyEngineId": ...,
    "policyId": ...,
}

parent.get_policy(**kwargs)
```

1. See [:material-code-braces: GetPolicyRequestTypeDef](./type_defs.md#getpolicyrequesttypedef)

### get\_policy\_engine

Retrieves detailed information about a specific policy engine within the
AgentCore Policy system.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").get_policy_engine` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/get_policy_engine.html)

```python
# get_policy_engine method definition

await def get_policy_engine(
    self,
    *,
    policyEngineId: str,
) -> GetPolicyEngineResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPolicyEngineResponseTypeDef](./type_defs.md#getpolicyengineresponsetypedef)


```python
# get_policy_engine method usage example with argument unpacking

kwargs: GetPolicyEngineRequestTypeDef = {  # (1)
    "policyEngineId": ...,
}

parent.get_policy_engine(**kwargs)
```

1. See [:material-code-braces: GetPolicyEngineRequestTypeDef](./type_defs.md#getpolicyenginerequesttypedef)

### get\_policy\_generation

Retrieves information about a policy generation request within the AgentCore
Policy system.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").get_policy_generation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/get_policy_generation.html)

```python
# get_policy_generation method definition

await def get_policy_generation(
    self,
    *,
    policyGenerationId: str,
    policyEngineId: str,
) -> GetPolicyGenerationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPolicyGenerationResponseTypeDef](./type_defs.md#getpolicygenerationresponsetypedef)


```python
# get_policy_generation method usage example with argument unpacking

kwargs: GetPolicyGenerationRequestTypeDef = {  # (1)
    "policyGenerationId": ...,
    "policyEngineId": ...,
}

parent.get_policy_generation(**kwargs)
```

1. See [:material-code-braces: GetPolicyGenerationRequestTypeDef](./type_defs.md#getpolicygenerationrequesttypedef)

### get\_resource\_policy

Retrieves the resource-based policy for a specified resource.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").get_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/get_resource_policy.html)

```python
# get_resource_policy method definition

await def get_resource_policy(
    self,
    *,
    resourceArn: str,
) -> GetResourcePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResourcePolicyResponseTypeDef](./type_defs.md#getresourcepolicyresponsetypedef)


```python
# get_resource_policy method usage example with argument unpacking

kwargs: GetResourcePolicyRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.get_resource_policy(**kwargs)
```

1. See [:material-code-braces: GetResourcePolicyRequestTypeDef](./type_defs.md#getresourcepolicyrequesttypedef)

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

### list\_evaluators

Lists all available evaluators, including both builtin evaluators provided by
the service and custom evaluators created by the user.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").list_evaluators` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/list_evaluators.html)

```python
# list_evaluators method definition

await def list_evaluators(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListEvaluatorsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEvaluatorsResponseTypeDef](./type_defs.md#listevaluatorsresponsetypedef)


```python
# list_evaluators method usage example with argument unpacking

kwargs: ListEvaluatorsRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_evaluators(**kwargs)
```

1. See [:material-code-braces: ListEvaluatorsRequestTypeDef](./type_defs.md#listevaluatorsrequesttypedef)

### list\_gateway\_targets

Lists all targets for a specific gateway.

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

Lists all gateways in the account.

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

Lists the available Amazon Bedrock AgentCore Memory resources in the current
Amazon Web Services Region.

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

### list\_online\_evaluation\_configs

Lists all online evaluation configurations in the account, providing summary
information about each configuration's status and settings.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").list_online_evaluation_configs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/list_online_evaluation_configs.html)

```python
# list_online_evaluation_configs method definition

await def list_online_evaluation_configs(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListOnlineEvaluationConfigsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListOnlineEvaluationConfigsResponseTypeDef](./type_defs.md#listonlineevaluationconfigsresponsetypedef)


```python
# list_online_evaluation_configs method usage example with argument unpacking

kwargs: ListOnlineEvaluationConfigsRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_online_evaluation_configs(**kwargs)
```

1. See [:material-code-braces: ListOnlineEvaluationConfigsRequestTypeDef](./type_defs.md#listonlineevaluationconfigsrequesttypedef)

### list\_policies

Retrieves a list of policies within the AgentCore Policy engine.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").list_policies` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/list_policies.html)

```python
# list_policies method definition

await def list_policies(
    self,
    *,
    policyEngineId: str,
    nextToken: str = ...,
    maxResults: int = ...,
    targetResourceScope: str = ...,
) -> ListPoliciesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPoliciesResponseTypeDef](./type_defs.md#listpoliciesresponsetypedef)


```python
# list_policies method usage example with argument unpacking

kwargs: ListPoliciesRequestTypeDef = {  # (1)
    "policyEngineId": ...,
}

parent.list_policies(**kwargs)
```

1. See [:material-code-braces: ListPoliciesRequestTypeDef](./type_defs.md#listpoliciesrequesttypedef)

### list\_policy\_engines

Retrieves a list of policy engines within the AgentCore Policy system.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").list_policy_engines` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/list_policy_engines.html)

```python
# list_policy_engines method definition

await def list_policy_engines(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListPolicyEnginesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPolicyEnginesResponseTypeDef](./type_defs.md#listpolicyenginesresponsetypedef)


```python
# list_policy_engines method usage example with argument unpacking

kwargs: ListPolicyEnginesRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_policy_engines(**kwargs)
```

1. See [:material-code-braces: ListPolicyEnginesRequestTypeDef](./type_defs.md#listpolicyenginesrequesttypedef)

### list\_policy\_generation\_assets

Retrieves a list of generated policy assets from a policy generation request
within the AgentCore Policy system.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").list_policy_generation_assets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/list_policy_generation_assets.html)

```python
# list_policy_generation_assets method definition

await def list_policy_generation_assets(
    self,
    *,
    policyGenerationId: str,
    policyEngineId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListPolicyGenerationAssetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPolicyGenerationAssetsResponseTypeDef](./type_defs.md#listpolicygenerationassetsresponsetypedef)


```python
# list_policy_generation_assets method usage example with argument unpacking

kwargs: ListPolicyGenerationAssetsRequestTypeDef = {  # (1)
    "policyGenerationId": ...,
    "policyEngineId": ...,
}

parent.list_policy_generation_assets(**kwargs)
```

1. See [:material-code-braces: ListPolicyGenerationAssetsRequestTypeDef](./type_defs.md#listpolicygenerationassetsrequesttypedef)

### list\_policy\_generations

Retrieves a list of policy generation requests within the AgentCore Policy
system.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").list_policy_generations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/list_policy_generations.html)

```python
# list_policy_generations method definition

await def list_policy_generations(
    self,
    *,
    policyEngineId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListPolicyGenerationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPolicyGenerationsResponseTypeDef](./type_defs.md#listpolicygenerationsresponsetypedef)


```python
# list_policy_generations method usage example with argument unpacking

kwargs: ListPolicyGenerationsRequestTypeDef = {  # (1)
    "policyEngineId": ...,
}

parent.list_policy_generations(**kwargs)
```

1. See [:material-code-braces: ListPolicyGenerationsRequestTypeDef](./type_defs.md#listpolicygenerationsrequesttypedef)

### list\_tags\_for\_resource

Lists the tags associated with the specified resource.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/list_tags_for_resource.html)

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

### put\_resource\_policy

Creates or updates a resource-based policy for a resource with the specified
resourceArn.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").put_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/put_resource_policy.html)

```python
# put_resource_policy method definition

await def put_resource_policy(
    self,
    *,
    resourceArn: str,
    policy: str,
) -> PutResourcePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutResourcePolicyResponseTypeDef](./type_defs.md#putresourcepolicyresponsetypedef)


```python
# put_resource_policy method usage example with argument unpacking

kwargs: PutResourcePolicyRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "policy": ...,
}

parent.put_resource_policy(**kwargs)
```

1. See [:material-code-braces: PutResourcePolicyRequestTypeDef](./type_defs.md#putresourcepolicyrequesttypedef)

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

### start\_policy\_generation

Initiates the AI-powered generation of Cedar policies from natural language
descriptions within the AgentCore Policy system.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").start_policy_generation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/start_policy_generation.html)

```python
# start_policy_generation method definition

await def start_policy_generation(
    self,
    *,
    policyEngineId: str,
    resource: ResourceTypeDef,  # (1)
    content: ContentTypeDef,  # (2)
    name: str,
    clientToken: str = ...,
) -> StartPolicyGenerationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef)
2. See [:material-code-braces: ContentTypeDef](./type_defs.md#contenttypedef)
3. See [:material-code-braces: StartPolicyGenerationResponseTypeDef](./type_defs.md#startpolicygenerationresponsetypedef)


```python
# start_policy_generation method usage example with argument unpacking

kwargs: StartPolicyGenerationRequestTypeDef = {  # (1)
    "policyEngineId": ...,
    "resource": ...,
    "content": ...,
    "name": ...,
}

parent.start_policy_generation(**kwargs)
```

1. See [:material-code-braces: StartPolicyGenerationRequestTypeDef](./type_defs.md#startpolicygenerationrequesttypedef)

### synchronize\_gateway\_targets

The gateway targets.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").synchronize_gateway_targets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/synchronize_gateway_targets.html)

```python
# synchronize_gateway_targets method definition

await def synchronize_gateway_targets(
    self,
    *,
    gatewayIdentifier: str,
    targetIdList: Sequence[str],
) -> SynchronizeGatewayTargetsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SynchronizeGatewayTargetsResponseTypeDef](./type_defs.md#synchronizegatewaytargetsresponsetypedef)


```python
# synchronize_gateway_targets method usage example with argument unpacking

kwargs: SynchronizeGatewayTargetsRequestTypeDef = {  # (1)
    "gatewayIdentifier": ...,
    "targetIdList": ...,
}

parent.synchronize_gateway_targets(**kwargs)
```

1. See [:material-code-braces: SynchronizeGatewayTargetsRequestTypeDef](./type_defs.md#synchronizegatewaytargetsrequesttypedef)

### tag\_resource

Associates the specified tags to a resource with the specified resourceArn.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/tag_resource.html)

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

Removes the specified tags from the specified resource.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/untag_resource.html)

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
    agentRuntimeArtifact: AgentRuntimeArtifactUnionTypeDef,  # (1)
    roleArn: str,
    networkConfiguration: NetworkConfigurationUnionTypeDef,  # (2)
    description: str = ...,
    authorizerConfiguration: AuthorizerConfigurationUnionTypeDef = ...,  # (3)
    requestHeaderConfiguration: RequestHeaderConfigurationUnionTypeDef = ...,  # (4)
    protocolConfiguration: ProtocolConfigurationTypeDef = ...,  # (5)
    lifecycleConfiguration: LifecycleConfigurationTypeDef = ...,  # (6)
    environmentVariables: Mapping[str, str] = ...,
    clientToken: str = ...,
) -> UpdateAgentRuntimeResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: AgentRuntimeArtifactUnionTypeDef](#agentruntimeartifactuniontypedef)
2. See [:material-code-braces: NetworkConfigurationUnionTypeDef](#networkconfigurationuniontypedef)
3. See [:material-code-braces: AuthorizerConfigurationUnionTypeDef](#authorizerconfigurationuniontypedef)
4. See [:material-code-braces: RequestHeaderConfigurationUnionTypeDef](#requestheaderconfigurationuniontypedef)
5. See [:material-code-braces: ProtocolConfigurationTypeDef](./type_defs.md#protocolconfigurationtypedef)
6. See [:material-code-braces: LifecycleConfigurationTypeDef](./type_defs.md#lifecycleconfigurationtypedef)
7. See [:material-code-braces: UpdateAgentRuntimeResponseTypeDef](./type_defs.md#updateagentruntimeresponsetypedef)


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

Updates an existing Amazon Bedrock AgentCore Runtime endpoint.

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

### update\_evaluator

Updates a custom evaluator's configuration, description, or evaluation level.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").update_evaluator` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/update_evaluator.html)

```python
# update_evaluator method definition

await def update_evaluator(
    self,
    *,
    evaluatorId: str,
    clientToken: str = ...,
    description: str = ...,
    evaluatorConfig: EvaluatorConfigUnionTypeDef = ...,  # (1)
    level: EvaluatorLevelType = ...,  # (2)
) -> UpdateEvaluatorResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: EvaluatorConfigUnionTypeDef](#evaluatorconfiguniontypedef)
2. See [:material-code-brackets: EvaluatorLevelType](./literals.md#evaluatorleveltype)
3. See [:material-code-braces: UpdateEvaluatorResponseTypeDef](./type_defs.md#updateevaluatorresponsetypedef)


```python
# update_evaluator method usage example with argument unpacking

kwargs: UpdateEvaluatorRequestTypeDef = {  # (1)
    "evaluatorId": ...,
}

parent.update_evaluator(**kwargs)
```

1. See [:material-code-braces: UpdateEvaluatorRequestTypeDef](./type_defs.md#updateevaluatorrequesttypedef)

### update\_gateway

Updates an existing gateway.

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
    description: str = ...,
    protocolConfiguration: GatewayProtocolConfigurationUnionTypeDef = ...,  # (3)
    authorizerConfiguration: AuthorizerConfigurationUnionTypeDef = ...,  # (4)
    kmsKeyArn: str = ...,
    interceptorConfigurations: Sequence[GatewayInterceptorConfigurationUnionTypeDef] = ...,  # (5)
    policyEngineConfiguration: GatewayPolicyEngineConfigurationTypeDef = ...,  # (6)
    exceptionLevel: ExceptionLevelType = ...,  # (7)
) -> UpdateGatewayResponseTypeDef:  # (8)
    ...
```

1. See [:material-code-brackets: GatewayProtocolTypeType](./literals.md#gatewayprotocoltypetype)
2. See [:material-code-brackets: AuthorizerTypeType](./literals.md#authorizertypetype)
3. See [:material-code-braces: GatewayProtocolConfigurationUnionTypeDef](#gatewayprotocolconfigurationuniontypedef)
4. See [:material-code-braces: AuthorizerConfigurationUnionTypeDef](#authorizerconfigurationuniontypedef)
5. See `Sequence[GatewayInterceptorConfigurationUnionTypeDef]`
6. See [:material-code-braces: GatewayPolicyEngineConfigurationTypeDef](./type_defs.md#gatewaypolicyengineconfigurationtypedef)
7. See [:material-code-brackets: ExceptionLevelType](./literals.md#exceptionleveltype)
8. See [:material-code-braces: UpdateGatewayResponseTypeDef](./type_defs.md#updategatewayresponsetypedef)


```python
# update_gateway method usage example with argument unpacking

kwargs: UpdateGatewayRequestTypeDef = {  # (1)
    "gatewayIdentifier": ...,
    "name": ...,
    "roleArn": ...,
    "protocolType": ...,
    "authorizerType": ...,
}

parent.update_gateway(**kwargs)
```

1. See [:material-code-braces: UpdateGatewayRequestTypeDef](./type_defs.md#updategatewayrequesttypedef)

### update\_gateway\_target

Updates an existing gateway target.

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
    description: str = ...,
    credentialProviderConfigurations: Sequence[CredentialProviderConfigurationUnionTypeDef] = ...,  # (2)
    metadataConfiguration: MetadataConfigurationUnionTypeDef = ...,  # (3)
) -> UpdateGatewayTargetResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: TargetConfigurationUnionTypeDef](#targetconfigurationuniontypedef)
2. See `Sequence[CredentialProviderConfigurationUnionTypeDef]`
3. See [:material-code-braces: MetadataConfigurationUnionTypeDef](#metadataconfigurationuniontypedef)
4. See [:material-code-braces: UpdateGatewayTargetResponseTypeDef](./type_defs.md#updategatewaytargetresponsetypedef)


```python
# update_gateway_target method usage example with argument unpacking

kwargs: UpdateGatewayTargetRequestTypeDef = {  # (1)
    "gatewayIdentifier": ...,
    "targetId": ...,
    "name": ...,
    "targetConfiguration": ...,
}

parent.update_gateway_target(**kwargs)
```

1. See [:material-code-braces: UpdateGatewayTargetRequestTypeDef](./type_defs.md#updategatewaytargetrequesttypedef)

### update\_memory

Update an Amazon Bedrock AgentCore Memory resource memory.

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

### update\_online\_evaluation\_config

Updates an online evaluation configuration's settings, including rules, data
sources, evaluators, and execution status.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").update_online_evaluation_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/update_online_evaluation_config.html)

```python
# update_online_evaluation_config method definition

await def update_online_evaluation_config(
    self,
    *,
    onlineEvaluationConfigId: str,
    clientToken: str = ...,
    description: str = ...,
    rule: RuleUnionTypeDef = ...,  # (1)
    dataSourceConfig: DataSourceConfigUnionTypeDef = ...,  # (2)
    evaluators: Sequence[EvaluatorReferenceTypeDef] = ...,  # (3)
    evaluationExecutionRoleArn: str = ...,
    executionStatus: OnlineEvaluationExecutionStatusType = ...,  # (4)
) -> UpdateOnlineEvaluationConfigResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: RuleUnionTypeDef](#ruleuniontypedef)
2. See [:material-code-braces: DataSourceConfigUnionTypeDef](#datasourceconfiguniontypedef)
3. See `Sequence[EvaluatorReferenceTypeDef]`
4. See [:material-code-brackets: OnlineEvaluationExecutionStatusType](./literals.md#onlineevaluationexecutionstatustype)
5. See [:material-code-braces: UpdateOnlineEvaluationConfigResponseTypeDef](./type_defs.md#updateonlineevaluationconfigresponsetypedef)


```python
# update_online_evaluation_config method usage example with argument unpacking

kwargs: UpdateOnlineEvaluationConfigRequestTypeDef = {  # (1)
    "onlineEvaluationConfigId": ...,
}

parent.update_online_evaluation_config(**kwargs)
```

1. See [:material-code-braces: UpdateOnlineEvaluationConfigRequestTypeDef](./type_defs.md#updateonlineevaluationconfigrequesttypedef)

### update\_policy

Updates an existing policy within the AgentCore Policy system.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").update_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/update_policy.html)

```python
# update_policy method definition

await def update_policy(
    self,
    *,
    policyEngineId: str,
    policyId: str,
    definition: PolicyDefinitionTypeDef,  # (1)
    description: str = ...,
    validationMode: PolicyValidationModeType = ...,  # (2)
) -> UpdatePolicyResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: PolicyDefinitionTypeDef](./type_defs.md#policydefinitiontypedef)
2. See [:material-code-brackets: PolicyValidationModeType](./literals.md#policyvalidationmodetype)
3. See [:material-code-braces: UpdatePolicyResponseTypeDef](./type_defs.md#updatepolicyresponsetypedef)


```python
# update_policy method usage example with argument unpacking

kwargs: UpdatePolicyRequestTypeDef = {  # (1)
    "policyEngineId": ...,
    "policyId": ...,
    "definition": ...,
}

parent.update_policy(**kwargs)
```

1. See [:material-code-braces: UpdatePolicyRequestTypeDef](./type_defs.md#updatepolicyrequesttypedef)

### update\_policy\_engine

Updates an existing policy engine within the AgentCore Policy system.

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").update_policy_engine` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control/client/update_policy_engine.html)

```python
# update_policy_engine method definition

await def update_policy_engine(
    self,
    *,
    policyEngineId: str,
    description: str = ...,
) -> UpdatePolicyEngineResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdatePolicyEngineResponseTypeDef](./type_defs.md#updatepolicyengineresponsetypedef)


```python
# update_policy_engine method usage example with argument unpacking

kwargs: UpdatePolicyEngineRequestTypeDef = {  # (1)
    "policyEngineId": ...,
}

parent.update_policy_engine(**kwargs)
```

1. See [:material-code-braces: UpdatePolicyEngineRequestTypeDef](./type_defs.md#updatepolicyenginerequesttypedef)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control.html#BedrockAgentCoreControl.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control.html#BedrockAgentCoreControl.Client)

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

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").get_paginator` method with overloads.

- `client.get_paginator("list_agent_runtime_endpoints")` -> [ListAgentRuntimeEndpointsPaginator](./paginators.md#listagentruntimeendpointspaginator)
- `client.get_paginator("list_agent_runtime_versions")` -> [ListAgentRuntimeVersionsPaginator](./paginators.md#listagentruntimeversionspaginator)
- `client.get_paginator("list_agent_runtimes")` -> [ListAgentRuntimesPaginator](./paginators.md#listagentruntimespaginator)
- `client.get_paginator("list_api_key_credential_providers")` -> [ListApiKeyCredentialProvidersPaginator](./paginators.md#listapikeycredentialproviderspaginator)
- `client.get_paginator("list_browsers")` -> [ListBrowsersPaginator](./paginators.md#listbrowserspaginator)
- `client.get_paginator("list_code_interpreters")` -> [ListCodeInterpretersPaginator](./paginators.md#listcodeinterpreterspaginator)
- `client.get_paginator("list_evaluators")` -> [ListEvaluatorsPaginator](./paginators.md#listevaluatorspaginator)
- `client.get_paginator("list_gateway_targets")` -> [ListGatewayTargetsPaginator](./paginators.md#listgatewaytargetspaginator)
- `client.get_paginator("list_gateways")` -> [ListGatewaysPaginator](./paginators.md#listgatewayspaginator)
- `client.get_paginator("list_memories")` -> [ListMemoriesPaginator](./paginators.md#listmemoriespaginator)
- `client.get_paginator("list_oauth2_credential_providers")` -> [ListOauth2CredentialProvidersPaginator](./paginators.md#listoauth2credentialproviderspaginator)
- `client.get_paginator("list_online_evaluation_configs")` -> [ListOnlineEvaluationConfigsPaginator](./paginators.md#listonlineevaluationconfigspaginator)
- `client.get_paginator("list_policies")` -> [ListPoliciesPaginator](./paginators.md#listpoliciespaginator)
- `client.get_paginator("list_policy_engines")` -> [ListPolicyEnginesPaginator](./paginators.md#listpolicyenginespaginator)
- `client.get_paginator("list_policy_generation_assets")` -> [ListPolicyGenerationAssetsPaginator](./paginators.md#listpolicygenerationassetspaginator)
- `client.get_paginator("list_policy_generations")` -> [ListPolicyGenerationsPaginator](./paginators.md#listpolicygenerationspaginator)
- `client.get_paginator("list_workload_identities")` -> [ListWorkloadIdentitiesPaginator](./paginators.md#listworkloadidentitiespaginator)




### get_waiter

Type annotations and code completion for `#!python session.create_client("bedrock-agentcore-control").get_waiter` method with overloads.

- `client.get_waiter("memory_created")` -> [MemoryCreatedWaiter](./waiters.md#memorycreatedwaiter)
- `client.get_waiter("policy_active")` -> [PolicyActiveWaiter](./waiters.md#policyactivewaiter)
- `client.get_waiter("policy_deleted")` -> [PolicyDeletedWaiter](./waiters.md#policydeletedwaiter)
- `client.get_waiter("policy_engine_active")` -> [PolicyEngineActiveWaiter](./waiters.md#policyengineactivewaiter)
- `client.get_waiter("policy_engine_deleted")` -> [PolicyEngineDeletedWaiter](./waiters.md#policyenginedeletedwaiter)
- `client.get_waiter("policy_generation_completed")` -> [PolicyGenerationCompletedWaiter](./waiters.md#policygenerationcompletedwaiter)

