# Type definitions

> [Index](../README.md) > [EKS](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [EKS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#EKS)
    type annotations stubs module [types-aiobotocore-eks](https://pypi.org/project/types-aiobotocore-eks/).



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
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
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

## CertificateTypeDef

```python
# CertificateTypeDef definition

class CertificateTypeDef(TypedDict):
    data: NotRequired[str],
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

## KubernetesNetworkConfigResponseTypeDef

```python
# KubernetesNetworkConfigResponseTypeDef definition

class KubernetesNetworkConfigResponseTypeDef(TypedDict):
    serviceIpv4Cidr: NotRequired[str],
    serviceIpv6Cidr: NotRequired[str],
    ipFamily: NotRequired[IpFamilyType],  # (1)
```

1. See [:material-code-brackets: IpFamilyType](./literals.md#ipfamilytype) 
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
```

1. See [:material-code-brackets: ResolveConflictsType](./literals.md#resolveconflictstype) 
## KubernetesNetworkConfigRequestTypeDef

```python
# KubernetesNetworkConfigRequestTypeDef definition

class KubernetesNetworkConfigRequestTypeDef(TypedDict):
    serviceIpv4Cidr: NotRequired[str],
    ipFamily: NotRequired[IpFamilyType],  # (1)
```

1. See [:material-code-brackets: IpFamilyType](./literals.md#ipfamilytype) 
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

## FargateProfileSelectorTypeDef

```python
# FargateProfileSelectorTypeDef definition

class FargateProfileSelectorTypeDef(TypedDict):
    namespace: NotRequired[str],
    labels: NotRequired[Mapping[str, str]],
```

## LaunchTemplateSpecificationTypeDef

```python
# LaunchTemplateSpecificationTypeDef definition

class LaunchTemplateSpecificationTypeDef(TypedDict):
    name: NotRequired[str],
    version: NotRequired[str],
    id: NotRequired[str],
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

## DeregisterClusterRequestRequestTypeDef

```python
# DeregisterClusterRequestRequestTypeDef definition

class DeregisterClusterRequestRequestTypeDef(TypedDict):
    name: str,
```

## DescribeAddonConfigurationRequestRequestTypeDef

```python
# DescribeAddonConfigurationRequestRequestTypeDef definition

class DescribeAddonConfigurationRequestRequestTypeDef(TypedDict):
    addonName: str,
    addonVersion: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeAddonRequestRequestTypeDef

```python
# DescribeAddonRequestRequestTypeDef definition

class DescribeAddonRequestRequestTypeDef(TypedDict):
    clusterName: str,
    addonName: str,
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

## DescribeNodegroupRequestRequestTypeDef

```python
# DescribeNodegroupRequestRequestTypeDef definition

class DescribeNodegroupRequestRequestTypeDef(TypedDict):
    clusterName: str,
    nodegroupName: str,
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
    status: NotRequired[configStatusType],  # (1)
```

1. See [:material-code-brackets: configStatusType](./literals.md#configstatustype) 
## OIDCTypeDef

```python
# OIDCTypeDef definition

class OIDCTypeDef(TypedDict):
    issuer: NotRequired[str],
```

## IssueTypeDef

```python
# IssueTypeDef definition

class IssueTypeDef(TypedDict):
    code: NotRequired[NodegroupIssueCodeType],  # (1)
    message: NotRequired[str],
    resourceIds: NotRequired[List[str]],
```

1. See [:material-code-brackets: NodegroupIssueCodeType](./literals.md#nodegroupissuecodetype) 
## ListAddonsRequestRequestTypeDef

```python
# ListAddonsRequestRequestTypeDef definition

class ListAddonsRequestRequestTypeDef(TypedDict):
    clusterName: str,
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

## LogSetupTypeDef

```python
# LogSetupTypeDef definition

class LogSetupTypeDef(TypedDict):
    types: NotRequired[Sequence[LogTypeType]],  # (1)
    enabled: NotRequired[bool],
```

1. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) 
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
```

1. See [:material-code-brackets: ResolveConflictsType](./literals.md#resolveconflictstype) 
## UpdateClusterVersionRequestRequestTypeDef

```python
# UpdateClusterVersionRequestRequestTypeDef definition

class UpdateClusterVersionRequestRequestTypeDef(TypedDict):
    name: str,
    version: str,
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
## AddonHealthTypeDef

```python
# AddonHealthTypeDef definition

class AddonHealthTypeDef(TypedDict):
    issues: NotRequired[List[AddonIssueTypeDef]],  # (1)
```

1. See [:material-code-braces: AddonIssueTypeDef](./type_defs.md#addonissuetypedef) 
## AddonVersionInfoTypeDef

```python
# AddonVersionInfoTypeDef definition

class AddonVersionInfoTypeDef(TypedDict):
    addonVersion: NotRequired[str],
    architecture: NotRequired[List[str]],
    compatibilities: NotRequired[List[CompatibilityTypeDef]],  # (1)
    requiresConfiguration: NotRequired[bool],
```

1. See [:material-code-braces: CompatibilityTypeDef](./type_defs.md#compatibilitytypedef) 
## DescribeAddonConfigurationResponseTypeDef

```python
# DescribeAddonConfigurationResponseTypeDef definition

class DescribeAddonConfigurationResponseTypeDef(TypedDict):
    addonName: str,
    addonVersion: str,
    configurationSchema: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAddonsResponseTypeDef

```python
# ListAddonsResponseTypeDef definition

class ListAddonsResponseTypeDef(TypedDict):
    addons: List[str],
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListClustersResponseTypeDef

```python
# ListClustersResponseTypeDef definition

class ListClustersResponseTypeDef(TypedDict):
    clusters: List[str],
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFargateProfilesResponseTypeDef

```python
# ListFargateProfilesResponseTypeDef definition

class ListFargateProfilesResponseTypeDef(TypedDict):
    fargateProfileNames: List[str],
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListNodegroupsResponseTypeDef

```python
# ListNodegroupsResponseTypeDef definition

class ListNodegroupsResponseTypeDef(TypedDict):
    nodegroups: List[str],
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
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
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## ClusterHealthTypeDef

```python
# ClusterHealthTypeDef definition

class ClusterHealthTypeDef(TypedDict):
    issues: NotRequired[List[ClusterIssueTypeDef]],  # (1)
```

1. See [:material-code-braces: ClusterIssueTypeDef](./type_defs.md#clusterissuetypedef) 
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
## CreateFargateProfileRequestRequestTypeDef

```python
# CreateFargateProfileRequestRequestTypeDef definition

class CreateFargateProfileRequestRequestTypeDef(TypedDict):
    fargateProfileName: str,
    clusterName: str,
    podExecutionRoleArn: str,
    subnets: NotRequired[Sequence[str]],
    selectors: NotRequired[Sequence[FargateProfileSelectorTypeDef]],  # (1)
    clientRequestToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: FargateProfileSelectorTypeDef](./type_defs.md#fargateprofileselectortypedef) 
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
    selectors: NotRequired[List[FargateProfileSelectorTypeDef]],  # (1)
    status: NotRequired[FargateProfileStatusType],  # (2)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: FargateProfileSelectorTypeDef](./type_defs.md#fargateprofileselectortypedef) 
2. See [:material-code-brackets: FargateProfileStatusType](./literals.md#fargateprofilestatustype) 
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
    capacityType: NotRequired[CapacityTypesType],  # (7)
    version: NotRequired[str],
    releaseVersion: NotRequired[str],
```

1. See [:material-code-braces: NodegroupScalingConfigTypeDef](./type_defs.md#nodegroupscalingconfigtypedef) 
2. See [:material-code-brackets: AMITypesType](./literals.md#amitypestype) 
3. See [:material-code-braces: RemoteAccessConfigTypeDef](./type_defs.md#remoteaccessconfigtypedef) 
4. See [:material-code-braces: TaintTypeDef](./type_defs.md#tainttypedef) 
5. See [:material-code-braces: LaunchTemplateSpecificationTypeDef](./type_defs.md#launchtemplatespecificationtypedef) 
6. See [:material-code-braces: NodegroupUpdateConfigTypeDef](./type_defs.md#nodegroupupdateconfigtypedef) 
7. See [:material-code-brackets: CapacityTypesType](./literals.md#capacitytypestype) 
## UpdateTaintsPayloadTypeDef

```python
# UpdateTaintsPayloadTypeDef definition

class UpdateTaintsPayloadTypeDef(TypedDict):
    addOrUpdateTaints: NotRequired[Sequence[TaintTypeDef]],  # (1)
    removeTaints: NotRequired[Sequence[TaintTypeDef]],  # (1)
```

1. See [:material-code-braces: TaintTypeDef](./type_defs.md#tainttypedef) 
2. See [:material-code-braces: TaintTypeDef](./type_defs.md#tainttypedef) 
## DescribeAddonRequestAddonActiveWaitTypeDef

```python
# DescribeAddonRequestAddonActiveWaitTypeDef definition

class DescribeAddonRequestAddonActiveWaitTypeDef(TypedDict):
    clusterName: str,
    addonName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeAddonRequestAddonDeletedWaitTypeDef

```python
# DescribeAddonRequestAddonDeletedWaitTypeDef definition

class DescribeAddonRequestAddonDeletedWaitTypeDef(TypedDict):
    clusterName: str,
    addonName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeClusterRequestClusterActiveWaitTypeDef

```python
# DescribeClusterRequestClusterActiveWaitTypeDef definition

class DescribeClusterRequestClusterActiveWaitTypeDef(TypedDict):
    name: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeClusterRequestClusterDeletedWaitTypeDef

```python
# DescribeClusterRequestClusterDeletedWaitTypeDef definition

class DescribeClusterRequestClusterDeletedWaitTypeDef(TypedDict):
    name: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeFargateProfileRequestFargateProfileActiveWaitTypeDef

```python
# DescribeFargateProfileRequestFargateProfileActiveWaitTypeDef definition

class DescribeFargateProfileRequestFargateProfileActiveWaitTypeDef(TypedDict):
    clusterName: str,
    fargateProfileName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef

```python
# DescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef definition

class DescribeFargateProfileRequestFargateProfileDeletedWaitTypeDef(TypedDict):
    clusterName: str,
    fargateProfileName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeNodegroupRequestNodegroupActiveWaitTypeDef

```python
# DescribeNodegroupRequestNodegroupActiveWaitTypeDef definition

class DescribeNodegroupRequestNodegroupActiveWaitTypeDef(TypedDict):
    clusterName: str,
    nodegroupName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeNodegroupRequestNodegroupDeletedWaitTypeDef

```python
# DescribeNodegroupRequestNodegroupDeletedWaitTypeDef definition

class DescribeNodegroupRequestNodegroupDeletedWaitTypeDef(TypedDict):
    clusterName: str,
    nodegroupName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef

```python
# DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef definition

class DescribeAddonVersionsRequestDescribeAddonVersionsPaginateTypeDef(TypedDict):
    kubernetesVersion: NotRequired[str],
    addonName: NotRequired[str],
    types: NotRequired[Sequence[str]],
    publishers: NotRequired[Sequence[str]],
    owners: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAddonsRequestListAddonsPaginateTypeDef

```python
# ListAddonsRequestListAddonsPaginateTypeDef definition

class ListAddonsRequestListAddonsPaginateTypeDef(TypedDict):
    clusterName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListClustersRequestListClustersPaginateTypeDef

```python
# ListClustersRequestListClustersPaginateTypeDef definition

class ListClustersRequestListClustersPaginateTypeDef(TypedDict):
    include: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFargateProfilesRequestListFargateProfilesPaginateTypeDef

```python
# ListFargateProfilesRequestListFargateProfilesPaginateTypeDef definition

class ListFargateProfilesRequestListFargateProfilesPaginateTypeDef(TypedDict):
    clusterName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef

```python
# ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef definition

class ListIdentityProviderConfigsRequestListIdentityProviderConfigsPaginateTypeDef(TypedDict):
    clusterName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNodegroupsRequestListNodegroupsPaginateTypeDef

```python
# ListNodegroupsRequestListNodegroupsPaginateTypeDef definition

class ListNodegroupsRequestListNodegroupsPaginateTypeDef(TypedDict):
    clusterName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUpdatesRequestListUpdatesPaginateTypeDef

```python
# ListUpdatesRequestListUpdatesPaginateTypeDef definition

class ListUpdatesRequestListUpdatesPaginateTypeDef(TypedDict):
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
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentityProviderConfigTypeDef](./type_defs.md#identityproviderconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EncryptionConfigTypeDef

```python
# EncryptionConfigTypeDef definition

class EncryptionConfigTypeDef(TypedDict):
    resources: NotRequired[Sequence[str]],
    provider: NotRequired[ProviderTypeDef],  # (1)
```

1. See [:material-code-braces: ProviderTypeDef](./type_defs.md#providertypedef) 
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
## NodegroupHealthTypeDef

```python
# NodegroupHealthTypeDef definition

class NodegroupHealthTypeDef(TypedDict):
    issues: NotRequired[List[IssueTypeDef]],  # (1)
```

1. See [:material-code-braces: IssueTypeDef](./type_defs.md#issuetypedef) 
## LoggingTypeDef

```python
# LoggingTypeDef definition

class LoggingTypeDef(TypedDict):
    clusterLogging: NotRequired[Sequence[LogSetupTypeDef]],  # (1)
```

1. See [:material-code-braces: LogSetupTypeDef](./type_defs.md#logsetuptypedef) 
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
    clientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: UpdateLabelsPayloadTypeDef](./type_defs.md#updatelabelspayloadtypedef) 
2. See [:material-code-braces: UpdateTaintsPayloadTypeDef](./type_defs.md#updatetaintspayloadtypedef) 
3. See [:material-code-braces: NodegroupScalingConfigTypeDef](./type_defs.md#nodegroupscalingconfigtypedef) 
4. See [:material-code-braces: NodegroupUpdateConfigTypeDef](./type_defs.md#nodegroupupdateconfigtypedef) 
## AssociateEncryptionConfigRequestRequestTypeDef

```python
# AssociateEncryptionConfigRequestRequestTypeDef definition

class AssociateEncryptionConfigRequestRequestTypeDef(TypedDict):
    clusterName: str,
    encryptionConfig: Sequence[EncryptionConfigTypeDef],  # (1)
    clientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef) 
## DescribeIdentityProviderConfigResponseTypeDef

```python
# DescribeIdentityProviderConfigResponseTypeDef definition

class DescribeIdentityProviderConfigResponseTypeDef(TypedDict):
    identityProviderConfig: IdentityProviderConfigResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentityProviderConfigResponseTypeDef](./type_defs.md#identityproviderconfigresponsetypedef) 
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
    remoteAccess: NotRequired[RemoteAccessConfigTypeDef],  # (4)
    amiType: NotRequired[AMITypesType],  # (5)
    nodeRole: NotRequired[str],
    labels: NotRequired[Dict[str, str]],
    taints: NotRequired[List[TaintTypeDef]],  # (6)
    resources: NotRequired[NodegroupResourcesTypeDef],  # (7)
    diskSize: NotRequired[int],
    health: NotRequired[NodegroupHealthTypeDef],  # (8)
    updateConfig: NotRequired[NodegroupUpdateConfigTypeDef],  # (9)
    launchTemplate: NotRequired[LaunchTemplateSpecificationTypeDef],  # (10)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: NodegroupStatusType](./literals.md#nodegroupstatustype) 
2. See [:material-code-brackets: CapacityTypesType](./literals.md#capacitytypestype) 
3. See [:material-code-braces: NodegroupScalingConfigTypeDef](./type_defs.md#nodegroupscalingconfigtypedef) 
4. See [:material-code-braces: RemoteAccessConfigTypeDef](./type_defs.md#remoteaccessconfigtypedef) 
5. See [:material-code-brackets: AMITypesType](./literals.md#amitypestype) 
6. See [:material-code-braces: TaintTypeDef](./type_defs.md#tainttypedef) 
7. See [:material-code-braces: NodegroupResourcesTypeDef](./type_defs.md#nodegroupresourcestypedef) 
8. See [:material-code-braces: NodegroupHealthTypeDef](./type_defs.md#nodegrouphealthtypedef) 
9. See [:material-code-braces: NodegroupUpdateConfigTypeDef](./type_defs.md#nodegroupupdateconfigtypedef) 
10. See [:material-code-braces: LaunchTemplateSpecificationTypeDef](./type_defs.md#launchtemplatespecificationtypedef) 
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
    logging: NotRequired[LoggingTypeDef],  # (3)
    identity: NotRequired[IdentityTypeDef],  # (4)
    status: NotRequired[ClusterStatusType],  # (5)
    certificateAuthority: NotRequired[CertificateTypeDef],  # (6)
    clientRequestToken: NotRequired[str],
    platformVersion: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    encryptionConfig: NotRequired[List[EncryptionConfigTypeDef]],  # (7)
    connectorConfig: NotRequired[ConnectorConfigResponseTypeDef],  # (8)
    id: NotRequired[str],
    health: NotRequired[ClusterHealthTypeDef],  # (9)
    outpostConfig: NotRequired[OutpostConfigResponseTypeDef],  # (10)
```

1. See [:material-code-braces: VpcConfigResponseTypeDef](./type_defs.md#vpcconfigresponsetypedef) 
2. See [:material-code-braces: KubernetesNetworkConfigResponseTypeDef](./type_defs.md#kubernetesnetworkconfigresponsetypedef) 
3. See [:material-code-braces: LoggingTypeDef](./type_defs.md#loggingtypedef) 
4. See [:material-code-braces: IdentityTypeDef](./type_defs.md#identitytypedef) 
5. See [:material-code-brackets: ClusterStatusType](./literals.md#clusterstatustype) 
6. See [:material-code-braces: CertificateTypeDef](./type_defs.md#certificatetypedef) 
7. See [:material-code-braces: EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef) 
8. See [:material-code-braces: ConnectorConfigResponseTypeDef](./type_defs.md#connectorconfigresponsetypedef) 
9. See [:material-code-braces: ClusterHealthTypeDef](./type_defs.md#clusterhealthtypedef) 
10. See [:material-code-braces: OutpostConfigResponseTypeDef](./type_defs.md#outpostconfigresponsetypedef) 
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
```

1. See [:material-code-braces: VpcConfigRequestTypeDef](./type_defs.md#vpcconfigrequesttypedef) 
2. See [:material-code-braces: KubernetesNetworkConfigRequestTypeDef](./type_defs.md#kubernetesnetworkconfigrequesttypedef) 
3. See [:material-code-braces: LoggingTypeDef](./type_defs.md#loggingtypedef) 
4. See [:material-code-braces: EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef) 
5. See [:material-code-braces: OutpostConfigRequestTypeDef](./type_defs.md#outpostconfigrequesttypedef) 
## UpdateClusterConfigRequestRequestTypeDef

```python
# UpdateClusterConfigRequestRequestTypeDef definition

class UpdateClusterConfigRequestRequestTypeDef(TypedDict):
    name: str,
    resourcesVpcConfig: NotRequired[VpcConfigRequestTypeDef],  # (1)
    logging: NotRequired[LoggingTypeDef],  # (2)
    clientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: VpcConfigRequestTypeDef](./type_defs.md#vpcconfigrequesttypedef) 
2. See [:material-code-braces: LoggingTypeDef](./type_defs.md#loggingtypedef) 
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
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AddonInfoTypeDef](./type_defs.md#addoninfotypedef) 
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
