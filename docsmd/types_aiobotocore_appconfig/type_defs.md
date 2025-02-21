# Type definitions

> [Index](../README.md) > [AppConfig](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [AppConfig](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#appconfig)
    type annotations stubs module [types-aiobotocore-appconfig](https://pypi.org/project/types-aiobotocore-appconfig/).

## BlobTypeDef

```python
# BlobTypeDef Union usage example

from types_aiobotocore_appconfig.type_defs import BlobTypeDef


def get_value() -> BlobTypeDef:
    return ...


# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```




## DeletionProtectionSettingsTypeDef

```python
# DeletionProtectionSettingsTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import DeletionProtectionSettingsTypeDef


def get_value() -> DeletionProtectionSettingsTypeDef:
    return {
        "Enabled": ...,
    }


# DeletionProtectionSettingsTypeDef definition

class DeletionProtectionSettingsTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    ProtectionPeriodInMinutes: NotRequired[int],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ResponseMetadataTypeDef


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

## ActionInvocationTypeDef

```python
# ActionInvocationTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ActionInvocationTypeDef


def get_value() -> ActionInvocationTypeDef:
    return {
        "ExtensionIdentifier": ...,
    }


# ActionInvocationTypeDef definition

class ActionInvocationTypeDef(TypedDict):
    ExtensionIdentifier: NotRequired[str],
    ActionName: NotRequired[str],
    Uri: NotRequired[str],
    RoleArn: NotRequired[str],
    ErrorMessage: NotRequired[str],
    ErrorCode: NotRequired[str],
    InvocationId: NotRequired[str],
```

## ActionTypeDef

```python
# ActionTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ActionTypeDef


def get_value() -> ActionTypeDef:
    return {
        "Name": ...,
    }


# ActionTypeDef definition

class ActionTypeDef(TypedDict):
    Name: NotRequired[str],
    Description: NotRequired[str],
    Uri: NotRequired[str],
    RoleArn: NotRequired[str],
```

## ApplicationTypeDef

```python
# ApplicationTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ApplicationTypeDef


def get_value() -> ApplicationTypeDef:
    return {
        "Id": ...,
    }


# ApplicationTypeDef definition

class ApplicationTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
```

## AppliedExtensionTypeDef

```python
# AppliedExtensionTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import AppliedExtensionTypeDef


def get_value() -> AppliedExtensionTypeDef:
    return {
        "ExtensionId": ...,
    }


# AppliedExtensionTypeDef definition

class AppliedExtensionTypeDef(TypedDict):
    ExtensionId: NotRequired[str],
    ExtensionAssociationId: NotRequired[str],
    VersionNumber: NotRequired[int],
    Parameters: NotRequired[Dict[str, str]],
```

## ConfigurationProfileSummaryTypeDef

```python
# ConfigurationProfileSummaryTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ConfigurationProfileSummaryTypeDef


def get_value() -> ConfigurationProfileSummaryTypeDef:
    return {
        "ApplicationId": ...,
    }


# ConfigurationProfileSummaryTypeDef definition

class ConfigurationProfileSummaryTypeDef(TypedDict):
    ApplicationId: NotRequired[str],
    Id: NotRequired[str],
    Name: NotRequired[str],
    LocationUri: NotRequired[str],
    ValidatorTypes: NotRequired[List[ValidatorTypeType]],  # (1)
    Type: NotRequired[str],
```

1. See [:material-code-brackets: ValidatorTypeType](./literals.md#validatortypetype) 
## ValidatorTypeDef

```python
# ValidatorTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ValidatorTypeDef


def get_value() -> ValidatorTypeDef:
    return {
        "Type": ...,
    }


# ValidatorTypeDef definition

class ValidatorTypeDef(TypedDict):
    Type: ValidatorTypeType,  # (1)
    Content: str,
```

1. See [:material-code-brackets: ValidatorTypeType](./literals.md#validatortypetype) 
## CreateApplicationRequestTypeDef

```python
# CreateApplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import CreateApplicationRequestTypeDef


def get_value() -> CreateApplicationRequestTypeDef:
    return {
        "Name": ...,
    }


# CreateApplicationRequestTypeDef definition

class CreateApplicationRequestTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

## CreateDeploymentStrategyRequestTypeDef

```python
# CreateDeploymentStrategyRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import CreateDeploymentStrategyRequestTypeDef


def get_value() -> CreateDeploymentStrategyRequestTypeDef:
    return {
        "Name": ...,
    }


# CreateDeploymentStrategyRequestTypeDef definition

class CreateDeploymentStrategyRequestTypeDef(TypedDict):
    Name: str,
    DeploymentDurationInMinutes: int,
    GrowthFactor: float,
    Description: NotRequired[str],
    FinalBakeTimeInMinutes: NotRequired[int],
    GrowthType: NotRequired[GrowthTypeType],  # (1)
    ReplicateTo: NotRequired[ReplicateToType],  # (2)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: GrowthTypeType](./literals.md#growthtypetype) 
2. See [:material-code-brackets: ReplicateToType](./literals.md#replicatetotype) 
## MonitorTypeDef

```python
# MonitorTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import MonitorTypeDef


def get_value() -> MonitorTypeDef:
    return {
        "AlarmArn": ...,
    }


# MonitorTypeDef definition

class MonitorTypeDef(TypedDict):
    AlarmArn: str,
    AlarmRoleArn: NotRequired[str],
```

## CreateExtensionAssociationRequestTypeDef

```python
# CreateExtensionAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import CreateExtensionAssociationRequestTypeDef


def get_value() -> CreateExtensionAssociationRequestTypeDef:
    return {
        "ExtensionIdentifier": ...,
    }


# CreateExtensionAssociationRequestTypeDef definition

class CreateExtensionAssociationRequestTypeDef(TypedDict):
    ExtensionIdentifier: str,
    ResourceIdentifier: str,
    ExtensionVersionNumber: NotRequired[int],
    Parameters: NotRequired[Mapping[str, str]],
    Tags: NotRequired[Mapping[str, str]],
```

## ParameterTypeDef

```python
# ParameterTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ParameterTypeDef


def get_value() -> ParameterTypeDef:
    return {
        "Description": ...,
    }


# ParameterTypeDef definition

class ParameterTypeDef(TypedDict):
    Description: NotRequired[str],
    Required: NotRequired[bool],
    Dynamic: NotRequired[bool],
```

## DeleteApplicationRequestTypeDef

```python
# DeleteApplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import DeleteApplicationRequestTypeDef


def get_value() -> DeleteApplicationRequestTypeDef:
    return {
        "ApplicationId": ...,
    }


# DeleteApplicationRequestTypeDef definition

class DeleteApplicationRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## DeleteConfigurationProfileRequestTypeDef

```python
# DeleteConfigurationProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import DeleteConfigurationProfileRequestTypeDef


def get_value() -> DeleteConfigurationProfileRequestTypeDef:
    return {
        "ApplicationId": ...,
    }


# DeleteConfigurationProfileRequestTypeDef definition

class DeleteConfigurationProfileRequestTypeDef(TypedDict):
    ApplicationId: str,
    ConfigurationProfileId: str,
    DeletionProtectionCheck: NotRequired[DeletionProtectionCheckType],  # (1)
```

1. See [:material-code-brackets: DeletionProtectionCheckType](./literals.md#deletionprotectionchecktype) 
## DeleteDeploymentStrategyRequestTypeDef

```python
# DeleteDeploymentStrategyRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import DeleteDeploymentStrategyRequestTypeDef


def get_value() -> DeleteDeploymentStrategyRequestTypeDef:
    return {
        "DeploymentStrategyId": ...,
    }


# DeleteDeploymentStrategyRequestTypeDef definition

class DeleteDeploymentStrategyRequestTypeDef(TypedDict):
    DeploymentStrategyId: str,
```

## DeleteEnvironmentRequestTypeDef

```python
# DeleteEnvironmentRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import DeleteEnvironmentRequestTypeDef


def get_value() -> DeleteEnvironmentRequestTypeDef:
    return {
        "EnvironmentId": ...,
    }


# DeleteEnvironmentRequestTypeDef definition

class DeleteEnvironmentRequestTypeDef(TypedDict):
    EnvironmentId: str,
    ApplicationId: str,
    DeletionProtectionCheck: NotRequired[DeletionProtectionCheckType],  # (1)
```

1. See [:material-code-brackets: DeletionProtectionCheckType](./literals.md#deletionprotectionchecktype) 
## DeleteExtensionAssociationRequestTypeDef

```python
# DeleteExtensionAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import DeleteExtensionAssociationRequestTypeDef


def get_value() -> DeleteExtensionAssociationRequestTypeDef:
    return {
        "ExtensionAssociationId": ...,
    }


# DeleteExtensionAssociationRequestTypeDef definition

class DeleteExtensionAssociationRequestTypeDef(TypedDict):
    ExtensionAssociationId: str,
```

## DeleteExtensionRequestTypeDef

```python
# DeleteExtensionRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import DeleteExtensionRequestTypeDef


def get_value() -> DeleteExtensionRequestTypeDef:
    return {
        "ExtensionIdentifier": ...,
    }


# DeleteExtensionRequestTypeDef definition

class DeleteExtensionRequestTypeDef(TypedDict):
    ExtensionIdentifier: str,
    VersionNumber: NotRequired[int],
```

## DeleteHostedConfigurationVersionRequestTypeDef

```python
# DeleteHostedConfigurationVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import DeleteHostedConfigurationVersionRequestTypeDef


def get_value() -> DeleteHostedConfigurationVersionRequestTypeDef:
    return {
        "ApplicationId": ...,
    }


# DeleteHostedConfigurationVersionRequestTypeDef definition

class DeleteHostedConfigurationVersionRequestTypeDef(TypedDict):
    ApplicationId: str,
    ConfigurationProfileId: str,
    VersionNumber: int,
```

## DeploymentStrategyTypeDef

```python
# DeploymentStrategyTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import DeploymentStrategyTypeDef


def get_value() -> DeploymentStrategyTypeDef:
    return {
        "Id": ...,
    }


# DeploymentStrategyTypeDef definition

class DeploymentStrategyTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    DeploymentDurationInMinutes: NotRequired[int],
    GrowthType: NotRequired[GrowthTypeType],  # (1)
    GrowthFactor: NotRequired[float],
    FinalBakeTimeInMinutes: NotRequired[int],
    ReplicateTo: NotRequired[ReplicateToType],  # (2)
```

1. See [:material-code-brackets: GrowthTypeType](./literals.md#growthtypetype) 
2. See [:material-code-brackets: ReplicateToType](./literals.md#replicatetotype) 
## DeploymentSummaryTypeDef

```python
# DeploymentSummaryTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import DeploymentSummaryTypeDef


def get_value() -> DeploymentSummaryTypeDef:
    return {
        "DeploymentNumber": ...,
    }


# DeploymentSummaryTypeDef definition

class DeploymentSummaryTypeDef(TypedDict):
    DeploymentNumber: NotRequired[int],
    ConfigurationName: NotRequired[str],
    ConfigurationVersion: NotRequired[str],
    DeploymentDurationInMinutes: NotRequired[int],
    GrowthType: NotRequired[GrowthTypeType],  # (1)
    GrowthFactor: NotRequired[float],
    FinalBakeTimeInMinutes: NotRequired[int],
    State: NotRequired[DeploymentStateType],  # (2)
    PercentageComplete: NotRequired[float],
    StartedAt: NotRequired[datetime],
    CompletedAt: NotRequired[datetime],
    VersionLabel: NotRequired[str],
```

1. See [:material-code-brackets: GrowthTypeType](./literals.md#growthtypetype) 
2. See [:material-code-brackets: DeploymentStateType](./literals.md#deploymentstatetype) 
## ExtensionAssociationSummaryTypeDef

```python
# ExtensionAssociationSummaryTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ExtensionAssociationSummaryTypeDef


def get_value() -> ExtensionAssociationSummaryTypeDef:
    return {
        "Id": ...,
    }


# ExtensionAssociationSummaryTypeDef definition

class ExtensionAssociationSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    ExtensionArn: NotRequired[str],
    ResourceArn: NotRequired[str],
```

## ExtensionSummaryTypeDef

```python
# ExtensionSummaryTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ExtensionSummaryTypeDef


def get_value() -> ExtensionSummaryTypeDef:
    return {
        "Id": ...,
    }


# ExtensionSummaryTypeDef definition

class ExtensionSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    VersionNumber: NotRequired[int],
    Arn: NotRequired[str],
    Description: NotRequired[str],
```

## GetApplicationRequestTypeDef

```python
# GetApplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import GetApplicationRequestTypeDef


def get_value() -> GetApplicationRequestTypeDef:
    return {
        "ApplicationId": ...,
    }


# GetApplicationRequestTypeDef definition

class GetApplicationRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## GetConfigurationProfileRequestTypeDef

```python
# GetConfigurationProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import GetConfigurationProfileRequestTypeDef


def get_value() -> GetConfigurationProfileRequestTypeDef:
    return {
        "ApplicationId": ...,
    }


# GetConfigurationProfileRequestTypeDef definition

class GetConfigurationProfileRequestTypeDef(TypedDict):
    ApplicationId: str,
    ConfigurationProfileId: str,
```

## GetConfigurationRequestTypeDef

```python
# GetConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import GetConfigurationRequestTypeDef


def get_value() -> GetConfigurationRequestTypeDef:
    return {
        "Application": ...,
    }


# GetConfigurationRequestTypeDef definition

class GetConfigurationRequestTypeDef(TypedDict):
    Application: str,
    Environment: str,
    Configuration: str,
    ClientId: str,
    ClientConfigurationVersion: NotRequired[str],
```

## GetDeploymentRequestTypeDef

```python
# GetDeploymentRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import GetDeploymentRequestTypeDef


def get_value() -> GetDeploymentRequestTypeDef:
    return {
        "ApplicationId": ...,
    }


# GetDeploymentRequestTypeDef definition

class GetDeploymentRequestTypeDef(TypedDict):
    ApplicationId: str,
    EnvironmentId: str,
    DeploymentNumber: int,
```

## GetDeploymentStrategyRequestTypeDef

```python
# GetDeploymentStrategyRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import GetDeploymentStrategyRequestTypeDef


def get_value() -> GetDeploymentStrategyRequestTypeDef:
    return {
        "DeploymentStrategyId": ...,
    }


# GetDeploymentStrategyRequestTypeDef definition

class GetDeploymentStrategyRequestTypeDef(TypedDict):
    DeploymentStrategyId: str,
```

## GetEnvironmentRequestTypeDef

```python
# GetEnvironmentRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import GetEnvironmentRequestTypeDef


def get_value() -> GetEnvironmentRequestTypeDef:
    return {
        "ApplicationId": ...,
    }


# GetEnvironmentRequestTypeDef definition

class GetEnvironmentRequestTypeDef(TypedDict):
    ApplicationId: str,
    EnvironmentId: str,
```

## GetExtensionAssociationRequestTypeDef

```python
# GetExtensionAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import GetExtensionAssociationRequestTypeDef


def get_value() -> GetExtensionAssociationRequestTypeDef:
    return {
        "ExtensionAssociationId": ...,
    }


# GetExtensionAssociationRequestTypeDef definition

class GetExtensionAssociationRequestTypeDef(TypedDict):
    ExtensionAssociationId: str,
```

## GetExtensionRequestTypeDef

```python
# GetExtensionRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import GetExtensionRequestTypeDef


def get_value() -> GetExtensionRequestTypeDef:
    return {
        "ExtensionIdentifier": ...,
    }


# GetExtensionRequestTypeDef definition

class GetExtensionRequestTypeDef(TypedDict):
    ExtensionIdentifier: str,
    VersionNumber: NotRequired[int],
```

## GetHostedConfigurationVersionRequestTypeDef

```python
# GetHostedConfigurationVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import GetHostedConfigurationVersionRequestTypeDef


def get_value() -> GetHostedConfigurationVersionRequestTypeDef:
    return {
        "ApplicationId": ...,
    }


# GetHostedConfigurationVersionRequestTypeDef definition

class GetHostedConfigurationVersionRequestTypeDef(TypedDict):
    ApplicationId: str,
    ConfigurationProfileId: str,
    VersionNumber: int,
```

## HostedConfigurationVersionSummaryTypeDef

```python
# HostedConfigurationVersionSummaryTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import HostedConfigurationVersionSummaryTypeDef


def get_value() -> HostedConfigurationVersionSummaryTypeDef:
    return {
        "ApplicationId": ...,
    }


# HostedConfigurationVersionSummaryTypeDef definition

class HostedConfigurationVersionSummaryTypeDef(TypedDict):
    ApplicationId: NotRequired[str],
    ConfigurationProfileId: NotRequired[str],
    VersionNumber: NotRequired[int],
    Description: NotRequired[str],
    ContentType: NotRequired[str],
    VersionLabel: NotRequired[str],
    KmsKeyArn: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import PaginatorConfigTypeDef


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

## ListApplicationsRequestTypeDef

```python
# ListApplicationsRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ListApplicationsRequestTypeDef


def get_value() -> ListApplicationsRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListApplicationsRequestTypeDef definition

class ListApplicationsRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListConfigurationProfilesRequestTypeDef

```python
# ListConfigurationProfilesRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ListConfigurationProfilesRequestTypeDef


def get_value() -> ListConfigurationProfilesRequestTypeDef:
    return {
        "ApplicationId": ...,
    }


# ListConfigurationProfilesRequestTypeDef definition

class ListConfigurationProfilesRequestTypeDef(TypedDict):
    ApplicationId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Type: NotRequired[str],
```

## ListDeploymentStrategiesRequestTypeDef

```python
# ListDeploymentStrategiesRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ListDeploymentStrategiesRequestTypeDef


def get_value() -> ListDeploymentStrategiesRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListDeploymentStrategiesRequestTypeDef definition

class ListDeploymentStrategiesRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListDeploymentsRequestTypeDef

```python
# ListDeploymentsRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ListDeploymentsRequestTypeDef


def get_value() -> ListDeploymentsRequestTypeDef:
    return {
        "ApplicationId": ...,
    }


# ListDeploymentsRequestTypeDef definition

class ListDeploymentsRequestTypeDef(TypedDict):
    ApplicationId: str,
    EnvironmentId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListEnvironmentsRequestTypeDef

```python
# ListEnvironmentsRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ListEnvironmentsRequestTypeDef


def get_value() -> ListEnvironmentsRequestTypeDef:
    return {
        "ApplicationId": ...,
    }


# ListEnvironmentsRequestTypeDef definition

class ListEnvironmentsRequestTypeDef(TypedDict):
    ApplicationId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListExtensionAssociationsRequestTypeDef

```python
# ListExtensionAssociationsRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ListExtensionAssociationsRequestTypeDef


def get_value() -> ListExtensionAssociationsRequestTypeDef:
    return {
        "ResourceIdentifier": ...,
    }


# ListExtensionAssociationsRequestTypeDef definition

class ListExtensionAssociationsRequestTypeDef(TypedDict):
    ResourceIdentifier: NotRequired[str],
    ExtensionIdentifier: NotRequired[str],
    ExtensionVersionNumber: NotRequired[int],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListExtensionsRequestTypeDef

```python
# ListExtensionsRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ListExtensionsRequestTypeDef


def get_value() -> ListExtensionsRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListExtensionsRequestTypeDef definition

class ListExtensionsRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Name: NotRequired[str],
```

## ListHostedConfigurationVersionsRequestTypeDef

```python
# ListHostedConfigurationVersionsRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ListHostedConfigurationVersionsRequestTypeDef


def get_value() -> ListHostedConfigurationVersionsRequestTypeDef:
    return {
        "ApplicationId": ...,
    }


# ListHostedConfigurationVersionsRequestTypeDef definition

class ListHostedConfigurationVersionsRequestTypeDef(TypedDict):
    ApplicationId: str,
    ConfigurationProfileId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    VersionLabel: NotRequired[str],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## StartDeploymentRequestTypeDef

```python
# StartDeploymentRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import StartDeploymentRequestTypeDef


def get_value() -> StartDeploymentRequestTypeDef:
    return {
        "ApplicationId": ...,
    }


# StartDeploymentRequestTypeDef definition

class StartDeploymentRequestTypeDef(TypedDict):
    ApplicationId: str,
    EnvironmentId: str,
    DeploymentStrategyId: str,
    ConfigurationProfileId: str,
    ConfigurationVersion: str,
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    KmsKeyIdentifier: NotRequired[str],
    DynamicExtensionParameters: NotRequired[Mapping[str, str]],
```

## StopDeploymentRequestTypeDef

```python
# StopDeploymentRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import StopDeploymentRequestTypeDef


def get_value() -> StopDeploymentRequestTypeDef:
    return {
        "ApplicationId": ...,
    }


# StopDeploymentRequestTypeDef definition

class StopDeploymentRequestTypeDef(TypedDict):
    ApplicationId: str,
    EnvironmentId: str,
    DeploymentNumber: int,
    AllowRevert: NotRequired[bool],
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateApplicationRequestTypeDef

```python
# UpdateApplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import UpdateApplicationRequestTypeDef


def get_value() -> UpdateApplicationRequestTypeDef:
    return {
        "ApplicationId": ...,
    }


# UpdateApplicationRequestTypeDef definition

class UpdateApplicationRequestTypeDef(TypedDict):
    ApplicationId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
```

## UpdateDeploymentStrategyRequestTypeDef

```python
# UpdateDeploymentStrategyRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import UpdateDeploymentStrategyRequestTypeDef


def get_value() -> UpdateDeploymentStrategyRequestTypeDef:
    return {
        "DeploymentStrategyId": ...,
    }


# UpdateDeploymentStrategyRequestTypeDef definition

class UpdateDeploymentStrategyRequestTypeDef(TypedDict):
    DeploymentStrategyId: str,
    Description: NotRequired[str],
    DeploymentDurationInMinutes: NotRequired[int],
    FinalBakeTimeInMinutes: NotRequired[int],
    GrowthFactor: NotRequired[float],
    GrowthType: NotRequired[GrowthTypeType],  # (1)
```

1. See [:material-code-brackets: GrowthTypeType](./literals.md#growthtypetype) 
## UpdateExtensionAssociationRequestTypeDef

```python
# UpdateExtensionAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import UpdateExtensionAssociationRequestTypeDef


def get_value() -> UpdateExtensionAssociationRequestTypeDef:
    return {
        "ExtensionAssociationId": ...,
    }


# UpdateExtensionAssociationRequestTypeDef definition

class UpdateExtensionAssociationRequestTypeDef(TypedDict):
    ExtensionAssociationId: str,
    Parameters: NotRequired[Mapping[str, str]],
```

## ValidateConfigurationRequestTypeDef

```python
# ValidateConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ValidateConfigurationRequestTypeDef


def get_value() -> ValidateConfigurationRequestTypeDef:
    return {
        "ApplicationId": ...,
    }


# ValidateConfigurationRequestTypeDef definition

class ValidateConfigurationRequestTypeDef(TypedDict):
    ApplicationId: str,
    ConfigurationProfileId: str,
    ConfigurationVersion: str,
```

## UpdateAccountSettingsRequestTypeDef

```python
# UpdateAccountSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import UpdateAccountSettingsRequestTypeDef


def get_value() -> UpdateAccountSettingsRequestTypeDef:
    return {
        "DeletionProtection": ...,
    }


# UpdateAccountSettingsRequestTypeDef definition

class UpdateAccountSettingsRequestTypeDef(TypedDict):
    DeletionProtection: NotRequired[DeletionProtectionSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: DeletionProtectionSettingsTypeDef](./type_defs.md#deletionprotectionsettingstypedef) 
## AccountSettingsTypeDef

```python
# AccountSettingsTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import AccountSettingsTypeDef


def get_value() -> AccountSettingsTypeDef:
    return {
        "DeletionProtection": ...,
    }


# AccountSettingsTypeDef definition

class AccountSettingsTypeDef(TypedDict):
    DeletionProtection: DeletionProtectionSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeletionProtectionSettingsTypeDef](./type_defs.md#deletionprotectionsettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ApplicationResponseTypeDef

```python
# ApplicationResponseTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ApplicationResponseTypeDef


def get_value() -> ApplicationResponseTypeDef:
    return {
        "Id": ...,
    }


# ApplicationResponseTypeDef definition

class ApplicationResponseTypeDef(TypedDict):
    Id: str,
    Name: str,
    Description: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConfigurationTypeDef

```python
# ConfigurationTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ConfigurationTypeDef


def get_value() -> ConfigurationTypeDef:
    return {
        "Content": ...,
    }


# ConfigurationTypeDef definition

class ConfigurationTypeDef(TypedDict):
    Content: StreamingBody,
    ConfigurationVersion: str,
    ContentType: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeploymentStrategyResponseTypeDef

```python
# DeploymentStrategyResponseTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import DeploymentStrategyResponseTypeDef


def get_value() -> DeploymentStrategyResponseTypeDef:
    return {
        "Id": ...,
    }


# DeploymentStrategyResponseTypeDef definition

class DeploymentStrategyResponseTypeDef(TypedDict):
    Id: str,
    Name: str,
    Description: str,
    DeploymentDurationInMinutes: int,
    GrowthType: GrowthTypeType,  # (1)
    GrowthFactor: float,
    FinalBakeTimeInMinutes: int,
    ReplicateTo: ReplicateToType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: GrowthTypeType](./literals.md#growthtypetype) 
2. See [:material-code-brackets: ReplicateToType](./literals.md#replicatetotype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExtensionAssociationTypeDef

```python
# ExtensionAssociationTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ExtensionAssociationTypeDef


def get_value() -> ExtensionAssociationTypeDef:
    return {
        "Id": ...,
    }


# ExtensionAssociationTypeDef definition

class ExtensionAssociationTypeDef(TypedDict):
    Id: str,
    ExtensionArn: str,
    ResourceArn: str,
    Arn: str,
    Parameters: Dict[str, str],
    ExtensionVersionNumber: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HostedConfigurationVersionTypeDef

```python
# HostedConfigurationVersionTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import HostedConfigurationVersionTypeDef


def get_value() -> HostedConfigurationVersionTypeDef:
    return {
        "ApplicationId": ...,
    }


# HostedConfigurationVersionTypeDef definition

class HostedConfigurationVersionTypeDef(TypedDict):
    ApplicationId: str,
    ConfigurationProfileId: str,
    VersionNumber: int,
    Description: str,
    Content: StreamingBody,
    ContentType: str,
    VersionLabel: str,
    KmsKeyArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResourceTagsTypeDef

```python
# ResourceTagsTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ResourceTagsTypeDef


def get_value() -> ResourceTagsTypeDef:
    return {
        "Tags": ...,
    }


# ResourceTagsTypeDef definition

class ResourceTagsTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeploymentEventTypeDef

```python
# DeploymentEventTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import DeploymentEventTypeDef


def get_value() -> DeploymentEventTypeDef:
    return {
        "EventType": ...,
    }


# DeploymentEventTypeDef definition

class DeploymentEventTypeDef(TypedDict):
    EventType: NotRequired[DeploymentEventTypeType],  # (1)
    TriggeredBy: NotRequired[TriggeredByType],  # (2)
    Description: NotRequired[str],
    ActionInvocations: NotRequired[List[ActionInvocationTypeDef]],  # (3)
    OccurredAt: NotRequired[datetime],
```

1. See [:material-code-brackets: DeploymentEventTypeType](./literals.md#deploymenteventtypetype) 
2. See [:material-code-brackets: TriggeredByType](./literals.md#triggeredbytype) 
3. See [:material-code-braces: ActionInvocationTypeDef](./type_defs.md#actioninvocationtypedef) 
## ApplicationsTypeDef

```python
# ApplicationsTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ApplicationsTypeDef


def get_value() -> ApplicationsTypeDef:
    return {
        "Items": ...,
    }


# ApplicationsTypeDef definition

class ApplicationsTypeDef(TypedDict):
    Items: List[ApplicationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ApplicationTypeDef](./type_defs.md#applicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateHostedConfigurationVersionRequestTypeDef

```python
# CreateHostedConfigurationVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import CreateHostedConfigurationVersionRequestTypeDef


def get_value() -> CreateHostedConfigurationVersionRequestTypeDef:
    return {
        "ApplicationId": ...,
    }


# CreateHostedConfigurationVersionRequestTypeDef definition

class CreateHostedConfigurationVersionRequestTypeDef(TypedDict):
    ApplicationId: str,
    ConfigurationProfileId: str,
    Content: BlobTypeDef,
    ContentType: str,
    Description: NotRequired[str],
    LatestVersionNumber: NotRequired[int],
    VersionLabel: NotRequired[str],
```

## ConfigurationProfilesTypeDef

```python
# ConfigurationProfilesTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ConfigurationProfilesTypeDef


def get_value() -> ConfigurationProfilesTypeDef:
    return {
        "Items": ...,
    }


# ConfigurationProfilesTypeDef definition

class ConfigurationProfilesTypeDef(TypedDict):
    Items: List[ConfigurationProfileSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConfigurationProfileSummaryTypeDef](./type_defs.md#configurationprofilesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConfigurationProfileTypeDef

```python
# ConfigurationProfileTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ConfigurationProfileTypeDef


def get_value() -> ConfigurationProfileTypeDef:
    return {
        "ApplicationId": ...,
    }


# ConfigurationProfileTypeDef definition

class ConfigurationProfileTypeDef(TypedDict):
    ApplicationId: str,
    Id: str,
    Name: str,
    Description: str,
    LocationUri: str,
    RetrievalRoleArn: str,
    Validators: List[ValidatorTypeDef],  # (1)
    Type: str,
    KmsKeyArn: str,
    KmsKeyIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ValidatorTypeDef](./type_defs.md#validatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConfigurationProfileRequestTypeDef

```python
# CreateConfigurationProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import CreateConfigurationProfileRequestTypeDef


def get_value() -> CreateConfigurationProfileRequestTypeDef:
    return {
        "ApplicationId": ...,
    }


# CreateConfigurationProfileRequestTypeDef definition

class CreateConfigurationProfileRequestTypeDef(TypedDict):
    ApplicationId: str,
    Name: str,
    LocationUri: str,
    Description: NotRequired[str],
    RetrievalRoleArn: NotRequired[str],
    Validators: NotRequired[Sequence[ValidatorTypeDef]],  # (1)
    Tags: NotRequired[Mapping[str, str]],
    Type: NotRequired[str],
    KmsKeyIdentifier: NotRequired[str],
```

1. See [:material-code-braces: ValidatorTypeDef](./type_defs.md#validatortypedef) 
## UpdateConfigurationProfileRequestTypeDef

```python
# UpdateConfigurationProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import UpdateConfigurationProfileRequestTypeDef


def get_value() -> UpdateConfigurationProfileRequestTypeDef:
    return {
        "ApplicationId": ...,
    }


# UpdateConfigurationProfileRequestTypeDef definition

class UpdateConfigurationProfileRequestTypeDef(TypedDict):
    ApplicationId: str,
    ConfigurationProfileId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    RetrievalRoleArn: NotRequired[str],
    Validators: NotRequired[Sequence[ValidatorTypeDef]],  # (1)
    KmsKeyIdentifier: NotRequired[str],
```

1. See [:material-code-braces: ValidatorTypeDef](./type_defs.md#validatortypedef) 
## CreateEnvironmentRequestTypeDef

```python
# CreateEnvironmentRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import CreateEnvironmentRequestTypeDef


def get_value() -> CreateEnvironmentRequestTypeDef:
    return {
        "ApplicationId": ...,
    }


# CreateEnvironmentRequestTypeDef definition

class CreateEnvironmentRequestTypeDef(TypedDict):
    ApplicationId: str,
    Name: str,
    Description: NotRequired[str],
    Monitors: NotRequired[Sequence[MonitorTypeDef]],  # (1)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: MonitorTypeDef](./type_defs.md#monitortypedef) 
## EnvironmentResponseTypeDef

```python
# EnvironmentResponseTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import EnvironmentResponseTypeDef


def get_value() -> EnvironmentResponseTypeDef:
    return {
        "ApplicationId": ...,
    }


# EnvironmentResponseTypeDef definition

class EnvironmentResponseTypeDef(TypedDict):
    ApplicationId: str,
    Id: str,
    Name: str,
    Description: str,
    State: EnvironmentStateType,  # (1)
    Monitors: List[MonitorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: EnvironmentStateType](./literals.md#environmentstatetype) 
2. See [:material-code-braces: MonitorTypeDef](./type_defs.md#monitortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnvironmentTypeDef

```python
# EnvironmentTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import EnvironmentTypeDef


def get_value() -> EnvironmentTypeDef:
    return {
        "ApplicationId": ...,
    }


# EnvironmentTypeDef definition

class EnvironmentTypeDef(TypedDict):
    ApplicationId: NotRequired[str],
    Id: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    State: NotRequired[EnvironmentStateType],  # (1)
    Monitors: NotRequired[List[MonitorTypeDef]],  # (2)
```

1. See [:material-code-brackets: EnvironmentStateType](./literals.md#environmentstatetype) 
2. See [:material-code-braces: MonitorTypeDef](./type_defs.md#monitortypedef) 
## UpdateEnvironmentRequestTypeDef

```python
# UpdateEnvironmentRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import UpdateEnvironmentRequestTypeDef


def get_value() -> UpdateEnvironmentRequestTypeDef:
    return {
        "ApplicationId": ...,
    }


# UpdateEnvironmentRequestTypeDef definition

class UpdateEnvironmentRequestTypeDef(TypedDict):
    ApplicationId: str,
    EnvironmentId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    Monitors: NotRequired[Sequence[MonitorTypeDef]],  # (1)
```

1. See [:material-code-braces: MonitorTypeDef](./type_defs.md#monitortypedef) 
## CreateExtensionRequestTypeDef

```python
# CreateExtensionRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import CreateExtensionRequestTypeDef


def get_value() -> CreateExtensionRequestTypeDef:
    return {
        "Name": ...,
    }


# CreateExtensionRequestTypeDef definition

class CreateExtensionRequestTypeDef(TypedDict):
    Name: str,
    Actions: Mapping[ActionPointType, Sequence[ActionTypeDef]],  # (1)
    Description: NotRequired[str],
    Parameters: NotRequired[Mapping[str, ParameterTypeDef]],  # (2)
    Tags: NotRequired[Mapping[str, str]],
    LatestVersionNumber: NotRequired[int],
```

1. See [:material-code-brackets: ActionPointType](./literals.md#actionpointtype) [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
## ExtensionTypeDef

```python
# ExtensionTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ExtensionTypeDef


def get_value() -> ExtensionTypeDef:
    return {
        "Id": ...,
    }


# ExtensionTypeDef definition

class ExtensionTypeDef(TypedDict):
    Id: str,
    Name: str,
    VersionNumber: int,
    Arn: str,
    Description: str,
    Actions: Dict[ActionPointType, List[ActionTypeDef]],  # (1)
    Parameters: Dict[str, ParameterTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ActionPointType](./literals.md#actionpointtype) [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateExtensionRequestTypeDef

```python
# UpdateExtensionRequestTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import UpdateExtensionRequestTypeDef


def get_value() -> UpdateExtensionRequestTypeDef:
    return {
        "ExtensionIdentifier": ...,
    }


# UpdateExtensionRequestTypeDef definition

class UpdateExtensionRequestTypeDef(TypedDict):
    ExtensionIdentifier: str,
    Description: NotRequired[str],
    Actions: NotRequired[Mapping[ActionPointType, Sequence[ActionTypeDef]]],  # (1)
    Parameters: NotRequired[Mapping[str, ParameterTypeDef]],  # (2)
    VersionNumber: NotRequired[int],
```

1. See [:material-code-brackets: ActionPointType](./literals.md#actionpointtype) [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
## DeploymentStrategiesTypeDef

```python
# DeploymentStrategiesTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import DeploymentStrategiesTypeDef


def get_value() -> DeploymentStrategiesTypeDef:
    return {
        "Items": ...,
    }


# DeploymentStrategiesTypeDef definition

class DeploymentStrategiesTypeDef(TypedDict):
    Items: List[DeploymentStrategyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DeploymentStrategyTypeDef](./type_defs.md#deploymentstrategytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeploymentsTypeDef

```python
# DeploymentsTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import DeploymentsTypeDef


def get_value() -> DeploymentsTypeDef:
    return {
        "Items": ...,
    }


# DeploymentsTypeDef definition

class DeploymentsTypeDef(TypedDict):
    Items: List[DeploymentSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DeploymentSummaryTypeDef](./type_defs.md#deploymentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExtensionAssociationsTypeDef

```python
# ExtensionAssociationsTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ExtensionAssociationsTypeDef


def get_value() -> ExtensionAssociationsTypeDef:
    return {
        "Items": ...,
    }


# ExtensionAssociationsTypeDef definition

class ExtensionAssociationsTypeDef(TypedDict):
    Items: List[ExtensionAssociationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ExtensionAssociationSummaryTypeDef](./type_defs.md#extensionassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExtensionsTypeDef

```python
# ExtensionsTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ExtensionsTypeDef


def get_value() -> ExtensionsTypeDef:
    return {
        "Items": ...,
    }


# ExtensionsTypeDef definition

class ExtensionsTypeDef(TypedDict):
    Items: List[ExtensionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ExtensionSummaryTypeDef](./type_defs.md#extensionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HostedConfigurationVersionsTypeDef

```python
# HostedConfigurationVersionsTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import HostedConfigurationVersionsTypeDef


def get_value() -> HostedConfigurationVersionsTypeDef:
    return {
        "Items": ...,
    }


# HostedConfigurationVersionsTypeDef definition

class HostedConfigurationVersionsTypeDef(TypedDict):
    Items: List[HostedConfigurationVersionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: HostedConfigurationVersionSummaryTypeDef](./type_defs.md#hostedconfigurationversionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApplicationsRequestPaginateTypeDef

```python
# ListApplicationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ListApplicationsRequestPaginateTypeDef


def get_value() -> ListApplicationsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListApplicationsRequestPaginateTypeDef definition

class ListApplicationsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConfigurationProfilesRequestPaginateTypeDef

```python
# ListConfigurationProfilesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ListConfigurationProfilesRequestPaginateTypeDef


def get_value() -> ListConfigurationProfilesRequestPaginateTypeDef:
    return {
        "ApplicationId": ...,
    }


# ListConfigurationProfilesRequestPaginateTypeDef definition

class ListConfigurationProfilesRequestPaginateTypeDef(TypedDict):
    ApplicationId: str,
    Type: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDeploymentStrategiesRequestPaginateTypeDef

```python
# ListDeploymentStrategiesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ListDeploymentStrategiesRequestPaginateTypeDef


def get_value() -> ListDeploymentStrategiesRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListDeploymentStrategiesRequestPaginateTypeDef definition

class ListDeploymentStrategiesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDeploymentsRequestPaginateTypeDef

```python
# ListDeploymentsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ListDeploymentsRequestPaginateTypeDef


def get_value() -> ListDeploymentsRequestPaginateTypeDef:
    return {
        "ApplicationId": ...,
    }


# ListDeploymentsRequestPaginateTypeDef definition

class ListDeploymentsRequestPaginateTypeDef(TypedDict):
    ApplicationId: str,
    EnvironmentId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEnvironmentsRequestPaginateTypeDef

```python
# ListEnvironmentsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ListEnvironmentsRequestPaginateTypeDef


def get_value() -> ListEnvironmentsRequestPaginateTypeDef:
    return {
        "ApplicationId": ...,
    }


# ListEnvironmentsRequestPaginateTypeDef definition

class ListEnvironmentsRequestPaginateTypeDef(TypedDict):
    ApplicationId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListExtensionAssociationsRequestPaginateTypeDef

```python
# ListExtensionAssociationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ListExtensionAssociationsRequestPaginateTypeDef


def get_value() -> ListExtensionAssociationsRequestPaginateTypeDef:
    return {
        "ResourceIdentifier": ...,
    }


# ListExtensionAssociationsRequestPaginateTypeDef definition

class ListExtensionAssociationsRequestPaginateTypeDef(TypedDict):
    ResourceIdentifier: NotRequired[str],
    ExtensionIdentifier: NotRequired[str],
    ExtensionVersionNumber: NotRequired[int],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListExtensionsRequestPaginateTypeDef

```python
# ListExtensionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ListExtensionsRequestPaginateTypeDef


def get_value() -> ListExtensionsRequestPaginateTypeDef:
    return {
        "Name": ...,
    }


# ListExtensionsRequestPaginateTypeDef definition

class ListExtensionsRequestPaginateTypeDef(TypedDict):
    Name: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListHostedConfigurationVersionsRequestPaginateTypeDef

```python
# ListHostedConfigurationVersionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import ListHostedConfigurationVersionsRequestPaginateTypeDef


def get_value() -> ListHostedConfigurationVersionsRequestPaginateTypeDef:
    return {
        "ApplicationId": ...,
    }


# ListHostedConfigurationVersionsRequestPaginateTypeDef definition

class ListHostedConfigurationVersionsRequestPaginateTypeDef(TypedDict):
    ApplicationId: str,
    ConfigurationProfileId: str,
    VersionLabel: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DeploymentTypeDef

```python
# DeploymentTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import DeploymentTypeDef


def get_value() -> DeploymentTypeDef:
    return {
        "ApplicationId": ...,
    }


# DeploymentTypeDef definition

class DeploymentTypeDef(TypedDict):
    ApplicationId: str,
    EnvironmentId: str,
    DeploymentStrategyId: str,
    ConfigurationProfileId: str,
    DeploymentNumber: int,
    ConfigurationName: str,
    ConfigurationLocationUri: str,
    ConfigurationVersion: str,
    Description: str,
    DeploymentDurationInMinutes: int,
    GrowthType: GrowthTypeType,  # (1)
    GrowthFactor: float,
    FinalBakeTimeInMinutes: int,
    State: DeploymentStateType,  # (2)
    EventLog: List[DeploymentEventTypeDef],  # (3)
    PercentageComplete: float,
    StartedAt: datetime,
    CompletedAt: datetime,
    AppliedExtensions: List[AppliedExtensionTypeDef],  # (4)
    KmsKeyArn: str,
    KmsKeyIdentifier: str,
    VersionLabel: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: GrowthTypeType](./literals.md#growthtypetype) 
2. See [:material-code-brackets: DeploymentStateType](./literals.md#deploymentstatetype) 
3. See [:material-code-braces: DeploymentEventTypeDef](./type_defs.md#deploymenteventtypedef) 
4. See [:material-code-braces: AppliedExtensionTypeDef](./type_defs.md#appliedextensiontypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnvironmentsTypeDef

```python
# EnvironmentsTypeDef TypedDict usage example

from types_aiobotocore_appconfig.type_defs import EnvironmentsTypeDef


def get_value() -> EnvironmentsTypeDef:
    return {
        "Items": ...,
    }


# EnvironmentsTypeDef definition

class EnvironmentsTypeDef(TypedDict):
    Items: List[EnvironmentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
