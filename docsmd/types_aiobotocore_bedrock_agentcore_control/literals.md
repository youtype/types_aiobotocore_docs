# Literals

> [Index](../README.md) > [BedrockAgentCoreControl](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [BedrockAgentCoreControl](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control.html#bedrockagentcorecontrol)
    type annotations stubs module [types-aiobotocore-bedrock-agentcore-control](https://pypi.org/project/types-aiobotocore-bedrock-agentcore-control/).

## AgentManagedRuntimeTypeType

```python
# AgentManagedRuntimeTypeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import AgentManagedRuntimeTypeType

def get_value() -> AgentManagedRuntimeTypeType:
    return "PYTHON_3_10"
```

```python
# AgentManagedRuntimeTypeType definition
AgentManagedRuntimeTypeType = Literal[
    "PYTHON_3_10",
    "PYTHON_3_11",
    "PYTHON_3_12",
    "PYTHON_3_13",
]
```
## AgentRuntimeEndpointStatusType

```python
# AgentRuntimeEndpointStatusType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import AgentRuntimeEndpointStatusType

def get_value() -> AgentRuntimeEndpointStatusType:
    return "CREATE_FAILED"
```

```python
# AgentRuntimeEndpointStatusType definition
AgentRuntimeEndpointStatusType = Literal[
    "CREATE_FAILED",
    "CREATING",
    "DELETING",
    "READY",
    "UPDATE_FAILED",
    "UPDATING",
]
```
## AgentRuntimeStatusType

```python
# AgentRuntimeStatusType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import AgentRuntimeStatusType

def get_value() -> AgentRuntimeStatusType:
    return "CREATE_FAILED"
```

```python
# AgentRuntimeStatusType definition
AgentRuntimeStatusType = Literal[
    "CREATE_FAILED",
    "CREATING",
    "DELETING",
    "READY",
    "UPDATE_FAILED",
    "UPDATING",
]
```
## ApiKeyCredentialLocationType

```python
# ApiKeyCredentialLocationType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ApiKeyCredentialLocationType

def get_value() -> ApiKeyCredentialLocationType:
    return "HEADER"
```

```python
# ApiKeyCredentialLocationType definition
ApiKeyCredentialLocationType = Literal[
    "HEADER",
    "QUERY_PARAMETER",
]
```
## AuthorizerTypeType

```python
# AuthorizerTypeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import AuthorizerTypeType

def get_value() -> AuthorizerTypeType:
    return "AWS_IAM"
```

```python
# AuthorizerTypeType definition
AuthorizerTypeType = Literal[
    "AWS_IAM",
    "CUSTOM_JWT",
    "NONE",
]
```
## BrowserNetworkModeType

```python
# BrowserNetworkModeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import BrowserNetworkModeType

def get_value() -> BrowserNetworkModeType:
    return "PUBLIC"
```

```python
# BrowserNetworkModeType definition
BrowserNetworkModeType = Literal[
    "PUBLIC",
    "VPC",
]
```
## BrowserStatusType

```python
# BrowserStatusType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import BrowserStatusType

def get_value() -> BrowserStatusType:
    return "CREATE_FAILED"
```

```python
# BrowserStatusType definition
BrowserStatusType = Literal[
    "CREATE_FAILED",
    "CREATING",
    "DELETE_FAILED",
    "DELETED",
    "DELETING",
    "READY",
]
```
## ClaimMatchOperatorTypeType

```python
# ClaimMatchOperatorTypeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ClaimMatchOperatorTypeType

def get_value() -> ClaimMatchOperatorTypeType:
    return "CONTAINS"
```

```python
# ClaimMatchOperatorTypeType definition
ClaimMatchOperatorTypeType = Literal[
    "CONTAINS",
    "CONTAINS_ANY",
    "EQUALS",
]
```
## CodeInterpreterNetworkModeType

```python
# CodeInterpreterNetworkModeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import CodeInterpreterNetworkModeType

def get_value() -> CodeInterpreterNetworkModeType:
    return "PUBLIC"
```

```python
# CodeInterpreterNetworkModeType definition
CodeInterpreterNetworkModeType = Literal[
    "PUBLIC",
    "SANDBOX",
    "VPC",
]
```
## CodeInterpreterStatusType

```python
# CodeInterpreterStatusType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import CodeInterpreterStatusType

def get_value() -> CodeInterpreterStatusType:
    return "CREATE_FAILED"
```

```python
# CodeInterpreterStatusType definition
CodeInterpreterStatusType = Literal[
    "CREATE_FAILED",
    "CREATING",
    "DELETE_FAILED",
    "DELETED",
    "DELETING",
    "READY",
]
```
## CredentialProviderTypeType

```python
# CredentialProviderTypeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import CredentialProviderTypeType

def get_value() -> CredentialProviderTypeType:
    return "API_KEY"
```

```python
# CredentialProviderTypeType definition
CredentialProviderTypeType = Literal[
    "API_KEY",
    "GATEWAY_IAM_ROLE",
    "OAUTH",
]
```
## CredentialProviderVendorTypeType

```python
# CredentialProviderVendorTypeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import CredentialProviderVendorTypeType

def get_value() -> CredentialProviderVendorTypeType:
    return "AtlassianOauth2"
```

```python
# CredentialProviderVendorTypeType definition
CredentialProviderVendorTypeType = Literal[
    "AtlassianOauth2",
    "Auth0Oauth2",
    "CognitoOauth2",
    "CustomOauth2",
    "CyberArkOauth2",
    "DropboxOauth2",
    "FacebookOauth2",
    "FusionAuthOauth2",
    "GithubOauth2",
    "GoogleOauth2",
    "HubspotOauth2",
    "LinkedinOauth2",
    "MicrosoftOauth2",
    "NotionOauth2",
    "OktaOauth2",
    "OneLoginOauth2",
    "PingOneOauth2",
    "RedditOauth2",
    "SalesforceOauth2",
    "SlackOauth2",
    "SpotifyOauth2",
    "TwitchOauth2",
    "XOauth2",
    "YandexOauth2",
    "ZoomOauth2",
]
```
## EvaluatorLevelType

```python
# EvaluatorLevelType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import EvaluatorLevelType

def get_value() -> EvaluatorLevelType:
    return "SESSION"
```

```python
# EvaluatorLevelType definition
EvaluatorLevelType = Literal[
    "SESSION",
    "TOOL_CALL",
    "TRACE",
]
```
## EvaluatorStatusType

```python
# EvaluatorStatusType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import EvaluatorStatusType

def get_value() -> EvaluatorStatusType:
    return "ACTIVE"
```

```python
# EvaluatorStatusType definition
EvaluatorStatusType = Literal[
    "ACTIVE",
    "CREATE_FAILED",
    "CREATING",
    "DELETING",
    "UPDATE_FAILED",
    "UPDATING",
]
```
## EvaluatorTypeType

```python
# EvaluatorTypeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import EvaluatorTypeType

def get_value() -> EvaluatorTypeType:
    return "Builtin"
```

```python
# EvaluatorTypeType definition
EvaluatorTypeType = Literal[
    "Builtin",
    "Custom",
]
```
## ExceptionLevelType

```python
# ExceptionLevelType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ExceptionLevelType

def get_value() -> ExceptionLevelType:
    return "DEBUG"
```

```python
# ExceptionLevelType definition
ExceptionLevelType = Literal[
    "DEBUG",
]
```
## FilterOperatorType

```python
# FilterOperatorType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import FilterOperatorType

def get_value() -> FilterOperatorType:
    return "Contains"
```

```python
# FilterOperatorType definition
FilterOperatorType = Literal[
    "Contains",
    "Equals",
    "GreaterThan",
    "GreaterThanOrEqual",
    "LessThan",
    "LessThanOrEqual",
    "NotContains",
    "NotEquals",
]
```
## FindingTypeType

```python
# FindingTypeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import FindingTypeType

def get_value() -> FindingTypeType:
    return "ALLOW_ALL"
```

```python
# FindingTypeType definition
FindingTypeType = Literal[
    "ALLOW_ALL",
    "ALLOW_NONE",
    "DENY_ALL",
    "DENY_NONE",
    "INVALID",
    "NOT_TRANSLATABLE",
    "VALID",
]
```
## GatewayInterceptionPointType

```python
# GatewayInterceptionPointType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import GatewayInterceptionPointType

def get_value() -> GatewayInterceptionPointType:
    return "REQUEST"
```

```python
# GatewayInterceptionPointType definition
GatewayInterceptionPointType = Literal[
    "REQUEST",
    "RESPONSE",
]
```
## GatewayPolicyEngineModeType

```python
# GatewayPolicyEngineModeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import GatewayPolicyEngineModeType

def get_value() -> GatewayPolicyEngineModeType:
    return "ENFORCE"
```

```python
# GatewayPolicyEngineModeType definition
GatewayPolicyEngineModeType = Literal[
    "ENFORCE",
    "LOG_ONLY",
]
```
## GatewayProtocolTypeType

```python
# GatewayProtocolTypeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import GatewayProtocolTypeType

def get_value() -> GatewayProtocolTypeType:
    return "MCP"
```

```python
# GatewayProtocolTypeType definition
GatewayProtocolTypeType = Literal[
    "MCP",
]
```
## GatewayStatusType

```python
# GatewayStatusType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import GatewayStatusType

def get_value() -> GatewayStatusType:
    return "CREATING"
```

```python
# GatewayStatusType definition
GatewayStatusType = Literal[
    "CREATING",
    "DELETING",
    "FAILED",
    "READY",
    "UPDATE_UNSUCCESSFUL",
    "UPDATING",
]
```
## InboundTokenClaimValueTypeType

```python
# InboundTokenClaimValueTypeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import InboundTokenClaimValueTypeType

def get_value() -> InboundTokenClaimValueTypeType:
    return "STRING"
```

```python
# InboundTokenClaimValueTypeType definition
InboundTokenClaimValueTypeType = Literal[
    "STRING",
    "STRING_ARRAY",
]
```
## KeyTypeType

```python
# KeyTypeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import KeyTypeType

def get_value() -> KeyTypeType:
    return "CustomerManagedKey"
```

```python
# KeyTypeType definition
KeyTypeType = Literal[
    "CustomerManagedKey",
    "ServiceManagedKey",
]
```
## ListAgentRuntimeEndpointsPaginatorName

```python
# ListAgentRuntimeEndpointsPaginatorName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ListAgentRuntimeEndpointsPaginatorName

def get_value() -> ListAgentRuntimeEndpointsPaginatorName:
    return "list_agent_runtime_endpoints"
```

```python
# ListAgentRuntimeEndpointsPaginatorName definition
ListAgentRuntimeEndpointsPaginatorName = Literal[
    "list_agent_runtime_endpoints",
]
```
## ListAgentRuntimeVersionsPaginatorName

```python
# ListAgentRuntimeVersionsPaginatorName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ListAgentRuntimeVersionsPaginatorName

def get_value() -> ListAgentRuntimeVersionsPaginatorName:
    return "list_agent_runtime_versions"
```

```python
# ListAgentRuntimeVersionsPaginatorName definition
ListAgentRuntimeVersionsPaginatorName = Literal[
    "list_agent_runtime_versions",
]
```
## ListAgentRuntimesPaginatorName

```python
# ListAgentRuntimesPaginatorName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ListAgentRuntimesPaginatorName

def get_value() -> ListAgentRuntimesPaginatorName:
    return "list_agent_runtimes"
```

```python
# ListAgentRuntimesPaginatorName definition
ListAgentRuntimesPaginatorName = Literal[
    "list_agent_runtimes",
]
```
## ListApiKeyCredentialProvidersPaginatorName

```python
# ListApiKeyCredentialProvidersPaginatorName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ListApiKeyCredentialProvidersPaginatorName

def get_value() -> ListApiKeyCredentialProvidersPaginatorName:
    return "list_api_key_credential_providers"
```

```python
# ListApiKeyCredentialProvidersPaginatorName definition
ListApiKeyCredentialProvidersPaginatorName = Literal[
    "list_api_key_credential_providers",
]
```
## ListBrowsersPaginatorName

```python
# ListBrowsersPaginatorName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ListBrowsersPaginatorName

def get_value() -> ListBrowsersPaginatorName:
    return "list_browsers"
```

```python
# ListBrowsersPaginatorName definition
ListBrowsersPaginatorName = Literal[
    "list_browsers",
]
```
## ListCodeInterpretersPaginatorName

```python
# ListCodeInterpretersPaginatorName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ListCodeInterpretersPaginatorName

def get_value() -> ListCodeInterpretersPaginatorName:
    return "list_code_interpreters"
```

```python
# ListCodeInterpretersPaginatorName definition
ListCodeInterpretersPaginatorName = Literal[
    "list_code_interpreters",
]
```
## ListEvaluatorsPaginatorName

```python
# ListEvaluatorsPaginatorName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ListEvaluatorsPaginatorName

def get_value() -> ListEvaluatorsPaginatorName:
    return "list_evaluators"
```

```python
# ListEvaluatorsPaginatorName definition
ListEvaluatorsPaginatorName = Literal[
    "list_evaluators",
]
```
## ListGatewayTargetsPaginatorName

```python
# ListGatewayTargetsPaginatorName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ListGatewayTargetsPaginatorName

def get_value() -> ListGatewayTargetsPaginatorName:
    return "list_gateway_targets"
```

```python
# ListGatewayTargetsPaginatorName definition
ListGatewayTargetsPaginatorName = Literal[
    "list_gateway_targets",
]
```
## ListGatewaysPaginatorName

```python
# ListGatewaysPaginatorName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ListGatewaysPaginatorName

def get_value() -> ListGatewaysPaginatorName:
    return "list_gateways"
```

```python
# ListGatewaysPaginatorName definition
ListGatewaysPaginatorName = Literal[
    "list_gateways",
]
```
## ListMemoriesPaginatorName

```python
# ListMemoriesPaginatorName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ListMemoriesPaginatorName

def get_value() -> ListMemoriesPaginatorName:
    return "list_memories"
```

```python
# ListMemoriesPaginatorName definition
ListMemoriesPaginatorName = Literal[
    "list_memories",
]
```
## ListOauth2CredentialProvidersPaginatorName

```python
# ListOauth2CredentialProvidersPaginatorName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ListOauth2CredentialProvidersPaginatorName

def get_value() -> ListOauth2CredentialProvidersPaginatorName:
    return "list_oauth2_credential_providers"
```

```python
# ListOauth2CredentialProvidersPaginatorName definition
ListOauth2CredentialProvidersPaginatorName = Literal[
    "list_oauth2_credential_providers",
]
```
## ListOnlineEvaluationConfigsPaginatorName

```python
# ListOnlineEvaluationConfigsPaginatorName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ListOnlineEvaluationConfigsPaginatorName

def get_value() -> ListOnlineEvaluationConfigsPaginatorName:
    return "list_online_evaluation_configs"
```

```python
# ListOnlineEvaluationConfigsPaginatorName definition
ListOnlineEvaluationConfigsPaginatorName = Literal[
    "list_online_evaluation_configs",
]
```
## ListPoliciesPaginatorName

```python
# ListPoliciesPaginatorName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ListPoliciesPaginatorName

def get_value() -> ListPoliciesPaginatorName:
    return "list_policies"
```

```python
# ListPoliciesPaginatorName definition
ListPoliciesPaginatorName = Literal[
    "list_policies",
]
```
## ListPolicyEnginesPaginatorName

```python
# ListPolicyEnginesPaginatorName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ListPolicyEnginesPaginatorName

def get_value() -> ListPolicyEnginesPaginatorName:
    return "list_policy_engines"
```

```python
# ListPolicyEnginesPaginatorName definition
ListPolicyEnginesPaginatorName = Literal[
    "list_policy_engines",
]
```
## ListPolicyGenerationAssetsPaginatorName

```python
# ListPolicyGenerationAssetsPaginatorName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ListPolicyGenerationAssetsPaginatorName

def get_value() -> ListPolicyGenerationAssetsPaginatorName:
    return "list_policy_generation_assets"
```

```python
# ListPolicyGenerationAssetsPaginatorName definition
ListPolicyGenerationAssetsPaginatorName = Literal[
    "list_policy_generation_assets",
]
```
## ListPolicyGenerationsPaginatorName

```python
# ListPolicyGenerationsPaginatorName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ListPolicyGenerationsPaginatorName

def get_value() -> ListPolicyGenerationsPaginatorName:
    return "list_policy_generations"
```

```python
# ListPolicyGenerationsPaginatorName definition
ListPolicyGenerationsPaginatorName = Literal[
    "list_policy_generations",
]
```
## ListWorkloadIdentitiesPaginatorName

```python
# ListWorkloadIdentitiesPaginatorName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ListWorkloadIdentitiesPaginatorName

def get_value() -> ListWorkloadIdentitiesPaginatorName:
    return "list_workload_identities"
```

```python
# ListWorkloadIdentitiesPaginatorName definition
ListWorkloadIdentitiesPaginatorName = Literal[
    "list_workload_identities",
]
```
## MemoryCreatedWaiterName

```python
# MemoryCreatedWaiterName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import MemoryCreatedWaiterName

def get_value() -> MemoryCreatedWaiterName:
    return "memory_created"
```

```python
# MemoryCreatedWaiterName definition
MemoryCreatedWaiterName = Literal[
    "memory_created",
]
```
## MemoryStatusType

```python
# MemoryStatusType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import MemoryStatusType

def get_value() -> MemoryStatusType:
    return "ACTIVE"
```

```python
# MemoryStatusType definition
MemoryStatusType = Literal[
    "ACTIVE",
    "CREATING",
    "DELETING",
    "FAILED",
]
```
## MemoryStrategyStatusType

```python
# MemoryStrategyStatusType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import MemoryStrategyStatusType

def get_value() -> MemoryStrategyStatusType:
    return "ACTIVE"
```

```python
# MemoryStrategyStatusType definition
MemoryStrategyStatusType = Literal[
    "ACTIVE",
    "CREATING",
    "DELETING",
    "FAILED",
]
```
## MemoryStrategyTypeType

```python
# MemoryStrategyTypeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import MemoryStrategyTypeType

def get_value() -> MemoryStrategyTypeType:
    return "CUSTOM"
```

```python
# MemoryStrategyTypeType definition
MemoryStrategyTypeType = Literal[
    "CUSTOM",
    "EPISODIC",
    "SEMANTIC",
    "SUMMARIZATION",
    "USER_PREFERENCE",
]
```
## MemoryViewType

```python
# MemoryViewType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import MemoryViewType

def get_value() -> MemoryViewType:
    return "full"
```

```python
# MemoryViewType definition
MemoryViewType = Literal[
    "full",
    "without_decryption",
]
```
## NetworkModeType

```python
# NetworkModeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import NetworkModeType

def get_value() -> NetworkModeType:
    return "PUBLIC"
```

```python
# NetworkModeType definition
NetworkModeType = Literal[
    "PUBLIC",
    "VPC",
]
```
## OAuthGrantTypeType

```python
# OAuthGrantTypeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import OAuthGrantTypeType

def get_value() -> OAuthGrantTypeType:
    return "AUTHORIZATION_CODE"
```

```python
# OAuthGrantTypeType definition
OAuthGrantTypeType = Literal[
    "AUTHORIZATION_CODE",
    "CLIENT_CREDENTIALS",
]
```
## OnlineEvaluationConfigStatusType

```python
# OnlineEvaluationConfigStatusType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import OnlineEvaluationConfigStatusType

def get_value() -> OnlineEvaluationConfigStatusType:
    return "ACTIVE"
```

```python
# OnlineEvaluationConfigStatusType definition
OnlineEvaluationConfigStatusType = Literal[
    "ACTIVE",
    "CREATE_FAILED",
    "CREATING",
    "DELETING",
    "UPDATE_FAILED",
    "UPDATING",
]
```
## OnlineEvaluationExecutionStatusType

```python
# OnlineEvaluationExecutionStatusType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import OnlineEvaluationExecutionStatusType

def get_value() -> OnlineEvaluationExecutionStatusType:
    return "DISABLED"
```

```python
# OnlineEvaluationExecutionStatusType definition
OnlineEvaluationExecutionStatusType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## OverrideTypeType

```python
# OverrideTypeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import OverrideTypeType

def get_value() -> OverrideTypeType:
    return "EPISODIC_OVERRIDE"
```

```python
# OverrideTypeType definition
OverrideTypeType = Literal[
    "EPISODIC_OVERRIDE",
    "SELF_MANAGED",
    "SEMANTIC_OVERRIDE",
    "SUMMARY_OVERRIDE",
    "USER_PREFERENCE_OVERRIDE",
]
```
## PolicyActiveWaiterName

```python
# PolicyActiveWaiterName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import PolicyActiveWaiterName

def get_value() -> PolicyActiveWaiterName:
    return "policy_active"
```

```python
# PolicyActiveWaiterName definition
PolicyActiveWaiterName = Literal[
    "policy_active",
]
```
## PolicyDeletedWaiterName

```python
# PolicyDeletedWaiterName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import PolicyDeletedWaiterName

def get_value() -> PolicyDeletedWaiterName:
    return "policy_deleted"
```

```python
# PolicyDeletedWaiterName definition
PolicyDeletedWaiterName = Literal[
    "policy_deleted",
]
```
## PolicyEngineActiveWaiterName

```python
# PolicyEngineActiveWaiterName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import PolicyEngineActiveWaiterName

def get_value() -> PolicyEngineActiveWaiterName:
    return "policy_engine_active"
```

```python
# PolicyEngineActiveWaiterName definition
PolicyEngineActiveWaiterName = Literal[
    "policy_engine_active",
]
```
## PolicyEngineDeletedWaiterName

```python
# PolicyEngineDeletedWaiterName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import PolicyEngineDeletedWaiterName

def get_value() -> PolicyEngineDeletedWaiterName:
    return "policy_engine_deleted"
```

```python
# PolicyEngineDeletedWaiterName definition
PolicyEngineDeletedWaiterName = Literal[
    "policy_engine_deleted",
]
```
## PolicyEngineStatusType

```python
# PolicyEngineStatusType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import PolicyEngineStatusType

def get_value() -> PolicyEngineStatusType:
    return "ACTIVE"
```

```python
# PolicyEngineStatusType definition
PolicyEngineStatusType = Literal[
    "ACTIVE",
    "CREATE_FAILED",
    "CREATING",
    "DELETE_FAILED",
    "DELETING",
    "UPDATE_FAILED",
    "UPDATING",
]
```
## PolicyGenerationCompletedWaiterName

```python
# PolicyGenerationCompletedWaiterName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import PolicyGenerationCompletedWaiterName

def get_value() -> PolicyGenerationCompletedWaiterName:
    return "policy_generation_completed"
```

```python
# PolicyGenerationCompletedWaiterName definition
PolicyGenerationCompletedWaiterName = Literal[
    "policy_generation_completed",
]
```
## PolicyGenerationStatusType

```python
# PolicyGenerationStatusType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import PolicyGenerationStatusType

def get_value() -> PolicyGenerationStatusType:
    return "DELETE_FAILED"
```

```python
# PolicyGenerationStatusType definition
PolicyGenerationStatusType = Literal[
    "DELETE_FAILED",
    "GENERATE_FAILED",
    "GENERATED",
    "GENERATING",
]
```
## PolicyStatusType

```python
# PolicyStatusType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import PolicyStatusType

def get_value() -> PolicyStatusType:
    return "ACTIVE"
```

```python
# PolicyStatusType definition
PolicyStatusType = Literal[
    "ACTIVE",
    "CREATE_FAILED",
    "CREATING",
    "DELETE_FAILED",
    "DELETING",
    "UPDATE_FAILED",
    "UPDATING",
]
```
## PolicyValidationModeType

```python
# PolicyValidationModeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import PolicyValidationModeType

def get_value() -> PolicyValidationModeType:
    return "FAIL_ON_ANY_FINDINGS"
```

```python
# PolicyValidationModeType definition
PolicyValidationModeType = Literal[
    "FAIL_ON_ANY_FINDINGS",
    "IGNORE_ALL_FINDINGS",
]
```
## ResourceTypeType

```python
# ResourceTypeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ResourceTypeType

def get_value() -> ResourceTypeType:
    return "CUSTOM"
```

```python
# ResourceTypeType definition
ResourceTypeType = Literal[
    "CUSTOM",
    "SYSTEM",
]
```
## RestApiMethodType

```python
# RestApiMethodType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import RestApiMethodType

def get_value() -> RestApiMethodType:
    return "DELETE"
```

```python
# RestApiMethodType definition
RestApiMethodType = Literal[
    "DELETE",
    "GET",
    "HEAD",
    "OPTIONS",
    "PATCH",
    "POST",
    "PUT",
]
```
## SchemaTypeType

```python
# SchemaTypeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import SchemaTypeType

def get_value() -> SchemaTypeType:
    return "array"
```

```python
# SchemaTypeType definition
SchemaTypeType = Literal[
    "array",
    "boolean",
    "integer",
    "number",
    "object",
    "string",
]
```
## SearchTypeType

```python
# SearchTypeType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import SearchTypeType

def get_value() -> SearchTypeType:
    return "SEMANTIC"
```

```python
# SearchTypeType definition
SearchTypeType = Literal[
    "SEMANTIC",
]
```
## ServerProtocolType

```python
# ServerProtocolType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ServerProtocolType

def get_value() -> ServerProtocolType:
    return "A2A"
```

```python
# ServerProtocolType definition
ServerProtocolType = Literal[
    "A2A",
    "HTTP",
    "MCP",
]
```
## TargetStatusType

```python
# TargetStatusType usage example
from types_aiobotocore_bedrock_agentcore_control.literals import TargetStatusType

def get_value() -> TargetStatusType:
    return "CREATING"
```

```python
# TargetStatusType definition
TargetStatusType = Literal[
    "CREATING",
    "DELETING",
    "FAILED",
    "READY",
    "SYNCHRONIZE_UNSUCCESSFUL",
    "SYNCHRONIZING",
    "UPDATE_UNSUCCESSFUL",
    "UPDATING",
]
```
## BedrockAgentCoreControlServiceName

```python
# BedrockAgentCoreControlServiceName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import BedrockAgentCoreControlServiceName

def get_value() -> BedrockAgentCoreControlServiceName:
    return "bedrock-agentcore-control"
```

```python
# BedrockAgentCoreControlServiceName definition
BedrockAgentCoreControlServiceName = Literal[
    "bedrock-agentcore-control",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ServiceName

def get_value() -> ServiceName:
    return "accessanalyzer"
```

```python
# ServiceName definition
ServiceName = Literal[
    "accessanalyzer",
    "account",
    "acm",
    "acm-pca",
    "aiops",
    "amp",
    "amplify",
    "amplifybackend",
    "amplifyuibuilder",
    "apigateway",
    "apigatewaymanagementapi",
    "apigatewayv2",
    "appconfig",
    "appconfigdata",
    "appfabric",
    "appflow",
    "appintegrations",
    "application-autoscaling",
    "application-insights",
    "application-signals",
    "applicationcostprofiler",
    "appmesh",
    "apprunner",
    "appstream",
    "appsync",
    "arc-region-switch",
    "arc-zonal-shift",
    "artifact",
    "athena",
    "auditmanager",
    "autoscaling",
    "autoscaling-plans",
    "b2bi",
    "backup",
    "backup-gateway",
    "backupsearch",
    "batch",
    "bcm-dashboards",
    "bcm-data-exports",
    "bcm-pricing-calculator",
    "bcm-recommended-actions",
    "bedrock",
    "bedrock-agent",
    "bedrock-agent-runtime",
    "bedrock-agentcore",
    "bedrock-agentcore-control",
    "bedrock-data-automation",
    "bedrock-data-automation-runtime",
    "bedrock-runtime",
    "billing",
    "billingconductor",
    "braket",
    "budgets",
    "ce",
    "chatbot",
    "chime",
    "chime-sdk-identity",
    "chime-sdk-media-pipelines",
    "chime-sdk-meetings",
    "chime-sdk-messaging",
    "chime-sdk-voice",
    "cleanrooms",
    "cleanroomsml",
    "cloud9",
    "cloudcontrol",
    "clouddirectory",
    "cloudformation",
    "cloudfront",
    "cloudfront-keyvaluestore",
    "cloudhsm",
    "cloudhsmv2",
    "cloudsearch",
    "cloudsearchdomain",
    "cloudtrail",
    "cloudtrail-data",
    "cloudwatch",
    "codeartifact",
    "codebuild",
    "codecatalyst",
    "codecommit",
    "codeconnections",
    "codedeploy",
    "codeguru-reviewer",
    "codeguru-security",
    "codeguruprofiler",
    "codepipeline",
    "codestar-connections",
    "codestar-notifications",
    "cognito-identity",
    "cognito-idp",
    "cognito-sync",
    "comprehend",
    "comprehendmedical",
    "compute-optimizer",
    "compute-optimizer-automation",
    "config",
    "connect",
    "connect-contact-lens",
    "connectcampaigns",
    "connectcampaignsv2",
    "connectcases",
    "connectparticipant",
    "controlcatalog",
    "controltower",
    "cost-optimization-hub",
    "cur",
    "customer-profiles",
    "databrew",
    "dataexchange",
    "datapipeline",
    "datasync",
    "datazone",
    "dax",
    "deadline",
    "detective",
    "devicefarm",
    "devops-guru",
    "directconnect",
    "discovery",
    "dlm",
    "dms",
    "docdb",
    "docdb-elastic",
    "drs",
    "ds",
    "ds-data",
    "dsql",
    "dynamodb",
    "dynamodbstreams",
    "ebs",
    "ec2",
    "ec2-instance-connect",
    "ecr",
    "ecr-public",
    "ecs",
    "efs",
    "eks",
    "eks-auth",
    "elasticache",
    "elasticbeanstalk",
    "elb",
    "elbv2",
    "emr",
    "emr-containers",
    "emr-serverless",
    "entityresolution",
    "es",
    "events",
    "evidently",
    "evs",
    "finspace",
    "finspace-data",
    "firehose",
    "fis",
    "fms",
    "forecast",
    "forecastquery",
    "frauddetector",
    "freetier",
    "fsx",
    "gamelift",
    "gameliftstreams",
    "geo-maps",
    "geo-places",
    "geo-routes",
    "glacier",
    "globalaccelerator",
    "glue",
    "grafana",
    "greengrass",
    "greengrassv2",
    "groundstation",
    "guardduty",
    "health",
    "healthlake",
    "iam",
    "identitystore",
    "imagebuilder",
    "importexport",
    "inspector",
    "inspector-scan",
    "inspector2",
    "internetmonitor",
    "invoicing",
    "iot",
    "iot-data",
    "iot-jobs-data",
    "iot-managed-integrations",
    "iotanalytics",
    "iotdeviceadvisor",
    "iotevents",
    "iotevents-data",
    "iotfleetwise",
    "iotsecuretunneling",
    "iotsitewise",
    "iotthingsgraph",
    "iottwinmaker",
    "iotwireless",
    "ivs",
    "ivs-realtime",
    "ivschat",
    "kafka",
    "kafkaconnect",
    "kendra",
    "kendra-ranking",
    "keyspaces",
    "keyspacesstreams",
    "kinesis",
    "kinesis-video-archived-media",
    "kinesis-video-media",
    "kinesis-video-signaling",
    "kinesis-video-webrtc-storage",
    "kinesisanalytics",
    "kinesisanalyticsv2",
    "kinesisvideo",
    "kms",
    "lakeformation",
    "lambda",
    "launch-wizard",
    "lex-models",
    "lex-runtime",
    "lexv2-models",
    "lexv2-runtime",
    "license-manager",
    "license-manager-linux-subscriptions",
    "license-manager-user-subscriptions",
    "lightsail",
    "location",
    "logs",
    "lookoutequipment",
    "m2",
    "machinelearning",
    "macie2",
    "mailmanager",
    "managedblockchain",
    "managedblockchain-query",
    "marketplace-agreement",
    "marketplace-catalog",
    "marketplace-deployment",
    "marketplace-entitlement",
    "marketplace-reporting",
    "marketplacecommerceanalytics",
    "mediaconnect",
    "mediaconvert",
    "medialive",
    "mediapackage",
    "mediapackage-vod",
    "mediapackagev2",
    "mediastore",
    "mediastore-data",
    "mediatailor",
    "medical-imaging",
    "memorydb",
    "meteringmarketplace",
    "mgh",
    "mgn",
    "migration-hub-refactor-spaces",
    "migrationhub-config",
    "migrationhuborchestrator",
    "migrationhubstrategy",
    "mpa",
    "mq",
    "mturk",
    "mwaa",
    "mwaa-serverless",
    "neptune",
    "neptune-graph",
    "neptunedata",
    "network-firewall",
    "networkflowmonitor",
    "networkmanager",
    "networkmonitor",
    "notifications",
    "notificationscontacts",
    "nova-act",
    "oam",
    "observabilityadmin",
    "odb",
    "omics",
    "opensearch",
    "opensearchserverless",
    "organizations",
    "osis",
    "outposts",
    "panorama",
    "partnercentral-account",
    "partnercentral-benefits",
    "partnercentral-channel",
    "partnercentral-selling",
    "payment-cryptography",
    "payment-cryptography-data",
    "pca-connector-ad",
    "pca-connector-scep",
    "pcs",
    "personalize",
    "personalize-events",
    "personalize-runtime",
    "pi",
    "pinpoint",
    "pinpoint-email",
    "pinpoint-sms-voice",
    "pinpoint-sms-voice-v2",
    "pipes",
    "polly",
    "pricing",
    "proton",
    "qapps",
    "qbusiness",
    "qconnect",
    "quicksight",
    "ram",
    "rbin",
    "rds",
    "rds-data",
    "redshift",
    "redshift-data",
    "redshift-serverless",
    "rekognition",
    "repostspace",
    "resiliencehub",
    "resource-explorer-2",
    "resource-groups",
    "resourcegroupstaggingapi",
    "rolesanywhere",
    "route53",
    "route53-recovery-cluster",
    "route53-recovery-control-config",
    "route53-recovery-readiness",
    "route53domains",
    "route53globalresolver",
    "route53profiles",
    "route53resolver",
    "rtbfabric",
    "rum",
    "s3",
    "s3control",
    "s3outposts",
    "s3tables",
    "s3vectors",
    "sagemaker",
    "sagemaker-a2i-runtime",
    "sagemaker-edge",
    "sagemaker-featurestore-runtime",
    "sagemaker-geospatial",
    "sagemaker-metrics",
    "sagemaker-runtime",
    "savingsplans",
    "scheduler",
    "schemas",
    "sdb",
    "secretsmanager",
    "security-ir",
    "securityhub",
    "securitylake",
    "serverlessrepo",
    "service-quotas",
    "servicecatalog",
    "servicecatalog-appregistry",
    "servicediscovery",
    "ses",
    "sesv2",
    "shield",
    "signer",
    "signin",
    "simspaceweaver",
    "snow-device-management",
    "snowball",
    "sns",
    "socialmessaging",
    "sqs",
    "ssm",
    "ssm-contacts",
    "ssm-guiconnect",
    "ssm-incidents",
    "ssm-quicksetup",
    "ssm-sap",
    "sso",
    "sso-admin",
    "sso-oidc",
    "stepfunctions",
    "storagegateway",
    "sts",
    "supplychain",
    "support",
    "support-app",
    "swf",
    "synthetics",
    "taxsettings",
    "textract",
    "timestream-influxdb",
    "timestream-query",
    "timestream-write",
    "tnb",
    "transcribe",
    "transfer",
    "translate",
    "trustedadvisor",
    "verifiedpermissions",
    "voice-id",
    "vpc-lattice",
    "waf",
    "waf-regional",
    "wafv2",
    "wellarchitected",
    "wickr",
    "wisdom",
    "workdocs",
    "workmail",
    "workmailmessageflow",
    "workspaces",
    "workspaces-instances",
    "workspaces-thin-client",
    "workspaces-web",
    "xray",
]
```
## ResourceServiceName

```python
# ResourceServiceName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import ResourceServiceName

def get_value() -> ResourceServiceName:
    return "cloudformation"
```

```python
# ResourceServiceName definition
ResourceServiceName = Literal[
    "cloudformation",
    "cloudwatch",
    "dynamodb",
    "ec2",
    "glacier",
    "iam",
    "s3",
    "sns",
    "sqs",
]
```
## PaginatorName

```python
# PaginatorName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_agent_runtime_endpoints"
```

```python
# PaginatorName definition
PaginatorName = Literal[
    "list_agent_runtime_endpoints",
    "list_agent_runtime_versions",
    "list_agent_runtimes",
    "list_api_key_credential_providers",
    "list_browsers",
    "list_code_interpreters",
    "list_evaluators",
    "list_gateway_targets",
    "list_gateways",
    "list_memories",
    "list_oauth2_credential_providers",
    "list_online_evaluation_configs",
    "list_policies",
    "list_policy_engines",
    "list_policy_generation_assets",
    "list_policy_generations",
    "list_workload_identities",
]
```
## WaiterName

```python
# WaiterName usage example
from types_aiobotocore_bedrock_agentcore_control.literals import WaiterName

def get_value() -> WaiterName:
    return "memory_created"
```

```python
# WaiterName definition
WaiterName = Literal[
    "memory_created",
    "policy_active",
    "policy_deleted",
    "policy_engine_active",
    "policy_engine_deleted",
    "policy_generation_completed",
]
```
