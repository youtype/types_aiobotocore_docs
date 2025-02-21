# Type definitions

> [Index](../README.md) > [EKS](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [EKS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#eks)
    type annotations stubs module [types-aiobotocore-eks](https://pypi.org/project/types-aiobotocore-eks/).

## AccessScopeUnionTypeDef

```python
# AccessScopeUnionTypeDef Union usage example

from types_aiobotocore_eks.type_defs import AccessScopeUnionTypeDef


def get_value() -> AccessScopeUnionTypeDef:
    return ...


# AccessScopeUnionTypeDef definition

AccessScopeUnionTypeDef = Union[
    AccessScopeTypeDef,  # (1)
    AccessScopeOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AccessScopeTypeDef](./type_defs.md#accessscopetypedef) 
2. See [:material-code-braces: AccessScopeOutputTypeDef](./type_defs.md#accessscopeoutputtypedef) 

## FargateProfileSelectorUnionTypeDef

```python
# FargateProfileSelectorUnionTypeDef Union usage example

from types_aiobotocore_eks.type_defs import FargateProfileSelectorUnionTypeDef


def get_value() -> FargateProfileSelectorUnionTypeDef:
    return ...


# FargateProfileSelectorUnionTypeDef definition

FargateProfileSelectorUnionTypeDef = Union[
    FargateProfileSelectorTypeDef,  # (1)
    FargateProfileSelectorOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FargateProfileSelectorTypeDef](./type_defs.md#fargateprofileselectortypedef) 
2. See [:material-code-braces: FargateProfileSelectorOutputTypeDef](./type_defs.md#fargateprofileselectoroutputtypedef) 

## RemoteAccessConfigUnionTypeDef

```python
# RemoteAccessConfigUnionTypeDef Union usage example

from types_aiobotocore_eks.type_defs import RemoteAccessConfigUnionTypeDef


def get_value() -> RemoteAccessConfigUnionTypeDef:
    return ...


# RemoteAccessConfigUnionTypeDef definition

RemoteAccessConfigUnionTypeDef = Union[
    RemoteAccessConfigTypeDef,  # (1)
    RemoteAccessConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RemoteAccessConfigTypeDef](./type_defs.md#remoteaccessconfigtypedef) 
2. See [:material-code-braces: RemoteAccessConfigOutputTypeDef](./type_defs.md#remoteaccessconfigoutputtypedef) 

## RemoteNodeNetworkUnionTypeDef

```python
# RemoteNodeNetworkUnionTypeDef Union usage example

from types_aiobotocore_eks.type_defs import RemoteNodeNetworkUnionTypeDef


def get_value() -> RemoteNodeNetworkUnionTypeDef:
    return ...


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
# RemotePodNetworkUnionTypeDef Union usage example

from types_aiobotocore_eks.type_defs import RemotePodNetworkUnionTypeDef


def get_value() -> RemotePodNetworkUnionTypeDef:
    return ...


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
# EncryptionConfigUnionTypeDef Union usage example

from types_aiobotocore_eks.type_defs import EncryptionConfigUnionTypeDef


def get_value() -> EncryptionConfigUnionTypeDef:
    return ...


# EncryptionConfigUnionTypeDef definition

EncryptionConfigUnionTypeDef = Union[
    EncryptionConfigTypeDef,  # (1)
    EncryptionConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef) 
2. See [:material-code-braces: EncryptionConfigOutputTypeDef](./type_defs.md#encryptionconfigoutputtypedef) 

## LoggingUnionTypeDef

```python
# LoggingUnionTypeDef Union usage example

from types_aiobotocore_eks.type_defs import LoggingUnionTypeDef


def get_value() -> LoggingUnionTypeDef:
    return ...


# LoggingUnionTypeDef definition

LoggingUnionTypeDef = Union[
    LoggingTypeDef,  # (1)
    LoggingOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: LoggingTypeDef](./type_defs.md#loggingtypedef) 
2. See [:material-code-braces: LoggingOutputTypeDef](./type_defs.md#loggingoutputtypedef) 



## AccessConfigResponseTypeDef

```python
# AccessConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import AccessConfigResponseTypeDef


def get_value() -> AccessConfigResponseTypeDef:
    return {
        "bootstrapClusterCreatorAdminPermissions": ...,
    }


# AccessConfigResponseTypeDef definition

class AccessConfigResponseTypeDef(TypedDict):
    bootstrapClusterCreatorAdminPermissions: NotRequired[bool],
    authenticationMode: NotRequired[AuthenticationModeType],  # (1)
```

1. See [:material-code-brackets: AuthenticationModeType](./literals.md#authenticationmodetype) 
## AccessEntryTypeDef

```python
# AccessEntryTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import AccessEntryTypeDef


def get_value() -> AccessEntryTypeDef:
    return {
        "clusterName": ...,
    }


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
# AccessPolicyTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import AccessPolicyTypeDef


def get_value() -> AccessPolicyTypeDef:
    return {
        "name": ...,
    }


# AccessPolicyTypeDef definition

class AccessPolicyTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
```

## AccessScopeOutputTypeDef

```python
# AccessScopeOutputTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import AccessScopeOutputTypeDef


def get_value() -> AccessScopeOutputTypeDef:
    return {
        "type": ...,
    }


# AccessScopeOutputTypeDef definition

class AccessScopeOutputTypeDef(TypedDict):
    type: NotRequired[AccessScopeTypeType],  # (1)
    namespaces: NotRequired[List[str]],
```

1. See [:material-code-brackets: AccessScopeTypeType](./literals.md#accessscopetypetype) 
## AccessScopeTypeDef

```python
# AccessScopeTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import AccessScopeTypeDef


def get_value() -> AccessScopeTypeDef:
    return {
        "type": ...,
    }


# AccessScopeTypeDef definition

class AccessScopeTypeDef(TypedDict):
    type: NotRequired[AccessScopeTypeType],  # (1)
    namespaces: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: AccessScopeTypeType](./literals.md#accessscopetypetype) 
## AddonCompatibilityDetailTypeDef

```python
# AddonCompatibilityDetailTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import AddonCompatibilityDetailTypeDef


def get_value() -> AddonCompatibilityDetailTypeDef:
    return {
        "name": ...,
    }


# AddonCompatibilityDetailTypeDef definition

class AddonCompatibilityDetailTypeDef(TypedDict):
    name: NotRequired[str],
    compatibleVersions: NotRequired[List[str]],
```

## AddonIssueTypeDef

```python
# AddonIssueTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import AddonIssueTypeDef


def get_value() -> AddonIssueTypeDef:
    return {
        "code": ...,
    }


# AddonIssueTypeDef definition

class AddonIssueTypeDef(TypedDict):
    code: NotRequired[AddonIssueCodeType],  # (1)
    message: NotRequired[str],
    resourceIds: NotRequired[List[str]],
```

1. See [:material-code-brackets: AddonIssueCodeType](./literals.md#addonissuecodetype) 
## MarketplaceInformationTypeDef

```python
# MarketplaceInformationTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import MarketplaceInformationTypeDef


def get_value() -> MarketplaceInformationTypeDef:
    return {
        "productId": ...,
    }


# MarketplaceInformationTypeDef definition

class MarketplaceInformationTypeDef(TypedDict):
    productId: NotRequired[str],
    productUrl: NotRequired[str],
```

## AddonPodIdentityAssociationsTypeDef

```python
# AddonPodIdentityAssociationsTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import AddonPodIdentityAssociationsTypeDef


def get_value() -> AddonPodIdentityAssociationsTypeDef:
    return {
        "serviceAccount": ...,
    }


# AddonPodIdentityAssociationsTypeDef definition

class AddonPodIdentityAssociationsTypeDef(TypedDict):
    serviceAccount: str,
    roleArn: str,
```

## AddonPodIdentityConfigurationTypeDef

```python
# AddonPodIdentityConfigurationTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import AddonPodIdentityConfigurationTypeDef


def get_value() -> AddonPodIdentityConfigurationTypeDef:
    return {
        "serviceAccount": ...,
    }


# AddonPodIdentityConfigurationTypeDef definition

class AddonPodIdentityConfigurationTypeDef(TypedDict):
    serviceAccount: NotRequired[str],
    recommendedManagedPolicies: NotRequired[List[str]],
```

## CompatibilityTypeDef

```python
# CompatibilityTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import CompatibilityTypeDef


def get_value() -> CompatibilityTypeDef:
    return {
        "clusterVersion": ...,
    }


# CompatibilityTypeDef definition

class CompatibilityTypeDef(TypedDict):
    clusterVersion: NotRequired[str],
    platformVersions: NotRequired[List[str]],
    defaultVersion: NotRequired[bool],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ResponseMetadataTypeDef


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

## OidcIdentityProviderConfigRequestTypeDef

```python
# OidcIdentityProviderConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import OidcIdentityProviderConfigRequestTypeDef


def get_value() -> OidcIdentityProviderConfigRequestTypeDef:
    return {
        "identityProviderConfigName": ...,
    }


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
# AutoScalingGroupTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import AutoScalingGroupTypeDef


def get_value() -> AutoScalingGroupTypeDef:
    return {
        "name": ...,
    }


# AutoScalingGroupTypeDef definition

class AutoScalingGroupTypeDef(TypedDict):
    name: NotRequired[str],
```

## BlockStorageTypeDef

```python
# BlockStorageTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import BlockStorageTypeDef


def get_value() -> BlockStorageTypeDef:
    return {
        "enabled": ...,
    }


# BlockStorageTypeDef definition

class BlockStorageTypeDef(TypedDict):
    enabled: NotRequired[bool],
```

## CertificateTypeDef

```python
# CertificateTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import CertificateTypeDef


def get_value() -> CertificateTypeDef:
    return {
        "data": ...,
    }


# CertificateTypeDef definition

class CertificateTypeDef(TypedDict):
    data: NotRequired[str],
```

## ClientStatTypeDef

```python
# ClientStatTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ClientStatTypeDef


def get_value() -> ClientStatTypeDef:
    return {
        "userAgent": ...,
    }


# ClientStatTypeDef definition

class ClientStatTypeDef(TypedDict):
    userAgent: NotRequired[str],
    numberOfRequestsLast30Days: NotRequired[int],
    lastRequestTime: NotRequired[datetime],
```

## ClusterIssueTypeDef

```python
# ClusterIssueTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ClusterIssueTypeDef


def get_value() -> ClusterIssueTypeDef:
    return {
        "code": ...,
    }


# ClusterIssueTypeDef definition

class ClusterIssueTypeDef(TypedDict):
    code: NotRequired[ClusterIssueCodeType],  # (1)
    message: NotRequired[str],
    resourceIds: NotRequired[List[str]],
```

1. See [:material-code-brackets: ClusterIssueCodeType](./literals.md#clusterissuecodetype) 
## ComputeConfigResponseTypeDef

```python
# ComputeConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ComputeConfigResponseTypeDef


def get_value() -> ComputeConfigResponseTypeDef:
    return {
        "enabled": ...,
    }


# ComputeConfigResponseTypeDef definition

class ComputeConfigResponseTypeDef(TypedDict):
    enabled: NotRequired[bool],
    nodePools: NotRequired[List[str]],
    nodeRoleArn: NotRequired[str],
```

## ConnectorConfigResponseTypeDef

```python
# ConnectorConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ConnectorConfigResponseTypeDef


def get_value() -> ConnectorConfigResponseTypeDef:
    return {
        "activationId": ...,
    }


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
# UpgradePolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import UpgradePolicyResponseTypeDef


def get_value() -> UpgradePolicyResponseTypeDef:
    return {
        "supportType": ...,
    }


# UpgradePolicyResponseTypeDef definition

class UpgradePolicyResponseTypeDef(TypedDict):
    supportType: NotRequired[SupportTypeType],  # (1)
```

1. See [:material-code-brackets: SupportTypeType](./literals.md#supporttypetype) 
## VpcConfigResponseTypeDef

```python
# VpcConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import VpcConfigResponseTypeDef


def get_value() -> VpcConfigResponseTypeDef:
    return {
        "subnetIds": ...,
    }


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
# ZonalShiftConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ZonalShiftConfigResponseTypeDef


def get_value() -> ZonalShiftConfigResponseTypeDef:
    return {
        "enabled": ...,
    }


# ZonalShiftConfigResponseTypeDef definition

class ZonalShiftConfigResponseTypeDef(TypedDict):
    enabled: NotRequired[bool],
```

## ClusterVersionInformationTypeDef

```python
# ClusterVersionInformationTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ClusterVersionInformationTypeDef


def get_value() -> ClusterVersionInformationTypeDef:
    return {
        "clusterVersion": ...,
    }


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
    versionStatus: NotRequired[VersionStatusType],  # (2)
    kubernetesPatchVersion: NotRequired[str],
```

1. See [:material-code-brackets: ClusterVersionStatusType](./literals.md#clusterversionstatustype) 
2. See [:material-code-brackets: VersionStatusType](./literals.md#versionstatustype) 
## ComputeConfigRequestTypeDef

```python
# ComputeConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ComputeConfigRequestTypeDef


def get_value() -> ComputeConfigRequestTypeDef:
    return {
        "enabled": ...,
    }


# ComputeConfigRequestTypeDef definition

class ComputeConfigRequestTypeDef(TypedDict):
    enabled: NotRequired[bool],
    nodePools: NotRequired[Sequence[str]],
    nodeRoleArn: NotRequired[str],
```

## ConnectorConfigRequestTypeDef

```python
# ConnectorConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ConnectorConfigRequestTypeDef


def get_value() -> ConnectorConfigRequestTypeDef:
    return {
        "roleArn": ...,
    }


# ConnectorConfigRequestTypeDef definition

class ConnectorConfigRequestTypeDef(TypedDict):
    roleArn: str,
    provider: ConnectorConfigProviderType,  # (1)
```

1. See [:material-code-brackets: ConnectorConfigProviderType](./literals.md#connectorconfigprovidertype) 
## ControlPlanePlacementRequestTypeDef

```python
# ControlPlanePlacementRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ControlPlanePlacementRequestTypeDef


def get_value() -> ControlPlanePlacementRequestTypeDef:
    return {
        "groupName": ...,
    }


# ControlPlanePlacementRequestTypeDef definition

class ControlPlanePlacementRequestTypeDef(TypedDict):
    groupName: NotRequired[str],
```

## ControlPlanePlacementResponseTypeDef

```python
# ControlPlanePlacementResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ControlPlanePlacementResponseTypeDef


def get_value() -> ControlPlanePlacementResponseTypeDef:
    return {
        "groupName": ...,
    }


# ControlPlanePlacementResponseTypeDef definition

class ControlPlanePlacementResponseTypeDef(TypedDict):
    groupName: NotRequired[str],
```

## CreateAccessConfigRequestTypeDef

```python
# CreateAccessConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import CreateAccessConfigRequestTypeDef


def get_value() -> CreateAccessConfigRequestTypeDef:
    return {
        "bootstrapClusterCreatorAdminPermissions": ...,
    }


# CreateAccessConfigRequestTypeDef definition

class CreateAccessConfigRequestTypeDef(TypedDict):
    bootstrapClusterCreatorAdminPermissions: NotRequired[bool],
    authenticationMode: NotRequired[AuthenticationModeType],  # (1)
```

1. See [:material-code-brackets: AuthenticationModeType](./literals.md#authenticationmodetype) 
## CreateAccessEntryRequestTypeDef

```python
# CreateAccessEntryRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import CreateAccessEntryRequestTypeDef


def get_value() -> CreateAccessEntryRequestTypeDef:
    return {
        "clusterName": ...,
    }


# CreateAccessEntryRequestTypeDef definition

class CreateAccessEntryRequestTypeDef(TypedDict):
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
# UpgradePolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import UpgradePolicyRequestTypeDef


def get_value() -> UpgradePolicyRequestTypeDef:
    return {
        "supportType": ...,
    }


# UpgradePolicyRequestTypeDef definition

class UpgradePolicyRequestTypeDef(TypedDict):
    supportType: NotRequired[SupportTypeType],  # (1)
```

1. See [:material-code-brackets: SupportTypeType](./literals.md#supporttypetype) 
## VpcConfigRequestTypeDef

```python
# VpcConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import VpcConfigRequestTypeDef


def get_value() -> VpcConfigRequestTypeDef:
    return {
        "subnetIds": ...,
    }


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
# ZonalShiftConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ZonalShiftConfigRequestTypeDef


def get_value() -> ZonalShiftConfigRequestTypeDef:
    return {
        "enabled": ...,
    }


# ZonalShiftConfigRequestTypeDef definition

class ZonalShiftConfigRequestTypeDef(TypedDict):
    enabled: NotRequired[bool],
```

## EksAnywhereSubscriptionTermTypeDef

```python
# EksAnywhereSubscriptionTermTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import EksAnywhereSubscriptionTermTypeDef


def get_value() -> EksAnywhereSubscriptionTermTypeDef:
    return {
        "duration": ...,
    }


# EksAnywhereSubscriptionTermTypeDef definition

class EksAnywhereSubscriptionTermTypeDef(TypedDict):
    duration: NotRequired[int],
    unit: NotRequired[EksAnywhereSubscriptionTermUnitType],  # (1)
```

1. See [:material-code-brackets: EksAnywhereSubscriptionTermUnitType](./literals.md#eksanywheresubscriptiontermunittype) 
## LaunchTemplateSpecificationTypeDef

```python
# LaunchTemplateSpecificationTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import LaunchTemplateSpecificationTypeDef


def get_value() -> LaunchTemplateSpecificationTypeDef:
    return {
        "name": ...,
    }


# LaunchTemplateSpecificationTypeDef definition

class LaunchTemplateSpecificationTypeDef(TypedDict):
    name: NotRequired[str],
    version: NotRequired[str],
    id: NotRequired[str],
```

## NodeRepairConfigTypeDef

```python
# NodeRepairConfigTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import NodeRepairConfigTypeDef


def get_value() -> NodeRepairConfigTypeDef:
    return {
        "enabled": ...,
    }


# NodeRepairConfigTypeDef definition

class NodeRepairConfigTypeDef(TypedDict):
    enabled: NotRequired[bool],
```

## NodegroupScalingConfigTypeDef

```python
# NodegroupScalingConfigTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import NodegroupScalingConfigTypeDef


def get_value() -> NodegroupScalingConfigTypeDef:
    return {
        "minSize": ...,
    }


# NodegroupScalingConfigTypeDef definition

class NodegroupScalingConfigTypeDef(TypedDict):
    minSize: NotRequired[int],
    maxSize: NotRequired[int],
    desiredSize: NotRequired[int],
```

## NodegroupUpdateConfigTypeDef

```python
# NodegroupUpdateConfigTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import NodegroupUpdateConfigTypeDef


def get_value() -> NodegroupUpdateConfigTypeDef:
    return {
        "maxUnavailable": ...,
    }


# NodegroupUpdateConfigTypeDef definition

class NodegroupUpdateConfigTypeDef(TypedDict):
    maxUnavailable: NotRequired[int],
    maxUnavailablePercentage: NotRequired[int],
    updateStrategy: NotRequired[NodegroupUpdateStrategiesType],  # (1)
```

1. See [:material-code-brackets: NodegroupUpdateStrategiesType](./literals.md#nodegroupupdatestrategiestype) 
## TaintTypeDef

```python
# TaintTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import TaintTypeDef


def get_value() -> TaintTypeDef:
    return {
        "key": ...,
    }


# TaintTypeDef definition

class TaintTypeDef(TypedDict):
    key: NotRequired[str],
    value: NotRequired[str],
    effect: NotRequired[TaintEffectType],  # (1)
```

1. See [:material-code-brackets: TaintEffectType](./literals.md#tainteffecttype) 
## CreatePodIdentityAssociationRequestTypeDef

```python
# CreatePodIdentityAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import CreatePodIdentityAssociationRequestTypeDef


def get_value() -> CreatePodIdentityAssociationRequestTypeDef:
    return {
        "clusterName": ...,
    }


# CreatePodIdentityAssociationRequestTypeDef definition

class CreatePodIdentityAssociationRequestTypeDef(TypedDict):
    clusterName: str,
    namespace: str,
    serviceAccount: str,
    roleArn: str,
    clientRequestToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## PodIdentityAssociationTypeDef

```python
# PodIdentityAssociationTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import PodIdentityAssociationTypeDef


def get_value() -> PodIdentityAssociationTypeDef:
    return {
        "clusterName": ...,
    }


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

## DeleteAccessEntryRequestTypeDef

```python
# DeleteAccessEntryRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DeleteAccessEntryRequestTypeDef


def get_value() -> DeleteAccessEntryRequestTypeDef:
    return {
        "clusterName": ...,
    }


# DeleteAccessEntryRequestTypeDef definition

class DeleteAccessEntryRequestTypeDef(TypedDict):
    clusterName: str,
    principalArn: str,
```

## DeleteAddonRequestTypeDef

```python
# DeleteAddonRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DeleteAddonRequestTypeDef


def get_value() -> DeleteAddonRequestTypeDef:
    return {
        "clusterName": ...,
    }


# DeleteAddonRequestTypeDef definition

class DeleteAddonRequestTypeDef(TypedDict):
    clusterName: str,
    addonName: str,
    preserve: NotRequired[bool],
```

## DeleteClusterRequestTypeDef

```python
# DeleteClusterRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DeleteClusterRequestTypeDef


def get_value() -> DeleteClusterRequestTypeDef:
    return {
        "name": ...,
    }


# DeleteClusterRequestTypeDef definition

class DeleteClusterRequestTypeDef(TypedDict):
    name: str,
```

## DeleteEksAnywhereSubscriptionRequestTypeDef

```python
# DeleteEksAnywhereSubscriptionRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DeleteEksAnywhereSubscriptionRequestTypeDef


def get_value() -> DeleteEksAnywhereSubscriptionRequestTypeDef:
    return {
        "id": ...,
    }


# DeleteEksAnywhereSubscriptionRequestTypeDef definition

class DeleteEksAnywhereSubscriptionRequestTypeDef(TypedDict):
    id: str,
```

## DeleteFargateProfileRequestTypeDef

```python
# DeleteFargateProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DeleteFargateProfileRequestTypeDef


def get_value() -> DeleteFargateProfileRequestTypeDef:
    return {
        "clusterName": ...,
    }


# DeleteFargateProfileRequestTypeDef definition

class DeleteFargateProfileRequestTypeDef(TypedDict):
    clusterName: str,
    fargateProfileName: str,
```

## DeleteNodegroupRequestTypeDef

```python
# DeleteNodegroupRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DeleteNodegroupRequestTypeDef


def get_value() -> DeleteNodegroupRequestTypeDef:
    return {
        "clusterName": ...,
    }


# DeleteNodegroupRequestTypeDef definition

class DeleteNodegroupRequestTypeDef(TypedDict):
    clusterName: str,
    nodegroupName: str,
```

## DeletePodIdentityAssociationRequestTypeDef

```python
# DeletePodIdentityAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DeletePodIdentityAssociationRequestTypeDef


def get_value() -> DeletePodIdentityAssociationRequestTypeDef:
    return {
        "clusterName": ...,
    }


# DeletePodIdentityAssociationRequestTypeDef definition

class DeletePodIdentityAssociationRequestTypeDef(TypedDict):
    clusterName: str,
    associationId: str,
```

## DeregisterClusterRequestTypeDef

```python
# DeregisterClusterRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DeregisterClusterRequestTypeDef


def get_value() -> DeregisterClusterRequestTypeDef:
    return {
        "name": ...,
    }


# DeregisterClusterRequestTypeDef definition

class DeregisterClusterRequestTypeDef(TypedDict):
    name: str,
```

## DescribeAccessEntryRequestTypeDef

```python
# DescribeAccessEntryRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeAccessEntryRequestTypeDef


def get_value() -> DescribeAccessEntryRequestTypeDef:
    return {
        "clusterName": ...,
    }


# DescribeAccessEntryRequestTypeDef definition

class DescribeAccessEntryRequestTypeDef(TypedDict):
    clusterName: str,
    principalArn: str,
```

## DescribeAddonConfigurationRequestTypeDef

```python
# DescribeAddonConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeAddonConfigurationRequestTypeDef


def get_value() -> DescribeAddonConfigurationRequestTypeDef:
    return {
        "addonName": ...,
    }


# DescribeAddonConfigurationRequestTypeDef definition

class DescribeAddonConfigurationRequestTypeDef(TypedDict):
    addonName: str,
    addonVersion: str,
```

## DescribeAddonRequestTypeDef

```python
# DescribeAddonRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeAddonRequestTypeDef


def get_value() -> DescribeAddonRequestTypeDef:
    return {
        "clusterName": ...,
    }


# DescribeAddonRequestTypeDef definition

class DescribeAddonRequestTypeDef(TypedDict):
    clusterName: str,
    addonName: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import WaiterConfigTypeDef


def get_value() -> WaiterConfigTypeDef:
    return {
        "Delay": ...,
    }


# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeAddonVersionsRequestTypeDef

```python
# DescribeAddonVersionsRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeAddonVersionsRequestTypeDef


def get_value() -> DescribeAddonVersionsRequestTypeDef:
    return {
        "kubernetesVersion": ...,
    }


# DescribeAddonVersionsRequestTypeDef definition

class DescribeAddonVersionsRequestTypeDef(TypedDict):
    kubernetesVersion: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    addonName: NotRequired[str],
    types: NotRequired[Sequence[str]],
    publishers: NotRequired[Sequence[str]],
    owners: NotRequired[Sequence[str]],
```

## DescribeClusterRequestTypeDef

```python
# DescribeClusterRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeClusterRequestTypeDef


def get_value() -> DescribeClusterRequestTypeDef:
    return {
        "name": ...,
    }


# DescribeClusterRequestTypeDef definition

class DescribeClusterRequestTypeDef(TypedDict):
    name: str,
```

## DescribeClusterVersionsRequestTypeDef

```python
# DescribeClusterVersionsRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeClusterVersionsRequestTypeDef


def get_value() -> DescribeClusterVersionsRequestTypeDef:
    return {
        "clusterType": ...,
    }


# DescribeClusterVersionsRequestTypeDef definition

class DescribeClusterVersionsRequestTypeDef(TypedDict):
    clusterType: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    defaultOnly: NotRequired[bool],
    includeAll: NotRequired[bool],
    clusterVersions: NotRequired[Sequence[str]],
    status: NotRequired[ClusterVersionStatusType],  # (1)
    versionStatus: NotRequired[VersionStatusType],  # (2)
```

1. See [:material-code-brackets: ClusterVersionStatusType](./literals.md#clusterversionstatustype) 
2. See [:material-code-brackets: VersionStatusType](./literals.md#versionstatustype) 
## DescribeEksAnywhereSubscriptionRequestTypeDef

```python
# DescribeEksAnywhereSubscriptionRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeEksAnywhereSubscriptionRequestTypeDef


def get_value() -> DescribeEksAnywhereSubscriptionRequestTypeDef:
    return {
        "id": ...,
    }


# DescribeEksAnywhereSubscriptionRequestTypeDef definition

class DescribeEksAnywhereSubscriptionRequestTypeDef(TypedDict):
    id: str,
```

## DescribeFargateProfileRequestTypeDef

```python
# DescribeFargateProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeFargateProfileRequestTypeDef


def get_value() -> DescribeFargateProfileRequestTypeDef:
    return {
        "clusterName": ...,
    }


# DescribeFargateProfileRequestTypeDef definition

class DescribeFargateProfileRequestTypeDef(TypedDict):
    clusterName: str,
    fargateProfileName: str,
```

## IdentityProviderConfigTypeDef

```python
# IdentityProviderConfigTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import IdentityProviderConfigTypeDef


def get_value() -> IdentityProviderConfigTypeDef:
    return {
        "type": ...,
    }


# IdentityProviderConfigTypeDef definition

class IdentityProviderConfigTypeDef(TypedDict):
    type: str,
    name: str,
```

## DescribeInsightRequestTypeDef

```python
# DescribeInsightRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeInsightRequestTypeDef


def get_value() -> DescribeInsightRequestTypeDef:
    return {
        "clusterName": ...,
    }


# DescribeInsightRequestTypeDef definition

class DescribeInsightRequestTypeDef(TypedDict):
    clusterName: str,
    id: str,
```

## DescribeNodegroupRequestTypeDef

```python
# DescribeNodegroupRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeNodegroupRequestTypeDef


def get_value() -> DescribeNodegroupRequestTypeDef:
    return {
        "clusterName": ...,
    }


# DescribeNodegroupRequestTypeDef definition

class DescribeNodegroupRequestTypeDef(TypedDict):
    clusterName: str,
    nodegroupName: str,
```

## DescribePodIdentityAssociationRequestTypeDef

```python
# DescribePodIdentityAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribePodIdentityAssociationRequestTypeDef


def get_value() -> DescribePodIdentityAssociationRequestTypeDef:
    return {
        "clusterName": ...,
    }


# DescribePodIdentityAssociationRequestTypeDef definition

class DescribePodIdentityAssociationRequestTypeDef(TypedDict):
    clusterName: str,
    associationId: str,
```

## DescribeUpdateRequestTypeDef

```python
# DescribeUpdateRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeUpdateRequestTypeDef


def get_value() -> DescribeUpdateRequestTypeDef:
    return {
        "name": ...,
    }


# DescribeUpdateRequestTypeDef definition

class DescribeUpdateRequestTypeDef(TypedDict):
    name: str,
    updateId: str,
    nodegroupName: NotRequired[str],
    addonName: NotRequired[str],
```

## DisassociateAccessPolicyRequestTypeDef

```python
# DisassociateAccessPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DisassociateAccessPolicyRequestTypeDef


def get_value() -> DisassociateAccessPolicyRequestTypeDef:
    return {
        "clusterName": ...,
    }


# DisassociateAccessPolicyRequestTypeDef definition

class DisassociateAccessPolicyRequestTypeDef(TypedDict):
    clusterName: str,
    principalArn: str,
    policyArn: str,
```

## ElasticLoadBalancingTypeDef

```python
# ElasticLoadBalancingTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ElasticLoadBalancingTypeDef


def get_value() -> ElasticLoadBalancingTypeDef:
    return {
        "enabled": ...,
    }


# ElasticLoadBalancingTypeDef definition

class ElasticLoadBalancingTypeDef(TypedDict):
    enabled: NotRequired[bool],
```

## ProviderTypeDef

```python
# ProviderTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ProviderTypeDef


def get_value() -> ProviderTypeDef:
    return {
        "keyArn": ...,
    }


# ProviderTypeDef definition

class ProviderTypeDef(TypedDict):
    keyArn: NotRequired[str],
```

## ErrorDetailTypeDef

```python
# ErrorDetailTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ErrorDetailTypeDef


def get_value() -> ErrorDetailTypeDef:
    return {
        "errorCode": ...,
    }


# ErrorDetailTypeDef definition

class ErrorDetailTypeDef(TypedDict):
    errorCode: NotRequired[ErrorCodeType],  # (1)
    errorMessage: NotRequired[str],
    resourceIds: NotRequired[List[str]],
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
## FargateProfileIssueTypeDef

```python
# FargateProfileIssueTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import FargateProfileIssueTypeDef


def get_value() -> FargateProfileIssueTypeDef:
    return {
        "code": ...,
    }


# FargateProfileIssueTypeDef definition

class FargateProfileIssueTypeDef(TypedDict):
    code: NotRequired[FargateProfileIssueCodeType],  # (1)
    message: NotRequired[str],
    resourceIds: NotRequired[List[str]],
```

1. See [:material-code-brackets: FargateProfileIssueCodeType](./literals.md#fargateprofileissuecodetype) 
## FargateProfileSelectorOutputTypeDef

```python
# FargateProfileSelectorOutputTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import FargateProfileSelectorOutputTypeDef


def get_value() -> FargateProfileSelectorOutputTypeDef:
    return {
        "namespace": ...,
    }


# FargateProfileSelectorOutputTypeDef definition

class FargateProfileSelectorOutputTypeDef(TypedDict):
    namespace: NotRequired[str],
    labels: NotRequired[Dict[str, str]],
```

## FargateProfileSelectorTypeDef

```python
# FargateProfileSelectorTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import FargateProfileSelectorTypeDef


def get_value() -> FargateProfileSelectorTypeDef:
    return {
        "namespace": ...,
    }


# FargateProfileSelectorTypeDef definition

class FargateProfileSelectorTypeDef(TypedDict):
    namespace: NotRequired[str],
    labels: NotRequired[Mapping[str, str]],
```

## OidcIdentityProviderConfigTypeDef

```python
# OidcIdentityProviderConfigTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import OidcIdentityProviderConfigTypeDef


def get_value() -> OidcIdentityProviderConfigTypeDef:
    return {
        "identityProviderConfigName": ...,
    }


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
# OIDCTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import OIDCTypeDef


def get_value() -> OIDCTypeDef:
    return {
        "issuer": ...,
    }


# OIDCTypeDef definition

class OIDCTypeDef(TypedDict):
    issuer: NotRequired[str],
```

## InsightStatusTypeDef

```python
# InsightStatusTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import InsightStatusTypeDef


def get_value() -> InsightStatusTypeDef:
    return {
        "status": ...,
    }


# InsightStatusTypeDef definition

class InsightStatusTypeDef(TypedDict):
    status: NotRequired[InsightStatusValueType],  # (1)
    reason: NotRequired[str],
```

1. See [:material-code-brackets: InsightStatusValueType](./literals.md#insightstatusvaluetype) 
## InsightsFilterTypeDef

```python
# InsightsFilterTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import InsightsFilterTypeDef


def get_value() -> InsightsFilterTypeDef:
    return {
        "categories": ...,
    }


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
# IssueTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import IssueTypeDef


def get_value() -> IssueTypeDef:
    return {
        "code": ...,
    }


# IssueTypeDef definition

class IssueTypeDef(TypedDict):
    code: NotRequired[NodegroupIssueCodeType],  # (1)
    message: NotRequired[str],
    resourceIds: NotRequired[List[str]],
```

1. See [:material-code-brackets: NodegroupIssueCodeType](./literals.md#nodegroupissuecodetype) 
## ListAccessEntriesRequestTypeDef

```python
# ListAccessEntriesRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListAccessEntriesRequestTypeDef


def get_value() -> ListAccessEntriesRequestTypeDef:
    return {
        "clusterName": ...,
    }


# ListAccessEntriesRequestTypeDef definition

class ListAccessEntriesRequestTypeDef(TypedDict):
    clusterName: str,
    associatedPolicyArn: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListAccessPoliciesRequestTypeDef

```python
# ListAccessPoliciesRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListAccessPoliciesRequestTypeDef


def get_value() -> ListAccessPoliciesRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListAccessPoliciesRequestTypeDef definition

class ListAccessPoliciesRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListAddonsRequestTypeDef

```python
# ListAddonsRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListAddonsRequestTypeDef


def get_value() -> ListAddonsRequestTypeDef:
    return {
        "clusterName": ...,
    }


# ListAddonsRequestTypeDef definition

class ListAddonsRequestTypeDef(TypedDict):
    clusterName: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListAssociatedAccessPoliciesRequestTypeDef

```python
# ListAssociatedAccessPoliciesRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListAssociatedAccessPoliciesRequestTypeDef


def get_value() -> ListAssociatedAccessPoliciesRequestTypeDef:
    return {
        "clusterName": ...,
    }


# ListAssociatedAccessPoliciesRequestTypeDef definition

class ListAssociatedAccessPoliciesRequestTypeDef(TypedDict):
    clusterName: str,
    principalArn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListClustersRequestTypeDef

```python
# ListClustersRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListClustersRequestTypeDef


def get_value() -> ListClustersRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListClustersRequestTypeDef definition

class ListClustersRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    include: NotRequired[Sequence[str]],
```

## ListEksAnywhereSubscriptionsRequestTypeDef

```python
# ListEksAnywhereSubscriptionsRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListEksAnywhereSubscriptionsRequestTypeDef


def get_value() -> ListEksAnywhereSubscriptionsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListEksAnywhereSubscriptionsRequestTypeDef definition

class ListEksAnywhereSubscriptionsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    includeStatus: NotRequired[Sequence[EksAnywhereSubscriptionStatusType]],  # (1)
```

1. See [:material-code-brackets: EksAnywhereSubscriptionStatusType](./literals.md#eksanywheresubscriptionstatustype) 
## ListFargateProfilesRequestTypeDef

```python
# ListFargateProfilesRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListFargateProfilesRequestTypeDef


def get_value() -> ListFargateProfilesRequestTypeDef:
    return {
        "clusterName": ...,
    }


# ListFargateProfilesRequestTypeDef definition

class ListFargateProfilesRequestTypeDef(TypedDict):
    clusterName: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListIdentityProviderConfigsRequestTypeDef

```python
# ListIdentityProviderConfigsRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListIdentityProviderConfigsRequestTypeDef


def get_value() -> ListIdentityProviderConfigsRequestTypeDef:
    return {
        "clusterName": ...,
    }


# ListIdentityProviderConfigsRequestTypeDef definition

class ListIdentityProviderConfigsRequestTypeDef(TypedDict):
    clusterName: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListNodegroupsRequestTypeDef

```python
# ListNodegroupsRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListNodegroupsRequestTypeDef


def get_value() -> ListNodegroupsRequestTypeDef:
    return {
        "clusterName": ...,
    }


# ListNodegroupsRequestTypeDef definition

class ListNodegroupsRequestTypeDef(TypedDict):
    clusterName: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListPodIdentityAssociationsRequestTypeDef

```python
# ListPodIdentityAssociationsRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListPodIdentityAssociationsRequestTypeDef


def get_value() -> ListPodIdentityAssociationsRequestTypeDef:
    return {
        "clusterName": ...,
    }


# ListPodIdentityAssociationsRequestTypeDef definition

class ListPodIdentityAssociationsRequestTypeDef(TypedDict):
    clusterName: str,
    namespace: NotRequired[str],
    serviceAccount: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## PodIdentityAssociationSummaryTypeDef

```python
# PodIdentityAssociationSummaryTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import PodIdentityAssociationSummaryTypeDef


def get_value() -> PodIdentityAssociationSummaryTypeDef:
    return {
        "clusterName": ...,
    }


# PodIdentityAssociationSummaryTypeDef definition

class PodIdentityAssociationSummaryTypeDef(TypedDict):
    clusterName: NotRequired[str],
    namespace: NotRequired[str],
    serviceAccount: NotRequired[str],
    associationArn: NotRequired[str],
    associationId: NotRequired[str],
    ownerArn: NotRequired[str],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListUpdatesRequestTypeDef

```python
# ListUpdatesRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListUpdatesRequestTypeDef


def get_value() -> ListUpdatesRequestTypeDef:
    return {
        "name": ...,
    }


# ListUpdatesRequestTypeDef definition

class ListUpdatesRequestTypeDef(TypedDict):
    name: str,
    nodegroupName: NotRequired[str],
    addonName: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## LogSetupOutputTypeDef

```python
# LogSetupOutputTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import LogSetupOutputTypeDef


def get_value() -> LogSetupOutputTypeDef:
    return {
        "types": ...,
    }


# LogSetupOutputTypeDef definition

class LogSetupOutputTypeDef(TypedDict):
    types: NotRequired[List[LogTypeType]],  # (1)
    enabled: NotRequired[bool],
```

1. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) 
## LogSetupTypeDef

```python
# LogSetupTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import LogSetupTypeDef


def get_value() -> LogSetupTypeDef:
    return {
        "types": ...,
    }


# LogSetupTypeDef definition

class LogSetupTypeDef(TypedDict):
    types: NotRequired[Sequence[LogTypeType]],  # (1)
    enabled: NotRequired[bool],
```

1. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) 
## RemoteAccessConfigOutputTypeDef

```python
# RemoteAccessConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import RemoteAccessConfigOutputTypeDef


def get_value() -> RemoteAccessConfigOutputTypeDef:
    return {
        "ec2SshKey": ...,
    }


# RemoteAccessConfigOutputTypeDef definition

class RemoteAccessConfigOutputTypeDef(TypedDict):
    ec2SshKey: NotRequired[str],
    sourceSecurityGroups: NotRequired[List[str]],
```

## RemoteAccessConfigTypeDef

```python
# RemoteAccessConfigTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import RemoteAccessConfigTypeDef


def get_value() -> RemoteAccessConfigTypeDef:
    return {
        "ec2SshKey": ...,
    }


# RemoteAccessConfigTypeDef definition

class RemoteAccessConfigTypeDef(TypedDict):
    ec2SshKey: NotRequired[str],
    sourceSecurityGroups: NotRequired[Sequence[str]],
```

## RemoteNodeNetworkOutputTypeDef

```python
# RemoteNodeNetworkOutputTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import RemoteNodeNetworkOutputTypeDef


def get_value() -> RemoteNodeNetworkOutputTypeDef:
    return {
        "cidrs": ...,
    }


# RemoteNodeNetworkOutputTypeDef definition

class RemoteNodeNetworkOutputTypeDef(TypedDict):
    cidrs: NotRequired[List[str]],
```

## RemotePodNetworkOutputTypeDef

```python
# RemotePodNetworkOutputTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import RemotePodNetworkOutputTypeDef


def get_value() -> RemotePodNetworkOutputTypeDef:
    return {
        "cidrs": ...,
    }


# RemotePodNetworkOutputTypeDef definition

class RemotePodNetworkOutputTypeDef(TypedDict):
    cidrs: NotRequired[List[str]],
```

## RemoteNodeNetworkTypeDef

```python
# RemoteNodeNetworkTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import RemoteNodeNetworkTypeDef


def get_value() -> RemoteNodeNetworkTypeDef:
    return {
        "cidrs": ...,
    }


# RemoteNodeNetworkTypeDef definition

class RemoteNodeNetworkTypeDef(TypedDict):
    cidrs: NotRequired[Sequence[str]],
```

## RemotePodNetworkTypeDef

```python
# RemotePodNetworkTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import RemotePodNetworkTypeDef


def get_value() -> RemotePodNetworkTypeDef:
    return {
        "cidrs": ...,
    }


# RemotePodNetworkTypeDef definition

class RemotePodNetworkTypeDef(TypedDict):
    cidrs: NotRequired[Sequence[str]],
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateAccessConfigRequestTypeDef

```python
# UpdateAccessConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import UpdateAccessConfigRequestTypeDef


def get_value() -> UpdateAccessConfigRequestTypeDef:
    return {
        "authenticationMode": ...,
    }


# UpdateAccessConfigRequestTypeDef definition

class UpdateAccessConfigRequestTypeDef(TypedDict):
    authenticationMode: NotRequired[AuthenticationModeType],  # (1)
```

1. See [:material-code-brackets: AuthenticationModeType](./literals.md#authenticationmodetype) 
## UpdateAccessEntryRequestTypeDef

```python
# UpdateAccessEntryRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import UpdateAccessEntryRequestTypeDef


def get_value() -> UpdateAccessEntryRequestTypeDef:
    return {
        "clusterName": ...,
    }


# UpdateAccessEntryRequestTypeDef definition

class UpdateAccessEntryRequestTypeDef(TypedDict):
    clusterName: str,
    principalArn: str,
    kubernetesGroups: NotRequired[Sequence[str]],
    clientRequestToken: NotRequired[str],
    username: NotRequired[str],
```

## UpdateClusterVersionRequestTypeDef

```python
# UpdateClusterVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import UpdateClusterVersionRequestTypeDef


def get_value() -> UpdateClusterVersionRequestTypeDef:
    return {
        "name": ...,
    }


# UpdateClusterVersionRequestTypeDef definition

class UpdateClusterVersionRequestTypeDef(TypedDict):
    name: str,
    version: str,
    clientRequestToken: NotRequired[str],
```

## UpdateEksAnywhereSubscriptionRequestTypeDef

```python
# UpdateEksAnywhereSubscriptionRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import UpdateEksAnywhereSubscriptionRequestTypeDef


def get_value() -> UpdateEksAnywhereSubscriptionRequestTypeDef:
    return {
        "id": ...,
    }


# UpdateEksAnywhereSubscriptionRequestTypeDef definition

class UpdateEksAnywhereSubscriptionRequestTypeDef(TypedDict):
    id: str,
    autoRenew: bool,
    clientRequestToken: NotRequired[str],
```

## UpdateLabelsPayloadTypeDef

```python
# UpdateLabelsPayloadTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import UpdateLabelsPayloadTypeDef


def get_value() -> UpdateLabelsPayloadTypeDef:
    return {
        "addOrUpdateLabels": ...,
    }


# UpdateLabelsPayloadTypeDef definition

class UpdateLabelsPayloadTypeDef(TypedDict):
    addOrUpdateLabels: NotRequired[Mapping[str, str]],
    removeLabels: NotRequired[Sequence[str]],
```

## UpdateParamTypeDef

```python
# UpdateParamTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import UpdateParamTypeDef


def get_value() -> UpdateParamTypeDef:
    return {
        "type": ...,
    }


# UpdateParamTypeDef definition

class UpdateParamTypeDef(TypedDict):
    type: NotRequired[UpdateParamTypeType],  # (1)
    value: NotRequired[str],
```

1. See [:material-code-brackets: UpdateParamTypeType](./literals.md#updateparamtypetype) 
## UpdatePodIdentityAssociationRequestTypeDef

```python
# UpdatePodIdentityAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import UpdatePodIdentityAssociationRequestTypeDef


def get_value() -> UpdatePodIdentityAssociationRequestTypeDef:
    return {
        "clusterName": ...,
    }


# UpdatePodIdentityAssociationRequestTypeDef definition

class UpdatePodIdentityAssociationRequestTypeDef(TypedDict):
    clusterName: str,
    associationId: str,
    roleArn: NotRequired[str],
    clientRequestToken: NotRequired[str],
```

## AssociatedAccessPolicyTypeDef

```python
# AssociatedAccessPolicyTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import AssociatedAccessPolicyTypeDef


def get_value() -> AssociatedAccessPolicyTypeDef:
    return {
        "policyArn": ...,
    }


# AssociatedAccessPolicyTypeDef definition

class AssociatedAccessPolicyTypeDef(TypedDict):
    policyArn: NotRequired[str],
    accessScope: NotRequired[AccessScopeOutputTypeDef],  # (1)
    associatedAt: NotRequired[datetime],
    modifiedAt: NotRequired[datetime],
```

1. See [:material-code-braces: AccessScopeOutputTypeDef](./type_defs.md#accessscopeoutputtypedef) 
## AddonHealthTypeDef

```python
# AddonHealthTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import AddonHealthTypeDef


def get_value() -> AddonHealthTypeDef:
    return {
        "issues": ...,
    }


# AddonHealthTypeDef definition

class AddonHealthTypeDef(TypedDict):
    issues: NotRequired[List[AddonIssueTypeDef]],  # (1)
```

1. See [:material-code-braces: AddonIssueTypeDef](./type_defs.md#addonissuetypedef) 
## CreateAddonRequestTypeDef

```python
# CreateAddonRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import CreateAddonRequestTypeDef


def get_value() -> CreateAddonRequestTypeDef:
    return {
        "clusterName": ...,
    }


# CreateAddonRequestTypeDef definition

class CreateAddonRequestTypeDef(TypedDict):
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
## UpdateAddonRequestTypeDef

```python
# UpdateAddonRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import UpdateAddonRequestTypeDef


def get_value() -> UpdateAddonRequestTypeDef:
    return {
        "clusterName": ...,
    }


# UpdateAddonRequestTypeDef definition

class UpdateAddonRequestTypeDef(TypedDict):
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
# AddonVersionInfoTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import AddonVersionInfoTypeDef


def get_value() -> AddonVersionInfoTypeDef:
    return {
        "addonVersion": ...,
    }


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
# CreateAccessEntryResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import CreateAccessEntryResponseTypeDef


def get_value() -> CreateAccessEntryResponseTypeDef:
    return {
        "accessEntry": ...,
    }


# CreateAccessEntryResponseTypeDef definition

class CreateAccessEntryResponseTypeDef(TypedDict):
    accessEntry: AccessEntryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccessEntryTypeDef](./type_defs.md#accessentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAccessEntryResponseTypeDef

```python
# DescribeAccessEntryResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeAccessEntryResponseTypeDef


def get_value() -> DescribeAccessEntryResponseTypeDef:
    return {
        "accessEntry": ...,
    }


# DescribeAccessEntryResponseTypeDef definition

class DescribeAccessEntryResponseTypeDef(TypedDict):
    accessEntry: AccessEntryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccessEntryTypeDef](./type_defs.md#accessentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAddonConfigurationResponseTypeDef

```python
# DescribeAddonConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeAddonConfigurationResponseTypeDef


def get_value() -> DescribeAddonConfigurationResponseTypeDef:
    return {
        "addonName": ...,
    }


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
# ListAccessEntriesResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListAccessEntriesResponseTypeDef


def get_value() -> ListAccessEntriesResponseTypeDef:
    return {
        "accessEntries": ...,
    }


# ListAccessEntriesResponseTypeDef definition

class ListAccessEntriesResponseTypeDef(TypedDict):
    accessEntries: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccessPoliciesResponseTypeDef

```python
# ListAccessPoliciesResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListAccessPoliciesResponseTypeDef


def get_value() -> ListAccessPoliciesResponseTypeDef:
    return {
        "accessPolicies": ...,
    }


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
# ListAddonsResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListAddonsResponseTypeDef


def get_value() -> ListAddonsResponseTypeDef:
    return {
        "addons": ...,
    }


# ListAddonsResponseTypeDef definition

class ListAddonsResponseTypeDef(TypedDict):
    addons: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListClustersResponseTypeDef

```python
# ListClustersResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListClustersResponseTypeDef


def get_value() -> ListClustersResponseTypeDef:
    return {
        "clusters": ...,
    }


# ListClustersResponseTypeDef definition

class ListClustersResponseTypeDef(TypedDict):
    clusters: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFargateProfilesResponseTypeDef

```python
# ListFargateProfilesResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListFargateProfilesResponseTypeDef


def get_value() -> ListFargateProfilesResponseTypeDef:
    return {
        "fargateProfileNames": ...,
    }


# ListFargateProfilesResponseTypeDef definition

class ListFargateProfilesResponseTypeDef(TypedDict):
    fargateProfileNames: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListNodegroupsResponseTypeDef

```python
# ListNodegroupsResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListNodegroupsResponseTypeDef


def get_value() -> ListNodegroupsResponseTypeDef:
    return {
        "nodegroups": ...,
    }


# ListNodegroupsResponseTypeDef definition

class ListNodegroupsResponseTypeDef(TypedDict):
    nodegroups: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUpdatesResponseTypeDef

```python
# ListUpdatesResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListUpdatesResponseTypeDef


def get_value() -> ListUpdatesResponseTypeDef:
    return {
        "updateIds": ...,
    }


# ListUpdatesResponseTypeDef definition

class ListUpdatesResponseTypeDef(TypedDict):
    updateIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAccessEntryResponseTypeDef

```python
# UpdateAccessEntryResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import UpdateAccessEntryResponseTypeDef


def get_value() -> UpdateAccessEntryResponseTypeDef:
    return {
        "accessEntry": ...,
    }


# UpdateAccessEntryResponseTypeDef definition

class UpdateAccessEntryResponseTypeDef(TypedDict):
    accessEntry: AccessEntryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccessEntryTypeDef](./type_defs.md#accessentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateIdentityProviderConfigRequestTypeDef

```python
# AssociateIdentityProviderConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import AssociateIdentityProviderConfigRequestTypeDef


def get_value() -> AssociateIdentityProviderConfigRequestTypeDef:
    return {
        "clusterName": ...,
    }


# AssociateIdentityProviderConfigRequestTypeDef definition

class AssociateIdentityProviderConfigRequestTypeDef(TypedDict):
    clusterName: str,
    oidc: OidcIdentityProviderConfigRequestTypeDef,  # (1)
    tags: NotRequired[Mapping[str, str]],
    clientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: OidcIdentityProviderConfigRequestTypeDef](./type_defs.md#oidcidentityproviderconfigrequesttypedef) 
## NodegroupResourcesTypeDef

```python
# NodegroupResourcesTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import NodegroupResourcesTypeDef


def get_value() -> NodegroupResourcesTypeDef:
    return {
        "autoScalingGroups": ...,
    }


# NodegroupResourcesTypeDef definition

class NodegroupResourcesTypeDef(TypedDict):
    autoScalingGroups: NotRequired[List[AutoScalingGroupTypeDef]],  # (1)
    remoteAccessSecurityGroup: NotRequired[str],
```

1. See [:material-code-braces: AutoScalingGroupTypeDef](./type_defs.md#autoscalinggrouptypedef) 
## StorageConfigRequestTypeDef

```python
# StorageConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import StorageConfigRequestTypeDef


def get_value() -> StorageConfigRequestTypeDef:
    return {
        "blockStorage": ...,
    }


# StorageConfigRequestTypeDef definition

class StorageConfigRequestTypeDef(TypedDict):
    blockStorage: NotRequired[BlockStorageTypeDef],  # (1)
```

1. See [:material-code-braces: BlockStorageTypeDef](./type_defs.md#blockstoragetypedef) 
## StorageConfigResponseTypeDef

```python
# StorageConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import StorageConfigResponseTypeDef


def get_value() -> StorageConfigResponseTypeDef:
    return {
        "blockStorage": ...,
    }


# StorageConfigResponseTypeDef definition

class StorageConfigResponseTypeDef(TypedDict):
    blockStorage: NotRequired[BlockStorageTypeDef],  # (1)
```

1. See [:material-code-braces: BlockStorageTypeDef](./type_defs.md#blockstoragetypedef) 
## DeprecationDetailTypeDef

```python
# DeprecationDetailTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DeprecationDetailTypeDef


def get_value() -> DeprecationDetailTypeDef:
    return {
        "usage": ...,
    }


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
# ClusterHealthTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ClusterHealthTypeDef


def get_value() -> ClusterHealthTypeDef:
    return {
        "issues": ...,
    }


# ClusterHealthTypeDef definition

class ClusterHealthTypeDef(TypedDict):
    issues: NotRequired[List[ClusterIssueTypeDef]],  # (1)
```

1. See [:material-code-braces: ClusterIssueTypeDef](./type_defs.md#clusterissuetypedef) 
## DescribeClusterVersionsResponseTypeDef

```python
# DescribeClusterVersionsResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeClusterVersionsResponseTypeDef


def get_value() -> DescribeClusterVersionsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# DescribeClusterVersionsResponseTypeDef definition

class DescribeClusterVersionsResponseTypeDef(TypedDict):
    clusterVersions: List[ClusterVersionInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ClusterVersionInformationTypeDef](./type_defs.md#clusterversioninformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterClusterRequestTypeDef

```python
# RegisterClusterRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import RegisterClusterRequestTypeDef


def get_value() -> RegisterClusterRequestTypeDef:
    return {
        "name": ...,
    }


# RegisterClusterRequestTypeDef definition

class RegisterClusterRequestTypeDef(TypedDict):
    name: str,
    connectorConfig: ConnectorConfigRequestTypeDef,  # (1)
    clientRequestToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ConnectorConfigRequestTypeDef](./type_defs.md#connectorconfigrequesttypedef) 
## OutpostConfigRequestTypeDef

```python
# OutpostConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import OutpostConfigRequestTypeDef


def get_value() -> OutpostConfigRequestTypeDef:
    return {
        "outpostArns": ...,
    }


# OutpostConfigRequestTypeDef definition

class OutpostConfigRequestTypeDef(TypedDict):
    outpostArns: Sequence[str],
    controlPlaneInstanceType: str,
    controlPlanePlacement: NotRequired[ControlPlanePlacementRequestTypeDef],  # (1)
```

1. See [:material-code-braces: ControlPlanePlacementRequestTypeDef](./type_defs.md#controlplaneplacementrequesttypedef) 
## OutpostConfigResponseTypeDef

```python
# OutpostConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import OutpostConfigResponseTypeDef


def get_value() -> OutpostConfigResponseTypeDef:
    return {
        "outpostArns": ...,
    }


# OutpostConfigResponseTypeDef definition

class OutpostConfigResponseTypeDef(TypedDict):
    outpostArns: List[str],
    controlPlaneInstanceType: str,
    controlPlanePlacement: NotRequired[ControlPlanePlacementResponseTypeDef],  # (1)
```

1. See [:material-code-braces: ControlPlanePlacementResponseTypeDef](./type_defs.md#controlplaneplacementresponsetypedef) 
## CreateEksAnywhereSubscriptionRequestTypeDef

```python
# CreateEksAnywhereSubscriptionRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import CreateEksAnywhereSubscriptionRequestTypeDef


def get_value() -> CreateEksAnywhereSubscriptionRequestTypeDef:
    return {
        "name": ...,
    }


# CreateEksAnywhereSubscriptionRequestTypeDef definition

class CreateEksAnywhereSubscriptionRequestTypeDef(TypedDict):
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
# EksAnywhereSubscriptionTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import EksAnywhereSubscriptionTypeDef


def get_value() -> EksAnywhereSubscriptionTypeDef:
    return {
        "id": ...,
    }


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
## UpdateNodegroupVersionRequestTypeDef

```python
# UpdateNodegroupVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import UpdateNodegroupVersionRequestTypeDef


def get_value() -> UpdateNodegroupVersionRequestTypeDef:
    return {
        "clusterName": ...,
    }


# UpdateNodegroupVersionRequestTypeDef definition

class UpdateNodegroupVersionRequestTypeDef(TypedDict):
    clusterName: str,
    nodegroupName: str,
    version: NotRequired[str],
    releaseVersion: NotRequired[str],
    launchTemplate: NotRequired[LaunchTemplateSpecificationTypeDef],  # (1)
    force: NotRequired[bool],
    clientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: LaunchTemplateSpecificationTypeDef](./type_defs.md#launchtemplatespecificationtypedef) 
## UpdateTaintsPayloadTypeDef

```python
# UpdateTaintsPayloadTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import UpdateTaintsPayloadTypeDef


def get_value() -> UpdateTaintsPayloadTypeDef:
    return {
        "addOrUpdateTaints": ...,
    }


# UpdateTaintsPayloadTypeDef definition

class UpdateTaintsPayloadTypeDef(TypedDict):
    addOrUpdateTaints: NotRequired[Sequence[TaintTypeDef]],  # (1)
    removeTaints: NotRequired[Sequence[TaintTypeDef]],  # (1)
```

1. See [:material-code-braces: TaintTypeDef](./type_defs.md#tainttypedef) 
2. See [:material-code-braces: TaintTypeDef](./type_defs.md#tainttypedef) 
## CreatePodIdentityAssociationResponseTypeDef

```python
# CreatePodIdentityAssociationResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import CreatePodIdentityAssociationResponseTypeDef


def get_value() -> CreatePodIdentityAssociationResponseTypeDef:
    return {
        "association": ...,
    }


# CreatePodIdentityAssociationResponseTypeDef definition

class CreatePodIdentityAssociationResponseTypeDef(TypedDict):
    association: PodIdentityAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PodIdentityAssociationTypeDef](./type_defs.md#podidentityassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeletePodIdentityAssociationResponseTypeDef

```python
# DeletePodIdentityAssociationResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DeletePodIdentityAssociationResponseTypeDef


def get_value() -> DeletePodIdentityAssociationResponseTypeDef:
    return {
        "association": ...,
    }


# DeletePodIdentityAssociationResponseTypeDef definition

class DeletePodIdentityAssociationResponseTypeDef(TypedDict):
    association: PodIdentityAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PodIdentityAssociationTypeDef](./type_defs.md#podidentityassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePodIdentityAssociationResponseTypeDef

```python
# DescribePodIdentityAssociationResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribePodIdentityAssociationResponseTypeDef


def get_value() -> DescribePodIdentityAssociationResponseTypeDef:
    return {
        "association": ...,
    }


# DescribePodIdentityAssociationResponseTypeDef definition

class DescribePodIdentityAssociationResponseTypeDef(TypedDict):
    association: PodIdentityAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PodIdentityAssociationTypeDef](./type_defs.md#podidentityassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePodIdentityAssociationResponseTypeDef

```python
# UpdatePodIdentityAssociationResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import UpdatePodIdentityAssociationResponseTypeDef


def get_value() -> UpdatePodIdentityAssociationResponseTypeDef:
    return {
        "association": ...,
    }


# UpdatePodIdentityAssociationResponseTypeDef definition

class UpdatePodIdentityAssociationResponseTypeDef(TypedDict):
    association: PodIdentityAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PodIdentityAssociationTypeDef](./type_defs.md#podidentityassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAddonRequestWaitExtraTypeDef

```python
# DescribeAddonRequestWaitExtraTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeAddonRequestWaitExtraTypeDef


def get_value() -> DescribeAddonRequestWaitExtraTypeDef:
    return {
        "clusterName": ...,
    }


# DescribeAddonRequestWaitExtraTypeDef definition

class DescribeAddonRequestWaitExtraTypeDef(TypedDict):
    clusterName: str,
    addonName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeAddonRequestWaitTypeDef

```python
# DescribeAddonRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeAddonRequestWaitTypeDef


def get_value() -> DescribeAddonRequestWaitTypeDef:
    return {
        "clusterName": ...,
    }


# DescribeAddonRequestWaitTypeDef definition

class DescribeAddonRequestWaitTypeDef(TypedDict):
    clusterName: str,
    addonName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeClusterRequestWaitExtraTypeDef

```python
# DescribeClusterRequestWaitExtraTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeClusterRequestWaitExtraTypeDef


def get_value() -> DescribeClusterRequestWaitExtraTypeDef:
    return {
        "name": ...,
    }


# DescribeClusterRequestWaitExtraTypeDef definition

class DescribeClusterRequestWaitExtraTypeDef(TypedDict):
    name: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeClusterRequestWaitTypeDef

```python
# DescribeClusterRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeClusterRequestWaitTypeDef


def get_value() -> DescribeClusterRequestWaitTypeDef:
    return {
        "name": ...,
    }


# DescribeClusterRequestWaitTypeDef definition

class DescribeClusterRequestWaitTypeDef(TypedDict):
    name: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeFargateProfileRequestWaitExtraTypeDef

```python
# DescribeFargateProfileRequestWaitExtraTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeFargateProfileRequestWaitExtraTypeDef


def get_value() -> DescribeFargateProfileRequestWaitExtraTypeDef:
    return {
        "clusterName": ...,
    }


# DescribeFargateProfileRequestWaitExtraTypeDef definition

class DescribeFargateProfileRequestWaitExtraTypeDef(TypedDict):
    clusterName: str,
    fargateProfileName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeFargateProfileRequestWaitTypeDef

```python
# DescribeFargateProfileRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeFargateProfileRequestWaitTypeDef


def get_value() -> DescribeFargateProfileRequestWaitTypeDef:
    return {
        "clusterName": ...,
    }


# DescribeFargateProfileRequestWaitTypeDef definition

class DescribeFargateProfileRequestWaitTypeDef(TypedDict):
    clusterName: str,
    fargateProfileName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeNodegroupRequestWaitExtraTypeDef

```python
# DescribeNodegroupRequestWaitExtraTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeNodegroupRequestWaitExtraTypeDef


def get_value() -> DescribeNodegroupRequestWaitExtraTypeDef:
    return {
        "clusterName": ...,
    }


# DescribeNodegroupRequestWaitExtraTypeDef definition

class DescribeNodegroupRequestWaitExtraTypeDef(TypedDict):
    clusterName: str,
    nodegroupName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeNodegroupRequestWaitTypeDef

```python
# DescribeNodegroupRequestWaitTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeNodegroupRequestWaitTypeDef


def get_value() -> DescribeNodegroupRequestWaitTypeDef:
    return {
        "clusterName": ...,
    }


# DescribeNodegroupRequestWaitTypeDef definition

class DescribeNodegroupRequestWaitTypeDef(TypedDict):
    clusterName: str,
    nodegroupName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeAddonVersionsRequestPaginateTypeDef

```python
# DescribeAddonVersionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeAddonVersionsRequestPaginateTypeDef


def get_value() -> DescribeAddonVersionsRequestPaginateTypeDef:
    return {
        "kubernetesVersion": ...,
    }


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
# DescribeClusterVersionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeClusterVersionsRequestPaginateTypeDef


def get_value() -> DescribeClusterVersionsRequestPaginateTypeDef:
    return {
        "clusterType": ...,
    }


# DescribeClusterVersionsRequestPaginateTypeDef definition

class DescribeClusterVersionsRequestPaginateTypeDef(TypedDict):
    clusterType: NotRequired[str],
    defaultOnly: NotRequired[bool],
    includeAll: NotRequired[bool],
    clusterVersions: NotRequired[Sequence[str]],
    status: NotRequired[ClusterVersionStatusType],  # (1)
    versionStatus: NotRequired[VersionStatusType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ClusterVersionStatusType](./literals.md#clusterversionstatustype) 
2. See [:material-code-brackets: VersionStatusType](./literals.md#versionstatustype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAccessEntriesRequestPaginateTypeDef

```python
# ListAccessEntriesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListAccessEntriesRequestPaginateTypeDef


def get_value() -> ListAccessEntriesRequestPaginateTypeDef:
    return {
        "clusterName": ...,
    }


# ListAccessEntriesRequestPaginateTypeDef definition

class ListAccessEntriesRequestPaginateTypeDef(TypedDict):
    clusterName: str,
    associatedPolicyArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAccessPoliciesRequestPaginateTypeDef

```python
# ListAccessPoliciesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListAccessPoliciesRequestPaginateTypeDef


def get_value() -> ListAccessPoliciesRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListAccessPoliciesRequestPaginateTypeDef definition

class ListAccessPoliciesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAddonsRequestPaginateTypeDef

```python
# ListAddonsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListAddonsRequestPaginateTypeDef


def get_value() -> ListAddonsRequestPaginateTypeDef:
    return {
        "clusterName": ...,
    }


# ListAddonsRequestPaginateTypeDef definition

class ListAddonsRequestPaginateTypeDef(TypedDict):
    clusterName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssociatedAccessPoliciesRequestPaginateTypeDef

```python
# ListAssociatedAccessPoliciesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListAssociatedAccessPoliciesRequestPaginateTypeDef


def get_value() -> ListAssociatedAccessPoliciesRequestPaginateTypeDef:
    return {
        "clusterName": ...,
    }


# ListAssociatedAccessPoliciesRequestPaginateTypeDef definition

class ListAssociatedAccessPoliciesRequestPaginateTypeDef(TypedDict):
    clusterName: str,
    principalArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListClustersRequestPaginateTypeDef

```python
# ListClustersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListClustersRequestPaginateTypeDef


def get_value() -> ListClustersRequestPaginateTypeDef:
    return {
        "include": ...,
    }


# ListClustersRequestPaginateTypeDef definition

class ListClustersRequestPaginateTypeDef(TypedDict):
    include: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEksAnywhereSubscriptionsRequestPaginateTypeDef

```python
# ListEksAnywhereSubscriptionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListEksAnywhereSubscriptionsRequestPaginateTypeDef


def get_value() -> ListEksAnywhereSubscriptionsRequestPaginateTypeDef:
    return {
        "includeStatus": ...,
    }


# ListEksAnywhereSubscriptionsRequestPaginateTypeDef definition

class ListEksAnywhereSubscriptionsRequestPaginateTypeDef(TypedDict):
    includeStatus: NotRequired[Sequence[EksAnywhereSubscriptionStatusType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: EksAnywhereSubscriptionStatusType](./literals.md#eksanywheresubscriptionstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFargateProfilesRequestPaginateTypeDef

```python
# ListFargateProfilesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListFargateProfilesRequestPaginateTypeDef


def get_value() -> ListFargateProfilesRequestPaginateTypeDef:
    return {
        "clusterName": ...,
    }


# ListFargateProfilesRequestPaginateTypeDef definition

class ListFargateProfilesRequestPaginateTypeDef(TypedDict):
    clusterName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIdentityProviderConfigsRequestPaginateTypeDef

```python
# ListIdentityProviderConfigsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListIdentityProviderConfigsRequestPaginateTypeDef


def get_value() -> ListIdentityProviderConfigsRequestPaginateTypeDef:
    return {
        "clusterName": ...,
    }


# ListIdentityProviderConfigsRequestPaginateTypeDef definition

class ListIdentityProviderConfigsRequestPaginateTypeDef(TypedDict):
    clusterName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNodegroupsRequestPaginateTypeDef

```python
# ListNodegroupsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListNodegroupsRequestPaginateTypeDef


def get_value() -> ListNodegroupsRequestPaginateTypeDef:
    return {
        "clusterName": ...,
    }


# ListNodegroupsRequestPaginateTypeDef definition

class ListNodegroupsRequestPaginateTypeDef(TypedDict):
    clusterName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPodIdentityAssociationsRequestPaginateTypeDef

```python
# ListPodIdentityAssociationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListPodIdentityAssociationsRequestPaginateTypeDef


def get_value() -> ListPodIdentityAssociationsRequestPaginateTypeDef:
    return {
        "clusterName": ...,
    }


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
# ListUpdatesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListUpdatesRequestPaginateTypeDef


def get_value() -> ListUpdatesRequestPaginateTypeDef:
    return {
        "name": ...,
    }


# ListUpdatesRequestPaginateTypeDef definition

class ListUpdatesRequestPaginateTypeDef(TypedDict):
    name: str,
    nodegroupName: NotRequired[str],
    addonName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeIdentityProviderConfigRequestTypeDef

```python
# DescribeIdentityProviderConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeIdentityProviderConfigRequestTypeDef


def get_value() -> DescribeIdentityProviderConfigRequestTypeDef:
    return {
        "clusterName": ...,
    }


# DescribeIdentityProviderConfigRequestTypeDef definition

class DescribeIdentityProviderConfigRequestTypeDef(TypedDict):
    clusterName: str,
    identityProviderConfig: IdentityProviderConfigTypeDef,  # (1)
```

1. See [:material-code-braces: IdentityProviderConfigTypeDef](./type_defs.md#identityproviderconfigtypedef) 
## DisassociateIdentityProviderConfigRequestTypeDef

```python
# DisassociateIdentityProviderConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DisassociateIdentityProviderConfigRequestTypeDef


def get_value() -> DisassociateIdentityProviderConfigRequestTypeDef:
    return {
        "clusterName": ...,
    }


# DisassociateIdentityProviderConfigRequestTypeDef definition

class DisassociateIdentityProviderConfigRequestTypeDef(TypedDict):
    clusterName: str,
    identityProviderConfig: IdentityProviderConfigTypeDef,  # (1)
    clientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: IdentityProviderConfigTypeDef](./type_defs.md#identityproviderconfigtypedef) 
## ListIdentityProviderConfigsResponseTypeDef

```python
# ListIdentityProviderConfigsResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListIdentityProviderConfigsResponseTypeDef


def get_value() -> ListIdentityProviderConfigsResponseTypeDef:
    return {
        "identityProviderConfigs": ...,
    }


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
# KubernetesNetworkConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import KubernetesNetworkConfigRequestTypeDef


def get_value() -> KubernetesNetworkConfigRequestTypeDef:
    return {
        "serviceIpv4Cidr": ...,
    }


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
# KubernetesNetworkConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import KubernetesNetworkConfigResponseTypeDef


def get_value() -> KubernetesNetworkConfigResponseTypeDef:
    return {
        "serviceIpv4Cidr": ...,
    }


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
# EncryptionConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import EncryptionConfigOutputTypeDef


def get_value() -> EncryptionConfigOutputTypeDef:
    return {
        "resources": ...,
    }


# EncryptionConfigOutputTypeDef definition

class EncryptionConfigOutputTypeDef(TypedDict):
    resources: NotRequired[List[str]],
    provider: NotRequired[ProviderTypeDef],  # (1)
```

1. See [:material-code-braces: ProviderTypeDef](./type_defs.md#providertypedef) 
## EncryptionConfigTypeDef

```python
# EncryptionConfigTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import EncryptionConfigTypeDef


def get_value() -> EncryptionConfigTypeDef:
    return {
        "resources": ...,
    }


# EncryptionConfigTypeDef definition

class EncryptionConfigTypeDef(TypedDict):
    resources: NotRequired[Sequence[str]],
    provider: NotRequired[ProviderTypeDef],  # (1)
```

1. See [:material-code-braces: ProviderTypeDef](./type_defs.md#providertypedef) 
## FargateProfileHealthTypeDef

```python
# FargateProfileHealthTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import FargateProfileHealthTypeDef


def get_value() -> FargateProfileHealthTypeDef:
    return {
        "issues": ...,
    }


# FargateProfileHealthTypeDef definition

class FargateProfileHealthTypeDef(TypedDict):
    issues: NotRequired[List[FargateProfileIssueTypeDef]],  # (1)
```

1. See [:material-code-braces: FargateProfileIssueTypeDef](./type_defs.md#fargateprofileissuetypedef) 
## IdentityProviderConfigResponseTypeDef

```python
# IdentityProviderConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import IdentityProviderConfigResponseTypeDef


def get_value() -> IdentityProviderConfigResponseTypeDef:
    return {
        "oidc": ...,
    }


# IdentityProviderConfigResponseTypeDef definition

class IdentityProviderConfigResponseTypeDef(TypedDict):
    oidc: NotRequired[OidcIdentityProviderConfigTypeDef],  # (1)
```

1. See [:material-code-braces: OidcIdentityProviderConfigTypeDef](./type_defs.md#oidcidentityproviderconfigtypedef) 
## IdentityTypeDef

```python
# IdentityTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import IdentityTypeDef


def get_value() -> IdentityTypeDef:
    return {
        "oidc": ...,
    }


# IdentityTypeDef definition

class IdentityTypeDef(TypedDict):
    oidc: NotRequired[OIDCTypeDef],  # (1)
```

1. See [:material-code-braces: OIDCTypeDef](./type_defs.md#oidctypedef) 
## InsightResourceDetailTypeDef

```python
# InsightResourceDetailTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import InsightResourceDetailTypeDef


def get_value() -> InsightResourceDetailTypeDef:
    return {
        "insightStatus": ...,
    }


# InsightResourceDetailTypeDef definition

class InsightResourceDetailTypeDef(TypedDict):
    insightStatus: NotRequired[InsightStatusTypeDef],  # (1)
    kubernetesResourceUri: NotRequired[str],
    arn: NotRequired[str],
```

1. See [:material-code-braces: InsightStatusTypeDef](./type_defs.md#insightstatustypedef) 
## InsightSummaryTypeDef

```python
# InsightSummaryTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import InsightSummaryTypeDef


def get_value() -> InsightSummaryTypeDef:
    return {
        "id": ...,
    }


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
# ListInsightsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListInsightsRequestPaginateTypeDef


def get_value() -> ListInsightsRequestPaginateTypeDef:
    return {
        "clusterName": ...,
    }


# ListInsightsRequestPaginateTypeDef definition

class ListInsightsRequestPaginateTypeDef(TypedDict):
    clusterName: str,
    filter: NotRequired[InsightsFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: InsightsFilterTypeDef](./type_defs.md#insightsfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInsightsRequestTypeDef

```python
# ListInsightsRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListInsightsRequestTypeDef


def get_value() -> ListInsightsRequestTypeDef:
    return {
        "clusterName": ...,
    }


# ListInsightsRequestTypeDef definition

class ListInsightsRequestTypeDef(TypedDict):
    clusterName: str,
    filter: NotRequired[InsightsFilterTypeDef],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: InsightsFilterTypeDef](./type_defs.md#insightsfiltertypedef) 
## NodegroupHealthTypeDef

```python
# NodegroupHealthTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import NodegroupHealthTypeDef


def get_value() -> NodegroupHealthTypeDef:
    return {
        "issues": ...,
    }


# NodegroupHealthTypeDef definition

class NodegroupHealthTypeDef(TypedDict):
    issues: NotRequired[List[IssueTypeDef]],  # (1)
```

1. See [:material-code-braces: IssueTypeDef](./type_defs.md#issuetypedef) 
## ListPodIdentityAssociationsResponseTypeDef

```python
# ListPodIdentityAssociationsResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListPodIdentityAssociationsResponseTypeDef


def get_value() -> ListPodIdentityAssociationsResponseTypeDef:
    return {
        "associations": ...,
    }


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
# LoggingOutputTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import LoggingOutputTypeDef


def get_value() -> LoggingOutputTypeDef:
    return {
        "clusterLogging": ...,
    }


# LoggingOutputTypeDef definition

class LoggingOutputTypeDef(TypedDict):
    clusterLogging: NotRequired[List[LogSetupOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: LogSetupOutputTypeDef](./type_defs.md#logsetupoutputtypedef) 
## LoggingTypeDef

```python
# LoggingTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import LoggingTypeDef


def get_value() -> LoggingTypeDef:
    return {
        "clusterLogging": ...,
    }


# LoggingTypeDef definition

class LoggingTypeDef(TypedDict):
    clusterLogging: NotRequired[Sequence[LogSetupTypeDef]],  # (1)
```

1. See [:material-code-braces: LogSetupTypeDef](./type_defs.md#logsetuptypedef) 
## RemoteNetworkConfigResponseTypeDef

```python
# RemoteNetworkConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import RemoteNetworkConfigResponseTypeDef


def get_value() -> RemoteNetworkConfigResponseTypeDef:
    return {
        "remoteNodeNetworks": ...,
    }


# RemoteNetworkConfigResponseTypeDef definition

class RemoteNetworkConfigResponseTypeDef(TypedDict):
    remoteNodeNetworks: NotRequired[List[RemoteNodeNetworkOutputTypeDef]],  # (1)
    remotePodNetworks: NotRequired[List[RemotePodNetworkOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: RemoteNodeNetworkOutputTypeDef](./type_defs.md#remotenodenetworkoutputtypedef) 
2. See [:material-code-braces: RemotePodNetworkOutputTypeDef](./type_defs.md#remotepodnetworkoutputtypedef) 
## UpdateTypeDef

```python
# UpdateTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import UpdateTypeDef


def get_value() -> UpdateTypeDef:
    return {
        "id": ...,
    }


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
# AssociateAccessPolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import AssociateAccessPolicyResponseTypeDef


def get_value() -> AssociateAccessPolicyResponseTypeDef:
    return {
        "clusterName": ...,
    }


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
# ListAssociatedAccessPoliciesResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListAssociatedAccessPoliciesResponseTypeDef


def get_value() -> ListAssociatedAccessPoliciesResponseTypeDef:
    return {
        "clusterName": ...,
    }


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
## AssociateAccessPolicyRequestTypeDef

```python
# AssociateAccessPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import AssociateAccessPolicyRequestTypeDef


def get_value() -> AssociateAccessPolicyRequestTypeDef:
    return {
        "clusterName": ...,
    }


# AssociateAccessPolicyRequestTypeDef definition

class AssociateAccessPolicyRequestTypeDef(TypedDict):
    clusterName: str,
    principalArn: str,
    policyArn: str,
    accessScope: AccessScopeUnionTypeDef,  # (1)
```

1. See [:material-code-braces: AccessScopeTypeDef](./type_defs.md#accessscopetypedef) [:material-code-braces: AccessScopeOutputTypeDef](./type_defs.md#accessscopeoutputtypedef) 
## AddonTypeDef

```python
# AddonTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import AddonTypeDef


def get_value() -> AddonTypeDef:
    return {
        "addonName": ...,
    }


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
# AddonInfoTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import AddonInfoTypeDef


def get_value() -> AddonInfoTypeDef:
    return {
        "addonName": ...,
    }


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
# InsightCategorySpecificSummaryTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import InsightCategorySpecificSummaryTypeDef


def get_value() -> InsightCategorySpecificSummaryTypeDef:
    return {
        "deprecationDetails": ...,
    }


# InsightCategorySpecificSummaryTypeDef definition

class InsightCategorySpecificSummaryTypeDef(TypedDict):
    deprecationDetails: NotRequired[List[DeprecationDetailTypeDef]],  # (1)
    addonCompatibilityDetails: NotRequired[List[AddonCompatibilityDetailTypeDef]],  # (2)
```

1. See [:material-code-braces: DeprecationDetailTypeDef](./type_defs.md#deprecationdetailtypedef) 
2. See [:material-code-braces: AddonCompatibilityDetailTypeDef](./type_defs.md#addoncompatibilitydetailtypedef) 
## CreateEksAnywhereSubscriptionResponseTypeDef

```python
# CreateEksAnywhereSubscriptionResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import CreateEksAnywhereSubscriptionResponseTypeDef


def get_value() -> CreateEksAnywhereSubscriptionResponseTypeDef:
    return {
        "subscription": ...,
    }


# CreateEksAnywhereSubscriptionResponseTypeDef definition

class CreateEksAnywhereSubscriptionResponseTypeDef(TypedDict):
    subscription: EksAnywhereSubscriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EksAnywhereSubscriptionTypeDef](./type_defs.md#eksanywheresubscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteEksAnywhereSubscriptionResponseTypeDef

```python
# DeleteEksAnywhereSubscriptionResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DeleteEksAnywhereSubscriptionResponseTypeDef


def get_value() -> DeleteEksAnywhereSubscriptionResponseTypeDef:
    return {
        "subscription": ...,
    }


# DeleteEksAnywhereSubscriptionResponseTypeDef definition

class DeleteEksAnywhereSubscriptionResponseTypeDef(TypedDict):
    subscription: EksAnywhereSubscriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EksAnywhereSubscriptionTypeDef](./type_defs.md#eksanywheresubscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEksAnywhereSubscriptionResponseTypeDef

```python
# DescribeEksAnywhereSubscriptionResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeEksAnywhereSubscriptionResponseTypeDef


def get_value() -> DescribeEksAnywhereSubscriptionResponseTypeDef:
    return {
        "subscription": ...,
    }


# DescribeEksAnywhereSubscriptionResponseTypeDef definition

class DescribeEksAnywhereSubscriptionResponseTypeDef(TypedDict):
    subscription: EksAnywhereSubscriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EksAnywhereSubscriptionTypeDef](./type_defs.md#eksanywheresubscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEksAnywhereSubscriptionsResponseTypeDef

```python
# ListEksAnywhereSubscriptionsResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListEksAnywhereSubscriptionsResponseTypeDef


def get_value() -> ListEksAnywhereSubscriptionsResponseTypeDef:
    return {
        "subscriptions": ...,
    }


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
# UpdateEksAnywhereSubscriptionResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import UpdateEksAnywhereSubscriptionResponseTypeDef


def get_value() -> UpdateEksAnywhereSubscriptionResponseTypeDef:
    return {
        "subscription": ...,
    }


# UpdateEksAnywhereSubscriptionResponseTypeDef definition

class UpdateEksAnywhereSubscriptionResponseTypeDef(TypedDict):
    subscription: EksAnywhereSubscriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EksAnywhereSubscriptionTypeDef](./type_defs.md#eksanywheresubscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateNodegroupConfigRequestTypeDef

```python
# UpdateNodegroupConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import UpdateNodegroupConfigRequestTypeDef


def get_value() -> UpdateNodegroupConfigRequestTypeDef:
    return {
        "clusterName": ...,
    }


# UpdateNodegroupConfigRequestTypeDef definition

class UpdateNodegroupConfigRequestTypeDef(TypedDict):
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
# FargateProfileTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import FargateProfileTypeDef


def get_value() -> FargateProfileTypeDef:
    return {
        "fargateProfileName": ...,
    }


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
## CreateFargateProfileRequestTypeDef

```python
# CreateFargateProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import CreateFargateProfileRequestTypeDef


def get_value() -> CreateFargateProfileRequestTypeDef:
    return {
        "fargateProfileName": ...,
    }


# CreateFargateProfileRequestTypeDef definition

class CreateFargateProfileRequestTypeDef(TypedDict):
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
# DescribeIdentityProviderConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeIdentityProviderConfigResponseTypeDef


def get_value() -> DescribeIdentityProviderConfigResponseTypeDef:
    return {
        "identityProviderConfig": ...,
    }


# DescribeIdentityProviderConfigResponseTypeDef definition

class DescribeIdentityProviderConfigResponseTypeDef(TypedDict):
    identityProviderConfig: IdentityProviderConfigResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IdentityProviderConfigResponseTypeDef](./type_defs.md#identityproviderconfigresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInsightsResponseTypeDef

```python
# ListInsightsResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ListInsightsResponseTypeDef


def get_value() -> ListInsightsResponseTypeDef:
    return {
        "insights": ...,
    }


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
# NodegroupTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import NodegroupTypeDef


def get_value() -> NodegroupTypeDef:
    return {
        "nodegroupName": ...,
    }


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
## CreateNodegroupRequestTypeDef

```python
# CreateNodegroupRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import CreateNodegroupRequestTypeDef


def get_value() -> CreateNodegroupRequestTypeDef:
    return {
        "clusterName": ...,
    }


# CreateNodegroupRequestTypeDef definition

class CreateNodegroupRequestTypeDef(TypedDict):
    clusterName: str,
    nodegroupName: str,
    subnets: Sequence[str],
    nodeRole: str,
    scalingConfig: NotRequired[NodegroupScalingConfigTypeDef],  # (1)
    diskSize: NotRequired[int],
    instanceTypes: NotRequired[Sequence[str]],
    amiType: NotRequired[AMITypesType],  # (2)
    remoteAccess: NotRequired[RemoteAccessConfigUnionTypeDef],  # (3)
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
3. See [:material-code-braces: RemoteAccessConfigTypeDef](./type_defs.md#remoteaccessconfigtypedef) [:material-code-braces: RemoteAccessConfigOutputTypeDef](./type_defs.md#remoteaccessconfigoutputtypedef) 
4. See [:material-code-braces: TaintTypeDef](./type_defs.md#tainttypedef) 
5. See [:material-code-braces: LaunchTemplateSpecificationTypeDef](./type_defs.md#launchtemplatespecificationtypedef) 
6. See [:material-code-braces: NodegroupUpdateConfigTypeDef](./type_defs.md#nodegroupupdateconfigtypedef) 
7. See [:material-code-braces: NodeRepairConfigTypeDef](./type_defs.md#noderepairconfigtypedef) 
8. See [:material-code-brackets: CapacityTypesType](./literals.md#capacitytypestype) 
## ClusterTypeDef

```python
# ClusterTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import ClusterTypeDef


def get_value() -> ClusterTypeDef:
    return {
        "name": ...,
    }


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
# RemoteNetworkConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import RemoteNetworkConfigRequestTypeDef


def get_value() -> RemoteNetworkConfigRequestTypeDef:
    return {
        "remoteNodeNetworks": ...,
    }


# RemoteNetworkConfigRequestTypeDef definition

class RemoteNetworkConfigRequestTypeDef(TypedDict):
    remoteNodeNetworks: NotRequired[Sequence[RemoteNodeNetworkUnionTypeDef]],  # (1)
    remotePodNetworks: NotRequired[Sequence[RemotePodNetworkUnionTypeDef]],  # (2)
```

1. See [:material-code-braces: RemoteNodeNetworkTypeDef](./type_defs.md#remotenodenetworktypedef) [:material-code-braces: RemoteNodeNetworkOutputTypeDef](./type_defs.md#remotenodenetworkoutputtypedef) 
2. See [:material-code-braces: RemotePodNetworkTypeDef](./type_defs.md#remotepodnetworktypedef) [:material-code-braces: RemotePodNetworkOutputTypeDef](./type_defs.md#remotepodnetworkoutputtypedef) 
## AssociateEncryptionConfigResponseTypeDef

```python
# AssociateEncryptionConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import AssociateEncryptionConfigResponseTypeDef


def get_value() -> AssociateEncryptionConfigResponseTypeDef:
    return {
        "update": ...,
    }


# AssociateEncryptionConfigResponseTypeDef definition

class AssociateEncryptionConfigResponseTypeDef(TypedDict):
    update: UpdateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UpdateTypeDef](./type_defs.md#updatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateIdentityProviderConfigResponseTypeDef

```python
# AssociateIdentityProviderConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import AssociateIdentityProviderConfigResponseTypeDef


def get_value() -> AssociateIdentityProviderConfigResponseTypeDef:
    return {
        "update": ...,
    }


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
# DescribeUpdateResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeUpdateResponseTypeDef


def get_value() -> DescribeUpdateResponseTypeDef:
    return {
        "update": ...,
    }


# DescribeUpdateResponseTypeDef definition

class DescribeUpdateResponseTypeDef(TypedDict):
    update: UpdateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UpdateTypeDef](./type_defs.md#updatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateIdentityProviderConfigResponseTypeDef

```python
# DisassociateIdentityProviderConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DisassociateIdentityProviderConfigResponseTypeDef


def get_value() -> DisassociateIdentityProviderConfigResponseTypeDef:
    return {
        "update": ...,
    }


# DisassociateIdentityProviderConfigResponseTypeDef definition

class DisassociateIdentityProviderConfigResponseTypeDef(TypedDict):
    update: UpdateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UpdateTypeDef](./type_defs.md#updatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAddonResponseTypeDef

```python
# UpdateAddonResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import UpdateAddonResponseTypeDef


def get_value() -> UpdateAddonResponseTypeDef:
    return {
        "update": ...,
    }


# UpdateAddonResponseTypeDef definition

class UpdateAddonResponseTypeDef(TypedDict):
    update: UpdateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UpdateTypeDef](./type_defs.md#updatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateClusterConfigResponseTypeDef

```python
# UpdateClusterConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import UpdateClusterConfigResponseTypeDef


def get_value() -> UpdateClusterConfigResponseTypeDef:
    return {
        "update": ...,
    }


# UpdateClusterConfigResponseTypeDef definition

class UpdateClusterConfigResponseTypeDef(TypedDict):
    update: UpdateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UpdateTypeDef](./type_defs.md#updatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateClusterVersionResponseTypeDef

```python
# UpdateClusterVersionResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import UpdateClusterVersionResponseTypeDef


def get_value() -> UpdateClusterVersionResponseTypeDef:
    return {
        "update": ...,
    }


# UpdateClusterVersionResponseTypeDef definition

class UpdateClusterVersionResponseTypeDef(TypedDict):
    update: UpdateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UpdateTypeDef](./type_defs.md#updatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateNodegroupConfigResponseTypeDef

```python
# UpdateNodegroupConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import UpdateNodegroupConfigResponseTypeDef


def get_value() -> UpdateNodegroupConfigResponseTypeDef:
    return {
        "update": ...,
    }


# UpdateNodegroupConfigResponseTypeDef definition

class UpdateNodegroupConfigResponseTypeDef(TypedDict):
    update: UpdateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UpdateTypeDef](./type_defs.md#updatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateNodegroupVersionResponseTypeDef

```python
# UpdateNodegroupVersionResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import UpdateNodegroupVersionResponseTypeDef


def get_value() -> UpdateNodegroupVersionResponseTypeDef:
    return {
        "update": ...,
    }


# UpdateNodegroupVersionResponseTypeDef definition

class UpdateNodegroupVersionResponseTypeDef(TypedDict):
    update: UpdateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UpdateTypeDef](./type_defs.md#updatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAddonResponseTypeDef

```python
# CreateAddonResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import CreateAddonResponseTypeDef


def get_value() -> CreateAddonResponseTypeDef:
    return {
        "addon": ...,
    }


# CreateAddonResponseTypeDef definition

class CreateAddonResponseTypeDef(TypedDict):
    addon: AddonTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AddonTypeDef](./type_defs.md#addontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAddonResponseTypeDef

```python
# DeleteAddonResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DeleteAddonResponseTypeDef


def get_value() -> DeleteAddonResponseTypeDef:
    return {
        "addon": ...,
    }


# DeleteAddonResponseTypeDef definition

class DeleteAddonResponseTypeDef(TypedDict):
    addon: AddonTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AddonTypeDef](./type_defs.md#addontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAddonResponseTypeDef

```python
# DescribeAddonResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeAddonResponseTypeDef


def get_value() -> DescribeAddonResponseTypeDef:
    return {
        "addon": ...,
    }


# DescribeAddonResponseTypeDef definition

class DescribeAddonResponseTypeDef(TypedDict):
    addon: AddonTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AddonTypeDef](./type_defs.md#addontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAddonVersionsResponseTypeDef

```python
# DescribeAddonVersionsResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeAddonVersionsResponseTypeDef


def get_value() -> DescribeAddonVersionsResponseTypeDef:
    return {
        "addons": ...,
    }


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
# InsightTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import InsightTypeDef


def get_value() -> InsightTypeDef:
    return {
        "id": ...,
    }


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
## AssociateEncryptionConfigRequestTypeDef

```python
# AssociateEncryptionConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import AssociateEncryptionConfigRequestTypeDef


def get_value() -> AssociateEncryptionConfigRequestTypeDef:
    return {
        "clusterName": ...,
    }


# AssociateEncryptionConfigRequestTypeDef definition

class AssociateEncryptionConfigRequestTypeDef(TypedDict):
    clusterName: str,
    encryptionConfig: Sequence[EncryptionConfigUnionTypeDef],  # (1)
    clientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef) [:material-code-braces: EncryptionConfigOutputTypeDef](./type_defs.md#encryptionconfigoutputtypedef) 
## CreateFargateProfileResponseTypeDef

```python
# CreateFargateProfileResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import CreateFargateProfileResponseTypeDef


def get_value() -> CreateFargateProfileResponseTypeDef:
    return {
        "fargateProfile": ...,
    }


# CreateFargateProfileResponseTypeDef definition

class CreateFargateProfileResponseTypeDef(TypedDict):
    fargateProfile: FargateProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FargateProfileTypeDef](./type_defs.md#fargateprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteFargateProfileResponseTypeDef

```python
# DeleteFargateProfileResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DeleteFargateProfileResponseTypeDef


def get_value() -> DeleteFargateProfileResponseTypeDef:
    return {
        "fargateProfile": ...,
    }


# DeleteFargateProfileResponseTypeDef definition

class DeleteFargateProfileResponseTypeDef(TypedDict):
    fargateProfile: FargateProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FargateProfileTypeDef](./type_defs.md#fargateprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeFargateProfileResponseTypeDef

```python
# DescribeFargateProfileResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeFargateProfileResponseTypeDef


def get_value() -> DescribeFargateProfileResponseTypeDef:
    return {
        "fargateProfile": ...,
    }


# DescribeFargateProfileResponseTypeDef definition

class DescribeFargateProfileResponseTypeDef(TypedDict):
    fargateProfile: FargateProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FargateProfileTypeDef](./type_defs.md#fargateprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateNodegroupResponseTypeDef

```python
# CreateNodegroupResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import CreateNodegroupResponseTypeDef


def get_value() -> CreateNodegroupResponseTypeDef:
    return {
        "nodegroup": ...,
    }


# CreateNodegroupResponseTypeDef definition

class CreateNodegroupResponseTypeDef(TypedDict):
    nodegroup: NodegroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NodegroupTypeDef](./type_defs.md#nodegrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteNodegroupResponseTypeDef

```python
# DeleteNodegroupResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DeleteNodegroupResponseTypeDef


def get_value() -> DeleteNodegroupResponseTypeDef:
    return {
        "nodegroup": ...,
    }


# DeleteNodegroupResponseTypeDef definition

class DeleteNodegroupResponseTypeDef(TypedDict):
    nodegroup: NodegroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NodegroupTypeDef](./type_defs.md#nodegrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeNodegroupResponseTypeDef

```python
# DescribeNodegroupResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeNodegroupResponseTypeDef


def get_value() -> DescribeNodegroupResponseTypeDef:
    return {
        "nodegroup": ...,
    }


# DescribeNodegroupResponseTypeDef definition

class DescribeNodegroupResponseTypeDef(TypedDict):
    nodegroup: NodegroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NodegroupTypeDef](./type_defs.md#nodegrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateClusterConfigRequestTypeDef

```python
# UpdateClusterConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import UpdateClusterConfigRequestTypeDef


def get_value() -> UpdateClusterConfigRequestTypeDef:
    return {
        "name": ...,
    }


# UpdateClusterConfigRequestTypeDef definition

class UpdateClusterConfigRequestTypeDef(TypedDict):
    name: str,
    resourcesVpcConfig: NotRequired[VpcConfigRequestTypeDef],  # (1)
    logging: NotRequired[LoggingUnionTypeDef],  # (2)
    clientRequestToken: NotRequired[str],
    accessConfig: NotRequired[UpdateAccessConfigRequestTypeDef],  # (3)
    upgradePolicy: NotRequired[UpgradePolicyRequestTypeDef],  # (4)
    zonalShiftConfig: NotRequired[ZonalShiftConfigRequestTypeDef],  # (5)
    computeConfig: NotRequired[ComputeConfigRequestTypeDef],  # (6)
    kubernetesNetworkConfig: NotRequired[KubernetesNetworkConfigRequestTypeDef],  # (7)
    storageConfig: NotRequired[StorageConfigRequestTypeDef],  # (8)
```

1. See [:material-code-braces: VpcConfigRequestTypeDef](./type_defs.md#vpcconfigrequesttypedef) 
2. See [:material-code-braces: LoggingTypeDef](./type_defs.md#loggingtypedef) [:material-code-braces: LoggingOutputTypeDef](./type_defs.md#loggingoutputtypedef) 
3. See [:material-code-braces: UpdateAccessConfigRequestTypeDef](./type_defs.md#updateaccessconfigrequesttypedef) 
4. See [:material-code-braces: UpgradePolicyRequestTypeDef](./type_defs.md#upgradepolicyrequesttypedef) 
5. See [:material-code-braces: ZonalShiftConfigRequestTypeDef](./type_defs.md#zonalshiftconfigrequesttypedef) 
6. See [:material-code-braces: ComputeConfigRequestTypeDef](./type_defs.md#computeconfigrequesttypedef) 
7. See [:material-code-braces: KubernetesNetworkConfigRequestTypeDef](./type_defs.md#kubernetesnetworkconfigrequesttypedef) 
8. See [:material-code-braces: StorageConfigRequestTypeDef](./type_defs.md#storageconfigrequesttypedef) 
## CreateClusterResponseTypeDef

```python
# CreateClusterResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import CreateClusterResponseTypeDef


def get_value() -> CreateClusterResponseTypeDef:
    return {
        "cluster": ...,
    }


# CreateClusterResponseTypeDef definition

class CreateClusterResponseTypeDef(TypedDict):
    cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteClusterResponseTypeDef

```python
# DeleteClusterResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DeleteClusterResponseTypeDef


def get_value() -> DeleteClusterResponseTypeDef:
    return {
        "cluster": ...,
    }


# DeleteClusterResponseTypeDef definition

class DeleteClusterResponseTypeDef(TypedDict):
    cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeregisterClusterResponseTypeDef

```python
# DeregisterClusterResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DeregisterClusterResponseTypeDef


def get_value() -> DeregisterClusterResponseTypeDef:
    return {
        "cluster": ...,
    }


# DeregisterClusterResponseTypeDef definition

class DeregisterClusterResponseTypeDef(TypedDict):
    cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeClusterResponseTypeDef

```python
# DescribeClusterResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeClusterResponseTypeDef


def get_value() -> DescribeClusterResponseTypeDef:
    return {
        "cluster": ...,
    }


# DescribeClusterResponseTypeDef definition

class DescribeClusterResponseTypeDef(TypedDict):
    cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterClusterResponseTypeDef

```python
# RegisterClusterResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import RegisterClusterResponseTypeDef


def get_value() -> RegisterClusterResponseTypeDef:
    return {
        "cluster": ...,
    }


# RegisterClusterResponseTypeDef definition

class RegisterClusterResponseTypeDef(TypedDict):
    cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateClusterRequestTypeDef

```python
# CreateClusterRequestTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import CreateClusterRequestTypeDef


def get_value() -> CreateClusterRequestTypeDef:
    return {
        "name": ...,
    }


# CreateClusterRequestTypeDef definition

class CreateClusterRequestTypeDef(TypedDict):
    name: str,
    roleArn: str,
    resourcesVpcConfig: VpcConfigRequestTypeDef,  # (1)
    version: NotRequired[str],
    kubernetesNetworkConfig: NotRequired[KubernetesNetworkConfigRequestTypeDef],  # (2)
    logging: NotRequired[LoggingUnionTypeDef],  # (3)
    clientRequestToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    encryptionConfig: NotRequired[Sequence[EncryptionConfigUnionTypeDef]],  # (4)
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
3. See [:material-code-braces: LoggingTypeDef](./type_defs.md#loggingtypedef) [:material-code-braces: LoggingOutputTypeDef](./type_defs.md#loggingoutputtypedef) 
4. See [:material-code-braces: EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef) [:material-code-braces: EncryptionConfigOutputTypeDef](./type_defs.md#encryptionconfigoutputtypedef) 
5. See [:material-code-braces: OutpostConfigRequestTypeDef](./type_defs.md#outpostconfigrequesttypedef) 
6. See [:material-code-braces: CreateAccessConfigRequestTypeDef](./type_defs.md#createaccessconfigrequesttypedef) 
7. See [:material-code-braces: UpgradePolicyRequestTypeDef](./type_defs.md#upgradepolicyrequesttypedef) 
8. See [:material-code-braces: ZonalShiftConfigRequestTypeDef](./type_defs.md#zonalshiftconfigrequesttypedef) 
9. See [:material-code-braces: RemoteNetworkConfigRequestTypeDef](./type_defs.md#remotenetworkconfigrequesttypedef) 
10. See [:material-code-braces: ComputeConfigRequestTypeDef](./type_defs.md#computeconfigrequesttypedef) 
11. See [:material-code-braces: StorageConfigRequestTypeDef](./type_defs.md#storageconfigrequesttypedef) 
## DescribeInsightResponseTypeDef

```python
# DescribeInsightResponseTypeDef TypedDict usage example

from types_aiobotocore_eks.type_defs import DescribeInsightResponseTypeDef


def get_value() -> DescribeInsightResponseTypeDef:
    return {
        "insight": ...,
    }


# DescribeInsightResponseTypeDef definition

class DescribeInsightResponseTypeDef(TypedDict):
    insight: InsightTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InsightTypeDef](./type_defs.md#insighttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
