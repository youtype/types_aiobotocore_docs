# Type definitions

> [Index](../README.md) > [ElasticBeanstalk](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ElasticBeanstalk](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
    type annotations stubs module [types-aiobotocore-elasticbeanstalk](https://pypi.org/project/types-aiobotocore-elasticbeanstalk/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AbortEnvironmentUpdateMessageRequestTypeDef

```python
# AbortEnvironmentUpdateMessageRequestTypeDef definition

class AbortEnvironmentUpdateMessageRequestTypeDef(TypedDict):
    EnvironmentId: NotRequired[str],
    EnvironmentName: NotRequired[str],
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

## LatencyTypeDef

```python
# LatencyTypeDef definition

class LatencyTypeDef(TypedDict):
    P999: NotRequired[float],
    P99: NotRequired[float],
    P95: NotRequired[float],
    P90: NotRequired[float],
    P85: NotRequired[float],
    P75: NotRequired[float],
    P50: NotRequired[float],
    P10: NotRequired[float],
```

## StatusCodesTypeDef

```python
# StatusCodesTypeDef definition

class StatusCodesTypeDef(TypedDict):
    Status2xx: NotRequired[int],
    Status3xx: NotRequired[int],
    Status4xx: NotRequired[int],
    Status5xx: NotRequired[int],
```

## S3LocationTypeDef

```python
# S3LocationTypeDef definition

class S3LocationTypeDef(TypedDict):
    S3Bucket: NotRequired[str],
    S3Key: NotRequired[str],
```

## SourceBuildInformationTypeDef

```python
# SourceBuildInformationTypeDef definition

class SourceBuildInformationTypeDef(TypedDict):
    SourceType: SourceTypeType,  # (1)
    SourceRepository: SourceRepositoryType,  # (2)
    SourceLocation: str,
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
2. See [:material-code-brackets: SourceRepositoryType](./literals.md#sourcerepositorytype) 
## MaxAgeRuleTypeDef

```python
# MaxAgeRuleTypeDef definition

class MaxAgeRuleTypeDef(TypedDict):
    Enabled: bool,
    MaxAgeInDays: NotRequired[int],
    DeleteSourceFromS3: NotRequired[bool],
```

## MaxCountRuleTypeDef

```python
# MaxCountRuleTypeDef definition

class MaxCountRuleTypeDef(TypedDict):
    Enabled: bool,
    MaxCount: NotRequired[int],
    DeleteSourceFromS3: NotRequired[bool],
```

## ApplyEnvironmentManagedActionRequestRequestTypeDef

```python
# ApplyEnvironmentManagedActionRequestRequestTypeDef definition

class ApplyEnvironmentManagedActionRequestRequestTypeDef(TypedDict):
    ActionId: str,
    EnvironmentName: NotRequired[str],
    EnvironmentId: NotRequired[str],
```

## AssociateEnvironmentOperationsRoleMessageRequestTypeDef

```python
# AssociateEnvironmentOperationsRoleMessageRequestTypeDef definition

class AssociateEnvironmentOperationsRoleMessageRequestTypeDef(TypedDict):
    EnvironmentName: str,
    OperationsRole: str,
```

## AutoScalingGroupTypeDef

```python
# AutoScalingGroupTypeDef definition

class AutoScalingGroupTypeDef(TypedDict):
    Name: NotRequired[str],
```

## BuildConfigurationTypeDef

```python
# BuildConfigurationTypeDef definition

class BuildConfigurationTypeDef(TypedDict):
    CodeBuildServiceRole: str,
    Image: str,
    ArtifactName: NotRequired[str],
    ComputeType: NotRequired[ComputeTypeType],  # (1)
    TimeoutInMinutes: NotRequired[int],
```

1. See [:material-code-brackets: ComputeTypeType](./literals.md#computetypetype) 
## BuilderTypeDef

```python
# BuilderTypeDef definition

class BuilderTypeDef(TypedDict):
    ARN: NotRequired[str],
```

## CPUUtilizationTypeDef

```python
# CPUUtilizationTypeDef definition

class CPUUtilizationTypeDef(TypedDict):
    User: NotRequired[float],
    Nice: NotRequired[float],
    System: NotRequired[float],
    Idle: NotRequired[float],
    IOWait: NotRequired[float],
    IRQ: NotRequired[float],
    SoftIRQ: NotRequired[float],
    Privileged: NotRequired[float],
```

## CheckDNSAvailabilityMessageRequestTypeDef

```python
# CheckDNSAvailabilityMessageRequestTypeDef definition

class CheckDNSAvailabilityMessageRequestTypeDef(TypedDict):
    CNAMEPrefix: str,
```

## ComposeEnvironmentsMessageRequestTypeDef

```python
# ComposeEnvironmentsMessageRequestTypeDef definition

class ComposeEnvironmentsMessageRequestTypeDef(TypedDict):
    ApplicationName: NotRequired[str],
    GroupName: NotRequired[str],
    VersionLabels: NotRequired[Sequence[str]],
```

## OptionRestrictionRegexTypeDef

```python
# OptionRestrictionRegexTypeDef definition

class OptionRestrictionRegexTypeDef(TypedDict):
    Pattern: NotRequired[str],
    Label: NotRequired[str],
```

## ConfigurationOptionSettingTypeDef

```python
# ConfigurationOptionSettingTypeDef definition

class ConfigurationOptionSettingTypeDef(TypedDict):
    ResourceName: NotRequired[str],
    Namespace: NotRequired[str],
    OptionName: NotRequired[str],
    Value: NotRequired[str],
```

## ValidationMessageTypeDef

```python
# ValidationMessageTypeDef definition

class ValidationMessageTypeDef(TypedDict):
    Message: NotRequired[str],
    Severity: NotRequired[ValidationSeverityType],  # (1)
    Namespace: NotRequired[str],
    OptionName: NotRequired[str],
```

1. See [:material-code-brackets: ValidationSeverityType](./literals.md#validationseveritytype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## SourceConfigurationTypeDef

```python
# SourceConfigurationTypeDef definition

class SourceConfigurationTypeDef(TypedDict):
    ApplicationName: NotRequired[str],
    TemplateName: NotRequired[str],
```

## EnvironmentTierTypeDef

```python
# EnvironmentTierTypeDef definition

class EnvironmentTierTypeDef(TypedDict):
    Name: NotRequired[str],
    Type: NotRequired[str],
    Version: NotRequired[str],
```

## OptionSpecificationTypeDef

```python
# OptionSpecificationTypeDef definition

class OptionSpecificationTypeDef(TypedDict):
    ResourceName: NotRequired[str],
    Namespace: NotRequired[str],
    OptionName: NotRequired[str],
```

## PlatformSummaryTypeDef

```python
# PlatformSummaryTypeDef definition

class PlatformSummaryTypeDef(TypedDict):
    PlatformArn: NotRequired[str],
    PlatformOwner: NotRequired[str],
    PlatformStatus: NotRequired[PlatformStatusType],  # (1)
    PlatformCategory: NotRequired[str],
    OperatingSystemName: NotRequired[str],
    OperatingSystemVersion: NotRequired[str],
    SupportedTierList: NotRequired[List[str]],
    SupportedAddonList: NotRequired[List[str]],
    PlatformLifecycleState: NotRequired[str],
    PlatformVersion: NotRequired[str],
    PlatformBranchName: NotRequired[str],
    PlatformBranchLifecycleState: NotRequired[str],
```

1. See [:material-code-brackets: PlatformStatusType](./literals.md#platformstatustype) 
## CustomAmiTypeDef

```python
# CustomAmiTypeDef definition

class CustomAmiTypeDef(TypedDict):
    VirtualizationType: NotRequired[str],
    ImageId: NotRequired[str],
```

## DeleteApplicationMessageRequestTypeDef

```python
# DeleteApplicationMessageRequestTypeDef definition

class DeleteApplicationMessageRequestTypeDef(TypedDict):
    ApplicationName: str,
    TerminateEnvByForce: NotRequired[bool],
```

## DeleteApplicationVersionMessageRequestTypeDef

```python
# DeleteApplicationVersionMessageRequestTypeDef definition

class DeleteApplicationVersionMessageRequestTypeDef(TypedDict):
    ApplicationName: str,
    VersionLabel: str,
    DeleteSourceBundle: NotRequired[bool],
```

## DeleteConfigurationTemplateMessageRequestTypeDef

```python
# DeleteConfigurationTemplateMessageRequestTypeDef definition

class DeleteConfigurationTemplateMessageRequestTypeDef(TypedDict):
    ApplicationName: str,
    TemplateName: str,
```

## DeleteEnvironmentConfigurationMessageRequestTypeDef

```python
# DeleteEnvironmentConfigurationMessageRequestTypeDef definition

class DeleteEnvironmentConfigurationMessageRequestTypeDef(TypedDict):
    ApplicationName: str,
    EnvironmentName: str,
```

## DeletePlatformVersionRequestRequestTypeDef

```python
# DeletePlatformVersionRequestRequestTypeDef definition

class DeletePlatformVersionRequestRequestTypeDef(TypedDict):
    PlatformArn: NotRequired[str],
```

## DeploymentTypeDef

```python
# DeploymentTypeDef definition

class DeploymentTypeDef(TypedDict):
    VersionLabel: NotRequired[str],
    DeploymentId: NotRequired[int],
    Status: NotRequired[str],
    DeploymentTime: NotRequired[datetime],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeApplicationVersionsMessageRequestTypeDef

```python
# DescribeApplicationVersionsMessageRequestTypeDef definition

class DescribeApplicationVersionsMessageRequestTypeDef(TypedDict):
    ApplicationName: NotRequired[str],
    VersionLabels: NotRequired[Sequence[str]],
    MaxRecords: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeApplicationsMessageRequestTypeDef

```python
# DescribeApplicationsMessageRequestTypeDef definition

class DescribeApplicationsMessageRequestTypeDef(TypedDict):
    ApplicationNames: NotRequired[Sequence[str]],
```

## DescribeConfigurationSettingsMessageRequestTypeDef

```python
# DescribeConfigurationSettingsMessageRequestTypeDef definition

class DescribeConfigurationSettingsMessageRequestTypeDef(TypedDict):
    ApplicationName: str,
    TemplateName: NotRequired[str],
    EnvironmentName: NotRequired[str],
```

## DescribeEnvironmentHealthRequestRequestTypeDef

```python
# DescribeEnvironmentHealthRequestRequestTypeDef definition

class DescribeEnvironmentHealthRequestRequestTypeDef(TypedDict):
    EnvironmentName: NotRequired[str],
    EnvironmentId: NotRequired[str],
    AttributeNames: NotRequired[Sequence[EnvironmentHealthAttributeType]],  # (1)
```

1. See [:material-code-brackets: EnvironmentHealthAttributeType](./literals.md#environmenthealthattributetype) 
## InstanceHealthSummaryTypeDef

```python
# InstanceHealthSummaryTypeDef definition

class InstanceHealthSummaryTypeDef(TypedDict):
    NoData: NotRequired[int],
    Unknown: NotRequired[int],
    Pending: NotRequired[int],
    Ok: NotRequired[int],
    Info: NotRequired[int],
    Warning: NotRequired[int],
    Degraded: NotRequired[int],
    Severe: NotRequired[int],
```

## DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef

```python
# DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef definition

class DescribeEnvironmentManagedActionHistoryRequestRequestTypeDef(TypedDict):
    EnvironmentId: NotRequired[str],
    EnvironmentName: NotRequired[str],
    NextToken: NotRequired[str],
    MaxItems: NotRequired[int],
```

## ManagedActionHistoryItemTypeDef

```python
# ManagedActionHistoryItemTypeDef definition

class ManagedActionHistoryItemTypeDef(TypedDict):
    ActionId: NotRequired[str],
    ActionType: NotRequired[ActionTypeType],  # (1)
    ActionDescription: NotRequired[str],
    FailureType: NotRequired[FailureTypeType],  # (2)
    Status: NotRequired[ActionHistoryStatusType],  # (3)
    FailureDescription: NotRequired[str],
    ExecutedTime: NotRequired[datetime],
    FinishedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ActionTypeType](./literals.md#actiontypetype) 
2. See [:material-code-brackets: FailureTypeType](./literals.md#failuretypetype) 
3. See [:material-code-brackets: ActionHistoryStatusType](./literals.md#actionhistorystatustype) 
## DescribeEnvironmentManagedActionsRequestRequestTypeDef

```python
# DescribeEnvironmentManagedActionsRequestRequestTypeDef definition

class DescribeEnvironmentManagedActionsRequestRequestTypeDef(TypedDict):
    EnvironmentName: NotRequired[str],
    EnvironmentId: NotRequired[str],
    Status: NotRequired[ActionStatusType],  # (1)
```

1. See [:material-code-brackets: ActionStatusType](./literals.md#actionstatustype) 
## ManagedActionTypeDef

```python
# ManagedActionTypeDef definition

class ManagedActionTypeDef(TypedDict):
    ActionId: NotRequired[str],
    ActionDescription: NotRequired[str],
    ActionType: NotRequired[ActionTypeType],  # (1)
    Status: NotRequired[ActionStatusType],  # (2)
    WindowStartTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ActionTypeType](./literals.md#actiontypetype) 
2. See [:material-code-brackets: ActionStatusType](./literals.md#actionstatustype) 
## DescribeEnvironmentResourcesMessageRequestTypeDef

```python
# DescribeEnvironmentResourcesMessageRequestTypeDef definition

class DescribeEnvironmentResourcesMessageRequestTypeDef(TypedDict):
    EnvironmentId: NotRequired[str],
    EnvironmentName: NotRequired[str],
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeInstancesHealthRequestRequestTypeDef

```python
# DescribeInstancesHealthRequestRequestTypeDef definition

class DescribeInstancesHealthRequestRequestTypeDef(TypedDict):
    EnvironmentName: NotRequired[str],
    EnvironmentId: NotRequired[str],
    AttributeNames: NotRequired[Sequence[InstancesHealthAttributeType]],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: InstancesHealthAttributeType](./literals.md#instanceshealthattributetype) 
## DescribePlatformVersionRequestRequestTypeDef

```python
# DescribePlatformVersionRequestRequestTypeDef definition

class DescribePlatformVersionRequestRequestTypeDef(TypedDict):
    PlatformArn: NotRequired[str],
```

## DisassociateEnvironmentOperationsRoleMessageRequestTypeDef

```python
# DisassociateEnvironmentOperationsRoleMessageRequestTypeDef definition

class DisassociateEnvironmentOperationsRoleMessageRequestTypeDef(TypedDict):
    EnvironmentName: str,
```

## EnvironmentLinkTypeDef

```python
# EnvironmentLinkTypeDef definition

class EnvironmentLinkTypeDef(TypedDict):
    LinkName: NotRequired[str],
    EnvironmentName: NotRequired[str],
```

## EnvironmentInfoDescriptionTypeDef

```python
# EnvironmentInfoDescriptionTypeDef definition

class EnvironmentInfoDescriptionTypeDef(TypedDict):
    InfoType: NotRequired[EnvironmentInfoTypeType],  # (1)
    Ec2InstanceId: NotRequired[str],
    SampleTimestamp: NotRequired[datetime],
    Message: NotRequired[str],
```

1. See [:material-code-brackets: EnvironmentInfoTypeType](./literals.md#environmentinfotypetype) 
## InstanceTypeDef

```python
# InstanceTypeDef definition

class InstanceTypeDef(TypedDict):
    Id: NotRequired[str],
```

## LaunchConfigurationTypeDef

```python
# LaunchConfigurationTypeDef definition

class LaunchConfigurationTypeDef(TypedDict):
    Name: NotRequired[str],
```

## LaunchTemplateTypeDef

```python
# LaunchTemplateTypeDef definition

class LaunchTemplateTypeDef(TypedDict):
    Id: NotRequired[str],
```

## LoadBalancerTypeDef

```python
# LoadBalancerTypeDef definition

class LoadBalancerTypeDef(TypedDict):
    Name: NotRequired[str],
```

## QueueTypeDef

```python
# QueueTypeDef definition

class QueueTypeDef(TypedDict):
    Name: NotRequired[str],
    URL: NotRequired[str],
```

## TriggerTypeDef

```python
# TriggerTypeDef definition

class TriggerTypeDef(TypedDict):
    Name: NotRequired[str],
```

## EventDescriptionTypeDef

```python
# EventDescriptionTypeDef definition

class EventDescriptionTypeDef(TypedDict):
    EventDate: NotRequired[datetime],
    Message: NotRequired[str],
    ApplicationName: NotRequired[str],
    VersionLabel: NotRequired[str],
    TemplateName: NotRequired[str],
    EnvironmentName: NotRequired[str],
    PlatformArn: NotRequired[str],
    RequestId: NotRequired[str],
    Severity: NotRequired[EventSeverityType],  # (1)
```

1. See [:material-code-brackets: EventSeverityType](./literals.md#eventseveritytype) 
## SolutionStackDescriptionTypeDef

```python
# SolutionStackDescriptionTypeDef definition

class SolutionStackDescriptionTypeDef(TypedDict):
    SolutionStackName: NotRequired[str],
    PermittedFileTypes: NotRequired[List[str]],
```

## SearchFilterTypeDef

```python
# SearchFilterTypeDef definition

class SearchFilterTypeDef(TypedDict):
    Attribute: NotRequired[str],
    Operator: NotRequired[str],
    Values: NotRequired[Sequence[str]],
```

## PlatformBranchSummaryTypeDef

```python
# PlatformBranchSummaryTypeDef definition

class PlatformBranchSummaryTypeDef(TypedDict):
    PlatformName: NotRequired[str],
    BranchName: NotRequired[str],
    LifecycleState: NotRequired[str],
    BranchOrder: NotRequired[int],
    SupportedTierList: NotRequired[List[str]],
```

## PlatformFilterTypeDef

```python
# PlatformFilterTypeDef definition

class PlatformFilterTypeDef(TypedDict):
    Type: NotRequired[str],
    Operator: NotRequired[str],
    Values: NotRequired[Sequence[str]],
```

## ListTagsForResourceMessageRequestTypeDef

```python
# ListTagsForResourceMessageRequestTypeDef definition

class ListTagsForResourceMessageRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ListenerTypeDef

```python
# ListenerTypeDef definition

class ListenerTypeDef(TypedDict):
    Protocol: NotRequired[str],
    Port: NotRequired[int],
```

## PlatformFrameworkTypeDef

```python
# PlatformFrameworkTypeDef definition

class PlatformFrameworkTypeDef(TypedDict):
    Name: NotRequired[str],
    Version: NotRequired[str],
```

## PlatformProgrammingLanguageTypeDef

```python
# PlatformProgrammingLanguageTypeDef definition

class PlatformProgrammingLanguageTypeDef(TypedDict):
    Name: NotRequired[str],
    Version: NotRequired[str],
```

## RebuildEnvironmentMessageRequestTypeDef

```python
# RebuildEnvironmentMessageRequestTypeDef definition

class RebuildEnvironmentMessageRequestTypeDef(TypedDict):
    EnvironmentId: NotRequired[str],
    EnvironmentName: NotRequired[str],
```

## RequestEnvironmentInfoMessageRequestTypeDef

```python
# RequestEnvironmentInfoMessageRequestTypeDef definition

class RequestEnvironmentInfoMessageRequestTypeDef(TypedDict):
    InfoType: EnvironmentInfoTypeType,  # (1)
    EnvironmentId: NotRequired[str],
    EnvironmentName: NotRequired[str],
```

1. See [:material-code-brackets: EnvironmentInfoTypeType](./literals.md#environmentinfotypetype) 
## ResourceQuotaTypeDef

```python
# ResourceQuotaTypeDef definition

class ResourceQuotaTypeDef(TypedDict):
    Maximum: NotRequired[int],
```

## RestartAppServerMessageRequestTypeDef

```python
# RestartAppServerMessageRequestTypeDef definition

class RestartAppServerMessageRequestTypeDef(TypedDict):
    EnvironmentId: NotRequired[str],
    EnvironmentName: NotRequired[str],
```

## RetrieveEnvironmentInfoMessageRequestTypeDef

```python
# RetrieveEnvironmentInfoMessageRequestTypeDef definition

class RetrieveEnvironmentInfoMessageRequestTypeDef(TypedDict):
    InfoType: EnvironmentInfoTypeType,  # (1)
    EnvironmentId: NotRequired[str],
    EnvironmentName: NotRequired[str],
```

1. See [:material-code-brackets: EnvironmentInfoTypeType](./literals.md#environmentinfotypetype) 
## SwapEnvironmentCNAMEsMessageRequestTypeDef

```python
# SwapEnvironmentCNAMEsMessageRequestTypeDef definition

class SwapEnvironmentCNAMEsMessageRequestTypeDef(TypedDict):
    SourceEnvironmentId: NotRequired[str],
    SourceEnvironmentName: NotRequired[str],
    DestinationEnvironmentId: NotRequired[str],
    DestinationEnvironmentName: NotRequired[str],
```

## TerminateEnvironmentMessageRequestTypeDef

```python
# TerminateEnvironmentMessageRequestTypeDef definition

class TerminateEnvironmentMessageRequestTypeDef(TypedDict):
    EnvironmentId: NotRequired[str],
    EnvironmentName: NotRequired[str],
    TerminateResources: NotRequired[bool],
    ForceTerminate: NotRequired[bool],
```

## UpdateApplicationMessageRequestTypeDef

```python
# UpdateApplicationMessageRequestTypeDef definition

class UpdateApplicationMessageRequestTypeDef(TypedDict):
    ApplicationName: str,
    Description: NotRequired[str],
```

## UpdateApplicationVersionMessageRequestTypeDef

```python
# UpdateApplicationVersionMessageRequestTypeDef definition

class UpdateApplicationVersionMessageRequestTypeDef(TypedDict):
    ApplicationName: str,
    VersionLabel: str,
    Description: NotRequired[str],
```

## ApplyEnvironmentManagedActionResultTypeDef

```python
# ApplyEnvironmentManagedActionResultTypeDef definition

class ApplyEnvironmentManagedActionResultTypeDef(TypedDict):
    ActionId: str,
    ActionDescription: str,
    ActionType: ActionTypeType,  # (1)
    Status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ActionTypeType](./literals.md#actiontypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CheckDNSAvailabilityResultMessageTypeDef

```python
# CheckDNSAvailabilityResultMessageTypeDef definition

class CheckDNSAvailabilityResultMessageTypeDef(TypedDict):
    Available: bool,
    FullyQualifiedCNAME: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStorageLocationResultMessageTypeDef

```python
# CreateStorageLocationResultMessageTypeDef definition

class CreateStorageLocationResultMessageTypeDef(TypedDict):
    S3Bucket: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ApplicationMetricsTypeDef

```python
# ApplicationMetricsTypeDef definition

class ApplicationMetricsTypeDef(TypedDict):
    Duration: NotRequired[int],
    RequestCount: NotRequired[int],
    StatusCodes: NotRequired[StatusCodesTypeDef],  # (1)
    Latency: NotRequired[LatencyTypeDef],  # (2)
```

1. See [:material-code-braces: StatusCodesTypeDef](./type_defs.md#statuscodestypedef) 
2. See [:material-code-braces: LatencyTypeDef](./type_defs.md#latencytypedef) 
## ApplicationVersionDescriptionTypeDef

```python
# ApplicationVersionDescriptionTypeDef definition

class ApplicationVersionDescriptionTypeDef(TypedDict):
    ApplicationVersionArn: NotRequired[str],
    ApplicationName: NotRequired[str],
    Description: NotRequired[str],
    VersionLabel: NotRequired[str],
    SourceBuildInformation: NotRequired[SourceBuildInformationTypeDef],  # (1)
    BuildArn: NotRequired[str],
    SourceBundle: NotRequired[S3LocationTypeDef],  # (2)
    DateCreated: NotRequired[datetime],
    DateUpdated: NotRequired[datetime],
    Status: NotRequired[ApplicationVersionStatusType],  # (3)
```

1. See [:material-code-braces: SourceBuildInformationTypeDef](./type_defs.md#sourcebuildinformationtypedef) 
2. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
3. See [:material-code-brackets: ApplicationVersionStatusType](./literals.md#applicationversionstatustype) 
## ApplicationVersionLifecycleConfigTypeDef

```python
# ApplicationVersionLifecycleConfigTypeDef definition

class ApplicationVersionLifecycleConfigTypeDef(TypedDict):
    MaxCountRule: NotRequired[MaxCountRuleTypeDef],  # (1)
    MaxAgeRule: NotRequired[MaxAgeRuleTypeDef],  # (2)
```

1. See [:material-code-braces: MaxCountRuleTypeDef](./type_defs.md#maxcountruletypedef) 
2. See [:material-code-braces: MaxAgeRuleTypeDef](./type_defs.md#maxageruletypedef) 
## SystemStatusTypeDef

```python
# SystemStatusTypeDef definition

class SystemStatusTypeDef(TypedDict):
    CPUUtilization: NotRequired[CPUUtilizationTypeDef],  # (1)
    LoadAverage: NotRequired[List[float]],
```

1. See [:material-code-braces: CPUUtilizationTypeDef](./type_defs.md#cpuutilizationtypedef) 
## ConfigurationOptionDescriptionTypeDef

```python
# ConfigurationOptionDescriptionTypeDef definition

class ConfigurationOptionDescriptionTypeDef(TypedDict):
    Namespace: NotRequired[str],
    Name: NotRequired[str],
    DefaultValue: NotRequired[str],
    ChangeSeverity: NotRequired[str],
    UserDefined: NotRequired[bool],
    ValueType: NotRequired[ConfigurationOptionValueTypeType],  # (1)
    ValueOptions: NotRequired[List[str]],
    MinValue: NotRequired[int],
    MaxValue: NotRequired[int],
    MaxLength: NotRequired[int],
    Regex: NotRequired[OptionRestrictionRegexTypeDef],  # (2)
```

1. See [:material-code-brackets: ConfigurationOptionValueTypeType](./literals.md#configurationoptionvaluetypetype) 
2. See [:material-code-braces: OptionRestrictionRegexTypeDef](./type_defs.md#optionrestrictionregextypedef) 
## ConfigurationSettingsDescriptionResponseTypeDef

```python
# ConfigurationSettingsDescriptionResponseTypeDef definition

class ConfigurationSettingsDescriptionResponseTypeDef(TypedDict):
    SolutionStackName: str,
    PlatformArn: str,
    ApplicationName: str,
    TemplateName: str,
    Description: str,
    EnvironmentName: str,
    DeploymentStatus: ConfigurationDeploymentStatusType,  # (1)
    DateCreated: datetime,
    DateUpdated: datetime,
    OptionSettings: List[ConfigurationOptionSettingTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ConfigurationDeploymentStatusType](./literals.md#configurationdeploymentstatustype) 
2. See [:material-code-braces: ConfigurationOptionSettingTypeDef](./type_defs.md#configurationoptionsettingtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConfigurationSettingsDescriptionTypeDef

```python
# ConfigurationSettingsDescriptionTypeDef definition

class ConfigurationSettingsDescriptionTypeDef(TypedDict):
    SolutionStackName: NotRequired[str],
    PlatformArn: NotRequired[str],
    ApplicationName: NotRequired[str],
    TemplateName: NotRequired[str],
    Description: NotRequired[str],
    EnvironmentName: NotRequired[str],
    DeploymentStatus: NotRequired[ConfigurationDeploymentStatusType],  # (1)
    DateCreated: NotRequired[datetime],
    DateUpdated: NotRequired[datetime],
    OptionSettings: NotRequired[List[ConfigurationOptionSettingTypeDef]],  # (2)
```

1. See [:material-code-brackets: ConfigurationDeploymentStatusType](./literals.md#configurationdeploymentstatustype) 
2. See [:material-code-braces: ConfigurationOptionSettingTypeDef](./type_defs.md#configurationoptionsettingtypedef) 
## ValidateConfigurationSettingsMessageRequestTypeDef

```python
# ValidateConfigurationSettingsMessageRequestTypeDef definition

class ValidateConfigurationSettingsMessageRequestTypeDef(TypedDict):
    ApplicationName: str,
    OptionSettings: Sequence[ConfigurationOptionSettingTypeDef],  # (1)
    TemplateName: NotRequired[str],
    EnvironmentName: NotRequired[str],
```

1. See [:material-code-braces: ConfigurationOptionSettingTypeDef](./type_defs.md#configurationoptionsettingtypedef) 
## ConfigurationSettingsValidationMessagesTypeDef

```python
# ConfigurationSettingsValidationMessagesTypeDef definition

class ConfigurationSettingsValidationMessagesTypeDef(TypedDict):
    Messages: List[ValidationMessageTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ValidationMessageTypeDef](./type_defs.md#validationmessagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateApplicationVersionMessageRequestTypeDef

```python
# CreateApplicationVersionMessageRequestTypeDef definition

class CreateApplicationVersionMessageRequestTypeDef(TypedDict):
    ApplicationName: str,
    VersionLabel: str,
    Description: NotRequired[str],
    SourceBuildInformation: NotRequired[SourceBuildInformationTypeDef],  # (1)
    SourceBundle: NotRequired[S3LocationTypeDef],  # (2)
    BuildConfiguration: NotRequired[BuildConfigurationTypeDef],  # (3)
    AutoCreateApplication: NotRequired[bool],
    Process: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
```

1. See [:material-code-braces: SourceBuildInformationTypeDef](./type_defs.md#sourcebuildinformationtypedef) 
2. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
3. See [:material-code-braces: BuildConfigurationTypeDef](./type_defs.md#buildconfigurationtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreatePlatformVersionRequestRequestTypeDef

```python
# CreatePlatformVersionRequestRequestTypeDef definition

class CreatePlatformVersionRequestRequestTypeDef(TypedDict):
    PlatformName: str,
    PlatformVersion: str,
    PlatformDefinitionBundle: S3LocationTypeDef,  # (1)
    EnvironmentName: NotRequired[str],
    OptionSettings: NotRequired[Sequence[ConfigurationOptionSettingTypeDef]],  # (2)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
2. See [:material-code-braces: ConfigurationOptionSettingTypeDef](./type_defs.md#configurationoptionsettingtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ResourceTagsDescriptionMessageTypeDef

```python
# ResourceTagsDescriptionMessageTypeDef definition

class ResourceTagsDescriptionMessageTypeDef(TypedDict):
    ResourceArn: str,
    ResourceTags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTagsForResourceMessageRequestTypeDef

```python
# UpdateTagsForResourceMessageRequestTypeDef definition

class UpdateTagsForResourceMessageRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagsToAdd: NotRequired[Sequence[TagTypeDef]],  # (1)
    TagsToRemove: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateConfigurationTemplateMessageRequestTypeDef

```python
# CreateConfigurationTemplateMessageRequestTypeDef definition

class CreateConfigurationTemplateMessageRequestTypeDef(TypedDict):
    ApplicationName: str,
    TemplateName: str,
    SolutionStackName: NotRequired[str],
    PlatformArn: NotRequired[str],
    SourceConfiguration: NotRequired[SourceConfigurationTypeDef],  # (1)
    EnvironmentId: NotRequired[str],
    Description: NotRequired[str],
    OptionSettings: NotRequired[Sequence[ConfigurationOptionSettingTypeDef]],  # (2)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: SourceConfigurationTypeDef](./type_defs.md#sourceconfigurationtypedef) 
2. See [:material-code-braces: ConfigurationOptionSettingTypeDef](./type_defs.md#configurationoptionsettingtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateEnvironmentMessageRequestTypeDef

```python
# CreateEnvironmentMessageRequestTypeDef definition

class CreateEnvironmentMessageRequestTypeDef(TypedDict):
    ApplicationName: str,
    EnvironmentName: NotRequired[str],
    GroupName: NotRequired[str],
    Description: NotRequired[str],
    CNAMEPrefix: NotRequired[str],
    Tier: NotRequired[EnvironmentTierTypeDef],  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    VersionLabel: NotRequired[str],
    TemplateName: NotRequired[str],
    SolutionStackName: NotRequired[str],
    PlatformArn: NotRequired[str],
    OptionSettings: NotRequired[Sequence[ConfigurationOptionSettingTypeDef]],  # (3)
    OptionsToRemove: NotRequired[Sequence[OptionSpecificationTypeDef]],  # (4)
    OperationsRole: NotRequired[str],
```

1. See [:material-code-braces: EnvironmentTierTypeDef](./type_defs.md#environmenttiertypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ConfigurationOptionSettingTypeDef](./type_defs.md#configurationoptionsettingtypedef) 
4. See [:material-code-braces: OptionSpecificationTypeDef](./type_defs.md#optionspecificationtypedef) 
## DescribeConfigurationOptionsMessageRequestTypeDef

```python
# DescribeConfigurationOptionsMessageRequestTypeDef definition

class DescribeConfigurationOptionsMessageRequestTypeDef(TypedDict):
    ApplicationName: NotRequired[str],
    TemplateName: NotRequired[str],
    EnvironmentName: NotRequired[str],
    SolutionStackName: NotRequired[str],
    PlatformArn: NotRequired[str],
    Options: NotRequired[Sequence[OptionSpecificationTypeDef]],  # (1)
```

1. See [:material-code-braces: OptionSpecificationTypeDef](./type_defs.md#optionspecificationtypedef) 
## UpdateConfigurationTemplateMessageRequestTypeDef

```python
# UpdateConfigurationTemplateMessageRequestTypeDef definition

class UpdateConfigurationTemplateMessageRequestTypeDef(TypedDict):
    ApplicationName: str,
    TemplateName: str,
    Description: NotRequired[str],
    OptionSettings: NotRequired[Sequence[ConfigurationOptionSettingTypeDef]],  # (1)
    OptionsToRemove: NotRequired[Sequence[OptionSpecificationTypeDef]],  # (2)
```

1. See [:material-code-braces: ConfigurationOptionSettingTypeDef](./type_defs.md#configurationoptionsettingtypedef) 
2. See [:material-code-braces: OptionSpecificationTypeDef](./type_defs.md#optionspecificationtypedef) 
## UpdateEnvironmentMessageRequestTypeDef

```python
# UpdateEnvironmentMessageRequestTypeDef definition

class UpdateEnvironmentMessageRequestTypeDef(TypedDict):
    ApplicationName: NotRequired[str],
    EnvironmentId: NotRequired[str],
    EnvironmentName: NotRequired[str],
    GroupName: NotRequired[str],
    Description: NotRequired[str],
    Tier: NotRequired[EnvironmentTierTypeDef],  # (1)
    VersionLabel: NotRequired[str],
    TemplateName: NotRequired[str],
    SolutionStackName: NotRequired[str],
    PlatformArn: NotRequired[str],
    OptionSettings: NotRequired[Sequence[ConfigurationOptionSettingTypeDef]],  # (2)
    OptionsToRemove: NotRequired[Sequence[OptionSpecificationTypeDef]],  # (3)
```

1. See [:material-code-braces: EnvironmentTierTypeDef](./type_defs.md#environmenttiertypedef) 
2. See [:material-code-braces: ConfigurationOptionSettingTypeDef](./type_defs.md#configurationoptionsettingtypedef) 
3. See [:material-code-braces: OptionSpecificationTypeDef](./type_defs.md#optionspecificationtypedef) 
## CreatePlatformVersionResultTypeDef

```python
# CreatePlatformVersionResultTypeDef definition

class CreatePlatformVersionResultTypeDef(TypedDict):
    PlatformSummary: PlatformSummaryTypeDef,  # (1)
    Builder: BuilderTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: PlatformSummaryTypeDef](./type_defs.md#platformsummarytypedef) 
2. See [:material-code-braces: BuilderTypeDef](./type_defs.md#buildertypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeletePlatformVersionResultTypeDef

```python
# DeletePlatformVersionResultTypeDef definition

class DeletePlatformVersionResultTypeDef(TypedDict):
    PlatformSummary: PlatformSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PlatformSummaryTypeDef](./type_defs.md#platformsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPlatformVersionsResultTypeDef

```python
# ListPlatformVersionsResultTypeDef definition

class ListPlatformVersionsResultTypeDef(TypedDict):
    PlatformSummaryList: List[PlatformSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PlatformSummaryTypeDef](./type_defs.md#platformsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef

```python
# DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef definition

class DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef(TypedDict):
    ApplicationName: NotRequired[str],
    VersionLabels: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef

```python
# DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef definition

class DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef(TypedDict):
    EnvironmentId: NotRequired[str],
    EnvironmentName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEnvironmentManagedActionHistoryResultTypeDef

```python
# DescribeEnvironmentManagedActionHistoryResultTypeDef definition

class DescribeEnvironmentManagedActionHistoryResultTypeDef(TypedDict):
    ManagedActionHistoryItems: List[ManagedActionHistoryItemTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ManagedActionHistoryItemTypeDef](./type_defs.md#managedactionhistoryitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEnvironmentManagedActionsResultTypeDef

```python
# DescribeEnvironmentManagedActionsResultTypeDef definition

class DescribeEnvironmentManagedActionsResultTypeDef(TypedDict):
    ManagedActions: List[ManagedActionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ManagedActionTypeDef](./type_defs.md#managedactiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef

```python
# DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef definition

class DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef(TypedDict):
    ApplicationName: NotRequired[str],
    VersionLabel: NotRequired[str],
    EnvironmentIds: NotRequired[Sequence[str]],
    EnvironmentNames: NotRequired[Sequence[str]],
    IncludeDeleted: NotRequired[bool],
    IncludedDeletedBackTo: NotRequired[Union[datetime, str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEnvironmentsMessageRequestTypeDef

```python
# DescribeEnvironmentsMessageRequestTypeDef definition

class DescribeEnvironmentsMessageRequestTypeDef(TypedDict):
    ApplicationName: NotRequired[str],
    VersionLabel: NotRequired[str],
    EnvironmentIds: NotRequired[Sequence[str]],
    EnvironmentNames: NotRequired[Sequence[str]],
    IncludeDeleted: NotRequired[bool],
    IncludedDeletedBackTo: NotRequired[Union[datetime, str]],
    MaxRecords: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeEventsMessageDescribeEventsPaginateTypeDef

```python
# DescribeEventsMessageDescribeEventsPaginateTypeDef definition

class DescribeEventsMessageDescribeEventsPaginateTypeDef(TypedDict):
    ApplicationName: NotRequired[str],
    VersionLabel: NotRequired[str],
    TemplateName: NotRequired[str],
    EnvironmentId: NotRequired[str],
    EnvironmentName: NotRequired[str],
    PlatformArn: NotRequired[str],
    RequestId: NotRequired[str],
    Severity: NotRequired[EventSeverityType],  # (1)
    StartTime: NotRequired[Union[datetime, str]],
    EndTime: NotRequired[Union[datetime, str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: EventSeverityType](./literals.md#eventseveritytype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEventsMessageRequestTypeDef

```python
# DescribeEventsMessageRequestTypeDef definition

class DescribeEventsMessageRequestTypeDef(TypedDict):
    ApplicationName: NotRequired[str],
    VersionLabel: NotRequired[str],
    TemplateName: NotRequired[str],
    EnvironmentId: NotRequired[str],
    EnvironmentName: NotRequired[str],
    PlatformArn: NotRequired[str],
    RequestId: NotRequired[str],
    Severity: NotRequired[EventSeverityType],  # (1)
    StartTime: NotRequired[Union[datetime, str]],
    EndTime: NotRequired[Union[datetime, str]],
    MaxRecords: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: EventSeverityType](./literals.md#eventseveritytype) 
## DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef

```python
# DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef definition

class DescribeEnvironmentsMessageEnvironmentExistsWaitTypeDef(TypedDict):
    ApplicationName: NotRequired[str],
    VersionLabel: NotRequired[str],
    EnvironmentIds: NotRequired[Sequence[str]],
    EnvironmentNames: NotRequired[Sequence[str]],
    IncludeDeleted: NotRequired[bool],
    IncludedDeletedBackTo: NotRequired[Union[datetime, str]],
    MaxRecords: NotRequired[int],
    NextToken: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeEnvironmentsMessageEnvironmentTerminatedWaitTypeDef

```python
# DescribeEnvironmentsMessageEnvironmentTerminatedWaitTypeDef definition

class DescribeEnvironmentsMessageEnvironmentTerminatedWaitTypeDef(TypedDict):
    ApplicationName: NotRequired[str],
    VersionLabel: NotRequired[str],
    EnvironmentIds: NotRequired[Sequence[str]],
    EnvironmentNames: NotRequired[Sequence[str]],
    IncludeDeleted: NotRequired[bool],
    IncludedDeletedBackTo: NotRequired[Union[datetime, str]],
    MaxRecords: NotRequired[int],
    NextToken: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeEnvironmentsMessageEnvironmentUpdatedWaitTypeDef

```python
# DescribeEnvironmentsMessageEnvironmentUpdatedWaitTypeDef definition

class DescribeEnvironmentsMessageEnvironmentUpdatedWaitTypeDef(TypedDict):
    ApplicationName: NotRequired[str],
    VersionLabel: NotRequired[str],
    EnvironmentIds: NotRequired[Sequence[str]],
    EnvironmentNames: NotRequired[Sequence[str]],
    IncludeDeleted: NotRequired[bool],
    IncludedDeletedBackTo: NotRequired[Union[datetime, str]],
    MaxRecords: NotRequired[int],
    NextToken: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## RetrieveEnvironmentInfoResultMessageTypeDef

```python
# RetrieveEnvironmentInfoResultMessageTypeDef definition

class RetrieveEnvironmentInfoResultMessageTypeDef(TypedDict):
    EnvironmentInfo: List[EnvironmentInfoDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentInfoDescriptionTypeDef](./type_defs.md#environmentinfodescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnvironmentResourceDescriptionTypeDef

```python
# EnvironmentResourceDescriptionTypeDef definition

class EnvironmentResourceDescriptionTypeDef(TypedDict):
    EnvironmentName: NotRequired[str],
    AutoScalingGroups: NotRequired[List[AutoScalingGroupTypeDef]],  # (1)
    Instances: NotRequired[List[InstanceTypeDef]],  # (2)
    LaunchConfigurations: NotRequired[List[LaunchConfigurationTypeDef]],  # (3)
    LaunchTemplates: NotRequired[List[LaunchTemplateTypeDef]],  # (4)
    LoadBalancers: NotRequired[List[LoadBalancerTypeDef]],  # (5)
    Triggers: NotRequired[List[TriggerTypeDef]],  # (6)
    Queues: NotRequired[List[QueueTypeDef]],  # (7)
```

1. See [:material-code-braces: AutoScalingGroupTypeDef](./type_defs.md#autoscalinggrouptypedef) 
2. See [:material-code-braces: InstanceTypeDef](./type_defs.md#instancetypedef) 
3. See [:material-code-braces: LaunchConfigurationTypeDef](./type_defs.md#launchconfigurationtypedef) 
4. See [:material-code-braces: LaunchTemplateTypeDef](./type_defs.md#launchtemplatetypedef) 
5. See [:material-code-braces: LoadBalancerTypeDef](./type_defs.md#loadbalancertypedef) 
6. See [:material-code-braces: TriggerTypeDef](./type_defs.md#triggertypedef) 
7. See [:material-code-braces: QueueTypeDef](./type_defs.md#queuetypedef) 
## EventDescriptionsMessageTypeDef

```python
# EventDescriptionsMessageTypeDef definition

class EventDescriptionsMessageTypeDef(TypedDict):
    Events: List[EventDescriptionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventDescriptionTypeDef](./type_defs.md#eventdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAvailableSolutionStacksResultMessageTypeDef

```python
# ListAvailableSolutionStacksResultMessageTypeDef definition

class ListAvailableSolutionStacksResultMessageTypeDef(TypedDict):
    SolutionStacks: List[str],
    SolutionStackDetails: List[SolutionStackDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SolutionStackDescriptionTypeDef](./type_defs.md#solutionstackdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPlatformBranchesRequestRequestTypeDef

```python
# ListPlatformBranchesRequestRequestTypeDef definition

class ListPlatformBranchesRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[SearchFilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SearchFilterTypeDef](./type_defs.md#searchfiltertypedef) 
## ListPlatformBranchesResultTypeDef

```python
# ListPlatformBranchesResultTypeDef definition

class ListPlatformBranchesResultTypeDef(TypedDict):
    PlatformBranchSummaryList: List[PlatformBranchSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PlatformBranchSummaryTypeDef](./type_defs.md#platformbranchsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPlatformVersionsRequestListPlatformVersionsPaginateTypeDef

```python
# ListPlatformVersionsRequestListPlatformVersionsPaginateTypeDef definition

class ListPlatformVersionsRequestListPlatformVersionsPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[PlatformFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: PlatformFilterTypeDef](./type_defs.md#platformfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPlatformVersionsRequestRequestTypeDef

```python
# ListPlatformVersionsRequestRequestTypeDef definition

class ListPlatformVersionsRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[PlatformFilterTypeDef]],  # (1)
    MaxRecords: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PlatformFilterTypeDef](./type_defs.md#platformfiltertypedef) 
## LoadBalancerDescriptionTypeDef

```python
# LoadBalancerDescriptionTypeDef definition

class LoadBalancerDescriptionTypeDef(TypedDict):
    LoadBalancerName: NotRequired[str],
    Domain: NotRequired[str],
    Listeners: NotRequired[List[ListenerTypeDef]],  # (1)
```

1. See [:material-code-braces: ListenerTypeDef](./type_defs.md#listenertypedef) 
## PlatformDescriptionTypeDef

```python
# PlatformDescriptionTypeDef definition

class PlatformDescriptionTypeDef(TypedDict):
    PlatformArn: NotRequired[str],
    PlatformOwner: NotRequired[str],
    PlatformName: NotRequired[str],
    PlatformVersion: NotRequired[str],
    SolutionStackName: NotRequired[str],
    PlatformStatus: NotRequired[PlatformStatusType],  # (1)
    DateCreated: NotRequired[datetime],
    DateUpdated: NotRequired[datetime],
    PlatformCategory: NotRequired[str],
    Description: NotRequired[str],
    Maintainer: NotRequired[str],
    OperatingSystemName: NotRequired[str],
    OperatingSystemVersion: NotRequired[str],
    ProgrammingLanguages: NotRequired[List[PlatformProgrammingLanguageTypeDef]],  # (2)
    Frameworks: NotRequired[List[PlatformFrameworkTypeDef]],  # (3)
    CustomAmiList: NotRequired[List[CustomAmiTypeDef]],  # (4)
    SupportedTierList: NotRequired[List[str]],
    SupportedAddonList: NotRequired[List[str]],
    PlatformLifecycleState: NotRequired[str],
    PlatformBranchName: NotRequired[str],
    PlatformBranchLifecycleState: NotRequired[str],
```

1. See [:material-code-brackets: PlatformStatusType](./literals.md#platformstatustype) 
2. See [:material-code-braces: PlatformProgrammingLanguageTypeDef](./type_defs.md#platformprogramminglanguagetypedef) 
3. See [:material-code-braces: PlatformFrameworkTypeDef](./type_defs.md#platformframeworktypedef) 
4. See [:material-code-braces: CustomAmiTypeDef](./type_defs.md#customamitypedef) 
## ResourceQuotasTypeDef

```python
# ResourceQuotasTypeDef definition

class ResourceQuotasTypeDef(TypedDict):
    ApplicationQuota: NotRequired[ResourceQuotaTypeDef],  # (1)
    ApplicationVersionQuota: NotRequired[ResourceQuotaTypeDef],  # (1)
    EnvironmentQuota: NotRequired[ResourceQuotaTypeDef],  # (1)
    ConfigurationTemplateQuota: NotRequired[ResourceQuotaTypeDef],  # (1)
    CustomPlatformQuota: NotRequired[ResourceQuotaTypeDef],  # (1)
```

1. See [:material-code-braces: ResourceQuotaTypeDef](./type_defs.md#resourcequotatypedef) 
2. See [:material-code-braces: ResourceQuotaTypeDef](./type_defs.md#resourcequotatypedef) 
3. See [:material-code-braces: ResourceQuotaTypeDef](./type_defs.md#resourcequotatypedef) 
4. See [:material-code-braces: ResourceQuotaTypeDef](./type_defs.md#resourcequotatypedef) 
5. See [:material-code-braces: ResourceQuotaTypeDef](./type_defs.md#resourcequotatypedef) 
## DescribeEnvironmentHealthResultTypeDef

```python
# DescribeEnvironmentHealthResultTypeDef definition

class DescribeEnvironmentHealthResultTypeDef(TypedDict):
    EnvironmentName: str,
    HealthStatus: str,
    Status: EnvironmentHealthType,  # (1)
    Color: str,
    Causes: List[str],
    ApplicationMetrics: ApplicationMetricsTypeDef,  # (2)
    InstancesHealth: InstanceHealthSummaryTypeDef,  # (3)
    RefreshedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: EnvironmentHealthType](./literals.md#environmenthealthtype) 
2. See [:material-code-braces: ApplicationMetricsTypeDef](./type_defs.md#applicationmetricstypedef) 
3. See [:material-code-braces: InstanceHealthSummaryTypeDef](./type_defs.md#instancehealthsummarytypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ApplicationVersionDescriptionMessageTypeDef

```python
# ApplicationVersionDescriptionMessageTypeDef definition

class ApplicationVersionDescriptionMessageTypeDef(TypedDict):
    ApplicationVersion: ApplicationVersionDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationVersionDescriptionTypeDef](./type_defs.md#applicationversiondescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ApplicationVersionDescriptionsMessageTypeDef

```python
# ApplicationVersionDescriptionsMessageTypeDef definition

class ApplicationVersionDescriptionsMessageTypeDef(TypedDict):
    ApplicationVersions: List[ApplicationVersionDescriptionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationVersionDescriptionTypeDef](./type_defs.md#applicationversiondescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ApplicationResourceLifecycleConfigTypeDef

```python
# ApplicationResourceLifecycleConfigTypeDef definition

class ApplicationResourceLifecycleConfigTypeDef(TypedDict):
    ServiceRole: NotRequired[str],
    VersionLifecycleConfig: NotRequired[ApplicationVersionLifecycleConfigTypeDef],  # (1)
```

1. See [:material-code-braces: ApplicationVersionLifecycleConfigTypeDef](./type_defs.md#applicationversionlifecycleconfigtypedef) 
## SingleInstanceHealthTypeDef

```python
# SingleInstanceHealthTypeDef definition

class SingleInstanceHealthTypeDef(TypedDict):
    InstanceId: NotRequired[str],
    HealthStatus: NotRequired[str],
    Color: NotRequired[str],
    Causes: NotRequired[List[str]],
    LaunchedAt: NotRequired[datetime],
    ApplicationMetrics: NotRequired[ApplicationMetricsTypeDef],  # (1)
    System: NotRequired[SystemStatusTypeDef],  # (2)
    Deployment: NotRequired[DeploymentTypeDef],  # (3)
    AvailabilityZone: NotRequired[str],
    InstanceType: NotRequired[str],
```

1. See [:material-code-braces: ApplicationMetricsTypeDef](./type_defs.md#applicationmetricstypedef) 
2. See [:material-code-braces: SystemStatusTypeDef](./type_defs.md#systemstatustypedef) 
3. See [:material-code-braces: DeploymentTypeDef](./type_defs.md#deploymenttypedef) 
## ConfigurationOptionsDescriptionTypeDef

```python
# ConfigurationOptionsDescriptionTypeDef definition

class ConfigurationOptionsDescriptionTypeDef(TypedDict):
    SolutionStackName: str,
    PlatformArn: str,
    Options: List[ConfigurationOptionDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfigurationOptionDescriptionTypeDef](./type_defs.md#configurationoptiondescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConfigurationSettingsDescriptionsTypeDef

```python
# ConfigurationSettingsDescriptionsTypeDef definition

class ConfigurationSettingsDescriptionsTypeDef(TypedDict):
    ConfigurationSettings: List[ConfigurationSettingsDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfigurationSettingsDescriptionTypeDef](./type_defs.md#configurationsettingsdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnvironmentResourceDescriptionsMessageTypeDef

```python
# EnvironmentResourceDescriptionsMessageTypeDef definition

class EnvironmentResourceDescriptionsMessageTypeDef(TypedDict):
    EnvironmentResources: EnvironmentResourceDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentResourceDescriptionTypeDef](./type_defs.md#environmentresourcedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnvironmentResourcesDescriptionTypeDef

```python
# EnvironmentResourcesDescriptionTypeDef definition

class EnvironmentResourcesDescriptionTypeDef(TypedDict):
    LoadBalancer: NotRequired[LoadBalancerDescriptionTypeDef],  # (1)
```

1. See [:material-code-braces: LoadBalancerDescriptionTypeDef](./type_defs.md#loadbalancerdescriptiontypedef) 
## DescribePlatformVersionResultTypeDef

```python
# DescribePlatformVersionResultTypeDef definition

class DescribePlatformVersionResultTypeDef(TypedDict):
    PlatformDescription: PlatformDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PlatformDescriptionTypeDef](./type_defs.md#platformdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAccountAttributesResultTypeDef

```python
# DescribeAccountAttributesResultTypeDef definition

class DescribeAccountAttributesResultTypeDef(TypedDict):
    ResourceQuotas: ResourceQuotasTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceQuotasTypeDef](./type_defs.md#resourcequotastypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ApplicationDescriptionTypeDef

```python
# ApplicationDescriptionTypeDef definition

class ApplicationDescriptionTypeDef(TypedDict):
    ApplicationArn: NotRequired[str],
    ApplicationName: NotRequired[str],
    Description: NotRequired[str],
    DateCreated: NotRequired[datetime],
    DateUpdated: NotRequired[datetime],
    Versions: NotRequired[List[str]],
    ConfigurationTemplates: NotRequired[List[str]],
    ResourceLifecycleConfig: NotRequired[ApplicationResourceLifecycleConfigTypeDef],  # (1)
```

1. See [:material-code-braces: ApplicationResourceLifecycleConfigTypeDef](./type_defs.md#applicationresourcelifecycleconfigtypedef) 
## ApplicationResourceLifecycleDescriptionMessageTypeDef

```python
# ApplicationResourceLifecycleDescriptionMessageTypeDef definition

class ApplicationResourceLifecycleDescriptionMessageTypeDef(TypedDict):
    ApplicationName: str,
    ResourceLifecycleConfig: ApplicationResourceLifecycleConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationResourceLifecycleConfigTypeDef](./type_defs.md#applicationresourcelifecycleconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateApplicationMessageRequestTypeDef

```python
# CreateApplicationMessageRequestTypeDef definition

class CreateApplicationMessageRequestTypeDef(TypedDict):
    ApplicationName: str,
    Description: NotRequired[str],
    ResourceLifecycleConfig: NotRequired[ApplicationResourceLifecycleConfigTypeDef],  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: ApplicationResourceLifecycleConfigTypeDef](./type_defs.md#applicationresourcelifecycleconfigtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateApplicationResourceLifecycleMessageRequestTypeDef

```python
# UpdateApplicationResourceLifecycleMessageRequestTypeDef definition

class UpdateApplicationResourceLifecycleMessageRequestTypeDef(TypedDict):
    ApplicationName: str,
    ResourceLifecycleConfig: ApplicationResourceLifecycleConfigTypeDef,  # (1)
```

1. See [:material-code-braces: ApplicationResourceLifecycleConfigTypeDef](./type_defs.md#applicationresourcelifecycleconfigtypedef) 
## DescribeInstancesHealthResultTypeDef

```python
# DescribeInstancesHealthResultTypeDef definition

class DescribeInstancesHealthResultTypeDef(TypedDict):
    InstanceHealthList: List[SingleInstanceHealthTypeDef],  # (1)
    RefreshedAt: datetime,
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SingleInstanceHealthTypeDef](./type_defs.md#singleinstancehealthtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnvironmentDescriptionResponseTypeDef

```python
# EnvironmentDescriptionResponseTypeDef definition

class EnvironmentDescriptionResponseTypeDef(TypedDict):
    EnvironmentName: str,
    EnvironmentId: str,
    ApplicationName: str,
    VersionLabel: str,
    SolutionStackName: str,
    PlatformArn: str,
    TemplateName: str,
    Description: str,
    EndpointURL: str,
    CNAME: str,
    DateCreated: datetime,
    DateUpdated: datetime,
    Status: EnvironmentStatusType,  # (1)
    AbortableOperationInProgress: bool,
    Health: EnvironmentHealthType,  # (2)
    HealthStatus: EnvironmentHealthStatusType,  # (3)
    Resources: EnvironmentResourcesDescriptionTypeDef,  # (4)
    Tier: EnvironmentTierTypeDef,  # (5)
    EnvironmentLinks: List[EnvironmentLinkTypeDef],  # (6)
    EnvironmentArn: str,
    OperationsRole: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-brackets: EnvironmentStatusType](./literals.md#environmentstatustype) 
2. See [:material-code-brackets: EnvironmentHealthType](./literals.md#environmenthealthtype) 
3. See [:material-code-brackets: EnvironmentHealthStatusType](./literals.md#environmenthealthstatustype) 
4. See [:material-code-braces: EnvironmentResourcesDescriptionTypeDef](./type_defs.md#environmentresourcesdescriptiontypedef) 
5. See [:material-code-braces: EnvironmentTierTypeDef](./type_defs.md#environmenttiertypedef) 
6. See [:material-code-braces: EnvironmentLinkTypeDef](./type_defs.md#environmentlinktypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnvironmentDescriptionTypeDef

```python
# EnvironmentDescriptionTypeDef definition

class EnvironmentDescriptionTypeDef(TypedDict):
    EnvironmentName: NotRequired[str],
    EnvironmentId: NotRequired[str],
    ApplicationName: NotRequired[str],
    VersionLabel: NotRequired[str],
    SolutionStackName: NotRequired[str],
    PlatformArn: NotRequired[str],
    TemplateName: NotRequired[str],
    Description: NotRequired[str],
    EndpointURL: NotRequired[str],
    CNAME: NotRequired[str],
    DateCreated: NotRequired[datetime],
    DateUpdated: NotRequired[datetime],
    Status: NotRequired[EnvironmentStatusType],  # (1)
    AbortableOperationInProgress: NotRequired[bool],
    Health: NotRequired[EnvironmentHealthType],  # (2)
    HealthStatus: NotRequired[EnvironmentHealthStatusType],  # (3)
    Resources: NotRequired[EnvironmentResourcesDescriptionTypeDef],  # (4)
    Tier: NotRequired[EnvironmentTierTypeDef],  # (5)
    EnvironmentLinks: NotRequired[List[EnvironmentLinkTypeDef]],  # (6)
    EnvironmentArn: NotRequired[str],
    OperationsRole: NotRequired[str],
```

1. See [:material-code-brackets: EnvironmentStatusType](./literals.md#environmentstatustype) 
2. See [:material-code-brackets: EnvironmentHealthType](./literals.md#environmenthealthtype) 
3. See [:material-code-brackets: EnvironmentHealthStatusType](./literals.md#environmenthealthstatustype) 
4. See [:material-code-braces: EnvironmentResourcesDescriptionTypeDef](./type_defs.md#environmentresourcesdescriptiontypedef) 
5. See [:material-code-braces: EnvironmentTierTypeDef](./type_defs.md#environmenttiertypedef) 
6. See [:material-code-braces: EnvironmentLinkTypeDef](./type_defs.md#environmentlinktypedef) 
## ApplicationDescriptionMessageTypeDef

```python
# ApplicationDescriptionMessageTypeDef definition

class ApplicationDescriptionMessageTypeDef(TypedDict):
    Application: ApplicationDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationDescriptionTypeDef](./type_defs.md#applicationdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ApplicationDescriptionsMessageTypeDef

```python
# ApplicationDescriptionsMessageTypeDef definition

class ApplicationDescriptionsMessageTypeDef(TypedDict):
    Applications: List[ApplicationDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationDescriptionTypeDef](./type_defs.md#applicationdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnvironmentDescriptionsMessageTypeDef

```python
# EnvironmentDescriptionsMessageTypeDef definition

class EnvironmentDescriptionsMessageTypeDef(TypedDict):
    Environments: List[EnvironmentDescriptionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentDescriptionTypeDef](./type_defs.md#environmentdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
