# Type definitions

> [Index](../README.md) > [OpenSearchServiceServerless](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [OpenSearchServiceServerless](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#opensearchserviceserverless)
    type annotations stubs module [types-aiobotocore-opensearchserverless](https://pypi.org/project/types-aiobotocore-opensearchserverless/).



## AccessPolicyDetailTypeDef

```python
# AccessPolicyDetailTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import AccessPolicyDetailTypeDef


def get_value() -> AccessPolicyDetailTypeDef:
    return {
        "type": ...,
    }


# AccessPolicyDetailTypeDef definition

class AccessPolicyDetailTypeDef(TypedDict):
    type: NotRequired[AccessPolicyTypeType],  # (1)
    name: NotRequired[str],
    policyVersion: NotRequired[str],
    description: NotRequired[str],
    policy: NotRequired[Dict[str, Any]],
    createdDate: NotRequired[int],
    lastModifiedDate: NotRequired[int],
```

1. See [:material-code-brackets: AccessPolicyTypeType](./literals.md#accesspolicytypetype) 
## AccessPolicyStatsTypeDef

```python
# AccessPolicyStatsTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import AccessPolicyStatsTypeDef


def get_value() -> AccessPolicyStatsTypeDef:
    return {
        "DataPolicyCount": ...,
    }


# AccessPolicyStatsTypeDef definition

class AccessPolicyStatsTypeDef(TypedDict):
    DataPolicyCount: NotRequired[int],
```

## AccessPolicySummaryTypeDef

```python
# AccessPolicySummaryTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import AccessPolicySummaryTypeDef


def get_value() -> AccessPolicySummaryTypeDef:
    return {
        "type": ...,
    }


# AccessPolicySummaryTypeDef definition

class AccessPolicySummaryTypeDef(TypedDict):
    type: NotRequired[AccessPolicyTypeType],  # (1)
    name: NotRequired[str],
    policyVersion: NotRequired[str],
    description: NotRequired[str],
    createdDate: NotRequired[int],
    lastModifiedDate: NotRequired[int],
```

1. See [:material-code-brackets: AccessPolicyTypeType](./literals.md#accesspolicytypetype) 
## CapacityLimitsTypeDef

```python
# CapacityLimitsTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import CapacityLimitsTypeDef


def get_value() -> CapacityLimitsTypeDef:
    return {
        "maxIndexingCapacityInOCU": ...,
    }


# CapacityLimitsTypeDef definition

class CapacityLimitsTypeDef(TypedDict):
    maxIndexingCapacityInOCU: NotRequired[int],
    maxSearchCapacityInOCU: NotRequired[int],
```

## BatchGetCollectionRequestTypeDef

```python
# BatchGetCollectionRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import BatchGetCollectionRequestTypeDef


def get_value() -> BatchGetCollectionRequestTypeDef:
    return {
        "ids": ...,
    }


# BatchGetCollectionRequestTypeDef definition

class BatchGetCollectionRequestTypeDef(TypedDict):
    ids: NotRequired[Sequence[str]],
    names: NotRequired[Sequence[str]],
```

## CollectionDetailTypeDef

```python
# CollectionDetailTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import CollectionDetailTypeDef


def get_value() -> CollectionDetailTypeDef:
    return {
        "id": ...,
    }


# CollectionDetailTypeDef definition

class CollectionDetailTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    status: NotRequired[CollectionStatusType],  # (1)
    type: NotRequired[CollectionTypeType],  # (2)
    description: NotRequired[str],
    arn: NotRequired[str],
    kmsKeyArn: NotRequired[str],
    standbyReplicas: NotRequired[StandbyReplicasType],  # (3)
    createdDate: NotRequired[int],
    lastModifiedDate: NotRequired[int],
    collectionEndpoint: NotRequired[str],
    dashboardEndpoint: NotRequired[str],
    failureCode: NotRequired[str],
    failureMessage: NotRequired[str],
```

1. See [:material-code-brackets: CollectionStatusType](./literals.md#collectionstatustype) 
2. See [:material-code-brackets: CollectionTypeType](./literals.md#collectiontypetype) 
3. See [:material-code-brackets: StandbyReplicasType](./literals.md#standbyreplicastype) 
## CollectionErrorDetailTypeDef

```python
# CollectionErrorDetailTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import CollectionErrorDetailTypeDef


def get_value() -> CollectionErrorDetailTypeDef:
    return {
        "id": ...,
    }


# CollectionErrorDetailTypeDef definition

class CollectionErrorDetailTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    errorMessage: NotRequired[str],
    errorCode: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## LifecyclePolicyResourceIdentifierTypeDef

```python
# LifecyclePolicyResourceIdentifierTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import LifecyclePolicyResourceIdentifierTypeDef


def get_value() -> LifecyclePolicyResourceIdentifierTypeDef:
    return {
        "type": ...,
    }


# LifecyclePolicyResourceIdentifierTypeDef definition

class LifecyclePolicyResourceIdentifierTypeDef(TypedDict):
    type: LifecyclePolicyTypeType,  # (1)
    resource: str,
```

1. See [:material-code-brackets: LifecyclePolicyTypeType](./literals.md#lifecyclepolicytypetype) 
## EffectiveLifecyclePolicyDetailTypeDef

```python
# EffectiveLifecyclePolicyDetailTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import EffectiveLifecyclePolicyDetailTypeDef


def get_value() -> EffectiveLifecyclePolicyDetailTypeDef:
    return {
        "type": ...,
    }


# EffectiveLifecyclePolicyDetailTypeDef definition

class EffectiveLifecyclePolicyDetailTypeDef(TypedDict):
    type: NotRequired[LifecyclePolicyTypeType],  # (1)
    resource: NotRequired[str],
    policyName: NotRequired[str],
    resourceType: NotRequired[ResourceTypeType],  # (2)
    retentionPeriod: NotRequired[str],
    noMinRetentionPeriod: NotRequired[bool],
```

1. See [:material-code-brackets: LifecyclePolicyTypeType](./literals.md#lifecyclepolicytypetype) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## EffectiveLifecyclePolicyErrorDetailTypeDef

```python
# EffectiveLifecyclePolicyErrorDetailTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import EffectiveLifecyclePolicyErrorDetailTypeDef


def get_value() -> EffectiveLifecyclePolicyErrorDetailTypeDef:
    return {
        "type": ...,
    }


# EffectiveLifecyclePolicyErrorDetailTypeDef definition

class EffectiveLifecyclePolicyErrorDetailTypeDef(TypedDict):
    type: NotRequired[LifecyclePolicyTypeType],  # (1)
    resource: NotRequired[str],
    errorMessage: NotRequired[str],
    errorCode: NotRequired[str],
```

1. See [:material-code-brackets: LifecyclePolicyTypeType](./literals.md#lifecyclepolicytypetype) 
## LifecyclePolicyIdentifierTypeDef

```python
# LifecyclePolicyIdentifierTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import LifecyclePolicyIdentifierTypeDef


def get_value() -> LifecyclePolicyIdentifierTypeDef:
    return {
        "type": ...,
    }


# LifecyclePolicyIdentifierTypeDef definition

class LifecyclePolicyIdentifierTypeDef(TypedDict):
    type: LifecyclePolicyTypeType,  # (1)
    name: str,
```

1. See [:material-code-brackets: LifecyclePolicyTypeType](./literals.md#lifecyclepolicytypetype) 
## LifecyclePolicyDetailTypeDef

```python
# LifecyclePolicyDetailTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import LifecyclePolicyDetailTypeDef


def get_value() -> LifecyclePolicyDetailTypeDef:
    return {
        "type": ...,
    }


# LifecyclePolicyDetailTypeDef definition

class LifecyclePolicyDetailTypeDef(TypedDict):
    type: NotRequired[LifecyclePolicyTypeType],  # (1)
    name: NotRequired[str],
    policyVersion: NotRequired[str],
    description: NotRequired[str],
    policy: NotRequired[Dict[str, Any]],
    createdDate: NotRequired[int],
    lastModifiedDate: NotRequired[int],
```

1. See [:material-code-brackets: LifecyclePolicyTypeType](./literals.md#lifecyclepolicytypetype) 
## LifecyclePolicyErrorDetailTypeDef

```python
# LifecyclePolicyErrorDetailTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import LifecyclePolicyErrorDetailTypeDef


def get_value() -> LifecyclePolicyErrorDetailTypeDef:
    return {
        "type": ...,
    }


# LifecyclePolicyErrorDetailTypeDef definition

class LifecyclePolicyErrorDetailTypeDef(TypedDict):
    type: NotRequired[LifecyclePolicyTypeType],  # (1)
    name: NotRequired[str],
    errorMessage: NotRequired[str],
    errorCode: NotRequired[str],
```

1. See [:material-code-brackets: LifecyclePolicyTypeType](./literals.md#lifecyclepolicytypetype) 
## BatchGetVpcEndpointRequestTypeDef

```python
# BatchGetVpcEndpointRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import BatchGetVpcEndpointRequestTypeDef


def get_value() -> BatchGetVpcEndpointRequestTypeDef:
    return {
        "ids": ...,
    }


# BatchGetVpcEndpointRequestTypeDef definition

class BatchGetVpcEndpointRequestTypeDef(TypedDict):
    ids: Sequence[str],
```

## VpcEndpointDetailTypeDef

```python
# VpcEndpointDetailTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import VpcEndpointDetailTypeDef


def get_value() -> VpcEndpointDetailTypeDef:
    return {
        "id": ...,
    }


# VpcEndpointDetailTypeDef definition

class VpcEndpointDetailTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    vpcId: NotRequired[str],
    subnetIds: NotRequired[List[str]],
    securityGroupIds: NotRequired[List[str]],
    status: NotRequired[VpcEndpointStatusType],  # (1)
    createdDate: NotRequired[int],
    failureCode: NotRequired[str],
    failureMessage: NotRequired[str],
```

1. See [:material-code-brackets: VpcEndpointStatusType](./literals.md#vpcendpointstatustype) 
## VpcEndpointErrorDetailTypeDef

```python
# VpcEndpointErrorDetailTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import VpcEndpointErrorDetailTypeDef


def get_value() -> VpcEndpointErrorDetailTypeDef:
    return {
        "id": ...,
    }


# VpcEndpointErrorDetailTypeDef definition

class VpcEndpointErrorDetailTypeDef(TypedDict):
    id: NotRequired[str],
    errorMessage: NotRequired[str],
    errorCode: NotRequired[str],
```

## CollectionFiltersTypeDef

```python
# CollectionFiltersTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import CollectionFiltersTypeDef


def get_value() -> CollectionFiltersTypeDef:
    return {
        "name": ...,
    }


# CollectionFiltersTypeDef definition

class CollectionFiltersTypeDef(TypedDict):
    name: NotRequired[str],
    status: NotRequired[CollectionStatusType],  # (1)
```

1. See [:material-code-brackets: CollectionStatusType](./literals.md#collectionstatustype) 
## CollectionSummaryTypeDef

```python
# CollectionSummaryTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import CollectionSummaryTypeDef


def get_value() -> CollectionSummaryTypeDef:
    return {
        "id": ...,
    }


# CollectionSummaryTypeDef definition

class CollectionSummaryTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    status: NotRequired[CollectionStatusType],  # (1)
    arn: NotRequired[str],
```

1. See [:material-code-brackets: CollectionStatusType](./literals.md#collectionstatustype) 
## CreateAccessPolicyRequestTypeDef

```python
# CreateAccessPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import CreateAccessPolicyRequestTypeDef


def get_value() -> CreateAccessPolicyRequestTypeDef:
    return {
        "type": ...,
    }


# CreateAccessPolicyRequestTypeDef definition

class CreateAccessPolicyRequestTypeDef(TypedDict):
    type: AccessPolicyTypeType,  # (1)
    name: str,
    policy: str,
    description: NotRequired[str],
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: AccessPolicyTypeType](./literals.md#accesspolicytypetype) 
## CreateCollectionDetailTypeDef

```python
# CreateCollectionDetailTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import CreateCollectionDetailTypeDef


def get_value() -> CreateCollectionDetailTypeDef:
    return {
        "id": ...,
    }


# CreateCollectionDetailTypeDef definition

class CreateCollectionDetailTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    status: NotRequired[CollectionStatusType],  # (1)
    type: NotRequired[CollectionTypeType],  # (2)
    description: NotRequired[str],
    arn: NotRequired[str],
    kmsKeyArn: NotRequired[str],
    standbyReplicas: NotRequired[StandbyReplicasType],  # (3)
    createdDate: NotRequired[int],
    lastModifiedDate: NotRequired[int],
```

1. See [:material-code-brackets: CollectionStatusType](./literals.md#collectionstatustype) 
2. See [:material-code-brackets: CollectionTypeType](./literals.md#collectiontypetype) 
3. See [:material-code-brackets: StandbyReplicasType](./literals.md#standbyreplicastype) 
## TagTypeDef

```python
# TagTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import TagTypeDef


def get_value() -> TagTypeDef:
    return {
        "key": ...,
    }


# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: str,
    value: str,
```

## CreateIamIdentityCenterConfigOptionsTypeDef

```python
# CreateIamIdentityCenterConfigOptionsTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import CreateIamIdentityCenterConfigOptionsTypeDef


def get_value() -> CreateIamIdentityCenterConfigOptionsTypeDef:
    return {
        "instanceArn": ...,
    }


# CreateIamIdentityCenterConfigOptionsTypeDef definition

class CreateIamIdentityCenterConfigOptionsTypeDef(TypedDict):
    instanceArn: str,
    userAttribute: NotRequired[IamIdentityCenterUserAttributeType],  # (1)
    groupAttribute: NotRequired[IamIdentityCenterGroupAttributeType],  # (2)
```

1. See [:material-code-brackets: IamIdentityCenterUserAttributeType](./literals.md#iamidentitycenteruserattributetype) 
2. See [:material-code-brackets: IamIdentityCenterGroupAttributeType](./literals.md#iamidentitycentergroupattributetype) 
## CreateLifecyclePolicyRequestTypeDef

```python
# CreateLifecyclePolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import CreateLifecyclePolicyRequestTypeDef


def get_value() -> CreateLifecyclePolicyRequestTypeDef:
    return {
        "type": ...,
    }


# CreateLifecyclePolicyRequestTypeDef definition

class CreateLifecyclePolicyRequestTypeDef(TypedDict):
    type: LifecyclePolicyTypeType,  # (1)
    name: str,
    policy: str,
    description: NotRequired[str],
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: LifecyclePolicyTypeType](./literals.md#lifecyclepolicytypetype) 
## SamlConfigOptionsTypeDef

```python
# SamlConfigOptionsTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import SamlConfigOptionsTypeDef


def get_value() -> SamlConfigOptionsTypeDef:
    return {
        "metadata": ...,
    }


# SamlConfigOptionsTypeDef definition

class SamlConfigOptionsTypeDef(TypedDict):
    metadata: str,
    userAttribute: NotRequired[str],
    groupAttribute: NotRequired[str],
    openSearchServerlessEntityId: NotRequired[str],
    sessionTimeout: NotRequired[int],
```

## CreateSecurityPolicyRequestTypeDef

```python
# CreateSecurityPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import CreateSecurityPolicyRequestTypeDef


def get_value() -> CreateSecurityPolicyRequestTypeDef:
    return {
        "type": ...,
    }


# CreateSecurityPolicyRequestTypeDef definition

class CreateSecurityPolicyRequestTypeDef(TypedDict):
    type: SecurityPolicyTypeType,  # (1)
    name: str,
    policy: str,
    description: NotRequired[str],
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: SecurityPolicyTypeType](./literals.md#securitypolicytypetype) 
## SecurityPolicyDetailTypeDef

```python
# SecurityPolicyDetailTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import SecurityPolicyDetailTypeDef


def get_value() -> SecurityPolicyDetailTypeDef:
    return {
        "type": ...,
    }


# SecurityPolicyDetailTypeDef definition

class SecurityPolicyDetailTypeDef(TypedDict):
    type: NotRequired[SecurityPolicyTypeType],  # (1)
    name: NotRequired[str],
    policyVersion: NotRequired[str],
    description: NotRequired[str],
    policy: NotRequired[Dict[str, Any]],
    createdDate: NotRequired[int],
    lastModifiedDate: NotRequired[int],
```

1. See [:material-code-brackets: SecurityPolicyTypeType](./literals.md#securitypolicytypetype) 
## CreateVpcEndpointDetailTypeDef

```python
# CreateVpcEndpointDetailTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import CreateVpcEndpointDetailTypeDef


def get_value() -> CreateVpcEndpointDetailTypeDef:
    return {
        "id": ...,
    }


# CreateVpcEndpointDetailTypeDef definition

class CreateVpcEndpointDetailTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    status: NotRequired[VpcEndpointStatusType],  # (1)
```

1. See [:material-code-brackets: VpcEndpointStatusType](./literals.md#vpcendpointstatustype) 
## CreateVpcEndpointRequestTypeDef

```python
# CreateVpcEndpointRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import CreateVpcEndpointRequestTypeDef


def get_value() -> CreateVpcEndpointRequestTypeDef:
    return {
        "name": ...,
    }


# CreateVpcEndpointRequestTypeDef definition

class CreateVpcEndpointRequestTypeDef(TypedDict):
    name: str,
    vpcId: str,
    subnetIds: Sequence[str],
    securityGroupIds: NotRequired[Sequence[str]],
    clientToken: NotRequired[str],
```

## DeleteAccessPolicyRequestTypeDef

```python
# DeleteAccessPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import DeleteAccessPolicyRequestTypeDef


def get_value() -> DeleteAccessPolicyRequestTypeDef:
    return {
        "type": ...,
    }


# DeleteAccessPolicyRequestTypeDef definition

class DeleteAccessPolicyRequestTypeDef(TypedDict):
    type: AccessPolicyTypeType,  # (1)
    name: str,
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: AccessPolicyTypeType](./literals.md#accesspolicytypetype) 
## DeleteCollectionDetailTypeDef

```python
# DeleteCollectionDetailTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import DeleteCollectionDetailTypeDef


def get_value() -> DeleteCollectionDetailTypeDef:
    return {
        "id": ...,
    }


# DeleteCollectionDetailTypeDef definition

class DeleteCollectionDetailTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    status: NotRequired[CollectionStatusType],  # (1)
```

1. See [:material-code-brackets: CollectionStatusType](./literals.md#collectionstatustype) 
## DeleteCollectionRequestTypeDef

```python
# DeleteCollectionRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import DeleteCollectionRequestTypeDef


def get_value() -> DeleteCollectionRequestTypeDef:
    return {
        "id": ...,
    }


# DeleteCollectionRequestTypeDef definition

class DeleteCollectionRequestTypeDef(TypedDict):
    id: str,
    clientToken: NotRequired[str],
```

## DeleteLifecyclePolicyRequestTypeDef

```python
# DeleteLifecyclePolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import DeleteLifecyclePolicyRequestTypeDef


def get_value() -> DeleteLifecyclePolicyRequestTypeDef:
    return {
        "type": ...,
    }


# DeleteLifecyclePolicyRequestTypeDef definition

class DeleteLifecyclePolicyRequestTypeDef(TypedDict):
    type: LifecyclePolicyTypeType,  # (1)
    name: str,
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: LifecyclePolicyTypeType](./literals.md#lifecyclepolicytypetype) 
## DeleteSecurityConfigRequestTypeDef

```python
# DeleteSecurityConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import DeleteSecurityConfigRequestTypeDef


def get_value() -> DeleteSecurityConfigRequestTypeDef:
    return {
        "id": ...,
    }


# DeleteSecurityConfigRequestTypeDef definition

class DeleteSecurityConfigRequestTypeDef(TypedDict):
    id: str,
    clientToken: NotRequired[str],
```

## DeleteSecurityPolicyRequestTypeDef

```python
# DeleteSecurityPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import DeleteSecurityPolicyRequestTypeDef


def get_value() -> DeleteSecurityPolicyRequestTypeDef:
    return {
        "type": ...,
    }


# DeleteSecurityPolicyRequestTypeDef definition

class DeleteSecurityPolicyRequestTypeDef(TypedDict):
    type: SecurityPolicyTypeType,  # (1)
    name: str,
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: SecurityPolicyTypeType](./literals.md#securitypolicytypetype) 
## DeleteVpcEndpointDetailTypeDef

```python
# DeleteVpcEndpointDetailTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import DeleteVpcEndpointDetailTypeDef


def get_value() -> DeleteVpcEndpointDetailTypeDef:
    return {
        "id": ...,
    }


# DeleteVpcEndpointDetailTypeDef definition

class DeleteVpcEndpointDetailTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    status: NotRequired[VpcEndpointStatusType],  # (1)
```

1. See [:material-code-brackets: VpcEndpointStatusType](./literals.md#vpcendpointstatustype) 
## DeleteVpcEndpointRequestTypeDef

```python
# DeleteVpcEndpointRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import DeleteVpcEndpointRequestTypeDef


def get_value() -> DeleteVpcEndpointRequestTypeDef:
    return {
        "id": ...,
    }


# DeleteVpcEndpointRequestTypeDef definition

class DeleteVpcEndpointRequestTypeDef(TypedDict):
    id: str,
    clientToken: NotRequired[str],
```

## GetAccessPolicyRequestTypeDef

```python
# GetAccessPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import GetAccessPolicyRequestTypeDef


def get_value() -> GetAccessPolicyRequestTypeDef:
    return {
        "type": ...,
    }


# GetAccessPolicyRequestTypeDef definition

class GetAccessPolicyRequestTypeDef(TypedDict):
    type: AccessPolicyTypeType,  # (1)
    name: str,
```

1. See [:material-code-brackets: AccessPolicyTypeType](./literals.md#accesspolicytypetype) 
## LifecyclePolicyStatsTypeDef

```python
# LifecyclePolicyStatsTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import LifecyclePolicyStatsTypeDef


def get_value() -> LifecyclePolicyStatsTypeDef:
    return {
        "RetentionPolicyCount": ...,
    }


# LifecyclePolicyStatsTypeDef definition

class LifecyclePolicyStatsTypeDef(TypedDict):
    RetentionPolicyCount: NotRequired[int],
```

## SecurityConfigStatsTypeDef

```python
# SecurityConfigStatsTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import SecurityConfigStatsTypeDef


def get_value() -> SecurityConfigStatsTypeDef:
    return {
        "SamlConfigCount": ...,
    }


# SecurityConfigStatsTypeDef definition

class SecurityConfigStatsTypeDef(TypedDict):
    SamlConfigCount: NotRequired[int],
```

## SecurityPolicyStatsTypeDef

```python
# SecurityPolicyStatsTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import SecurityPolicyStatsTypeDef


def get_value() -> SecurityPolicyStatsTypeDef:
    return {
        "EncryptionPolicyCount": ...,
    }


# SecurityPolicyStatsTypeDef definition

class SecurityPolicyStatsTypeDef(TypedDict):
    EncryptionPolicyCount: NotRequired[int],
    NetworkPolicyCount: NotRequired[int],
```

## GetSecurityConfigRequestTypeDef

```python
# GetSecurityConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import GetSecurityConfigRequestTypeDef


def get_value() -> GetSecurityConfigRequestTypeDef:
    return {
        "id": ...,
    }


# GetSecurityConfigRequestTypeDef definition

class GetSecurityConfigRequestTypeDef(TypedDict):
    id: str,
```

## GetSecurityPolicyRequestTypeDef

```python
# GetSecurityPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import GetSecurityPolicyRequestTypeDef


def get_value() -> GetSecurityPolicyRequestTypeDef:
    return {
        "type": ...,
    }


# GetSecurityPolicyRequestTypeDef definition

class GetSecurityPolicyRequestTypeDef(TypedDict):
    type: SecurityPolicyTypeType,  # (1)
    name: str,
```

1. See [:material-code-brackets: SecurityPolicyTypeType](./literals.md#securitypolicytypetype) 
## IamIdentityCenterConfigOptionsTypeDef

```python
# IamIdentityCenterConfigOptionsTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import IamIdentityCenterConfigOptionsTypeDef


def get_value() -> IamIdentityCenterConfigOptionsTypeDef:
    return {
        "instanceArn": ...,
    }


# IamIdentityCenterConfigOptionsTypeDef definition

class IamIdentityCenterConfigOptionsTypeDef(TypedDict):
    instanceArn: NotRequired[str],
    applicationArn: NotRequired[str],
    applicationName: NotRequired[str],
    applicationDescription: NotRequired[str],
    userAttribute: NotRequired[IamIdentityCenterUserAttributeType],  # (1)
    groupAttribute: NotRequired[IamIdentityCenterGroupAttributeType],  # (2)
```

1. See [:material-code-brackets: IamIdentityCenterUserAttributeType](./literals.md#iamidentitycenteruserattributetype) 
2. See [:material-code-brackets: IamIdentityCenterGroupAttributeType](./literals.md#iamidentitycentergroupattributetype) 
## LifecyclePolicySummaryTypeDef

```python
# LifecyclePolicySummaryTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import LifecyclePolicySummaryTypeDef


def get_value() -> LifecyclePolicySummaryTypeDef:
    return {
        "type": ...,
    }


# LifecyclePolicySummaryTypeDef definition

class LifecyclePolicySummaryTypeDef(TypedDict):
    type: NotRequired[LifecyclePolicyTypeType],  # (1)
    name: NotRequired[str],
    policyVersion: NotRequired[str],
    description: NotRequired[str],
    createdDate: NotRequired[int],
    lastModifiedDate: NotRequired[int],
```

1. See [:material-code-brackets: LifecyclePolicyTypeType](./literals.md#lifecyclepolicytypetype) 
## ListAccessPoliciesRequestTypeDef

```python
# ListAccessPoliciesRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import ListAccessPoliciesRequestTypeDef


def get_value() -> ListAccessPoliciesRequestTypeDef:
    return {
        "type": ...,
    }


# ListAccessPoliciesRequestTypeDef definition

class ListAccessPoliciesRequestTypeDef(TypedDict):
    type: AccessPolicyTypeType,  # (1)
    resource: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: AccessPolicyTypeType](./literals.md#accesspolicytypetype) 
## ListLifecyclePoliciesRequestTypeDef

```python
# ListLifecyclePoliciesRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import ListLifecyclePoliciesRequestTypeDef


def get_value() -> ListLifecyclePoliciesRequestTypeDef:
    return {
        "type": ...,
    }


# ListLifecyclePoliciesRequestTypeDef definition

class ListLifecyclePoliciesRequestTypeDef(TypedDict):
    type: LifecyclePolicyTypeType,  # (1)
    resources: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: LifecyclePolicyTypeType](./literals.md#lifecyclepolicytypetype) 
## ListSecurityConfigsRequestTypeDef

```python
# ListSecurityConfigsRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import ListSecurityConfigsRequestTypeDef


def get_value() -> ListSecurityConfigsRequestTypeDef:
    return {
        "type": ...,
    }


# ListSecurityConfigsRequestTypeDef definition

class ListSecurityConfigsRequestTypeDef(TypedDict):
    type: SecurityConfigTypeType,  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: SecurityConfigTypeType](./literals.md#securityconfigtypetype) 
## SecurityConfigSummaryTypeDef

```python
# SecurityConfigSummaryTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import SecurityConfigSummaryTypeDef


def get_value() -> SecurityConfigSummaryTypeDef:
    return {
        "id": ...,
    }


# SecurityConfigSummaryTypeDef definition

class SecurityConfigSummaryTypeDef(TypedDict):
    id: NotRequired[str],
    type: NotRequired[SecurityConfigTypeType],  # (1)
    configVersion: NotRequired[str],
    description: NotRequired[str],
    createdDate: NotRequired[int],
    lastModifiedDate: NotRequired[int],
```

1. See [:material-code-brackets: SecurityConfigTypeType](./literals.md#securityconfigtypetype) 
## ListSecurityPoliciesRequestTypeDef

```python
# ListSecurityPoliciesRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import ListSecurityPoliciesRequestTypeDef


def get_value() -> ListSecurityPoliciesRequestTypeDef:
    return {
        "type": ...,
    }


# ListSecurityPoliciesRequestTypeDef definition

class ListSecurityPoliciesRequestTypeDef(TypedDict):
    type: SecurityPolicyTypeType,  # (1)
    resource: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: SecurityPolicyTypeType](./literals.md#securitypolicytypetype) 
## SecurityPolicySummaryTypeDef

```python
# SecurityPolicySummaryTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import SecurityPolicySummaryTypeDef


def get_value() -> SecurityPolicySummaryTypeDef:
    return {
        "type": ...,
    }


# SecurityPolicySummaryTypeDef definition

class SecurityPolicySummaryTypeDef(TypedDict):
    type: NotRequired[SecurityPolicyTypeType],  # (1)
    name: NotRequired[str],
    policyVersion: NotRequired[str],
    description: NotRequired[str],
    createdDate: NotRequired[int],
    lastModifiedDate: NotRequired[int],
```

1. See [:material-code-brackets: SecurityPolicyTypeType](./literals.md#securitypolicytypetype) 
## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```

## VpcEndpointFiltersTypeDef

```python
# VpcEndpointFiltersTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import VpcEndpointFiltersTypeDef


def get_value() -> VpcEndpointFiltersTypeDef:
    return {
        "status": ...,
    }


# VpcEndpointFiltersTypeDef definition

class VpcEndpointFiltersTypeDef(TypedDict):
    status: NotRequired[VpcEndpointStatusType],  # (1)
```

1. See [:material-code-brackets: VpcEndpointStatusType](./literals.md#vpcendpointstatustype) 
## VpcEndpointSummaryTypeDef

```python
# VpcEndpointSummaryTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import VpcEndpointSummaryTypeDef


def get_value() -> VpcEndpointSummaryTypeDef:
    return {
        "id": ...,
    }


# VpcEndpointSummaryTypeDef definition

class VpcEndpointSummaryTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    status: NotRequired[VpcEndpointStatusType],  # (1)
```

1. See [:material-code-brackets: VpcEndpointStatusType](./literals.md#vpcendpointstatustype) 
## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateAccessPolicyRequestTypeDef

```python
# UpdateAccessPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import UpdateAccessPolicyRequestTypeDef


def get_value() -> UpdateAccessPolicyRequestTypeDef:
    return {
        "type": ...,
    }


# UpdateAccessPolicyRequestTypeDef definition

class UpdateAccessPolicyRequestTypeDef(TypedDict):
    type: AccessPolicyTypeType,  # (1)
    name: str,
    policyVersion: str,
    description: NotRequired[str],
    policy: NotRequired[str],
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: AccessPolicyTypeType](./literals.md#accesspolicytypetype) 
## UpdateCollectionDetailTypeDef

```python
# UpdateCollectionDetailTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import UpdateCollectionDetailTypeDef


def get_value() -> UpdateCollectionDetailTypeDef:
    return {
        "id": ...,
    }


# UpdateCollectionDetailTypeDef definition

class UpdateCollectionDetailTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    status: NotRequired[CollectionStatusType],  # (1)
    type: NotRequired[CollectionTypeType],  # (2)
    description: NotRequired[str],
    arn: NotRequired[str],
    createdDate: NotRequired[int],
    lastModifiedDate: NotRequired[int],
```

1. See [:material-code-brackets: CollectionStatusType](./literals.md#collectionstatustype) 
2. See [:material-code-brackets: CollectionTypeType](./literals.md#collectiontypetype) 
## UpdateCollectionRequestTypeDef

```python
# UpdateCollectionRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import UpdateCollectionRequestTypeDef


def get_value() -> UpdateCollectionRequestTypeDef:
    return {
        "id": ...,
    }


# UpdateCollectionRequestTypeDef definition

class UpdateCollectionRequestTypeDef(TypedDict):
    id: str,
    description: NotRequired[str],
    clientToken: NotRequired[str],
```

## UpdateIamIdentityCenterConfigOptionsTypeDef

```python
# UpdateIamIdentityCenterConfigOptionsTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import UpdateIamIdentityCenterConfigOptionsTypeDef


def get_value() -> UpdateIamIdentityCenterConfigOptionsTypeDef:
    return {
        "userAttribute": ...,
    }


# UpdateIamIdentityCenterConfigOptionsTypeDef definition

class UpdateIamIdentityCenterConfigOptionsTypeDef(TypedDict):
    userAttribute: NotRequired[IamIdentityCenterUserAttributeType],  # (1)
    groupAttribute: NotRequired[IamIdentityCenterGroupAttributeType],  # (2)
```

1. See [:material-code-brackets: IamIdentityCenterUserAttributeType](./literals.md#iamidentitycenteruserattributetype) 
2. See [:material-code-brackets: IamIdentityCenterGroupAttributeType](./literals.md#iamidentitycentergroupattributetype) 
## UpdateLifecyclePolicyRequestTypeDef

```python
# UpdateLifecyclePolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import UpdateLifecyclePolicyRequestTypeDef


def get_value() -> UpdateLifecyclePolicyRequestTypeDef:
    return {
        "type": ...,
    }


# UpdateLifecyclePolicyRequestTypeDef definition

class UpdateLifecyclePolicyRequestTypeDef(TypedDict):
    type: LifecyclePolicyTypeType,  # (1)
    name: str,
    policyVersion: str,
    description: NotRequired[str],
    policy: NotRequired[str],
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: LifecyclePolicyTypeType](./literals.md#lifecyclepolicytypetype) 
## UpdateSecurityPolicyRequestTypeDef

```python
# UpdateSecurityPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import UpdateSecurityPolicyRequestTypeDef


def get_value() -> UpdateSecurityPolicyRequestTypeDef:
    return {
        "type": ...,
    }


# UpdateSecurityPolicyRequestTypeDef definition

class UpdateSecurityPolicyRequestTypeDef(TypedDict):
    type: SecurityPolicyTypeType,  # (1)
    name: str,
    policyVersion: str,
    description: NotRequired[str],
    policy: NotRequired[str],
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: SecurityPolicyTypeType](./literals.md#securitypolicytypetype) 
## UpdateVpcEndpointDetailTypeDef

```python
# UpdateVpcEndpointDetailTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import UpdateVpcEndpointDetailTypeDef


def get_value() -> UpdateVpcEndpointDetailTypeDef:
    return {
        "id": ...,
    }


# UpdateVpcEndpointDetailTypeDef definition

class UpdateVpcEndpointDetailTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    status: NotRequired[VpcEndpointStatusType],  # (1)
    subnetIds: NotRequired[List[str]],
    securityGroupIds: NotRequired[List[str]],
    lastModifiedDate: NotRequired[int],
```

1. See [:material-code-brackets: VpcEndpointStatusType](./literals.md#vpcendpointstatustype) 
## UpdateVpcEndpointRequestTypeDef

```python
# UpdateVpcEndpointRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import UpdateVpcEndpointRequestTypeDef


def get_value() -> UpdateVpcEndpointRequestTypeDef:
    return {
        "id": ...,
    }


# UpdateVpcEndpointRequestTypeDef definition

class UpdateVpcEndpointRequestTypeDef(TypedDict):
    id: str,
    addSubnetIds: NotRequired[Sequence[str]],
    removeSubnetIds: NotRequired[Sequence[str]],
    addSecurityGroupIds: NotRequired[Sequence[str]],
    removeSecurityGroupIds: NotRequired[Sequence[str]],
    clientToken: NotRequired[str],
```

## AccountSettingsDetailTypeDef

```python
# AccountSettingsDetailTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import AccountSettingsDetailTypeDef


def get_value() -> AccountSettingsDetailTypeDef:
    return {
        "capacityLimits": ...,
    }


# AccountSettingsDetailTypeDef definition

class AccountSettingsDetailTypeDef(TypedDict):
    capacityLimits: NotRequired[CapacityLimitsTypeDef],  # (1)
```

1. See [:material-code-braces: CapacityLimitsTypeDef](./type_defs.md#capacitylimitstypedef) 
## UpdateAccountSettingsRequestTypeDef

```python
# UpdateAccountSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import UpdateAccountSettingsRequestTypeDef


def get_value() -> UpdateAccountSettingsRequestTypeDef:
    return {
        "capacityLimits": ...,
    }


# UpdateAccountSettingsRequestTypeDef definition

class UpdateAccountSettingsRequestTypeDef(TypedDict):
    capacityLimits: NotRequired[CapacityLimitsTypeDef],  # (1)
```

1. See [:material-code-braces: CapacityLimitsTypeDef](./type_defs.md#capacitylimitstypedef) 
## BatchGetCollectionResponseTypeDef

```python
# BatchGetCollectionResponseTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import BatchGetCollectionResponseTypeDef


def get_value() -> BatchGetCollectionResponseTypeDef:
    return {
        "collectionDetails": ...,
    }


# BatchGetCollectionResponseTypeDef definition

class BatchGetCollectionResponseTypeDef(TypedDict):
    collectionDetails: List[CollectionDetailTypeDef],  # (1)
    collectionErrorDetails: List[CollectionErrorDetailTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: CollectionDetailTypeDef](./type_defs.md#collectiondetailtypedef) 
2. See [:material-code-braces: CollectionErrorDetailTypeDef](./type_defs.md#collectionerrordetailtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAccessPolicyResponseTypeDef

```python
# CreateAccessPolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import CreateAccessPolicyResponseTypeDef


def get_value() -> CreateAccessPolicyResponseTypeDef:
    return {
        "accessPolicyDetail": ...,
    }


# CreateAccessPolicyResponseTypeDef definition

class CreateAccessPolicyResponseTypeDef(TypedDict):
    accessPolicyDetail: AccessPolicyDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccessPolicyDetailTypeDef](./type_defs.md#accesspolicydetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAccessPolicyResponseTypeDef

```python
# GetAccessPolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import GetAccessPolicyResponseTypeDef


def get_value() -> GetAccessPolicyResponseTypeDef:
    return {
        "accessPolicyDetail": ...,
    }


# GetAccessPolicyResponseTypeDef definition

class GetAccessPolicyResponseTypeDef(TypedDict):
    accessPolicyDetail: AccessPolicyDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccessPolicyDetailTypeDef](./type_defs.md#accesspolicydetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccessPoliciesResponseTypeDef

```python
# ListAccessPoliciesResponseTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import ListAccessPoliciesResponseTypeDef


def get_value() -> ListAccessPoliciesResponseTypeDef:
    return {
        "accessPolicySummaries": ...,
    }


# ListAccessPoliciesResponseTypeDef definition

class ListAccessPoliciesResponseTypeDef(TypedDict):
    accessPolicySummaries: List[AccessPolicySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AccessPolicySummaryTypeDef](./type_defs.md#accesspolicysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAccessPolicyResponseTypeDef

```python
# UpdateAccessPolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import UpdateAccessPolicyResponseTypeDef


def get_value() -> UpdateAccessPolicyResponseTypeDef:
    return {
        "accessPolicyDetail": ...,
    }


# UpdateAccessPolicyResponseTypeDef definition

class UpdateAccessPolicyResponseTypeDef(TypedDict):
    accessPolicyDetail: AccessPolicyDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccessPolicyDetailTypeDef](./type_defs.md#accesspolicydetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetEffectiveLifecyclePolicyRequestTypeDef

```python
# BatchGetEffectiveLifecyclePolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import BatchGetEffectiveLifecyclePolicyRequestTypeDef


def get_value() -> BatchGetEffectiveLifecyclePolicyRequestTypeDef:
    return {
        "resourceIdentifiers": ...,
    }


# BatchGetEffectiveLifecyclePolicyRequestTypeDef definition

class BatchGetEffectiveLifecyclePolicyRequestTypeDef(TypedDict):
    resourceIdentifiers: Sequence[LifecyclePolicyResourceIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: LifecyclePolicyResourceIdentifierTypeDef](./type_defs.md#lifecyclepolicyresourceidentifiertypedef) 
## BatchGetEffectiveLifecyclePolicyResponseTypeDef

```python
# BatchGetEffectiveLifecyclePolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import BatchGetEffectiveLifecyclePolicyResponseTypeDef


def get_value() -> BatchGetEffectiveLifecyclePolicyResponseTypeDef:
    return {
        "effectiveLifecyclePolicyDetails": ...,
    }


# BatchGetEffectiveLifecyclePolicyResponseTypeDef definition

class BatchGetEffectiveLifecyclePolicyResponseTypeDef(TypedDict):
    effectiveLifecyclePolicyDetails: List[EffectiveLifecyclePolicyDetailTypeDef],  # (1)
    effectiveLifecyclePolicyErrorDetails: List[EffectiveLifecyclePolicyErrorDetailTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: EffectiveLifecyclePolicyDetailTypeDef](./type_defs.md#effectivelifecyclepolicydetailtypedef) 
2. See [:material-code-braces: EffectiveLifecyclePolicyErrorDetailTypeDef](./type_defs.md#effectivelifecyclepolicyerrordetailtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetLifecyclePolicyRequestTypeDef

```python
# BatchGetLifecyclePolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import BatchGetLifecyclePolicyRequestTypeDef


def get_value() -> BatchGetLifecyclePolicyRequestTypeDef:
    return {
        "identifiers": ...,
    }


# BatchGetLifecyclePolicyRequestTypeDef definition

class BatchGetLifecyclePolicyRequestTypeDef(TypedDict):
    identifiers: Sequence[LifecyclePolicyIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: LifecyclePolicyIdentifierTypeDef](./type_defs.md#lifecyclepolicyidentifiertypedef) 
## CreateLifecyclePolicyResponseTypeDef

```python
# CreateLifecyclePolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import CreateLifecyclePolicyResponseTypeDef


def get_value() -> CreateLifecyclePolicyResponseTypeDef:
    return {
        "lifecyclePolicyDetail": ...,
    }


# CreateLifecyclePolicyResponseTypeDef definition

class CreateLifecyclePolicyResponseTypeDef(TypedDict):
    lifecyclePolicyDetail: LifecyclePolicyDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LifecyclePolicyDetailTypeDef](./type_defs.md#lifecyclepolicydetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateLifecyclePolicyResponseTypeDef

```python
# UpdateLifecyclePolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import UpdateLifecyclePolicyResponseTypeDef


def get_value() -> UpdateLifecyclePolicyResponseTypeDef:
    return {
        "lifecyclePolicyDetail": ...,
    }


# UpdateLifecyclePolicyResponseTypeDef definition

class UpdateLifecyclePolicyResponseTypeDef(TypedDict):
    lifecyclePolicyDetail: LifecyclePolicyDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LifecyclePolicyDetailTypeDef](./type_defs.md#lifecyclepolicydetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetLifecyclePolicyResponseTypeDef

```python
# BatchGetLifecyclePolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import BatchGetLifecyclePolicyResponseTypeDef


def get_value() -> BatchGetLifecyclePolicyResponseTypeDef:
    return {
        "lifecyclePolicyDetails": ...,
    }


# BatchGetLifecyclePolicyResponseTypeDef definition

class BatchGetLifecyclePolicyResponseTypeDef(TypedDict):
    lifecyclePolicyDetails: List[LifecyclePolicyDetailTypeDef],  # (1)
    lifecyclePolicyErrorDetails: List[LifecyclePolicyErrorDetailTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: LifecyclePolicyDetailTypeDef](./type_defs.md#lifecyclepolicydetailtypedef) 
2. See [:material-code-braces: LifecyclePolicyErrorDetailTypeDef](./type_defs.md#lifecyclepolicyerrordetailtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetVpcEndpointResponseTypeDef

```python
# BatchGetVpcEndpointResponseTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import BatchGetVpcEndpointResponseTypeDef


def get_value() -> BatchGetVpcEndpointResponseTypeDef:
    return {
        "vpcEndpointDetails": ...,
    }


# BatchGetVpcEndpointResponseTypeDef definition

class BatchGetVpcEndpointResponseTypeDef(TypedDict):
    vpcEndpointDetails: List[VpcEndpointDetailTypeDef],  # (1)
    vpcEndpointErrorDetails: List[VpcEndpointErrorDetailTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: VpcEndpointDetailTypeDef](./type_defs.md#vpcendpointdetailtypedef) 
2. See [:material-code-braces: VpcEndpointErrorDetailTypeDef](./type_defs.md#vpcendpointerrordetailtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCollectionsRequestTypeDef

```python
# ListCollectionsRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import ListCollectionsRequestTypeDef


def get_value() -> ListCollectionsRequestTypeDef:
    return {
        "collectionFilters": ...,
    }


# ListCollectionsRequestTypeDef definition

class ListCollectionsRequestTypeDef(TypedDict):
    collectionFilters: NotRequired[CollectionFiltersTypeDef],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: CollectionFiltersTypeDef](./type_defs.md#collectionfilterstypedef) 
## ListCollectionsResponseTypeDef

```python
# ListCollectionsResponseTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import ListCollectionsResponseTypeDef


def get_value() -> ListCollectionsResponseTypeDef:
    return {
        "collectionSummaries": ...,
    }


# ListCollectionsResponseTypeDef definition

class ListCollectionsResponseTypeDef(TypedDict):
    collectionSummaries: List[CollectionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CollectionSummaryTypeDef](./type_defs.md#collectionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCollectionResponseTypeDef

```python
# CreateCollectionResponseTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import CreateCollectionResponseTypeDef


def get_value() -> CreateCollectionResponseTypeDef:
    return {
        "createCollectionDetail": ...,
    }


# CreateCollectionResponseTypeDef definition

class CreateCollectionResponseTypeDef(TypedDict):
    createCollectionDetail: CreateCollectionDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CreateCollectionDetailTypeDef](./type_defs.md#createcollectiondetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCollectionRequestTypeDef

```python
# CreateCollectionRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import CreateCollectionRequestTypeDef


def get_value() -> CreateCollectionRequestTypeDef:
    return {
        "name": ...,
    }


# CreateCollectionRequestTypeDef definition

class CreateCollectionRequestTypeDef(TypedDict):
    name: str,
    type: NotRequired[CollectionTypeType],  # (1)
    description: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    standbyReplicas: NotRequired[StandbyReplicasType],  # (3)
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: CollectionTypeType](./literals.md#collectiontypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: StandbyReplicasType](./literals.md#standbyreplicastype) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateSecurityConfigRequestTypeDef

```python
# CreateSecurityConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import CreateSecurityConfigRequestTypeDef


def get_value() -> CreateSecurityConfigRequestTypeDef:
    return {
        "type": ...,
    }


# CreateSecurityConfigRequestTypeDef definition

class CreateSecurityConfigRequestTypeDef(TypedDict):
    type: SecurityConfigTypeType,  # (1)
    name: str,
    description: NotRequired[str],
    samlOptions: NotRequired[SamlConfigOptionsTypeDef],  # (2)
    iamIdentityCenterOptions: NotRequired[CreateIamIdentityCenterConfigOptionsTypeDef],  # (3)
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: SecurityConfigTypeType](./literals.md#securityconfigtypetype) 
2. See [:material-code-braces: SamlConfigOptionsTypeDef](./type_defs.md#samlconfigoptionstypedef) 
3. See [:material-code-braces: CreateIamIdentityCenterConfigOptionsTypeDef](./type_defs.md#createiamidentitycenterconfigoptionstypedef) 
## CreateSecurityPolicyResponseTypeDef

```python
# CreateSecurityPolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import CreateSecurityPolicyResponseTypeDef


def get_value() -> CreateSecurityPolicyResponseTypeDef:
    return {
        "securityPolicyDetail": ...,
    }


# CreateSecurityPolicyResponseTypeDef definition

class CreateSecurityPolicyResponseTypeDef(TypedDict):
    securityPolicyDetail: SecurityPolicyDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SecurityPolicyDetailTypeDef](./type_defs.md#securitypolicydetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSecurityPolicyResponseTypeDef

```python
# GetSecurityPolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import GetSecurityPolicyResponseTypeDef


def get_value() -> GetSecurityPolicyResponseTypeDef:
    return {
        "securityPolicyDetail": ...,
    }


# GetSecurityPolicyResponseTypeDef definition

class GetSecurityPolicyResponseTypeDef(TypedDict):
    securityPolicyDetail: SecurityPolicyDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SecurityPolicyDetailTypeDef](./type_defs.md#securitypolicydetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSecurityPolicyResponseTypeDef

```python
# UpdateSecurityPolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import UpdateSecurityPolicyResponseTypeDef


def get_value() -> UpdateSecurityPolicyResponseTypeDef:
    return {
        "securityPolicyDetail": ...,
    }


# UpdateSecurityPolicyResponseTypeDef definition

class UpdateSecurityPolicyResponseTypeDef(TypedDict):
    securityPolicyDetail: SecurityPolicyDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SecurityPolicyDetailTypeDef](./type_defs.md#securitypolicydetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateVpcEndpointResponseTypeDef

```python
# CreateVpcEndpointResponseTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import CreateVpcEndpointResponseTypeDef


def get_value() -> CreateVpcEndpointResponseTypeDef:
    return {
        "createVpcEndpointDetail": ...,
    }


# CreateVpcEndpointResponseTypeDef definition

class CreateVpcEndpointResponseTypeDef(TypedDict):
    createVpcEndpointDetail: CreateVpcEndpointDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CreateVpcEndpointDetailTypeDef](./type_defs.md#createvpcendpointdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteCollectionResponseTypeDef

```python
# DeleteCollectionResponseTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import DeleteCollectionResponseTypeDef


def get_value() -> DeleteCollectionResponseTypeDef:
    return {
        "deleteCollectionDetail": ...,
    }


# DeleteCollectionResponseTypeDef definition

class DeleteCollectionResponseTypeDef(TypedDict):
    deleteCollectionDetail: DeleteCollectionDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeleteCollectionDetailTypeDef](./type_defs.md#deletecollectiondetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteVpcEndpointResponseTypeDef

```python
# DeleteVpcEndpointResponseTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import DeleteVpcEndpointResponseTypeDef


def get_value() -> DeleteVpcEndpointResponseTypeDef:
    return {
        "deleteVpcEndpointDetail": ...,
    }


# DeleteVpcEndpointResponseTypeDef definition

class DeleteVpcEndpointResponseTypeDef(TypedDict):
    deleteVpcEndpointDetail: DeleteVpcEndpointDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeleteVpcEndpointDetailTypeDef](./type_defs.md#deletevpcendpointdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPoliciesStatsResponseTypeDef

```python
# GetPoliciesStatsResponseTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import GetPoliciesStatsResponseTypeDef


def get_value() -> GetPoliciesStatsResponseTypeDef:
    return {
        "AccessPolicyStats": ...,
    }


# GetPoliciesStatsResponseTypeDef definition

class GetPoliciesStatsResponseTypeDef(TypedDict):
    AccessPolicyStats: AccessPolicyStatsTypeDef,  # (1)
    SecurityPolicyStats: SecurityPolicyStatsTypeDef,  # (2)
    SecurityConfigStats: SecurityConfigStatsTypeDef,  # (3)
    LifecyclePolicyStats: LifecyclePolicyStatsTypeDef,  # (4)
    TotalPolicyCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: AccessPolicyStatsTypeDef](./type_defs.md#accesspolicystatstypedef) 
2. See [:material-code-braces: SecurityPolicyStatsTypeDef](./type_defs.md#securitypolicystatstypedef) 
3. See [:material-code-braces: SecurityConfigStatsTypeDef](./type_defs.md#securityconfigstatstypedef) 
4. See [:material-code-braces: LifecyclePolicyStatsTypeDef](./type_defs.md#lifecyclepolicystatstypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SecurityConfigDetailTypeDef

```python
# SecurityConfigDetailTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import SecurityConfigDetailTypeDef


def get_value() -> SecurityConfigDetailTypeDef:
    return {
        "id": ...,
    }


# SecurityConfigDetailTypeDef definition

class SecurityConfigDetailTypeDef(TypedDict):
    id: NotRequired[str],
    type: NotRequired[SecurityConfigTypeType],  # (1)
    configVersion: NotRequired[str],
    description: NotRequired[str],
    samlOptions: NotRequired[SamlConfigOptionsTypeDef],  # (2)
    iamIdentityCenterOptions: NotRequired[IamIdentityCenterConfigOptionsTypeDef],  # (3)
    createdDate: NotRequired[int],
    lastModifiedDate: NotRequired[int],
```

1. See [:material-code-brackets: SecurityConfigTypeType](./literals.md#securityconfigtypetype) 
2. See [:material-code-braces: SamlConfigOptionsTypeDef](./type_defs.md#samlconfigoptionstypedef) 
3. See [:material-code-braces: IamIdentityCenterConfigOptionsTypeDef](./type_defs.md#iamidentitycenterconfigoptionstypedef) 
## ListLifecyclePoliciesResponseTypeDef

```python
# ListLifecyclePoliciesResponseTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import ListLifecyclePoliciesResponseTypeDef


def get_value() -> ListLifecyclePoliciesResponseTypeDef:
    return {
        "lifecyclePolicySummaries": ...,
    }


# ListLifecyclePoliciesResponseTypeDef definition

class ListLifecyclePoliciesResponseTypeDef(TypedDict):
    lifecyclePolicySummaries: List[LifecyclePolicySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: LifecyclePolicySummaryTypeDef](./type_defs.md#lifecyclepolicysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSecurityConfigsResponseTypeDef

```python
# ListSecurityConfigsResponseTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import ListSecurityConfigsResponseTypeDef


def get_value() -> ListSecurityConfigsResponseTypeDef:
    return {
        "securityConfigSummaries": ...,
    }


# ListSecurityConfigsResponseTypeDef definition

class ListSecurityConfigsResponseTypeDef(TypedDict):
    securityConfigSummaries: List[SecurityConfigSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SecurityConfigSummaryTypeDef](./type_defs.md#securityconfigsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSecurityPoliciesResponseTypeDef

```python
# ListSecurityPoliciesResponseTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import ListSecurityPoliciesResponseTypeDef


def get_value() -> ListSecurityPoliciesResponseTypeDef:
    return {
        "securityPolicySummaries": ...,
    }


# ListSecurityPoliciesResponseTypeDef definition

class ListSecurityPoliciesResponseTypeDef(TypedDict):
    securityPolicySummaries: List[SecurityPolicySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SecurityPolicySummaryTypeDef](./type_defs.md#securitypolicysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVpcEndpointsRequestTypeDef

```python
# ListVpcEndpointsRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import ListVpcEndpointsRequestTypeDef


def get_value() -> ListVpcEndpointsRequestTypeDef:
    return {
        "vpcEndpointFilters": ...,
    }


# ListVpcEndpointsRequestTypeDef definition

class ListVpcEndpointsRequestTypeDef(TypedDict):
    vpcEndpointFilters: NotRequired[VpcEndpointFiltersTypeDef],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: VpcEndpointFiltersTypeDef](./type_defs.md#vpcendpointfilterstypedef) 
## ListVpcEndpointsResponseTypeDef

```python
# ListVpcEndpointsResponseTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import ListVpcEndpointsResponseTypeDef


def get_value() -> ListVpcEndpointsResponseTypeDef:
    return {
        "vpcEndpointSummaries": ...,
    }


# ListVpcEndpointsResponseTypeDef definition

class ListVpcEndpointsResponseTypeDef(TypedDict):
    vpcEndpointSummaries: List[VpcEndpointSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: VpcEndpointSummaryTypeDef](./type_defs.md#vpcendpointsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCollectionResponseTypeDef

```python
# UpdateCollectionResponseTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import UpdateCollectionResponseTypeDef


def get_value() -> UpdateCollectionResponseTypeDef:
    return {
        "updateCollectionDetail": ...,
    }


# UpdateCollectionResponseTypeDef definition

class UpdateCollectionResponseTypeDef(TypedDict):
    updateCollectionDetail: UpdateCollectionDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UpdateCollectionDetailTypeDef](./type_defs.md#updatecollectiondetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSecurityConfigRequestTypeDef

```python
# UpdateSecurityConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import UpdateSecurityConfigRequestTypeDef


def get_value() -> UpdateSecurityConfigRequestTypeDef:
    return {
        "id": ...,
    }


# UpdateSecurityConfigRequestTypeDef definition

class UpdateSecurityConfigRequestTypeDef(TypedDict):
    id: str,
    configVersion: str,
    description: NotRequired[str],
    samlOptions: NotRequired[SamlConfigOptionsTypeDef],  # (1)
    iamIdentityCenterOptionsUpdates: NotRequired[UpdateIamIdentityCenterConfigOptionsTypeDef],  # (2)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: SamlConfigOptionsTypeDef](./type_defs.md#samlconfigoptionstypedef) 
2. See [:material-code-braces: UpdateIamIdentityCenterConfigOptionsTypeDef](./type_defs.md#updateiamidentitycenterconfigoptionstypedef) 
## UpdateVpcEndpointResponseTypeDef

```python
# UpdateVpcEndpointResponseTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import UpdateVpcEndpointResponseTypeDef


def get_value() -> UpdateVpcEndpointResponseTypeDef:
    return {
        "UpdateVpcEndpointDetail": ...,
    }


# UpdateVpcEndpointResponseTypeDef definition

class UpdateVpcEndpointResponseTypeDef(TypedDict):
    UpdateVpcEndpointDetail: UpdateVpcEndpointDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UpdateVpcEndpointDetailTypeDef](./type_defs.md#updatevpcendpointdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAccountSettingsResponseTypeDef

```python
# GetAccountSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import GetAccountSettingsResponseTypeDef


def get_value() -> GetAccountSettingsResponseTypeDef:
    return {
        "accountSettingsDetail": ...,
    }


# GetAccountSettingsResponseTypeDef definition

class GetAccountSettingsResponseTypeDef(TypedDict):
    accountSettingsDetail: AccountSettingsDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountSettingsDetailTypeDef](./type_defs.md#accountsettingsdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAccountSettingsResponseTypeDef

```python
# UpdateAccountSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import UpdateAccountSettingsResponseTypeDef


def get_value() -> UpdateAccountSettingsResponseTypeDef:
    return {
        "accountSettingsDetail": ...,
    }


# UpdateAccountSettingsResponseTypeDef definition

class UpdateAccountSettingsResponseTypeDef(TypedDict):
    accountSettingsDetail: AccountSettingsDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountSettingsDetailTypeDef](./type_defs.md#accountsettingsdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSecurityConfigResponseTypeDef

```python
# CreateSecurityConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import CreateSecurityConfigResponseTypeDef


def get_value() -> CreateSecurityConfigResponseTypeDef:
    return {
        "securityConfigDetail": ...,
    }


# CreateSecurityConfigResponseTypeDef definition

class CreateSecurityConfigResponseTypeDef(TypedDict):
    securityConfigDetail: SecurityConfigDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SecurityConfigDetailTypeDef](./type_defs.md#securityconfigdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSecurityConfigResponseTypeDef

```python
# GetSecurityConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import GetSecurityConfigResponseTypeDef


def get_value() -> GetSecurityConfigResponseTypeDef:
    return {
        "securityConfigDetail": ...,
    }


# GetSecurityConfigResponseTypeDef definition

class GetSecurityConfigResponseTypeDef(TypedDict):
    securityConfigDetail: SecurityConfigDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SecurityConfigDetailTypeDef](./type_defs.md#securityconfigdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSecurityConfigResponseTypeDef

```python
# UpdateSecurityConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_opensearchserverless.type_defs import UpdateSecurityConfigResponseTypeDef


def get_value() -> UpdateSecurityConfigResponseTypeDef:
    return {
        "securityConfigDetail": ...,
    }


# UpdateSecurityConfigResponseTypeDef definition

class UpdateSecurityConfigResponseTypeDef(TypedDict):
    securityConfigDetail: SecurityConfigDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SecurityConfigDetailTypeDef](./type_defs.md#securityconfigdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
