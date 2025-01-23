# Type definitions

> [Index](../README.md) > [EKS](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [EKS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#eks)
    type annotations stubs module [types-aiobotocore-eks](https://pypi.org/project/types-aiobotocore-eks/).

## FargateProfileSelectorUnionTypeDef

```python
# FargateProfileSelectorUnionTypeDef definition

FargateProfileSelectorUnionTypeDef = Union[
    FargateProfileSelectorTypeDef,  # (1)
    FargateProfileSelectorOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FargateProfileSelectorTypeDef](./type_defs.md#fargateprofileselectortypedef) 
2. See [:material-code-braces: FargateProfileSelectorOutputTypeDef](./type_defs.md#fargateprofileselectoroutputtypedef) 

## LogSetupUnionTypeDef

```python
# LogSetupUnionTypeDef definition

LogSetupUnionTypeDef = Union[
    LogSetupTypeDef,  # (1)
    LogSetupOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: LogSetupTypeDef](./type_defs.md#logsetuptypedef) 
2. See [:material-code-braces: LogSetupOutputTypeDef](./type_defs.md#logsetupoutputtypedef) 

## RemoteNodeNetworkUnionTypeDef

```python
# RemoteNodeNetworkUnionTypeDef definition

RemoteNodeNetworkUnionTypeDef = Union[
    RemoteNodeNetworkTypeDef,  # (1)
    RemoteNodeNetworkOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RemoteNodeNetworkTypeDef](./type_defs.md#remotenodenetworktypedef) 
2. See [:material-code-braces: RemoteNodeNetworkOutputTypeDef](./type_defs.md#remotenodenetworkoutputtypedef) 

## RemotePodNetworkUnionTypeDef

```python
# RemotePodNetworkUnionTypeDef definition

RemotePodNetworkUnionTypeDef = Union[
    RemotePodNetworkTypeDef,  # (1)
    RemotePodNetworkOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RemotePodNetworkTypeDef](./type_defs.md#remotepodnetworktypedef) 
2. See [:material-code-braces: RemotePodNetworkOutputTypeDef](./type_defs.md#remotepodnetworkoutputtypedef) 

## EncryptionConfigUnionTypeDef

```python
# EncryptionConfigUnionTypeDef definition

EncryptionConfigUnionTypeDef = Union[
    EncryptionConfigTypeDef,  # (1)
    EncryptionConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef) 
2. See [:material-code-braces: EncryptionConfigOutputTypeDef](./type_defs.md#encryptionconfigoutputtypedef) 



## AccessConfigResponseTypeDef

```python
# AccessConfigResponseTypeDef definition

class AccessConfigResponseTypeDef(TypedDict):
    bootstrapClusterCreatorAdminPermissions: NotRequired[bool],
    authenticationMode: NotRequired[AuthenticationModeType],  # (1)
```

1. See [:material-code-brackets: AuthenticationModeType](./literals.md#authenticationmodetype) 
## AccessEntryTypeDef

```python
# AccessEntryTypeDef definition

class AccessEntryTypeDef(TypedDict):
    clusterName: NotRequired[str],
    principalArn: NotRequired[str],
    kubernetesGroups: NotRequired[List[str]],
    accessEntryArn: NotRequired[str],
    createdAt: NotRequired[datetime],
    modifiedAt: NotRequired[datetime],
    tags: NotRequired[Dict[str, str]],
    username: NotRequired[str],
    type: NotRequired[str],
```

## AccessPolicyTypeDef

```python
# AccessPolicyTypeDef definition

class AccessPolicyTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
```

## AccessScopeOutputTypeDef

```python
# AccessScopeOutputTypeDef definition

class AccessScopeOutputTypeDef(TypedDict):
    type: NotRequired[AccessScopeTypeType],  # (1)
    namespaces: NotRequired[List[str]],
```

1. See [:material-code-brackets: AccessScopeTypeType](./literals.md#accessscopetypetype) 
## AccessScopeTypeDef

```python
# AccessScopeTypeDef definition

class AccessScopeTypeDef(TypedDict):
    type: NotRequired[AccessScopeTypeType],  # (1)
    namespaces: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: AccessScopeTypeType](./literals.md#accessscopetypetype) 
## AddonCompatibilityDetailTypeDef

```python
# AddonCompatibilityDetailTypeDef definition

class AddonCompatibilityDetailTypeDef(TypedDict):
    name: NotRequired[str],
    compatibleVersions: NotRequired[List[str]],
```

## AddonIssueTypeDef

```python
# AddonIssueTypeDef definition

class AddonIssueTypeDef(TypedDict):
    code: NotRequired[AddonIssueCodeType],  # (1)
    message: NotRequired[str],
    resourceIds: NotRequired[List[str]],
```

1. See [:material-code-brackets: AddonIssueCodeType](./literals.md#addonissuecodetype) 
## MarketplaceInformationTypeDef

```python
# MarketplaceInformationTypeDef definition

class MarketplaceInformationTypeDef(TypedDict):
    productId: NotRequired[str],
    productUrl: NotRequired[str],
```

## AddonPodIdentityAssociationsTypeDef

```python
# AddonPodIdentityAssociationsTypeDef definition

class AddonPodIdentityAssociationsTypeDef(TypedDict):
    serviceAccount: str,
    roleArn: str,
```

## AddonPodIdentityConfigurationTypeDef

```python
# AddonPodIdentityConfigurationTypeDef definition

class AddonPodIdentityConfigurationTypeDef(TypedDict):
    serviceAccount: NotRequired[str],
    recommendedManagedPolicies: NotRequired[List[str]],
```

## CompatibilityTypeDef

```python
# CompatibilityTypeDef definition

class CompatibilityTypeDef(TypedDict):
    clusterVersion: NotRequired[str],
    platformVersions: NotRequired[List[str]],
    defaultVersion: NotRequired[bool],
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

## OidcIdentityProviderConfigRequestTypeDef

```python
# OidcIdentityProviderConfigRequestTypeDef definition

class OidcIdentityProviderConfigRequestTypeDef(TypedDict):
    identityProviderConfigName: str,
    issuerUrl: str,
    clientId: str,
    usernameClaim: NotRequired[str],
    usernamePrefix: NotRequired[str],
    groupsClaim: NotRequired[str],
    groupsPrefix: NotRequired[str],
    requiredClaims: NotRequired[Mapping[str, str]],
```

## AutoScalingGroupTypeDef

```python
# AutoScalingGroupTypeDef definition

class AutoScalingGroupTypeDef(TypedDict):
    name: NotRequired[str],
```

## BlockStorageTypeDef

```python
# BlockStorageTypeDef definition

class BlockStorageTypeDef(TypedDict):
    enabled: NotRequired[bool],
```

## CertificateTypeDef

```python
# CertificateTypeDef definition

class CertificateTypeDef(TypedDict):
    data: NotRequired[str],
```

## ClientStatTypeDef

```python
# ClientStatTypeDef definition

class ClientStatTypeDef(TypedDict):
    userAgent: NotRequired[str],
    numberOfRequestsLast30Days: NotRequired[int],
    lastRequestTime: NotRequired[datetime],
```

## ClusterIssueTypeDef

```python
# ClusterIssueTypeDef definition

class ClusterIssueTypeDef(TypedDict):
    code: NotRequired[ClusterIssueCodeType],  # (1)
    message: NotRequired[str],
    resourceIds: NotRequired[List[str]],
```

1. See [:material-code-brackets: ClusterIssueCodeType](./literals.md#clusterissuecodetype) 
## ComputeConfigResponseTypeDef

```python
# ComputeConfigResponseTypeDef definition

class ComputeConfigResponseTypeDef(TypedDict):
    enabled: NotRequired[bool],
    nodePools: NotRequired[List[str]],
    nodeRoleArn: NotRequired[str],
```

## ConnectorConfigResponseTypeDef

```python
# ConnectorConfigResponseTypeDef definition

class ConnectorConfigResponseTypeDef(TypedDict):
    activationId: NotRequired[str],
    activationCode: NotRequired[str],
    activationExpiry: NotRequired[datetime],
    provider: NotRequired[str],
    roleArn: NotRequired[str],
```

## UpgradePolicyResponseTypeDef

```python
# UpgradePolicyResponseTypeDef definition

class UpgradePolicyResponseTypeDef(TypedDict):
    supportType: NotRequired[SupportTypeType],  # (1)
```

1. See [:material-code-brackets: SupportTypeType](./literals.md#supporttypetype) 
## VpcConfigResponseTypeDef

```python
# VpcConfigResponseTypeDef definition

class VpcConfigResponseTypeDef(TypedDict):
    subnetIds: NotRequired[List[str]],
    securityGroupIds: NotRequired[List[str]],
    clusterSecurityGroupId: NotRequired[str],
    vpcId: NotRequired[str],
    endpointPublicAccess: NotRequired[bool],
    endpointPrivateAccess: NotRequired[bool],
    publicAccessCidrs: NotRequired[List[str]],
```

## ZonalShiftConfigResponseTypeDef

```python
# ZonalShiftConfigResponseTypeDef definition

class ZonalShiftConfigResponseTypeDef(TypedDict):
    enabled: NotRequired[bool],
```

## ClusterVersionInformationTypeDef

```python
# ClusterVersionInformationTypeDef definition

class ClusterVersionInformationTypeDef(TypedDict):
    clusterVersion: NotRequired[str],
    clusterType: NotRequired[str],
    defaultPlatformVersion: NotRequired[str],
    defaultVersion: NotRequired[bool],
    releaseDate: NotRequired[datetime],
    endOfStandardSupportDate: NotRequired[datetime],
    endOfExtendedSupportDate: NotRequired[datetime],
    status: NotRequired[ClusterVersionStatusType],  # (1)
    kubernetesPatchVersion: NotRequired[str],
```

1. See [:material-code-brackets: ClusterVersionStatusType](./literals.md#clusterversionstatustype) 
## ComputeConfigRequestTypeDef

```python
# ComputeConfigRequestTypeDef definition

class ComputeConfigRequestTypeDef(TypedDict):
    enabled: NotRequired[bool],
    nodePools: NotRequired[Sequence[str]],
    nodeRoleArn: NotRequired[str],
```

## ConnectorConfigRequestTypeDef

```python
# ConnectorConfigRequestTypeDef definition

class ConnectorConfigRequestTypeDef(TypedDict):
    roleArn: str,
    provider: ConnectorConfigProviderType,  # (1)
```

1. See [:material-code-brackets: ConnectorConfigProviderType](./literals.md#connectorconfigprovidertype) 
## ControlPlanePlacementRequestTypeDef

```python
# ControlPlanePlacementRequestTypeDef definition

class ControlPlanePlacementRequestTypeDef(TypedDict):
    groupName: NotRequired[str],
```

## ControlPlanePlacementResponseTypeDef

```python
# ControlPlanePlacementResponseTypeDef definition

class ControlPlanePlacementResponseTypeDef(TypedDict):
    groupName: NotRequired[str],
```

## CreateAccessConfigRequestTypeDef

```python
# CreateAccessConfigRequestTypeDef definition

class CreateAccessConfigRequestTypeDef(TypedDict):
    bootstrapClusterCreatorAdminPermissions: NotRequired[bool],
    authenticationMode: NotRequired[AuthenticationModeType],  # (1)
```

1. See [:material-code-brackets: AuthenticationModeType](./literals.md#authenticationmodetype) 
## CreateAccessEntryRequestRequestTypeDef

```python
# CreateAccessEntryRequestRequestTypeDef definition

class CreateAccessEntryRequestRequestTypeDef(TypedDict):
    clusterName: str,
    principalArn: str,
    kubernetesGroups: NotRequired[Sequence[str]],
    tags: NotRequired[Mapping[str, str]],
    clientRequestToken: NotRequired[str],
    username: NotRequired[str],
    type: NotRequired[str],
```

## UpgradePolicyRequestTypeDef

```python
# UpgradePolicyRequestTypeDef definition

class UpgradePolicyRequestTypeDef(TypedDict):
    supportType: NotRequired[SupportTypeType],  # (1)
```

1. See [:material-code-brackets: SupportTypeType](./literals.md#supporttypetype) 
## VpcConfigRequestTypeDef

```python
# VpcConfigRequestTypeDef definition

class VpcConfigRequestTypeDef(TypedDict):
    subnetIds: NotRequired[Sequence[str]],
    securityGroupIds: NotRequired[Sequence[str]],
    endpointPublicAccess: NotRequired[bool],
    endpointPrivateAccess: NotRequired[bool],
    publicAccessCidrs: NotRequired[Sequence[str]],
```

## ZonalShiftConfigRequestTypeDef

```python
# ZonalShiftConfigRequestTypeDef definition

class ZonalShiftConfigRequestTypeDef(TypedDict):
    enabled: NotRequired[bool],
```

## EksAnywhereSubscriptionTermTypeDef

```python
# EksAnywhereSubscriptionTermTypeDef definition

class EksAnywhereSubscriptionTermTypeDef(TypedDict):
    duration: NotRequired[int],
    unit: NotRequired[EksAnywhereSubscriptionTermUnitType],  # (1)
```

1. See [:material-code-brackets: EksAnywhereSubscriptionTermUnitType](./literals.md#eksanywheresubscriptiontermunittype) 
## LaunchTemplateSpecificationTypeDef

```python
# LaunchTemplateSpecificationTypeDef definition

class LaunchTemplateSpecificationTypeDef(TypedDict):
    name: NotRequired[str],
    version: NotRequired[str],
    id: NotRequired[str],
```

## NodeRepairConfigTypeDef

```python
# NodeRepairConfigTypeDef definition

class NodeRepairConfigTypeDef(TypedDict):
    enabled: NotRequired[bool],
```

## NodegroupScalingConfigTypeDef

```python
# NodegroupScalingConfigTypeDef definition

class NodegroupScalingConfigTypeDef(TypedDict):
    minSize: NotRequired[int],
    maxSize: NotRequired[int],
    desiredSize: NotRequired[int],
```

## NodegroupUpdateConfigTypeDef

```python
# NodegroupUpdateConfigTypeDef definition

class NodegroupUpdateConfigTypeDef(TypedDict):
    maxUnavailable: NotRequired[int],
    maxUnavailablePercentage: NotRequired[int],
```

## RemoteAccessConfigTypeDef

```python
# RemoteAccessConfigTypeDef definition

class RemoteAccessConfigTypeDef(TypedDict):
    ec2SshKey: NotRequired[str],
    sourceSecurityGroups: NotRequired[Sequence[str]],
```

## TaintTypeDef

```python
# TaintTypeDef definition

class TaintTypeDef(TypedDict):
    key: NotRequired[str],
    value: NotRequired[str],
    effect: NotRequired[TaintEffectType],  # (1)
```

1. See [:material-code-brackets: TaintEffectType](./literals.md#tainteffecttype) 
## CreatePodIdentityAssociationRequestRequestTypeDef

```python
# CreatePodIdentityAssociationRequestRequestTypeDef definition

class CreatePodIdentityAssociationRequestRequestTypeDef(TypedDict):
    clusterName: str,
    namespace: str,
    serviceAccount: str,
    roleArn: str,
    clientRequestToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## PodIdentityAssociationTypeDef

```python
# PodIdentityAssociationTypeDef definition

class PodIdentityAssociationTypeDef(TypedDict):
    clusterName: NotRequired[str],
    namespace: NotRequired[str],
    serviceAccount: NotRequired[str],
    roleArn: NotRequired[str],
    associationArn: NotRequired[str],
    associationId: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    createdAt: NotRequired[datetime],
    modifiedAt: NotRequired[datetime],
    ownerArn: NotRequired[str],
```

## DeleteAccessEntryRequestRequestTypeDef

```python
# DeleteAccessEntryRequestRequestTypeDef definition

class DeleteAccessEntryRequestRequestTypeDef(TypedDict):
    clusterName: str,
    principalArn: str,
```

## DeleteAddonRequestRequestTypeDef

```python
# DeleteAddonRequestRequestTypeDef definition

class DeleteAddonRequestRequestTypeDef(TypedDict):
    clusterName: str,
    addonName: str,
    preserve: NotRequired[bool],
```

## DeleteClusterRequestRequestTypeDef

```python
# DeleteClusterRequestRequestTypeDef definition

class DeleteClusterRequestRequestTypeDef(TypedDict):
    name: str,
```

## DeleteEksAnywhereSubscriptionRequestRequestTypeDef

```python
# DeleteEksAnywhereSubscriptionRequestRequestTypeDef definition

class DeleteEksAnywhereSubscriptionRequestRequestTypeDef(TypedDict):
    id: str,
```

## DeleteFargateProfileRequestRequestTypeDef

```python
# DeleteFargateProfileRequestRequestTypeDef definition

class DeleteFargateProfileRequestRequestTypeDef(TypedDict):
    clusterName: str,
    fargateProfileName: str,
```

## DeleteNodegroupRequestRequestTypeDef

```python
# DeleteNodegroupRequestRequestTypeDef definition

class DeleteNodegroupRequestRequestTypeDef(TypedDict):
    clusterName: str,
    nodegroupName: str,
```

## DeletePodIdentityAssociationRequestRequestTypeDef

```python
# DeletePodIdentityAssociationRequestRequestTypeDef definition

class DeletePodIdentityAssociationRequestRequestTypeDef(TypedDict):
    clusterName: str,
    associationId: str,
```

## DeregisterClusterRequestRequestTypeDef

```python
# DeregisterClusterRequestRequestTypeDef definition

class DeregisterClusterRequestRequestTypeDef(TypedDict):
    name: str,
```

## DescribeAccessEntryRequestRequestTypeDef

```python
# DescribeAccessEntryRequestRequestTypeDef definition

class DescribeAccessEntryRequestRequestTypeDef(TypedDict):
    clusterName: str,
    principalArn: str,
```

## DescribeAddonConfigurationRequestRequestTypeDef

```python
# DescribeAddonConfigurationRequestRequestTypeDef definition

class DescribeAddonConfigurationRequestRequestTypeDef(TypedDict):
    addonName: str,
    addonVersion: str,
```

## DescribeAddonRequestRequestTypeDef

```python
# DescribeAddonRequestRequestTypeDef definition

class DescribeAddonRequestRequestTypeDef(TypedDict):
    clusterName: str,
    addonName: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeAddonVersionsRequestRequestTypeDef

```python
# DescribeAddonVersionsRequestRequestTypeDef definition

class DescribeAddonVersionsRequestRequestTypeDef(TypedDict):
    kubernetesVersion: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    addonName: NotRequired[str],
    types: NotRequired[Sequence[str]],
    publishers: NotRequired[Sequence[str]],
    owners: NotRequired[Sequence[str]],
```

## DescribeClusterRequestRequestTypeDef

```python
# DescribeClusterRequestRequestTypeDef definition

class DescribeClusterRequestRequestTypeDef(TypedDict):
    name: str,
```

## DescribeClusterVersionsRequestRequestTypeDef

```python
# DescribeClusterVersionsRequestRequestTypeDef definition

class DescribeClusterVersionsRequestRequestTypeDef(TypedDict):
    clusterType: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    defaultOnly: NotRequired[bool],
    includeAll: NotRequired[bool],
    clusterVersions: NotRequired[Sequence[str]],
    status: NotRequired[ClusterVersionStatusType],  # (1)
```

1. See [:material-code-brackets: ClusterVersionStatusType](./literals.md#clusterversionstatustype) 
## DescribeEksAnywhereSubscriptionRequestRequestTypeDef

```python
# DescribeEksAnywhereSubscriptionRequestRequestTypeDef definition

class DescribeEksAnywhereSubscriptionRequestRequestTypeDef(TypedDict):
    id: str,
```

## DescribeFargateProfileRequestRequestTypeDef

```python
# DescribeFargateProfileRequestRequestTypeDef definition

class DescribeFargateProfileRequestRequestTypeDef(TypedDict):
    clusterName: str,
    fargateProfileName: str,
```

## IdentityProviderConfigTypeDef

```python
# IdentityProviderConfigTypeDef definition

class IdentityProviderConfigTypeDef(TypedDict):
    type: str,
    name: str,
```

## DescribeInsightRequestRequestTypeDef

```python
# DescribeInsightRequestRequestTypeDef definition

class DescribeInsightRequestRequestTypeDef(TypedDict):
    clusterName: str,
    id: str,
```

## DescribeNodegroupRequestRequestTypeDef

```python
# DescribeNodegroupRequestRequestTypeDef definition

class DescribeNodegroupRequestRequestTypeDef(TypedDict):
    clusterName: str,
    nodegroupName: str,
```

## DescribePodIdentityAssociationRequestRequestTypeDef

```python
# DescribePodIdentityAssociationRequestRequestTypeDef definition

class DescribePodIdentityAssociationRequestRequestTypeDef(TypedDict):
    clusterName: str,
    associationId: str,
```

## DescribeUpdateRequestRequestTypeDef

```python
# DescribeUpdateRequestRequestTypeDef definition

class DescribeUpdateRequestRequestTypeDef(TypedDict):
    name: str,
    updateId: str,
    nodegroupName: NotRequired[str],
    addonName: NotRequired[str],
```

## DisassociateAccessPolicyRequestRequestTypeDef

```python
# DisassociateAccessPolicyRequestRequestTypeDef definition

class DisassociateAccessPolicyRequestRequestTypeDef(TypedDict):
    clusterName: str,
    principalArn: str,
    policyArn: str,
```

## ElasticLoadBalancingTypeDef

```python
# ElasticLoadBalancingTypeDef definition

class ElasticLoadBalancingTypeDef(TypedDict):
    enabled: NotRequired[bool],
```

## ProviderTypeDef

```python
# ProviderTypeDef definition

class ProviderTypeDef(TypedDict):
    keyArn: NotRequired[str],
```

## ErrorDetailTypeDef

```python
# ErrorDetailTypeDef definition

class ErrorDetailTypeDef(TypedDict):
    errorCode: NotRequired[ErrorCodeType],  # (1)
    errorMessage: NotRequired[str],
    resourceIds: NotRequired[List[str]],
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
## FargateProfileIssueTypeDef

```python
# FargateProfileIssueTypeDef definition

class FargateProfileIssueTypeDef(TypedDict):
    code: NotRequired[FargateProfileIssueCodeType],  # (1)
    message: NotRequired[str],
    resourceIds: NotRequired[List[str]],
```

1. See [:material-code-brackets: FargateProfileIssueCodeType](./literals.md#fargateprofileissuecodetype) 
## FargateProfileSelectorOutputTypeDef

```python
# FargateProfileSelectorOutputTypeDef definition

class FargateProfileSelectorOutputTypeDef(TypedDict):
    namespace: NotRequired[str],
    labels: NotRequired[Dict[str, str]],
```

## FargateProfileSelectorTypeDef

```python
# FargateProfileSelectorTypeDef definition

class FargateProfileSelectorTypeDef(TypedDict):
    namespace: NotRequired[str],
    labels: NotRequired[Mapping[str, str]],
```

## OidcIdentityProviderConfigTypeDef

```python
# OidcIdentityProviderConfigTypeDef definition

class OidcIdentityProviderConfigTypeDef(TypedDict):
    identityProviderConfigName: NotRequired[str],
    identityProviderConfigArn: NotRequired[str],
    clusterName: NotRequired[str],
    issuerUrl: NotRequired[str],
    clientId: NotRequired[str],
    usernameClaim: NotRequired[str],
    usernamePrefix: NotRequired[str],
    groupsClaim: NotRequired[str],
    groupsPrefix: NotRequired[str],
    requiredClaims: NotRequired[Dict[str, str]],
    tags: NotRequired[Dict[str, str]],
    status: NotRequired[ConfigStatusType],  # (1)
```

1. See [:material-code-brackets: ConfigStatusType](./literals.md#configstatustype) 
## OIDCTypeDef

```python
# OIDCTypeDef definition

class OIDCTypeDef(TypedDict):
    issuer: NotRequired[str],
```

## InsightStatusTypeDef

```python
# InsightStatusTypeDef definition

class InsightStatusTypeDef(TypedDict):
    status: NotRequired[InsightStatusValueType],  # (1)
    reason: NotRequired[str],
```

1. See [:material-code-brackets: InsightStatusValueType](./literals.md#insightstatusvaluetype) 
## InsightsFilterTypeDef

```python
# InsightsFilterTypeDef definition

class InsightsFilterTypeDef(TypedDict):
    categories: NotRequired[Sequence[CategoryType]],  # (1)
    kubernetesVersions: NotRequired[Sequence[str]],
    statuses: NotRequired[Sequence[InsightStatusValueType]],  # (2)
```

1. See [:material-code-brackets: CategoryType](./literals.md#categorytype) 
2. See [:material-code-brackets: InsightStatusValueType](./literals.md#insightstatusvaluetype) 
## IssueTypeDef

```python
# IssueTypeDef definition

class IssueTypeDef(TypedDict):
    code: NotRequired[NodegroupIssueCodeType],  # (1)
    message: NotRequired[str],
    resourceIds: NotRequired[List[str]],
```

1. See [:material-code-brackets: NodegroupIssueCodeType](./literals.md#nodegroupissuecodetype) 
## ListAccessEntriesRequestRequestTypeDef

```python
# ListAccessEntriesRequestRequestTypeDef definition

class ListAccessEntriesRequestRequestTypeDef(TypedDict):
    clusterName: str,
    associatedPolicyArn: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListAccessPoliciesRequestRequestTypeDef

```python
# ListAccessPoliciesRequestRequestTypeDef definition

class ListAccessPoliciesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListAddonsRequestRequestTypeDef

```python
# ListAddonsRequestRequestTypeDef definition

class ListAddonsRequestRequestTypeDef(TypedDict):
    clusterName: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListAssociatedAccessPoliciesRequestRequestTypeDef

```python
# ListAssociatedAccessPoliciesRequestRequestTypeDef definition

class ListAssociatedAccessPoliciesRequestRequestTypeDef(TypedDict):
    clusterName: str,
    principalArn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListClustersRequestRequestTypeDef

```python
# ListClustersRequestRequestTypeDef definition

class ListClustersRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    include: NotRequired[Sequence[str]],
```

## ListEksAnywhereSubscriptionsRequestRequestTypeDef

```python
# ListEksAnywhereSubscriptionsRequestRequestTypeDef definition

class ListEksAnywhereSubscriptionsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    includeStatus: NotRequired[Sequence[EksAnywhereSubscriptionStatusType]],  # (1)
```

1. See [:material-code-brackets: EksAnywhereSubscriptionStatusType](./literals.md#eksanywheresubscriptionstatustype) 
## ListFargateProfilesRequestRequestTypeDef

```python
# ListFargateProfilesRequestRequestTypeDef definition

class ListFargateProfilesRequestRequestTypeDef(TypedDict):
    clusterName: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListIdentityProviderConfigsRequestRequestTypeDef

```python
# ListIdentityProviderConfigsRequestRequestTypeDef definition

class ListIdentityProviderConfigsRequestRequestTypeDef(TypedDict):
    clusterName: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListNodegroupsRequestRequestTypeDef

```python
# ListNodegroupsRequestRequestTypeDef definition

class ListNodegroupsRequestRequestTypeDef(TypedDict):
    clusterName: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListPodIdentityAssociationsRequestRequestTypeDef

```python
# ListPodIdentityAssociationsRequestRequestTypeDef definition

class ListPodIdentityAssociationsRequestRequestTypeDef(TypedDict):
    clusterName: str,
    namespace: NotRequired[str],
    serviceAccount: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## PodIdentityAssociationSummaryTypeDef

```python
# PodIdentityAssociationSummaryTypeDef definition

class PodIdentityAssociationSummaryTypeDef(TypedDict):
    clusterName: NotRequired[str],
    namespace: NotRequired[str],
    serviceAccount: NotRequired[str],
    associationArn: NotRequired[str],
    associationId: NotRequired[str],
    ownerArn: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListUpdatesRequestRequestTypeDef

```python
# ListUpdatesRequestRequestTypeDef definition

class ListUpdatesRequestRequestTypeDef(TypedDict):
    name: str,
    nodegroupName: NotRequired[str],
    addonName: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## LogSetupOutputTypeDef

```python
# LogSetupOutputTypeDef definition

class LogSetupOutputTypeDef(TypedDict):
    types: NotRequired[List[LogTypeType]],  # (1)
    enabled: NotRequired[bool],
```

1. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) 
## LogSetupTypeDef

```python
# LogSetupTypeDef definition

class LogSetupTypeDef(TypedDict):
    types: NotRequired[Sequence[LogTypeType]],  # (1)
    enabled: NotRequired[bool],
```

1. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) 
## RemoteAccessConfigOutputTypeDef

```python
# RemoteAccessConfigOutputTypeDef definition

class RemoteAccessConfigOutputTypeDef(TypedDict):
    ec2SshKey: NotRequired[str],
    sourceSecurityGroups: NotRequired[List[str]],
```

## RemoteNodeNetworkOutputTypeDef

```python
# RemoteNodeNetworkOutputTypeDef definition

class RemoteNodeNetworkOutputTypeDef(TypedDict):
    cidrs: NotRequired[List[str]],
```

## RemotePodNetworkOutputTypeDef

```python
# RemotePodNetworkOutputTypeDef definition

class RemotePodNetworkOutputTypeDef(TypedDict):
    cidrs: NotRequired[List[str]],
```

## RemoteNodeNetworkTypeDef

```python
# RemoteNodeNetworkTypeDef definition

class RemoteNodeNetworkTypeDef(TypedDict):
    cidrs: NotRequired[Sequence[str]],
```

## RemotePodNetworkTypeDef

```python
# RemotePodNetworkTypeDef definition

class RemotePodNetworkTypeDef(TypedDict):
    cidrs: NotRequired[Sequence[str]],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateAccessConfigRequestTypeDef

```python
# UpdateAccessConfigRequestTypeDef definition

class UpdateAccessConfigRequestTypeDef(TypedDict):
    authenticationMode: NotRequired[AuthenticationModeType],  # (1)
```

1. See [:material-code-brackets: AuthenticationModeType](./literals.md#authenticationmodetype) 
## UpdateAccessEntryRequestRequestTypeDef

```python
# UpdateAccessEntryRequestRequestTypeDef definition

class UpdateAccessEntryRequestRequestTypeDef(TypedDict):
    clusterName: str,
    principalArn: str,
    kubernetesGroups: NotRequired[Sequence[str]],
    clientRequestToken: NotRequired[str],
    username: NotRequired[str],
```

## UpdateClusterVersionRequestRequestTypeDef

```python
# UpdateClusterVersionRequestRequestTypeDef definition

class UpdateClusterVersionRequestRequestTypeDef(TypedDict):
    name: str,
    version: str,
    clientRequestToken: NotRequired[str],
```

## UpdateEksAnywhereSubscriptionRequestRequestTypeDef

```python
# UpdateEksAnywhereSubscriptionRequestRequestTypeDef definition

class UpdateEksAnywhereSubscriptionRequestRequestTypeDef(TypedDict):
    id: str,
    autoRenew: bool,
    clientRequestToken: NotRequired[str],
```

## UpdateLabelsPayloadTypeDef

```python
# UpdateLabelsPayloadTypeDef definition

class UpdateLabelsPayloadTypeDef(TypedDict):
    addOrUpdateLabels: NotRequired[Mapping[str, str]],
    removeLabels: NotRequired[Sequence[str]],
```

## UpdateParamTypeDef

```python
# UpdateParamTypeDef definition

class UpdateParamTypeDef(TypedDict):
    type: NotRequired[UpdateParamTypeType],  # (1)
    value: NotRequired[str],
```

1. See [:material-code-brackets: UpdateParamTypeType](./literals.md#updateparamtypetype) 
## UpdatePodIdentityAssociationRequestRequestTypeDef

```python
# UpdatePodIdentityAssociationRequestRequestTypeDef definition

class UpdatePodIdentityAssociationRequestRequestTypeDef(TypedDict):
    clusterName: str,
    associationId: str,
    roleArn: NotRequired[str],
    clientRequestToken: NotRequired[str],
```

## AssociatedAccessPolicyTypeDef

```python
# AssociatedAccessPolicyTypeDef definition

class AssociatedAccessPolicyTypeDef(TypedDict):
    policyArn: NotRequired[str],
    accessScope: NotRequired[AccessScopeOutputTypeDef],  # (1)
    associatedAt: NotRequired[datetime],
    modifiedAt: NotRequired[datetime],
```

1. See [:material-code-braces: AccessScopeOutputTypeDef](./type_defs.md#accessscopeoutputtypedef) 
## AssociateAccessPolicyRequestRequestTypeDef

```python
# AssociateAccessPolicyRequestRequestTypeDef definition

class AssociateAccessPolicyRequestRequestTypeDef(TypedDict):
    clusterName: str,
    principalArn: str,
    policyArn: str,
    accessScope: AccessScopeTypeDef,  # (1)
```

1. See [:material-code-braces: AccessScopeTypeDef](./type_defs.md#accessscopetypedef) 
## AddonHealthTypeDef

```python
# AddonHealthTypeDef definition

class AddonHealthTypeDef(TypedDict):
    issues: NotRequired[List[AddonIssueTypeDef]],  # (1)
```

1. See [:material-code-braces: AddonIssueTypeDef](./type_defs.md#addonissuetypedef) 
## CreateAddonRequestRequestTypeDef

```python
# CreateAddonRequestRequestTypeDef definition

class CreateAddonRequestRequestTypeDef(TypedDict):
    clusterName: str,
    addonName: str,
    addonVersion: NotRequired[str],
    serviceAccountRoleArn: NotRequired[str],
    resolveConflicts: NotRequired[ResolveConflictsType],  # (1)
    clientRequestToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    configurationValues: NotRequired[str],
    podIdentityAssociations: NotRequired[Sequence[AddonPodIdentityAssociationsTypeDef]],  # (2)
```

1. See [:material-code-brackets: ResolveConflictsType](./literals.md#resolveconflictstype) 
2. See [:material-code-braces: AddonPodIdentityAssociationsTypeDef](./type_defs.md#addonpodidentityassociationstypedef) 
## UpdateAddonRequestRequestTypeDef

```python
# UpdateAddonRequestRequestTypeDef definition

class UpdateAddonRequestRequestTypeDef(TypedDict):
    clusterName: str,
    addonName: str,
    addonVersion: NotRequired[str],
    serviceAccountRoleArn: NotRequired[str],
    resolveConflicts: NotRequired[ResolveConflictsType],  # (1)
    clientRequestToken: NotRequired[str],
    configurationValues: NotRequired[str],
    podIdentityAssociations: NotRequired[Sequence[AddonPodIdentityAssociationsTypeDef]],  # (2)
```

1. See [:material-code-brackets: ResolveConflictsType](./literals.md#resolveconflictstype) 
2. See [:material-code-braces: AddonPodIdentityAssociationsTypeDef](./type_defs.md#addonpodidentityassociationstypedef) 
## AddonVersionInfoTypeDef

```python
# AddonVersionInfoTypeDef definition

class AddonVersionInfoTypeDef(TypedDict):
    addonVersion: NotRequired[str],
    architecture: NotRequired[List[str]],
    computeTypes: NotRequired[List[str]],
    compatibilities: NotRequired[List[CompatibilityTypeDef]],  # (1)
    requiresConfiguration: NotRequired[bool],
    requiresIamPermissions: NotRequired[bool],
```

1. See [:material-code-braces: CompatibilityTypeDef](./type_defs.md#compatibilitytypedef) 
## CreateAccessEntryResponseTypeDef

```python
# CreateAccessEntryResponseTypeDef definition

class CreateAccessEntryResponseTypeDef(TypedDict):
    accessEntry: AccessEntryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccessEntryTypeDef](./type_defs.md#accessentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAccessEntryResponseTypeDef

```python
# DescribeAccessEntryResponseTypeDef definition

class DescribeAccessEntryResponseTypeDef(TypedDict):
    accessEntry: AccessEntryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccessEntryTypeDef](./type_defs.md#accessentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAddonConfigurationResponseTypeDef

```python
# DescribeAddonConfigurationResponseTypeDef definition

class DescribeAddonConfigurationResponseTypeDef(TypedDict):
    addonName: str,
    addonVersion: str,
    configurationSchema: str,
    podIdentityConfiguration: List[AddonPodIdentityConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AddonPodIdentityConfigurationTypeDef](./type_defs.md#addonpodidentityconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccessEntriesResponseTypeDef

```python
# ListAccessEntriesResponseTypeDef definition

class ListAccessEntriesResponseTypeDef(TypedDict):
    accessEntries: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccessPoliciesResponseTypeDef

```python
# ListAccessPoliciesResponseTypeDef definition

class ListAccessPoliciesResponseTypeDef(TypedDict):
    accessPolicies: List[AccessPolicyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AccessPolicyTypeDef](./type_defs.md#accesspolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAddonsResponseTypeDef

```python
# ListAddonsResponseTypeDef definition

class ListAddonsResponseTypeDef(TypedDict):
    addons: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListClustersResponseTypeDef

```python
# ListClustersResponseTypeDef definition

class ListClustersResponseTypeDef(TypedDict):
    clusters: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFargateProfilesResponseTypeDef

```python
# ListFargateProfilesResponseTypeDef definition

class ListFargateProfilesResponseTypeDef(TypedDict):
    fargateProfileNames: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListNodegroupsResponseTypeDef

```python
# ListNodegroupsResponseTypeDef definition

class ListNodegroupsResponseTypeDef(TypedDict):
    nodegroups: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUpdatesResponseTypeDef

```python
# ListUpdatesResponseTypeDef definition

class ListUpdatesResponseTypeDef(TypedDict):
    updateIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAccessEntryResponseTypeDef

```python
# UpdateAccessEntryResponseTypeDef definition

class UpdateAccessEntryResponseTypeDef(TypedDict):
    accessEntry: AccessEntryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccessEntryTypeDef](./type_defs.md#accessentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateIdentityProviderConfigRequestRequestTypeDef

```python
# AssociateIdentityProviderConfigRequestRequestTypeDef definition

class AssociateIdentityProviderConfigRequestRequestTypeDef(TypedDict):
    clusterName: str,
    oidc: OidcIdentityProviderConfigRequestTypeDef,  # (1)
    tags: NotRequired[Mapping[str, str]],
    clientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: OidcIdentityProviderConfigRequestTypeDef](./type_defs.md#oidcidentityproviderconfigrequesttypedef) 
## NodegroupResourcesTypeDef

```python
# NodegroupResourcesTypeDef definition

class NodegroupResourcesTypeDef(TypedDict):
    autoScalingGroups: NotRequired[List[AutoScalingGroupTypeDef]],  # (1)
    remoteAccessSecurityGroup: NotRequired[str],
```

1. See [:material-code-braces: AutoScalingGroupTypeDef](./type_defs.md#autoscalinggrouptypedef) 
## StorageConfigRequestTypeDef

```python
# StorageConfigRequestTypeDef definition

class StorageConfigRequestTypeDef(TypedDict):
    blockStorage: NotRequired[BlockStorageTypeDef],  # (1)
```

1. See [:material-code-braces: BlockStorageTypeDef](./type_defs.md#blockstoragetypedef) 
## StorageConfigResponseTypeDef

```python
# StorageConfigResponseTypeDef definition

class StorageConfigResponseTypeDef(TypedDict):
    blockStorage: NotRequired[BlockStorageTypeDef],  # (1)
```

1. See [:material-code-braces: BlockStorageTypeDef](./type_defs.md#blockstoragetypedef) 
## DeprecationDetailTypeDef

```python
# DeprecationDetailTypeDef definition

class DeprecationDetailTypeDef(TypedDict):
    usage: NotRequired[str],
    replacedWith: NotRequired[str],
    stopServingVersion: NotRequired[str],
    startServingReplacementVersion: NotRequired[str],
    clientStats: NotRequired[List[ClientStatTypeDef]],  # (1)
```

1. See [:material-code-braces: ClientStatTypeDef](./type_defs.md#clientstattypedef) 
## ClusterHealthTypeDef

```python
# ClusterHealthTypeDef definition

class ClusterHealthTypeDef(TypedDict):
    issues: NotRequired[List[ClusterIssueTypeDef]],  # (1)
```

1. See [:material-code-braces: ClusterIssueTypeDef](./type_defs.md#clusterissuetypedef) 
## DescribeClusterVersionsResponseTypeDef

```python
# DescribeClusterVersionsResponseTypeDef definition

class DescribeClusterVersionsResponseTypeDef(TypedDict):
    clusterVersions: List[ClusterVersionInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ClusterVersionInformationTypeDef](./type_defs.md#clusterversioninformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterClusterRequestRequestTypeDef

```python
# RegisterClusterRequestRequestTypeDef definition

class RegisterClusterRequestRequestTypeDef(TypedDict):
    name: str,
    connectorConfig: ConnectorConfigRequestTypeDef,  # (1)
    clientRequestToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ConnectorConfigRequestTypeDef](./type_defs.md#connectorconfigrequesttypedef) 
## OutpostConfigRequestTypeDef

```python
# OutpostConfigRequestTypeDef definition

class OutpostConfigRequestTypeDef(TypedDict):
    outpostArns: Sequence[str],
    controlPlaneInstanceType: str,
    controlPlanePlacement: NotRequired[ControlPlanePlacementRequestTypeDef],  # (1)
```

1. See [:material-code-braces: ControlPlanePlacementRequestTypeDef](./type_defs.md#controlplaneplacementrequesttypedef) 
## OutpostConfigResponseTypeDef

```python
# OutpostConfigResponseTypeDef definition

class OutpostConfigResponseTypeDef(TypedDict):
    outpostArns: List[str],
    controlPlaneInstanceType: str,
    controlPlanePlacement: NotRequired[ControlPlanePlacementResponseTypeDef],  # (1)
```

1. See [:material-code-braces: ControlPlanePlacementResponseTypeDef](./type_defs.md#controlplaneplacementresponsetypedef) 
## CreateEksAnywhereSubscriptionRequestRequestTypeDef

```python
# CreateEksAnywhereSubscriptionRequestRequestTypeDef definition

class CreateEksAnywhereSubscriptionRequestRequestTypeDef(TypedDict):
    name: str,
    term: EksAnywhereSubscriptionTermTypeDef,  # (1)
    licenseQuantity: NotRequired[int],
    licenseType: NotRequired[EksAnywhereSubscriptionLicenseTypeType],  # (2)
    autoRenew: NotRequired[bool],
    clientRequestToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: EksAnywhereSubscriptionTermTypeDef](./type_defs.md#eksanywheresubscriptiontermtypedef) 
2. See [:material-code-brackets: EksAnywhereSubscriptionLicenseTypeType](./literals.md#eksanywheresubscriptionlicensetypetype) 
## EksAnywhereSubscriptionTypeDef

```python
# EksAnywhereSubscriptionTypeDef definition

class EksAnywhereSubscriptionTypeDef(TypedDict):
    id: NotRequired[str],
    arn: NotRequired[str],
    createdAt: NotRequired[datetime],
    effectiveDate: NotRequired[datetime],
    expirationDate: NotRequired[datetime],
    licenseQuantity: NotRequired[int],
    licenseType: NotRequired[EksAnywhereSubscriptionLicenseTypeType],  # (1)
    term: NotRequired[EksAnywhereSubscriptionTermTypeDef],  # (2)
    status: NotRequired[str],
    autoRenew: NotRequired[bool],
    licenseArns: NotRequired[List[str]],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: EksAnywhereSubscriptionLicenseTypeType](./literals.md#eksanywheresubscriptionlicensetypetype) 
2. See [:material-code-braces: EksAnywhereSubscriptionTermTypeDef](./type_defs.md#eksanywheresubscriptiontermtypedef) 
## UpdateNodegroupVersionRequestRequestTypeDef

```python
# UpdateNodegroupVersionRequestRequestTypeDef definition

class UpdateNodegroupVersionRequestRequestTypeDef(TypedDict):
    clusterName: str,
    nodegroupName: str,
    version: NotRequired[str],
    releaseVersion: NotRequired[str],
    launchTemplate: NotRequired[LaunchTemplateSpecificationTypeDef],  # (1)
    force: NotRequired[bool],
    clientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: LaunchTemplateSpecificationTypeDef](./type_defs.md#launchtemplatespecificationtypedef) 
## CreateNodegroupRequestRequestTypeDef

```python
# CreateNodegroupRequestRequestTypeDef definition

class CreateNodegroupRequestRequestTypeDef(TypedDict):
    clusterName: str,
    nodegroupName: str,
    subnets: Sequence[str],
    nodeRole: str,
    scalingConfig: NotRequired[NodegroupScalingConfigTypeDef],  # (1)
    diskSize: NotRequired[int],
    instanceTypes: NotRequired[Sequence[str]],
    amiType: NotRequired[AMITypesType],  # (2)
    remoteAccess: NotRequired[RemoteAccessConfigTypeDef],  # (3)
    labels: NotRequired[Mapping[str, str]],
    taints: NotRequired[Sequence[TaintTypeDef]],  # (4)
    tags: NotRequired[Mapping[str, str]],
    clientRequestToken: NotRequired[str],
    launchTemplate: NotRequired[LaunchTemplateSpecificationTypeDef],  # (5)
    updateConfig: NotRequired[NodegroupUpdateConfigTypeDef],  # (6)
    nodeRepairConfig: NotRequired[NodeRepairConfigTypeDef],  # (7)
    capacityType: NotRequired[CapacityTypesType],  # (8)
    version: NotRequired[str],
    releaseVersion: NotRequired[str],
```

1. See [:material-code-braces: NodegroupScalingConfigTypeDef](./type_defs.md#nodegroupscalingconfigtypedef) 
2. See [:material-code-brackets: AMITypesType](./literals.md#amitypestype) 
3. See [:material-code-braces: RemoteAccessConfigTypeDef](./type_defs.md#remoteaccessconfigtypedef) 
4. See [:material-code-braces: TaintTypeDef](./type_defs.md#tainttypedef) 
5. See [:material-code-braces: LaunchTemplateSpecificationTypeDef](./type_defs.md#launchtemplatespecificationtypedef) 
6. See [:material-code-braces: NodegroupUpdateConfigTypeDef](./type_defs.md#nodegroupupdateconfigtypedef) 
7. See [:material-code-braces: NodeRepairConfigTypeDef](./type_defs.md#noderepairconfigtypedef) 
8. See [:material-code-brackets: CapacityTypesType](./literals.md#capacitytypestype) 
## UpdateTaintsPayloadTypeDef

```python
# UpdateTaintsPayloadTypeDef definition

class UpdateTaintsPayloadTypeDef(TypedDict):
    addOrUpdateTaints: NotRequired[Sequence[TaintTypeDef]],  # (1)
    removeTaints: NotRequired[Sequence[TaintTypeDef]],  # (1)
```

1. See [:material-code-braces: TaintTypeDef](./type_defs.md#tainttypedef) 
2. See [:material-code-braces: TaintTypeDef](./type_defs.md#tainttypedef) 
## CreatePodIdentityAssociationResponseTypeDef

```python
# CreatePodIdentityAssociationResponseTypeDef definition

class CreatePodIdentityAssociationResponseTypeDef(TypedDict):
    association: PodIdentityAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PodIdentityAssociationTypeDef](./type_defs.md#podidentityassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeletePodIdentityAssociationResponseTypeDef

```python
# DeletePodIdentityAssociationResponseTypeDef definition

class DeletePodIdentityAssociationResponseTypeDef(TypedDict):
    association: PodIdentityAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PodIdentityAssociationTypeDef](./type_defs.md#podidentityassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePodIdentityAssociationResponseTypeDef

```python
# DescribePodIdentityAssociationResponseTypeDef definition

class DescribePodIdentityAssociationResponseTypeDef(TypedDict):
    association: PodIdentityAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PodIdentityAssociationTypeDef](./type_defs.md#podidentityassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePodIdentityAssociationResponseTypeDef

```python
# UpdatePodIdentityAssociationResponseTypeDef definition

class UpdatePodIdentityAssociationResponseTypeDef(TypedDict):
    association: PodIdentityAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PodIdentityAssociationTypeDef](./type_defs.md#podidentityassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAddonRequestWaitTypeDef

```python
# DescribeAddonRequestWaitTypeDef definition

class DescribeAddonRequestWaitTypeDef(TypedDict):
    clusterName: str,
    addonName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeClusterRequestWaitTypeDef

```python
# DescribeClusterRequestWaitTypeDef definition

class DescribeClusterRequestWaitTypeDef(TypedDict):
    name: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeFargateProfileRequestWaitTypeDef

```python
# DescribeFargateProfileRequestWaitTypeDef definition

class DescribeFargateProfileRequestWaitTypeDef(TypedDict):
    clusterName: str,
    fargateProfileName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeNodegroupRequestWaitTypeDef

```python
# DescribeNodegroupRequestWaitTypeDef definition

class DescribeNodegroupRequestWaitTypeDef(TypedDict):
    clusterName: str,
    nodegroupName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeAddonVersionsRequestPaginateTypeDef

```python
# DescribeAddonVersionsRequestPaginateTypeDef definition

class DescribeAddonVersionsRequestPaginateTypeDef(TypedDict):
    kubernetesVersion: NotRequired[str],
    addonName: NotRequired[str],
    types: NotRequired[Sequence[str]],
    publishers: NotRequired[Sequence[str]],
    owners: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeClusterVersionsRequestPaginateTypeDef

```python
# DescribeClusterVersionsRequestPaginateTypeDef definition

class DescribeClusterVersionsRequestPaginateTypeDef(TypedDict):
    clusterType: NotRequired[str],
    defaultOnly: NotRequired[bool],
    includeAll: NotRequired[bool],
    clusterVersions: NotRequired[Sequence[str]],
    status: NotRequired[ClusterVersionStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ClusterVersionStatusType](./literals.md#clusterversionstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAccessEntriesRequestPaginateTypeDef

```python
# ListAccessEntriesRequestPaginateTypeDef definition

class ListAccessEntriesRequestPaginateTypeDef(TypedDict):
    clusterName: str,
    associatedPolicyArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAccessPoliciesRequestPaginateTypeDef

```python
# ListAccessPoliciesRequestPaginateTypeDef definition

class ListAccessPoliciesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAddonsRequestPaginateTypeDef

```python
# ListAddonsRequestPaginateTypeDef definition

class ListAddonsRequestPaginateTypeDef(TypedDict):
    clusterName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssociatedAccessPoliciesRequestPaginateTypeDef

```python
# ListAssociatedAccessPoliciesRequestPaginateTypeDef definition

class ListAssociatedAccessPoliciesRequestPaginateTypeDef(TypedDict):
    clusterName: str,
    principalArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListClustersRequestPaginateTypeDef

```python
# ListClustersRequestPaginateTypeDef definition

class ListClustersRequestPaginateTypeDef(TypedDict):
    include: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEksAnywhereSubscriptionsRequestPaginateTypeDef

```python
# ListEksAnywhereSubscriptionsRequestPaginateTypeDef definition

class ListEksAnywhereSubscriptionsRequestPaginateTypeDef(TypedDict):
    includeStatus: NotRequired[Sequence[EksAnywhereSubscriptionStatusType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: EksAnywhereSubscriptionStatusType](./literals.md#eksanywheresubscriptionstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFargateProfilesRequestPaginateTypeDef

```python
# ListFargateProfilesRequestPaginateTypeDef definition

class ListFargateProfilesRequestPaginateTypeDef(TypedDict):
    clusterName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIdentityProviderConfigsRequestPaginateTypeDef

```python
# ListIdentityProviderConfigsRequestPaginateTypeDef definition

class ListIdentityProviderConfigsRequestPaginateTypeDef(TypedDict):
    clusterName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNodegroupsRequestPaginateTypeDef

```python
# ListNodegroupsRequestPaginateTypeDef definition

class ListNodegroupsRequestPaginateTypeDef(TypedDict):
    clusterName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPodIdentityAssociationsRequestPaginateTypeDef

```python
# ListPodIdentityAssociationsRequestPaginateTypeDef definition

class ListPodIdentityAssociationsRequestPaginateTypeDef(TypedDict):
    clusterName: str,
    namespace: NotRequired[str],
    serviceAccount: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUpdatesRequestPaginateTypeDef

```python
# ListUpdatesRequestPaginateTypeDef definition

class ListUpdatesRequestPaginateTypeDef(TypedDict):
    name: str,
    nodegroupName: NotRequired[str],
    addonName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeIdentityProviderConfigRequestRequestTypeDef

```python
# DescribeIdentityProviderConfigRequestRequestTypeDef definition

class DescribeIdentityProviderConfigRequestRequestTypeDef(TypedDict):
    clusterName: str,
    identityProviderConfig: IdentityProviderConfigTypeDef,  # (1)
```

1. See [:material-code-braces: IdentityProviderConfigTypeDef](./type_defs.md#identityproviderconfigtypedef) 
## DisassociateIdentityProviderConfigRequestRequestTypeDef

```python
# DisassociateIdentityProviderConfigRequestRequestTypeDef definition

class DisassociateIdentityProviderConfigRequestRequestTypeDef(TypedDict):
    clusterName: str,
    identityProviderConfig: IdentityProviderConfigTypeDef,  # (1)
    clientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: IdentityProviderConfigTypeDef](./type_defs.md#identityproviderconfigtypedef) 
## ListIdentityProviderConfigsResponseTypeDef

```python
# ListIdentityProviderConfigsResponseTypeDef definition

class ListIdentityProviderConfigsResponseTypeDef(TypedDict):
    identityProviderConfigs: List[IdentityProviderConfigTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: IdentityProviderConfigTypeDef](./type_defs.md#identityproviderconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## KubernetesNetworkConfigRequestTypeDef

```python
# KubernetesNetworkConfigRequestTypeDef definition

class KubernetesNetworkConfigRequestTypeDef(TypedDict):
    serviceIpv4Cidr: NotRequired[str],
    ipFamily: NotRequired[IpFamilyType],  # (1)
    elasticLoadBalancing: NotRequired[ElasticLoadBalancingTypeDef],  # (2)
```

1. See [:material-code-brackets: IpFamilyType](./literals.md#ipfamilytype) 
2. See [:material-code-braces: ElasticLoadBalancingTypeDef](./type_defs.md#elasticloadbalancingtypedef) 
## KubernetesNetworkConfigResponseTypeDef

```python
# KubernetesNetworkConfigResponseTypeDef definition

class KubernetesNetworkConfigResponseTypeDef(TypedDict):
    serviceIpv4Cidr: NotRequired[str],
    serviceIpv6Cidr: NotRequired[str],
    ipFamily: NotRequired[IpFamilyType],  # (1)
    elasticLoadBalancing: NotRequired[ElasticLoadBalancingTypeDef],  # (2)
```

1. See [:material-code-brackets: IpFamilyType](./literals.md#ipfamilytype) 
2. See [:material-code-braces: ElasticLoadBalancingTypeDef](./type_defs.md#elasticloadbalancingtypedef) 
## EncryptionConfigOutputTypeDef

```python
# EncryptionConfigOutputTypeDef definition

class EncryptionConfigOutputTypeDef(TypedDict):
    resources: NotRequired[List[str]],
    provider: NotRequired[ProviderTypeDef],  # (1)
```

1. See [:material-code-braces: ProviderTypeDef](./type_defs.md#providertypedef) 
## EncryptionConfigTypeDef

```python
# EncryptionConfigTypeDef definition

class EncryptionConfigTypeDef(TypedDict):
    resources: NotRequired[Sequence[str]],
    provider: NotRequired[ProviderTypeDef],  # (1)
```

1. See [:material-code-braces: ProviderTypeDef](./type_defs.md#providertypedef) 
## FargateProfileHealthTypeDef

```python
# FargateProfileHealthTypeDef definition

class FargateProfileHealthTypeDef(TypedDict):
    issues: NotRequired[List[FargateProfileIssueTypeDef]],  # (1)
```

1. See [:material-code-braces: FargateProfileIssueTypeDef](./type_defs.md#fargateprofileissuetypedef) 
## IdentityProviderConfigResponseTypeDef

```python
# IdentityProviderConfigResponseTypeDef definition

class IdentityProviderConfigResponseTypeDef(TypedDict):
    oidc: NotRequired[OidcIdentityProviderConfigTypeDef],  # (1)
```

1. See [:material-code-braces: OidcIdentityProviderConfigTypeDef](./type_defs.md#oidcidentityproviderconfigtypedef) 
## IdentityTypeDef

```python
# IdentityTypeDef definition

class IdentityTypeDef(TypedDict):
    oidc: NotRequired[OIDCTypeDef],  # (1)
```

1. See [:material-code-braces: OIDCTypeDef](./type_defs.md#oidctypedef) 
## InsightResourceDetailTypeDef

```python
# InsightResourceDetailTypeDef definition

class InsightResourceDetailTypeDef(TypedDict):
    insightStatus: NotRequired[InsightStatusTypeDef],  # (1)
    kubernetesResourceUri: NotRequired[str],
    arn: NotRequired[str],
```

1. See [:material-code-braces: InsightStatusTypeDef](./type_defs.md#insightstatustypedef) 
## InsightSummaryTypeDef

```python
# InsightSummaryTypeDef definition

class InsightSummaryTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    category: NotRequired[CategoryType],  # (1)
    kubernetesVersion: NotRequired[str],
    lastRefreshTime: NotRequired[datetime],
    lastTransitionTime: NotRequired[datetime],
    description: NotRequired[str],
    insightStatus: NotRequired[InsightStatusTypeDef],  # (2)
```

1. See [:material-code-brackets: CategoryType](./literals.md#categorytype) 
2. See [:material-code-braces: InsightStatusTypeDef](./type_defs.md#insightstatustypedef) 
## ListInsightsRequestPaginateTypeDef

```python
# ListInsightsRequestPaginateTypeDef definition

class ListInsightsRequestPaginateTypeDef(TypedDict):
    clusterName: str,
    filter: NotRequired[InsightsFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: InsightsFilterTypeDef](./type_defs.md#insightsfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInsightsRequestRequestTypeDef

```python
# ListInsightsRequestRequestTypeDef definition

class ListInsightsRequestRequestTypeDef(TypedDict):
    clusterName: str,
    filter: NotRequired[InsightsFilterTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: InsightsFilterTypeDef](./type_defs.md#insightsfiltertypedef) 
## NodegroupHealthTypeDef

```python
# NodegroupHealthTypeDef definition

class NodegroupHealthTypeDef(TypedDict):
    issues: NotRequired[List[IssueTypeDef]],  # (1)
```

1. See [:material-code-braces: IssueTypeDef](./type_defs.md#issuetypedef) 
## ListPodIdentityAssociationsResponseTypeDef

```python
# ListPodIdentityAssociationsResponseTypeDef definition

class ListPodIdentityAssociationsResponseTypeDef(TypedDict):
    associations: List[PodIdentityAssociationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PodIdentityAssociationSummaryTypeDef](./type_defs.md#podidentityassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LoggingOutputTypeDef

```python
# LoggingOutputTypeDef definition

class LoggingOutputTypeDef(TypedDict):
    clusterLogging: NotRequired[List[LogSetupOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: LogSetupOutputTypeDef](./type_defs.md#logsetupoutputtypedef) 
## RemoteNetworkConfigResponseTypeDef

```python
# RemoteNetworkConfigResponseTypeDef definition

class RemoteNetworkConfigResponseTypeDef(TypedDict):
    remoteNodeNetworks: NotRequired[List[RemoteNodeNetworkOutputTypeDef]],  # (1)
    remotePodNetworks: NotRequired[List[RemotePodNetworkOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: RemoteNodeNetworkOutputTypeDef](./type_defs.md#remotenodenetworkoutputtypedef) 
2. See [:material-code-braces: RemotePodNetworkOutputTypeDef](./type_defs.md#remotepodnetworkoutputtypedef) 
## UpdateTypeDef

```python
# UpdateTypeDef definition

class UpdateTypeDef(TypedDict):
    id: NotRequired[str],
    status: NotRequired[UpdateStatusType],  # (1)
    type: NotRequired[UpdateTypeType],  # (2)
    params: NotRequired[List[UpdateParamTypeDef]],  # (3)
    createdAt: NotRequired[datetime],
    errors: NotRequired[List[ErrorDetailTypeDef]],  # (4)
```

1. See [:material-code-brackets: UpdateStatusType](./literals.md#updatestatustype) 
2. See [:material-code-brackets: UpdateTypeType](./literals.md#updatetypetype) 
3. See [:material-code-braces: UpdateParamTypeDef](./type_defs.md#updateparamtypedef) 
4. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
## AssociateAccessPolicyResponseTypeDef

```python
# AssociateAccessPolicyResponseTypeDef definition

class AssociateAccessPolicyResponseTypeDef(TypedDict):
    clusterName: str,
    principalArn: str,
    associatedAccessPolicy: AssociatedAccessPolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssociatedAccessPolicyTypeDef](./type_defs.md#associatedaccesspolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssociatedAccessPoliciesResponseTypeDef

```python
# ListAssociatedAccessPoliciesResponseTypeDef definition

class ListAssociatedAccessPoliciesResponseTypeDef(TypedDict):
    clusterName: str,
    principalArn: str,
    associatedAccessPolicies: List[AssociatedAccessPolicyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AssociatedAccessPolicyTypeDef](./type_defs.md#associatedaccesspolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddonTypeDef

```python
# AddonTypeDef definition

class AddonTypeDef(TypedDict):
    addonName: NotRequired[str],
    clusterName: NotRequired[str],
    status: NotRequired[AddonStatusType],  # (1)
    addonVersion: NotRequired[str],
    health: NotRequired[AddonHealthTypeDef],  # (2)
    addonArn: NotRequired[str],
    createdAt: NotRequired[datetime],
    modifiedAt: NotRequired[datetime],
    serviceAccountRoleArn: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    publisher: NotRequired[str],
    owner: NotRequired[str],
    marketplaceInformation: NotRequired[MarketplaceInformationTypeDef],  # (3)
    configurationValues: NotRequired[str],
    podIdentityAssociations: NotRequired[List[str]],
```

1. See [:material-code-brackets: AddonStatusType](./literals.md#addonstatustype) 
2. See [:material-code-braces: AddonHealthTypeDef](./type_defs.md#addonhealthtypedef) 
3. See [:material-code-braces: MarketplaceInformationTypeDef](./type_defs.md#marketplaceinformationtypedef) 
## AddonInfoTypeDef

```python
# AddonInfoTypeDef definition

class AddonInfoTypeDef(TypedDict):
    addonName: NotRequired[str],
    type: NotRequired[str],
    addonVersions: NotRequired[List[AddonVersionInfoTypeDef]],  # (1)
    publisher: NotRequired[str],
    owner: NotRequired[str],
    marketplaceInformation: NotRequired[MarketplaceInformationTypeDef],  # (2)
```

1. See [:material-code-braces: AddonVersionInfoTypeDef](./type_defs.md#addonversioninfotypedef) 
2. See [:material-code-braces: MarketplaceInformationTypeDef](./type_defs.md#marketplaceinformationtypedef) 
## InsightCategorySpecificSummaryTypeDef

```python
# InsightCategorySpecificSummaryTypeDef definition

class InsightCategorySpecificSummaryTypeDef(TypedDict):
    deprecationDetails: NotRequired[List[DeprecationDetailTypeDef]],  # (1)
    addonCompatibilityDetails: NotRequired[List[AddonCompatibilityDetailTypeDef]],  # (2)
```

1. See [:material-code-braces: DeprecationDetailTypeDef](./type_defs.md#deprecationdetailtypedef) 
2. See [:material-code-braces: AddonCompatibilityDetailTypeDef](./type_defs.md#addoncompatibilitydetailtypedef) 
## CreateEksAnywhereSubscriptionResponseTypeDef

```python
# CreateEksAnywhereSubscriptionResponseTypeDef definition

class CreateEksAnywhereSubscriptionResponseTypeDef(TypedDict):
    subscription: EksAnywhereSubscriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EksAnywhereSubscriptionTypeDef](./type_defs.md#eksanywheresubscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteEksAnywhereSubscriptionResponseTypeDef

```python
# DeleteEksAnywhereSubscriptionResponseTypeDef definition

class DeleteEksAnywhereSubscriptionResponseTypeDef(TypedDict):
    subscription: EksAnywhereSubscriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EksAnywhereSubscriptionTypeDef](./type_defs.md#eksanywheresubscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEksAnywhereSubscriptionResponseTypeDef

```python
# DescribeEksAnywhereSubscriptionResponseTypeDef definition

class DescribeEksAnywhereSubscriptionResponseTypeDef(TypedDict):
    subscription: EksAnywhereSubscriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EksAnywhereSubscriptionTypeDef](./type_defs.md#eksanywheresubscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEksAnywhereSubscriptionsResponseTypeDef

```python
# ListEksAnywhereSubscriptionsResponseTypeDef definition

class ListEksAnywhereSubscriptionsResponseTypeDef(TypedDict):
    subscriptions: List[EksAnywhereSubscriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: EksAnywhereSubscriptionTypeDef](./type_defs.md#eksanywheresubscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEksAnywhereSubscriptionResponseTypeDef

```python
# UpdateEksAnywhereSubscriptionResponseTypeDef definition

class UpdateEksAnywhereSubscriptionResponseTypeDef(TypedDict):
    subscription: EksAnywhereSubscriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EksAnywhereSubscriptionTypeDef](./type_defs.md#eksanywheresubscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateNodegroupConfigRequestRequestTypeDef

```python
# UpdateNodegroupConfigRequestRequestTypeDef definition

class UpdateNodegroupConfigRequestRequestTypeDef(TypedDict):
    clusterName: str,
    nodegroupName: str,
    labels: NotRequired[UpdateLabelsPayloadTypeDef],  # (1)
    taints: NotRequired[UpdateTaintsPayloadTypeDef],  # (2)
    scalingConfig: NotRequired[NodegroupScalingConfigTypeDef],  # (3)
    updateConfig: NotRequired[NodegroupUpdateConfigTypeDef],  # (4)
    nodeRepairConfig: NotRequired[NodeRepairConfigTypeDef],  # (5)
    clientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: UpdateLabelsPayloadTypeDef](./type_defs.md#updatelabelspayloadtypedef) 
2. See [:material-code-braces: UpdateTaintsPayloadTypeDef](./type_defs.md#updatetaintspayloadtypedef) 
3. See [:material-code-braces: NodegroupScalingConfigTypeDef](./type_defs.md#nodegroupscalingconfigtypedef) 
4. See [:material-code-braces: NodegroupUpdateConfigTypeDef](./type_defs.md#nodegroupupdateconfigtypedef) 
5. See [:material-code-braces: NodeRepairConfigTypeDef](./type_defs.md#noderepairconfigtypedef) 
## FargateProfileTypeDef

```python
# FargateProfileTypeDef definition

class FargateProfileTypeDef(TypedDict):
    fargateProfileName: NotRequired[str],
    fargateProfileArn: NotRequired[str],
    clusterName: NotRequired[str],
    createdAt: NotRequired[datetime],
    podExecutionRoleArn: NotRequired[str],
    subnets: NotRequired[List[str]],
    selectors: NotRequired[List[FargateProfileSelectorOutputTypeDef]],  # (1)
    status: NotRequired[FargateProfileStatusType],  # (2)
    tags: NotRequired[Dict[str, str]],
    health: NotRequired[FargateProfileHealthTypeDef],  # (3)
```

1. See [:material-code-braces: FargateProfileSelectorOutputTypeDef](./type_defs.md#fargateprofileselectoroutputtypedef) 
2. See [:material-code-brackets: FargateProfileStatusType](./literals.md#fargateprofilestatustype) 
3. See [:material-code-braces: FargateProfileHealthTypeDef](./type_defs.md#fargateprofilehealthtypedef) 
## CreateFargateProfileRequestRequestTypeDef

```python
# CreateFargateProfileRequestRequestTypeDef definition

class CreateFargateProfileRequestRequestTypeDef(TypedDict):
    fargateProfileName: str,
    clusterName: str,
    podExecutionRoleArn: str,
    subnets: NotRequired[Sequence[str]],
    selectors: NotRequired[Sequence[FargateProfileSelectorUnionTypeDef]],  # (1)
    clientRequestToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: FargateProfileSelectorTypeDef](./type_defs.md#fargateprofileselectortypedef) [:material-code-braces: FargateProfileSelectorOutputTypeDef](./type_defs.md#fargateprofileselectoroutputtypedef) 
## DescribeIdentityProviderConfigResponseTypeDef

```python
# DescribeIdentityProviderConfigResponseTypeDef definition

class DescribeIdentityProviderConfigResponseTypeDef(TypedDict):
    identityProviderConfig: IdentityProviderConfigResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentityProviderConfigResponseTypeDef](./type_defs.md#identityproviderconfigresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInsightsResponseTypeDef

```python
# ListInsightsResponseTypeDef definition

class ListInsightsResponseTypeDef(TypedDict):
    insights: List[InsightSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: InsightSummaryTypeDef](./type_defs.md#insightsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NodegroupTypeDef

```python
# NodegroupTypeDef definition

class NodegroupTypeDef(TypedDict):
    nodegroupName: NotRequired[str],
    nodegroupArn: NotRequired[str],
    clusterName: NotRequired[str],
    version: NotRequired[str],
    releaseVersion: NotRequired[str],
    createdAt: NotRequired[datetime],
    modifiedAt: NotRequired[datetime],
    status: NotRequired[NodegroupStatusType],  # (1)
    capacityType: NotRequired[CapacityTypesType],  # (2)
    scalingConfig: NotRequired[NodegroupScalingConfigTypeDef],  # (3)
    instanceTypes: NotRequired[List[str]],
    subnets: NotRequired[List[str]],
    remoteAccess: NotRequired[RemoteAccessConfigOutputTypeDef],  # (4)
    amiType: NotRequired[AMITypesType],  # (5)
    nodeRole: NotRequired[str],
    labels: NotRequired[Dict[str, str]],
    taints: NotRequired[List[TaintTypeDef]],  # (6)
    resources: NotRequired[NodegroupResourcesTypeDef],  # (7)
    diskSize: NotRequired[int],
    health: NotRequired[NodegroupHealthTypeDef],  # (8)
    updateConfig: NotRequired[NodegroupUpdateConfigTypeDef],  # (9)
    nodeRepairConfig: NotRequired[NodeRepairConfigTypeDef],  # (10)
    launchTemplate: NotRequired[LaunchTemplateSpecificationTypeDef],  # (11)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: NodegroupStatusType](./literals.md#nodegroupstatustype) 
2. See [:material-code-brackets: CapacityTypesType](./literals.md#capacitytypestype) 
3. See [:material-code-braces: NodegroupScalingConfigTypeDef](./type_defs.md#nodegroupscalingconfigtypedef) 
4. See [:material-code-braces: RemoteAccessConfigOutputTypeDef](./type_defs.md#remoteaccessconfigoutputtypedef) 
5. See [:material-code-brackets: AMITypesType](./literals.md#amitypestype) 
6. See [:material-code-braces: TaintTypeDef](./type_defs.md#tainttypedef) 
7. See [:material-code-braces: NodegroupResourcesTypeDef](./type_defs.md#nodegroupresourcestypedef) 
8. See [:material-code-braces: NodegroupHealthTypeDef](./type_defs.md#nodegrouphealthtypedef) 
9. See [:material-code-braces: NodegroupUpdateConfigTypeDef](./type_defs.md#nodegroupupdateconfigtypedef) 
10. See [:material-code-braces: NodeRepairConfigTypeDef](./type_defs.md#noderepairconfigtypedef) 
11. See [:material-code-braces: LaunchTemplateSpecificationTypeDef](./type_defs.md#launchtemplatespecificationtypedef) 
## LoggingTypeDef

```python
# LoggingTypeDef definition

class LoggingTypeDef(TypedDict):
    clusterLogging: NotRequired[Sequence[LogSetupUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: LogSetupTypeDef](./type_defs.md#logsetuptypedef) [:material-code-braces: LogSetupOutputTypeDef](./type_defs.md#logsetupoutputtypedef) 
## ClusterTypeDef

```python
# ClusterTypeDef definition

class ClusterTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
    createdAt: NotRequired[datetime],
    version: NotRequired[str],
    endpoint: NotRequired[str],
    roleArn: NotRequired[str],
    resourcesVpcConfig: NotRequired[VpcConfigResponseTypeDef],  # (1)
    kubernetesNetworkConfig: NotRequired[KubernetesNetworkConfigResponseTypeDef],  # (2)
    logging: NotRequired[LoggingOutputTypeDef],  # (3)
    identity: NotRequired[IdentityTypeDef],  # (4)
    status: NotRequired[ClusterStatusType],  # (5)
    certificateAuthority: NotRequired[CertificateTypeDef],  # (6)
    clientRequestToken: NotRequired[str],
    platformVersion: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    encryptionConfig: NotRequired[List[EncryptionConfigOutputTypeDef]],  # (7)
    connectorConfig: NotRequired[ConnectorConfigResponseTypeDef],  # (8)
    id: NotRequired[str],
    health: NotRequired[ClusterHealthTypeDef],  # (9)
    outpostConfig: NotRequired[OutpostConfigResponseTypeDef],  # (10)
    accessConfig: NotRequired[AccessConfigResponseTypeDef],  # (11)
    upgradePolicy: NotRequired[UpgradePolicyResponseTypeDef],  # (12)
    zonalShiftConfig: NotRequired[ZonalShiftConfigResponseTypeDef],  # (13)
    remoteNetworkConfig: NotRequired[RemoteNetworkConfigResponseTypeDef],  # (14)
    computeConfig: NotRequired[ComputeConfigResponseTypeDef],  # (15)
    storageConfig: NotRequired[StorageConfigResponseTypeDef],  # (16)
```

1. See [:material-code-braces: VpcConfigResponseTypeDef](./type_defs.md#vpcconfigresponsetypedef) 
2. See [:material-code-braces: KubernetesNetworkConfigResponseTypeDef](./type_defs.md#kubernetesnetworkconfigresponsetypedef) 
3. See [:material-code-braces: LoggingOutputTypeDef](./type_defs.md#loggingoutputtypedef) 
4. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
5. See [:material-code-brackets: ClusterStatusType](./literals.md#clusterstatustype) 
6. See [:material-code-braces: CertificateTypeDef](./type_defs.md#certificatetypedef) 
7. See [:material-code-braces: EncryptionConfigOutputTypeDef](./type_defs.md#encryptionconfigoutputtypedef) 
8. See [:material-code-braces: ConnectorConfigResponseTypeDef](./type_defs.md#connectorconfigresponsetypedef) 
9. See [:material-code-braces: ClusterHealthTypeDef](./type_defs.md#clusterhealthtypedef) 
10. See [:material-code-braces: OutpostConfigResponseTypeDef](./type_defs.md#outpostconfigresponsetypedef) 
11. See [:material-code-braces: AccessConfigResponseTypeDef](./type_defs.md#accessconfigresponsetypedef) 
12. See [:material-code-braces: UpgradePolicyResponseTypeDef](./type_defs.md#upgradepolicyresponsetypedef) 
13. See [:material-code-braces: ZonalShiftConfigResponseTypeDef](./type_defs.md#zonalshiftconfigresponsetypedef) 
14. See [:material-code-braces: RemoteNetworkConfigResponseTypeDef](./type_defs.md#remotenetworkconfigresponsetypedef) 
15. See [:material-code-braces: ComputeConfigResponseTypeDef](./type_defs.md#computeconfigresponsetypedef) 
16. See [:material-code-braces: StorageConfigResponseTypeDef](./type_defs.md#storageconfigresponsetypedef) 
## RemoteNetworkConfigRequestTypeDef

```python
# RemoteNetworkConfigRequestTypeDef definition

class RemoteNetworkConfigRequestTypeDef(TypedDict):
    remoteNodeNetworks: NotRequired[Sequence[RemoteNodeNetworkUnionTypeDef]],  # (1)
    remotePodNetworks: NotRequired[Sequence[RemotePodNetworkUnionTypeDef]],  # (2)
```

1. See [:material-code-braces: RemoteNodeNetworkTypeDef](./type_defs.md#remotenodenetworktypedef) [:material-code-braces: RemoteNodeNetworkOutputTypeDef](./type_defs.md#remotenodenetworkoutputtypedef) 
2. See [:material-code-braces: RemotePodNetworkTypeDef](./type_defs.md#remotepodnetworktypedef) [:material-code-braces: RemotePodNetworkOutputTypeDef](./type_defs.md#remotepodnetworkoutputtypedef) 
## AssociateEncryptionConfigResponseTypeDef

```python
# AssociateEncryptionConfigResponseTypeDef definition

class AssociateEncryptionConfigResponseTypeDef(TypedDict):
    update: UpdateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UpdateTypeDef](./type_defs.md#updatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateIdentityProviderConfigResponseTypeDef

```python
# AssociateIdentityProviderConfigResponseTypeDef definition

class AssociateIdentityProviderConfigResponseTypeDef(TypedDict):
    update: UpdateTypeDef,  # (1)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UpdateTypeDef](./type_defs.md#updatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeUpdateResponseTypeDef

```python
# DescribeUpdateResponseTypeDef definition

class DescribeUpdateResponseTypeDef(TypedDict):
    update: UpdateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UpdateTypeDef](./type_defs.md#updatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateIdentityProviderConfigResponseTypeDef

```python
# DisassociateIdentityProviderConfigResponseTypeDef definition

class DisassociateIdentityProviderConfigResponseTypeDef(TypedDict):
    update: UpdateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UpdateTypeDef](./type_defs.md#updatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAddonResponseTypeDef

```python
# UpdateAddonResponseTypeDef definition

class UpdateAddonResponseTypeDef(TypedDict):
    update: UpdateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UpdateTypeDef](./type_defs.md#updatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateClusterConfigResponseTypeDef

```python
# UpdateClusterConfigResponseTypeDef definition

class UpdateClusterConfigResponseTypeDef(TypedDict):
    update: UpdateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UpdateTypeDef](./type_defs.md#updatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateClusterVersionResponseTypeDef

```python
# UpdateClusterVersionResponseTypeDef definition

class UpdateClusterVersionResponseTypeDef(TypedDict):
    update: UpdateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UpdateTypeDef](./type_defs.md#updatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateNodegroupConfigResponseTypeDef

```python
# UpdateNodegroupConfigResponseTypeDef definition

class UpdateNodegroupConfigResponseTypeDef(TypedDict):
    update: UpdateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UpdateTypeDef](./type_defs.md#updatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateNodegroupVersionResponseTypeDef

```python
# UpdateNodegroupVersionResponseTypeDef definition

class UpdateNodegroupVersionResponseTypeDef(TypedDict):
    update: UpdateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UpdateTypeDef](./type_defs.md#updatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAddonResponseTypeDef

```python
# CreateAddonResponseTypeDef definition

class CreateAddonResponseTypeDef(TypedDict):
    addon: AddonTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AddonTypeDef](./type_defs.md#addontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAddonResponseTypeDef

```python
# DeleteAddonResponseTypeDef definition

class DeleteAddonResponseTypeDef(TypedDict):
    addon: AddonTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AddonTypeDef](./type_defs.md#addontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAddonResponseTypeDef

```python
# DescribeAddonResponseTypeDef definition

class DescribeAddonResponseTypeDef(TypedDict):
    addon: AddonTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AddonTypeDef](./type_defs.md#addontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAddonVersionsResponseTypeDef

```python
# DescribeAddonVersionsResponseTypeDef definition

class DescribeAddonVersionsResponseTypeDef(TypedDict):
    addons: List[AddonInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AddonInfoTypeDef](./type_defs.md#addoninfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InsightTypeDef

```python
# InsightTypeDef definition

class InsightTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    category: NotRequired[CategoryType],  # (1)
    kubernetesVersion: NotRequired[str],
    lastRefreshTime: NotRequired[datetime],
    lastTransitionTime: NotRequired[datetime],
    description: NotRequired[str],
    insightStatus: NotRequired[InsightStatusTypeDef],  # (2)
    recommendation: NotRequired[str],
    additionalInfo: NotRequired[Dict[str, str]],
    resources: NotRequired[List[InsightResourceDetailTypeDef]],  # (3)
    categorySpecificSummary: NotRequired[InsightCategorySpecificSummaryTypeDef],  # (4)
```

1. See [:material-code-brackets: CategoryType](./literals.md#categorytype) 
2. See [:material-code-braces: InsightStatusTypeDef](./type_defs.md#insightstatustypedef) 
3. See [:material-code-braces: InsightResourceDetailTypeDef](./type_defs.md#insightresourcedetailtypedef) 
4. See [:material-code-braces: InsightCategorySpecificSummaryTypeDef](./type_defs.md#insightcategoryspecificsummarytypedef) 
## AssociateEncryptionConfigRequestRequestTypeDef

```python
# AssociateEncryptionConfigRequestRequestTypeDef definition

class AssociateEncryptionConfigRequestRequestTypeDef(TypedDict):
    clusterName: str,
    encryptionConfig: Sequence[EncryptionConfigUnionTypeDef],  # (1)
    clientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef) [:material-code-braces: EncryptionConfigOutputTypeDef](./type_defs.md#encryptionconfigoutputtypedef) 
## CreateFargateProfileResponseTypeDef

```python
# CreateFargateProfileResponseTypeDef definition

class CreateFargateProfileResponseTypeDef(TypedDict):
    fargateProfile: FargateProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FargateProfileTypeDef](./type_defs.md#fargateprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteFargateProfileResponseTypeDef

```python
# DeleteFargateProfileResponseTypeDef definition

class DeleteFargateProfileResponseTypeDef(TypedDict):
    fargateProfile: FargateProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FargateProfileTypeDef](./type_defs.md#fargateprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeFargateProfileResponseTypeDef

```python
# DescribeFargateProfileResponseTypeDef definition

class DescribeFargateProfileResponseTypeDef(TypedDict):
    fargateProfile: FargateProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FargateProfileTypeDef](./type_defs.md#fargateprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateNodegroupResponseTypeDef

```python
# CreateNodegroupResponseTypeDef definition

class CreateNodegroupResponseTypeDef(TypedDict):
    nodegroup: NodegroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NodegroupTypeDef](./type_defs.md#nodegrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteNodegroupResponseTypeDef

```python
# DeleteNodegroupResponseTypeDef definition

class DeleteNodegroupResponseTypeDef(TypedDict):
    nodegroup: NodegroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NodegroupTypeDef](./type_defs.md#nodegrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeNodegroupResponseTypeDef

```python
# DescribeNodegroupResponseTypeDef definition

class DescribeNodegroupResponseTypeDef(TypedDict):
    nodegroup: NodegroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NodegroupTypeDef](./type_defs.md#nodegrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateClusterConfigRequestRequestTypeDef

```python
# UpdateClusterConfigRequestRequestTypeDef definition

class UpdateClusterConfigRequestRequestTypeDef(TypedDict):
    name: str,
    resourcesVpcConfig: NotRequired[VpcConfigRequestTypeDef],  # (1)
    logging: NotRequired[LoggingTypeDef],  # (2)
    clientRequestToken: NotRequired[str],
    accessConfig: NotRequired[UpdateAccessConfigRequestTypeDef],  # (3)
    upgradePolicy: NotRequired[UpgradePolicyRequestTypeDef],  # (4)
    zonalShiftConfig: NotRequired[ZonalShiftConfigRequestTypeDef],  # (5)
    computeConfig: NotRequired[ComputeConfigRequestTypeDef],  # (6)
    kubernetesNetworkConfig: NotRequired[KubernetesNetworkConfigRequestTypeDef],  # (7)
    storageConfig: NotRequired[StorageConfigRequestTypeDef],  # (8)
```

1. See [:material-code-braces: VpcConfigRequestTypeDef](./type_defs.md#vpcconfigrequesttypedef) 
2. See [:material-code-braces: LoggingTypeDef](./type_defs.md#loggingtypedef) 
3. See [:material-code-braces: UpdateAccessConfigRequestTypeDef](./type_defs.md#updateaccessconfigrequesttypedef) 
4. See [:material-code-braces: UpgradePolicyRequestTypeDef](./type_defs.md#upgradepolicyrequesttypedef) 
5. See [:material-code-braces: ZonalShiftConfigRequestTypeDef](./type_defs.md#zonalshiftconfigrequesttypedef) 
6. See [:material-code-braces: ComputeConfigRequestTypeDef](./type_defs.md#computeconfigrequesttypedef) 
7. See [:material-code-braces: KubernetesNetworkConfigRequestTypeDef](./type_defs.md#kubernetesnetworkconfigrequesttypedef) 
8. See [:material-code-braces: StorageConfigRequestTypeDef](./type_defs.md#storageconfigrequesttypedef) 
## CreateClusterResponseTypeDef

```python
# CreateClusterResponseTypeDef definition

class CreateClusterResponseTypeDef(TypedDict):
    cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteClusterResponseTypeDef

```python
# DeleteClusterResponseTypeDef definition

class DeleteClusterResponseTypeDef(TypedDict):
    cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeregisterClusterResponseTypeDef

```python
# DeregisterClusterResponseTypeDef definition

class DeregisterClusterResponseTypeDef(TypedDict):
    cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeClusterResponseTypeDef

```python
# DescribeClusterResponseTypeDef definition

class DescribeClusterResponseTypeDef(TypedDict):
    cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterClusterResponseTypeDef

```python
# RegisterClusterResponseTypeDef definition

class RegisterClusterResponseTypeDef(TypedDict):
    cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateClusterRequestRequestTypeDef

```python
# CreateClusterRequestRequestTypeDef definition

class CreateClusterRequestRequestTypeDef(TypedDict):
    name: str,
    roleArn: str,
    resourcesVpcConfig: VpcConfigRequestTypeDef,  # (1)
    version: NotRequired[str],
    kubernetesNetworkConfig: NotRequired[KubernetesNetworkConfigRequestTypeDef],  # (2)
    logging: NotRequired[LoggingTypeDef],  # (3)
    clientRequestToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    encryptionConfig: NotRequired[Sequence[EncryptionConfigTypeDef]],  # (4)
    outpostConfig: NotRequired[OutpostConfigRequestTypeDef],  # (5)
    accessConfig: NotRequired[CreateAccessConfigRequestTypeDef],  # (6)
    bootstrapSelfManagedAddons: NotRequired[bool],
    upgradePolicy: NotRequired[UpgradePolicyRequestTypeDef],  # (7)
    zonalShiftConfig: NotRequired[ZonalShiftConfigRequestTypeDef],  # (8)
    remoteNetworkConfig: NotRequired[RemoteNetworkConfigRequestTypeDef],  # (9)
    computeConfig: NotRequired[ComputeConfigRequestTypeDef],  # (10)
    storageConfig: NotRequired[StorageConfigRequestTypeDef],  # (11)
```

1. See [:material-code-braces: VpcConfigRequestTypeDef](./type_defs.md#vpcconfigrequesttypedef) 
2. See [:material-code-braces: KubernetesNetworkConfigRequestTypeDef](./type_defs.md#kubernetesnetworkconfigrequesttypedef) 
3. See [:material-code-braces: LoggingTypeDef](./type_defs.md#loggingtypedef) 
4. See [:material-code-braces: EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef) 
5. See [:material-code-braces: OutpostConfigRequestTypeDef](./type_defs.md#outpostconfigrequesttypedef) 
6. See [:material-code-braces: CreateAccessConfigRequestTypeDef](./type_defs.md#createaccessconfigrequesttypedef) 
7. See [:material-code-braces: UpgradePolicyRequestTypeDef](./type_defs.md#upgradepolicyrequesttypedef) 
8. See [:material-code-braces: ZonalShiftConfigRequestTypeDef](./type_defs.md#zonalshiftconfigrequesttypedef) 
9. See [:material-code-braces: RemoteNetworkConfigRequestTypeDef](./type_defs.md#remotenetworkconfigrequesttypedef) 
10. See [:material-code-braces: ComputeConfigRequestTypeDef](./type_defs.md#computeconfigrequesttypedef) 
11. See [:material-code-braces: StorageConfigRequestTypeDef](./type_defs.md#storageconfigrequesttypedef) 
## DescribeInsightResponseTypeDef

```python
# DescribeInsightResponseTypeDef definition

class DescribeInsightResponseTypeDef(TypedDict):
    insight: InsightTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InsightTypeDef](./type_defs.md#insighttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
