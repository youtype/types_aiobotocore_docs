# Type definitions

> [Index](../README.md) > [OpenSearchServiceServerless](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [OpenSearchServiceServerless](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless)
    type annotations stubs module [types-aiobotocore-opensearchserverless](https://pypi.org/project/types-aiobotocore-opensearchserverless/).



## AccessPolicyDetailTypeDef

```python
# AccessPolicyDetailTypeDef definition

class AccessPolicyDetailTypeDef(TypedDict):
    createdDate: NotRequired[int],
    description: NotRequired[str],
    lastModifiedDate: NotRequired[int],
    name: NotRequired[str],
    policy: NotRequired[Dict[str, Any]],
    policyVersion: NotRequired[str],
    type: NotRequired[AccessPolicyTypeType],  # (1)
```

1. See [:material-code-brackets: AccessPolicyTypeType](./literals.md#accesspolicytypetype) 
## AccessPolicyStatsTypeDef

```python
# AccessPolicyStatsTypeDef definition

class AccessPolicyStatsTypeDef(TypedDict):
    DataPolicyCount: NotRequired[int],
```

## AccessPolicySummaryTypeDef

```python
# AccessPolicySummaryTypeDef definition

class AccessPolicySummaryTypeDef(TypedDict):
    createdDate: NotRequired[int],
    description: NotRequired[str],
    lastModifiedDate: NotRequired[int],
    name: NotRequired[str],
    policyVersion: NotRequired[str],
    type: NotRequired[AccessPolicyTypeType],  # (1)
```

1. See [:material-code-brackets: AccessPolicyTypeType](./literals.md#accesspolicytypetype) 
## CapacityLimitsTypeDef

```python
# CapacityLimitsTypeDef definition

class CapacityLimitsTypeDef(TypedDict):
    maxIndexingCapacityInOCU: NotRequired[int],
    maxSearchCapacityInOCU: NotRequired[int],
```

## BatchGetCollectionRequestRequestTypeDef

```python
# BatchGetCollectionRequestRequestTypeDef definition

class BatchGetCollectionRequestRequestTypeDef(TypedDict):
    ids: NotRequired[Sequence[str]],
    names: NotRequired[Sequence[str]],
```

## CollectionDetailTypeDef

```python
# CollectionDetailTypeDef definition

class CollectionDetailTypeDef(TypedDict):
    arn: NotRequired[str],
    collectionEndpoint: NotRequired[str],
    createdDate: NotRequired[int],
    dashboardEndpoint: NotRequired[str],
    description: NotRequired[str],
    failureCode: NotRequired[str],
    failureMessage: NotRequired[str],
    id: NotRequired[str],
    kmsKeyArn: NotRequired[str],
    lastModifiedDate: NotRequired[int],
    name: NotRequired[str],
    standbyReplicas: NotRequired[StandbyReplicasType],  # (1)
    status: NotRequired[CollectionStatusType],  # (2)
    type: NotRequired[CollectionTypeType],  # (3)
```

1. See [:material-code-brackets: StandbyReplicasType](./literals.md#standbyreplicastype) 
2. See [:material-code-brackets: CollectionStatusType](./literals.md#collectionstatustype) 
3. See [:material-code-brackets: CollectionTypeType](./literals.md#collectiontypetype) 
## CollectionErrorDetailTypeDef

```python
# CollectionErrorDetailTypeDef definition

class CollectionErrorDetailTypeDef(TypedDict):
    errorCode: NotRequired[str],
    errorMessage: NotRequired[str],
    id: NotRequired[str],
    name: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
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
# LifecyclePolicyResourceIdentifierTypeDef definition

class LifecyclePolicyResourceIdentifierTypeDef(TypedDict):
    resource: str,
    type: LifecyclePolicyTypeType,  # (1)
```

1. See [:material-code-brackets: LifecyclePolicyTypeType](./literals.md#lifecyclepolicytypetype) 
## EffectiveLifecyclePolicyDetailTypeDef

```python
# EffectiveLifecyclePolicyDetailTypeDef definition

class EffectiveLifecyclePolicyDetailTypeDef(TypedDict):
    noMinRetentionPeriod: NotRequired[bool],
    policyName: NotRequired[str],
    resource: NotRequired[str],
    resourceType: NotRequired[ResourceTypeType],  # (1)
    retentionPeriod: NotRequired[str],
    type: NotRequired[LifecyclePolicyTypeType],  # (2)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: LifecyclePolicyTypeType](./literals.md#lifecyclepolicytypetype) 
## EffectiveLifecyclePolicyErrorDetailTypeDef

```python
# EffectiveLifecyclePolicyErrorDetailTypeDef definition

class EffectiveLifecyclePolicyErrorDetailTypeDef(TypedDict):
    errorCode: NotRequired[str],
    errorMessage: NotRequired[str],
    resource: NotRequired[str],
    type: NotRequired[LifecyclePolicyTypeType],  # (1)
```

1. See [:material-code-brackets: LifecyclePolicyTypeType](./literals.md#lifecyclepolicytypetype) 
## LifecyclePolicyIdentifierTypeDef

```python
# LifecyclePolicyIdentifierTypeDef definition

class LifecyclePolicyIdentifierTypeDef(TypedDict):
    name: str,
    type: LifecyclePolicyTypeType,  # (1)
```

1. See [:material-code-brackets: LifecyclePolicyTypeType](./literals.md#lifecyclepolicytypetype) 
## LifecyclePolicyDetailTypeDef

```python
# LifecyclePolicyDetailTypeDef definition

class LifecyclePolicyDetailTypeDef(TypedDict):
    createdDate: NotRequired[int],
    description: NotRequired[str],
    lastModifiedDate: NotRequired[int],
    name: NotRequired[str],
    policy: NotRequired[Dict[str, Any]],
    policyVersion: NotRequired[str],
    type: NotRequired[LifecyclePolicyTypeType],  # (1)
```

1. See [:material-code-brackets: LifecyclePolicyTypeType](./literals.md#lifecyclepolicytypetype) 
## LifecyclePolicyErrorDetailTypeDef

```python
# LifecyclePolicyErrorDetailTypeDef definition

class LifecyclePolicyErrorDetailTypeDef(TypedDict):
    errorCode: NotRequired[str],
    errorMessage: NotRequired[str],
    name: NotRequired[str],
    type: NotRequired[LifecyclePolicyTypeType],  # (1)
```

1. See [:material-code-brackets: LifecyclePolicyTypeType](./literals.md#lifecyclepolicytypetype) 
## BatchGetVpcEndpointRequestRequestTypeDef

```python
# BatchGetVpcEndpointRequestRequestTypeDef definition

class BatchGetVpcEndpointRequestRequestTypeDef(TypedDict):
    ids: Sequence[str],
```

## VpcEndpointDetailTypeDef

```python
# VpcEndpointDetailTypeDef definition

class VpcEndpointDetailTypeDef(TypedDict):
    createdDate: NotRequired[int],
    failureCode: NotRequired[str],
    failureMessage: NotRequired[str],
    id: NotRequired[str],
    name: NotRequired[str],
    securityGroupIds: NotRequired[List[str]],
    status: NotRequired[VpcEndpointStatusType],  # (1)
    subnetIds: NotRequired[List[str]],
    vpcId: NotRequired[str],
```

1. See [:material-code-brackets: VpcEndpointStatusType](./literals.md#vpcendpointstatustype) 
## VpcEndpointErrorDetailTypeDef

```python
# VpcEndpointErrorDetailTypeDef definition

class VpcEndpointErrorDetailTypeDef(TypedDict):
    errorCode: NotRequired[str],
    errorMessage: NotRequired[str],
    id: NotRequired[str],
```

## CollectionFiltersTypeDef

```python
# CollectionFiltersTypeDef definition

class CollectionFiltersTypeDef(TypedDict):
    name: NotRequired[str],
    status: NotRequired[CollectionStatusType],  # (1)
```

1. See [:material-code-brackets: CollectionStatusType](./literals.md#collectionstatustype) 
## CollectionSummaryTypeDef

```python
# CollectionSummaryTypeDef definition

class CollectionSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    id: NotRequired[str],
    name: NotRequired[str],
    status: NotRequired[CollectionStatusType],  # (1)
```

1. See [:material-code-brackets: CollectionStatusType](./literals.md#collectionstatustype) 
## CreateAccessPolicyRequestRequestTypeDef

```python
# CreateAccessPolicyRequestRequestTypeDef definition

class CreateAccessPolicyRequestRequestTypeDef(TypedDict):
    name: str,
    policy: str,
    type: AccessPolicyTypeType,  # (1)
    clientToken: NotRequired[str],
    description: NotRequired[str],
```

1. See [:material-code-brackets: AccessPolicyTypeType](./literals.md#accesspolicytypetype) 
## CreateCollectionDetailTypeDef

```python
# CreateCollectionDetailTypeDef definition

class CreateCollectionDetailTypeDef(TypedDict):
    arn: NotRequired[str],
    createdDate: NotRequired[int],
    description: NotRequired[str],
    id: NotRequired[str],
    kmsKeyArn: NotRequired[str],
    lastModifiedDate: NotRequired[int],
    name: NotRequired[str],
    standbyReplicas: NotRequired[StandbyReplicasType],  # (1)
    status: NotRequired[CollectionStatusType],  # (2)
    type: NotRequired[CollectionTypeType],  # (3)
```

1. See [:material-code-brackets: StandbyReplicasType](./literals.md#standbyreplicastype) 
2. See [:material-code-brackets: CollectionStatusType](./literals.md#collectionstatustype) 
3. See [:material-code-brackets: CollectionTypeType](./literals.md#collectiontypetype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: str,
    value: str,
```

## CreateLifecyclePolicyRequestRequestTypeDef

```python
# CreateLifecyclePolicyRequestRequestTypeDef definition

class CreateLifecyclePolicyRequestRequestTypeDef(TypedDict):
    name: str,
    policy: str,
    type: LifecyclePolicyTypeType,  # (1)
    clientToken: NotRequired[str],
    description: NotRequired[str],
```

1. See [:material-code-brackets: LifecyclePolicyTypeType](./literals.md#lifecyclepolicytypetype) 
## SamlConfigOptionsTypeDef

```python
# SamlConfigOptionsTypeDef definition

class SamlConfigOptionsTypeDef(TypedDict):
    metadata: str,
    groupAttribute: NotRequired[str],
    sessionTimeout: NotRequired[int],
    userAttribute: NotRequired[str],
```

## CreateSecurityPolicyRequestRequestTypeDef

```python
# CreateSecurityPolicyRequestRequestTypeDef definition

class CreateSecurityPolicyRequestRequestTypeDef(TypedDict):
    name: str,
    policy: str,
    type: SecurityPolicyTypeType,  # (1)
    clientToken: NotRequired[str],
    description: NotRequired[str],
```

1. See [:material-code-brackets: SecurityPolicyTypeType](./literals.md#securitypolicytypetype) 
## SecurityPolicyDetailTypeDef

```python
# SecurityPolicyDetailTypeDef definition

class SecurityPolicyDetailTypeDef(TypedDict):
    createdDate: NotRequired[int],
    description: NotRequired[str],
    lastModifiedDate: NotRequired[int],
    name: NotRequired[str],
    policy: NotRequired[Dict[str, Any]],
    policyVersion: NotRequired[str],
    type: NotRequired[SecurityPolicyTypeType],  # (1)
```

1. See [:material-code-brackets: SecurityPolicyTypeType](./literals.md#securitypolicytypetype) 
## CreateVpcEndpointDetailTypeDef

```python
# CreateVpcEndpointDetailTypeDef definition

class CreateVpcEndpointDetailTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    status: NotRequired[VpcEndpointStatusType],  # (1)
```

1. See [:material-code-brackets: VpcEndpointStatusType](./literals.md#vpcendpointstatustype) 
## CreateVpcEndpointRequestRequestTypeDef

```python
# CreateVpcEndpointRequestRequestTypeDef definition

class CreateVpcEndpointRequestRequestTypeDef(TypedDict):
    name: str,
    subnetIds: Sequence[str],
    vpcId: str,
    clientToken: NotRequired[str],
    securityGroupIds: NotRequired[Sequence[str]],
```

## DeleteAccessPolicyRequestRequestTypeDef

```python
# DeleteAccessPolicyRequestRequestTypeDef definition

class DeleteAccessPolicyRequestRequestTypeDef(TypedDict):
    name: str,
    type: AccessPolicyTypeType,  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: AccessPolicyTypeType](./literals.md#accesspolicytypetype) 
## DeleteCollectionDetailTypeDef

```python
# DeleteCollectionDetailTypeDef definition

class DeleteCollectionDetailTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    status: NotRequired[CollectionStatusType],  # (1)
```

1. See [:material-code-brackets: CollectionStatusType](./literals.md#collectionstatustype) 
## DeleteCollectionRequestRequestTypeDef

```python
# DeleteCollectionRequestRequestTypeDef definition

class DeleteCollectionRequestRequestTypeDef(TypedDict):
    id: str,
    clientToken: NotRequired[str],
```

## DeleteLifecyclePolicyRequestRequestTypeDef

```python
# DeleteLifecyclePolicyRequestRequestTypeDef definition

class DeleteLifecyclePolicyRequestRequestTypeDef(TypedDict):
    name: str,
    type: LifecyclePolicyTypeType,  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: LifecyclePolicyTypeType](./literals.md#lifecyclepolicytypetype) 
## DeleteSecurityConfigRequestRequestTypeDef

```python
# DeleteSecurityConfigRequestRequestTypeDef definition

class DeleteSecurityConfigRequestRequestTypeDef(TypedDict):
    id: str,
    clientToken: NotRequired[str],
```

## DeleteSecurityPolicyRequestRequestTypeDef

```python
# DeleteSecurityPolicyRequestRequestTypeDef definition

class DeleteSecurityPolicyRequestRequestTypeDef(TypedDict):
    name: str,
    type: SecurityPolicyTypeType,  # (1)
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: SecurityPolicyTypeType](./literals.md#securitypolicytypetype) 
## DeleteVpcEndpointDetailTypeDef

```python
# DeleteVpcEndpointDetailTypeDef definition

class DeleteVpcEndpointDetailTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    status: NotRequired[VpcEndpointStatusType],  # (1)
```

1. See [:material-code-brackets: VpcEndpointStatusType](./literals.md#vpcendpointstatustype) 
## DeleteVpcEndpointRequestRequestTypeDef

```python
# DeleteVpcEndpointRequestRequestTypeDef definition

class DeleteVpcEndpointRequestRequestTypeDef(TypedDict):
    id: str,
    clientToken: NotRequired[str],
```

## GetAccessPolicyRequestRequestTypeDef

```python
# GetAccessPolicyRequestRequestTypeDef definition

class GetAccessPolicyRequestRequestTypeDef(TypedDict):
    name: str,
    type: AccessPolicyTypeType,  # (1)
```

1. See [:material-code-brackets: AccessPolicyTypeType](./literals.md#accesspolicytypetype) 
## LifecyclePolicyStatsTypeDef

```python
# LifecyclePolicyStatsTypeDef definition

class LifecyclePolicyStatsTypeDef(TypedDict):
    RetentionPolicyCount: NotRequired[int],
```

## SecurityConfigStatsTypeDef

```python
# SecurityConfigStatsTypeDef definition

class SecurityConfigStatsTypeDef(TypedDict):
    SamlConfigCount: NotRequired[int],
```

## SecurityPolicyStatsTypeDef

```python
# SecurityPolicyStatsTypeDef definition

class SecurityPolicyStatsTypeDef(TypedDict):
    EncryptionPolicyCount: NotRequired[int],
    NetworkPolicyCount: NotRequired[int],
```

## GetSecurityConfigRequestRequestTypeDef

```python
# GetSecurityConfigRequestRequestTypeDef definition

class GetSecurityConfigRequestRequestTypeDef(TypedDict):
    id: str,
```

## GetSecurityPolicyRequestRequestTypeDef

```python
# GetSecurityPolicyRequestRequestTypeDef definition

class GetSecurityPolicyRequestRequestTypeDef(TypedDict):
    name: str,
    type: SecurityPolicyTypeType,  # (1)
```

1. See [:material-code-brackets: SecurityPolicyTypeType](./literals.md#securitypolicytypetype) 
## LifecyclePolicySummaryTypeDef

```python
# LifecyclePolicySummaryTypeDef definition

class LifecyclePolicySummaryTypeDef(TypedDict):
    createdDate: NotRequired[int],
    description: NotRequired[str],
    lastModifiedDate: NotRequired[int],
    name: NotRequired[str],
    policyVersion: NotRequired[str],
    type: NotRequired[LifecyclePolicyTypeType],  # (1)
```

1. See [:material-code-brackets: LifecyclePolicyTypeType](./literals.md#lifecyclepolicytypetype) 
## ListAccessPoliciesRequestRequestTypeDef

```python
# ListAccessPoliciesRequestRequestTypeDef definition

class ListAccessPoliciesRequestRequestTypeDef(TypedDict):
    type: AccessPolicyTypeType,  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    resource: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: AccessPolicyTypeType](./literals.md#accesspolicytypetype) 
## ListLifecyclePoliciesRequestRequestTypeDef

```python
# ListLifecyclePoliciesRequestRequestTypeDef definition

class ListLifecyclePoliciesRequestRequestTypeDef(TypedDict):
    type: LifecyclePolicyTypeType,  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    resources: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: LifecyclePolicyTypeType](./literals.md#lifecyclepolicytypetype) 
## ListSecurityConfigsRequestRequestTypeDef

```python
# ListSecurityConfigsRequestRequestTypeDef definition

class ListSecurityConfigsRequestRequestTypeDef(TypedDict):
    type: SecurityConfigTypeType,  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: SecurityConfigTypeType](./literals.md#securityconfigtypetype) 
## SecurityConfigSummaryTypeDef

```python
# SecurityConfigSummaryTypeDef definition

class SecurityConfigSummaryTypeDef(TypedDict):
    configVersion: NotRequired[str],
    createdDate: NotRequired[int],
    description: NotRequired[str],
    id: NotRequired[str],
    lastModifiedDate: NotRequired[int],
    type: NotRequired[SecurityConfigTypeType],  # (1)
```

1. See [:material-code-brackets: SecurityConfigTypeType](./literals.md#securityconfigtypetype) 
## ListSecurityPoliciesRequestRequestTypeDef

```python
# ListSecurityPoliciesRequestRequestTypeDef definition

class ListSecurityPoliciesRequestRequestTypeDef(TypedDict):
    type: SecurityPolicyTypeType,  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    resource: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: SecurityPolicyTypeType](./literals.md#securitypolicytypetype) 
## SecurityPolicySummaryTypeDef

```python
# SecurityPolicySummaryTypeDef definition

class SecurityPolicySummaryTypeDef(TypedDict):
    createdDate: NotRequired[int],
    description: NotRequired[str],
    lastModifiedDate: NotRequired[int],
    name: NotRequired[str],
    policyVersion: NotRequired[str],
    type: NotRequired[SecurityPolicyTypeType],  # (1)
```

1. See [:material-code-brackets: SecurityPolicyTypeType](./literals.md#securitypolicytypetype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## VpcEndpointFiltersTypeDef

```python
# VpcEndpointFiltersTypeDef definition

class VpcEndpointFiltersTypeDef(TypedDict):
    status: NotRequired[VpcEndpointStatusType],  # (1)
```

1. See [:material-code-brackets: VpcEndpointStatusType](./literals.md#vpcendpointstatustype) 
## VpcEndpointSummaryTypeDef

```python
# VpcEndpointSummaryTypeDef definition

class VpcEndpointSummaryTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    status: NotRequired[VpcEndpointStatusType],  # (1)
```

1. See [:material-code-brackets: VpcEndpointStatusType](./literals.md#vpcendpointstatustype) 
## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateAccessPolicyRequestRequestTypeDef

```python
# UpdateAccessPolicyRequestRequestTypeDef definition

class UpdateAccessPolicyRequestRequestTypeDef(TypedDict):
    name: str,
    policyVersion: str,
    type: AccessPolicyTypeType,  # (1)
    clientToken: NotRequired[str],
    description: NotRequired[str],
    policy: NotRequired[str],
```

1. See [:material-code-brackets: AccessPolicyTypeType](./literals.md#accesspolicytypetype) 
## UpdateCollectionDetailTypeDef

```python
# UpdateCollectionDetailTypeDef definition

class UpdateCollectionDetailTypeDef(TypedDict):
    arn: NotRequired[str],
    createdDate: NotRequired[int],
    description: NotRequired[str],
    id: NotRequired[str],
    lastModifiedDate: NotRequired[int],
    name: NotRequired[str],
    status: NotRequired[CollectionStatusType],  # (1)
    type: NotRequired[CollectionTypeType],  # (2)
```

1. See [:material-code-brackets: CollectionStatusType](./literals.md#collectionstatustype) 
2. See [:material-code-brackets: CollectionTypeType](./literals.md#collectiontypetype) 
## UpdateCollectionRequestRequestTypeDef

```python
# UpdateCollectionRequestRequestTypeDef definition

class UpdateCollectionRequestRequestTypeDef(TypedDict):
    id: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
```

## UpdateLifecyclePolicyRequestRequestTypeDef

```python
# UpdateLifecyclePolicyRequestRequestTypeDef definition

class UpdateLifecyclePolicyRequestRequestTypeDef(TypedDict):
    name: str,
    policyVersion: str,
    type: LifecyclePolicyTypeType,  # (1)
    clientToken: NotRequired[str],
    description: NotRequired[str],
    policy: NotRequired[str],
```

1. See [:material-code-brackets: LifecyclePolicyTypeType](./literals.md#lifecyclepolicytypetype) 
## UpdateSecurityPolicyRequestRequestTypeDef

```python
# UpdateSecurityPolicyRequestRequestTypeDef definition

class UpdateSecurityPolicyRequestRequestTypeDef(TypedDict):
    name: str,
    policyVersion: str,
    type: SecurityPolicyTypeType,  # (1)
    clientToken: NotRequired[str],
    description: NotRequired[str],
    policy: NotRequired[str],
```

1. See [:material-code-brackets: SecurityPolicyTypeType](./literals.md#securitypolicytypetype) 
## UpdateVpcEndpointDetailTypeDef

```python
# UpdateVpcEndpointDetailTypeDef definition

class UpdateVpcEndpointDetailTypeDef(TypedDict):
    id: NotRequired[str],
    lastModifiedDate: NotRequired[int],
    name: NotRequired[str],
    securityGroupIds: NotRequired[List[str]],
    status: NotRequired[VpcEndpointStatusType],  # (1)
    subnetIds: NotRequired[List[str]],
```

1. See [:material-code-brackets: VpcEndpointStatusType](./literals.md#vpcendpointstatustype) 
## UpdateVpcEndpointRequestRequestTypeDef

```python
# UpdateVpcEndpointRequestRequestTypeDef definition

class UpdateVpcEndpointRequestRequestTypeDef(TypedDict):
    id: str,
    addSecurityGroupIds: NotRequired[Sequence[str]],
    addSubnetIds: NotRequired[Sequence[str]],
    clientToken: NotRequired[str],
    removeSecurityGroupIds: NotRequired[Sequence[str]],
    removeSubnetIds: NotRequired[Sequence[str]],
```

## AccountSettingsDetailTypeDef

```python
# AccountSettingsDetailTypeDef definition

class AccountSettingsDetailTypeDef(TypedDict):
    capacityLimits: NotRequired[CapacityLimitsTypeDef],  # (1)
```

1. See [:material-code-braces: CapacityLimitsTypeDef](./type_defs.md#capacitylimitstypedef) 
## UpdateAccountSettingsRequestRequestTypeDef

```python
# UpdateAccountSettingsRequestRequestTypeDef definition

class UpdateAccountSettingsRequestRequestTypeDef(TypedDict):
    capacityLimits: NotRequired[CapacityLimitsTypeDef],  # (1)
```

1. See [:material-code-braces: CapacityLimitsTypeDef](./type_defs.md#capacitylimitstypedef) 
## BatchGetCollectionResponseTypeDef

```python
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
# CreateAccessPolicyResponseTypeDef definition

class CreateAccessPolicyResponseTypeDef(TypedDict):
    accessPolicyDetail: AccessPolicyDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccessPolicyDetailTypeDef](./type_defs.md#accesspolicydetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAccessPolicyResponseTypeDef

```python
# GetAccessPolicyResponseTypeDef definition

class GetAccessPolicyResponseTypeDef(TypedDict):
    accessPolicyDetail: AccessPolicyDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccessPolicyDetailTypeDef](./type_defs.md#accesspolicydetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccessPoliciesResponseTypeDef

```python
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
# UpdateAccessPolicyResponseTypeDef definition

class UpdateAccessPolicyResponseTypeDef(TypedDict):
    accessPolicyDetail: AccessPolicyDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccessPolicyDetailTypeDef](./type_defs.md#accesspolicydetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetEffectiveLifecyclePolicyRequestRequestTypeDef

```python
# BatchGetEffectiveLifecyclePolicyRequestRequestTypeDef definition

class BatchGetEffectiveLifecyclePolicyRequestRequestTypeDef(TypedDict):
    resourceIdentifiers: Sequence[LifecyclePolicyResourceIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: LifecyclePolicyResourceIdentifierTypeDef](./type_defs.md#lifecyclepolicyresourceidentifiertypedef) 
## BatchGetEffectiveLifecyclePolicyResponseTypeDef

```python
# BatchGetEffectiveLifecyclePolicyResponseTypeDef definition

class BatchGetEffectiveLifecyclePolicyResponseTypeDef(TypedDict):
    effectiveLifecyclePolicyDetails: List[EffectiveLifecyclePolicyDetailTypeDef],  # (1)
    effectiveLifecyclePolicyErrorDetails: List[EffectiveLifecyclePolicyErrorDetailTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: EffectiveLifecyclePolicyDetailTypeDef](./type_defs.md#effectivelifecyclepolicydetailtypedef) 
2. See [:material-code-braces: EffectiveLifecyclePolicyErrorDetailTypeDef](./type_defs.md#effectivelifecyclepolicyerrordetailtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetLifecyclePolicyRequestRequestTypeDef

```python
# BatchGetLifecyclePolicyRequestRequestTypeDef definition

class BatchGetLifecyclePolicyRequestRequestTypeDef(TypedDict):
    identifiers: Sequence[LifecyclePolicyIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: LifecyclePolicyIdentifierTypeDef](./type_defs.md#lifecyclepolicyidentifiertypedef) 
## CreateLifecyclePolicyResponseTypeDef

```python
# CreateLifecyclePolicyResponseTypeDef definition

class CreateLifecyclePolicyResponseTypeDef(TypedDict):
    lifecyclePolicyDetail: LifecyclePolicyDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LifecyclePolicyDetailTypeDef](./type_defs.md#lifecyclepolicydetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateLifecyclePolicyResponseTypeDef

```python
# UpdateLifecyclePolicyResponseTypeDef definition

class UpdateLifecyclePolicyResponseTypeDef(TypedDict):
    lifecyclePolicyDetail: LifecyclePolicyDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LifecyclePolicyDetailTypeDef](./type_defs.md#lifecyclepolicydetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetLifecyclePolicyResponseTypeDef

```python
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
# BatchGetVpcEndpointResponseTypeDef definition

class BatchGetVpcEndpointResponseTypeDef(TypedDict):
    vpcEndpointDetails: List[VpcEndpointDetailTypeDef],  # (1)
    vpcEndpointErrorDetails: List[VpcEndpointErrorDetailTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: VpcEndpointDetailTypeDef](./type_defs.md#vpcendpointdetailtypedef) 
2. See [:material-code-braces: VpcEndpointErrorDetailTypeDef](./type_defs.md#vpcendpointerrordetailtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCollectionsRequestRequestTypeDef

```python
# ListCollectionsRequestRequestTypeDef definition

class ListCollectionsRequestRequestTypeDef(TypedDict):
    collectionFilters: NotRequired[CollectionFiltersTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CollectionFiltersTypeDef](./type_defs.md#collectionfilterstypedef) 
## ListCollectionsResponseTypeDef

```python
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
# CreateCollectionResponseTypeDef definition

class CreateCollectionResponseTypeDef(TypedDict):
    createCollectionDetail: CreateCollectionDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CreateCollectionDetailTypeDef](./type_defs.md#createcollectiondetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCollectionRequestRequestTypeDef

```python
# CreateCollectionRequestRequestTypeDef definition

class CreateCollectionRequestRequestTypeDef(TypedDict):
    name: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    standbyReplicas: NotRequired[StandbyReplicasType],  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    type: NotRequired[CollectionTypeType],  # (3)
```

1. See [:material-code-brackets: StandbyReplicasType](./literals.md#standbyreplicastype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: CollectionTypeType](./literals.md#collectiontypetype) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateSecurityConfigRequestRequestTypeDef

```python
# CreateSecurityConfigRequestRequestTypeDef definition

class CreateSecurityConfigRequestRequestTypeDef(TypedDict):
    name: str,
    type: SecurityConfigTypeType,  # (1)
    clientToken: NotRequired[str],
    description: NotRequired[str],
    samlOptions: NotRequired[SamlConfigOptionsTypeDef],  # (2)
```

1. See [:material-code-brackets: SecurityConfigTypeType](./literals.md#securityconfigtypetype) 
2. See [:material-code-braces: SamlConfigOptionsTypeDef](./type_defs.md#samlconfigoptionstypedef) 
## SecurityConfigDetailTypeDef

```python
# SecurityConfigDetailTypeDef definition

class SecurityConfigDetailTypeDef(TypedDict):
    configVersion: NotRequired[str],
    createdDate: NotRequired[int],
    description: NotRequired[str],
    id: NotRequired[str],
    lastModifiedDate: NotRequired[int],
    samlOptions: NotRequired[SamlConfigOptionsTypeDef],  # (1)
    type: NotRequired[SecurityConfigTypeType],  # (2)
```

1. See [:material-code-braces: SamlConfigOptionsTypeDef](./type_defs.md#samlconfigoptionstypedef) 
2. See [:material-code-brackets: SecurityConfigTypeType](./literals.md#securityconfigtypetype) 
## UpdateSecurityConfigRequestRequestTypeDef

```python
# UpdateSecurityConfigRequestRequestTypeDef definition

class UpdateSecurityConfigRequestRequestTypeDef(TypedDict):
    configVersion: str,
    id: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    samlOptions: NotRequired[SamlConfigOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: SamlConfigOptionsTypeDef](./type_defs.md#samlconfigoptionstypedef) 
## CreateSecurityPolicyResponseTypeDef

```python
# CreateSecurityPolicyResponseTypeDef definition

class CreateSecurityPolicyResponseTypeDef(TypedDict):
    securityPolicyDetail: SecurityPolicyDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SecurityPolicyDetailTypeDef](./type_defs.md#securitypolicydetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSecurityPolicyResponseTypeDef

```python
# GetSecurityPolicyResponseTypeDef definition

class GetSecurityPolicyResponseTypeDef(TypedDict):
    securityPolicyDetail: SecurityPolicyDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SecurityPolicyDetailTypeDef](./type_defs.md#securitypolicydetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSecurityPolicyResponseTypeDef

```python
# UpdateSecurityPolicyResponseTypeDef definition

class UpdateSecurityPolicyResponseTypeDef(TypedDict):
    securityPolicyDetail: SecurityPolicyDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SecurityPolicyDetailTypeDef](./type_defs.md#securitypolicydetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateVpcEndpointResponseTypeDef

```python
# CreateVpcEndpointResponseTypeDef definition

class CreateVpcEndpointResponseTypeDef(TypedDict):
    createVpcEndpointDetail: CreateVpcEndpointDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CreateVpcEndpointDetailTypeDef](./type_defs.md#createvpcendpointdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteCollectionResponseTypeDef

```python
# DeleteCollectionResponseTypeDef definition

class DeleteCollectionResponseTypeDef(TypedDict):
    deleteCollectionDetail: DeleteCollectionDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeleteCollectionDetailTypeDef](./type_defs.md#deletecollectiondetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteVpcEndpointResponseTypeDef

```python
# DeleteVpcEndpointResponseTypeDef definition

class DeleteVpcEndpointResponseTypeDef(TypedDict):
    deleteVpcEndpointDetail: DeleteVpcEndpointDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeleteVpcEndpointDetailTypeDef](./type_defs.md#deletevpcendpointdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPoliciesStatsResponseTypeDef

```python
# GetPoliciesStatsResponseTypeDef definition

class GetPoliciesStatsResponseTypeDef(TypedDict):
    AccessPolicyStats: AccessPolicyStatsTypeDef,  # (1)
    LifecyclePolicyStats: LifecyclePolicyStatsTypeDef,  # (2)
    SecurityConfigStats: SecurityConfigStatsTypeDef,  # (3)
    SecurityPolicyStats: SecurityPolicyStatsTypeDef,  # (4)
    TotalPolicyCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: AccessPolicyStatsTypeDef](./type_defs.md#accesspolicystatstypedef) 
2. See [:material-code-braces: LifecyclePolicyStatsTypeDef](./type_defs.md#lifecyclepolicystatstypedef) 
3. See [:material-code-braces: SecurityConfigStatsTypeDef](./type_defs.md#securityconfigstatstypedef) 
4. See [:material-code-braces: SecurityPolicyStatsTypeDef](./type_defs.md#securitypolicystatstypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLifecyclePoliciesResponseTypeDef

```python
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
# ListSecurityPoliciesResponseTypeDef definition

class ListSecurityPoliciesResponseTypeDef(TypedDict):
    securityPolicySummaries: List[SecurityPolicySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SecurityPolicySummaryTypeDef](./type_defs.md#securitypolicysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVpcEndpointsRequestRequestTypeDef

```python
# ListVpcEndpointsRequestRequestTypeDef definition

class ListVpcEndpointsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    vpcEndpointFilters: NotRequired[VpcEndpointFiltersTypeDef],  # (1)
```

1. See [:material-code-braces: VpcEndpointFiltersTypeDef](./type_defs.md#vpcendpointfilterstypedef) 
## ListVpcEndpointsResponseTypeDef

```python
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
# UpdateCollectionResponseTypeDef definition

class UpdateCollectionResponseTypeDef(TypedDict):
    updateCollectionDetail: UpdateCollectionDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UpdateCollectionDetailTypeDef](./type_defs.md#updatecollectiondetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateVpcEndpointResponseTypeDef

```python
# UpdateVpcEndpointResponseTypeDef definition

class UpdateVpcEndpointResponseTypeDef(TypedDict):
    UpdateVpcEndpointDetail: UpdateVpcEndpointDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UpdateVpcEndpointDetailTypeDef](./type_defs.md#updatevpcendpointdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAccountSettingsResponseTypeDef

```python
# GetAccountSettingsResponseTypeDef definition

class GetAccountSettingsResponseTypeDef(TypedDict):
    accountSettingsDetail: AccountSettingsDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountSettingsDetailTypeDef](./type_defs.md#accountsettingsdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAccountSettingsResponseTypeDef

```python
# UpdateAccountSettingsResponseTypeDef definition

class UpdateAccountSettingsResponseTypeDef(TypedDict):
    accountSettingsDetail: AccountSettingsDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountSettingsDetailTypeDef](./type_defs.md#accountsettingsdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSecurityConfigResponseTypeDef

```python
# CreateSecurityConfigResponseTypeDef definition

class CreateSecurityConfigResponseTypeDef(TypedDict):
    securityConfigDetail: SecurityConfigDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SecurityConfigDetailTypeDef](./type_defs.md#securityconfigdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSecurityConfigResponseTypeDef

```python
# GetSecurityConfigResponseTypeDef definition

class GetSecurityConfigResponseTypeDef(TypedDict):
    securityConfigDetail: SecurityConfigDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SecurityConfigDetailTypeDef](./type_defs.md#securityconfigdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSecurityConfigResponseTypeDef

```python
# UpdateSecurityConfigResponseTypeDef definition

class UpdateSecurityConfigResponseTypeDef(TypedDict):
    securityConfigDetail: SecurityConfigDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SecurityConfigDetailTypeDef](./type_defs.md#securityconfigdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
