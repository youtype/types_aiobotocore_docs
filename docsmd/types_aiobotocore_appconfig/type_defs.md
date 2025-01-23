# Type definitions

> [Index](../README.md) > [AppConfig](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [AppConfig](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#appconfig)
    type annotations stubs module [types-aiobotocore-appconfig](https://pypi.org/project/types-aiobotocore-appconfig/).

## BlobTypeDef

```python
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
# DeletionProtectionSettingsTypeDef definition

class DeletionProtectionSettingsTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    ProtectionPeriodInMinutes: NotRequired[int],
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

## ActionInvocationTypeDef

```python
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
# ActionTypeDef definition

class ActionTypeDef(TypedDict):
    Name: NotRequired[str],
    Description: NotRequired[str],
    Uri: NotRequired[str],
    RoleArn: NotRequired[str],
```

## ApplicationTypeDef

```python
# ApplicationTypeDef definition

class ApplicationTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
```

## AppliedExtensionTypeDef

```python
# AppliedExtensionTypeDef definition

class AppliedExtensionTypeDef(TypedDict):
    ExtensionId: NotRequired[str],
    ExtensionAssociationId: NotRequired[str],
    VersionNumber: NotRequired[int],
    Parameters: NotRequired[Dict[str, str]],
```

## ConfigurationProfileSummaryTypeDef

```python
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
# ValidatorTypeDef definition

class ValidatorTypeDef(TypedDict):
    Type: ValidatorTypeType,  # (1)
    Content: str,
```

1. See [:material-code-brackets: ValidatorTypeType](./literals.md#validatortypetype) 
## CreateApplicationRequestRequestTypeDef

```python
# CreateApplicationRequestRequestTypeDef definition

class CreateApplicationRequestRequestTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

## CreateDeploymentStrategyRequestRequestTypeDef

```python
# CreateDeploymentStrategyRequestRequestTypeDef definition

class CreateDeploymentStrategyRequestRequestTypeDef(TypedDict):
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
# MonitorTypeDef definition

class MonitorTypeDef(TypedDict):
    AlarmArn: str,
    AlarmRoleArn: NotRequired[str],
```

## CreateExtensionAssociationRequestRequestTypeDef

```python
# CreateExtensionAssociationRequestRequestTypeDef definition

class CreateExtensionAssociationRequestRequestTypeDef(TypedDict):
    ExtensionIdentifier: str,
    ResourceIdentifier: str,
    ExtensionVersionNumber: NotRequired[int],
    Parameters: NotRequired[Mapping[str, str]],
    Tags: NotRequired[Mapping[str, str]],
```

## ParameterTypeDef

```python
# ParameterTypeDef definition

class ParameterTypeDef(TypedDict):
    Description: NotRequired[str],
    Required: NotRequired[bool],
    Dynamic: NotRequired[bool],
```

## DeleteApplicationRequestRequestTypeDef

```python
# DeleteApplicationRequestRequestTypeDef definition

class DeleteApplicationRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## DeleteConfigurationProfileRequestRequestTypeDef

```python
# DeleteConfigurationProfileRequestRequestTypeDef definition

class DeleteConfigurationProfileRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    ConfigurationProfileId: str,
    DeletionProtectionCheck: NotRequired[DeletionProtectionCheckType],  # (1)
```

1. See [:material-code-brackets: DeletionProtectionCheckType](./literals.md#deletionprotectionchecktype) 
## DeleteDeploymentStrategyRequestRequestTypeDef

```python
# DeleteDeploymentStrategyRequestRequestTypeDef definition

class DeleteDeploymentStrategyRequestRequestTypeDef(TypedDict):
    DeploymentStrategyId: str,
```

## DeleteEnvironmentRequestRequestTypeDef

```python
# DeleteEnvironmentRequestRequestTypeDef definition

class DeleteEnvironmentRequestRequestTypeDef(TypedDict):
    EnvironmentId: str,
    ApplicationId: str,
    DeletionProtectionCheck: NotRequired[DeletionProtectionCheckType],  # (1)
```

1. See [:material-code-brackets: DeletionProtectionCheckType](./literals.md#deletionprotectionchecktype) 
## DeleteExtensionAssociationRequestRequestTypeDef

```python
# DeleteExtensionAssociationRequestRequestTypeDef definition

class DeleteExtensionAssociationRequestRequestTypeDef(TypedDict):
    ExtensionAssociationId: str,
```

## DeleteExtensionRequestRequestTypeDef

```python
# DeleteExtensionRequestRequestTypeDef definition

class DeleteExtensionRequestRequestTypeDef(TypedDict):
    ExtensionIdentifier: str,
    VersionNumber: NotRequired[int],
```

## DeleteHostedConfigurationVersionRequestRequestTypeDef

```python
# DeleteHostedConfigurationVersionRequestRequestTypeDef definition

class DeleteHostedConfigurationVersionRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    ConfigurationProfileId: str,
    VersionNumber: int,
```

## DeploymentStrategyTypeDef

```python
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
# ExtensionAssociationSummaryTypeDef definition

class ExtensionAssociationSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    ExtensionArn: NotRequired[str],
    ResourceArn: NotRequired[str],
```

## ExtensionSummaryTypeDef

```python
# ExtensionSummaryTypeDef definition

class ExtensionSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    VersionNumber: NotRequired[int],
    Arn: NotRequired[str],
    Description: NotRequired[str],
```

## GetApplicationRequestRequestTypeDef

```python
# GetApplicationRequestRequestTypeDef definition

class GetApplicationRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## GetConfigurationProfileRequestRequestTypeDef

```python
# GetConfigurationProfileRequestRequestTypeDef definition

class GetConfigurationProfileRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    ConfigurationProfileId: str,
```

## GetConfigurationRequestRequestTypeDef

```python
# GetConfigurationRequestRequestTypeDef definition

class GetConfigurationRequestRequestTypeDef(TypedDict):
    Application: str,
    Environment: str,
    Configuration: str,
    ClientId: str,
    ClientConfigurationVersion: NotRequired[str],
```

## GetDeploymentRequestRequestTypeDef

```python
# GetDeploymentRequestRequestTypeDef definition

class GetDeploymentRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    EnvironmentId: str,
    DeploymentNumber: int,
```

## GetDeploymentStrategyRequestRequestTypeDef

```python
# GetDeploymentStrategyRequestRequestTypeDef definition

class GetDeploymentStrategyRequestRequestTypeDef(TypedDict):
    DeploymentStrategyId: str,
```

## GetEnvironmentRequestRequestTypeDef

```python
# GetEnvironmentRequestRequestTypeDef definition

class GetEnvironmentRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    EnvironmentId: str,
```

## GetExtensionAssociationRequestRequestTypeDef

```python
# GetExtensionAssociationRequestRequestTypeDef definition

class GetExtensionAssociationRequestRequestTypeDef(TypedDict):
    ExtensionAssociationId: str,
```

## GetExtensionRequestRequestTypeDef

```python
# GetExtensionRequestRequestTypeDef definition

class GetExtensionRequestRequestTypeDef(TypedDict):
    ExtensionIdentifier: str,
    VersionNumber: NotRequired[int],
```

## GetHostedConfigurationVersionRequestRequestTypeDef

```python
# GetHostedConfigurationVersionRequestRequestTypeDef definition

class GetHostedConfigurationVersionRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    ConfigurationProfileId: str,
    VersionNumber: int,
```

## HostedConfigurationVersionSummaryTypeDef

```python
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
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListApplicationsRequestRequestTypeDef

```python
# ListApplicationsRequestRequestTypeDef definition

class ListApplicationsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListConfigurationProfilesRequestRequestTypeDef

```python
# ListConfigurationProfilesRequestRequestTypeDef definition

class ListConfigurationProfilesRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Type: NotRequired[str],
```

## ListDeploymentStrategiesRequestRequestTypeDef

```python
# ListDeploymentStrategiesRequestRequestTypeDef definition

class ListDeploymentStrategiesRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListDeploymentsRequestRequestTypeDef

```python
# ListDeploymentsRequestRequestTypeDef definition

class ListDeploymentsRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    EnvironmentId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListEnvironmentsRequestRequestTypeDef

```python
# ListEnvironmentsRequestRequestTypeDef definition

class ListEnvironmentsRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListExtensionAssociationsRequestRequestTypeDef

```python
# ListExtensionAssociationsRequestRequestTypeDef definition

class ListExtensionAssociationsRequestRequestTypeDef(TypedDict):
    ResourceIdentifier: NotRequired[str],
    ExtensionIdentifier: NotRequired[str],
    ExtensionVersionNumber: NotRequired[int],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListExtensionsRequestRequestTypeDef

```python
# ListExtensionsRequestRequestTypeDef definition

class ListExtensionsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Name: NotRequired[str],
```

## ListHostedConfigurationVersionsRequestRequestTypeDef

```python
# ListHostedConfigurationVersionsRequestRequestTypeDef definition

class ListHostedConfigurationVersionsRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    ConfigurationProfileId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    VersionLabel: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## StartDeploymentRequestRequestTypeDef

```python
# StartDeploymentRequestRequestTypeDef definition

class StartDeploymentRequestRequestTypeDef(TypedDict):
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

## StopDeploymentRequestRequestTypeDef

```python
# StopDeploymentRequestRequestTypeDef definition

class StopDeploymentRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    EnvironmentId: str,
    DeploymentNumber: int,
    AllowRevert: NotRequired[bool],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateApplicationRequestRequestTypeDef

```python
# UpdateApplicationRequestRequestTypeDef definition

class UpdateApplicationRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
```

## UpdateDeploymentStrategyRequestRequestTypeDef

```python
# UpdateDeploymentStrategyRequestRequestTypeDef definition

class UpdateDeploymentStrategyRequestRequestTypeDef(TypedDict):
    DeploymentStrategyId: str,
    Description: NotRequired[str],
    DeploymentDurationInMinutes: NotRequired[int],
    FinalBakeTimeInMinutes: NotRequired[int],
    GrowthFactor: NotRequired[float],
    GrowthType: NotRequired[GrowthTypeType],  # (1)
```

1. See [:material-code-brackets: GrowthTypeType](./literals.md#growthtypetype) 
## UpdateExtensionAssociationRequestRequestTypeDef

```python
# UpdateExtensionAssociationRequestRequestTypeDef definition

class UpdateExtensionAssociationRequestRequestTypeDef(TypedDict):
    ExtensionAssociationId: str,
    Parameters: NotRequired[Mapping[str, str]],
```

## ValidateConfigurationRequestRequestTypeDef

```python
# ValidateConfigurationRequestRequestTypeDef definition

class ValidateConfigurationRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    ConfigurationProfileId: str,
    ConfigurationVersion: str,
```

## UpdateAccountSettingsRequestRequestTypeDef

```python
# UpdateAccountSettingsRequestRequestTypeDef definition

class UpdateAccountSettingsRequestRequestTypeDef(TypedDict):
    DeletionProtection: NotRequired[DeletionProtectionSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: DeletionProtectionSettingsTypeDef](./type_defs.md#deletionprotectionsettingstypedef) 
## AccountSettingsTypeDef

```python
# AccountSettingsTypeDef definition

class AccountSettingsTypeDef(TypedDict):
    DeletionProtection: DeletionProtectionSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeletionProtectionSettingsTypeDef](./type_defs.md#deletionprotectionsettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ApplicationResponseTypeDef

```python
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
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExtensionAssociationTypeDef

```python
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
# ResourceTagsTypeDef definition

class ResourceTagsTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeploymentEventTypeDef

```python
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
# ApplicationsTypeDef definition

class ApplicationsTypeDef(TypedDict):
    Items: List[ApplicationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ApplicationTypeDef](./type_defs.md#applicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateHostedConfigurationVersionRequestRequestTypeDef

```python
# CreateHostedConfigurationVersionRequestRequestTypeDef definition

class CreateHostedConfigurationVersionRequestRequestTypeDef(TypedDict):
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
## CreateConfigurationProfileRequestRequestTypeDef

```python
# CreateConfigurationProfileRequestRequestTypeDef definition

class CreateConfigurationProfileRequestRequestTypeDef(TypedDict):
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
## UpdateConfigurationProfileRequestRequestTypeDef

```python
# UpdateConfigurationProfileRequestRequestTypeDef definition

class UpdateConfigurationProfileRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    ConfigurationProfileId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    RetrievalRoleArn: NotRequired[str],
    Validators: NotRequired[Sequence[ValidatorTypeDef]],  # (1)
    KmsKeyIdentifier: NotRequired[str],
```

1. See [:material-code-braces: ValidatorTypeDef](./type_defs.md#validatortypedef) 
## CreateEnvironmentRequestRequestTypeDef

```python
# CreateEnvironmentRequestRequestTypeDef definition

class CreateEnvironmentRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    Name: str,
    Description: NotRequired[str],
    Monitors: NotRequired[Sequence[MonitorTypeDef]],  # (1)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: MonitorTypeDef](./type_defs.md#monitortypedef) 
## EnvironmentResponseTypeDef

```python
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
## UpdateEnvironmentRequestRequestTypeDef

```python
# UpdateEnvironmentRequestRequestTypeDef definition

class UpdateEnvironmentRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    EnvironmentId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    Monitors: NotRequired[Sequence[MonitorTypeDef]],  # (1)
```

1. See [:material-code-braces: MonitorTypeDef](./type_defs.md#monitortypedef) 
## CreateExtensionRequestRequestTypeDef

```python
# CreateExtensionRequestRequestTypeDef definition

class CreateExtensionRequestRequestTypeDef(TypedDict):
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
## UpdateExtensionRequestRequestTypeDef

```python
# UpdateExtensionRequestRequestTypeDef definition

class UpdateExtensionRequestRequestTypeDef(TypedDict):
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
# ListApplicationsRequestPaginateTypeDef definition

class ListApplicationsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConfigurationProfilesRequestPaginateTypeDef

```python
# ListConfigurationProfilesRequestPaginateTypeDef definition

class ListConfigurationProfilesRequestPaginateTypeDef(TypedDict):
    ApplicationId: str,
    Type: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDeploymentStrategiesRequestPaginateTypeDef

```python
# ListDeploymentStrategiesRequestPaginateTypeDef definition

class ListDeploymentStrategiesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDeploymentsRequestPaginateTypeDef

```python
# ListDeploymentsRequestPaginateTypeDef definition

class ListDeploymentsRequestPaginateTypeDef(TypedDict):
    ApplicationId: str,
    EnvironmentId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEnvironmentsRequestPaginateTypeDef

```python
# ListEnvironmentsRequestPaginateTypeDef definition

class ListEnvironmentsRequestPaginateTypeDef(TypedDict):
    ApplicationId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListExtensionAssociationsRequestPaginateTypeDef

```python
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
# ListExtensionsRequestPaginateTypeDef definition

class ListExtensionsRequestPaginateTypeDef(TypedDict):
    Name: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListHostedConfigurationVersionsRequestPaginateTypeDef

```python
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
# EnvironmentsTypeDef definition

class EnvironmentsTypeDef(TypedDict):
    Items: List[EnvironmentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
