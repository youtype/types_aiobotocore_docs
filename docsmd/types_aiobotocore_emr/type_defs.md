# Type definitions

> [Index](../README.md) > [EMR](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [EMR](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#emr)
    type annotations stubs module [types-aiobotocore-emr](https://pypi.org/project/types-aiobotocore-emr/).

## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_emr.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## ApplicationUnionTypeDef

```python
# ApplicationUnionTypeDef Union usage example

from types_aiobotocore_emr.type_defs import ApplicationUnionTypeDef


def get_value() -> ApplicationUnionTypeDef:
    return ...


# ApplicationUnionTypeDef definition

ApplicationUnionTypeDef = Union[
    ApplicationTypeDef,  # (1)
    ApplicationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ApplicationTypeDef](./type_defs.md#applicationtypedef) 
2. See [:material-code-braces: ApplicationOutputTypeDef](./type_defs.md#applicationoutputtypedef) 

## ConfigurationUnionTypeDef

```python
# ConfigurationUnionTypeDef Union usage example

from types_aiobotocore_emr.type_defs import ConfigurationUnionTypeDef


def get_value() -> ConfigurationUnionTypeDef:
    return ...


# ConfigurationUnionTypeDef definition

ConfigurationUnionTypeDef = Union[
    ConfigurationTypeDef,  # (1)
    ConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ConfigurationTypeDef](./type_defs.md#configurationtypedef) 
2. See [:material-code-braces: ConfigurationOutputTypeDef](./type_defs.md#configurationoutputtypedef) 

## InstanceResizePolicyUnionTypeDef

```python
# InstanceResizePolicyUnionTypeDef Union usage example

from types_aiobotocore_emr.type_defs import InstanceResizePolicyUnionTypeDef


def get_value() -> InstanceResizePolicyUnionTypeDef:
    return ...


# InstanceResizePolicyUnionTypeDef definition

InstanceResizePolicyUnionTypeDef = Union[
    InstanceResizePolicyTypeDef,  # (1)
    InstanceResizePolicyOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: InstanceResizePolicyTypeDef](./type_defs.md#instanceresizepolicytypedef) 
2. See [:material-code-braces: InstanceResizePolicyOutputTypeDef](./type_defs.md#instanceresizepolicyoutputtypedef) 

## PlacementTypeUnionTypeDef

```python
# PlacementTypeUnionTypeDef Union usage example

from types_aiobotocore_emr.type_defs import PlacementTypeUnionTypeDef


def get_value() -> PlacementTypeUnionTypeDef:
    return ...


# PlacementTypeUnionTypeDef definition

PlacementTypeUnionTypeDef = Union[
    PlacementTypeTypeDef,  # (1)
    PlacementTypeOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PlacementTypeTypeDef](./type_defs.md#placementtypetypedef) 
2. See [:material-code-braces: PlacementTypeOutputTypeDef](./type_defs.md#placementtypeoutputtypedef) 

## ScriptBootstrapActionConfigUnionTypeDef

```python
# ScriptBootstrapActionConfigUnionTypeDef Union usage example

from types_aiobotocore_emr.type_defs import ScriptBootstrapActionConfigUnionTypeDef


def get_value() -> ScriptBootstrapActionConfigUnionTypeDef:
    return ...


# ScriptBootstrapActionConfigUnionTypeDef definition

ScriptBootstrapActionConfigUnionTypeDef = Union[
    ScriptBootstrapActionConfigTypeDef,  # (1)
    ScriptBootstrapActionConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ScriptBootstrapActionConfigTypeDef](./type_defs.md#scriptbootstrapactionconfigtypedef) 
2. See [:material-code-braces: ScriptBootstrapActionConfigOutputTypeDef](./type_defs.md#scriptbootstrapactionconfigoutputtypedef) 

## BlockPublicAccessConfigurationUnionTypeDef

```python
# BlockPublicAccessConfigurationUnionTypeDef Union usage example

from types_aiobotocore_emr.type_defs import BlockPublicAccessConfigurationUnionTypeDef


def get_value() -> BlockPublicAccessConfigurationUnionTypeDef:
    return ...


# BlockPublicAccessConfigurationUnionTypeDef definition

BlockPublicAccessConfigurationUnionTypeDef = Union[
    BlockPublicAccessConfigurationTypeDef,  # (1)
    BlockPublicAccessConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: BlockPublicAccessConfigurationTypeDef](./type_defs.md#blockpublicaccessconfigurationtypedef) 
2. See [:material-code-braces: BlockPublicAccessConfigurationOutputTypeDef](./type_defs.md#blockpublicaccessconfigurationoutputtypedef) 

## CloudWatchAlarmDefinitionUnionTypeDef

```python
# CloudWatchAlarmDefinitionUnionTypeDef Union usage example

from types_aiobotocore_emr.type_defs import CloudWatchAlarmDefinitionUnionTypeDef


def get_value() -> CloudWatchAlarmDefinitionUnionTypeDef:
    return ...


# CloudWatchAlarmDefinitionUnionTypeDef definition

CloudWatchAlarmDefinitionUnionTypeDef = Union[
    CloudWatchAlarmDefinitionTypeDef,  # (1)
    CloudWatchAlarmDefinitionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CloudWatchAlarmDefinitionTypeDef](./type_defs.md#cloudwatchalarmdefinitiontypedef) 
2. See [:material-code-braces: CloudWatchAlarmDefinitionOutputTypeDef](./type_defs.md#cloudwatchalarmdefinitionoutputtypedef) 

## HadoopJarStepConfigUnionTypeDef

```python
# HadoopJarStepConfigUnionTypeDef Union usage example

from types_aiobotocore_emr.type_defs import HadoopJarStepConfigUnionTypeDef


def get_value() -> HadoopJarStepConfigUnionTypeDef:
    return ...


# HadoopJarStepConfigUnionTypeDef definition

HadoopJarStepConfigUnionTypeDef = Union[
    HadoopJarStepConfigTypeDef,  # (1)
    HadoopJarStepConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: HadoopJarStepConfigTypeDef](./type_defs.md#hadoopjarstepconfigtypedef) 
2. See [:material-code-braces: HadoopJarStepConfigOutputTypeDef](./type_defs.md#hadoopjarstepconfigoutputtypedef) 

## ShrinkPolicyUnionTypeDef

```python
# ShrinkPolicyUnionTypeDef Union usage example

from types_aiobotocore_emr.type_defs import ShrinkPolicyUnionTypeDef


def get_value() -> ShrinkPolicyUnionTypeDef:
    return ...


# ShrinkPolicyUnionTypeDef definition

ShrinkPolicyUnionTypeDef = Union[
    ShrinkPolicyTypeDef,  # (1)
    ShrinkPolicyOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ShrinkPolicyTypeDef](./type_defs.md#shrinkpolicytypedef) 
2. See [:material-code-braces: ShrinkPolicyOutputTypeDef](./type_defs.md#shrinkpolicyoutputtypedef) 

## BootstrapActionConfigUnionTypeDef

```python
# BootstrapActionConfigUnionTypeDef Union usage example

from types_aiobotocore_emr.type_defs import BootstrapActionConfigUnionTypeDef


def get_value() -> BootstrapActionConfigUnionTypeDef:
    return ...


# BootstrapActionConfigUnionTypeDef definition

BootstrapActionConfigUnionTypeDef = Union[
    BootstrapActionConfigTypeDef,  # (1)
    BootstrapActionConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: BootstrapActionConfigTypeDef](./type_defs.md#bootstrapactionconfigtypedef) 
2. See [:material-code-braces: BootstrapActionConfigOutputTypeDef](./type_defs.md#bootstrapactionconfigoutputtypedef) 

## ScalingTriggerUnionTypeDef

```python
# ScalingTriggerUnionTypeDef Union usage example

from types_aiobotocore_emr.type_defs import ScalingTriggerUnionTypeDef


def get_value() -> ScalingTriggerUnionTypeDef:
    return ...


# ScalingTriggerUnionTypeDef definition

ScalingTriggerUnionTypeDef = Union[
    ScalingTriggerTypeDef,  # (1)
    ScalingTriggerOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ScalingTriggerTypeDef](./type_defs.md#scalingtriggertypedef) 
2. See [:material-code-braces: ScalingTriggerOutputTypeDef](./type_defs.md#scalingtriggeroutputtypedef) 

## StepConfigUnionTypeDef

```python
# StepConfigUnionTypeDef Union usage example

from types_aiobotocore_emr.type_defs import StepConfigUnionTypeDef


def get_value() -> StepConfigUnionTypeDef:
    return ...


# StepConfigUnionTypeDef definition

StepConfigUnionTypeDef = Union[
    StepConfigTypeDef,  # (1)
    StepConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: StepConfigTypeDef](./type_defs.md#stepconfigtypedef) 
2. See [:material-code-braces: StepConfigOutputTypeDef](./type_defs.md#stepconfigoutputtypedef) 

## ScalingRuleUnionTypeDef

```python
# ScalingRuleUnionTypeDef Union usage example

from types_aiobotocore_emr.type_defs import ScalingRuleUnionTypeDef


def get_value() -> ScalingRuleUnionTypeDef:
    return ...


# ScalingRuleUnionTypeDef definition

ScalingRuleUnionTypeDef = Union[
    ScalingRuleTypeDef,  # (1)
    ScalingRuleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ScalingRuleTypeDef](./type_defs.md#scalingruletypedef) 
2. See [:material-code-braces: ScalingRuleOutputTypeDef](./type_defs.md#scalingruleoutputtypedef) 



## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ResponseMetadataTypeDef


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

## TagTypeDef

```python
# TagTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import TagTypeDef


def get_value() -> TagTypeDef:
    return {
        "Key": ...,
    }


# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## ApplicationOutputTypeDef

```python
# ApplicationOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ApplicationOutputTypeDef


def get_value() -> ApplicationOutputTypeDef:
    return {
        "Name": ...,
    }


# ApplicationOutputTypeDef definition

class ApplicationOutputTypeDef(TypedDict):
    Name: NotRequired[str],
    Version: NotRequired[str],
    Args: NotRequired[List[str]],
    AdditionalInfo: NotRequired[Dict[str, str]],
```

## ApplicationTypeDef

```python
# ApplicationTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ApplicationTypeDef


def get_value() -> ApplicationTypeDef:
    return {
        "Name": ...,
    }


# ApplicationTypeDef definition

class ApplicationTypeDef(TypedDict):
    Name: NotRequired[str],
    Version: NotRequired[str],
    Args: NotRequired[Sequence[str]],
    AdditionalInfo: NotRequired[Mapping[str, str]],
```

## ScalingConstraintsTypeDef

```python
# ScalingConstraintsTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ScalingConstraintsTypeDef


def get_value() -> ScalingConstraintsTypeDef:
    return {
        "MinCapacity": ...,
    }


# ScalingConstraintsTypeDef definition

class ScalingConstraintsTypeDef(TypedDict):
    MinCapacity: int,
    MaxCapacity: int,
```

## AutoScalingPolicyStateChangeReasonTypeDef

```python
# AutoScalingPolicyStateChangeReasonTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import AutoScalingPolicyStateChangeReasonTypeDef


def get_value() -> AutoScalingPolicyStateChangeReasonTypeDef:
    return {
        "Code": ...,
    }


# AutoScalingPolicyStateChangeReasonTypeDef definition

class AutoScalingPolicyStateChangeReasonTypeDef(TypedDict):
    Code: NotRequired[AutoScalingPolicyStateChangeReasonCodeType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: AutoScalingPolicyStateChangeReasonCodeType](./literals.md#autoscalingpolicystatechangereasoncodetype) 
## AutoTerminationPolicyTypeDef

```python
# AutoTerminationPolicyTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import AutoTerminationPolicyTypeDef


def get_value() -> AutoTerminationPolicyTypeDef:
    return {
        "IdleTimeout": ...,
    }


# AutoTerminationPolicyTypeDef definition

class AutoTerminationPolicyTypeDef(TypedDict):
    IdleTimeout: NotRequired[int],
```

## BlockPublicAccessConfigurationMetadataTypeDef

```python
# BlockPublicAccessConfigurationMetadataTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import BlockPublicAccessConfigurationMetadataTypeDef


def get_value() -> BlockPublicAccessConfigurationMetadataTypeDef:
    return {
        "CreationDateTime": ...,
    }


# BlockPublicAccessConfigurationMetadataTypeDef definition

class BlockPublicAccessConfigurationMetadataTypeDef(TypedDict):
    CreationDateTime: datetime,
    CreatedByArn: str,
```

## PortRangeTypeDef

```python
# PortRangeTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import PortRangeTypeDef


def get_value() -> PortRangeTypeDef:
    return {
        "MinRange": ...,
    }


# PortRangeTypeDef definition

class PortRangeTypeDef(TypedDict):
    MinRange: int,
    MaxRange: NotRequired[int],
```

## ScriptBootstrapActionConfigOutputTypeDef

```python
# ScriptBootstrapActionConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ScriptBootstrapActionConfigOutputTypeDef


def get_value() -> ScriptBootstrapActionConfigOutputTypeDef:
    return {
        "Path": ...,
    }


# ScriptBootstrapActionConfigOutputTypeDef definition

class ScriptBootstrapActionConfigOutputTypeDef(TypedDict):
    Path: str,
    Args: NotRequired[List[str]],
```

## CancelStepsInfoTypeDef

```python
# CancelStepsInfoTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import CancelStepsInfoTypeDef


def get_value() -> CancelStepsInfoTypeDef:
    return {
        "StepId": ...,
    }


# CancelStepsInfoTypeDef definition

class CancelStepsInfoTypeDef(TypedDict):
    StepId: NotRequired[str],
    Status: NotRequired[CancelStepsRequestStatusType],  # (1)
    Reason: NotRequired[str],
```

1. See [:material-code-brackets: CancelStepsRequestStatusType](./literals.md#cancelstepsrequeststatustype) 
## CancelStepsInputTypeDef

```python
# CancelStepsInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import CancelStepsInputTypeDef


def get_value() -> CancelStepsInputTypeDef:
    return {
        "ClusterId": ...,
    }


# CancelStepsInputTypeDef definition

class CancelStepsInputTypeDef(TypedDict):
    ClusterId: str,
    StepIds: Sequence[str],
    StepCancellationOption: NotRequired[StepCancellationOptionType],  # (1)
```

1. See [:material-code-brackets: StepCancellationOptionType](./literals.md#stepcancellationoptiontype) 
## MetricDimensionTypeDef

```python
# MetricDimensionTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import MetricDimensionTypeDef


def get_value() -> MetricDimensionTypeDef:
    return {
        "Key": ...,
    }


# MetricDimensionTypeDef definition

class MetricDimensionTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## ClusterStateChangeReasonTypeDef

```python
# ClusterStateChangeReasonTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ClusterStateChangeReasonTypeDef


def get_value() -> ClusterStateChangeReasonTypeDef:
    return {
        "Code": ...,
    }


# ClusterStateChangeReasonTypeDef definition

class ClusterStateChangeReasonTypeDef(TypedDict):
    Code: NotRequired[ClusterStateChangeReasonCodeType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: ClusterStateChangeReasonCodeType](./literals.md#clusterstatechangereasoncodetype) 
## ClusterTimelineTypeDef

```python
# ClusterTimelineTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ClusterTimelineTypeDef


def get_value() -> ClusterTimelineTypeDef:
    return {
        "CreationDateTime": ...,
    }


# ClusterTimelineTypeDef definition

class ClusterTimelineTypeDef(TypedDict):
    CreationDateTime: NotRequired[datetime],
    ReadyDateTime: NotRequired[datetime],
    EndDateTime: NotRequired[datetime],
```

## ErrorDetailTypeDef

```python
# ErrorDetailTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ErrorDetailTypeDef


def get_value() -> ErrorDetailTypeDef:
    return {
        "ErrorCode": ...,
    }


# ErrorDetailTypeDef definition

class ErrorDetailTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    ErrorData: NotRequired[List[Dict[str, str]]],
    ErrorMessage: NotRequired[str],
```

## ConfigurationOutputTypeDef

```python
# ConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ConfigurationOutputTypeDef


def get_value() -> ConfigurationOutputTypeDef:
    return {
        "Classification": ...,
    }


# ConfigurationOutputTypeDef definition

class ConfigurationOutputTypeDef(TypedDict):
    Classification: NotRequired[str],
    Configurations: NotRequired[List[Dict[str, Any]]],
    Properties: NotRequired[Dict[str, str]],
```

## Ec2InstanceAttributesTypeDef

```python
# Ec2InstanceAttributesTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import Ec2InstanceAttributesTypeDef


def get_value() -> Ec2InstanceAttributesTypeDef:
    return {
        "Ec2KeyName": ...,
    }


# Ec2InstanceAttributesTypeDef definition

class Ec2InstanceAttributesTypeDef(TypedDict):
    Ec2KeyName: NotRequired[str],
    Ec2SubnetId: NotRequired[str],
    RequestedEc2SubnetIds: NotRequired[List[str]],
    Ec2AvailabilityZone: NotRequired[str],
    RequestedEc2AvailabilityZones: NotRequired[List[str]],
    IamInstanceProfile: NotRequired[str],
    EmrManagedMasterSecurityGroup: NotRequired[str],
    EmrManagedSlaveSecurityGroup: NotRequired[str],
    ServiceAccessSecurityGroup: NotRequired[str],
    AdditionalMasterSecurityGroups: NotRequired[List[str]],
    AdditionalSlaveSecurityGroups: NotRequired[List[str]],
```

## KerberosAttributesTypeDef

```python
# KerberosAttributesTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import KerberosAttributesTypeDef


def get_value() -> KerberosAttributesTypeDef:
    return {
        "Realm": ...,
    }


# KerberosAttributesTypeDef definition

class KerberosAttributesTypeDef(TypedDict):
    Realm: str,
    KdcAdminPassword: str,
    CrossRealmTrustPrincipalPassword: NotRequired[str],
    ADDomainJoinUser: NotRequired[str],
    ADDomainJoinPassword: NotRequired[str],
```

## PlacementGroupConfigTypeDef

```python
# PlacementGroupConfigTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import PlacementGroupConfigTypeDef


def get_value() -> PlacementGroupConfigTypeDef:
    return {
        "InstanceRole": ...,
    }


# PlacementGroupConfigTypeDef definition

class PlacementGroupConfigTypeDef(TypedDict):
    InstanceRole: InstanceRoleTypeType,  # (1)
    PlacementStrategy: NotRequired[PlacementGroupStrategyType],  # (2)
```

1. See [:material-code-brackets: InstanceRoleTypeType](./literals.md#instanceroletypetype) 
2. See [:material-code-brackets: PlacementGroupStrategyType](./literals.md#placementgroupstrategytype) 
## CommandTypeDef

```python
# CommandTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import CommandTypeDef


def get_value() -> CommandTypeDef:
    return {
        "Name": ...,
    }


# CommandTypeDef definition

class CommandTypeDef(TypedDict):
    Name: NotRequired[str],
    ScriptPath: NotRequired[str],
    Args: NotRequired[List[str]],
```

## ComputeLimitsTypeDef

```python
# ComputeLimitsTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ComputeLimitsTypeDef


def get_value() -> ComputeLimitsTypeDef:
    return {
        "UnitType": ...,
    }


# ComputeLimitsTypeDef definition

class ComputeLimitsTypeDef(TypedDict):
    UnitType: ComputeLimitsUnitTypeType,  # (1)
    MinimumCapacityUnits: int,
    MaximumCapacityUnits: int,
    MaximumOnDemandCapacityUnits: NotRequired[int],
    MaximumCoreCapacityUnits: NotRequired[int],
```

1. See [:material-code-brackets: ComputeLimitsUnitTypeType](./literals.md#computelimitsunittypetype) 
## ConfigurationPaginatorTypeDef

```python
# ConfigurationPaginatorTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ConfigurationPaginatorTypeDef


def get_value() -> ConfigurationPaginatorTypeDef:
    return {
        "Classification": ...,
    }


# ConfigurationPaginatorTypeDef definition

class ConfigurationPaginatorTypeDef(TypedDict):
    Classification: NotRequired[str],
    Configurations: NotRequired[List[Dict[str, Any]]],
    Properties: NotRequired[Dict[str, str]],
```

## ConfigurationTypeDef

```python
# ConfigurationTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ConfigurationTypeDef


def get_value() -> ConfigurationTypeDef:
    return {
        "Classification": ...,
    }


# ConfigurationTypeDef definition

class ConfigurationTypeDef(TypedDict):
    Classification: NotRequired[str],
    Configurations: NotRequired[Sequence[Mapping[str, Any]]],
    Properties: NotRequired[Mapping[str, str]],
```

## CreateSecurityConfigurationInputTypeDef

```python
# CreateSecurityConfigurationInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import CreateSecurityConfigurationInputTypeDef


def get_value() -> CreateSecurityConfigurationInputTypeDef:
    return {
        "Name": ...,
    }


# CreateSecurityConfigurationInputTypeDef definition

class CreateSecurityConfigurationInputTypeDef(TypedDict):
    Name: str,
    SecurityConfiguration: str,
```

## CreateStudioSessionMappingInputTypeDef

```python
# CreateStudioSessionMappingInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import CreateStudioSessionMappingInputTypeDef


def get_value() -> CreateStudioSessionMappingInputTypeDef:
    return {
        "StudioId": ...,
    }


# CreateStudioSessionMappingInputTypeDef definition

class CreateStudioSessionMappingInputTypeDef(TypedDict):
    StudioId: str,
    IdentityType: IdentityTypeType,  # (1)
    SessionPolicyArn: str,
    IdentityId: NotRequired[str],
    IdentityName: NotRequired[str],
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
## UsernamePasswordTypeDef

```python
# UsernamePasswordTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import UsernamePasswordTypeDef


def get_value() -> UsernamePasswordTypeDef:
    return {
        "Username": ...,
    }


# UsernamePasswordTypeDef definition

class UsernamePasswordTypeDef(TypedDict):
    Username: NotRequired[str],
    Password: NotRequired[str],
```

## DeleteSecurityConfigurationInputTypeDef

```python
# DeleteSecurityConfigurationInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import DeleteSecurityConfigurationInputTypeDef


def get_value() -> DeleteSecurityConfigurationInputTypeDef:
    return {
        "Name": ...,
    }


# DeleteSecurityConfigurationInputTypeDef definition

class DeleteSecurityConfigurationInputTypeDef(TypedDict):
    Name: str,
```

## DeleteStudioInputTypeDef

```python
# DeleteStudioInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import DeleteStudioInputTypeDef


def get_value() -> DeleteStudioInputTypeDef:
    return {
        "StudioId": ...,
    }


# DeleteStudioInputTypeDef definition

class DeleteStudioInputTypeDef(TypedDict):
    StudioId: str,
```

## DeleteStudioSessionMappingInputTypeDef

```python
# DeleteStudioSessionMappingInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import DeleteStudioSessionMappingInputTypeDef


def get_value() -> DeleteStudioSessionMappingInputTypeDef:
    return {
        "StudioId": ...,
    }


# DeleteStudioSessionMappingInputTypeDef definition

class DeleteStudioSessionMappingInputTypeDef(TypedDict):
    StudioId: str,
    IdentityType: IdentityTypeType,  # (1)
    IdentityId: NotRequired[str],
    IdentityName: NotRequired[str],
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
## DescribeClusterInputTypeDef

```python
# DescribeClusterInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import DescribeClusterInputTypeDef


def get_value() -> DescribeClusterInputTypeDef:
    return {
        "ClusterId": ...,
    }


# DescribeClusterInputTypeDef definition

class DescribeClusterInputTypeDef(TypedDict):
    ClusterId: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import WaiterConfigTypeDef


def get_value() -> WaiterConfigTypeDef:
    return {
        "Delay": ...,
    }


# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeNotebookExecutionInputTypeDef

```python
# DescribeNotebookExecutionInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import DescribeNotebookExecutionInputTypeDef


def get_value() -> DescribeNotebookExecutionInputTypeDef:
    return {
        "NotebookExecutionId": ...,
    }


# DescribeNotebookExecutionInputTypeDef definition

class DescribeNotebookExecutionInputTypeDef(TypedDict):
    NotebookExecutionId: str,
```

## DescribeReleaseLabelInputTypeDef

```python
# DescribeReleaseLabelInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import DescribeReleaseLabelInputTypeDef


def get_value() -> DescribeReleaseLabelInputTypeDef:
    return {
        "ReleaseLabel": ...,
    }


# DescribeReleaseLabelInputTypeDef definition

class DescribeReleaseLabelInputTypeDef(TypedDict):
    ReleaseLabel: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## OSReleaseTypeDef

```python
# OSReleaseTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import OSReleaseTypeDef


def get_value() -> OSReleaseTypeDef:
    return {
        "Label": ...,
    }


# OSReleaseTypeDef definition

class OSReleaseTypeDef(TypedDict):
    Label: NotRequired[str],
```

## SimplifiedApplicationTypeDef

```python
# SimplifiedApplicationTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import SimplifiedApplicationTypeDef


def get_value() -> SimplifiedApplicationTypeDef:
    return {
        "Name": ...,
    }


# SimplifiedApplicationTypeDef definition

class SimplifiedApplicationTypeDef(TypedDict):
    Name: NotRequired[str],
    Version: NotRequired[str],
```

## DescribeSecurityConfigurationInputTypeDef

```python
# DescribeSecurityConfigurationInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import DescribeSecurityConfigurationInputTypeDef


def get_value() -> DescribeSecurityConfigurationInputTypeDef:
    return {
        "Name": ...,
    }


# DescribeSecurityConfigurationInputTypeDef definition

class DescribeSecurityConfigurationInputTypeDef(TypedDict):
    Name: str,
```

## DescribeStepInputTypeDef

```python
# DescribeStepInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import DescribeStepInputTypeDef


def get_value() -> DescribeStepInputTypeDef:
    return {
        "ClusterId": ...,
    }


# DescribeStepInputTypeDef definition

class DescribeStepInputTypeDef(TypedDict):
    ClusterId: str,
    StepId: str,
```

## DescribeStudioInputTypeDef

```python
# DescribeStudioInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import DescribeStudioInputTypeDef


def get_value() -> DescribeStudioInputTypeDef:
    return {
        "StudioId": ...,
    }


# DescribeStudioInputTypeDef definition

class DescribeStudioInputTypeDef(TypedDict):
    StudioId: str,
```

## VolumeSpecificationTypeDef

```python
# VolumeSpecificationTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import VolumeSpecificationTypeDef


def get_value() -> VolumeSpecificationTypeDef:
    return {
        "VolumeType": ...,
    }


# VolumeSpecificationTypeDef definition

class VolumeSpecificationTypeDef(TypedDict):
    VolumeType: str,
    SizeInGB: int,
    Iops: NotRequired[int],
    Throughput: NotRequired[int],
```

## EbsVolumeTypeDef

```python
# EbsVolumeTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import EbsVolumeTypeDef


def get_value() -> EbsVolumeTypeDef:
    return {
        "Device": ...,
    }


# EbsVolumeTypeDef definition

class EbsVolumeTypeDef(TypedDict):
    Device: NotRequired[str],
    VolumeId: NotRequired[str],
```

## ExecutionEngineConfigTypeDef

```python
# ExecutionEngineConfigTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ExecutionEngineConfigTypeDef


def get_value() -> ExecutionEngineConfigTypeDef:
    return {
        "Id": ...,
    }


# ExecutionEngineConfigTypeDef definition

class ExecutionEngineConfigTypeDef(TypedDict):
    Id: str,
    Type: NotRequired[ExecutionEngineTypeType],  # (1)
    MasterInstanceSecurityGroupId: NotRequired[str],
    ExecutionRoleArn: NotRequired[str],
```

1. See [:material-code-brackets: ExecutionEngineTypeType](./literals.md#executionenginetypetype) 
## FailureDetailsTypeDef

```python
# FailureDetailsTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import FailureDetailsTypeDef


def get_value() -> FailureDetailsTypeDef:
    return {
        "Reason": ...,
    }


# FailureDetailsTypeDef definition

class FailureDetailsTypeDef(TypedDict):
    Reason: NotRequired[str],
    Message: NotRequired[str],
    LogFile: NotRequired[str],
```

## GetAutoTerminationPolicyInputTypeDef

```python
# GetAutoTerminationPolicyInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import GetAutoTerminationPolicyInputTypeDef


def get_value() -> GetAutoTerminationPolicyInputTypeDef:
    return {
        "ClusterId": ...,
    }


# GetAutoTerminationPolicyInputTypeDef definition

class GetAutoTerminationPolicyInputTypeDef(TypedDict):
    ClusterId: str,
```

## GetClusterSessionCredentialsInputTypeDef

```python
# GetClusterSessionCredentialsInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import GetClusterSessionCredentialsInputTypeDef


def get_value() -> GetClusterSessionCredentialsInputTypeDef:
    return {
        "ClusterId": ...,
    }


# GetClusterSessionCredentialsInputTypeDef definition

class GetClusterSessionCredentialsInputTypeDef(TypedDict):
    ClusterId: str,
    ExecutionRoleArn: NotRequired[str],
```

## GetManagedScalingPolicyInputTypeDef

```python
# GetManagedScalingPolicyInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import GetManagedScalingPolicyInputTypeDef


def get_value() -> GetManagedScalingPolicyInputTypeDef:
    return {
        "ClusterId": ...,
    }


# GetManagedScalingPolicyInputTypeDef definition

class GetManagedScalingPolicyInputTypeDef(TypedDict):
    ClusterId: str,
```

## GetStudioSessionMappingInputTypeDef

```python
# GetStudioSessionMappingInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import GetStudioSessionMappingInputTypeDef


def get_value() -> GetStudioSessionMappingInputTypeDef:
    return {
        "StudioId": ...,
    }


# GetStudioSessionMappingInputTypeDef definition

class GetStudioSessionMappingInputTypeDef(TypedDict):
    StudioId: str,
    IdentityType: IdentityTypeType,  # (1)
    IdentityId: NotRequired[str],
    IdentityName: NotRequired[str],
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
## SessionMappingDetailTypeDef

```python
# SessionMappingDetailTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import SessionMappingDetailTypeDef


def get_value() -> SessionMappingDetailTypeDef:
    return {
        "StudioId": ...,
    }


# SessionMappingDetailTypeDef definition

class SessionMappingDetailTypeDef(TypedDict):
    StudioId: NotRequired[str],
    IdentityId: NotRequired[str],
    IdentityName: NotRequired[str],
    IdentityType: NotRequired[IdentityTypeType],  # (1)
    SessionPolicyArn: NotRequired[str],
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
## KeyValueTypeDef

```python
# KeyValueTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import KeyValueTypeDef


def get_value() -> KeyValueTypeDef:
    return {
        "Key": ...,
    }


# KeyValueTypeDef definition

class KeyValueTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## HadoopStepConfigTypeDef

```python
# HadoopStepConfigTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import HadoopStepConfigTypeDef


def get_value() -> HadoopStepConfigTypeDef:
    return {
        "Jar": ...,
    }


# HadoopStepConfigTypeDef definition

class HadoopStepConfigTypeDef(TypedDict):
    Jar: NotRequired[str],
    Properties: NotRequired[Dict[str, str]],
    MainClass: NotRequired[str],
    Args: NotRequired[List[str]],
```

## SpotProvisioningSpecificationTypeDef

```python
# SpotProvisioningSpecificationTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import SpotProvisioningSpecificationTypeDef


def get_value() -> SpotProvisioningSpecificationTypeDef:
    return {
        "TimeoutDurationMinutes": ...,
    }


# SpotProvisioningSpecificationTypeDef definition

class SpotProvisioningSpecificationTypeDef(TypedDict):
    TimeoutDurationMinutes: int,
    TimeoutAction: SpotProvisioningTimeoutActionType,  # (1)
    BlockDurationMinutes: NotRequired[int],
    AllocationStrategy: NotRequired[SpotProvisioningAllocationStrategyType],  # (2)
```

1. See [:material-code-brackets: SpotProvisioningTimeoutActionType](./literals.md#spotprovisioningtimeoutactiontype) 
2. See [:material-code-brackets: SpotProvisioningAllocationStrategyType](./literals.md#spotprovisioningallocationstrategytype) 
## SpotResizingSpecificationTypeDef

```python
# SpotResizingSpecificationTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import SpotResizingSpecificationTypeDef


def get_value() -> SpotResizingSpecificationTypeDef:
    return {
        "TimeoutDurationMinutes": ...,
    }


# SpotResizingSpecificationTypeDef definition

class SpotResizingSpecificationTypeDef(TypedDict):
    TimeoutDurationMinutes: NotRequired[int],
    AllocationStrategy: NotRequired[SpotProvisioningAllocationStrategyType],  # (1)
```

1. See [:material-code-brackets: SpotProvisioningAllocationStrategyType](./literals.md#spotprovisioningallocationstrategytype) 
## InstanceFleetStateChangeReasonTypeDef

```python
# InstanceFleetStateChangeReasonTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import InstanceFleetStateChangeReasonTypeDef


def get_value() -> InstanceFleetStateChangeReasonTypeDef:
    return {
        "Code": ...,
    }


# InstanceFleetStateChangeReasonTypeDef definition

class InstanceFleetStateChangeReasonTypeDef(TypedDict):
    Code: NotRequired[InstanceFleetStateChangeReasonCodeType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: InstanceFleetStateChangeReasonCodeType](./literals.md#instancefleetstatechangereasoncodetype) 
## InstanceFleetTimelineTypeDef

```python
# InstanceFleetTimelineTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import InstanceFleetTimelineTypeDef


def get_value() -> InstanceFleetTimelineTypeDef:
    return {
        "CreationDateTime": ...,
    }


# InstanceFleetTimelineTypeDef definition

class InstanceFleetTimelineTypeDef(TypedDict):
    CreationDateTime: NotRequired[datetime],
    ReadyDateTime: NotRequired[datetime],
    EndDateTime: NotRequired[datetime],
```

## InstanceGroupDetailTypeDef

```python
# InstanceGroupDetailTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import InstanceGroupDetailTypeDef


def get_value() -> InstanceGroupDetailTypeDef:
    return {
        "InstanceGroupId": ...,
    }


# InstanceGroupDetailTypeDef definition

class InstanceGroupDetailTypeDef(TypedDict):
    Market: MarketTypeType,  # (1)
    InstanceRole: InstanceRoleTypeType,  # (2)
    InstanceType: str,
    InstanceRequestCount: int,
    InstanceRunningCount: int,
    State: InstanceGroupStateType,  # (3)
    CreationDateTime: datetime,
    InstanceGroupId: NotRequired[str],
    Name: NotRequired[str],
    BidPrice: NotRequired[str],
    LastStateChangeReason: NotRequired[str],
    StartDateTime: NotRequired[datetime],
    ReadyDateTime: NotRequired[datetime],
    EndDateTime: NotRequired[datetime],
    CustomAmiId: NotRequired[str],
```

1. See [:material-code-brackets: MarketTypeType](./literals.md#markettypetype) 
2. See [:material-code-brackets: InstanceRoleTypeType](./literals.md#instanceroletypetype) 
3. See [:material-code-brackets: InstanceGroupStateType](./literals.md#instancegroupstatetype) 
## InstanceGroupStateChangeReasonTypeDef

```python
# InstanceGroupStateChangeReasonTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import InstanceGroupStateChangeReasonTypeDef


def get_value() -> InstanceGroupStateChangeReasonTypeDef:
    return {
        "Code": ...,
    }


# InstanceGroupStateChangeReasonTypeDef definition

class InstanceGroupStateChangeReasonTypeDef(TypedDict):
    Code: NotRequired[InstanceGroupStateChangeReasonCodeType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: InstanceGroupStateChangeReasonCodeType](./literals.md#instancegroupstatechangereasoncodetype) 
## InstanceGroupTimelineTypeDef

```python
# InstanceGroupTimelineTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import InstanceGroupTimelineTypeDef


def get_value() -> InstanceGroupTimelineTypeDef:
    return {
        "CreationDateTime": ...,
    }


# InstanceGroupTimelineTypeDef definition

class InstanceGroupTimelineTypeDef(TypedDict):
    CreationDateTime: NotRequired[datetime],
    ReadyDateTime: NotRequired[datetime],
    EndDateTime: NotRequired[datetime],
```

## InstanceResizePolicyOutputTypeDef

```python
# InstanceResizePolicyOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import InstanceResizePolicyOutputTypeDef


def get_value() -> InstanceResizePolicyOutputTypeDef:
    return {
        "InstancesToTerminate": ...,
    }


# InstanceResizePolicyOutputTypeDef definition

class InstanceResizePolicyOutputTypeDef(TypedDict):
    InstancesToTerminate: NotRequired[List[str]],
    InstancesToProtect: NotRequired[List[str]],
    InstanceTerminationTimeout: NotRequired[int],
```

## InstanceResizePolicyTypeDef

```python
# InstanceResizePolicyTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import InstanceResizePolicyTypeDef


def get_value() -> InstanceResizePolicyTypeDef:
    return {
        "InstancesToTerminate": ...,
    }


# InstanceResizePolicyTypeDef definition

class InstanceResizePolicyTypeDef(TypedDict):
    InstancesToTerminate: NotRequired[Sequence[str]],
    InstancesToProtect: NotRequired[Sequence[str]],
    InstanceTerminationTimeout: NotRequired[int],
```

## InstanceStateChangeReasonTypeDef

```python
# InstanceStateChangeReasonTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import InstanceStateChangeReasonTypeDef


def get_value() -> InstanceStateChangeReasonTypeDef:
    return {
        "Code": ...,
    }


# InstanceStateChangeReasonTypeDef definition

class InstanceStateChangeReasonTypeDef(TypedDict):
    Code: NotRequired[InstanceStateChangeReasonCodeType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: InstanceStateChangeReasonCodeType](./literals.md#instancestatechangereasoncodetype) 
## InstanceTimelineTypeDef

```python
# InstanceTimelineTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import InstanceTimelineTypeDef


def get_value() -> InstanceTimelineTypeDef:
    return {
        "CreationDateTime": ...,
    }


# InstanceTimelineTypeDef definition

class InstanceTimelineTypeDef(TypedDict):
    CreationDateTime: NotRequired[datetime],
    ReadyDateTime: NotRequired[datetime],
    EndDateTime: NotRequired[datetime],
```

## JobFlowExecutionStatusDetailTypeDef

```python
# JobFlowExecutionStatusDetailTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import JobFlowExecutionStatusDetailTypeDef


def get_value() -> JobFlowExecutionStatusDetailTypeDef:
    return {
        "State": ...,
    }


# JobFlowExecutionStatusDetailTypeDef definition

class JobFlowExecutionStatusDetailTypeDef(TypedDict):
    State: JobFlowExecutionStateType,  # (1)
    CreationDateTime: datetime,
    StartDateTime: NotRequired[datetime],
    ReadyDateTime: NotRequired[datetime],
    EndDateTime: NotRequired[datetime],
    LastStateChangeReason: NotRequired[str],
```

1. See [:material-code-brackets: JobFlowExecutionStateType](./literals.md#jobflowexecutionstatetype) 
## PlacementTypeOutputTypeDef

```python
# PlacementTypeOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import PlacementTypeOutputTypeDef


def get_value() -> PlacementTypeOutputTypeDef:
    return {
        "AvailabilityZone": ...,
    }


# PlacementTypeOutputTypeDef definition

class PlacementTypeOutputTypeDef(TypedDict):
    AvailabilityZone: NotRequired[str],
    AvailabilityZones: NotRequired[List[str]],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import PaginatorConfigTypeDef


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

## ListBootstrapActionsInputTypeDef

```python
# ListBootstrapActionsInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListBootstrapActionsInputTypeDef


def get_value() -> ListBootstrapActionsInputTypeDef:
    return {
        "ClusterId": ...,
    }


# ListBootstrapActionsInputTypeDef definition

class ListBootstrapActionsInputTypeDef(TypedDict):
    ClusterId: str,
    Marker: NotRequired[str],
```

## ListInstanceFleetsInputTypeDef

```python
# ListInstanceFleetsInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListInstanceFleetsInputTypeDef


def get_value() -> ListInstanceFleetsInputTypeDef:
    return {
        "ClusterId": ...,
    }


# ListInstanceFleetsInputTypeDef definition

class ListInstanceFleetsInputTypeDef(TypedDict):
    ClusterId: str,
    Marker: NotRequired[str],
```

## ListInstanceGroupsInputTypeDef

```python
# ListInstanceGroupsInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListInstanceGroupsInputTypeDef


def get_value() -> ListInstanceGroupsInputTypeDef:
    return {
        "ClusterId": ...,
    }


# ListInstanceGroupsInputTypeDef definition

class ListInstanceGroupsInputTypeDef(TypedDict):
    ClusterId: str,
    Marker: NotRequired[str],
```

## ListInstancesInputTypeDef

```python
# ListInstancesInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListInstancesInputTypeDef


def get_value() -> ListInstancesInputTypeDef:
    return {
        "ClusterId": ...,
    }


# ListInstancesInputTypeDef definition

class ListInstancesInputTypeDef(TypedDict):
    ClusterId: str,
    InstanceGroupId: NotRequired[str],
    InstanceGroupTypes: NotRequired[Sequence[InstanceGroupTypeType]],  # (1)
    InstanceFleetId: NotRequired[str],
    InstanceFleetType: NotRequired[InstanceFleetTypeType],  # (2)
    InstanceStates: NotRequired[Sequence[InstanceStateType]],  # (3)
    Marker: NotRequired[str],
```

1. See [:material-code-brackets: InstanceGroupTypeType](./literals.md#instancegrouptypetype) 
2. See [:material-code-brackets: InstanceFleetTypeType](./literals.md#instancefleettypetype) 
3. See [:material-code-brackets: InstanceStateType](./literals.md#instancestatetype) 
## ReleaseLabelFilterTypeDef

```python
# ReleaseLabelFilterTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ReleaseLabelFilterTypeDef


def get_value() -> ReleaseLabelFilterTypeDef:
    return {
        "Prefix": ...,
    }


# ReleaseLabelFilterTypeDef definition

class ReleaseLabelFilterTypeDef(TypedDict):
    Prefix: NotRequired[str],
    Application: NotRequired[str],
```

## ListSecurityConfigurationsInputTypeDef

```python
# ListSecurityConfigurationsInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListSecurityConfigurationsInputTypeDef


def get_value() -> ListSecurityConfigurationsInputTypeDef:
    return {
        "Marker": ...,
    }


# ListSecurityConfigurationsInputTypeDef definition

class ListSecurityConfigurationsInputTypeDef(TypedDict):
    Marker: NotRequired[str],
```

## SecurityConfigurationSummaryTypeDef

```python
# SecurityConfigurationSummaryTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import SecurityConfigurationSummaryTypeDef


def get_value() -> SecurityConfigurationSummaryTypeDef:
    return {
        "Name": ...,
    }


# SecurityConfigurationSummaryTypeDef definition

class SecurityConfigurationSummaryTypeDef(TypedDict):
    Name: NotRequired[str],
    CreationDateTime: NotRequired[datetime],
```

## ListStepsInputTypeDef

```python
# ListStepsInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListStepsInputTypeDef


def get_value() -> ListStepsInputTypeDef:
    return {
        "ClusterId": ...,
    }


# ListStepsInputTypeDef definition

class ListStepsInputTypeDef(TypedDict):
    ClusterId: str,
    StepStates: NotRequired[Sequence[StepStateType]],  # (1)
    StepIds: NotRequired[Sequence[str]],
    Marker: NotRequired[str],
```

1. See [:material-code-brackets: StepStateType](./literals.md#stepstatetype) 
## ListStudioSessionMappingsInputTypeDef

```python
# ListStudioSessionMappingsInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListStudioSessionMappingsInputTypeDef


def get_value() -> ListStudioSessionMappingsInputTypeDef:
    return {
        "StudioId": ...,
    }


# ListStudioSessionMappingsInputTypeDef definition

class ListStudioSessionMappingsInputTypeDef(TypedDict):
    StudioId: NotRequired[str],
    IdentityType: NotRequired[IdentityTypeType],  # (1)
    Marker: NotRequired[str],
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
## SessionMappingSummaryTypeDef

```python
# SessionMappingSummaryTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import SessionMappingSummaryTypeDef


def get_value() -> SessionMappingSummaryTypeDef:
    return {
        "StudioId": ...,
    }


# SessionMappingSummaryTypeDef definition

class SessionMappingSummaryTypeDef(TypedDict):
    StudioId: NotRequired[str],
    IdentityId: NotRequired[str],
    IdentityName: NotRequired[str],
    IdentityType: NotRequired[IdentityTypeType],  # (1)
    SessionPolicyArn: NotRequired[str],
    CreationTime: NotRequired[datetime],
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
## ListStudiosInputTypeDef

```python
# ListStudiosInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListStudiosInputTypeDef


def get_value() -> ListStudiosInputTypeDef:
    return {
        "Marker": ...,
    }


# ListStudiosInputTypeDef definition

class ListStudiosInputTypeDef(TypedDict):
    Marker: NotRequired[str],
```

## StudioSummaryTypeDef

```python
# StudioSummaryTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import StudioSummaryTypeDef


def get_value() -> StudioSummaryTypeDef:
    return {
        "StudioId": ...,
    }


# StudioSummaryTypeDef definition

class StudioSummaryTypeDef(TypedDict):
    StudioId: NotRequired[str],
    Name: NotRequired[str],
    VpcId: NotRequired[str],
    Description: NotRequired[str],
    Url: NotRequired[str],
    AuthMode: NotRequired[AuthModeType],  # (1)
    CreationTime: NotRequired[datetime],
```

1. See [:material-code-brackets: AuthModeType](./literals.md#authmodetype) 
## ListSupportedInstanceTypesInputTypeDef

```python
# ListSupportedInstanceTypesInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListSupportedInstanceTypesInputTypeDef


def get_value() -> ListSupportedInstanceTypesInputTypeDef:
    return {
        "ReleaseLabel": ...,
    }


# ListSupportedInstanceTypesInputTypeDef definition

class ListSupportedInstanceTypesInputTypeDef(TypedDict):
    ReleaseLabel: str,
    Marker: NotRequired[str],
```

## SupportedInstanceTypeTypeDef

```python
# SupportedInstanceTypeTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import SupportedInstanceTypeTypeDef


def get_value() -> SupportedInstanceTypeTypeDef:
    return {
        "Type": ...,
    }


# SupportedInstanceTypeTypeDef definition

class SupportedInstanceTypeTypeDef(TypedDict):
    Type: NotRequired[str],
    MemoryGB: NotRequired[float],
    StorageGB: NotRequired[int],
    VCPU: NotRequired[int],
    Is64BitsOnly: NotRequired[bool],
    InstanceFamilyId: NotRequired[str],
    EbsOptimizedAvailable: NotRequired[bool],
    EbsOptimizedByDefault: NotRequired[bool],
    NumberOfDisks: NotRequired[int],
    EbsStorageOnly: NotRequired[bool],
    Architecture: NotRequired[str],
```

## ModifyClusterInputTypeDef

```python
# ModifyClusterInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ModifyClusterInputTypeDef


def get_value() -> ModifyClusterInputTypeDef:
    return {
        "ClusterId": ...,
    }


# ModifyClusterInputTypeDef definition

class ModifyClusterInputTypeDef(TypedDict):
    ClusterId: str,
    StepConcurrencyLevel: NotRequired[int],
```

## NotebookS3LocationForOutputTypeDef

```python
# NotebookS3LocationForOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import NotebookS3LocationForOutputTypeDef


def get_value() -> NotebookS3LocationForOutputTypeDef:
    return {
        "Bucket": ...,
    }


# NotebookS3LocationForOutputTypeDef definition

class NotebookS3LocationForOutputTypeDef(TypedDict):
    Bucket: NotRequired[str],
    Key: NotRequired[str],
```

## OutputNotebookS3LocationForOutputTypeDef

```python
# OutputNotebookS3LocationForOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import OutputNotebookS3LocationForOutputTypeDef


def get_value() -> OutputNotebookS3LocationForOutputTypeDef:
    return {
        "Bucket": ...,
    }


# OutputNotebookS3LocationForOutputTypeDef definition

class OutputNotebookS3LocationForOutputTypeDef(TypedDict):
    Bucket: NotRequired[str],
    Key: NotRequired[str],
```

## NotebookS3LocationFromInputTypeDef

```python
# NotebookS3LocationFromInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import NotebookS3LocationFromInputTypeDef


def get_value() -> NotebookS3LocationFromInputTypeDef:
    return {
        "Bucket": ...,
    }


# NotebookS3LocationFromInputTypeDef definition

class NotebookS3LocationFromInputTypeDef(TypedDict):
    Bucket: NotRequired[str],
    Key: NotRequired[str],
```

## OnDemandCapacityReservationOptionsTypeDef

```python
# OnDemandCapacityReservationOptionsTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import OnDemandCapacityReservationOptionsTypeDef


def get_value() -> OnDemandCapacityReservationOptionsTypeDef:
    return {
        "UsageStrategy": ...,
    }


# OnDemandCapacityReservationOptionsTypeDef definition

class OnDemandCapacityReservationOptionsTypeDef(TypedDict):
    UsageStrategy: NotRequired[OnDemandCapacityReservationUsageStrategyType],  # (1)
    CapacityReservationPreference: NotRequired[OnDemandCapacityReservationPreferenceType],  # (2)
    CapacityReservationResourceGroupArn: NotRequired[str],
```

1. See [:material-code-brackets: OnDemandCapacityReservationUsageStrategyType](./literals.md#ondemandcapacityreservationusagestrategytype) 
2. See [:material-code-brackets: OnDemandCapacityReservationPreferenceType](./literals.md#ondemandcapacityreservationpreferencetype) 
## OutputNotebookS3LocationFromInputTypeDef

```python
# OutputNotebookS3LocationFromInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import OutputNotebookS3LocationFromInputTypeDef


def get_value() -> OutputNotebookS3LocationFromInputTypeDef:
    return {
        "Bucket": ...,
    }


# OutputNotebookS3LocationFromInputTypeDef definition

class OutputNotebookS3LocationFromInputTypeDef(TypedDict):
    Bucket: NotRequired[str],
    Key: NotRequired[str],
```

## PlacementTypeTypeDef

```python
# PlacementTypeTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import PlacementTypeTypeDef


def get_value() -> PlacementTypeTypeDef:
    return {
        "AvailabilityZone": ...,
    }


# PlacementTypeTypeDef definition

class PlacementTypeTypeDef(TypedDict):
    AvailabilityZone: NotRequired[str],
    AvailabilityZones: NotRequired[Sequence[str]],
```

## RemoveAutoScalingPolicyInputTypeDef

```python
# RemoveAutoScalingPolicyInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import RemoveAutoScalingPolicyInputTypeDef


def get_value() -> RemoveAutoScalingPolicyInputTypeDef:
    return {
        "ClusterId": ...,
    }


# RemoveAutoScalingPolicyInputTypeDef definition

class RemoveAutoScalingPolicyInputTypeDef(TypedDict):
    ClusterId: str,
    InstanceGroupId: str,
```

## RemoveAutoTerminationPolicyInputTypeDef

```python
# RemoveAutoTerminationPolicyInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import RemoveAutoTerminationPolicyInputTypeDef


def get_value() -> RemoveAutoTerminationPolicyInputTypeDef:
    return {
        "ClusterId": ...,
    }


# RemoveAutoTerminationPolicyInputTypeDef definition

class RemoveAutoTerminationPolicyInputTypeDef(TypedDict):
    ClusterId: str,
```

## RemoveManagedScalingPolicyInputTypeDef

```python
# RemoveManagedScalingPolicyInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import RemoveManagedScalingPolicyInputTypeDef


def get_value() -> RemoveManagedScalingPolicyInputTypeDef:
    return {
        "ClusterId": ...,
    }


# RemoveManagedScalingPolicyInputTypeDef definition

class RemoveManagedScalingPolicyInputTypeDef(TypedDict):
    ClusterId: str,
```

## RemoveTagsInputTypeDef

```python
# RemoveTagsInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import RemoveTagsInputTypeDef


def get_value() -> RemoveTagsInputTypeDef:
    return {
        "ResourceId": ...,
    }


# RemoveTagsInputTypeDef definition

class RemoveTagsInputTypeDef(TypedDict):
    ResourceId: str,
    TagKeys: Sequence[str],
```

## SupportedProductConfigTypeDef

```python
# SupportedProductConfigTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import SupportedProductConfigTypeDef


def get_value() -> SupportedProductConfigTypeDef:
    return {
        "Name": ...,
    }


# SupportedProductConfigTypeDef definition

class SupportedProductConfigTypeDef(TypedDict):
    Name: NotRequired[str],
    Args: NotRequired[Sequence[str]],
```

## SimpleScalingPolicyConfigurationTypeDef

```python
# SimpleScalingPolicyConfigurationTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import SimpleScalingPolicyConfigurationTypeDef


def get_value() -> SimpleScalingPolicyConfigurationTypeDef:
    return {
        "AdjustmentType": ...,
    }


# SimpleScalingPolicyConfigurationTypeDef definition

class SimpleScalingPolicyConfigurationTypeDef(TypedDict):
    ScalingAdjustment: int,
    AdjustmentType: NotRequired[AdjustmentTypeType],  # (1)
    CoolDown: NotRequired[int],
```

1. See [:material-code-brackets: AdjustmentTypeType](./literals.md#adjustmenttypetype) 
## ScriptBootstrapActionConfigTypeDef

```python
# ScriptBootstrapActionConfigTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ScriptBootstrapActionConfigTypeDef


def get_value() -> ScriptBootstrapActionConfigTypeDef:
    return {
        "Path": ...,
    }


# ScriptBootstrapActionConfigTypeDef definition

class ScriptBootstrapActionConfigTypeDef(TypedDict):
    Path: str,
    Args: NotRequired[Sequence[str]],
```

## SetKeepJobFlowAliveWhenNoStepsInputTypeDef

```python
# SetKeepJobFlowAliveWhenNoStepsInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import SetKeepJobFlowAliveWhenNoStepsInputTypeDef


def get_value() -> SetKeepJobFlowAliveWhenNoStepsInputTypeDef:
    return {
        "JobFlowIds": ...,
    }


# SetKeepJobFlowAliveWhenNoStepsInputTypeDef definition

class SetKeepJobFlowAliveWhenNoStepsInputTypeDef(TypedDict):
    JobFlowIds: Sequence[str],
    KeepJobFlowAliveWhenNoSteps: bool,
```

## SetTerminationProtectionInputTypeDef

```python
# SetTerminationProtectionInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import SetTerminationProtectionInputTypeDef


def get_value() -> SetTerminationProtectionInputTypeDef:
    return {
        "JobFlowIds": ...,
    }


# SetTerminationProtectionInputTypeDef definition

class SetTerminationProtectionInputTypeDef(TypedDict):
    JobFlowIds: Sequence[str],
    TerminationProtected: bool,
```

## SetUnhealthyNodeReplacementInputTypeDef

```python
# SetUnhealthyNodeReplacementInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import SetUnhealthyNodeReplacementInputTypeDef


def get_value() -> SetUnhealthyNodeReplacementInputTypeDef:
    return {
        "JobFlowIds": ...,
    }


# SetUnhealthyNodeReplacementInputTypeDef definition

class SetUnhealthyNodeReplacementInputTypeDef(TypedDict):
    JobFlowIds: Sequence[str],
    UnhealthyNodeReplacement: bool,
```

## SetVisibleToAllUsersInputTypeDef

```python
# SetVisibleToAllUsersInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import SetVisibleToAllUsersInputTypeDef


def get_value() -> SetVisibleToAllUsersInputTypeDef:
    return {
        "JobFlowIds": ...,
    }


# SetVisibleToAllUsersInputTypeDef definition

class SetVisibleToAllUsersInputTypeDef(TypedDict):
    JobFlowIds: Sequence[str],
    VisibleToAllUsers: bool,
```

## StepExecutionStatusDetailTypeDef

```python
# StepExecutionStatusDetailTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import StepExecutionStatusDetailTypeDef


def get_value() -> StepExecutionStatusDetailTypeDef:
    return {
        "State": ...,
    }


# StepExecutionStatusDetailTypeDef definition

class StepExecutionStatusDetailTypeDef(TypedDict):
    State: StepExecutionStateType,  # (1)
    CreationDateTime: datetime,
    StartDateTime: NotRequired[datetime],
    EndDateTime: NotRequired[datetime],
    LastStateChangeReason: NotRequired[str],
```

1. See [:material-code-brackets: StepExecutionStateType](./literals.md#stepexecutionstatetype) 
## StepStateChangeReasonTypeDef

```python
# StepStateChangeReasonTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import StepStateChangeReasonTypeDef


def get_value() -> StepStateChangeReasonTypeDef:
    return {
        "Code": ...,
    }


# StepStateChangeReasonTypeDef definition

class StepStateChangeReasonTypeDef(TypedDict):
    Code: NotRequired[StepStateChangeReasonCodeType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: StepStateChangeReasonCodeType](./literals.md#stepstatechangereasoncodetype) 
## StepTimelineTypeDef

```python
# StepTimelineTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import StepTimelineTypeDef


def get_value() -> StepTimelineTypeDef:
    return {
        "CreationDateTime": ...,
    }


# StepTimelineTypeDef definition

class StepTimelineTypeDef(TypedDict):
    CreationDateTime: NotRequired[datetime],
    StartDateTime: NotRequired[datetime],
    EndDateTime: NotRequired[datetime],
```

## StopNotebookExecutionInputTypeDef

```python
# StopNotebookExecutionInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import StopNotebookExecutionInputTypeDef


def get_value() -> StopNotebookExecutionInputTypeDef:
    return {
        "NotebookExecutionId": ...,
    }


# StopNotebookExecutionInputTypeDef definition

class StopNotebookExecutionInputTypeDef(TypedDict):
    NotebookExecutionId: str,
```

## TerminateJobFlowsInputTypeDef

```python
# TerminateJobFlowsInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import TerminateJobFlowsInputTypeDef


def get_value() -> TerminateJobFlowsInputTypeDef:
    return {
        "JobFlowIds": ...,
    }


# TerminateJobFlowsInputTypeDef definition

class TerminateJobFlowsInputTypeDef(TypedDict):
    JobFlowIds: Sequence[str],
```

## UpdateStudioInputTypeDef

```python
# UpdateStudioInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import UpdateStudioInputTypeDef


def get_value() -> UpdateStudioInputTypeDef:
    return {
        "StudioId": ...,
    }


# UpdateStudioInputTypeDef definition

class UpdateStudioInputTypeDef(TypedDict):
    StudioId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    SubnetIds: NotRequired[Sequence[str]],
    DefaultS3Location: NotRequired[str],
    EncryptionKeyArn: NotRequired[str],
```

## UpdateStudioSessionMappingInputTypeDef

```python
# UpdateStudioSessionMappingInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import UpdateStudioSessionMappingInputTypeDef


def get_value() -> UpdateStudioSessionMappingInputTypeDef:
    return {
        "StudioId": ...,
    }


# UpdateStudioSessionMappingInputTypeDef definition

class UpdateStudioSessionMappingInputTypeDef(TypedDict):
    StudioId: str,
    IdentityType: IdentityTypeType,  # (1)
    SessionPolicyArn: str,
    IdentityId: NotRequired[str],
    IdentityName: NotRequired[str],
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
## AddInstanceFleetOutputTypeDef

```python
# AddInstanceFleetOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import AddInstanceFleetOutputTypeDef


def get_value() -> AddInstanceFleetOutputTypeDef:
    return {
        "ClusterId": ...,
    }


# AddInstanceFleetOutputTypeDef definition

class AddInstanceFleetOutputTypeDef(TypedDict):
    ClusterId: str,
    InstanceFleetId: str,
    ClusterArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddInstanceGroupsOutputTypeDef

```python
# AddInstanceGroupsOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import AddInstanceGroupsOutputTypeDef


def get_value() -> AddInstanceGroupsOutputTypeDef:
    return {
        "JobFlowId": ...,
    }


# AddInstanceGroupsOutputTypeDef definition

class AddInstanceGroupsOutputTypeDef(TypedDict):
    JobFlowId: str,
    InstanceGroupIds: List[str],
    ClusterArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddJobFlowStepsOutputTypeDef

```python
# AddJobFlowStepsOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import AddJobFlowStepsOutputTypeDef


def get_value() -> AddJobFlowStepsOutputTypeDef:
    return {
        "StepIds": ...,
    }


# AddJobFlowStepsOutputTypeDef definition

class AddJobFlowStepsOutputTypeDef(TypedDict):
    StepIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSecurityConfigurationOutputTypeDef

```python
# CreateSecurityConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import CreateSecurityConfigurationOutputTypeDef


def get_value() -> CreateSecurityConfigurationOutputTypeDef:
    return {
        "Name": ...,
    }


# CreateSecurityConfigurationOutputTypeDef definition

class CreateSecurityConfigurationOutputTypeDef(TypedDict):
    Name: str,
    CreationDateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStudioOutputTypeDef

```python
# CreateStudioOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import CreateStudioOutputTypeDef


def get_value() -> CreateStudioOutputTypeDef:
    return {
        "StudioId": ...,
    }


# CreateStudioOutputTypeDef definition

class CreateStudioOutputTypeDef(TypedDict):
    StudioId: str,
    Url: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSecurityConfigurationOutputTypeDef

```python
# DescribeSecurityConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import DescribeSecurityConfigurationOutputTypeDef


def get_value() -> DescribeSecurityConfigurationOutputTypeDef:
    return {
        "Name": ...,
    }


# DescribeSecurityConfigurationOutputTypeDef definition

class DescribeSecurityConfigurationOutputTypeDef(TypedDict):
    Name: str,
    SecurityConfiguration: str,
    CreationDateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListReleaseLabelsOutputTypeDef

```python
# ListReleaseLabelsOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListReleaseLabelsOutputTypeDef


def get_value() -> ListReleaseLabelsOutputTypeDef:
    return {
        "ReleaseLabels": ...,
    }


# ListReleaseLabelsOutputTypeDef definition

class ListReleaseLabelsOutputTypeDef(TypedDict):
    ReleaseLabels: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModifyClusterOutputTypeDef

```python
# ModifyClusterOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ModifyClusterOutputTypeDef


def get_value() -> ModifyClusterOutputTypeDef:
    return {
        "StepConcurrencyLevel": ...,
    }


# ModifyClusterOutputTypeDef definition

class ModifyClusterOutputTypeDef(TypedDict):
    StepConcurrencyLevel: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RunJobFlowOutputTypeDef

```python
# RunJobFlowOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import RunJobFlowOutputTypeDef


def get_value() -> RunJobFlowOutputTypeDef:
    return {
        "JobFlowId": ...,
    }


# RunJobFlowOutputTypeDef definition

class RunJobFlowOutputTypeDef(TypedDict):
    JobFlowId: str,
    ClusterArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartNotebookExecutionOutputTypeDef

```python
# StartNotebookExecutionOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import StartNotebookExecutionOutputTypeDef


def get_value() -> StartNotebookExecutionOutputTypeDef:
    return {
        "NotebookExecutionId": ...,
    }


# StartNotebookExecutionOutputTypeDef definition

class StartNotebookExecutionOutputTypeDef(TypedDict):
    NotebookExecutionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddTagsInputTypeDef

```python
# AddTagsInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import AddTagsInputTypeDef


def get_value() -> AddTagsInputTypeDef:
    return {
        "ResourceId": ...,
    }


# AddTagsInputTypeDef definition

class AddTagsInputTypeDef(TypedDict):
    ResourceId: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateStudioInputTypeDef

```python
# CreateStudioInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import CreateStudioInputTypeDef


def get_value() -> CreateStudioInputTypeDef:
    return {
        "Name": ...,
    }


# CreateStudioInputTypeDef definition

class CreateStudioInputTypeDef(TypedDict):
    Name: str,
    AuthMode: AuthModeType,  # (1)
    VpcId: str,
    SubnetIds: Sequence[str],
    ServiceRole: str,
    WorkspaceSecurityGroupId: str,
    EngineSecurityGroupId: str,
    DefaultS3Location: str,
    Description: NotRequired[str],
    UserRole: NotRequired[str],
    IdpAuthUrl: NotRequired[str],
    IdpRelayStateParameterName: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    TrustedIdentityPropagationEnabled: NotRequired[bool],
    IdcUserAssignment: NotRequired[IdcUserAssignmentType],  # (3)
    IdcInstanceArn: NotRequired[str],
    EncryptionKeyArn: NotRequired[str],
```

1. See [:material-code-brackets: AuthModeType](./literals.md#authmodetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: IdcUserAssignmentType](./literals.md#idcuserassignmenttype) 
## StudioTypeDef

```python
# StudioTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import StudioTypeDef


def get_value() -> StudioTypeDef:
    return {
        "StudioId": ...,
    }


# StudioTypeDef definition

class StudioTypeDef(TypedDict):
    StudioId: NotRequired[str],
    StudioArn: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    AuthMode: NotRequired[AuthModeType],  # (1)
    VpcId: NotRequired[str],
    SubnetIds: NotRequired[List[str]],
    ServiceRole: NotRequired[str],
    UserRole: NotRequired[str],
    WorkspaceSecurityGroupId: NotRequired[str],
    EngineSecurityGroupId: NotRequired[str],
    Url: NotRequired[str],
    CreationTime: NotRequired[datetime],
    DefaultS3Location: NotRequired[str],
    IdpAuthUrl: NotRequired[str],
    IdpRelayStateParameterName: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (2)
    IdcInstanceArn: NotRequired[str],
    TrustedIdentityPropagationEnabled: NotRequired[bool],
    IdcUserAssignment: NotRequired[IdcUserAssignmentType],  # (3)
    EncryptionKeyArn: NotRequired[str],
```

1. See [:material-code-brackets: AuthModeType](./literals.md#authmodetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: IdcUserAssignmentType](./literals.md#idcuserassignmenttype) 
## AutoScalingPolicyStatusTypeDef

```python
# AutoScalingPolicyStatusTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import AutoScalingPolicyStatusTypeDef


def get_value() -> AutoScalingPolicyStatusTypeDef:
    return {
        "State": ...,
    }


# AutoScalingPolicyStatusTypeDef definition

class AutoScalingPolicyStatusTypeDef(TypedDict):
    State: NotRequired[AutoScalingPolicyStateType],  # (1)
    StateChangeReason: NotRequired[AutoScalingPolicyStateChangeReasonTypeDef],  # (2)
```

1. See [:material-code-brackets: AutoScalingPolicyStateType](./literals.md#autoscalingpolicystatetype) 
2. See [:material-code-braces: AutoScalingPolicyStateChangeReasonTypeDef](./type_defs.md#autoscalingpolicystatechangereasontypedef) 
## GetAutoTerminationPolicyOutputTypeDef

```python
# GetAutoTerminationPolicyOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import GetAutoTerminationPolicyOutputTypeDef


def get_value() -> GetAutoTerminationPolicyOutputTypeDef:
    return {
        "AutoTerminationPolicy": ...,
    }


# GetAutoTerminationPolicyOutputTypeDef definition

class GetAutoTerminationPolicyOutputTypeDef(TypedDict):
    AutoTerminationPolicy: AutoTerminationPolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AutoTerminationPolicyTypeDef](./type_defs.md#autoterminationpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutAutoTerminationPolicyInputTypeDef

```python
# PutAutoTerminationPolicyInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import PutAutoTerminationPolicyInputTypeDef


def get_value() -> PutAutoTerminationPolicyInputTypeDef:
    return {
        "ClusterId": ...,
    }


# PutAutoTerminationPolicyInputTypeDef definition

class PutAutoTerminationPolicyInputTypeDef(TypedDict):
    ClusterId: str,
    AutoTerminationPolicy: NotRequired[AutoTerminationPolicyTypeDef],  # (1)
```

1. See [:material-code-braces: AutoTerminationPolicyTypeDef](./type_defs.md#autoterminationpolicytypedef) 
## BlockPublicAccessConfigurationOutputTypeDef

```python
# BlockPublicAccessConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import BlockPublicAccessConfigurationOutputTypeDef


def get_value() -> BlockPublicAccessConfigurationOutputTypeDef:
    return {
        "BlockPublicSecurityGroupRules": ...,
    }


# BlockPublicAccessConfigurationOutputTypeDef definition

class BlockPublicAccessConfigurationOutputTypeDef(TypedDict):
    BlockPublicSecurityGroupRules: bool,
    PermittedPublicSecurityGroupRuleRanges: NotRequired[List[PortRangeTypeDef]],  # (1)
```

1. See [:material-code-braces: PortRangeTypeDef](./type_defs.md#portrangetypedef) 
## BlockPublicAccessConfigurationTypeDef

```python
# BlockPublicAccessConfigurationTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import BlockPublicAccessConfigurationTypeDef


def get_value() -> BlockPublicAccessConfigurationTypeDef:
    return {
        "BlockPublicSecurityGroupRules": ...,
    }


# BlockPublicAccessConfigurationTypeDef definition

class BlockPublicAccessConfigurationTypeDef(TypedDict):
    BlockPublicSecurityGroupRules: bool,
    PermittedPublicSecurityGroupRuleRanges: NotRequired[Sequence[PortRangeTypeDef]],  # (1)
```

1. See [:material-code-braces: PortRangeTypeDef](./type_defs.md#portrangetypedef) 
## BootstrapActionConfigOutputTypeDef

```python
# BootstrapActionConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import BootstrapActionConfigOutputTypeDef


def get_value() -> BootstrapActionConfigOutputTypeDef:
    return {
        "Name": ...,
    }


# BootstrapActionConfigOutputTypeDef definition

class BootstrapActionConfigOutputTypeDef(TypedDict):
    Name: str,
    ScriptBootstrapAction: ScriptBootstrapActionConfigOutputTypeDef,  # (1)
```

1. See [:material-code-braces: ScriptBootstrapActionConfigOutputTypeDef](./type_defs.md#scriptbootstrapactionconfigoutputtypedef) 
## CancelStepsOutputTypeDef

```python
# CancelStepsOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import CancelStepsOutputTypeDef


def get_value() -> CancelStepsOutputTypeDef:
    return {
        "CancelStepsInfoList": ...,
    }


# CancelStepsOutputTypeDef definition

class CancelStepsOutputTypeDef(TypedDict):
    CancelStepsInfoList: List[CancelStepsInfoTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CancelStepsInfoTypeDef](./type_defs.md#cancelstepsinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CloudWatchAlarmDefinitionOutputTypeDef

```python
# CloudWatchAlarmDefinitionOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import CloudWatchAlarmDefinitionOutputTypeDef


def get_value() -> CloudWatchAlarmDefinitionOutputTypeDef:
    return {
        "ComparisonOperator": ...,
    }


# CloudWatchAlarmDefinitionOutputTypeDef definition

class CloudWatchAlarmDefinitionOutputTypeDef(TypedDict):
    ComparisonOperator: ComparisonOperatorType,  # (1)
    MetricName: str,
    Period: int,
    Threshold: float,
    EvaluationPeriods: NotRequired[int],
    Namespace: NotRequired[str],
    Statistic: NotRequired[StatisticType],  # (2)
    Unit: NotRequired[UnitType],  # (3)
    Dimensions: NotRequired[List[MetricDimensionTypeDef]],  # (4)
```

1. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
2. See [:material-code-brackets: StatisticType](./literals.md#statistictype) 
3. See [:material-code-brackets: UnitType](./literals.md#unittype) 
4. See [:material-code-braces: MetricDimensionTypeDef](./type_defs.md#metricdimensiontypedef) 
## CloudWatchAlarmDefinitionTypeDef

```python
# CloudWatchAlarmDefinitionTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import CloudWatchAlarmDefinitionTypeDef


def get_value() -> CloudWatchAlarmDefinitionTypeDef:
    return {
        "ComparisonOperator": ...,
    }


# CloudWatchAlarmDefinitionTypeDef definition

class CloudWatchAlarmDefinitionTypeDef(TypedDict):
    ComparisonOperator: ComparisonOperatorType,  # (1)
    MetricName: str,
    Period: int,
    Threshold: float,
    EvaluationPeriods: NotRequired[int],
    Namespace: NotRequired[str],
    Statistic: NotRequired[StatisticType],  # (2)
    Unit: NotRequired[UnitType],  # (3)
    Dimensions: NotRequired[Sequence[MetricDimensionTypeDef]],  # (4)
```

1. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
2. See [:material-code-brackets: StatisticType](./literals.md#statistictype) 
3. See [:material-code-brackets: UnitType](./literals.md#unittype) 
4. See [:material-code-braces: MetricDimensionTypeDef](./type_defs.md#metricdimensiontypedef) 
## ClusterStatusTypeDef

```python
# ClusterStatusTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ClusterStatusTypeDef


def get_value() -> ClusterStatusTypeDef:
    return {
        "State": ...,
    }


# ClusterStatusTypeDef definition

class ClusterStatusTypeDef(TypedDict):
    State: NotRequired[ClusterStateType],  # (1)
    StateChangeReason: NotRequired[ClusterStateChangeReasonTypeDef],  # (2)
    Timeline: NotRequired[ClusterTimelineTypeDef],  # (3)
    ErrorDetails: NotRequired[List[ErrorDetailTypeDef]],  # (4)
```

1. See [:material-code-brackets: ClusterStateType](./literals.md#clusterstatetype) 
2. See [:material-code-braces: ClusterStateChangeReasonTypeDef](./type_defs.md#clusterstatechangereasontypedef) 
3. See [:material-code-braces: ClusterTimelineTypeDef](./type_defs.md#clustertimelinetypedef) 
4. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
## ListBootstrapActionsOutputTypeDef

```python
# ListBootstrapActionsOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListBootstrapActionsOutputTypeDef


def get_value() -> ListBootstrapActionsOutputTypeDef:
    return {
        "BootstrapActions": ...,
    }


# ListBootstrapActionsOutputTypeDef definition

class ListBootstrapActionsOutputTypeDef(TypedDict):
    BootstrapActions: List[CommandTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CommandTypeDef](./type_defs.md#commandtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ManagedScalingPolicyTypeDef

```python
# ManagedScalingPolicyTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ManagedScalingPolicyTypeDef


def get_value() -> ManagedScalingPolicyTypeDef:
    return {
        "ComputeLimits": ...,
    }


# ManagedScalingPolicyTypeDef definition

class ManagedScalingPolicyTypeDef(TypedDict):
    ComputeLimits: NotRequired[ComputeLimitsTypeDef],  # (1)
    UtilizationPerformanceIndex: NotRequired[int],
    ScalingStrategy: NotRequired[ScalingStrategyType],  # (2)
```

1. See [:material-code-braces: ComputeLimitsTypeDef](./type_defs.md#computelimitstypedef) 
2. See [:material-code-brackets: ScalingStrategyType](./literals.md#scalingstrategytype) 
## CredentialsTypeDef

```python
# CredentialsTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import CredentialsTypeDef


def get_value() -> CredentialsTypeDef:
    return {
        "UsernamePassword": ...,
    }


# CredentialsTypeDef definition

class CredentialsTypeDef(TypedDict):
    UsernamePassword: NotRequired[UsernamePasswordTypeDef],  # (1)
```

1. See [:material-code-braces: UsernamePasswordTypeDef](./type_defs.md#usernamepasswordtypedef) 
## DescribeClusterInputWaitExtraTypeDef

```python
# DescribeClusterInputWaitExtraTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import DescribeClusterInputWaitExtraTypeDef


def get_value() -> DescribeClusterInputWaitExtraTypeDef:
    return {
        "ClusterId": ...,
    }


# DescribeClusterInputWaitExtraTypeDef definition

class DescribeClusterInputWaitExtraTypeDef(TypedDict):
    ClusterId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeClusterInputWaitTypeDef

```python
# DescribeClusterInputWaitTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import DescribeClusterInputWaitTypeDef


def get_value() -> DescribeClusterInputWaitTypeDef:
    return {
        "ClusterId": ...,
    }


# DescribeClusterInputWaitTypeDef definition

class DescribeClusterInputWaitTypeDef(TypedDict):
    ClusterId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeStepInputWaitTypeDef

```python
# DescribeStepInputWaitTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import DescribeStepInputWaitTypeDef


def get_value() -> DescribeStepInputWaitTypeDef:
    return {
        "ClusterId": ...,
    }


# DescribeStepInputWaitTypeDef definition

class DescribeStepInputWaitTypeDef(TypedDict):
    ClusterId: str,
    StepId: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeJobFlowsInputTypeDef

```python
# DescribeJobFlowsInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import DescribeJobFlowsInputTypeDef


def get_value() -> DescribeJobFlowsInputTypeDef:
    return {
        "CreatedAfter": ...,
    }


# DescribeJobFlowsInputTypeDef definition

class DescribeJobFlowsInputTypeDef(TypedDict):
    CreatedAfter: NotRequired[TimestampTypeDef],
    CreatedBefore: NotRequired[TimestampTypeDef],
    JobFlowIds: NotRequired[Sequence[str]],
    JobFlowStates: NotRequired[Sequence[JobFlowExecutionStateType]],  # (1)
```

1. See [:material-code-brackets: JobFlowExecutionStateType](./literals.md#jobflowexecutionstatetype) 
## ListClustersInputTypeDef

```python
# ListClustersInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListClustersInputTypeDef


def get_value() -> ListClustersInputTypeDef:
    return {
        "CreatedAfter": ...,
    }


# ListClustersInputTypeDef definition

class ListClustersInputTypeDef(TypedDict):
    CreatedAfter: NotRequired[TimestampTypeDef],
    CreatedBefore: NotRequired[TimestampTypeDef],
    ClusterStates: NotRequired[Sequence[ClusterStateType]],  # (1)
    Marker: NotRequired[str],
```

1. See [:material-code-brackets: ClusterStateType](./literals.md#clusterstatetype) 
## ListNotebookExecutionsInputTypeDef

```python
# ListNotebookExecutionsInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListNotebookExecutionsInputTypeDef


def get_value() -> ListNotebookExecutionsInputTypeDef:
    return {
        "EditorId": ...,
    }


# ListNotebookExecutionsInputTypeDef definition

class ListNotebookExecutionsInputTypeDef(TypedDict):
    EditorId: NotRequired[str],
    Status: NotRequired[NotebookExecutionStatusType],  # (1)
    From: NotRequired[TimestampTypeDef],
    To: NotRequired[TimestampTypeDef],
    Marker: NotRequired[str],
    ExecutionEngineId: NotRequired[str],
```

1. See [:material-code-brackets: NotebookExecutionStatusType](./literals.md#notebookexecutionstatustype) 
## DescribeReleaseLabelOutputTypeDef

```python
# DescribeReleaseLabelOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import DescribeReleaseLabelOutputTypeDef


def get_value() -> DescribeReleaseLabelOutputTypeDef:
    return {
        "ReleaseLabel": ...,
    }


# DescribeReleaseLabelOutputTypeDef definition

class DescribeReleaseLabelOutputTypeDef(TypedDict):
    ReleaseLabel: str,
    Applications: List[SimplifiedApplicationTypeDef],  # (1)
    AvailableOSReleases: List[OSReleaseTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SimplifiedApplicationTypeDef](./type_defs.md#simplifiedapplicationtypedef) 
2. See [:material-code-braces: OSReleaseTypeDef](./type_defs.md#osreleasetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EbsBlockDeviceConfigTypeDef

```python
# EbsBlockDeviceConfigTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import EbsBlockDeviceConfigTypeDef


def get_value() -> EbsBlockDeviceConfigTypeDef:
    return {
        "VolumeSpecification": ...,
    }


# EbsBlockDeviceConfigTypeDef definition

class EbsBlockDeviceConfigTypeDef(TypedDict):
    VolumeSpecification: VolumeSpecificationTypeDef,  # (1)
    VolumesPerInstance: NotRequired[int],
```

1. See [:material-code-braces: VolumeSpecificationTypeDef](./type_defs.md#volumespecificationtypedef) 
## EbsBlockDeviceTypeDef

```python
# EbsBlockDeviceTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import EbsBlockDeviceTypeDef


def get_value() -> EbsBlockDeviceTypeDef:
    return {
        "VolumeSpecification": ...,
    }


# EbsBlockDeviceTypeDef definition

class EbsBlockDeviceTypeDef(TypedDict):
    VolumeSpecification: NotRequired[VolumeSpecificationTypeDef],  # (1)
    Device: NotRequired[str],
```

1. See [:material-code-braces: VolumeSpecificationTypeDef](./type_defs.md#volumespecificationtypedef) 
## GetStudioSessionMappingOutputTypeDef

```python
# GetStudioSessionMappingOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import GetStudioSessionMappingOutputTypeDef


def get_value() -> GetStudioSessionMappingOutputTypeDef:
    return {
        "SessionMapping": ...,
    }


# GetStudioSessionMappingOutputTypeDef definition

class GetStudioSessionMappingOutputTypeDef(TypedDict):
    SessionMapping: SessionMappingDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SessionMappingDetailTypeDef](./type_defs.md#sessionmappingdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HadoopJarStepConfigOutputTypeDef

```python
# HadoopJarStepConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import HadoopJarStepConfigOutputTypeDef


def get_value() -> HadoopJarStepConfigOutputTypeDef:
    return {
        "Properties": ...,
    }


# HadoopJarStepConfigOutputTypeDef definition

class HadoopJarStepConfigOutputTypeDef(TypedDict):
    Jar: str,
    Properties: NotRequired[List[KeyValueTypeDef]],  # (1)
    MainClass: NotRequired[str],
    Args: NotRequired[List[str]],
```

1. See [:material-code-braces: KeyValueTypeDef](./type_defs.md#keyvaluetypedef) 
## HadoopJarStepConfigTypeDef

```python
# HadoopJarStepConfigTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import HadoopJarStepConfigTypeDef


def get_value() -> HadoopJarStepConfigTypeDef:
    return {
        "Properties": ...,
    }


# HadoopJarStepConfigTypeDef definition

class HadoopJarStepConfigTypeDef(TypedDict):
    Jar: str,
    Properties: NotRequired[Sequence[KeyValueTypeDef]],  # (1)
    MainClass: NotRequired[str],
    Args: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: KeyValueTypeDef](./type_defs.md#keyvaluetypedef) 
## InstanceFleetStatusTypeDef

```python
# InstanceFleetStatusTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import InstanceFleetStatusTypeDef


def get_value() -> InstanceFleetStatusTypeDef:
    return {
        "State": ...,
    }


# InstanceFleetStatusTypeDef definition

class InstanceFleetStatusTypeDef(TypedDict):
    State: NotRequired[InstanceFleetStateType],  # (1)
    StateChangeReason: NotRequired[InstanceFleetStateChangeReasonTypeDef],  # (2)
    Timeline: NotRequired[InstanceFleetTimelineTypeDef],  # (3)
```

1. See [:material-code-brackets: InstanceFleetStateType](./literals.md#instancefleetstatetype) 
2. See [:material-code-braces: InstanceFleetStateChangeReasonTypeDef](./type_defs.md#instancefleetstatechangereasontypedef) 
3. See [:material-code-braces: InstanceFleetTimelineTypeDef](./type_defs.md#instancefleettimelinetypedef) 
## InstanceGroupStatusTypeDef

```python
# InstanceGroupStatusTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import InstanceGroupStatusTypeDef


def get_value() -> InstanceGroupStatusTypeDef:
    return {
        "State": ...,
    }


# InstanceGroupStatusTypeDef definition

class InstanceGroupStatusTypeDef(TypedDict):
    State: NotRequired[InstanceGroupStateType],  # (1)
    StateChangeReason: NotRequired[InstanceGroupStateChangeReasonTypeDef],  # (2)
    Timeline: NotRequired[InstanceGroupTimelineTypeDef],  # (3)
```

1. See [:material-code-brackets: InstanceGroupStateType](./literals.md#instancegroupstatetype) 
2. See [:material-code-braces: InstanceGroupStateChangeReasonTypeDef](./type_defs.md#instancegroupstatechangereasontypedef) 
3. See [:material-code-braces: InstanceGroupTimelineTypeDef](./type_defs.md#instancegrouptimelinetypedef) 
## ShrinkPolicyOutputTypeDef

```python
# ShrinkPolicyOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ShrinkPolicyOutputTypeDef


def get_value() -> ShrinkPolicyOutputTypeDef:
    return {
        "DecommissionTimeout": ...,
    }


# ShrinkPolicyOutputTypeDef definition

class ShrinkPolicyOutputTypeDef(TypedDict):
    DecommissionTimeout: NotRequired[int],
    InstanceResizePolicy: NotRequired[InstanceResizePolicyOutputTypeDef],  # (1)
```

1. See [:material-code-braces: InstanceResizePolicyOutputTypeDef](./type_defs.md#instanceresizepolicyoutputtypedef) 
## InstanceStatusTypeDef

```python
# InstanceStatusTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import InstanceStatusTypeDef


def get_value() -> InstanceStatusTypeDef:
    return {
        "State": ...,
    }


# InstanceStatusTypeDef definition

class InstanceStatusTypeDef(TypedDict):
    State: NotRequired[InstanceStateType],  # (1)
    StateChangeReason: NotRequired[InstanceStateChangeReasonTypeDef],  # (2)
    Timeline: NotRequired[InstanceTimelineTypeDef],  # (3)
```

1. See [:material-code-brackets: InstanceStateType](./literals.md#instancestatetype) 
2. See [:material-code-braces: InstanceStateChangeReasonTypeDef](./type_defs.md#instancestatechangereasontypedef) 
3. See [:material-code-braces: InstanceTimelineTypeDef](./type_defs.md#instancetimelinetypedef) 
## JobFlowInstancesDetailTypeDef

```python
# JobFlowInstancesDetailTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import JobFlowInstancesDetailTypeDef


def get_value() -> JobFlowInstancesDetailTypeDef:
    return {
        "MasterInstanceType": ...,
    }


# JobFlowInstancesDetailTypeDef definition

class JobFlowInstancesDetailTypeDef(TypedDict):
    MasterInstanceType: str,
    SlaveInstanceType: str,
    InstanceCount: int,
    MasterPublicDnsName: NotRequired[str],
    MasterInstanceId: NotRequired[str],
    InstanceGroups: NotRequired[List[InstanceGroupDetailTypeDef]],  # (1)
    NormalizedInstanceHours: NotRequired[int],
    Ec2KeyName: NotRequired[str],
    Ec2SubnetId: NotRequired[str],
    Placement: NotRequired[PlacementTypeOutputTypeDef],  # (2)
    KeepJobFlowAliveWhenNoSteps: NotRequired[bool],
    TerminationProtected: NotRequired[bool],
    UnhealthyNodeReplacement: NotRequired[bool],
    HadoopVersion: NotRequired[str],
```

1. See [:material-code-braces: InstanceGroupDetailTypeDef](./type_defs.md#instancegroupdetailtypedef) 
2. See [:material-code-braces: PlacementTypeOutputTypeDef](./type_defs.md#placementtypeoutputtypedef) 
## ListBootstrapActionsInputPaginateTypeDef

```python
# ListBootstrapActionsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListBootstrapActionsInputPaginateTypeDef


def get_value() -> ListBootstrapActionsInputPaginateTypeDef:
    return {
        "ClusterId": ...,
    }


# ListBootstrapActionsInputPaginateTypeDef definition

class ListBootstrapActionsInputPaginateTypeDef(TypedDict):
    ClusterId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListClustersInputPaginateTypeDef

```python
# ListClustersInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListClustersInputPaginateTypeDef


def get_value() -> ListClustersInputPaginateTypeDef:
    return {
        "CreatedAfter": ...,
    }


# ListClustersInputPaginateTypeDef definition

class ListClustersInputPaginateTypeDef(TypedDict):
    CreatedAfter: NotRequired[TimestampTypeDef],
    CreatedBefore: NotRequired[TimestampTypeDef],
    ClusterStates: NotRequired[Sequence[ClusterStateType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ClusterStateType](./literals.md#clusterstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInstanceFleetsInputPaginateTypeDef

```python
# ListInstanceFleetsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListInstanceFleetsInputPaginateTypeDef


def get_value() -> ListInstanceFleetsInputPaginateTypeDef:
    return {
        "ClusterId": ...,
    }


# ListInstanceFleetsInputPaginateTypeDef definition

class ListInstanceFleetsInputPaginateTypeDef(TypedDict):
    ClusterId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInstanceGroupsInputPaginateTypeDef

```python
# ListInstanceGroupsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListInstanceGroupsInputPaginateTypeDef


def get_value() -> ListInstanceGroupsInputPaginateTypeDef:
    return {
        "ClusterId": ...,
    }


# ListInstanceGroupsInputPaginateTypeDef definition

class ListInstanceGroupsInputPaginateTypeDef(TypedDict):
    ClusterId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInstancesInputPaginateTypeDef

```python
# ListInstancesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListInstancesInputPaginateTypeDef


def get_value() -> ListInstancesInputPaginateTypeDef:
    return {
        "ClusterId": ...,
    }


# ListInstancesInputPaginateTypeDef definition

class ListInstancesInputPaginateTypeDef(TypedDict):
    ClusterId: str,
    InstanceGroupId: NotRequired[str],
    InstanceGroupTypes: NotRequired[Sequence[InstanceGroupTypeType]],  # (1)
    InstanceFleetId: NotRequired[str],
    InstanceFleetType: NotRequired[InstanceFleetTypeType],  # (2)
    InstanceStates: NotRequired[Sequence[InstanceStateType]],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: InstanceGroupTypeType](./literals.md#instancegrouptypetype) 
2. See [:material-code-brackets: InstanceFleetTypeType](./literals.md#instancefleettypetype) 
3. See [:material-code-brackets: InstanceStateType](./literals.md#instancestatetype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNotebookExecutionsInputPaginateTypeDef

```python
# ListNotebookExecutionsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListNotebookExecutionsInputPaginateTypeDef


def get_value() -> ListNotebookExecutionsInputPaginateTypeDef:
    return {
        "EditorId": ...,
    }


# ListNotebookExecutionsInputPaginateTypeDef definition

class ListNotebookExecutionsInputPaginateTypeDef(TypedDict):
    EditorId: NotRequired[str],
    Status: NotRequired[NotebookExecutionStatusType],  # (1)
    From: NotRequired[TimestampTypeDef],
    To: NotRequired[TimestampTypeDef],
    ExecutionEngineId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: NotebookExecutionStatusType](./literals.md#notebookexecutionstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSecurityConfigurationsInputPaginateTypeDef

```python
# ListSecurityConfigurationsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListSecurityConfigurationsInputPaginateTypeDef


def get_value() -> ListSecurityConfigurationsInputPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListSecurityConfigurationsInputPaginateTypeDef definition

class ListSecurityConfigurationsInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStepsInputPaginateTypeDef

```python
# ListStepsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListStepsInputPaginateTypeDef


def get_value() -> ListStepsInputPaginateTypeDef:
    return {
        "ClusterId": ...,
    }


# ListStepsInputPaginateTypeDef definition

class ListStepsInputPaginateTypeDef(TypedDict):
    ClusterId: str,
    StepStates: NotRequired[Sequence[StepStateType]],  # (1)
    StepIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: StepStateType](./literals.md#stepstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStudioSessionMappingsInputPaginateTypeDef

```python
# ListStudioSessionMappingsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListStudioSessionMappingsInputPaginateTypeDef


def get_value() -> ListStudioSessionMappingsInputPaginateTypeDef:
    return {
        "StudioId": ...,
    }


# ListStudioSessionMappingsInputPaginateTypeDef definition

class ListStudioSessionMappingsInputPaginateTypeDef(TypedDict):
    StudioId: NotRequired[str],
    IdentityType: NotRequired[IdentityTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStudiosInputPaginateTypeDef

```python
# ListStudiosInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListStudiosInputPaginateTypeDef


def get_value() -> ListStudiosInputPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListStudiosInputPaginateTypeDef definition

class ListStudiosInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListReleaseLabelsInputTypeDef

```python
# ListReleaseLabelsInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListReleaseLabelsInputTypeDef


def get_value() -> ListReleaseLabelsInputTypeDef:
    return {
        "Filters": ...,
    }


# ListReleaseLabelsInputTypeDef definition

class ListReleaseLabelsInputTypeDef(TypedDict):
    Filters: NotRequired[ReleaseLabelFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ReleaseLabelFilterTypeDef](./type_defs.md#releaselabelfiltertypedef) 
## ListSecurityConfigurationsOutputTypeDef

```python
# ListSecurityConfigurationsOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListSecurityConfigurationsOutputTypeDef


def get_value() -> ListSecurityConfigurationsOutputTypeDef:
    return {
        "SecurityConfigurations": ...,
    }


# ListSecurityConfigurationsOutputTypeDef definition

class ListSecurityConfigurationsOutputTypeDef(TypedDict):
    SecurityConfigurations: List[SecurityConfigurationSummaryTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SecurityConfigurationSummaryTypeDef](./type_defs.md#securityconfigurationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStudioSessionMappingsOutputTypeDef

```python
# ListStudioSessionMappingsOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListStudioSessionMappingsOutputTypeDef


def get_value() -> ListStudioSessionMappingsOutputTypeDef:
    return {
        "SessionMappings": ...,
    }


# ListStudioSessionMappingsOutputTypeDef definition

class ListStudioSessionMappingsOutputTypeDef(TypedDict):
    SessionMappings: List[SessionMappingSummaryTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SessionMappingSummaryTypeDef](./type_defs.md#sessionmappingsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStudiosOutputTypeDef

```python
# ListStudiosOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListStudiosOutputTypeDef


def get_value() -> ListStudiosOutputTypeDef:
    return {
        "Studios": ...,
    }


# ListStudiosOutputTypeDef definition

class ListStudiosOutputTypeDef(TypedDict):
    Studios: List[StudioSummaryTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StudioSummaryTypeDef](./type_defs.md#studiosummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSupportedInstanceTypesOutputTypeDef

```python
# ListSupportedInstanceTypesOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListSupportedInstanceTypesOutputTypeDef


def get_value() -> ListSupportedInstanceTypesOutputTypeDef:
    return {
        "SupportedInstanceTypes": ...,
    }


# ListSupportedInstanceTypesOutputTypeDef definition

class ListSupportedInstanceTypesOutputTypeDef(TypedDict):
    SupportedInstanceTypes: List[SupportedInstanceTypeTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SupportedInstanceTypeTypeDef](./type_defs.md#supportedinstancetypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NotebookExecutionSummaryTypeDef

```python
# NotebookExecutionSummaryTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import NotebookExecutionSummaryTypeDef


def get_value() -> NotebookExecutionSummaryTypeDef:
    return {
        "NotebookExecutionId": ...,
    }


# NotebookExecutionSummaryTypeDef definition

class NotebookExecutionSummaryTypeDef(TypedDict):
    NotebookExecutionId: NotRequired[str],
    EditorId: NotRequired[str],
    NotebookExecutionName: NotRequired[str],
    Status: NotRequired[NotebookExecutionStatusType],  # (1)
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    NotebookS3Location: NotRequired[NotebookS3LocationForOutputTypeDef],  # (2)
    ExecutionEngineId: NotRequired[str],
```

1. See [:material-code-brackets: NotebookExecutionStatusType](./literals.md#notebookexecutionstatustype) 
2. See [:material-code-braces: NotebookS3LocationForOutputTypeDef](./type_defs.md#notebooks3locationforoutputtypedef) 
## NotebookExecutionTypeDef

```python
# NotebookExecutionTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import NotebookExecutionTypeDef


def get_value() -> NotebookExecutionTypeDef:
    return {
        "NotebookExecutionId": ...,
    }


# NotebookExecutionTypeDef definition

class NotebookExecutionTypeDef(TypedDict):
    NotebookExecutionId: NotRequired[str],
    EditorId: NotRequired[str],
    ExecutionEngine: NotRequired[ExecutionEngineConfigTypeDef],  # (1)
    NotebookExecutionName: NotRequired[str],
    NotebookParams: NotRequired[str],
    Status: NotRequired[NotebookExecutionStatusType],  # (2)
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    Arn: NotRequired[str],
    OutputNotebookURI: NotRequired[str],
    LastStateChangeReason: NotRequired[str],
    NotebookInstanceSecurityGroupId: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (3)
    NotebookS3Location: NotRequired[NotebookS3LocationForOutputTypeDef],  # (4)
    OutputNotebookS3Location: NotRequired[OutputNotebookS3LocationForOutputTypeDef],  # (5)
    OutputNotebookFormat: NotRequired[OutputNotebookFormatType],  # (6)
    EnvironmentVariables: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: ExecutionEngineConfigTypeDef](./type_defs.md#executionengineconfigtypedef) 
2. See [:material-code-brackets: NotebookExecutionStatusType](./literals.md#notebookexecutionstatustype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: NotebookS3LocationForOutputTypeDef](./type_defs.md#notebooks3locationforoutputtypedef) 
5. See [:material-code-braces: OutputNotebookS3LocationForOutputTypeDef](./type_defs.md#outputnotebooks3locationforoutputtypedef) 
6. See [:material-code-brackets: OutputNotebookFormatType](./literals.md#outputnotebookformattype) 
## OnDemandProvisioningSpecificationTypeDef

```python
# OnDemandProvisioningSpecificationTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import OnDemandProvisioningSpecificationTypeDef


def get_value() -> OnDemandProvisioningSpecificationTypeDef:
    return {
        "AllocationStrategy": ...,
    }


# OnDemandProvisioningSpecificationTypeDef definition

class OnDemandProvisioningSpecificationTypeDef(TypedDict):
    AllocationStrategy: OnDemandProvisioningAllocationStrategyType,  # (1)
    CapacityReservationOptions: NotRequired[OnDemandCapacityReservationOptionsTypeDef],  # (2)
```

1. See [:material-code-brackets: OnDemandProvisioningAllocationStrategyType](./literals.md#ondemandprovisioningallocationstrategytype) 
2. See [:material-code-braces: OnDemandCapacityReservationOptionsTypeDef](./type_defs.md#ondemandcapacityreservationoptionstypedef) 
## OnDemandResizingSpecificationTypeDef

```python
# OnDemandResizingSpecificationTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import OnDemandResizingSpecificationTypeDef


def get_value() -> OnDemandResizingSpecificationTypeDef:
    return {
        "TimeoutDurationMinutes": ...,
    }


# OnDemandResizingSpecificationTypeDef definition

class OnDemandResizingSpecificationTypeDef(TypedDict):
    TimeoutDurationMinutes: NotRequired[int],
    AllocationStrategy: NotRequired[OnDemandProvisioningAllocationStrategyType],  # (1)
    CapacityReservationOptions: NotRequired[OnDemandCapacityReservationOptionsTypeDef],  # (2)
```

1. See [:material-code-brackets: OnDemandProvisioningAllocationStrategyType](./literals.md#ondemandprovisioningallocationstrategytype) 
2. See [:material-code-braces: OnDemandCapacityReservationOptionsTypeDef](./type_defs.md#ondemandcapacityreservationoptionstypedef) 
## StartNotebookExecutionInputTypeDef

```python
# StartNotebookExecutionInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import StartNotebookExecutionInputTypeDef


def get_value() -> StartNotebookExecutionInputTypeDef:
    return {
        "ExecutionEngine": ...,
    }


# StartNotebookExecutionInputTypeDef definition

class StartNotebookExecutionInputTypeDef(TypedDict):
    ExecutionEngine: ExecutionEngineConfigTypeDef,  # (1)
    ServiceRole: str,
    EditorId: NotRequired[str],
    RelativePath: NotRequired[str],
    NotebookExecutionName: NotRequired[str],
    NotebookParams: NotRequired[str],
    NotebookInstanceSecurityGroupId: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    NotebookS3Location: NotRequired[NotebookS3LocationFromInputTypeDef],  # (3)
    OutputNotebookS3Location: NotRequired[OutputNotebookS3LocationFromInputTypeDef],  # (4)
    OutputNotebookFormat: NotRequired[OutputNotebookFormatType],  # (5)
    EnvironmentVariables: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ExecutionEngineConfigTypeDef](./type_defs.md#executionengineconfigtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: NotebookS3LocationFromInputTypeDef](./type_defs.md#notebooks3locationfrominputtypedef) 
4. See [:material-code-braces: OutputNotebookS3LocationFromInputTypeDef](./type_defs.md#outputnotebooks3locationfrominputtypedef) 
5. See [:material-code-brackets: OutputNotebookFormatType](./literals.md#outputnotebookformattype) 
## ScalingActionTypeDef

```python
# ScalingActionTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ScalingActionTypeDef


def get_value() -> ScalingActionTypeDef:
    return {
        "Market": ...,
    }


# ScalingActionTypeDef definition

class ScalingActionTypeDef(TypedDict):
    SimpleScalingPolicyConfiguration: SimpleScalingPolicyConfigurationTypeDef,  # (2)
    Market: NotRequired[MarketTypeType],  # (1)
```

1. See [:material-code-brackets: MarketTypeType](./literals.md#markettypetype) 
2. See [:material-code-braces: SimpleScalingPolicyConfigurationTypeDef](./type_defs.md#simplescalingpolicyconfigurationtypedef) 
## StepStatusTypeDef

```python
# StepStatusTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import StepStatusTypeDef


def get_value() -> StepStatusTypeDef:
    return {
        "State": ...,
    }


# StepStatusTypeDef definition

class StepStatusTypeDef(TypedDict):
    State: NotRequired[StepStateType],  # (1)
    StateChangeReason: NotRequired[StepStateChangeReasonTypeDef],  # (2)
    FailureDetails: NotRequired[FailureDetailsTypeDef],  # (3)
    Timeline: NotRequired[StepTimelineTypeDef],  # (4)
```

1. See [:material-code-brackets: StepStateType](./literals.md#stepstatetype) 
2. See [:material-code-braces: StepStateChangeReasonTypeDef](./type_defs.md#stepstatechangereasontypedef) 
3. See [:material-code-braces: FailureDetailsTypeDef](./type_defs.md#failuredetailstypedef) 
4. See [:material-code-braces: StepTimelineTypeDef](./type_defs.md#steptimelinetypedef) 
## DescribeStudioOutputTypeDef

```python
# DescribeStudioOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import DescribeStudioOutputTypeDef


def get_value() -> DescribeStudioOutputTypeDef:
    return {
        "Studio": ...,
    }


# DescribeStudioOutputTypeDef definition

class DescribeStudioOutputTypeDef(TypedDict):
    Studio: StudioTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StudioTypeDef](./type_defs.md#studiotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBlockPublicAccessConfigurationOutputTypeDef

```python
# GetBlockPublicAccessConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import GetBlockPublicAccessConfigurationOutputTypeDef


def get_value() -> GetBlockPublicAccessConfigurationOutputTypeDef:
    return {
        "BlockPublicAccessConfiguration": ...,
    }


# GetBlockPublicAccessConfigurationOutputTypeDef definition

class GetBlockPublicAccessConfigurationOutputTypeDef(TypedDict):
    BlockPublicAccessConfiguration: BlockPublicAccessConfigurationOutputTypeDef,  # (1)
    BlockPublicAccessConfigurationMetadata: BlockPublicAccessConfigurationMetadataTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BlockPublicAccessConfigurationOutputTypeDef](./type_defs.md#blockpublicaccessconfigurationoutputtypedef) 
2. See [:material-code-braces: BlockPublicAccessConfigurationMetadataTypeDef](./type_defs.md#blockpublicaccessconfigurationmetadatatypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BootstrapActionDetailTypeDef

```python
# BootstrapActionDetailTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import BootstrapActionDetailTypeDef


def get_value() -> BootstrapActionDetailTypeDef:
    return {
        "BootstrapActionConfig": ...,
    }


# BootstrapActionDetailTypeDef definition

class BootstrapActionDetailTypeDef(TypedDict):
    BootstrapActionConfig: NotRequired[BootstrapActionConfigOutputTypeDef],  # (1)
```

1. See [:material-code-braces: BootstrapActionConfigOutputTypeDef](./type_defs.md#bootstrapactionconfigoutputtypedef) 
## ScalingTriggerOutputTypeDef

```python
# ScalingTriggerOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ScalingTriggerOutputTypeDef


def get_value() -> ScalingTriggerOutputTypeDef:
    return {
        "CloudWatchAlarmDefinition": ...,
    }


# ScalingTriggerOutputTypeDef definition

class ScalingTriggerOutputTypeDef(TypedDict):
    CloudWatchAlarmDefinition: CloudWatchAlarmDefinitionOutputTypeDef,  # (1)
```

1. See [:material-code-braces: CloudWatchAlarmDefinitionOutputTypeDef](./type_defs.md#cloudwatchalarmdefinitionoutputtypedef) 
## ClusterSummaryTypeDef

```python
# ClusterSummaryTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ClusterSummaryTypeDef


def get_value() -> ClusterSummaryTypeDef:
    return {
        "Id": ...,
    }


# ClusterSummaryTypeDef definition

class ClusterSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Status: NotRequired[ClusterStatusTypeDef],  # (1)
    NormalizedInstanceHours: NotRequired[int],
    ClusterArn: NotRequired[str],
    OutpostArn: NotRequired[str],
```

1. See [:material-code-braces: ClusterStatusTypeDef](./type_defs.md#clusterstatustypedef) 
## ClusterTypeDef

```python
# ClusterTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ClusterTypeDef


def get_value() -> ClusterTypeDef:
    return {
        "Id": ...,
    }


# ClusterTypeDef definition

class ClusterTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Status: NotRequired[ClusterStatusTypeDef],  # (1)
    Ec2InstanceAttributes: NotRequired[Ec2InstanceAttributesTypeDef],  # (2)
    InstanceCollectionType: NotRequired[InstanceCollectionTypeType],  # (3)
    LogUri: NotRequired[str],
    LogEncryptionKmsKeyId: NotRequired[str],
    RequestedAmiVersion: NotRequired[str],
    RunningAmiVersion: NotRequired[str],
    ReleaseLabel: NotRequired[str],
    AutoTerminate: NotRequired[bool],
    TerminationProtected: NotRequired[bool],
    UnhealthyNodeReplacement: NotRequired[bool],
    VisibleToAllUsers: NotRequired[bool],
    Applications: NotRequired[List[ApplicationOutputTypeDef]],  # (4)
    Tags: NotRequired[List[TagTypeDef]],  # (5)
    ServiceRole: NotRequired[str],
    NormalizedInstanceHours: NotRequired[int],
    MasterPublicDnsName: NotRequired[str],
    Configurations: NotRequired[List[ConfigurationOutputTypeDef]],  # (6)
    SecurityConfiguration: NotRequired[str],
    AutoScalingRole: NotRequired[str],
    ScaleDownBehavior: NotRequired[ScaleDownBehaviorType],  # (7)
    CustomAmiId: NotRequired[str],
    EbsRootVolumeSize: NotRequired[int],
    RepoUpgradeOnBoot: NotRequired[RepoUpgradeOnBootType],  # (8)
    KerberosAttributes: NotRequired[KerberosAttributesTypeDef],  # (9)
    ClusterArn: NotRequired[str],
    OutpostArn: NotRequired[str],
    StepConcurrencyLevel: NotRequired[int],
    PlacementGroups: NotRequired[List[PlacementGroupConfigTypeDef]],  # (10)
    OSReleaseLabel: NotRequired[str],
    EbsRootVolumeIops: NotRequired[int],
    EbsRootVolumeThroughput: NotRequired[int],
```

1. See [:material-code-braces: ClusterStatusTypeDef](./type_defs.md#clusterstatustypedef) 
2. See [:material-code-braces: Ec2InstanceAttributesTypeDef](./type_defs.md#ec2instanceattributestypedef) 
3. See [:material-code-brackets: InstanceCollectionTypeType](./literals.md#instancecollectiontypetype) 
4. See [:material-code-braces: ApplicationOutputTypeDef](./type_defs.md#applicationoutputtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: ConfigurationOutputTypeDef](./type_defs.md#configurationoutputtypedef) 
7. See [:material-code-brackets: ScaleDownBehaviorType](./literals.md#scaledownbehaviortype) 
8. See [:material-code-brackets: RepoUpgradeOnBootType](./literals.md#repoupgradeonboottype) 
9. See [:material-code-braces: KerberosAttributesTypeDef](./type_defs.md#kerberosattributestypedef) 
10. See [:material-code-braces: PlacementGroupConfigTypeDef](./type_defs.md#placementgroupconfigtypedef) 
## GetManagedScalingPolicyOutputTypeDef

```python
# GetManagedScalingPolicyOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import GetManagedScalingPolicyOutputTypeDef


def get_value() -> GetManagedScalingPolicyOutputTypeDef:
    return {
        "ManagedScalingPolicy": ...,
    }


# GetManagedScalingPolicyOutputTypeDef definition

class GetManagedScalingPolicyOutputTypeDef(TypedDict):
    ManagedScalingPolicy: ManagedScalingPolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ManagedScalingPolicyTypeDef](./type_defs.md#managedscalingpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutManagedScalingPolicyInputTypeDef

```python
# PutManagedScalingPolicyInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import PutManagedScalingPolicyInputTypeDef


def get_value() -> PutManagedScalingPolicyInputTypeDef:
    return {
        "ClusterId": ...,
    }


# PutManagedScalingPolicyInputTypeDef definition

class PutManagedScalingPolicyInputTypeDef(TypedDict):
    ClusterId: str,
    ManagedScalingPolicy: ManagedScalingPolicyTypeDef,  # (1)
```

1. See [:material-code-braces: ManagedScalingPolicyTypeDef](./type_defs.md#managedscalingpolicytypedef) 
## GetClusterSessionCredentialsOutputTypeDef

```python
# GetClusterSessionCredentialsOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import GetClusterSessionCredentialsOutputTypeDef


def get_value() -> GetClusterSessionCredentialsOutputTypeDef:
    return {
        "Credentials": ...,
    }


# GetClusterSessionCredentialsOutputTypeDef definition

class GetClusterSessionCredentialsOutputTypeDef(TypedDict):
    Credentials: CredentialsTypeDef,  # (1)
    ExpiresAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CredentialsTypeDef](./type_defs.md#credentialstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EbsConfigurationTypeDef

```python
# EbsConfigurationTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import EbsConfigurationTypeDef


def get_value() -> EbsConfigurationTypeDef:
    return {
        "EbsBlockDeviceConfigs": ...,
    }


# EbsConfigurationTypeDef definition

class EbsConfigurationTypeDef(TypedDict):
    EbsBlockDeviceConfigs: NotRequired[Sequence[EbsBlockDeviceConfigTypeDef]],  # (1)
    EbsOptimized: NotRequired[bool],
```

1. See [:material-code-braces: EbsBlockDeviceConfigTypeDef](./type_defs.md#ebsblockdeviceconfigtypedef) 
## InstanceTypeSpecificationPaginatorTypeDef

```python
# InstanceTypeSpecificationPaginatorTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import InstanceTypeSpecificationPaginatorTypeDef


def get_value() -> InstanceTypeSpecificationPaginatorTypeDef:
    return {
        "InstanceType": ...,
    }


# InstanceTypeSpecificationPaginatorTypeDef definition

class InstanceTypeSpecificationPaginatorTypeDef(TypedDict):
    InstanceType: NotRequired[str],
    WeightedCapacity: NotRequired[int],
    BidPrice: NotRequired[str],
    BidPriceAsPercentageOfOnDemandPrice: NotRequired[float],
    Configurations: NotRequired[List[ConfigurationPaginatorTypeDef]],  # (1)
    EbsBlockDevices: NotRequired[List[EbsBlockDeviceTypeDef]],  # (2)
    EbsOptimized: NotRequired[bool],
    CustomAmiId: NotRequired[str],
    Priority: NotRequired[float],
```

1. See [:material-code-braces: ConfigurationPaginatorTypeDef](./type_defs.md#configurationpaginatortypedef) 
2. See [:material-code-braces: EbsBlockDeviceTypeDef](./type_defs.md#ebsblockdevicetypedef) 
## InstanceTypeSpecificationTypeDef

```python
# InstanceTypeSpecificationTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import InstanceTypeSpecificationTypeDef


def get_value() -> InstanceTypeSpecificationTypeDef:
    return {
        "InstanceType": ...,
    }


# InstanceTypeSpecificationTypeDef definition

class InstanceTypeSpecificationTypeDef(TypedDict):
    InstanceType: NotRequired[str],
    WeightedCapacity: NotRequired[int],
    BidPrice: NotRequired[str],
    BidPriceAsPercentageOfOnDemandPrice: NotRequired[float],
    Configurations: NotRequired[List[ConfigurationOutputTypeDef]],  # (1)
    EbsBlockDevices: NotRequired[List[EbsBlockDeviceTypeDef]],  # (2)
    EbsOptimized: NotRequired[bool],
    CustomAmiId: NotRequired[str],
    Priority: NotRequired[float],
```

1. See [:material-code-braces: ConfigurationOutputTypeDef](./type_defs.md#configurationoutputtypedef) 
2. See [:material-code-braces: EbsBlockDeviceTypeDef](./type_defs.md#ebsblockdevicetypedef) 
## StepConfigOutputTypeDef

```python
# StepConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import StepConfigOutputTypeDef


def get_value() -> StepConfigOutputTypeDef:
    return {
        "Name": ...,
    }


# StepConfigOutputTypeDef definition

class StepConfigOutputTypeDef(TypedDict):
    Name: str,
    HadoopJarStep: HadoopJarStepConfigOutputTypeDef,  # (2)
    ActionOnFailure: NotRequired[ActionOnFailureType],  # (1)
```

1. See [:material-code-brackets: ActionOnFailureType](./literals.md#actiononfailuretype) 
2. See [:material-code-braces: HadoopJarStepConfigOutputTypeDef](./type_defs.md#hadoopjarstepconfigoutputtypedef) 
## ShrinkPolicyTypeDef

```python
# ShrinkPolicyTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ShrinkPolicyTypeDef


def get_value() -> ShrinkPolicyTypeDef:
    return {
        "DecommissionTimeout": ...,
    }


# ShrinkPolicyTypeDef definition

class ShrinkPolicyTypeDef(TypedDict):
    DecommissionTimeout: NotRequired[int],
    InstanceResizePolicy: NotRequired[InstanceResizePolicyUnionTypeDef],  # (1)
```

1. See [:material-code-braces: InstanceResizePolicyTypeDef](./type_defs.md#instanceresizepolicytypedef) [:material-code-braces: InstanceResizePolicyOutputTypeDef](./type_defs.md#instanceresizepolicyoutputtypedef) 
## InstanceTypeDef

```python
# InstanceTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import InstanceTypeDef


def get_value() -> InstanceTypeDef:
    return {
        "Id": ...,
    }


# InstanceTypeDef definition

class InstanceTypeDef(TypedDict):
    Id: NotRequired[str],
    Ec2InstanceId: NotRequired[str],
    PublicDnsName: NotRequired[str],
    PublicIpAddress: NotRequired[str],
    PrivateDnsName: NotRequired[str],
    PrivateIpAddress: NotRequired[str],
    Status: NotRequired[InstanceStatusTypeDef],  # (1)
    InstanceGroupId: NotRequired[str],
    InstanceFleetId: NotRequired[str],
    Market: NotRequired[MarketTypeType],  # (2)
    InstanceType: NotRequired[str],
    EbsVolumes: NotRequired[List[EbsVolumeTypeDef]],  # (3)
```

1. See [:material-code-braces: InstanceStatusTypeDef](./type_defs.md#instancestatustypedef) 
2. See [:material-code-brackets: MarketTypeType](./literals.md#markettypetype) 
3. See [:material-code-braces: EbsVolumeTypeDef](./type_defs.md#ebsvolumetypedef) 
## ListNotebookExecutionsOutputTypeDef

```python
# ListNotebookExecutionsOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListNotebookExecutionsOutputTypeDef


def get_value() -> ListNotebookExecutionsOutputTypeDef:
    return {
        "NotebookExecutions": ...,
    }


# ListNotebookExecutionsOutputTypeDef definition

class ListNotebookExecutionsOutputTypeDef(TypedDict):
    NotebookExecutions: List[NotebookExecutionSummaryTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NotebookExecutionSummaryTypeDef](./type_defs.md#notebookexecutionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeNotebookExecutionOutputTypeDef

```python
# DescribeNotebookExecutionOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import DescribeNotebookExecutionOutputTypeDef


def get_value() -> DescribeNotebookExecutionOutputTypeDef:
    return {
        "NotebookExecution": ...,
    }


# DescribeNotebookExecutionOutputTypeDef definition

class DescribeNotebookExecutionOutputTypeDef(TypedDict):
    NotebookExecution: NotebookExecutionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NotebookExecutionTypeDef](./type_defs.md#notebookexecutiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InstanceFleetProvisioningSpecificationsTypeDef

```python
# InstanceFleetProvisioningSpecificationsTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import InstanceFleetProvisioningSpecificationsTypeDef


def get_value() -> InstanceFleetProvisioningSpecificationsTypeDef:
    return {
        "SpotSpecification": ...,
    }


# InstanceFleetProvisioningSpecificationsTypeDef definition

class InstanceFleetProvisioningSpecificationsTypeDef(TypedDict):
    SpotSpecification: NotRequired[SpotProvisioningSpecificationTypeDef],  # (1)
    OnDemandSpecification: NotRequired[OnDemandProvisioningSpecificationTypeDef],  # (2)
```

1. See [:material-code-braces: SpotProvisioningSpecificationTypeDef](./type_defs.md#spotprovisioningspecificationtypedef) 
2. See [:material-code-braces: OnDemandProvisioningSpecificationTypeDef](./type_defs.md#ondemandprovisioningspecificationtypedef) 
## InstanceFleetResizingSpecificationsTypeDef

```python
# InstanceFleetResizingSpecificationsTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import InstanceFleetResizingSpecificationsTypeDef


def get_value() -> InstanceFleetResizingSpecificationsTypeDef:
    return {
        "SpotResizeSpecification": ...,
    }


# InstanceFleetResizingSpecificationsTypeDef definition

class InstanceFleetResizingSpecificationsTypeDef(TypedDict):
    SpotResizeSpecification: NotRequired[SpotResizingSpecificationTypeDef],  # (1)
    OnDemandResizeSpecification: NotRequired[OnDemandResizingSpecificationTypeDef],  # (2)
```

1. See [:material-code-braces: SpotResizingSpecificationTypeDef](./type_defs.md#spotresizingspecificationtypedef) 
2. See [:material-code-braces: OnDemandResizingSpecificationTypeDef](./type_defs.md#ondemandresizingspecificationtypedef) 
## BootstrapActionConfigTypeDef

```python
# BootstrapActionConfigTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import BootstrapActionConfigTypeDef


def get_value() -> BootstrapActionConfigTypeDef:
    return {
        "Name": ...,
    }


# BootstrapActionConfigTypeDef definition

class BootstrapActionConfigTypeDef(TypedDict):
    Name: str,
    ScriptBootstrapAction: ScriptBootstrapActionConfigUnionTypeDef,  # (1)
```

1. See [:material-code-braces: ScriptBootstrapActionConfigTypeDef](./type_defs.md#scriptbootstrapactionconfigtypedef) [:material-code-braces: ScriptBootstrapActionConfigOutputTypeDef](./type_defs.md#scriptbootstrapactionconfigoutputtypedef) 
## StepSummaryTypeDef

```python
# StepSummaryTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import StepSummaryTypeDef


def get_value() -> StepSummaryTypeDef:
    return {
        "Id": ...,
    }


# StepSummaryTypeDef definition

class StepSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Config: NotRequired[HadoopStepConfigTypeDef],  # (1)
    ActionOnFailure: NotRequired[ActionOnFailureType],  # (2)
    Status: NotRequired[StepStatusTypeDef],  # (3)
```

1. See [:material-code-braces: HadoopStepConfigTypeDef](./type_defs.md#hadoopstepconfigtypedef) 
2. See [:material-code-brackets: ActionOnFailureType](./literals.md#actiononfailuretype) 
3. See [:material-code-braces: StepStatusTypeDef](./type_defs.md#stepstatustypedef) 
## StepTypeDef

```python
# StepTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import StepTypeDef


def get_value() -> StepTypeDef:
    return {
        "Id": ...,
    }


# StepTypeDef definition

class StepTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Config: NotRequired[HadoopStepConfigTypeDef],  # (1)
    ActionOnFailure: NotRequired[ActionOnFailureType],  # (2)
    Status: NotRequired[StepStatusTypeDef],  # (3)
    ExecutionRoleArn: NotRequired[str],
```

1. See [:material-code-braces: HadoopStepConfigTypeDef](./type_defs.md#hadoopstepconfigtypedef) 
2. See [:material-code-brackets: ActionOnFailureType](./literals.md#actiononfailuretype) 
3. See [:material-code-braces: StepStatusTypeDef](./type_defs.md#stepstatustypedef) 
## PutBlockPublicAccessConfigurationInputTypeDef

```python
# PutBlockPublicAccessConfigurationInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import PutBlockPublicAccessConfigurationInputTypeDef


def get_value() -> PutBlockPublicAccessConfigurationInputTypeDef:
    return {
        "BlockPublicAccessConfiguration": ...,
    }


# PutBlockPublicAccessConfigurationInputTypeDef definition

class PutBlockPublicAccessConfigurationInputTypeDef(TypedDict):
    BlockPublicAccessConfiguration: BlockPublicAccessConfigurationUnionTypeDef,  # (1)
```

1. See [:material-code-braces: BlockPublicAccessConfigurationTypeDef](./type_defs.md#blockpublicaccessconfigurationtypedef) [:material-code-braces: BlockPublicAccessConfigurationOutputTypeDef](./type_defs.md#blockpublicaccessconfigurationoutputtypedef) 
## ScalingRuleOutputTypeDef

```python
# ScalingRuleOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ScalingRuleOutputTypeDef


def get_value() -> ScalingRuleOutputTypeDef:
    return {
        "Name": ...,
    }


# ScalingRuleOutputTypeDef definition

class ScalingRuleOutputTypeDef(TypedDict):
    Name: str,
    Action: ScalingActionTypeDef,  # (1)
    Trigger: ScalingTriggerOutputTypeDef,  # (2)
    Description: NotRequired[str],
```

1. See [:material-code-braces: ScalingActionTypeDef](./type_defs.md#scalingactiontypedef) 
2. See [:material-code-braces: ScalingTriggerOutputTypeDef](./type_defs.md#scalingtriggeroutputtypedef) 
## ScalingTriggerTypeDef

```python
# ScalingTriggerTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ScalingTriggerTypeDef


def get_value() -> ScalingTriggerTypeDef:
    return {
        "CloudWatchAlarmDefinition": ...,
    }


# ScalingTriggerTypeDef definition

class ScalingTriggerTypeDef(TypedDict):
    CloudWatchAlarmDefinition: CloudWatchAlarmDefinitionUnionTypeDef,  # (1)
```

1. See [:material-code-braces: CloudWatchAlarmDefinitionTypeDef](./type_defs.md#cloudwatchalarmdefinitiontypedef) [:material-code-braces: CloudWatchAlarmDefinitionOutputTypeDef](./type_defs.md#cloudwatchalarmdefinitionoutputtypedef) 
## ListClustersOutputTypeDef

```python
# ListClustersOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListClustersOutputTypeDef


def get_value() -> ListClustersOutputTypeDef:
    return {
        "Clusters": ...,
    }


# ListClustersOutputTypeDef definition

class ListClustersOutputTypeDef(TypedDict):
    Clusters: List[ClusterSummaryTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterSummaryTypeDef](./type_defs.md#clustersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeClusterOutputTypeDef

```python
# DescribeClusterOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import DescribeClusterOutputTypeDef


def get_value() -> DescribeClusterOutputTypeDef:
    return {
        "Cluster": ...,
    }


# DescribeClusterOutputTypeDef definition

class DescribeClusterOutputTypeDef(TypedDict):
    Cluster: ClusterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClusterTypeDef](./type_defs.md#clustertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InstanceTypeConfigTypeDef

```python
# InstanceTypeConfigTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import InstanceTypeConfigTypeDef


def get_value() -> InstanceTypeConfigTypeDef:
    return {
        "InstanceType": ...,
    }


# InstanceTypeConfigTypeDef definition

class InstanceTypeConfigTypeDef(TypedDict):
    InstanceType: str,
    WeightedCapacity: NotRequired[int],
    BidPrice: NotRequired[str],
    BidPriceAsPercentageOfOnDemandPrice: NotRequired[float],
    EbsConfiguration: NotRequired[EbsConfigurationTypeDef],  # (1)
    Configurations: NotRequired[Sequence[ConfigurationUnionTypeDef]],  # (2)
    CustomAmiId: NotRequired[str],
    Priority: NotRequired[float],
```

1. See [:material-code-braces: EbsConfigurationTypeDef](./type_defs.md#ebsconfigurationtypedef) 
2. See [:material-code-braces: ConfigurationTypeDef](./type_defs.md#configurationtypedef) [:material-code-braces: ConfigurationOutputTypeDef](./type_defs.md#configurationoutputtypedef) 
## StepDetailTypeDef

```python
# StepDetailTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import StepDetailTypeDef


def get_value() -> StepDetailTypeDef:
    return {
        "StepConfig": ...,
    }


# StepDetailTypeDef definition

class StepDetailTypeDef(TypedDict):
    StepConfig: StepConfigOutputTypeDef,  # (1)
    ExecutionStatusDetail: StepExecutionStatusDetailTypeDef,  # (2)
```

1. See [:material-code-braces: StepConfigOutputTypeDef](./type_defs.md#stepconfigoutputtypedef) 
2. See [:material-code-braces: StepExecutionStatusDetailTypeDef](./type_defs.md#stepexecutionstatusdetailtypedef) 
## StepConfigTypeDef

```python
# StepConfigTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import StepConfigTypeDef


def get_value() -> StepConfigTypeDef:
    return {
        "Name": ...,
    }


# StepConfigTypeDef definition

class StepConfigTypeDef(TypedDict):
    Name: str,
    HadoopJarStep: HadoopJarStepConfigUnionTypeDef,  # (2)
    ActionOnFailure: NotRequired[ActionOnFailureType],  # (1)
```

1. See [:material-code-brackets: ActionOnFailureType](./literals.md#actiononfailuretype) 
2. See [:material-code-braces: HadoopJarStepConfigTypeDef](./type_defs.md#hadoopjarstepconfigtypedef) [:material-code-braces: HadoopJarStepConfigOutputTypeDef](./type_defs.md#hadoopjarstepconfigoutputtypedef) 
## ListInstancesOutputTypeDef

```python
# ListInstancesOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListInstancesOutputTypeDef


def get_value() -> ListInstancesOutputTypeDef:
    return {
        "Instances": ...,
    }


# ListInstancesOutputTypeDef definition

class ListInstancesOutputTypeDef(TypedDict):
    Instances: List[InstanceTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InstanceFleetPaginatorTypeDef

```python
# InstanceFleetPaginatorTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import InstanceFleetPaginatorTypeDef


def get_value() -> InstanceFleetPaginatorTypeDef:
    return {
        "Id": ...,
    }


# InstanceFleetPaginatorTypeDef definition

class InstanceFleetPaginatorTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Status: NotRequired[InstanceFleetStatusTypeDef],  # (1)
    InstanceFleetType: NotRequired[InstanceFleetTypeType],  # (2)
    TargetOnDemandCapacity: NotRequired[int],
    TargetSpotCapacity: NotRequired[int],
    ProvisionedOnDemandCapacity: NotRequired[int],
    ProvisionedSpotCapacity: NotRequired[int],
    InstanceTypeSpecifications: NotRequired[List[InstanceTypeSpecificationPaginatorTypeDef]],  # (3)
    LaunchSpecifications: NotRequired[InstanceFleetProvisioningSpecificationsTypeDef],  # (4)
    ResizeSpecifications: NotRequired[InstanceFleetResizingSpecificationsTypeDef],  # (5)
    Context: NotRequired[str],
```

1. See [:material-code-braces: InstanceFleetStatusTypeDef](./type_defs.md#instancefleetstatustypedef) 
2. See [:material-code-brackets: InstanceFleetTypeType](./literals.md#instancefleettypetype) 
3. See [:material-code-braces: InstanceTypeSpecificationPaginatorTypeDef](./type_defs.md#instancetypespecificationpaginatortypedef) 
4. See [:material-code-braces: InstanceFleetProvisioningSpecificationsTypeDef](./type_defs.md#instancefleetprovisioningspecificationstypedef) 
5. See [:material-code-braces: InstanceFleetResizingSpecificationsTypeDef](./type_defs.md#instancefleetresizingspecificationstypedef) 
## InstanceFleetTypeDef

```python
# InstanceFleetTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import InstanceFleetTypeDef


def get_value() -> InstanceFleetTypeDef:
    return {
        "Id": ...,
    }


# InstanceFleetTypeDef definition

class InstanceFleetTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Status: NotRequired[InstanceFleetStatusTypeDef],  # (1)
    InstanceFleetType: NotRequired[InstanceFleetTypeType],  # (2)
    TargetOnDemandCapacity: NotRequired[int],
    TargetSpotCapacity: NotRequired[int],
    ProvisionedOnDemandCapacity: NotRequired[int],
    ProvisionedSpotCapacity: NotRequired[int],
    InstanceTypeSpecifications: NotRequired[List[InstanceTypeSpecificationTypeDef]],  # (3)
    LaunchSpecifications: NotRequired[InstanceFleetProvisioningSpecificationsTypeDef],  # (4)
    ResizeSpecifications: NotRequired[InstanceFleetResizingSpecificationsTypeDef],  # (5)
    Context: NotRequired[str],
```

1. See [:material-code-braces: InstanceFleetStatusTypeDef](./type_defs.md#instancefleetstatustypedef) 
2. See [:material-code-brackets: InstanceFleetTypeType](./literals.md#instancefleettypetype) 
3. See [:material-code-braces: InstanceTypeSpecificationTypeDef](./type_defs.md#instancetypespecificationtypedef) 
4. See [:material-code-braces: InstanceFleetProvisioningSpecificationsTypeDef](./type_defs.md#instancefleetprovisioningspecificationstypedef) 
5. See [:material-code-braces: InstanceFleetResizingSpecificationsTypeDef](./type_defs.md#instancefleetresizingspecificationstypedef) 
## ListStepsOutputTypeDef

```python
# ListStepsOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListStepsOutputTypeDef


def get_value() -> ListStepsOutputTypeDef:
    return {
        "Steps": ...,
    }


# ListStepsOutputTypeDef definition

class ListStepsOutputTypeDef(TypedDict):
    Steps: List[StepSummaryTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StepSummaryTypeDef](./type_defs.md#stepsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeStepOutputTypeDef

```python
# DescribeStepOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import DescribeStepOutputTypeDef


def get_value() -> DescribeStepOutputTypeDef:
    return {
        "Step": ...,
    }


# DescribeStepOutputTypeDef definition

class DescribeStepOutputTypeDef(TypedDict):
    Step: StepTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StepTypeDef](./type_defs.md#steptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AutoScalingPolicyDescriptionTypeDef

```python
# AutoScalingPolicyDescriptionTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import AutoScalingPolicyDescriptionTypeDef


def get_value() -> AutoScalingPolicyDescriptionTypeDef:
    return {
        "Status": ...,
    }


# AutoScalingPolicyDescriptionTypeDef definition

class AutoScalingPolicyDescriptionTypeDef(TypedDict):
    Status: NotRequired[AutoScalingPolicyStatusTypeDef],  # (1)
    Constraints: NotRequired[ScalingConstraintsTypeDef],  # (2)
    Rules: NotRequired[List[ScalingRuleOutputTypeDef]],  # (3)
```

1. See [:material-code-braces: AutoScalingPolicyStatusTypeDef](./type_defs.md#autoscalingpolicystatustypedef) 
2. See [:material-code-braces: ScalingConstraintsTypeDef](./type_defs.md#scalingconstraintstypedef) 
3. See [:material-code-braces: ScalingRuleOutputTypeDef](./type_defs.md#scalingruleoutputtypedef) 
## InstanceFleetConfigTypeDef

```python
# InstanceFleetConfigTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import InstanceFleetConfigTypeDef


def get_value() -> InstanceFleetConfigTypeDef:
    return {
        "Name": ...,
    }


# InstanceFleetConfigTypeDef definition

class InstanceFleetConfigTypeDef(TypedDict):
    InstanceFleetType: InstanceFleetTypeType,  # (1)
    Name: NotRequired[str],
    TargetOnDemandCapacity: NotRequired[int],
    TargetSpotCapacity: NotRequired[int],
    InstanceTypeConfigs: NotRequired[Sequence[InstanceTypeConfigTypeDef]],  # (2)
    LaunchSpecifications: NotRequired[InstanceFleetProvisioningSpecificationsTypeDef],  # (3)
    ResizeSpecifications: NotRequired[InstanceFleetResizingSpecificationsTypeDef],  # (4)
    Context: NotRequired[str],
```

1. See [:material-code-brackets: InstanceFleetTypeType](./literals.md#instancefleettypetype) 
2. See [:material-code-braces: InstanceTypeConfigTypeDef](./type_defs.md#instancetypeconfigtypedef) 
3. See [:material-code-braces: InstanceFleetProvisioningSpecificationsTypeDef](./type_defs.md#instancefleetprovisioningspecificationstypedef) 
4. See [:material-code-braces: InstanceFleetResizingSpecificationsTypeDef](./type_defs.md#instancefleetresizingspecificationstypedef) 
## InstanceFleetModifyConfigTypeDef

```python
# InstanceFleetModifyConfigTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import InstanceFleetModifyConfigTypeDef


def get_value() -> InstanceFleetModifyConfigTypeDef:
    return {
        "InstanceFleetId": ...,
    }


# InstanceFleetModifyConfigTypeDef definition

class InstanceFleetModifyConfigTypeDef(TypedDict):
    InstanceFleetId: str,
    TargetOnDemandCapacity: NotRequired[int],
    TargetSpotCapacity: NotRequired[int],
    ResizeSpecifications: NotRequired[InstanceFleetResizingSpecificationsTypeDef],  # (1)
    InstanceTypeConfigs: NotRequired[Sequence[InstanceTypeConfigTypeDef]],  # (2)
    Context: NotRequired[str],
```

1. See [:material-code-braces: InstanceFleetResizingSpecificationsTypeDef](./type_defs.md#instancefleetresizingspecificationstypedef) 
2. See [:material-code-braces: InstanceTypeConfigTypeDef](./type_defs.md#instancetypeconfigtypedef) 
## JobFlowDetailTypeDef

```python
# JobFlowDetailTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import JobFlowDetailTypeDef


def get_value() -> JobFlowDetailTypeDef:
    return {
        "JobFlowId": ...,
    }


# JobFlowDetailTypeDef definition

class JobFlowDetailTypeDef(TypedDict):
    JobFlowId: str,
    Name: str,
    ExecutionStatusDetail: JobFlowExecutionStatusDetailTypeDef,  # (1)
    Instances: JobFlowInstancesDetailTypeDef,  # (2)
    LogUri: NotRequired[str],
    LogEncryptionKmsKeyId: NotRequired[str],
    AmiVersion: NotRequired[str],
    Steps: NotRequired[List[StepDetailTypeDef]],  # (3)
    BootstrapActions: NotRequired[List[BootstrapActionDetailTypeDef]],  # (4)
    SupportedProducts: NotRequired[List[str]],
    VisibleToAllUsers: NotRequired[bool],
    JobFlowRole: NotRequired[str],
    ServiceRole: NotRequired[str],
    AutoScalingRole: NotRequired[str],
    ScaleDownBehavior: NotRequired[ScaleDownBehaviorType],  # (5)
```

1. See [:material-code-braces: JobFlowExecutionStatusDetailTypeDef](./type_defs.md#jobflowexecutionstatusdetailtypedef) 
2. See [:material-code-braces: JobFlowInstancesDetailTypeDef](./type_defs.md#jobflowinstancesdetailtypedef) 
3. See [:material-code-braces: StepDetailTypeDef](./type_defs.md#stepdetailtypedef) 
4. See [:material-code-braces: BootstrapActionDetailTypeDef](./type_defs.md#bootstrapactiondetailtypedef) 
5. See [:material-code-brackets: ScaleDownBehaviorType](./literals.md#scaledownbehaviortype) 
## InstanceGroupModifyConfigTypeDef

```python
# InstanceGroupModifyConfigTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import InstanceGroupModifyConfigTypeDef


def get_value() -> InstanceGroupModifyConfigTypeDef:
    return {
        "InstanceGroupId": ...,
    }


# InstanceGroupModifyConfigTypeDef definition

class InstanceGroupModifyConfigTypeDef(TypedDict):
    InstanceGroupId: str,
    InstanceCount: NotRequired[int],
    EC2InstanceIdsToTerminate: NotRequired[Sequence[str]],
    ShrinkPolicy: NotRequired[ShrinkPolicyUnionTypeDef],  # (1)
    ReconfigurationType: NotRequired[ReconfigurationTypeType],  # (2)
    Configurations: NotRequired[Sequence[ConfigurationUnionTypeDef]],  # (3)
```

1. See [:material-code-braces: ShrinkPolicyTypeDef](./type_defs.md#shrinkpolicytypedef) [:material-code-braces: ShrinkPolicyOutputTypeDef](./type_defs.md#shrinkpolicyoutputtypedef) 
2. See [:material-code-brackets: ReconfigurationTypeType](./literals.md#reconfigurationtypetype) 
3. See [:material-code-braces: ConfigurationTypeDef](./type_defs.md#configurationtypedef) [:material-code-braces: ConfigurationOutputTypeDef](./type_defs.md#configurationoutputtypedef) 
## ListInstanceFleetsOutputPaginatorTypeDef

```python
# ListInstanceFleetsOutputPaginatorTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListInstanceFleetsOutputPaginatorTypeDef


def get_value() -> ListInstanceFleetsOutputPaginatorTypeDef:
    return {
        "InstanceFleets": ...,
    }


# ListInstanceFleetsOutputPaginatorTypeDef definition

class ListInstanceFleetsOutputPaginatorTypeDef(TypedDict):
    InstanceFleets: List[InstanceFleetPaginatorTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceFleetPaginatorTypeDef](./type_defs.md#instancefleetpaginatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInstanceFleetsOutputTypeDef

```python
# ListInstanceFleetsOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListInstanceFleetsOutputTypeDef


def get_value() -> ListInstanceFleetsOutputTypeDef:
    return {
        "InstanceFleets": ...,
    }


# ListInstanceFleetsOutputTypeDef definition

class ListInstanceFleetsOutputTypeDef(TypedDict):
    InstanceFleets: List[InstanceFleetTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceFleetTypeDef](./type_defs.md#instancefleettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InstanceGroupPaginatorTypeDef

```python
# InstanceGroupPaginatorTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import InstanceGroupPaginatorTypeDef


def get_value() -> InstanceGroupPaginatorTypeDef:
    return {
        "Id": ...,
    }


# InstanceGroupPaginatorTypeDef definition

class InstanceGroupPaginatorTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Market: NotRequired[MarketTypeType],  # (1)
    InstanceGroupType: NotRequired[InstanceGroupTypeType],  # (2)
    BidPrice: NotRequired[str],
    InstanceType: NotRequired[str],
    RequestedInstanceCount: NotRequired[int],
    RunningInstanceCount: NotRequired[int],
    Status: NotRequired[InstanceGroupStatusTypeDef],  # (3)
    Configurations: NotRequired[List[ConfigurationPaginatorTypeDef]],  # (4)
    ConfigurationsVersion: NotRequired[int],
    LastSuccessfullyAppliedConfigurations: NotRequired[List[ConfigurationPaginatorTypeDef]],  # (4)
    LastSuccessfullyAppliedConfigurationsVersion: NotRequired[int],
    EbsBlockDevices: NotRequired[List[EbsBlockDeviceTypeDef]],  # (6)
    EbsOptimized: NotRequired[bool],
    ShrinkPolicy: NotRequired[ShrinkPolicyOutputTypeDef],  # (7)
    AutoScalingPolicy: NotRequired[AutoScalingPolicyDescriptionTypeDef],  # (8)
    CustomAmiId: NotRequired[str],
```

1. See [:material-code-brackets: MarketTypeType](./literals.md#markettypetype) 
2. See [:material-code-brackets: InstanceGroupTypeType](./literals.md#instancegrouptypetype) 
3. See [:material-code-braces: InstanceGroupStatusTypeDef](./type_defs.md#instancegroupstatustypedef) 
4. See [:material-code-braces: ConfigurationPaginatorTypeDef](./type_defs.md#configurationpaginatortypedef) 
5. See [:material-code-braces: ConfigurationPaginatorTypeDef](./type_defs.md#configurationpaginatortypedef) 
6. See [:material-code-braces: EbsBlockDeviceTypeDef](./type_defs.md#ebsblockdevicetypedef) 
7. See [:material-code-braces: ShrinkPolicyOutputTypeDef](./type_defs.md#shrinkpolicyoutputtypedef) 
8. See [:material-code-braces: AutoScalingPolicyDescriptionTypeDef](./type_defs.md#autoscalingpolicydescriptiontypedef) 
## InstanceGroupTypeDef

```python
# InstanceGroupTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import InstanceGroupTypeDef


def get_value() -> InstanceGroupTypeDef:
    return {
        "Id": ...,
    }


# InstanceGroupTypeDef definition

class InstanceGroupTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Market: NotRequired[MarketTypeType],  # (1)
    InstanceGroupType: NotRequired[InstanceGroupTypeType],  # (2)
    BidPrice: NotRequired[str],
    InstanceType: NotRequired[str],
    RequestedInstanceCount: NotRequired[int],
    RunningInstanceCount: NotRequired[int],
    Status: NotRequired[InstanceGroupStatusTypeDef],  # (3)
    Configurations: NotRequired[List[ConfigurationOutputTypeDef]],  # (4)
    ConfigurationsVersion: NotRequired[int],
    LastSuccessfullyAppliedConfigurations: NotRequired[List[ConfigurationOutputTypeDef]],  # (4)
    LastSuccessfullyAppliedConfigurationsVersion: NotRequired[int],
    EbsBlockDevices: NotRequired[List[EbsBlockDeviceTypeDef]],  # (6)
    EbsOptimized: NotRequired[bool],
    ShrinkPolicy: NotRequired[ShrinkPolicyOutputTypeDef],  # (7)
    AutoScalingPolicy: NotRequired[AutoScalingPolicyDescriptionTypeDef],  # (8)
    CustomAmiId: NotRequired[str],
```

1. See [:material-code-brackets: MarketTypeType](./literals.md#markettypetype) 
2. See [:material-code-brackets: InstanceGroupTypeType](./literals.md#instancegrouptypetype) 
3. See [:material-code-braces: InstanceGroupStatusTypeDef](./type_defs.md#instancegroupstatustypedef) 
4. See [:material-code-braces: ConfigurationOutputTypeDef](./type_defs.md#configurationoutputtypedef) 
5. See [:material-code-braces: ConfigurationOutputTypeDef](./type_defs.md#configurationoutputtypedef) 
6. See [:material-code-braces: EbsBlockDeviceTypeDef](./type_defs.md#ebsblockdevicetypedef) 
7. See [:material-code-braces: ShrinkPolicyOutputTypeDef](./type_defs.md#shrinkpolicyoutputtypedef) 
8. See [:material-code-braces: AutoScalingPolicyDescriptionTypeDef](./type_defs.md#autoscalingpolicydescriptiontypedef) 
## PutAutoScalingPolicyOutputTypeDef

```python
# PutAutoScalingPolicyOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import PutAutoScalingPolicyOutputTypeDef


def get_value() -> PutAutoScalingPolicyOutputTypeDef:
    return {
        "ClusterId": ...,
    }


# PutAutoScalingPolicyOutputTypeDef definition

class PutAutoScalingPolicyOutputTypeDef(TypedDict):
    ClusterId: str,
    InstanceGroupId: str,
    AutoScalingPolicy: AutoScalingPolicyDescriptionTypeDef,  # (1)
    ClusterArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AutoScalingPolicyDescriptionTypeDef](./type_defs.md#autoscalingpolicydescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ScalingRuleTypeDef

```python
# ScalingRuleTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ScalingRuleTypeDef


def get_value() -> ScalingRuleTypeDef:
    return {
        "Name": ...,
    }


# ScalingRuleTypeDef definition

class ScalingRuleTypeDef(TypedDict):
    Name: str,
    Action: ScalingActionTypeDef,  # (1)
    Trigger: ScalingTriggerUnionTypeDef,  # (2)
    Description: NotRequired[str],
```

1. See [:material-code-braces: ScalingActionTypeDef](./type_defs.md#scalingactiontypedef) 
2. See [:material-code-braces: ScalingTriggerTypeDef](./type_defs.md#scalingtriggertypedef) [:material-code-braces: ScalingTriggerOutputTypeDef](./type_defs.md#scalingtriggeroutputtypedef) 
## AddInstanceFleetInputTypeDef

```python
# AddInstanceFleetInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import AddInstanceFleetInputTypeDef


def get_value() -> AddInstanceFleetInputTypeDef:
    return {
        "ClusterId": ...,
    }


# AddInstanceFleetInputTypeDef definition

class AddInstanceFleetInputTypeDef(TypedDict):
    ClusterId: str,
    InstanceFleet: InstanceFleetConfigTypeDef,  # (1)
```

1. See [:material-code-braces: InstanceFleetConfigTypeDef](./type_defs.md#instancefleetconfigtypedef) 
## ModifyInstanceFleetInputTypeDef

```python
# ModifyInstanceFleetInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ModifyInstanceFleetInputTypeDef


def get_value() -> ModifyInstanceFleetInputTypeDef:
    return {
        "ClusterId": ...,
    }


# ModifyInstanceFleetInputTypeDef definition

class ModifyInstanceFleetInputTypeDef(TypedDict):
    ClusterId: str,
    InstanceFleet: InstanceFleetModifyConfigTypeDef,  # (1)
```

1. See [:material-code-braces: InstanceFleetModifyConfigTypeDef](./type_defs.md#instancefleetmodifyconfigtypedef) 
## DescribeJobFlowsOutputTypeDef

```python
# DescribeJobFlowsOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import DescribeJobFlowsOutputTypeDef


def get_value() -> DescribeJobFlowsOutputTypeDef:
    return {
        "JobFlows": ...,
    }


# DescribeJobFlowsOutputTypeDef definition

class DescribeJobFlowsOutputTypeDef(TypedDict):
    JobFlows: List[JobFlowDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobFlowDetailTypeDef](./type_defs.md#jobflowdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddJobFlowStepsInputTypeDef

```python
# AddJobFlowStepsInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import AddJobFlowStepsInputTypeDef


def get_value() -> AddJobFlowStepsInputTypeDef:
    return {
        "JobFlowId": ...,
    }


# AddJobFlowStepsInputTypeDef definition

class AddJobFlowStepsInputTypeDef(TypedDict):
    JobFlowId: str,
    Steps: Sequence[StepConfigUnionTypeDef],  # (1)
    ExecutionRoleArn: NotRequired[str],
```

1. See [:material-code-braces: StepConfigTypeDef](./type_defs.md#stepconfigtypedef) [:material-code-braces: StepConfigOutputTypeDef](./type_defs.md#stepconfigoutputtypedef) 
## ModifyInstanceGroupsInputTypeDef

```python
# ModifyInstanceGroupsInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ModifyInstanceGroupsInputTypeDef


def get_value() -> ModifyInstanceGroupsInputTypeDef:
    return {
        "ClusterId": ...,
    }


# ModifyInstanceGroupsInputTypeDef definition

class ModifyInstanceGroupsInputTypeDef(TypedDict):
    ClusterId: NotRequired[str],
    InstanceGroups: NotRequired[Sequence[InstanceGroupModifyConfigTypeDef]],  # (1)
```

1. See [:material-code-braces: InstanceGroupModifyConfigTypeDef](./type_defs.md#instancegroupmodifyconfigtypedef) 
## ListInstanceGroupsOutputPaginatorTypeDef

```python
# ListInstanceGroupsOutputPaginatorTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListInstanceGroupsOutputPaginatorTypeDef


def get_value() -> ListInstanceGroupsOutputPaginatorTypeDef:
    return {
        "InstanceGroups": ...,
    }


# ListInstanceGroupsOutputPaginatorTypeDef definition

class ListInstanceGroupsOutputPaginatorTypeDef(TypedDict):
    InstanceGroups: List[InstanceGroupPaginatorTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceGroupPaginatorTypeDef](./type_defs.md#instancegrouppaginatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInstanceGroupsOutputTypeDef

```python
# ListInstanceGroupsOutputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import ListInstanceGroupsOutputTypeDef


def get_value() -> ListInstanceGroupsOutputTypeDef:
    return {
        "InstanceGroups": ...,
    }


# ListInstanceGroupsOutputTypeDef definition

class ListInstanceGroupsOutputTypeDef(TypedDict):
    InstanceGroups: List[InstanceGroupTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceGroupTypeDef](./type_defs.md#instancegrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AutoScalingPolicyTypeDef

```python
# AutoScalingPolicyTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import AutoScalingPolicyTypeDef


def get_value() -> AutoScalingPolicyTypeDef:
    return {
        "Constraints": ...,
    }


# AutoScalingPolicyTypeDef definition

class AutoScalingPolicyTypeDef(TypedDict):
    Constraints: ScalingConstraintsTypeDef,  # (1)
    Rules: Sequence[ScalingRuleUnionTypeDef],  # (2)
```

1. See [:material-code-braces: ScalingConstraintsTypeDef](./type_defs.md#scalingconstraintstypedef) 
2. See [:material-code-braces: ScalingRuleTypeDef](./type_defs.md#scalingruletypedef) [:material-code-braces: ScalingRuleOutputTypeDef](./type_defs.md#scalingruleoutputtypedef) 
## InstanceGroupConfigTypeDef

```python
# InstanceGroupConfigTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import InstanceGroupConfigTypeDef


def get_value() -> InstanceGroupConfigTypeDef:
    return {
        "Name": ...,
    }


# InstanceGroupConfigTypeDef definition

class InstanceGroupConfigTypeDef(TypedDict):
    InstanceRole: InstanceRoleTypeType,  # (2)
    InstanceType: str,
    InstanceCount: int,
    Name: NotRequired[str],
    Market: NotRequired[MarketTypeType],  # (1)
    BidPrice: NotRequired[str],
    Configurations: NotRequired[Sequence[ConfigurationUnionTypeDef]],  # (3)
    EbsConfiguration: NotRequired[EbsConfigurationTypeDef],  # (4)
    AutoScalingPolicy: NotRequired[AutoScalingPolicyTypeDef],  # (5)
    CustomAmiId: NotRequired[str],
```

1. See [:material-code-brackets: MarketTypeType](./literals.md#markettypetype) 
2. See [:material-code-brackets: InstanceRoleTypeType](./literals.md#instanceroletypetype) 
3. See [:material-code-braces: ConfigurationTypeDef](./type_defs.md#configurationtypedef) [:material-code-braces: ConfigurationOutputTypeDef](./type_defs.md#configurationoutputtypedef) 
4. See [:material-code-braces: EbsConfigurationTypeDef](./type_defs.md#ebsconfigurationtypedef) 
5. See [:material-code-braces: AutoScalingPolicyTypeDef](./type_defs.md#autoscalingpolicytypedef) 
## PutAutoScalingPolicyInputTypeDef

```python
# PutAutoScalingPolicyInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import PutAutoScalingPolicyInputTypeDef


def get_value() -> PutAutoScalingPolicyInputTypeDef:
    return {
        "ClusterId": ...,
    }


# PutAutoScalingPolicyInputTypeDef definition

class PutAutoScalingPolicyInputTypeDef(TypedDict):
    ClusterId: str,
    InstanceGroupId: str,
    AutoScalingPolicy: AutoScalingPolicyTypeDef,  # (1)
```

1. See [:material-code-braces: AutoScalingPolicyTypeDef](./type_defs.md#autoscalingpolicytypedef) 
## AddInstanceGroupsInputTypeDef

```python
# AddInstanceGroupsInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import AddInstanceGroupsInputTypeDef


def get_value() -> AddInstanceGroupsInputTypeDef:
    return {
        "InstanceGroups": ...,
    }


# AddInstanceGroupsInputTypeDef definition

class AddInstanceGroupsInputTypeDef(TypedDict):
    InstanceGroups: Sequence[InstanceGroupConfigTypeDef],  # (1)
    JobFlowId: str,
```

1. See [:material-code-braces: InstanceGroupConfigTypeDef](./type_defs.md#instancegroupconfigtypedef) 
## JobFlowInstancesConfigTypeDef

```python
# JobFlowInstancesConfigTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import JobFlowInstancesConfigTypeDef


def get_value() -> JobFlowInstancesConfigTypeDef:
    return {
        "MasterInstanceType": ...,
    }


# JobFlowInstancesConfigTypeDef definition

class JobFlowInstancesConfigTypeDef(TypedDict):
    MasterInstanceType: NotRequired[str],
    SlaveInstanceType: NotRequired[str],
    InstanceCount: NotRequired[int],
    InstanceGroups: NotRequired[Sequence[InstanceGroupConfigTypeDef]],  # (1)
    InstanceFleets: NotRequired[Sequence[InstanceFleetConfigTypeDef]],  # (2)
    Ec2KeyName: NotRequired[str],
    Placement: NotRequired[PlacementTypeUnionTypeDef],  # (3)
    KeepJobFlowAliveWhenNoSteps: NotRequired[bool],
    TerminationProtected: NotRequired[bool],
    UnhealthyNodeReplacement: NotRequired[bool],
    HadoopVersion: NotRequired[str],
    Ec2SubnetId: NotRequired[str],
    Ec2SubnetIds: NotRequired[Sequence[str]],
    EmrManagedMasterSecurityGroup: NotRequired[str],
    EmrManagedSlaveSecurityGroup: NotRequired[str],
    ServiceAccessSecurityGroup: NotRequired[str],
    AdditionalMasterSecurityGroups: NotRequired[Sequence[str]],
    AdditionalSlaveSecurityGroups: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: InstanceGroupConfigTypeDef](./type_defs.md#instancegroupconfigtypedef) 
2. See [:material-code-braces: InstanceFleetConfigTypeDef](./type_defs.md#instancefleetconfigtypedef) 
3. See [:material-code-braces: PlacementTypeTypeDef](./type_defs.md#placementtypetypedef) [:material-code-braces: PlacementTypeOutputTypeDef](./type_defs.md#placementtypeoutputtypedef) 
## RunJobFlowInputTypeDef

```python
# RunJobFlowInputTypeDef TypedDict usage example

from types_aiobotocore_emr.type_defs import RunJobFlowInputTypeDef


def get_value() -> RunJobFlowInputTypeDef:
    return {
        "Name": ...,
    }


# RunJobFlowInputTypeDef definition

class RunJobFlowInputTypeDef(TypedDict):
    Name: str,
    Instances: JobFlowInstancesConfigTypeDef,  # (1)
    LogUri: NotRequired[str],
    LogEncryptionKmsKeyId: NotRequired[str],
    AdditionalInfo: NotRequired[str],
    AmiVersion: NotRequired[str],
    ReleaseLabel: NotRequired[str],
    Steps: NotRequired[Sequence[StepConfigUnionTypeDef]],  # (2)
    BootstrapActions: NotRequired[Sequence[BootstrapActionConfigUnionTypeDef]],  # (3)
    SupportedProducts: NotRequired[Sequence[str]],
    NewSupportedProducts: NotRequired[Sequence[SupportedProductConfigTypeDef]],  # (4)
    Applications: NotRequired[Sequence[ApplicationUnionTypeDef]],  # (5)
    Configurations: NotRequired[Sequence[ConfigurationUnionTypeDef]],  # (6)
    VisibleToAllUsers: NotRequired[bool],
    JobFlowRole: NotRequired[str],
    ServiceRole: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (7)
    SecurityConfiguration: NotRequired[str],
    AutoScalingRole: NotRequired[str],
    ScaleDownBehavior: NotRequired[ScaleDownBehaviorType],  # (8)
    CustomAmiId: NotRequired[str],
    EbsRootVolumeSize: NotRequired[int],
    RepoUpgradeOnBoot: NotRequired[RepoUpgradeOnBootType],  # (9)
    KerberosAttributes: NotRequired[KerberosAttributesTypeDef],  # (10)
    StepConcurrencyLevel: NotRequired[int],
    ManagedScalingPolicy: NotRequired[ManagedScalingPolicyTypeDef],  # (11)
    PlacementGroupConfigs: NotRequired[Sequence[PlacementGroupConfigTypeDef]],  # (12)
    AutoTerminationPolicy: NotRequired[AutoTerminationPolicyTypeDef],  # (13)
    OSReleaseLabel: NotRequired[str],
    EbsRootVolumeIops: NotRequired[int],
    EbsRootVolumeThroughput: NotRequired[int],
```

1. See [:material-code-braces: JobFlowInstancesConfigTypeDef](./type_defs.md#jobflowinstancesconfigtypedef) 
2. See [:material-code-braces: StepConfigTypeDef](./type_defs.md#stepconfigtypedef) [:material-code-braces: StepConfigOutputTypeDef](./type_defs.md#stepconfigoutputtypedef) 
3. See [:material-code-braces: BootstrapActionConfigTypeDef](./type_defs.md#bootstrapactionconfigtypedef) [:material-code-braces: BootstrapActionConfigOutputTypeDef](./type_defs.md#bootstrapactionconfigoutputtypedef) 
4. See [:material-code-braces: SupportedProductConfigTypeDef](./type_defs.md#supportedproductconfigtypedef) 
5. See [:material-code-braces: ApplicationTypeDef](./type_defs.md#applicationtypedef) [:material-code-braces: ApplicationOutputTypeDef](./type_defs.md#applicationoutputtypedef) 
6. See [:material-code-braces: ConfigurationTypeDef](./type_defs.md#configurationtypedef) [:material-code-braces: ConfigurationOutputTypeDef](./type_defs.md#configurationoutputtypedef) 
7. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
8. See [:material-code-brackets: ScaleDownBehaviorType](./literals.md#scaledownbehaviortype) 
9. See [:material-code-brackets: RepoUpgradeOnBootType](./literals.md#repoupgradeonboottype) 
10. See [:material-code-braces: KerberosAttributesTypeDef](./type_defs.md#kerberosattributestypedef) 
11. See [:material-code-braces: ManagedScalingPolicyTypeDef](./type_defs.md#managedscalingpolicytypedef) 
12. See [:material-code-braces: PlacementGroupConfigTypeDef](./type_defs.md#placementgroupconfigtypedef) 
13. See [:material-code-braces: AutoTerminationPolicyTypeDef](./type_defs.md#autoterminationpolicytypedef) 
