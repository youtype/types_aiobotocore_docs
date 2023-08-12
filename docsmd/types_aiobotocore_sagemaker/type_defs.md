# Type definitions

> [Index](../README.md) > [SageMaker](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SageMaker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
    type annotations stubs module [types-aiobotocore-sagemaker](https://pypi.org/project/types-aiobotocore-sagemaker/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## ActionSourceTypeDef

```python
# ActionSourceTypeDef definition

class ActionSourceTypeDef(TypedDict):
    SourceUri: str,
    SourceType: NotRequired[str],
    SourceId: NotRequired[str],
```

## AddAssociationRequestRequestTypeDef

```python
# AddAssociationRequestRequestTypeDef definition

class AddAssociationRequestRequestTypeDef(TypedDict):
    SourceArn: str,
    DestinationArn: str,
    AssociationType: NotRequired[AssociationEdgeTypeType],  # (1)
```

1. See [:material-code-brackets: AssociationEdgeTypeType](./literals.md#associationedgetypetype) 
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

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## AgentVersionTypeDef

```python
# AgentVersionTypeDef definition

class AgentVersionTypeDef(TypedDict):
    Version: str,
    AgentCount: int,
```

## AlarmTypeDef

```python
# AlarmTypeDef definition

class AlarmTypeDef(TypedDict):
    AlarmName: NotRequired[str],
```

## MetricDefinitionTypeDef

```python
# MetricDefinitionTypeDef definition

class MetricDefinitionTypeDef(TypedDict):
    Name: str,
    Regex: str,
```

## AlgorithmStatusItemTypeDef

```python
# AlgorithmStatusItemTypeDef definition

class AlgorithmStatusItemTypeDef(TypedDict):
    Name: str,
    Status: DetailedAlgorithmStatusType,  # (1)
    FailureReason: NotRequired[str],
```

1. See [:material-code-brackets: DetailedAlgorithmStatusType](./literals.md#detailedalgorithmstatustype) 
## AlgorithmSummaryTypeDef

```python
# AlgorithmSummaryTypeDef definition

class AlgorithmSummaryTypeDef(TypedDict):
    AlgorithmName: str,
    AlgorithmArn: str,
    CreationTime: datetime,
    AlgorithmStatus: AlgorithmStatusType,  # (1)
    AlgorithmDescription: NotRequired[str],
```

1. See [:material-code-brackets: AlgorithmStatusType](./literals.md#algorithmstatustype) 
## AnnotationConsolidationConfigTypeDef

```python
# AnnotationConsolidationConfigTypeDef definition

class AnnotationConsolidationConfigTypeDef(TypedDict):
    AnnotationConsolidationLambdaArn: str,
```

## AppDetailsTypeDef

```python
# AppDetailsTypeDef definition

class AppDetailsTypeDef(TypedDict):
    DomainId: NotRequired[str],
    UserProfileName: NotRequired[str],
    AppType: NotRequired[AppTypeType],  # (1)
    AppName: NotRequired[str],
    Status: NotRequired[AppStatusType],  # (2)
    CreationTime: NotRequired[datetime],
    SpaceName: NotRequired[str],
```

1. See [:material-code-brackets: AppTypeType](./literals.md#apptypetype) 
2. See [:material-code-brackets: AppStatusType](./literals.md#appstatustype) 
## AppSpecificationTypeDef

```python
# AppSpecificationTypeDef definition

class AppSpecificationTypeDef(TypedDict):
    ImageUri: str,
    ContainerEntrypoint: NotRequired[Sequence[str]],
    ContainerArguments: NotRequired[Sequence[str]],
```

## ArtifactSourceTypeTypeDef

```python
# ArtifactSourceTypeTypeDef definition

class ArtifactSourceTypeTypeDef(TypedDict):
    SourceIdType: ArtifactSourceIdTypeType,  # (1)
    Value: str,
```

1. See [:material-code-brackets: ArtifactSourceIdTypeType](./literals.md#artifactsourceidtypetype) 
## AssociateTrialComponentRequestRequestTypeDef

```python
# AssociateTrialComponentRequestRequestTypeDef definition

class AssociateTrialComponentRequestRequestTypeDef(TypedDict):
    TrialComponentName: str,
    TrialName: str,
```

## AsyncInferenceClientConfigTypeDef

```python
# AsyncInferenceClientConfigTypeDef definition

class AsyncInferenceClientConfigTypeDef(TypedDict):
    MaxConcurrentInvocationsPerInstance: NotRequired[int],
```

## AsyncInferenceNotificationConfigTypeDef

```python
# AsyncInferenceNotificationConfigTypeDef definition

class AsyncInferenceNotificationConfigTypeDef(TypedDict):
    SuccessTopic: NotRequired[str],
    ErrorTopic: NotRequired[str],
    IncludeInferenceResponseIn: NotRequired[Sequence[AsyncNotificationTopicTypesType]],  # (1)
```

1. See [:material-code-brackets: AsyncNotificationTopicTypesType](./literals.md#asyncnotificationtopictypestype) 
## AthenaDatasetDefinitionTypeDef

```python
# AthenaDatasetDefinitionTypeDef definition

class AthenaDatasetDefinitionTypeDef(TypedDict):
    Catalog: str,
    Database: str,
    QueryString: str,
    OutputS3Uri: str,
    OutputFormat: AthenaResultFormatType,  # (1)
    WorkGroup: NotRequired[str],
    KmsKeyId: NotRequired[str],
    OutputCompression: NotRequired[AthenaResultCompressionTypeType],  # (2)
```

1. See [:material-code-brackets: AthenaResultFormatType](./literals.md#athenaresultformattype) 
2. See [:material-code-brackets: AthenaResultCompressionTypeType](./literals.md#athenaresultcompressiontypetype) 
## AutoMLAlgorithmConfigTypeDef

```python
# AutoMLAlgorithmConfigTypeDef definition

class AutoMLAlgorithmConfigTypeDef(TypedDict):
    AutoMLAlgorithms: Sequence[AutoMLAlgorithmType],  # (1)
```

1. See [:material-code-brackets: AutoMLAlgorithmType](./literals.md#automlalgorithmtype) 
## AutoMLCandidateStepTypeDef

```python
# AutoMLCandidateStepTypeDef definition

class AutoMLCandidateStepTypeDef(TypedDict):
    CandidateStepType: CandidateStepTypeType,  # (1)
    CandidateStepArn: str,
    CandidateStepName: str,
```

1. See [:material-code-brackets: CandidateStepTypeType](./literals.md#candidatesteptypetype) 
## AutoMLContainerDefinitionTypeDef

```python
# AutoMLContainerDefinitionTypeDef definition

class AutoMLContainerDefinitionTypeDef(TypedDict):
    Image: str,
    ModelDataUrl: str,
    Environment: NotRequired[Dict[str, str]],
```

## FinalAutoMLJobObjectiveMetricTypeDef

```python
# FinalAutoMLJobObjectiveMetricTypeDef definition

class FinalAutoMLJobObjectiveMetricTypeDef(TypedDict):
    MetricName: AutoMLMetricEnumType,  # (2)
    Value: float,
    Type: NotRequired[AutoMLJobObjectiveTypeType],  # (1)
    StandardMetricName: NotRequired[AutoMLMetricEnumType],  # (2)
```

1. See [:material-code-brackets: AutoMLJobObjectiveTypeType](./literals.md#automljobobjectivetypetype) 
2. See [:material-code-brackets: AutoMLMetricEnumType](./literals.md#automlmetricenumtype) 
3. See [:material-code-brackets: AutoMLMetricEnumType](./literals.md#automlmetricenumtype) 
## AutoMLS3DataSourceTypeDef

```python
# AutoMLS3DataSourceTypeDef definition

class AutoMLS3DataSourceTypeDef(TypedDict):
    S3DataType: AutoMLS3DataTypeType,  # (1)
    S3Uri: str,
```

1. See [:material-code-brackets: AutoMLS3DataTypeType](./literals.md#automls3datatypetype) 
## AutoMLDataSplitConfigTypeDef

```python
# AutoMLDataSplitConfigTypeDef definition

class AutoMLDataSplitConfigTypeDef(TypedDict):
    ValidationFraction: NotRequired[float],
```

## AutoMLJobArtifactsTypeDef

```python
# AutoMLJobArtifactsTypeDef definition

class AutoMLJobArtifactsTypeDef(TypedDict):
    CandidateDefinitionNotebookLocation: NotRequired[str],
    DataExplorationNotebookLocation: NotRequired[str],
```

## AutoMLJobCompletionCriteriaTypeDef

```python
# AutoMLJobCompletionCriteriaTypeDef definition

class AutoMLJobCompletionCriteriaTypeDef(TypedDict):
    MaxCandidates: NotRequired[int],
    MaxRuntimePerTrainingJobInSeconds: NotRequired[int],
    MaxAutoMLJobRuntimeInSeconds: NotRequired[int],
```

## AutoMLJobObjectiveTypeDef

```python
# AutoMLJobObjectiveTypeDef definition

class AutoMLJobObjectiveTypeDef(TypedDict):
    MetricName: AutoMLMetricEnumType,  # (1)
```

1. See [:material-code-brackets: AutoMLMetricEnumType](./literals.md#automlmetricenumtype) 
## AutoMLJobStepMetadataTypeDef

```python
# AutoMLJobStepMetadataTypeDef definition

class AutoMLJobStepMetadataTypeDef(TypedDict):
    Arn: NotRequired[str],
```

## AutoMLPartialFailureReasonTypeDef

```python
# AutoMLPartialFailureReasonTypeDef definition

class AutoMLPartialFailureReasonTypeDef(TypedDict):
    PartialFailureMessage: NotRequired[str],
```

## AutoMLOutputDataConfigTypeDef

```python
# AutoMLOutputDataConfigTypeDef definition

class AutoMLOutputDataConfigTypeDef(TypedDict):
    S3OutputPath: str,
    KmsKeyId: NotRequired[str],
```

## TabularResolvedAttributesTypeDef

```python
# TabularResolvedAttributesTypeDef definition

class TabularResolvedAttributesTypeDef(TypedDict):
    ProblemType: NotRequired[ProblemTypeType],  # (1)
```

1. See [:material-code-brackets: ProblemTypeType](./literals.md#problemtypetype) 
## VpcConfigTypeDef

```python
# VpcConfigTypeDef definition

class VpcConfigTypeDef(TypedDict):
    SecurityGroupIds: Sequence[str],
    Subnets: Sequence[str],
```

## AutoParameterTypeDef

```python
# AutoParameterTypeDef definition

class AutoParameterTypeDef(TypedDict):
    Name: str,
    ValueHint: str,
```

## AutotuneTypeDef

```python
# AutotuneTypeDef definition

class AutotuneTypeDef(TypedDict):
    Mode: AutotuneModeType,  # (1)
```

1. See [:material-code-brackets: AutotuneModeType](./literals.md#autotunemodetype) 
## BatchDataCaptureConfigTypeDef

```python
# BatchDataCaptureConfigTypeDef definition

class BatchDataCaptureConfigTypeDef(TypedDict):
    DestinationS3Uri: str,
    KmsKeyId: NotRequired[str],
    GenerateInferenceId: NotRequired[bool],
```

## BatchDescribeModelPackageErrorTypeDef

```python
# BatchDescribeModelPackageErrorTypeDef definition

class BatchDescribeModelPackageErrorTypeDef(TypedDict):
    ErrorCode: str,
    ErrorResponse: str,
```

## BatchDescribeModelPackageInputRequestTypeDef

```python
# BatchDescribeModelPackageInputRequestTypeDef definition

class BatchDescribeModelPackageInputRequestTypeDef(TypedDict):
    ModelPackageArnList: Sequence[str],
```

## BestObjectiveNotImprovingTypeDef

```python
# BestObjectiveNotImprovingTypeDef definition

class BestObjectiveNotImprovingTypeDef(TypedDict):
    MaxNumberOfTrainingJobsNotImproving: NotRequired[int],
```

## MetricsSourceTypeDef

```python
# MetricsSourceTypeDef definition

class MetricsSourceTypeDef(TypedDict):
    ContentType: str,
    S3Uri: str,
    ContentDigest: NotRequired[str],
```

## CacheHitResultTypeDef

```python
# CacheHitResultTypeDef definition

class CacheHitResultTypeDef(TypedDict):
    SourcePipelineExecutionArn: NotRequired[str],
```

## OutputParameterTypeDef

```python
# OutputParameterTypeDef definition

class OutputParameterTypeDef(TypedDict):
    Name: str,
    Value: str,
```

## CandidateArtifactLocationsTypeDef

```python
# CandidateArtifactLocationsTypeDef definition

class CandidateArtifactLocationsTypeDef(TypedDict):
    Explainability: str,
    ModelInsights: NotRequired[str],
    BacktestResults: NotRequired[str],
```

## MetricDatumTypeDef

```python
# MetricDatumTypeDef definition

class MetricDatumTypeDef(TypedDict):
    MetricName: NotRequired[AutoMLMetricEnumType],  # (1)
    Value: NotRequired[float],
    Set: NotRequired[MetricSetSourceType],  # (2)
    StandardMetricName: NotRequired[AutoMLMetricExtendedEnumType],  # (3)
```

1. See [:material-code-brackets: AutoMLMetricEnumType](./literals.md#automlmetricenumtype) 
2. See [:material-code-brackets: MetricSetSourceType](./literals.md#metricsetsourcetype) 
3. See [:material-code-brackets: AutoMLMetricExtendedEnumType](./literals.md#automlmetricextendedenumtype) 
## ModelRegisterSettingsTypeDef

```python
# ModelRegisterSettingsTypeDef definition

class ModelRegisterSettingsTypeDef(TypedDict):
    Status: NotRequired[FeatureStatusType],  # (1)
    CrossAccountModelRegisterRoleArn: NotRequired[str],
```

1. See [:material-code-brackets: FeatureStatusType](./literals.md#featurestatustype) 
## TimeSeriesForecastingSettingsTypeDef

```python
# TimeSeriesForecastingSettingsTypeDef definition

class TimeSeriesForecastingSettingsTypeDef(TypedDict):
    Status: NotRequired[FeatureStatusType],  # (1)
    AmazonForecastRoleArn: NotRequired[str],
```

1. See [:material-code-brackets: FeatureStatusType](./literals.md#featurestatustype) 
## WorkspaceSettingsTypeDef

```python
# WorkspaceSettingsTypeDef definition

class WorkspaceSettingsTypeDef(TypedDict):
    S3ArtifactPath: NotRequired[str],
    S3KmsKeyId: NotRequired[str],
```

## CapacitySizeTypeDef

```python
# CapacitySizeTypeDef definition

class CapacitySizeTypeDef(TypedDict):
    Type: CapacitySizeTypeType,  # (1)
    Value: int,
```

1. See [:material-code-brackets: CapacitySizeTypeType](./literals.md#capacitysizetypetype) 
## CaptureContentTypeHeaderTypeDef

```python
# CaptureContentTypeHeaderTypeDef definition

class CaptureContentTypeHeaderTypeDef(TypedDict):
    CsvContentTypes: NotRequired[Sequence[str]],
    JsonContentTypes: NotRequired[Sequence[str]],
```

## CaptureOptionTypeDef

```python
# CaptureOptionTypeDef definition

class CaptureOptionTypeDef(TypedDict):
    CaptureMode: CaptureModeType,  # (1)
```

1. See [:material-code-brackets: CaptureModeType](./literals.md#capturemodetype) 
## CategoricalParameterRangeSpecificationTypeDef

```python
# CategoricalParameterRangeSpecificationTypeDef definition

class CategoricalParameterRangeSpecificationTypeDef(TypedDict):
    Values: Sequence[str],
```

## CategoricalParameterRangeTypeDef

```python
# CategoricalParameterRangeTypeDef definition

class CategoricalParameterRangeTypeDef(TypedDict):
    Name: str,
    Values: Sequence[str],
```

## CategoricalParameterTypeDef

```python
# CategoricalParameterTypeDef definition

class CategoricalParameterTypeDef(TypedDict):
    Name: str,
    Value: Sequence[str],
```

## ChannelSpecificationTypeDef

```python
# ChannelSpecificationTypeDef definition

class ChannelSpecificationTypeDef(TypedDict):
    Name: str,
    SupportedContentTypes: Sequence[str],
    SupportedInputModes: Sequence[TrainingInputModeType],  # (2)
    Description: NotRequired[str],
    IsRequired: NotRequired[bool],
    SupportedCompressionTypes: NotRequired[Sequence[CompressionTypeType]],  # (1)
```

1. See [:material-code-brackets: CompressionTypeType](./literals.md#compressiontypetype) 
2. See [:material-code-brackets: TrainingInputModeType](./literals.md#traininginputmodetype) 
## ShuffleConfigTypeDef

```python
# ShuffleConfigTypeDef definition

class ShuffleConfigTypeDef(TypedDict):
    Seed: int,
```

## CheckpointConfigTypeDef

```python
# CheckpointConfigTypeDef definition

class CheckpointConfigTypeDef(TypedDict):
    S3Uri: str,
    LocalPath: NotRequired[str],
```

## ClarifyCheckStepMetadataTypeDef

```python
# ClarifyCheckStepMetadataTypeDef definition

class ClarifyCheckStepMetadataTypeDef(TypedDict):
    CheckType: NotRequired[str],
    BaselineUsedForDriftCheckConstraints: NotRequired[str],
    CalculatedBaselineConstraints: NotRequired[str],
    ModelPackageGroupName: NotRequired[str],
    ViolationReport: NotRequired[str],
    CheckJobArn: NotRequired[str],
    SkipCheck: NotRequired[bool],
    RegisterNewBaseline: NotRequired[bool],
```

## ClarifyInferenceConfigTypeDef

```python
# ClarifyInferenceConfigTypeDef definition

class ClarifyInferenceConfigTypeDef(TypedDict):
    FeaturesAttribute: NotRequired[str],
    ContentTemplate: NotRequired[str],
    MaxRecordCount: NotRequired[int],
    MaxPayloadInMB: NotRequired[int],
    ProbabilityIndex: NotRequired[int],
    LabelIndex: NotRequired[int],
    ProbabilityAttribute: NotRequired[str],
    LabelAttribute: NotRequired[str],
    LabelHeaders: NotRequired[Sequence[str]],
    FeatureHeaders: NotRequired[Sequence[str]],
    FeatureTypes: NotRequired[Sequence[ClarifyFeatureTypeType]],  # (1)
```

1. See [:material-code-brackets: ClarifyFeatureTypeType](./literals.md#clarifyfeaturetypetype) 
## ClarifyShapBaselineConfigTypeDef

```python
# ClarifyShapBaselineConfigTypeDef definition

class ClarifyShapBaselineConfigTypeDef(TypedDict):
    MimeType: NotRequired[str],
    ShapBaseline: NotRequired[str],
    ShapBaselineUri: NotRequired[str],
```

## ClarifyTextConfigTypeDef

```python
# ClarifyTextConfigTypeDef definition

class ClarifyTextConfigTypeDef(TypedDict):
    Language: ClarifyTextLanguageType,  # (1)
    Granularity: ClarifyTextGranularityType,  # (2)
```

1. See [:material-code-brackets: ClarifyTextLanguageType](./literals.md#clarifytextlanguagetype) 
2. See [:material-code-brackets: ClarifyTextGranularityType](./literals.md#clarifytextgranularitytype) 
## GitConfigTypeDef

```python
# GitConfigTypeDef definition

class GitConfigTypeDef(TypedDict):
    RepositoryUrl: str,
    Branch: NotRequired[str],
    SecretArn: NotRequired[str],
```

## CodeRepositoryTypeDef

```python
# CodeRepositoryTypeDef definition

class CodeRepositoryTypeDef(TypedDict):
    RepositoryUrl: str,
```

## CognitoConfigTypeDef

```python
# CognitoConfigTypeDef definition

class CognitoConfigTypeDef(TypedDict):
    UserPool: str,
    ClientId: str,
```

## CognitoMemberDefinitionTypeDef

```python
# CognitoMemberDefinitionTypeDef definition

class CognitoMemberDefinitionTypeDef(TypedDict):
    UserPool: str,
    UserGroup: str,
    ClientId: str,
```

## CollectionConfigurationTypeDef

```python
# CollectionConfigurationTypeDef definition

class CollectionConfigurationTypeDef(TypedDict):
    CollectionName: NotRequired[str],
    CollectionParameters: NotRequired[Mapping[str, str]],
```

## CompilationJobSummaryTypeDef

```python
# CompilationJobSummaryTypeDef definition

class CompilationJobSummaryTypeDef(TypedDict):
    CompilationJobName: str,
    CompilationJobArn: str,
    CreationTime: datetime,
    CompilationJobStatus: CompilationJobStatusType,  # (5)
    CompilationStartTime: NotRequired[datetime],
    CompilationEndTime: NotRequired[datetime],
    CompilationTargetDevice: NotRequired[TargetDeviceType],  # (1)
    CompilationTargetPlatformOs: NotRequired[TargetPlatformOsType],  # (2)
    CompilationTargetPlatformArch: NotRequired[TargetPlatformArchType],  # (3)
    CompilationTargetPlatformAccelerator: NotRequired[TargetPlatformAcceleratorType],  # (4)
    LastModifiedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: TargetDeviceType](./literals.md#targetdevicetype) 
2. See [:material-code-brackets: TargetPlatformOsType](./literals.md#targetplatformostype) 
3. See [:material-code-brackets: TargetPlatformArchType](./literals.md#targetplatformarchtype) 
4. See [:material-code-brackets: TargetPlatformAcceleratorType](./literals.md#targetplatformacceleratortype) 
5. See [:material-code-brackets: CompilationJobStatusType](./literals.md#compilationjobstatustype) 
## ConditionStepMetadataTypeDef

```python
# ConditionStepMetadataTypeDef definition

class ConditionStepMetadataTypeDef(TypedDict):
    Outcome: NotRequired[ConditionOutcomeType],  # (1)
```

1. See [:material-code-brackets: ConditionOutcomeType](./literals.md#conditionoutcometype) 
## MultiModelConfigTypeDef

```python
# MultiModelConfigTypeDef definition

class MultiModelConfigTypeDef(TypedDict):
    ModelCacheSetting: NotRequired[ModelCacheSettingType],  # (1)
```

1. See [:material-code-brackets: ModelCacheSettingType](./literals.md#modelcachesettingtype) 
## ContextSourceTypeDef

```python
# ContextSourceTypeDef definition

class ContextSourceTypeDef(TypedDict):
    SourceUri: str,
    SourceType: NotRequired[str],
    SourceId: NotRequired[str],
```

## ContinuousParameterRangeSpecificationTypeDef

```python
# ContinuousParameterRangeSpecificationTypeDef definition

class ContinuousParameterRangeSpecificationTypeDef(TypedDict):
    MinValue: str,
    MaxValue: str,
```

## ContinuousParameterRangeTypeDef

```python
# ContinuousParameterRangeTypeDef definition

class ContinuousParameterRangeTypeDef(TypedDict):
    Name: str,
    MinValue: str,
    MaxValue: str,
    ScalingType: NotRequired[HyperParameterScalingTypeType],  # (1)
```

1. See [:material-code-brackets: HyperParameterScalingTypeType](./literals.md#hyperparameterscalingtypetype) 
## ConvergenceDetectedTypeDef

```python
# ConvergenceDetectedTypeDef definition

class ConvergenceDetectedTypeDef(TypedDict):
    CompleteOnConvergence: NotRequired[CompleteOnConvergenceType],  # (1)
```

1. See [:material-code-brackets: CompleteOnConvergenceType](./literals.md#completeonconvergencetype) 
## MetadataPropertiesTypeDef

```python
# MetadataPropertiesTypeDef definition

class MetadataPropertiesTypeDef(TypedDict):
    CommitId: NotRequired[str],
    Repository: NotRequired[str],
    GeneratedBy: NotRequired[str],
    ProjectId: NotRequired[str],
```

## ResourceSpecTypeDef

```python
# ResourceSpecTypeDef definition

class ResourceSpecTypeDef(TypedDict):
    SageMakerImageArn: NotRequired[str],
    SageMakerImageVersionArn: NotRequired[str],
    InstanceType: NotRequired[AppInstanceTypeType],  # (1)
    LifecycleConfigArn: NotRequired[str],
```

1. See [:material-code-brackets: AppInstanceTypeType](./literals.md#appinstancetypetype) 
## ModelDeployConfigTypeDef

```python
# ModelDeployConfigTypeDef definition

class ModelDeployConfigTypeDef(TypedDict):
    AutoGenerateEndpointName: NotRequired[bool],
    EndpointName: NotRequired[str],
```

## InputConfigTypeDef

```python
# InputConfigTypeDef definition

class InputConfigTypeDef(TypedDict):
    S3Uri: str,
    DataInputConfig: str,
    Framework: FrameworkType,  # (1)
    FrameworkVersion: NotRequired[str],
```

1. See [:material-code-brackets: FrameworkType](./literals.md#frameworktype) 
## NeoVpcConfigTypeDef

```python
# NeoVpcConfigTypeDef definition

class NeoVpcConfigTypeDef(TypedDict):
    SecurityGroupIds: Sequence[str],
    Subnets: Sequence[str],
```

## StoppingConditionTypeDef

```python
# StoppingConditionTypeDef definition

class StoppingConditionTypeDef(TypedDict):
    MaxRuntimeInSeconds: NotRequired[int],
    MaxWaitTimeInSeconds: NotRequired[int],
```

## DataQualityAppSpecificationTypeDef

```python
# DataQualityAppSpecificationTypeDef definition

class DataQualityAppSpecificationTypeDef(TypedDict):
    ImageUri: str,
    ContainerEntrypoint: NotRequired[Sequence[str]],
    ContainerArguments: NotRequired[Sequence[str]],
    RecordPreprocessorSourceUri: NotRequired[str],
    PostAnalyticsProcessorSourceUri: NotRequired[str],
    Environment: NotRequired[Mapping[str, str]],
```

## MonitoringStoppingConditionTypeDef

```python
# MonitoringStoppingConditionTypeDef definition

class MonitoringStoppingConditionTypeDef(TypedDict):
    MaxRuntimeInSeconds: int,
```

## EdgeOutputConfigTypeDef

```python
# EdgeOutputConfigTypeDef definition

class EdgeOutputConfigTypeDef(TypedDict):
    S3OutputLocation: str,
    KmsKeyId: NotRequired[str],
    PresetDeploymentType: NotRequired[EdgePresetDeploymentTypeType],  # (1)
    PresetDeploymentConfig: NotRequired[str],
```

1. See [:material-code-brackets: EdgePresetDeploymentTypeType](./literals.md#edgepresetdeploymenttypetype) 
## EdgeDeploymentModelConfigTypeDef

```python
# EdgeDeploymentModelConfigTypeDef definition

class EdgeDeploymentModelConfigTypeDef(TypedDict):
    ModelHandle: str,
    EdgePackagingJobName: str,
```

## FeatureDefinitionTypeDef

```python
# FeatureDefinitionTypeDef definition

class FeatureDefinitionTypeDef(TypedDict):
    FeatureName: NotRequired[str],
    FeatureType: NotRequired[FeatureTypeType],  # (1)
```

1. See [:material-code-brackets: FeatureTypeType](./literals.md#featuretypetype) 
## FlowDefinitionOutputConfigTypeDef

```python
# FlowDefinitionOutputConfigTypeDef definition

class FlowDefinitionOutputConfigTypeDef(TypedDict):
    S3OutputPath: str,
    KmsKeyId: NotRequired[str],
```

## HumanLoopRequestSourceTypeDef

```python
# HumanLoopRequestSourceTypeDef definition

class HumanLoopRequestSourceTypeDef(TypedDict):
    AwsManagedHumanLoopRequestSource: AwsManagedHumanLoopRequestSourceType,  # (1)
```

1. See [:material-code-brackets: AwsManagedHumanLoopRequestSourceType](./literals.md#awsmanagedhumanlooprequestsourcetype) 
## HubS3StorageConfigTypeDef

```python
# HubS3StorageConfigTypeDef definition

class HubS3StorageConfigTypeDef(TypedDict):
    S3OutputPath: NotRequired[str],
```

## UiTemplateTypeDef

```python
# UiTemplateTypeDef definition

class UiTemplateTypeDef(TypedDict):
    Content: str,
```

## CreateImageVersionRequestRequestTypeDef

```python
# CreateImageVersionRequestRequestTypeDef definition

class CreateImageVersionRequestRequestTypeDef(TypedDict):
    BaseImage: str,
    ClientToken: str,
    ImageName: str,
    Aliases: NotRequired[Sequence[str]],
    VendorGuidance: NotRequired[VendorGuidanceType],  # (1)
    JobType: NotRequired[JobTypeType],  # (2)
    MLFramework: NotRequired[str],
    ProgrammingLang: NotRequired[str],
    Processor: NotRequired[ProcessorType],  # (3)
    Horovod: NotRequired[bool],
    ReleaseNotes: NotRequired[str],
```

1. See [:material-code-brackets: VendorGuidanceType](./literals.md#vendorguidancetype) 
2. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
3. See [:material-code-brackets: ProcessorType](./literals.md#processortype) 
## LabelingJobOutputConfigTypeDef

```python
# LabelingJobOutputConfigTypeDef definition

class LabelingJobOutputConfigTypeDef(TypedDict):
    S3OutputPath: str,
    KmsKeyId: NotRequired[str],
    SnsTopicArn: NotRequired[str],
```

## LabelingJobStoppingConditionsTypeDef

```python
# LabelingJobStoppingConditionsTypeDef definition

class LabelingJobStoppingConditionsTypeDef(TypedDict):
    MaxHumanLabeledObjectCount: NotRequired[int],
    MaxPercentageOfInputDatasetLabeled: NotRequired[int],
```

## ModelBiasAppSpecificationTypeDef

```python
# ModelBiasAppSpecificationTypeDef definition

class ModelBiasAppSpecificationTypeDef(TypedDict):
    ImageUri: str,
    ConfigUri: str,
    Environment: NotRequired[Mapping[str, str]],
```

## ModelCardExportOutputConfigTypeDef

```python
# ModelCardExportOutputConfigTypeDef definition

class ModelCardExportOutputConfigTypeDef(TypedDict):
    S3OutputPath: str,
```

## ModelCardSecurityConfigTypeDef

```python
# ModelCardSecurityConfigTypeDef definition

class ModelCardSecurityConfigTypeDef(TypedDict):
    KmsKeyId: NotRequired[str],
```

## ModelExplainabilityAppSpecificationTypeDef

```python
# ModelExplainabilityAppSpecificationTypeDef definition

class ModelExplainabilityAppSpecificationTypeDef(TypedDict):
    ImageUri: str,
    ConfigUri: str,
    Environment: NotRequired[Mapping[str, str]],
```

## InferenceExecutionConfigTypeDef

```python
# InferenceExecutionConfigTypeDef definition

class InferenceExecutionConfigTypeDef(TypedDict):
    Mode: InferenceExecutionModeType,  # (1)
```

1. See [:material-code-brackets: InferenceExecutionModeType](./literals.md#inferenceexecutionmodetype) 
## ModelQualityAppSpecificationTypeDef

```python
# ModelQualityAppSpecificationTypeDef definition

class ModelQualityAppSpecificationTypeDef(TypedDict):
    ImageUri: str,
    ContainerEntrypoint: NotRequired[Sequence[str]],
    ContainerArguments: NotRequired[Sequence[str]],
    RecordPreprocessorSourceUri: NotRequired[str],
    PostAnalyticsProcessorSourceUri: NotRequired[str],
    ProblemType: NotRequired[MonitoringProblemTypeType],  # (1)
    Environment: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: MonitoringProblemTypeType](./literals.md#monitoringproblemtypetype) 
## InstanceMetadataServiceConfigurationTypeDef

```python
# InstanceMetadataServiceConfigurationTypeDef definition

class InstanceMetadataServiceConfigurationTypeDef(TypedDict):
    MinimumInstanceMetadataServiceVersion: str,
```

## NotebookInstanceLifecycleHookTypeDef

```python
# NotebookInstanceLifecycleHookTypeDef definition

class NotebookInstanceLifecycleHookTypeDef(TypedDict):
    Content: NotRequired[str],
```

## ParallelismConfigurationTypeDef

```python
# ParallelismConfigurationTypeDef definition

class ParallelismConfigurationTypeDef(TypedDict):
    MaxParallelExecutionSteps: int,
```

## PipelineDefinitionS3LocationTypeDef

```python
# PipelineDefinitionS3LocationTypeDef definition

class PipelineDefinitionS3LocationTypeDef(TypedDict):
    Bucket: str,
    ObjectKey: str,
    VersionId: NotRequired[str],
```

## CreatePresignedDomainUrlRequestRequestTypeDef

```python
# CreatePresignedDomainUrlRequestRequestTypeDef definition

class CreatePresignedDomainUrlRequestRequestTypeDef(TypedDict):
    DomainId: str,
    UserProfileName: str,
    SessionExpirationDurationInSeconds: NotRequired[int],
    ExpiresInSeconds: NotRequired[int],
    SpaceName: NotRequired[str],
```

## CreatePresignedNotebookInstanceUrlInputRequestTypeDef

```python
# CreatePresignedNotebookInstanceUrlInputRequestTypeDef definition

class CreatePresignedNotebookInstanceUrlInputRequestTypeDef(TypedDict):
    NotebookInstanceName: str,
    SessionExpirationDurationInSeconds: NotRequired[int],
```

## ExperimentConfigTypeDef

```python
# ExperimentConfigTypeDef definition

class ExperimentConfigTypeDef(TypedDict):
    ExperimentName: NotRequired[str],
    TrialName: NotRequired[str],
    TrialComponentDisplayName: NotRequired[str],
    RunName: NotRequired[str],
```

## ProcessingStoppingConditionTypeDef

```python
# ProcessingStoppingConditionTypeDef definition

class ProcessingStoppingConditionTypeDef(TypedDict):
    MaxRuntimeInSeconds: int,
```

## DebugRuleConfigurationTypeDef

```python
# DebugRuleConfigurationTypeDef definition

class DebugRuleConfigurationTypeDef(TypedDict):
    RuleConfigurationName: str,
    RuleEvaluatorImage: str,
    LocalPath: NotRequired[str],
    S3OutputPath: NotRequired[str],
    InstanceType: NotRequired[ProcessingInstanceTypeType],  # (1)
    VolumeSizeInGB: NotRequired[int],
    RuleParameters: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ProcessingInstanceTypeType](./literals.md#processinginstancetypetype) 
## OutputDataConfigTypeDef

```python
# OutputDataConfigTypeDef definition

class OutputDataConfigTypeDef(TypedDict):
    S3OutputPath: str,
    KmsKeyId: NotRequired[str],
    CompressionType: NotRequired[OutputCompressionTypeType],  # (1)
```

1. See [:material-code-brackets: OutputCompressionTypeType](./literals.md#outputcompressiontypetype) 
## ProfilerConfigTypeDef

```python
# ProfilerConfigTypeDef definition

class ProfilerConfigTypeDef(TypedDict):
    S3OutputPath: NotRequired[str],
    ProfilingIntervalInMilliseconds: NotRequired[int],
    ProfilingParameters: NotRequired[Mapping[str, str]],
    DisableProfiler: NotRequired[bool],
```

## ProfilerRuleConfigurationTypeDef

```python
# ProfilerRuleConfigurationTypeDef definition

class ProfilerRuleConfigurationTypeDef(TypedDict):
    RuleConfigurationName: str,
    RuleEvaluatorImage: str,
    LocalPath: NotRequired[str],
    S3OutputPath: NotRequired[str],
    InstanceType: NotRequired[ProcessingInstanceTypeType],  # (1)
    VolumeSizeInGB: NotRequired[int],
    RuleParameters: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ProcessingInstanceTypeType](./literals.md#processinginstancetypetype) 
## RetryStrategyTypeDef

```python
# RetryStrategyTypeDef definition

class RetryStrategyTypeDef(TypedDict):
    MaximumRetryAttempts: int,
```

## TensorBoardOutputConfigTypeDef

```python
# TensorBoardOutputConfigTypeDef definition

class TensorBoardOutputConfigTypeDef(TypedDict):
    S3OutputPath: str,
    LocalPath: NotRequired[str],
```

## DataProcessingTypeDef

```python
# DataProcessingTypeDef definition

class DataProcessingTypeDef(TypedDict):
    InputFilter: NotRequired[str],
    OutputFilter: NotRequired[str],
    JoinSource: NotRequired[JoinSourceType],  # (1)
```

1. See [:material-code-brackets: JoinSourceType](./literals.md#joinsourcetype) 
## ModelClientConfigTypeDef

```python
# ModelClientConfigTypeDef definition

class ModelClientConfigTypeDef(TypedDict):
    InvocationsTimeoutInSeconds: NotRequired[int],
    InvocationsMaxRetries: NotRequired[int],
```

## TransformOutputTypeDef

```python
# TransformOutputTypeDef definition

class TransformOutputTypeDef(TypedDict):
    S3OutputPath: str,
    Accept: NotRequired[str],
    AssembleWith: NotRequired[AssemblyTypeType],  # (1)
    KmsKeyId: NotRequired[str],
```

1. See [:material-code-brackets: AssemblyTypeType](./literals.md#assemblytypetype) 
## TransformResourcesTypeDef

```python
# TransformResourcesTypeDef definition

class TransformResourcesTypeDef(TypedDict):
    InstanceType: TransformInstanceTypeType,  # (1)
    InstanceCount: int,
    VolumeKmsKeyId: NotRequired[str],
```

1. See [:material-code-brackets: TransformInstanceTypeType](./literals.md#transforminstancetypetype) 
## TrialComponentArtifactTypeDef

```python
# TrialComponentArtifactTypeDef definition

class TrialComponentArtifactTypeDef(TypedDict):
    Value: str,
    MediaType: NotRequired[str],
```

## TrialComponentParameterValueTypeDef

```python
# TrialComponentParameterValueTypeDef definition

class TrialComponentParameterValueTypeDef(TypedDict):
    StringValue: NotRequired[str],
    NumberValue: NotRequired[float],
```

## TrialComponentStatusTypeDef

```python
# TrialComponentStatusTypeDef definition

class TrialComponentStatusTypeDef(TypedDict):
    PrimaryStatus: NotRequired[TrialComponentPrimaryStatusType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: TrialComponentPrimaryStatusType](./literals.md#trialcomponentprimarystatustype) 
## OidcConfigTypeDef

```python
# OidcConfigTypeDef definition

class OidcConfigTypeDef(TypedDict):
    ClientId: str,
    ClientSecret: str,
    Issuer: str,
    AuthorizationEndpoint: str,
    TokenEndpoint: str,
    UserInfoEndpoint: str,
    LogoutEndpoint: str,
    JwksUri: str,
```

## SourceIpConfigTypeDef

```python
# SourceIpConfigTypeDef definition

class SourceIpConfigTypeDef(TypedDict):
    Cidrs: Sequence[str],
```

## WorkforceVpcConfigRequestTypeDef

```python
# WorkforceVpcConfigRequestTypeDef definition

class WorkforceVpcConfigRequestTypeDef(TypedDict):
    VpcId: NotRequired[str],
    SecurityGroupIds: NotRequired[Sequence[str]],
    Subnets: NotRequired[Sequence[str]],
```

## NotificationConfigurationTypeDef

```python
# NotificationConfigurationTypeDef definition

class NotificationConfigurationTypeDef(TypedDict):
    NotificationTopicArn: NotRequired[str],
```

## CustomImageTypeDef

```python
# CustomImageTypeDef definition

class CustomImageTypeDef(TypedDict):
    ImageName: str,
    AppImageConfigName: str,
    ImageVersionNumber: NotRequired[int],
```

## CustomizedMetricSpecificationTypeDef

```python
# CustomizedMetricSpecificationTypeDef definition

class CustomizedMetricSpecificationTypeDef(TypedDict):
    MetricName: NotRequired[str],
    Namespace: NotRequired[str],
    Statistic: NotRequired[StatisticType],  # (1)
```

1. See [:material-code-brackets: StatisticType](./literals.md#statistictype) 
## DataCaptureConfigSummaryTypeDef

```python
# DataCaptureConfigSummaryTypeDef definition

class DataCaptureConfigSummaryTypeDef(TypedDict):
    EnableCapture: bool,
    CaptureStatus: CaptureStatusType,  # (1)
    CurrentSamplingPercentage: int,
    DestinationS3Uri: str,
    KmsKeyId: str,
```

1. See [:material-code-brackets: CaptureStatusType](./literals.md#capturestatustype) 
## DataCatalogConfigTypeDef

```python
# DataCatalogConfigTypeDef definition

class DataCatalogConfigTypeDef(TypedDict):
    TableName: str,
    Catalog: str,
    Database: str,
```

## MonitoringConstraintsResourceTypeDef

```python
# MonitoringConstraintsResourceTypeDef definition

class MonitoringConstraintsResourceTypeDef(TypedDict):
    S3Uri: NotRequired[str],
```

## MonitoringStatisticsResourceTypeDef

```python
# MonitoringStatisticsResourceTypeDef definition

class MonitoringStatisticsResourceTypeDef(TypedDict):
    S3Uri: NotRequired[str],
```

## EndpointInputTypeDef

```python
# EndpointInputTypeDef definition

class EndpointInputTypeDef(TypedDict):
    EndpointName: str,
    LocalPath: str,
    S3InputMode: NotRequired[ProcessingS3InputModeType],  # (1)
    S3DataDistributionType: NotRequired[ProcessingS3DataDistributionTypeType],  # (2)
    FeaturesAttribute: NotRequired[str],
    InferenceAttribute: NotRequired[str],
    ProbabilityAttribute: NotRequired[str],
    ProbabilityThresholdAttribute: NotRequired[float],
    StartTimeOffset: NotRequired[str],
    EndTimeOffset: NotRequired[str],
```

1. See [:material-code-brackets: ProcessingS3InputModeType](./literals.md#processings3inputmodetype) 
2. See [:material-code-brackets: ProcessingS3DataDistributionTypeType](./literals.md#processings3datadistributiontypetype) 
## FileSystemDataSourceTypeDef

```python
# FileSystemDataSourceTypeDef definition

class FileSystemDataSourceTypeDef(TypedDict):
    FileSystemId: str,
    FileSystemAccessMode: FileSystemAccessModeType,  # (1)
    FileSystemType: FileSystemTypeType,  # (2)
    DirectoryPath: str,
```

1. See [:material-code-brackets: FileSystemAccessModeType](./literals.md#filesystemaccessmodetype) 
2. See [:material-code-brackets: FileSystemTypeType](./literals.md#filesystemtypetype) 
## S3DataSourceTypeDef

```python
# S3DataSourceTypeDef definition

class S3DataSourceTypeDef(TypedDict):
    S3DataType: S3DataTypeType,  # (1)
    S3Uri: str,
    S3DataDistributionType: NotRequired[S3DataDistributionType],  # (2)
    AttributeNames: NotRequired[Sequence[str]],
    InstanceGroupNames: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: S3DataTypeType](./literals.md#s3datatypetype) 
2. See [:material-code-brackets: S3DataDistributionType](./literals.md#s3datadistributiontype) 
## RedshiftDatasetDefinitionTypeDef

```python
# RedshiftDatasetDefinitionTypeDef definition

class RedshiftDatasetDefinitionTypeDef(TypedDict):
    ClusterId: str,
    Database: str,
    DbUser: str,
    QueryString: str,
    ClusterRoleArn: str,
    OutputS3Uri: str,
    OutputFormat: RedshiftResultFormatType,  # (1)
    KmsKeyId: NotRequired[str],
    OutputCompression: NotRequired[RedshiftResultCompressionTypeType],  # (2)
```

1. See [:material-code-brackets: RedshiftResultFormatType](./literals.md#redshiftresultformattype) 
2. See [:material-code-brackets: RedshiftResultCompressionTypeType](./literals.md#redshiftresultcompressiontypetype) 
## DebugRuleEvaluationStatusTypeDef

```python
# DebugRuleEvaluationStatusTypeDef definition

class DebugRuleEvaluationStatusTypeDef(TypedDict):
    RuleConfigurationName: NotRequired[str],
    RuleEvaluationJobArn: NotRequired[str],
    RuleEvaluationStatus: NotRequired[RuleEvaluationStatusType],  # (1)
    StatusDetails: NotRequired[str],
    LastModifiedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: RuleEvaluationStatusType](./literals.md#ruleevaluationstatustype) 
## DeleteActionRequestRequestTypeDef

```python
# DeleteActionRequestRequestTypeDef definition

class DeleteActionRequestRequestTypeDef(TypedDict):
    ActionName: str,
```

## DeleteAlgorithmInputRequestTypeDef

```python
# DeleteAlgorithmInputRequestTypeDef definition

class DeleteAlgorithmInputRequestTypeDef(TypedDict):
    AlgorithmName: str,
```

## DeleteAppImageConfigRequestRequestTypeDef

```python
# DeleteAppImageConfigRequestRequestTypeDef definition

class DeleteAppImageConfigRequestRequestTypeDef(TypedDict):
    AppImageConfigName: str,
```

## DeleteAppRequestRequestTypeDef

```python
# DeleteAppRequestRequestTypeDef definition

class DeleteAppRequestRequestTypeDef(TypedDict):
    DomainId: str,
    AppType: AppTypeType,  # (1)
    AppName: str,
    UserProfileName: NotRequired[str],
    SpaceName: NotRequired[str],
```

1. See [:material-code-brackets: AppTypeType](./literals.md#apptypetype) 
## DeleteAssociationRequestRequestTypeDef

```python
# DeleteAssociationRequestRequestTypeDef definition

class DeleteAssociationRequestRequestTypeDef(TypedDict):
    SourceArn: str,
    DestinationArn: str,
```

## DeleteCodeRepositoryInputRequestTypeDef

```python
# DeleteCodeRepositoryInputRequestTypeDef definition

class DeleteCodeRepositoryInputRequestTypeDef(TypedDict):
    CodeRepositoryName: str,
```

## DeleteContextRequestRequestTypeDef

```python
# DeleteContextRequestRequestTypeDef definition

class DeleteContextRequestRequestTypeDef(TypedDict):
    ContextName: str,
```

## DeleteDataQualityJobDefinitionRequestRequestTypeDef

```python
# DeleteDataQualityJobDefinitionRequestRequestTypeDef definition

class DeleteDataQualityJobDefinitionRequestRequestTypeDef(TypedDict):
    JobDefinitionName: str,
```

## DeleteDeviceFleetRequestRequestTypeDef

```python
# DeleteDeviceFleetRequestRequestTypeDef definition

class DeleteDeviceFleetRequestRequestTypeDef(TypedDict):
    DeviceFleetName: str,
```

## RetentionPolicyTypeDef

```python
# RetentionPolicyTypeDef definition

class RetentionPolicyTypeDef(TypedDict):
    HomeEfsFileSystem: NotRequired[RetentionTypeType],  # (1)
```

1. See [:material-code-brackets: RetentionTypeType](./literals.md#retentiontypetype) 
## DeleteEdgeDeploymentPlanRequestRequestTypeDef

```python
# DeleteEdgeDeploymentPlanRequestRequestTypeDef definition

class DeleteEdgeDeploymentPlanRequestRequestTypeDef(TypedDict):
    EdgeDeploymentPlanName: str,
```

## DeleteEdgeDeploymentStageRequestRequestTypeDef

```python
# DeleteEdgeDeploymentStageRequestRequestTypeDef definition

class DeleteEdgeDeploymentStageRequestRequestTypeDef(TypedDict):
    EdgeDeploymentPlanName: str,
    StageName: str,
```

## DeleteEndpointConfigInputRequestTypeDef

```python
# DeleteEndpointConfigInputRequestTypeDef definition

class DeleteEndpointConfigInputRequestTypeDef(TypedDict):
    EndpointConfigName: str,
```

## DeleteEndpointInputRequestTypeDef

```python
# DeleteEndpointInputRequestTypeDef definition

class DeleteEndpointInputRequestTypeDef(TypedDict):
    EndpointName: str,
```

## DeleteExperimentRequestRequestTypeDef

```python
# DeleteExperimentRequestRequestTypeDef definition

class DeleteExperimentRequestRequestTypeDef(TypedDict):
    ExperimentName: str,
```

## DeleteFeatureGroupRequestRequestTypeDef

```python
# DeleteFeatureGroupRequestRequestTypeDef definition

class DeleteFeatureGroupRequestRequestTypeDef(TypedDict):
    FeatureGroupName: str,
```

## DeleteFlowDefinitionRequestRequestTypeDef

```python
# DeleteFlowDefinitionRequestRequestTypeDef definition

class DeleteFlowDefinitionRequestRequestTypeDef(TypedDict):
    FlowDefinitionName: str,
```

## DeleteHubContentRequestRequestTypeDef

```python
# DeleteHubContentRequestRequestTypeDef definition

class DeleteHubContentRequestRequestTypeDef(TypedDict):
    HubName: str,
    HubContentType: HubContentTypeType,  # (1)
    HubContentName: str,
    HubContentVersion: str,
```

1. See [:material-code-brackets: HubContentTypeType](./literals.md#hubcontenttypetype) 
## DeleteHubRequestRequestTypeDef

```python
# DeleteHubRequestRequestTypeDef definition

class DeleteHubRequestRequestTypeDef(TypedDict):
    HubName: str,
```

## DeleteHumanTaskUiRequestRequestTypeDef

```python
# DeleteHumanTaskUiRequestRequestTypeDef definition

class DeleteHumanTaskUiRequestRequestTypeDef(TypedDict):
    HumanTaskUiName: str,
```

## DeleteImageRequestRequestTypeDef

```python
# DeleteImageRequestRequestTypeDef definition

class DeleteImageRequestRequestTypeDef(TypedDict):
    ImageName: str,
```

## DeleteImageVersionRequestRequestTypeDef

```python
# DeleteImageVersionRequestRequestTypeDef definition

class DeleteImageVersionRequestRequestTypeDef(TypedDict):
    ImageName: str,
    Version: NotRequired[int],
    Alias: NotRequired[str],
```

## DeleteInferenceExperimentRequestRequestTypeDef

```python
# DeleteInferenceExperimentRequestRequestTypeDef definition

class DeleteInferenceExperimentRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteModelBiasJobDefinitionRequestRequestTypeDef

```python
# DeleteModelBiasJobDefinitionRequestRequestTypeDef definition

class DeleteModelBiasJobDefinitionRequestRequestTypeDef(TypedDict):
    JobDefinitionName: str,
```

## DeleteModelCardRequestRequestTypeDef

```python
# DeleteModelCardRequestRequestTypeDef definition

class DeleteModelCardRequestRequestTypeDef(TypedDict):
    ModelCardName: str,
```

## DeleteModelExplainabilityJobDefinitionRequestRequestTypeDef

```python
# DeleteModelExplainabilityJobDefinitionRequestRequestTypeDef definition

class DeleteModelExplainabilityJobDefinitionRequestRequestTypeDef(TypedDict):
    JobDefinitionName: str,
```

## DeleteModelInputRequestTypeDef

```python
# DeleteModelInputRequestTypeDef definition

class DeleteModelInputRequestTypeDef(TypedDict):
    ModelName: str,
```

## DeleteModelPackageGroupInputRequestTypeDef

```python
# DeleteModelPackageGroupInputRequestTypeDef definition

class DeleteModelPackageGroupInputRequestTypeDef(TypedDict):
    ModelPackageGroupName: str,
```

## DeleteModelPackageGroupPolicyInputRequestTypeDef

```python
# DeleteModelPackageGroupPolicyInputRequestTypeDef definition

class DeleteModelPackageGroupPolicyInputRequestTypeDef(TypedDict):
    ModelPackageGroupName: str,
```

## DeleteModelPackageInputRequestTypeDef

```python
# DeleteModelPackageInputRequestTypeDef definition

class DeleteModelPackageInputRequestTypeDef(TypedDict):
    ModelPackageName: str,
```

## DeleteModelQualityJobDefinitionRequestRequestTypeDef

```python
# DeleteModelQualityJobDefinitionRequestRequestTypeDef definition

class DeleteModelQualityJobDefinitionRequestRequestTypeDef(TypedDict):
    JobDefinitionName: str,
```

## DeleteMonitoringScheduleRequestRequestTypeDef

```python
# DeleteMonitoringScheduleRequestRequestTypeDef definition

class DeleteMonitoringScheduleRequestRequestTypeDef(TypedDict):
    MonitoringScheduleName: str,
```

## DeleteNotebookInstanceInputRequestTypeDef

```python
# DeleteNotebookInstanceInputRequestTypeDef definition

class DeleteNotebookInstanceInputRequestTypeDef(TypedDict):
    NotebookInstanceName: str,
```

## DeleteNotebookInstanceLifecycleConfigInputRequestTypeDef

```python
# DeleteNotebookInstanceLifecycleConfigInputRequestTypeDef definition

class DeleteNotebookInstanceLifecycleConfigInputRequestTypeDef(TypedDict):
    NotebookInstanceLifecycleConfigName: str,
```

## DeletePipelineRequestRequestTypeDef

```python
# DeletePipelineRequestRequestTypeDef definition

class DeletePipelineRequestRequestTypeDef(TypedDict):
    PipelineName: str,
    ClientRequestToken: str,
```

## DeleteProjectInputRequestTypeDef

```python
# DeleteProjectInputRequestTypeDef definition

class DeleteProjectInputRequestTypeDef(TypedDict):
    ProjectName: str,
```

## DeleteSpaceRequestRequestTypeDef

```python
# DeleteSpaceRequestRequestTypeDef definition

class DeleteSpaceRequestRequestTypeDef(TypedDict):
    DomainId: str,
    SpaceName: str,
```

## DeleteStudioLifecycleConfigRequestRequestTypeDef

```python
# DeleteStudioLifecycleConfigRequestRequestTypeDef definition

class DeleteStudioLifecycleConfigRequestRequestTypeDef(TypedDict):
    StudioLifecycleConfigName: str,
```

## DeleteTagsInputRequestTypeDef

```python
# DeleteTagsInputRequestTypeDef definition

class DeleteTagsInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## DeleteTrialComponentRequestRequestTypeDef

```python
# DeleteTrialComponentRequestRequestTypeDef definition

class DeleteTrialComponentRequestRequestTypeDef(TypedDict):
    TrialComponentName: str,
```

## DeleteTrialRequestRequestTypeDef

```python
# DeleteTrialRequestRequestTypeDef definition

class DeleteTrialRequestRequestTypeDef(TypedDict):
    TrialName: str,
```

## DeleteUserProfileRequestRequestTypeDef

```python
# DeleteUserProfileRequestRequestTypeDef definition

class DeleteUserProfileRequestRequestTypeDef(TypedDict):
    DomainId: str,
    UserProfileName: str,
```

## DeleteWorkforceRequestRequestTypeDef

```python
# DeleteWorkforceRequestRequestTypeDef definition

class DeleteWorkforceRequestRequestTypeDef(TypedDict):
    WorkforceName: str,
```

## DeleteWorkteamRequestRequestTypeDef

```python
# DeleteWorkteamRequestRequestTypeDef definition

class DeleteWorkteamRequestRequestTypeDef(TypedDict):
    WorkteamName: str,
```

## DeployedImageTypeDef

```python
# DeployedImageTypeDef definition

class DeployedImageTypeDef(TypedDict):
    SpecifiedImage: NotRequired[str],
    ResolvedImage: NotRequired[str],
    ResolutionTime: NotRequired[datetime],
```

## RealTimeInferenceRecommendationTypeDef

```python
# RealTimeInferenceRecommendationTypeDef definition

class RealTimeInferenceRecommendationTypeDef(TypedDict):
    RecommendationId: str,
    InstanceType: ProductionVariantInstanceTypeType,  # (1)
    Environment: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: ProductionVariantInstanceTypeType](./literals.md#productionvariantinstancetypetype) 
## DeviceSelectionConfigTypeDef

```python
# DeviceSelectionConfigTypeDef definition

class DeviceSelectionConfigTypeDef(TypedDict):
    DeviceSubsetType: DeviceSubsetTypeType,  # (1)
    Percentage: NotRequired[int],
    DeviceNames: NotRequired[Sequence[str]],
    DeviceNameContains: NotRequired[str],
```

1. See [:material-code-brackets: DeviceSubsetTypeType](./literals.md#devicesubsettypetype) 
## EdgeDeploymentConfigTypeDef

```python
# EdgeDeploymentConfigTypeDef definition

class EdgeDeploymentConfigTypeDef(TypedDict):
    FailureHandlingPolicy: FailureHandlingPolicyType,  # (1)
```

1. See [:material-code-brackets: FailureHandlingPolicyType](./literals.md#failurehandlingpolicytype) 
## EdgeDeploymentStatusTypeDef

```python
# EdgeDeploymentStatusTypeDef definition

class EdgeDeploymentStatusTypeDef(TypedDict):
    StageStatus: StageStatusType,  # (1)
    EdgeDeploymentSuccessInStage: int,
    EdgeDeploymentPendingInStage: int,
    EdgeDeploymentFailedInStage: int,
    EdgeDeploymentStatusMessage: NotRequired[str],
    EdgeDeploymentStageStartTime: NotRequired[datetime],
```

1. See [:material-code-brackets: StageStatusType](./literals.md#stagestatustype) 
## DeregisterDevicesRequestRequestTypeDef

```python
# DeregisterDevicesRequestRequestTypeDef definition

class DeregisterDevicesRequestRequestTypeDef(TypedDict):
    DeviceFleetName: str,
    DeviceNames: Sequence[str],
```

## DescribeActionRequestRequestTypeDef

```python
# DescribeActionRequestRequestTypeDef definition

class DescribeActionRequestRequestTypeDef(TypedDict):
    ActionName: str,
```

## DescribeAlgorithmInputRequestTypeDef

```python
# DescribeAlgorithmInputRequestTypeDef definition

class DescribeAlgorithmInputRequestTypeDef(TypedDict):
    AlgorithmName: str,
```

## DescribeAppImageConfigRequestRequestTypeDef

```python
# DescribeAppImageConfigRequestRequestTypeDef definition

class DescribeAppImageConfigRequestRequestTypeDef(TypedDict):
    AppImageConfigName: str,
```

## DescribeAppRequestRequestTypeDef

```python
# DescribeAppRequestRequestTypeDef definition

class DescribeAppRequestRequestTypeDef(TypedDict):
    DomainId: str,
    AppType: AppTypeType,  # (1)
    AppName: str,
    UserProfileName: NotRequired[str],
    SpaceName: NotRequired[str],
```

1. See [:material-code-brackets: AppTypeType](./literals.md#apptypetype) 
## DescribeArtifactRequestRequestTypeDef

```python
# DescribeArtifactRequestRequestTypeDef definition

class DescribeArtifactRequestRequestTypeDef(TypedDict):
    ArtifactArn: str,
```

## DescribeAutoMLJobRequestRequestTypeDef

```python
# DescribeAutoMLJobRequestRequestTypeDef definition

class DescribeAutoMLJobRequestRequestTypeDef(TypedDict):
    AutoMLJobName: str,
```

## ModelDeployResultTypeDef

```python
# ModelDeployResultTypeDef definition

class ModelDeployResultTypeDef(TypedDict):
    EndpointName: NotRequired[str],
```

## DescribeAutoMLJobV2RequestRequestTypeDef

```python
# DescribeAutoMLJobV2RequestRequestTypeDef definition

class DescribeAutoMLJobV2RequestRequestTypeDef(TypedDict):
    AutoMLJobName: str,
```

## DescribeCodeRepositoryInputRequestTypeDef

```python
# DescribeCodeRepositoryInputRequestTypeDef definition

class DescribeCodeRepositoryInputRequestTypeDef(TypedDict):
    CodeRepositoryName: str,
```

## DescribeCompilationJobRequestRequestTypeDef

```python
# DescribeCompilationJobRequestRequestTypeDef definition

class DescribeCompilationJobRequestRequestTypeDef(TypedDict):
    CompilationJobName: str,
```

## ModelArtifactsTypeDef

```python
# ModelArtifactsTypeDef definition

class ModelArtifactsTypeDef(TypedDict):
    S3ModelArtifacts: str,
```

## ModelDigestsTypeDef

```python
# ModelDigestsTypeDef definition

class ModelDigestsTypeDef(TypedDict):
    ArtifactDigest: NotRequired[str],
```

## DescribeContextRequestRequestTypeDef

```python
# DescribeContextRequestRequestTypeDef definition

class DescribeContextRequestRequestTypeDef(TypedDict):
    ContextName: str,
```

## DescribeDataQualityJobDefinitionRequestRequestTypeDef

```python
# DescribeDataQualityJobDefinitionRequestRequestTypeDef definition

class DescribeDataQualityJobDefinitionRequestRequestTypeDef(TypedDict):
    JobDefinitionName: str,
```

## DescribeDeviceFleetRequestRequestTypeDef

```python
# DescribeDeviceFleetRequestRequestTypeDef definition

class DescribeDeviceFleetRequestRequestTypeDef(TypedDict):
    DeviceFleetName: str,
```

## DescribeDeviceRequestRequestTypeDef

```python
# DescribeDeviceRequestRequestTypeDef definition

class DescribeDeviceRequestRequestTypeDef(TypedDict):
    DeviceName: str,
    DeviceFleetName: str,
    NextToken: NotRequired[str],
```

## EdgeModelTypeDef

```python
# EdgeModelTypeDef definition

class EdgeModelTypeDef(TypedDict):
    ModelName: str,
    ModelVersion: str,
    LatestSampleTime: NotRequired[datetime],
    LatestInference: NotRequired[datetime],
```

## DescribeDomainRequestRequestTypeDef

```python
# DescribeDomainRequestRequestTypeDef definition

class DescribeDomainRequestRequestTypeDef(TypedDict):
    DomainId: str,
```

## DescribeEdgeDeploymentPlanRequestRequestTypeDef

```python
# DescribeEdgeDeploymentPlanRequestRequestTypeDef definition

class DescribeEdgeDeploymentPlanRequestRequestTypeDef(TypedDict):
    EdgeDeploymentPlanName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## DescribeEdgePackagingJobRequestRequestTypeDef

```python
# DescribeEdgePackagingJobRequestRequestTypeDef definition

class DescribeEdgePackagingJobRequestRequestTypeDef(TypedDict):
    EdgePackagingJobName: str,
```

## EdgePresetDeploymentOutputTypeDef

```python
# EdgePresetDeploymentOutputTypeDef definition

class EdgePresetDeploymentOutputTypeDef(TypedDict):
    Type: EdgePresetDeploymentTypeType,  # (1)
    Artifact: NotRequired[str],
    Status: NotRequired[EdgePresetDeploymentStatusType],  # (2)
    StatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: EdgePresetDeploymentTypeType](./literals.md#edgepresetdeploymenttypetype) 
2. See [:material-code-brackets: EdgePresetDeploymentStatusType](./literals.md#edgepresetdeploymentstatustype) 
## DescribeEndpointConfigInputRequestTypeDef

```python
# DescribeEndpointConfigInputRequestTypeDef definition

class DescribeEndpointConfigInputRequestTypeDef(TypedDict):
    EndpointConfigName: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## DescribeEndpointInputRequestTypeDef

```python
# DescribeEndpointInputRequestTypeDef definition

class DescribeEndpointInputRequestTypeDef(TypedDict):
    EndpointName: str,
```

## DescribeExperimentRequestRequestTypeDef

```python
# DescribeExperimentRequestRequestTypeDef definition

class DescribeExperimentRequestRequestTypeDef(TypedDict):
    ExperimentName: str,
```

## ExperimentSourceTypeDef

```python
# ExperimentSourceTypeDef definition

class ExperimentSourceTypeDef(TypedDict):
    SourceArn: str,
    SourceType: NotRequired[str],
```

## DescribeFeatureGroupRequestRequestTypeDef

```python
# DescribeFeatureGroupRequestRequestTypeDef definition

class DescribeFeatureGroupRequestRequestTypeDef(TypedDict):
    FeatureGroupName: str,
    NextToken: NotRequired[str],
```

## LastUpdateStatusTypeDef

```python
# LastUpdateStatusTypeDef definition

class LastUpdateStatusTypeDef(TypedDict):
    Status: LastUpdateStatusValueType,  # (1)
    FailureReason: NotRequired[str],
```

1. See [:material-code-brackets: LastUpdateStatusValueType](./literals.md#lastupdatestatusvaluetype) 
## OfflineStoreStatusTypeDef

```python
# OfflineStoreStatusTypeDef definition

class OfflineStoreStatusTypeDef(TypedDict):
    Status: OfflineStoreStatusValueType,  # (1)
    BlockedReason: NotRequired[str],
```

1. See [:material-code-brackets: OfflineStoreStatusValueType](./literals.md#offlinestorestatusvaluetype) 
## DescribeFeatureMetadataRequestRequestTypeDef

```python
# DescribeFeatureMetadataRequestRequestTypeDef definition

class DescribeFeatureMetadataRequestRequestTypeDef(TypedDict):
    FeatureGroupName: str,
    FeatureName: str,
```

## FeatureParameterTypeDef

```python
# FeatureParameterTypeDef definition

class FeatureParameterTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## DescribeFlowDefinitionRequestRequestTypeDef

```python
# DescribeFlowDefinitionRequestRequestTypeDef definition

class DescribeFlowDefinitionRequestRequestTypeDef(TypedDict):
    FlowDefinitionName: str,
```

## DescribeHubContentRequestRequestTypeDef

```python
# DescribeHubContentRequestRequestTypeDef definition

class DescribeHubContentRequestRequestTypeDef(TypedDict):
    HubName: str,
    HubContentType: HubContentTypeType,  # (1)
    HubContentName: str,
    HubContentVersion: NotRequired[str],
```

1. See [:material-code-brackets: HubContentTypeType](./literals.md#hubcontenttypetype) 
## HubContentDependencyTypeDef

```python
# HubContentDependencyTypeDef definition

class HubContentDependencyTypeDef(TypedDict):
    DependencyOriginPath: NotRequired[str],
    DependencyCopyPath: NotRequired[str],
```

## DescribeHubRequestRequestTypeDef

```python
# DescribeHubRequestRequestTypeDef definition

class DescribeHubRequestRequestTypeDef(TypedDict):
    HubName: str,
```

## DescribeHumanTaskUiRequestRequestTypeDef

```python
# DescribeHumanTaskUiRequestRequestTypeDef definition

class DescribeHumanTaskUiRequestRequestTypeDef(TypedDict):
    HumanTaskUiName: str,
```

## UiTemplateInfoTypeDef

```python
# UiTemplateInfoTypeDef definition

class UiTemplateInfoTypeDef(TypedDict):
    Url: NotRequired[str],
    ContentSha256: NotRequired[str],
```

## DescribeHyperParameterTuningJobRequestRequestTypeDef

```python
# DescribeHyperParameterTuningJobRequestRequestTypeDef definition

class DescribeHyperParameterTuningJobRequestRequestTypeDef(TypedDict):
    HyperParameterTuningJobName: str,
```

## HyperParameterTuningJobCompletionDetailsTypeDef

```python
# HyperParameterTuningJobCompletionDetailsTypeDef definition

class HyperParameterTuningJobCompletionDetailsTypeDef(TypedDict):
    NumberOfTrainingJobsObjectiveNotImproving: NotRequired[int],
    ConvergenceDetectedTime: NotRequired[datetime],
```

## HyperParameterTuningJobConsumedResourcesTypeDef

```python
# HyperParameterTuningJobConsumedResourcesTypeDef definition

class HyperParameterTuningJobConsumedResourcesTypeDef(TypedDict):
    RuntimeInSeconds: NotRequired[int],
```

## ObjectiveStatusCountersTypeDef

```python
# ObjectiveStatusCountersTypeDef definition

class ObjectiveStatusCountersTypeDef(TypedDict):
    Succeeded: NotRequired[int],
    Pending: NotRequired[int],
    Failed: NotRequired[int],
```

## TrainingJobStatusCountersTypeDef

```python
# TrainingJobStatusCountersTypeDef definition

class TrainingJobStatusCountersTypeDef(TypedDict):
    Completed: NotRequired[int],
    InProgress: NotRequired[int],
    RetryableError: NotRequired[int],
    NonRetryableError: NotRequired[int],
    Stopped: NotRequired[int],
```

## DescribeImageRequestRequestTypeDef

```python
# DescribeImageRequestRequestTypeDef definition

class DescribeImageRequestRequestTypeDef(TypedDict):
    ImageName: str,
```

## DescribeImageVersionRequestRequestTypeDef

```python
# DescribeImageVersionRequestRequestTypeDef definition

class DescribeImageVersionRequestRequestTypeDef(TypedDict):
    ImageName: str,
    Version: NotRequired[int],
    Alias: NotRequired[str],
```

## DescribeInferenceExperimentRequestRequestTypeDef

```python
# DescribeInferenceExperimentRequestRequestTypeDef definition

class DescribeInferenceExperimentRequestRequestTypeDef(TypedDict):
    Name: str,
```

## EndpointMetadataTypeDef

```python
# EndpointMetadataTypeDef definition

class EndpointMetadataTypeDef(TypedDict):
    EndpointName: str,
    EndpointConfigName: NotRequired[str],
    EndpointStatus: NotRequired[EndpointStatusType],  # (1)
    FailureReason: NotRequired[str],
```

1. See [:material-code-brackets: EndpointStatusType](./literals.md#endpointstatustype) 
## DescribeInferenceRecommendationsJobRequestRequestTypeDef

```python
# DescribeInferenceRecommendationsJobRequestRequestTypeDef definition

class DescribeInferenceRecommendationsJobRequestRequestTypeDef(TypedDict):
    JobName: str,
```

## DescribeLabelingJobRequestRequestTypeDef

```python
# DescribeLabelingJobRequestRequestTypeDef definition

class DescribeLabelingJobRequestRequestTypeDef(TypedDict):
    LabelingJobName: str,
```

## LabelCountersTypeDef

```python
# LabelCountersTypeDef definition

class LabelCountersTypeDef(TypedDict):
    TotalLabeled: NotRequired[int],
    HumanLabeled: NotRequired[int],
    MachineLabeled: NotRequired[int],
    FailedNonRetryableError: NotRequired[int],
    Unlabeled: NotRequired[int],
```

## LabelingJobOutputTypeDef

```python
# LabelingJobOutputTypeDef definition

class LabelingJobOutputTypeDef(TypedDict):
    OutputDatasetS3Uri: str,
    FinalActiveLearningModelArn: NotRequired[str],
```

## DescribeLineageGroupRequestRequestTypeDef

```python
# DescribeLineageGroupRequestRequestTypeDef definition

class DescribeLineageGroupRequestRequestTypeDef(TypedDict):
    LineageGroupName: str,
```

## DescribeModelBiasJobDefinitionRequestRequestTypeDef

```python
# DescribeModelBiasJobDefinitionRequestRequestTypeDef definition

class DescribeModelBiasJobDefinitionRequestRequestTypeDef(TypedDict):
    JobDefinitionName: str,
```

## DescribeModelCardExportJobRequestRequestTypeDef

```python
# DescribeModelCardExportJobRequestRequestTypeDef definition

class DescribeModelCardExportJobRequestRequestTypeDef(TypedDict):
    ModelCardExportJobArn: str,
```

## ModelCardExportArtifactsTypeDef

```python
# ModelCardExportArtifactsTypeDef definition

class ModelCardExportArtifactsTypeDef(TypedDict):
    S3ExportArtifacts: str,
```

## DescribeModelCardRequestRequestTypeDef

```python
# DescribeModelCardRequestRequestTypeDef definition

class DescribeModelCardRequestRequestTypeDef(TypedDict):
    ModelCardName: str,
    ModelCardVersion: NotRequired[int],
```

## DescribeModelExplainabilityJobDefinitionRequestRequestTypeDef

```python
# DescribeModelExplainabilityJobDefinitionRequestRequestTypeDef definition

class DescribeModelExplainabilityJobDefinitionRequestRequestTypeDef(TypedDict):
    JobDefinitionName: str,
```

## DescribeModelInputRequestTypeDef

```python
# DescribeModelInputRequestTypeDef definition

class DescribeModelInputRequestTypeDef(TypedDict):
    ModelName: str,
```

## DescribeModelPackageGroupInputRequestTypeDef

```python
# DescribeModelPackageGroupInputRequestTypeDef definition

class DescribeModelPackageGroupInputRequestTypeDef(TypedDict):
    ModelPackageGroupName: str,
```

## DescribeModelPackageInputRequestTypeDef

```python
# DescribeModelPackageInputRequestTypeDef definition

class DescribeModelPackageInputRequestTypeDef(TypedDict):
    ModelPackageName: str,
```

## DescribeModelQualityJobDefinitionRequestRequestTypeDef

```python
# DescribeModelQualityJobDefinitionRequestRequestTypeDef definition

class DescribeModelQualityJobDefinitionRequestRequestTypeDef(TypedDict):
    JobDefinitionName: str,
```

## DescribeMonitoringScheduleRequestRequestTypeDef

```python
# DescribeMonitoringScheduleRequestRequestTypeDef definition

class DescribeMonitoringScheduleRequestRequestTypeDef(TypedDict):
    MonitoringScheduleName: str,
```

## MonitoringExecutionSummaryTypeDef

```python
# MonitoringExecutionSummaryTypeDef definition

class MonitoringExecutionSummaryTypeDef(TypedDict):
    MonitoringScheduleName: str,
    ScheduledTime: datetime,
    CreationTime: datetime,
    LastModifiedTime: datetime,
    MonitoringExecutionStatus: ExecutionStatusType,  # (1)
    ProcessingJobArn: NotRequired[str],
    EndpointName: NotRequired[str],
    FailureReason: NotRequired[str],
    MonitoringJobDefinitionName: NotRequired[str],
    MonitoringType: NotRequired[MonitoringTypeType],  # (2)
```

1. See [:material-code-brackets: ExecutionStatusType](./literals.md#executionstatustype) 
2. See [:material-code-brackets: MonitoringTypeType](./literals.md#monitoringtypetype) 
## DescribeNotebookInstanceInputRequestTypeDef

```python
# DescribeNotebookInstanceInputRequestTypeDef definition

class DescribeNotebookInstanceInputRequestTypeDef(TypedDict):
    NotebookInstanceName: str,
```

## DescribeNotebookInstanceLifecycleConfigInputRequestTypeDef

```python
# DescribeNotebookInstanceLifecycleConfigInputRequestTypeDef definition

class DescribeNotebookInstanceLifecycleConfigInputRequestTypeDef(TypedDict):
    NotebookInstanceLifecycleConfigName: str,
```

## DescribePipelineDefinitionForExecutionRequestRequestTypeDef

```python
# DescribePipelineDefinitionForExecutionRequestRequestTypeDef definition

class DescribePipelineDefinitionForExecutionRequestRequestTypeDef(TypedDict):
    PipelineExecutionArn: str,
```

## DescribePipelineExecutionRequestRequestTypeDef

```python
# DescribePipelineExecutionRequestRequestTypeDef definition

class DescribePipelineExecutionRequestRequestTypeDef(TypedDict):
    PipelineExecutionArn: str,
```

## PipelineExperimentConfigTypeDef

```python
# PipelineExperimentConfigTypeDef definition

class PipelineExperimentConfigTypeDef(TypedDict):
    ExperimentName: NotRequired[str],
    TrialName: NotRequired[str],
```

## DescribePipelineRequestRequestTypeDef

```python
# DescribePipelineRequestRequestTypeDef definition

class DescribePipelineRequestRequestTypeDef(TypedDict):
    PipelineName: str,
```

## DescribeProcessingJobRequestRequestTypeDef

```python
# DescribeProcessingJobRequestRequestTypeDef definition

class DescribeProcessingJobRequestRequestTypeDef(TypedDict):
    ProcessingJobName: str,
```

## DescribeProjectInputRequestTypeDef

```python
# DescribeProjectInputRequestTypeDef definition

class DescribeProjectInputRequestTypeDef(TypedDict):
    ProjectName: str,
```

## ServiceCatalogProvisionedProductDetailsTypeDef

```python
# ServiceCatalogProvisionedProductDetailsTypeDef definition

class ServiceCatalogProvisionedProductDetailsTypeDef(TypedDict):
    ProvisionedProductId: NotRequired[str],
    ProvisionedProductStatusMessage: NotRequired[str],
```

## DescribeSpaceRequestRequestTypeDef

```python
# DescribeSpaceRequestRequestTypeDef definition

class DescribeSpaceRequestRequestTypeDef(TypedDict):
    DomainId: str,
    SpaceName: str,
```

## DescribeStudioLifecycleConfigRequestRequestTypeDef

```python
# DescribeStudioLifecycleConfigRequestRequestTypeDef definition

class DescribeStudioLifecycleConfigRequestRequestTypeDef(TypedDict):
    StudioLifecycleConfigName: str,
```

## DescribeSubscribedWorkteamRequestRequestTypeDef

```python
# DescribeSubscribedWorkteamRequestRequestTypeDef definition

class DescribeSubscribedWorkteamRequestRequestTypeDef(TypedDict):
    WorkteamArn: str,
```

## SubscribedWorkteamTypeDef

```python
# SubscribedWorkteamTypeDef definition

class SubscribedWorkteamTypeDef(TypedDict):
    WorkteamArn: str,
    MarketplaceTitle: NotRequired[str],
    SellerName: NotRequired[str],
    MarketplaceDescription: NotRequired[str],
    ListingId: NotRequired[str],
```

## DescribeTrainingJobRequestRequestTypeDef

```python
# DescribeTrainingJobRequestRequestTypeDef definition

class DescribeTrainingJobRequestRequestTypeDef(TypedDict):
    TrainingJobName: str,
```

## MetricDataTypeDef

```python
# MetricDataTypeDef definition

class MetricDataTypeDef(TypedDict):
    MetricName: NotRequired[str],
    Value: NotRequired[float],
    Timestamp: NotRequired[datetime],
```

## ProfilerRuleEvaluationStatusTypeDef

```python
# ProfilerRuleEvaluationStatusTypeDef definition

class ProfilerRuleEvaluationStatusTypeDef(TypedDict):
    RuleConfigurationName: NotRequired[str],
    RuleEvaluationJobArn: NotRequired[str],
    RuleEvaluationStatus: NotRequired[RuleEvaluationStatusType],  # (1)
    StatusDetails: NotRequired[str],
    LastModifiedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: RuleEvaluationStatusType](./literals.md#ruleevaluationstatustype) 
## SecondaryStatusTransitionTypeDef

```python
# SecondaryStatusTransitionTypeDef definition

class SecondaryStatusTransitionTypeDef(TypedDict):
    Status: SecondaryStatusType,  # (1)
    StartTime: datetime,
    EndTime: NotRequired[datetime],
    StatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: SecondaryStatusType](./literals.md#secondarystatustype) 
## WarmPoolStatusTypeDef

```python
# WarmPoolStatusTypeDef definition

class WarmPoolStatusTypeDef(TypedDict):
    Status: WarmPoolResourceStatusType,  # (1)
    ResourceRetainedBillableTimeInSeconds: NotRequired[int],
    ReusedByJob: NotRequired[str],
```

1. See [:material-code-brackets: WarmPoolResourceStatusType](./literals.md#warmpoolresourcestatustype) 
## DescribeTransformJobRequestRequestTypeDef

```python
# DescribeTransformJobRequestRequestTypeDef definition

class DescribeTransformJobRequestRequestTypeDef(TypedDict):
    TransformJobName: str,
```

## DescribeTrialComponentRequestRequestTypeDef

```python
# DescribeTrialComponentRequestRequestTypeDef definition

class DescribeTrialComponentRequestRequestTypeDef(TypedDict):
    TrialComponentName: str,
```

## TrialComponentMetricSummaryTypeDef

```python
# TrialComponentMetricSummaryTypeDef definition

class TrialComponentMetricSummaryTypeDef(TypedDict):
    MetricName: NotRequired[str],
    SourceArn: NotRequired[str],
    TimeStamp: NotRequired[datetime],
    Max: NotRequired[float],
    Min: NotRequired[float],
    Last: NotRequired[float],
    Count: NotRequired[int],
    Avg: NotRequired[float],
    StdDev: NotRequired[float],
```

## TrialComponentSourceTypeDef

```python
# TrialComponentSourceTypeDef definition

class TrialComponentSourceTypeDef(TypedDict):
    SourceArn: str,
    SourceType: NotRequired[str],
```

## DescribeTrialRequestRequestTypeDef

```python
# DescribeTrialRequestRequestTypeDef definition

class DescribeTrialRequestRequestTypeDef(TypedDict):
    TrialName: str,
```

## TrialSourceTypeDef

```python
# TrialSourceTypeDef definition

class TrialSourceTypeDef(TypedDict):
    SourceArn: str,
    SourceType: NotRequired[str],
```

## DescribeUserProfileRequestRequestTypeDef

```python
# DescribeUserProfileRequestRequestTypeDef definition

class DescribeUserProfileRequestRequestTypeDef(TypedDict):
    DomainId: str,
    UserProfileName: str,
```

## DescribeWorkforceRequestRequestTypeDef

```python
# DescribeWorkforceRequestRequestTypeDef definition

class DescribeWorkforceRequestRequestTypeDef(TypedDict):
    WorkforceName: str,
```

## DescribeWorkteamRequestRequestTypeDef

```python
# DescribeWorkteamRequestRequestTypeDef definition

class DescribeWorkteamRequestRequestTypeDef(TypedDict):
    WorkteamName: str,
```

## ProductionVariantServerlessUpdateConfigTypeDef

```python
# ProductionVariantServerlessUpdateConfigTypeDef definition

class ProductionVariantServerlessUpdateConfigTypeDef(TypedDict):
    MaxConcurrency: NotRequired[int],
    ProvisionedConcurrency: NotRequired[int],
```

## DeviceDeploymentSummaryTypeDef

```python
# DeviceDeploymentSummaryTypeDef definition

class DeviceDeploymentSummaryTypeDef(TypedDict):
    EdgeDeploymentPlanArn: str,
    EdgeDeploymentPlanName: str,
    StageName: str,
    DeviceName: str,
    DeviceArn: str,
    DeployedStageName: NotRequired[str],
    DeviceFleetName: NotRequired[str],
    DeviceDeploymentStatus: NotRequired[DeviceDeploymentStatusType],  # (1)
    DeviceDeploymentStatusMessage: NotRequired[str],
    Description: NotRequired[str],
    DeploymentStartTime: NotRequired[datetime],
```

1. See [:material-code-brackets: DeviceDeploymentStatusType](./literals.md#devicedeploymentstatustype) 
## DeviceFleetSummaryTypeDef

```python
# DeviceFleetSummaryTypeDef definition

class DeviceFleetSummaryTypeDef(TypedDict):
    DeviceFleetArn: str,
    DeviceFleetName: str,
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
```

## DeviceStatsTypeDef

```python
# DeviceStatsTypeDef definition

class DeviceStatsTypeDef(TypedDict):
    ConnectedDeviceCount: int,
    RegisteredDeviceCount: int,
```

## EdgeModelSummaryTypeDef

```python
# EdgeModelSummaryTypeDef definition

class EdgeModelSummaryTypeDef(TypedDict):
    ModelName: str,
    ModelVersion: str,
```

## DeviceTypeDef

```python
# DeviceTypeDef definition

class DeviceTypeDef(TypedDict):
    DeviceName: str,
    Description: NotRequired[str],
    IotThingName: NotRequired[str],
```

## DisassociateTrialComponentRequestRequestTypeDef

```python
# DisassociateTrialComponentRequestRequestTypeDef definition

class DisassociateTrialComponentRequestRequestTypeDef(TypedDict):
    TrialComponentName: str,
    TrialName: str,
```

## DomainDetailsTypeDef

```python
# DomainDetailsTypeDef definition

class DomainDetailsTypeDef(TypedDict):
    DomainArn: NotRequired[str],
    DomainId: NotRequired[str],
    DomainName: NotRequired[str],
    Status: NotRequired[DomainStatusType],  # (1)
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
    Url: NotRequired[str],
```

1. See [:material-code-brackets: DomainStatusType](./literals.md#domainstatustype) 
## FileSourceTypeDef

```python
# FileSourceTypeDef definition

class FileSourceTypeDef(TypedDict):
    S3Uri: str,
    ContentType: NotRequired[str],
    ContentDigest: NotRequired[str],
```

## EMRStepMetadataTypeDef

```python
# EMRStepMetadataTypeDef definition

class EMRStepMetadataTypeDef(TypedDict):
    ClusterId: NotRequired[str],
    StepId: NotRequired[str],
    StepName: NotRequired[str],
    LogFilePath: NotRequired[str],
```

## EdgeDeploymentPlanSummaryTypeDef

```python
# EdgeDeploymentPlanSummaryTypeDef definition

class EdgeDeploymentPlanSummaryTypeDef(TypedDict):
    EdgeDeploymentPlanArn: str,
    EdgeDeploymentPlanName: str,
    DeviceFleetName: str,
    EdgeDeploymentSuccess: int,
    EdgeDeploymentPending: int,
    EdgeDeploymentFailed: int,
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
```

## EdgeModelStatTypeDef

```python
# EdgeModelStatTypeDef definition

class EdgeModelStatTypeDef(TypedDict):
    ModelName: str,
    ModelVersion: str,
    OfflineDeviceCount: int,
    ConnectedDeviceCount: int,
    ActiveDeviceCount: int,
    SamplingDeviceCount: int,
```

## EdgePackagingJobSummaryTypeDef

```python
# EdgePackagingJobSummaryTypeDef definition

class EdgePackagingJobSummaryTypeDef(TypedDict):
    EdgePackagingJobArn: str,
    EdgePackagingJobName: str,
    EdgePackagingJobStatus: EdgePackagingJobStatusType,  # (1)
    CompilationJobName: NotRequired[str],
    ModelName: NotRequired[str],
    ModelVersion: NotRequired[str],
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: EdgePackagingJobStatusType](./literals.md#edgepackagingjobstatustype) 
## EdgeTypeDef

```python
# EdgeTypeDef definition

class EdgeTypeDef(TypedDict):
    SourceArn: NotRequired[str],
    DestinationArn: NotRequired[str],
    AssociationType: NotRequired[AssociationEdgeTypeType],  # (1)
```

1. See [:material-code-brackets: AssociationEdgeTypeType](./literals.md#associationedgetypetype) 
## EndpointConfigSummaryTypeDef

```python
# EndpointConfigSummaryTypeDef definition

class EndpointConfigSummaryTypeDef(TypedDict):
    EndpointConfigName: str,
    EndpointConfigArn: str,
    CreationTime: datetime,
```

## EndpointInfoTypeDef

```python
# EndpointInfoTypeDef definition

class EndpointInfoTypeDef(TypedDict):
    EndpointName: str,
```

## ProductionVariantServerlessConfigTypeDef

```python
# ProductionVariantServerlessConfigTypeDef definition

class ProductionVariantServerlessConfigTypeDef(TypedDict):
    MemorySizeInMB: int,
    MaxConcurrency: int,
    ProvisionedConcurrency: NotRequired[int],
```

## InferenceMetricsTypeDef

```python
# InferenceMetricsTypeDef definition

class InferenceMetricsTypeDef(TypedDict):
    MaxInvocations: int,
    ModelLatency: int,
```

## EndpointSummaryTypeDef

```python
# EndpointSummaryTypeDef definition

class EndpointSummaryTypeDef(TypedDict):
    EndpointName: str,
    EndpointArn: str,
    CreationTime: datetime,
    LastModifiedTime: datetime,
    EndpointStatus: EndpointStatusType,  # (1)
```

1. See [:material-code-brackets: EndpointStatusType](./literals.md#endpointstatustype) 
## EnvironmentParameterTypeDef

```python
# EnvironmentParameterTypeDef definition

class EnvironmentParameterTypeDef(TypedDict):
    Key: str,
    ValueType: str,
    Value: str,
```

## FailStepMetadataTypeDef

```python
# FailStepMetadataTypeDef definition

class FailStepMetadataTypeDef(TypedDict):
    ErrorMessage: NotRequired[str],
```

## FileSystemConfigTypeDef

```python
# FileSystemConfigTypeDef definition

class FileSystemConfigTypeDef(TypedDict):
    MountPath: NotRequired[str],
    DefaultUid: NotRequired[int],
    DefaultGid: NotRequired[int],
```

## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Name: str,
    Operator: NotRequired[OperatorType],  # (1)
    Value: NotRequired[str],
```

1. See [:material-code-brackets: OperatorType](./literals.md#operatortype) 
## FinalHyperParameterTuningJobObjectiveMetricTypeDef

```python
# FinalHyperParameterTuningJobObjectiveMetricTypeDef definition

class FinalHyperParameterTuningJobObjectiveMetricTypeDef(TypedDict):
    MetricName: str,
    Value: float,
    Type: NotRequired[HyperParameterTuningJobObjectiveTypeType],  # (1)
```

1. See [:material-code-brackets: HyperParameterTuningJobObjectiveTypeType](./literals.md#hyperparametertuningjobobjectivetypetype) 
## FlowDefinitionSummaryTypeDef

```python
# FlowDefinitionSummaryTypeDef definition

class FlowDefinitionSummaryTypeDef(TypedDict):
    FlowDefinitionName: str,
    FlowDefinitionArn: str,
    FlowDefinitionStatus: FlowDefinitionStatusType,  # (1)
    CreationTime: datetime,
    FailureReason: NotRequired[str],
```

1. See [:material-code-brackets: FlowDefinitionStatusType](./literals.md#flowdefinitionstatustype) 
## GetDeviceFleetReportRequestRequestTypeDef

```python
# GetDeviceFleetReportRequestRequestTypeDef definition

class GetDeviceFleetReportRequestRequestTypeDef(TypedDict):
    DeviceFleetName: str,
```

## GetLineageGroupPolicyRequestRequestTypeDef

```python
# GetLineageGroupPolicyRequestRequestTypeDef definition

class GetLineageGroupPolicyRequestRequestTypeDef(TypedDict):
    LineageGroupName: str,
```

## GetModelPackageGroupPolicyInputRequestTypeDef

```python
# GetModelPackageGroupPolicyInputRequestTypeDef definition

class GetModelPackageGroupPolicyInputRequestTypeDef(TypedDict):
    ModelPackageGroupName: str,
```

## ScalingPolicyObjectiveTypeDef

```python
# ScalingPolicyObjectiveTypeDef definition

class ScalingPolicyObjectiveTypeDef(TypedDict):
    MinInvocationsPerMinute: NotRequired[int],
    MaxInvocationsPerMinute: NotRequired[int],
```

## ScalingPolicyMetricTypeDef

```python
# ScalingPolicyMetricTypeDef definition

class ScalingPolicyMetricTypeDef(TypedDict):
    InvocationsPerInstance: NotRequired[int],
    ModelLatency: NotRequired[int],
```

## PropertyNameSuggestionTypeDef

```python
# PropertyNameSuggestionTypeDef definition

class PropertyNameSuggestionTypeDef(TypedDict):
    PropertyName: NotRequired[str],
```

## GitConfigForUpdateTypeDef

```python
# GitConfigForUpdateTypeDef definition

class GitConfigForUpdateTypeDef(TypedDict):
    SecretArn: NotRequired[str],
```

## HubContentInfoTypeDef

```python
# HubContentInfoTypeDef definition

class HubContentInfoTypeDef(TypedDict):
    HubContentName: str,
    HubContentArn: str,
    HubContentVersion: str,
    HubContentType: HubContentTypeType,  # (1)
    DocumentSchemaVersion: str,
    HubContentStatus: HubContentStatusType,  # (2)
    CreationTime: datetime,
    HubContentDisplayName: NotRequired[str],
    HubContentDescription: NotRequired[str],
    HubContentSearchKeywords: NotRequired[List[str]],
```

1. See [:material-code-brackets: HubContentTypeType](./literals.md#hubcontenttypetype) 
2. See [:material-code-brackets: HubContentStatusType](./literals.md#hubcontentstatustype) 
## HubInfoTypeDef

```python
# HubInfoTypeDef definition

class HubInfoTypeDef(TypedDict):
    HubName: str,
    HubArn: str,
    HubStatus: HubStatusType,  # (1)
    CreationTime: datetime,
    LastModifiedTime: datetime,
    HubDisplayName: NotRequired[str],
    HubDescription: NotRequired[str],
    HubSearchKeywords: NotRequired[List[str]],
```

1. See [:material-code-brackets: HubStatusType](./literals.md#hubstatustype) 
## HumanLoopActivationConditionsConfigTypeDef

```python
# HumanLoopActivationConditionsConfigTypeDef definition

class HumanLoopActivationConditionsConfigTypeDef(TypedDict):
    HumanLoopActivationConditions: str,
```

## UiConfigTypeDef

```python
# UiConfigTypeDef definition

class UiConfigTypeDef(TypedDict):
    UiTemplateS3Uri: NotRequired[str],
    HumanTaskUiArn: NotRequired[str],
```

## HumanTaskUiSummaryTypeDef

```python
# HumanTaskUiSummaryTypeDef definition

class HumanTaskUiSummaryTypeDef(TypedDict):
    HumanTaskUiName: str,
    HumanTaskUiArn: str,
    CreationTime: datetime,
```

## HyperParameterTuningJobObjectiveTypeDef

```python
# HyperParameterTuningJobObjectiveTypeDef definition

class HyperParameterTuningJobObjectiveTypeDef(TypedDict):
    Type: HyperParameterTuningJobObjectiveTypeType,  # (1)
    MetricName: str,
```

1. See [:material-code-brackets: HyperParameterTuningJobObjectiveTypeType](./literals.md#hyperparametertuningjobobjectivetypetype) 
## HyperParameterTuningInstanceConfigTypeDef

```python
# HyperParameterTuningInstanceConfigTypeDef definition

class HyperParameterTuningInstanceConfigTypeDef(TypedDict):
    InstanceType: TrainingInstanceTypeType,  # (1)
    InstanceCount: int,
    VolumeSizeInGB: int,
```

1. See [:material-code-brackets: TrainingInstanceTypeType](./literals.md#traininginstancetypetype) 
## ResourceLimitsTypeDef

```python
# ResourceLimitsTypeDef definition

class ResourceLimitsTypeDef(TypedDict):
    MaxParallelTrainingJobs: int,
    MaxNumberOfTrainingJobs: NotRequired[int],
    MaxRuntimeInSeconds: NotRequired[int],
```

## HyperbandStrategyConfigTypeDef

```python
# HyperbandStrategyConfigTypeDef definition

class HyperbandStrategyConfigTypeDef(TypedDict):
    MinResource: NotRequired[int],
    MaxResource: NotRequired[int],
```

## ParentHyperParameterTuningJobTypeDef

```python
# ParentHyperParameterTuningJobTypeDef definition

class ParentHyperParameterTuningJobTypeDef(TypedDict):
    HyperParameterTuningJobName: NotRequired[str],
```

## IamIdentityTypeDef

```python
# IamIdentityTypeDef definition

class IamIdentityTypeDef(TypedDict):
    Arn: NotRequired[str],
    PrincipalId: NotRequired[str],
    SourceIdentity: NotRequired[str],
```

## RepositoryAuthConfigTypeDef

```python
# RepositoryAuthConfigTypeDef definition

class RepositoryAuthConfigTypeDef(TypedDict):
    RepositoryCredentialsProviderArn: str,
```

## ImageTypeDef

```python
# ImageTypeDef definition

class ImageTypeDef(TypedDict):
    CreationTime: datetime,
    ImageArn: str,
    ImageName: str,
    ImageStatus: ImageStatusType,  # (1)
    LastModifiedTime: datetime,
    Description: NotRequired[str],
    DisplayName: NotRequired[str],
    FailureReason: NotRequired[str],
```

1. See [:material-code-brackets: ImageStatusType](./literals.md#imagestatustype) 
## ImageVersionTypeDef

```python
# ImageVersionTypeDef definition

class ImageVersionTypeDef(TypedDict):
    CreationTime: datetime,
    ImageArn: str,
    ImageVersionArn: str,
    ImageVersionStatus: ImageVersionStatusType,  # (1)
    LastModifiedTime: datetime,
    Version: int,
    FailureReason: NotRequired[str],
```

1. See [:material-code-brackets: ImageVersionStatusType](./literals.md#imageversionstatustype) 
## RecommendationMetricsTypeDef

```python
# RecommendationMetricsTypeDef definition

class RecommendationMetricsTypeDef(TypedDict):
    CostPerHour: float,
    CostPerInference: float,
    MaxInvocations: int,
    ModelLatency: int,
    CpuUtilization: NotRequired[float],
    MemoryUtilization: NotRequired[float],
    ModelSetupTime: NotRequired[int],
```

## InferenceRecommendationsJobTypeDef

```python
# InferenceRecommendationsJobTypeDef definition

class InferenceRecommendationsJobTypeDef(TypedDict):
    JobName: str,
    JobDescription: str,
    JobType: RecommendationJobTypeType,  # (1)
    JobArn: str,
    Status: RecommendationJobStatusType,  # (2)
    CreationTime: datetime,
    RoleArn: str,
    LastModifiedTime: datetime,
    CompletionTime: NotRequired[datetime],
    FailureReason: NotRequired[str],
    ModelName: NotRequired[str],
    SamplePayloadUrl: NotRequired[str],
    ModelPackageVersionArn: NotRequired[str],
```

1. See [:material-code-brackets: RecommendationJobTypeType](./literals.md#recommendationjobtypetype) 
2. See [:material-code-brackets: RecommendationJobStatusType](./literals.md#recommendationjobstatustype) 
## InstanceGroupTypeDef

```python
# InstanceGroupTypeDef definition

class InstanceGroupTypeDef(TypedDict):
    InstanceType: TrainingInstanceTypeType,  # (1)
    InstanceCount: int,
    InstanceGroupName: str,
```

1. See [:material-code-brackets: TrainingInstanceTypeType](./literals.md#traininginstancetypetype) 
## IntegerParameterRangeSpecificationTypeDef

```python
# IntegerParameterRangeSpecificationTypeDef definition

class IntegerParameterRangeSpecificationTypeDef(TypedDict):
    MinValue: str,
    MaxValue: str,
```

## IntegerParameterRangeTypeDef

```python
# IntegerParameterRangeTypeDef definition

class IntegerParameterRangeTypeDef(TypedDict):
    Name: str,
    MinValue: str,
    MaxValue: str,
    ScalingType: NotRequired[HyperParameterScalingTypeType],  # (1)
```

1. See [:material-code-brackets: HyperParameterScalingTypeType](./literals.md#hyperparameterscalingtypetype) 
## KernelSpecTypeDef

```python
# KernelSpecTypeDef definition

class KernelSpecTypeDef(TypedDict):
    Name: str,
    DisplayName: NotRequired[str],
```

## LabelCountersForWorkteamTypeDef

```python
# LabelCountersForWorkteamTypeDef definition

class LabelCountersForWorkteamTypeDef(TypedDict):
    HumanLabeled: NotRequired[int],
    PendingHuman: NotRequired[int],
    Total: NotRequired[int],
```

## LabelingJobDataAttributesTypeDef

```python
# LabelingJobDataAttributesTypeDef definition

class LabelingJobDataAttributesTypeDef(TypedDict):
    ContentClassifiers: NotRequired[Sequence[ContentClassifierType]],  # (1)
```

1. See [:material-code-brackets: ContentClassifierType](./literals.md#contentclassifiertype) 
## LabelingJobS3DataSourceTypeDef

```python
# LabelingJobS3DataSourceTypeDef definition

class LabelingJobS3DataSourceTypeDef(TypedDict):
    ManifestS3Uri: str,
```

## LabelingJobSnsDataSourceTypeDef

```python
# LabelingJobSnsDataSourceTypeDef definition

class LabelingJobSnsDataSourceTypeDef(TypedDict):
    SnsTopicArn: str,
```

## LineageGroupSummaryTypeDef

```python
# LineageGroupSummaryTypeDef definition

class LineageGroupSummaryTypeDef(TypedDict):
    LineageGroupArn: NotRequired[str],
    LineageGroupName: NotRequired[str],
    DisplayName: NotRequired[str],
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAliasesRequestRequestTypeDef

```python
# ListAliasesRequestRequestTypeDef definition

class ListAliasesRequestRequestTypeDef(TypedDict):
    ImageName: str,
    Alias: NotRequired[str],
    Version: NotRequired[int],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListAppsRequestRequestTypeDef

```python
# ListAppsRequestRequestTypeDef definition

class ListAppsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SortOrder: NotRequired[SortOrderType],  # (1)
    SortBy: NotRequired[AppSortKeyType],  # (2)
    DomainIdEquals: NotRequired[str],
    UserProfileNameEquals: NotRequired[str],
    SpaceNameEquals: NotRequired[str],
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-brackets: AppSortKeyType](./literals.md#appsortkeytype) 
## ListCandidatesForAutoMLJobRequestRequestTypeDef

```python
# ListCandidatesForAutoMLJobRequestRequestTypeDef definition

class ListCandidatesForAutoMLJobRequestRequestTypeDef(TypedDict):
    AutoMLJobName: str,
    StatusEquals: NotRequired[CandidateStatusType],  # (1)
    CandidateNameEquals: NotRequired[str],
    SortOrder: NotRequired[AutoMLSortOrderType],  # (2)
    SortBy: NotRequired[CandidateSortByType],  # (3)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: CandidateStatusType](./literals.md#candidatestatustype) 
2. See [:material-code-brackets: AutoMLSortOrderType](./literals.md#automlsortordertype) 
3. See [:material-code-brackets: CandidateSortByType](./literals.md#candidatesortbytype) 
## MonitoringJobDefinitionSummaryTypeDef

```python
# MonitoringJobDefinitionSummaryTypeDef definition

class MonitoringJobDefinitionSummaryTypeDef(TypedDict):
    MonitoringJobDefinitionName: str,
    MonitoringJobDefinitionArn: str,
    CreationTime: datetime,
    EndpointName: str,
```

## ListDomainsRequestRequestTypeDef

```python
# ListDomainsRequestRequestTypeDef definition

class ListDomainsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListInferenceRecommendationsJobStepsRequestRequestTypeDef

```python
# ListInferenceRecommendationsJobStepsRequestRequestTypeDef definition

class ListInferenceRecommendationsJobStepsRequestRequestTypeDef(TypedDict):
    JobName: str,
    Status: NotRequired[RecommendationJobStatusType],  # (1)
    StepType: NotRequired[RecommendationStepTypeType],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: RecommendationJobStatusType](./literals.md#recommendationjobstatustype) 
2. See [:material-code-brackets: RecommendationStepTypeType](./literals.md#recommendationsteptypetype) 
## ModelCardExportJobSummaryTypeDef

```python
# ModelCardExportJobSummaryTypeDef definition

class ModelCardExportJobSummaryTypeDef(TypedDict):
    ModelCardExportJobName: str,
    ModelCardExportJobArn: str,
    Status: ModelCardExportJobStatusType,  # (1)
    ModelCardName: str,
    ModelCardVersion: int,
    CreatedAt: datetime,
    LastModifiedAt: datetime,
```

1. See [:material-code-brackets: ModelCardExportJobStatusType](./literals.md#modelcardexportjobstatustype) 
## ModelCardVersionSummaryTypeDef

```python
# ModelCardVersionSummaryTypeDef definition

class ModelCardVersionSummaryTypeDef(TypedDict):
    ModelCardName: str,
    ModelCardArn: str,
    ModelCardStatus: ModelCardStatusType,  # (1)
    ModelCardVersion: int,
    CreationTime: datetime,
    LastModifiedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ModelCardStatusType](./literals.md#modelcardstatustype) 
## ModelCardSummaryTypeDef

```python
# ModelCardSummaryTypeDef definition

class ModelCardSummaryTypeDef(TypedDict):
    ModelCardName: str,
    ModelCardArn: str,
    ModelCardStatus: ModelCardStatusType,  # (1)
    CreationTime: datetime,
    LastModifiedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ModelCardStatusType](./literals.md#modelcardstatustype) 
## ModelMetadataSummaryTypeDef

```python
# ModelMetadataSummaryTypeDef definition

class ModelMetadataSummaryTypeDef(TypedDict):
    Domain: str,
    Framework: str,
    Task: str,
    Model: str,
    FrameworkVersion: str,
```

## ModelPackageGroupSummaryTypeDef

```python
# ModelPackageGroupSummaryTypeDef definition

class ModelPackageGroupSummaryTypeDef(TypedDict):
    ModelPackageGroupName: str,
    ModelPackageGroupArn: str,
    CreationTime: datetime,
    ModelPackageGroupStatus: ModelPackageGroupStatusType,  # (1)
    ModelPackageGroupDescription: NotRequired[str],
```

1. See [:material-code-brackets: ModelPackageGroupStatusType](./literals.md#modelpackagegroupstatustype) 
## ModelPackageSummaryTypeDef

```python
# ModelPackageSummaryTypeDef definition

class ModelPackageSummaryTypeDef(TypedDict):
    ModelPackageName: str,
    ModelPackageArn: str,
    CreationTime: datetime,
    ModelPackageStatus: ModelPackageStatusType,  # (1)
    ModelPackageGroupName: NotRequired[str],
    ModelPackageVersion: NotRequired[int],
    ModelPackageDescription: NotRequired[str],
    ModelApprovalStatus: NotRequired[ModelApprovalStatusType],  # (2)
```

1. See [:material-code-brackets: ModelPackageStatusType](./literals.md#modelpackagestatustype) 
2. See [:material-code-brackets: ModelApprovalStatusType](./literals.md#modelapprovalstatustype) 
## ModelSummaryTypeDef

```python
# ModelSummaryTypeDef definition

class ModelSummaryTypeDef(TypedDict):
    ModelName: str,
    ModelArn: str,
    CreationTime: datetime,
```

## MonitoringAlertHistorySummaryTypeDef

```python
# MonitoringAlertHistorySummaryTypeDef definition

class MonitoringAlertHistorySummaryTypeDef(TypedDict):
    MonitoringScheduleName: str,
    MonitoringAlertName: str,
    CreationTime: datetime,
    AlertStatus: MonitoringAlertStatusType,  # (1)
```

1. See [:material-code-brackets: MonitoringAlertStatusType](./literals.md#monitoringalertstatustype) 
## ListMonitoringAlertsRequestRequestTypeDef

```python
# ListMonitoringAlertsRequestRequestTypeDef definition

class ListMonitoringAlertsRequestRequestTypeDef(TypedDict):
    MonitoringScheduleName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## MonitoringScheduleSummaryTypeDef

```python
# MonitoringScheduleSummaryTypeDef definition

class MonitoringScheduleSummaryTypeDef(TypedDict):
    MonitoringScheduleName: str,
    MonitoringScheduleArn: str,
    CreationTime: datetime,
    LastModifiedTime: datetime,
    MonitoringScheduleStatus: ScheduleStatusType,  # (1)
    EndpointName: NotRequired[str],
    MonitoringJobDefinitionName: NotRequired[str],
    MonitoringType: NotRequired[MonitoringTypeType],  # (2)
```

1. See [:material-code-brackets: ScheduleStatusType](./literals.md#schedulestatustype) 
2. See [:material-code-brackets: MonitoringTypeType](./literals.md#monitoringtypetype) 
## NotebookInstanceLifecycleConfigSummaryTypeDef

```python
# NotebookInstanceLifecycleConfigSummaryTypeDef definition

class NotebookInstanceLifecycleConfigSummaryTypeDef(TypedDict):
    NotebookInstanceLifecycleConfigName: str,
    NotebookInstanceLifecycleConfigArn: str,
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
```

## NotebookInstanceSummaryTypeDef

```python
# NotebookInstanceSummaryTypeDef definition

class NotebookInstanceSummaryTypeDef(TypedDict):
    NotebookInstanceName: str,
    NotebookInstanceArn: str,
    NotebookInstanceStatus: NotRequired[NotebookInstanceStatusType],  # (1)
    Url: NotRequired[str],
    InstanceType: NotRequired[InstanceTypeType],  # (2)
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
    NotebookInstanceLifecycleConfigName: NotRequired[str],
    DefaultCodeRepository: NotRequired[str],
    AdditionalCodeRepositories: NotRequired[List[str]],
```

1. See [:material-code-brackets: NotebookInstanceStatusType](./literals.md#notebookinstancestatustype) 
2. See [:material-code-brackets: InstanceTypeType](./literals.md#instancetypetype) 
## ListPipelineExecutionStepsRequestRequestTypeDef

```python
# ListPipelineExecutionStepsRequestRequestTypeDef definition

class ListPipelineExecutionStepsRequestRequestTypeDef(TypedDict):
    PipelineExecutionArn: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SortOrder: NotRequired[SortOrderType],  # (1)
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## PipelineExecutionSummaryTypeDef

```python
# PipelineExecutionSummaryTypeDef definition

class PipelineExecutionSummaryTypeDef(TypedDict):
    PipelineExecutionArn: NotRequired[str],
    StartTime: NotRequired[datetime],
    PipelineExecutionStatus: NotRequired[PipelineExecutionStatusType],  # (1)
    PipelineExecutionDescription: NotRequired[str],
    PipelineExecutionDisplayName: NotRequired[str],
    PipelineExecutionFailureReason: NotRequired[str],
```

1. See [:material-code-brackets: PipelineExecutionStatusType](./literals.md#pipelineexecutionstatustype) 
## ListPipelineParametersForExecutionRequestRequestTypeDef

```python
# ListPipelineParametersForExecutionRequestRequestTypeDef definition

class ListPipelineParametersForExecutionRequestRequestTypeDef(TypedDict):
    PipelineExecutionArn: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ParameterTypeDef

```python
# ParameterTypeDef definition

class ParameterTypeDef(TypedDict):
    Name: str,
    Value: str,
```

## PipelineSummaryTypeDef

```python
# PipelineSummaryTypeDef definition

class PipelineSummaryTypeDef(TypedDict):
    PipelineArn: NotRequired[str],
    PipelineName: NotRequired[str],
    PipelineDisplayName: NotRequired[str],
    PipelineDescription: NotRequired[str],
    RoleArn: NotRequired[str],
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
    LastExecutionTime: NotRequired[datetime],
```

## ProcessingJobSummaryTypeDef

```python
# ProcessingJobSummaryTypeDef definition

class ProcessingJobSummaryTypeDef(TypedDict):
    ProcessingJobName: str,
    ProcessingJobArn: str,
    CreationTime: datetime,
    ProcessingJobStatus: ProcessingJobStatusType,  # (1)
    ProcessingEndTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
    FailureReason: NotRequired[str],
    ExitMessage: NotRequired[str],
```

1. See [:material-code-brackets: ProcessingJobStatusType](./literals.md#processingjobstatustype) 
## ProjectSummaryTypeDef

```python
# ProjectSummaryTypeDef definition

class ProjectSummaryTypeDef(TypedDict):
    ProjectName: str,
    ProjectArn: str,
    ProjectId: str,
    CreationTime: datetime,
    ProjectStatus: ProjectStatusType,  # (1)
    ProjectDescription: NotRequired[str],
```

1. See [:material-code-brackets: ProjectStatusType](./literals.md#projectstatustype) 
## ResourceCatalogTypeDef

```python
# ResourceCatalogTypeDef definition

class ResourceCatalogTypeDef(TypedDict):
    ResourceCatalogArn: str,
    ResourceCatalogName: str,
    Description: str,
    CreationTime: datetime,
```

## ListSpacesRequestRequestTypeDef

```python
# ListSpacesRequestRequestTypeDef definition

class ListSpacesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SortOrder: NotRequired[SortOrderType],  # (1)
    SortBy: NotRequired[SpaceSortKeyType],  # (2)
    DomainIdEquals: NotRequired[str],
    SpaceNameContains: NotRequired[str],
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-brackets: SpaceSortKeyType](./literals.md#spacesortkeytype) 
## SpaceDetailsTypeDef

```python
# SpaceDetailsTypeDef definition

class SpaceDetailsTypeDef(TypedDict):
    DomainId: NotRequired[str],
    SpaceName: NotRequired[str],
    Status: NotRequired[SpaceStatusType],  # (1)
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: SpaceStatusType](./literals.md#spacestatustype) 
## ListStageDevicesRequestRequestTypeDef

```python
# ListStageDevicesRequestRequestTypeDef definition

class ListStageDevicesRequestRequestTypeDef(TypedDict):
    EdgeDeploymentPlanName: str,
    StageName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ExcludeDevicesDeployedInOtherStage: NotRequired[bool],
```

## StudioLifecycleConfigDetailsTypeDef

```python
# StudioLifecycleConfigDetailsTypeDef definition

class StudioLifecycleConfigDetailsTypeDef(TypedDict):
    StudioLifecycleConfigArn: NotRequired[str],
    StudioLifecycleConfigName: NotRequired[str],
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
    StudioLifecycleConfigAppType: NotRequired[StudioLifecycleConfigAppTypeType],  # (1)
```

1. See [:material-code-brackets: StudioLifecycleConfigAppTypeType](./literals.md#studiolifecycleconfigapptypetype) 
## ListSubscribedWorkteamsRequestRequestTypeDef

```python
# ListSubscribedWorkteamsRequestRequestTypeDef definition

class ListSubscribedWorkteamsRequestRequestTypeDef(TypedDict):
    NameContains: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListTagsInputRequestTypeDef

```python
# ListTagsInputRequestTypeDef definition

class ListTagsInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListTrainingJobsForHyperParameterTuningJobRequestRequestTypeDef

```python
# ListTrainingJobsForHyperParameterTuningJobRequestRequestTypeDef definition

class ListTrainingJobsForHyperParameterTuningJobRequestRequestTypeDef(TypedDict):
    HyperParameterTuningJobName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    StatusEquals: NotRequired[TrainingJobStatusType],  # (1)
    SortBy: NotRequired[TrainingJobSortByOptionsType],  # (2)
    SortOrder: NotRequired[SortOrderType],  # (3)
```

1. See [:material-code-brackets: TrainingJobStatusType](./literals.md#trainingjobstatustype) 
2. See [:material-code-brackets: TrainingJobSortByOptionsType](./literals.md#trainingjobsortbyoptionstype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## TransformJobSummaryTypeDef

```python
# TransformJobSummaryTypeDef definition

class TransformJobSummaryTypeDef(TypedDict):
    TransformJobName: str,
    TransformJobArn: str,
    CreationTime: datetime,
    TransformJobStatus: TransformJobStatusType,  # (1)
    TransformEndTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
    FailureReason: NotRequired[str],
```

1. See [:material-code-brackets: TransformJobStatusType](./literals.md#transformjobstatustype) 
## ListUserProfilesRequestRequestTypeDef

```python
# ListUserProfilesRequestRequestTypeDef definition

class ListUserProfilesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SortOrder: NotRequired[SortOrderType],  # (1)
    SortBy: NotRequired[UserProfileSortKeyType],  # (2)
    DomainIdEquals: NotRequired[str],
    UserProfileNameContains: NotRequired[str],
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-brackets: UserProfileSortKeyType](./literals.md#userprofilesortkeytype) 
## UserProfileDetailsTypeDef

```python
# UserProfileDetailsTypeDef definition

class UserProfileDetailsTypeDef(TypedDict):
    DomainId: NotRequired[str],
    UserProfileName: NotRequired[str],
    Status: NotRequired[UserProfileStatusType],  # (1)
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: UserProfileStatusType](./literals.md#userprofilestatustype) 
## ListWorkforcesRequestRequestTypeDef

```python
# ListWorkforcesRequestRequestTypeDef definition

class ListWorkforcesRequestRequestTypeDef(TypedDict):
    SortBy: NotRequired[ListWorkforcesSortByOptionsType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    NameContains: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: ListWorkforcesSortByOptionsType](./literals.md#listworkforcessortbyoptionstype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListWorkteamsRequestRequestTypeDef

```python
# ListWorkteamsRequestRequestTypeDef definition

class ListWorkteamsRequestRequestTypeDef(TypedDict):
    SortBy: NotRequired[ListWorkteamsSortByOptionsType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    NameContains: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: ListWorkteamsSortByOptionsType](./literals.md#listworkteamssortbyoptionstype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## OidcMemberDefinitionTypeDef

```python
# OidcMemberDefinitionTypeDef definition

class OidcMemberDefinitionTypeDef(TypedDict):
    Groups: Sequence[str],
```

## PredefinedMetricSpecificationTypeDef

```python
# PredefinedMetricSpecificationTypeDef definition

class PredefinedMetricSpecificationTypeDef(TypedDict):
    PredefinedMetricType: NotRequired[str],
```

## MonitoringGroundTruthS3InputTypeDef

```python
# MonitoringGroundTruthS3InputTypeDef definition

class MonitoringGroundTruthS3InputTypeDef(TypedDict):
    S3Uri: NotRequired[str],
```

## ModelDashboardEndpointTypeDef

```python
# ModelDashboardEndpointTypeDef definition

class ModelDashboardEndpointTypeDef(TypedDict):
    EndpointName: str,
    EndpointArn: str,
    CreationTime: datetime,
    LastModifiedTime: datetime,
    EndpointStatus: EndpointStatusType,  # (1)
```

1. See [:material-code-brackets: EndpointStatusType](./literals.md#endpointstatustype) 
## ModelDashboardIndicatorActionTypeDef

```python
# ModelDashboardIndicatorActionTypeDef definition

class ModelDashboardIndicatorActionTypeDef(TypedDict):
    Enabled: NotRequired[bool],
```

## S3ModelDataSourceTypeDef

```python
# S3ModelDataSourceTypeDef definition

class S3ModelDataSourceTypeDef(TypedDict):
    S3Uri: str,
    S3DataType: S3ModelDataTypeType,  # (1)
    CompressionType: ModelCompressionTypeType,  # (2)
```

1. See [:material-code-brackets: S3ModelDataTypeType](./literals.md#s3modeldatatypetype) 
2. See [:material-code-brackets: ModelCompressionTypeType](./literals.md#modelcompressiontypetype) 
## RealTimeInferenceConfigTypeDef

```python
# RealTimeInferenceConfigTypeDef definition

class RealTimeInferenceConfigTypeDef(TypedDict):
    InstanceType: InstanceTypeType,  # (1)
    InstanceCount: int,
```

1. See [:material-code-brackets: InstanceTypeType](./literals.md#instancetypetype) 
## ModelInputTypeDef

```python
# ModelInputTypeDef definition

class ModelInputTypeDef(TypedDict):
    DataInputConfig: str,
```

## ModelLatencyThresholdTypeDef

```python
# ModelLatencyThresholdTypeDef definition

class ModelLatencyThresholdTypeDef(TypedDict):
    Percentile: NotRequired[str],
    ValueInMilliseconds: NotRequired[int],
```

## ModelMetadataFilterTypeDef

```python
# ModelMetadataFilterTypeDef definition

class ModelMetadataFilterTypeDef(TypedDict):
    Name: ModelMetadataFilterTypeType,  # (1)
    Value: str,
```

1. See [:material-code-brackets: ModelMetadataFilterTypeType](./literals.md#modelmetadatafiltertypetype) 
## ModelPackageStatusItemTypeDef

```python
# ModelPackageStatusItemTypeDef definition

class ModelPackageStatusItemTypeDef(TypedDict):
    Name: str,
    Status: DetailedModelPackageStatusType,  # (1)
    FailureReason: NotRequired[str],
```

1. See [:material-code-brackets: DetailedModelPackageStatusType](./literals.md#detailedmodelpackagestatustype) 
## ModelStepMetadataTypeDef

```python
# ModelStepMetadataTypeDef definition

class ModelStepMetadataTypeDef(TypedDict):
    Arn: NotRequired[str],
```

## MonitoringAppSpecificationTypeDef

```python
# MonitoringAppSpecificationTypeDef definition

class MonitoringAppSpecificationTypeDef(TypedDict):
    ImageUri: str,
    ContainerEntrypoint: NotRequired[Sequence[str]],
    ContainerArguments: NotRequired[Sequence[str]],
    RecordPreprocessorSourceUri: NotRequired[str],
    PostAnalyticsProcessorSourceUri: NotRequired[str],
```

## MonitoringClusterConfigTypeDef

```python
# MonitoringClusterConfigTypeDef definition

class MonitoringClusterConfigTypeDef(TypedDict):
    InstanceCount: int,
    InstanceType: ProcessingInstanceTypeType,  # (1)
    VolumeSizeInGB: int,
    VolumeKmsKeyId: NotRequired[str],
```

1. See [:material-code-brackets: ProcessingInstanceTypeType](./literals.md#processinginstancetypetype) 
## MonitoringCsvDatasetFormatTypeDef

```python
# MonitoringCsvDatasetFormatTypeDef definition

class MonitoringCsvDatasetFormatTypeDef(TypedDict):
    Header: NotRequired[bool],
```

## MonitoringJsonDatasetFormatTypeDef

```python
# MonitoringJsonDatasetFormatTypeDef definition

class MonitoringJsonDatasetFormatTypeDef(TypedDict):
    Line: NotRequired[bool],
```

## MonitoringS3OutputTypeDef

```python
# MonitoringS3OutputTypeDef definition

class MonitoringS3OutputTypeDef(TypedDict):
    S3Uri: str,
    LocalPath: str,
    S3UploadMode: NotRequired[ProcessingS3UploadModeType],  # (1)
```

1. See [:material-code-brackets: ProcessingS3UploadModeType](./literals.md#processings3uploadmodetype) 
## ScheduleConfigTypeDef

```python
# ScheduleConfigTypeDef definition

class ScheduleConfigTypeDef(TypedDict):
    ScheduleExpression: str,
```

## S3StorageConfigTypeDef

```python
# S3StorageConfigTypeDef definition

class S3StorageConfigTypeDef(TypedDict):
    S3Uri: str,
    KmsKeyId: NotRequired[str],
    ResolvedOutputS3Uri: NotRequired[str],
```

## OidcConfigForResponseTypeDef

```python
# OidcConfigForResponseTypeDef definition

class OidcConfigForResponseTypeDef(TypedDict):
    ClientId: NotRequired[str],
    Issuer: NotRequired[str],
    AuthorizationEndpoint: NotRequired[str],
    TokenEndpoint: NotRequired[str],
    UserInfoEndpoint: NotRequired[str],
    LogoutEndpoint: NotRequired[str],
    JwksUri: NotRequired[str],
```

## OnlineStoreSecurityConfigTypeDef

```python
# OnlineStoreSecurityConfigTypeDef definition

class OnlineStoreSecurityConfigTypeDef(TypedDict):
    KmsKeyId: NotRequired[str],
```

## TtlDurationTypeDef

```python
# TtlDurationTypeDef definition

class TtlDurationTypeDef(TypedDict):
    Unit: NotRequired[TtlDurationUnitType],  # (1)
    Value: NotRequired[int],
```

1. See [:material-code-brackets: TtlDurationUnitType](./literals.md#ttldurationunittype) 
## TargetPlatformTypeDef

```python
# TargetPlatformTypeDef definition

class TargetPlatformTypeDef(TypedDict):
    Os: TargetPlatformOsType,  # (1)
    Arch: TargetPlatformArchType,  # (2)
    Accelerator: NotRequired[TargetPlatformAcceleratorType],  # (3)
```

1. See [:material-code-brackets: TargetPlatformOsType](./literals.md#targetplatformostype) 
2. See [:material-code-brackets: TargetPlatformArchType](./literals.md#targetplatformarchtype) 
3. See [:material-code-brackets: TargetPlatformAcceleratorType](./literals.md#targetplatformacceleratortype) 
## ParentTypeDef

```python
# ParentTypeDef definition

class ParentTypeDef(TypedDict):
    TrialName: NotRequired[str],
    ExperimentName: NotRequired[str],
```

## ProductionVariantStatusTypeDef

```python
# ProductionVariantStatusTypeDef definition

class ProductionVariantStatusTypeDef(TypedDict):
    Status: VariantStatusType,  # (1)
    StatusMessage: NotRequired[str],
    StartTime: NotRequired[datetime],
```

1. See [:material-code-brackets: VariantStatusType](./literals.md#variantstatustype) 
## PhaseTypeDef

```python
# PhaseTypeDef definition

class PhaseTypeDef(TypedDict):
    InitialNumberOfUsers: NotRequired[int],
    SpawnRate: NotRequired[int],
    DurationInSeconds: NotRequired[int],
```

## ProcessingJobStepMetadataTypeDef

```python
# ProcessingJobStepMetadataTypeDef definition

class ProcessingJobStepMetadataTypeDef(TypedDict):
    Arn: NotRequired[str],
```

## QualityCheckStepMetadataTypeDef

```python
# QualityCheckStepMetadataTypeDef definition

class QualityCheckStepMetadataTypeDef(TypedDict):
    CheckType: NotRequired[str],
    BaselineUsedForDriftCheckStatistics: NotRequired[str],
    BaselineUsedForDriftCheckConstraints: NotRequired[str],
    CalculatedBaselineStatistics: NotRequired[str],
    CalculatedBaselineConstraints: NotRequired[str],
    ModelPackageGroupName: NotRequired[str],
    ViolationReport: NotRequired[str],
    CheckJobArn: NotRequired[str],
    SkipCheck: NotRequired[bool],
    RegisterNewBaseline: NotRequired[bool],
```

## RegisterModelStepMetadataTypeDef

```python
# RegisterModelStepMetadataTypeDef definition

class RegisterModelStepMetadataTypeDef(TypedDict):
    Arn: NotRequired[str],
```

## TrainingJobStepMetadataTypeDef

```python
# TrainingJobStepMetadataTypeDef definition

class TrainingJobStepMetadataTypeDef(TypedDict):
    Arn: NotRequired[str],
```

## TransformJobStepMetadataTypeDef

```python
# TransformJobStepMetadataTypeDef definition

class TransformJobStepMetadataTypeDef(TypedDict):
    Arn: NotRequired[str],
```

## TuningJobStepMetaDataTypeDef

```python
# TuningJobStepMetaDataTypeDef definition

class TuningJobStepMetaDataTypeDef(TypedDict):
    Arn: NotRequired[str],
```

## SelectiveExecutionResultTypeDef

```python
# SelectiveExecutionResultTypeDef definition

class SelectiveExecutionResultTypeDef(TypedDict):
    SourcePipelineExecutionArn: NotRequired[str],
```

## ProcessingClusterConfigTypeDef

```python
# ProcessingClusterConfigTypeDef definition

class ProcessingClusterConfigTypeDef(TypedDict):
    InstanceCount: int,
    InstanceType: ProcessingInstanceTypeType,  # (1)
    VolumeSizeInGB: int,
    VolumeKmsKeyId: NotRequired[str],
```

1. See [:material-code-brackets: ProcessingInstanceTypeType](./literals.md#processinginstancetypetype) 
## ProcessingFeatureStoreOutputTypeDef

```python
# ProcessingFeatureStoreOutputTypeDef definition

class ProcessingFeatureStoreOutputTypeDef(TypedDict):
    FeatureGroupName: str,
```

## ProcessingS3InputTypeDef

```python
# ProcessingS3InputTypeDef definition

class ProcessingS3InputTypeDef(TypedDict):
    S3Uri: str,
    S3DataType: ProcessingS3DataTypeType,  # (1)
    LocalPath: NotRequired[str],
    S3InputMode: NotRequired[ProcessingS3InputModeType],  # (2)
    S3DataDistributionType: NotRequired[ProcessingS3DataDistributionTypeType],  # (3)
    S3CompressionType: NotRequired[ProcessingS3CompressionTypeType],  # (4)
```

1. See [:material-code-brackets: ProcessingS3DataTypeType](./literals.md#processings3datatypetype) 
2. See [:material-code-brackets: ProcessingS3InputModeType](./literals.md#processings3inputmodetype) 
3. See [:material-code-brackets: ProcessingS3DataDistributionTypeType](./literals.md#processings3datadistributiontypetype) 
4. See [:material-code-brackets: ProcessingS3CompressionTypeType](./literals.md#processings3compressiontypetype) 
## ProcessingS3OutputTypeDef

```python
# ProcessingS3OutputTypeDef definition

class ProcessingS3OutputTypeDef(TypedDict):
    S3Uri: str,
    LocalPath: str,
    S3UploadMode: ProcessingS3UploadModeType,  # (1)
```

1. See [:material-code-brackets: ProcessingS3UploadModeType](./literals.md#processings3uploadmodetype) 
## ProductionVariantCoreDumpConfigTypeDef

```python
# ProductionVariantCoreDumpConfigTypeDef definition

class ProductionVariantCoreDumpConfigTypeDef(TypedDict):
    DestinationS3Uri: str,
    KmsKeyId: NotRequired[str],
```

## ProfilerConfigForUpdateTypeDef

```python
# ProfilerConfigForUpdateTypeDef definition

class ProfilerConfigForUpdateTypeDef(TypedDict):
    S3OutputPath: NotRequired[str],
    ProfilingIntervalInMilliseconds: NotRequired[int],
    ProfilingParameters: NotRequired[Mapping[str, str]],
    DisableProfiler: NotRequired[bool],
```

## PropertyNameQueryTypeDef

```python
# PropertyNameQueryTypeDef definition

class PropertyNameQueryTypeDef(TypedDict):
    PropertyNameHint: str,
```

## ProvisioningParameterTypeDef

```python
# ProvisioningParameterTypeDef definition

class ProvisioningParameterTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## USDTypeDef

```python
# USDTypeDef definition

class USDTypeDef(TypedDict):
    Dollars: NotRequired[int],
    Cents: NotRequired[int],
    TenthFractionsOfACent: NotRequired[int],
```

## PutModelPackageGroupPolicyInputRequestTypeDef

```python
# PutModelPackageGroupPolicyInputRequestTypeDef definition

class PutModelPackageGroupPolicyInputRequestTypeDef(TypedDict):
    ModelPackageGroupName: str,
    ResourcePolicy: str,
```

## VertexTypeDef

```python
# VertexTypeDef definition

class VertexTypeDef(TypedDict):
    Arn: NotRequired[str],
    Type: NotRequired[str],
    LineageType: NotRequired[LineageTypeType],  # (1)
```

1. See [:material-code-brackets: LineageTypeType](./literals.md#lineagetypetype) 
## RStudioServerProAppSettingsTypeDef

```python
# RStudioServerProAppSettingsTypeDef definition

class RStudioServerProAppSettingsTypeDef(TypedDict):
    AccessStatus: NotRequired[RStudioServerProAccessStatusType],  # (1)
    UserGroup: NotRequired[RStudioServerProUserGroupType],  # (2)
```

1. See [:material-code-brackets: RStudioServerProAccessStatusType](./literals.md#rstudioserverproaccessstatustype) 
2. See [:material-code-brackets: RStudioServerProUserGroupType](./literals.md#rstudioserverprousergrouptype) 
## RecommendationJobCompiledOutputConfigTypeDef

```python
# RecommendationJobCompiledOutputConfigTypeDef definition

class RecommendationJobCompiledOutputConfigTypeDef(TypedDict):
    S3OutputUri: NotRequired[str],
```

## RecommendationJobPayloadConfigTypeDef

```python
# RecommendationJobPayloadConfigTypeDef definition

class RecommendationJobPayloadConfigTypeDef(TypedDict):
    SamplePayloadUrl: NotRequired[str],
    SupportedContentTypes: NotRequired[Sequence[str]],
```

## RecommendationJobResourceLimitTypeDef

```python
# RecommendationJobResourceLimitTypeDef definition

class RecommendationJobResourceLimitTypeDef(TypedDict):
    MaxNumberOfTests: NotRequired[int],
    MaxParallelOfTests: NotRequired[int],
```

## RecommendationJobVpcConfigTypeDef

```python
# RecommendationJobVpcConfigTypeDef definition

class RecommendationJobVpcConfigTypeDef(TypedDict):
    SecurityGroupIds: Sequence[str],
    Subnets: Sequence[str],
```

## RenderableTaskTypeDef

```python
# RenderableTaskTypeDef definition

class RenderableTaskTypeDef(TypedDict):
    Input: str,
```

## RenderingErrorTypeDef

```python
# RenderingErrorTypeDef definition

class RenderingErrorTypeDef(TypedDict):
    Code: str,
    Message: str,
```

## ResourceConfigForUpdateTypeDef

```python
# ResourceConfigForUpdateTypeDef definition

class ResourceConfigForUpdateTypeDef(TypedDict):
    KeepAlivePeriodInSeconds: int,
```

## SearchRequestRequestTypeDef

```python
# SearchRequestRequestTypeDef definition

class SearchRequestRequestTypeDef(TypedDict):
    Resource: ResourceTypeType,  # (1)
    SearchExpression: NotRequired[SearchExpressionTypeDef],  # (2)
    SortBy: NotRequired[str],
    SortOrder: NotRequired[SearchSortOrderType],  # (3)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    CrossAccountFilterOption: NotRequired[CrossAccountFilterOptionType],  # (4)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: SearchExpressionTypeDef](./type_defs.md#searchexpressiontypedef) 
3. See [:material-code-brackets: SearchSortOrderType](./literals.md#searchsortordertype) 
4. See [:material-code-brackets: CrossAccountFilterOptionType](./literals.md#crossaccountfilteroptiontype) 
## SelectedStepTypeDef

```python
# SelectedStepTypeDef definition

class SelectedStepTypeDef(TypedDict):
    StepName: str,
```

## SendPipelineExecutionStepFailureRequestRequestTypeDef

```python
# SendPipelineExecutionStepFailureRequestRequestTypeDef definition

class SendPipelineExecutionStepFailureRequestRequestTypeDef(TypedDict):
    CallbackToken: str,
    FailureReason: NotRequired[str],
    ClientRequestToken: NotRequired[str],
```

## ShadowModelVariantConfigTypeDef

```python
# ShadowModelVariantConfigTypeDef definition

class ShadowModelVariantConfigTypeDef(TypedDict):
    ShadowModelVariantName: str,
    SamplingPercentage: int,
```

## SharingSettingsTypeDef

```python
# SharingSettingsTypeDef definition

class SharingSettingsTypeDef(TypedDict):
    NotebookOutputOption: NotRequired[NotebookOutputOptionType],  # (1)
    S3OutputPath: NotRequired[str],
    S3KmsKeyId: NotRequired[str],
```

1. See [:material-code-brackets: NotebookOutputOptionType](./literals.md#notebookoutputoptiontype) 
## SourceAlgorithmTypeDef

```python
# SourceAlgorithmTypeDef definition

class SourceAlgorithmTypeDef(TypedDict):
    AlgorithmName: str,
    ModelDataUrl: NotRequired[str],
```

## StairsTypeDef

```python
# StairsTypeDef definition

class StairsTypeDef(TypedDict):
    DurationInSeconds: NotRequired[int],
    NumberOfSteps: NotRequired[int],
    UsersPerStep: NotRequired[int],
```

## StartEdgeDeploymentStageRequestRequestTypeDef

```python
# StartEdgeDeploymentStageRequestRequestTypeDef definition

class StartEdgeDeploymentStageRequestRequestTypeDef(TypedDict):
    EdgeDeploymentPlanName: str,
    StageName: str,
```

## StartInferenceExperimentRequestRequestTypeDef

```python
# StartInferenceExperimentRequestRequestTypeDef definition

class StartInferenceExperimentRequestRequestTypeDef(TypedDict):
    Name: str,
```

## StartMonitoringScheduleRequestRequestTypeDef

```python
# StartMonitoringScheduleRequestRequestTypeDef definition

class StartMonitoringScheduleRequestRequestTypeDef(TypedDict):
    MonitoringScheduleName: str,
```

## StartNotebookInstanceInputRequestTypeDef

```python
# StartNotebookInstanceInputRequestTypeDef definition

class StartNotebookInstanceInputRequestTypeDef(TypedDict):
    NotebookInstanceName: str,
```

## StopAutoMLJobRequestRequestTypeDef

```python
# StopAutoMLJobRequestRequestTypeDef definition

class StopAutoMLJobRequestRequestTypeDef(TypedDict):
    AutoMLJobName: str,
```

## StopCompilationJobRequestRequestTypeDef

```python
# StopCompilationJobRequestRequestTypeDef definition

class StopCompilationJobRequestRequestTypeDef(TypedDict):
    CompilationJobName: str,
```

## StopEdgeDeploymentStageRequestRequestTypeDef

```python
# StopEdgeDeploymentStageRequestRequestTypeDef definition

class StopEdgeDeploymentStageRequestRequestTypeDef(TypedDict):
    EdgeDeploymentPlanName: str,
    StageName: str,
```

## StopEdgePackagingJobRequestRequestTypeDef

```python
# StopEdgePackagingJobRequestRequestTypeDef definition

class StopEdgePackagingJobRequestRequestTypeDef(TypedDict):
    EdgePackagingJobName: str,
```

## StopHyperParameterTuningJobRequestRequestTypeDef

```python
# StopHyperParameterTuningJobRequestRequestTypeDef definition

class StopHyperParameterTuningJobRequestRequestTypeDef(TypedDict):
    HyperParameterTuningJobName: str,
```

## StopInferenceRecommendationsJobRequestRequestTypeDef

```python
# StopInferenceRecommendationsJobRequestRequestTypeDef definition

class StopInferenceRecommendationsJobRequestRequestTypeDef(TypedDict):
    JobName: str,
```

## StopLabelingJobRequestRequestTypeDef

```python
# StopLabelingJobRequestRequestTypeDef definition

class StopLabelingJobRequestRequestTypeDef(TypedDict):
    LabelingJobName: str,
```

## StopMonitoringScheduleRequestRequestTypeDef

```python
# StopMonitoringScheduleRequestRequestTypeDef definition

class StopMonitoringScheduleRequestRequestTypeDef(TypedDict):
    MonitoringScheduleName: str,
```

## StopNotebookInstanceInputRequestTypeDef

```python
# StopNotebookInstanceInputRequestTypeDef definition

class StopNotebookInstanceInputRequestTypeDef(TypedDict):
    NotebookInstanceName: str,
```

## StopPipelineExecutionRequestRequestTypeDef

```python
# StopPipelineExecutionRequestRequestTypeDef definition

class StopPipelineExecutionRequestRequestTypeDef(TypedDict):
    PipelineExecutionArn: str,
    ClientRequestToken: str,
```

## StopProcessingJobRequestRequestTypeDef

```python
# StopProcessingJobRequestRequestTypeDef definition

class StopProcessingJobRequestRequestTypeDef(TypedDict):
    ProcessingJobName: str,
```

## StopTrainingJobRequestRequestTypeDef

```python
# StopTrainingJobRequestRequestTypeDef definition

class StopTrainingJobRequestRequestTypeDef(TypedDict):
    TrainingJobName: str,
```

## StopTransformJobRequestRequestTypeDef

```python
# StopTransformJobRequestRequestTypeDef definition

class StopTransformJobRequestRequestTypeDef(TypedDict):
    TransformJobName: str,
```

## TimeSeriesConfigTypeDef

```python
# TimeSeriesConfigTypeDef definition

class TimeSeriesConfigTypeDef(TypedDict):
    TargetAttributeName: str,
    TimestampAttributeName: str,
    ItemIdentifierAttributeName: str,
    GroupingAttributeNames: NotRequired[Sequence[str]],
```

## TimeSeriesTransformationsTypeDef

```python
# TimeSeriesTransformationsTypeDef definition

class TimeSeriesTransformationsTypeDef(TypedDict):
    Filling: NotRequired[Mapping[str, Mapping[FillingTypeType, str]]],  # (1)
    Aggregation: NotRequired[Mapping[str, AggregationTransformationValueType]],  # (2)
```

1. See [:material-code-brackets: FillingTypeType](./literals.md#fillingtypetype) 
2. See [:material-code-brackets: AggregationTransformationValueType](./literals.md#aggregationtransformationvaluetype) 
## TrainingRepositoryAuthConfigTypeDef

```python
# TrainingRepositoryAuthConfigTypeDef definition

class TrainingRepositoryAuthConfigTypeDef(TypedDict):
    TrainingRepositoryCredentialsProviderArn: str,
```

## TransformS3DataSourceTypeDef

```python
# TransformS3DataSourceTypeDef definition

class TransformS3DataSourceTypeDef(TypedDict):
    S3DataType: S3DataTypeType,  # (1)
    S3Uri: str,
```

1. See [:material-code-brackets: S3DataTypeType](./literals.md#s3datatypetype) 
## UpdateActionRequestRequestTypeDef

```python
# UpdateActionRequestRequestTypeDef definition

class UpdateActionRequestRequestTypeDef(TypedDict):
    ActionName: str,
    Description: NotRequired[str],
    Status: NotRequired[ActionStatusType],  # (1)
    Properties: NotRequired[Mapping[str, str]],
    PropertiesToRemove: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: ActionStatusType](./literals.md#actionstatustype) 
## UpdateArtifactRequestRequestTypeDef

```python
# UpdateArtifactRequestRequestTypeDef definition

class UpdateArtifactRequestRequestTypeDef(TypedDict):
    ArtifactArn: str,
    ArtifactName: NotRequired[str],
    Properties: NotRequired[Mapping[str, str]],
    PropertiesToRemove: NotRequired[Sequence[str]],
```

## UpdateContextRequestRequestTypeDef

```python
# UpdateContextRequestRequestTypeDef definition

class UpdateContextRequestRequestTypeDef(TypedDict):
    ContextName: str,
    Description: NotRequired[str],
    Properties: NotRequired[Mapping[str, str]],
    PropertiesToRemove: NotRequired[Sequence[str]],
```

## VariantPropertyTypeDef

```python
# VariantPropertyTypeDef definition

class VariantPropertyTypeDef(TypedDict):
    VariantPropertyType: VariantPropertyTypeType,  # (1)
```

1. See [:material-code-brackets: VariantPropertyTypeType](./literals.md#variantpropertytypetype) 
## UpdateExperimentRequestRequestTypeDef

```python
# UpdateExperimentRequestRequestTypeDef definition

class UpdateExperimentRequestRequestTypeDef(TypedDict):
    ExperimentName: str,
    DisplayName: NotRequired[str],
    Description: NotRequired[str],
```

## UpdateHubRequestRequestTypeDef

```python
# UpdateHubRequestRequestTypeDef definition

class UpdateHubRequestRequestTypeDef(TypedDict):
    HubName: str,
    HubDescription: NotRequired[str],
    HubDisplayName: NotRequired[str],
    HubSearchKeywords: NotRequired[Sequence[str]],
```

## UpdateImageRequestRequestTypeDef

```python
# UpdateImageRequestRequestTypeDef definition

class UpdateImageRequestRequestTypeDef(TypedDict):
    ImageName: str,
    DeleteProperties: NotRequired[Sequence[str]],
    Description: NotRequired[str],
    DisplayName: NotRequired[str],
    RoleArn: NotRequired[str],
```

## UpdateImageVersionRequestRequestTypeDef

```python
# UpdateImageVersionRequestRequestTypeDef definition

class UpdateImageVersionRequestRequestTypeDef(TypedDict):
    ImageName: str,
    Alias: NotRequired[str],
    Version: NotRequired[int],
    AliasesToAdd: NotRequired[Sequence[str]],
    AliasesToDelete: NotRequired[Sequence[str]],
    VendorGuidance: NotRequired[VendorGuidanceType],  # (1)
    JobType: NotRequired[JobTypeType],  # (2)
    MLFramework: NotRequired[str],
    ProgrammingLang: NotRequired[str],
    Processor: NotRequired[ProcessorType],  # (3)
    Horovod: NotRequired[bool],
    ReleaseNotes: NotRequired[str],
```

1. See [:material-code-brackets: VendorGuidanceType](./literals.md#vendorguidancetype) 
2. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
3. See [:material-code-brackets: ProcessorType](./literals.md#processortype) 
## UpdateModelCardRequestRequestTypeDef

```python
# UpdateModelCardRequestRequestTypeDef definition

class UpdateModelCardRequestRequestTypeDef(TypedDict):
    ModelCardName: str,
    Content: NotRequired[str],
    ModelCardStatus: NotRequired[ModelCardStatusType],  # (1)
```

1. See [:material-code-brackets: ModelCardStatusType](./literals.md#modelcardstatustype) 
## UpdateMonitoringAlertRequestRequestTypeDef

```python
# UpdateMonitoringAlertRequestRequestTypeDef definition

class UpdateMonitoringAlertRequestRequestTypeDef(TypedDict):
    MonitoringScheduleName: str,
    MonitoringAlertName: str,
    DatapointsToAlert: int,
    EvaluationPeriod: int,
```

## UpdateTrialRequestRequestTypeDef

```python
# UpdateTrialRequestRequestTypeDef definition

class UpdateTrialRequestRequestTypeDef(TypedDict):
    TrialName: str,
    DisplayName: NotRequired[str],
```

## WorkforceVpcConfigResponseTypeDef

```python
# WorkforceVpcConfigResponseTypeDef definition

class WorkforceVpcConfigResponseTypeDef(TypedDict):
    VpcId: str,
    SecurityGroupIds: List[str],
    Subnets: List[str],
    VpcEndpointId: NotRequired[str],
```

## ActionSummaryTypeDef

```python
# ActionSummaryTypeDef definition

class ActionSummaryTypeDef(TypedDict):
    ActionArn: NotRequired[str],
    ActionName: NotRequired[str],
    Source: NotRequired[ActionSourceTypeDef],  # (1)
    ActionType: NotRequired[str],
    Status: NotRequired[ActionStatusType],  # (2)
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
```

1. See [:material-code-braces: ActionSourceTypeDef](./type_defs.md#actionsourcetypedef) 
2. See [:material-code-brackets: ActionStatusType](./literals.md#actionstatustype) 
## AddAssociationResponseTypeDef

```python
# AddAssociationResponseTypeDef definition

class AddAssociationResponseTypeDef(TypedDict):
    SourceArn: str,
    DestinationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateTrialComponentResponseTypeDef

```python
# AssociateTrialComponentResponseTypeDef definition

class AssociateTrialComponentResponseTypeDef(TypedDict):
    TrialComponentArn: str,
    TrialArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateActionResponseTypeDef

```python
# CreateActionResponseTypeDef definition

class CreateActionResponseTypeDef(TypedDict):
    ActionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAlgorithmOutputTypeDef

```python
# CreateAlgorithmOutputTypeDef definition

class CreateAlgorithmOutputTypeDef(TypedDict):
    AlgorithmArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAppImageConfigResponseTypeDef

```python
# CreateAppImageConfigResponseTypeDef definition

class CreateAppImageConfigResponseTypeDef(TypedDict):
    AppImageConfigArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAppResponseTypeDef

```python
# CreateAppResponseTypeDef definition

class CreateAppResponseTypeDef(TypedDict):
    AppArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateArtifactResponseTypeDef

```python
# CreateArtifactResponseTypeDef definition

class CreateArtifactResponseTypeDef(TypedDict):
    ArtifactArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAutoMLJobResponseTypeDef

```python
# CreateAutoMLJobResponseTypeDef definition

class CreateAutoMLJobResponseTypeDef(TypedDict):
    AutoMLJobArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAutoMLJobV2ResponseTypeDef

```python
# CreateAutoMLJobV2ResponseTypeDef definition

class CreateAutoMLJobV2ResponseTypeDef(TypedDict):
    AutoMLJobArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCodeRepositoryOutputTypeDef

```python
# CreateCodeRepositoryOutputTypeDef definition

class CreateCodeRepositoryOutputTypeDef(TypedDict):
    CodeRepositoryArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCompilationJobResponseTypeDef

```python
# CreateCompilationJobResponseTypeDef definition

class CreateCompilationJobResponseTypeDef(TypedDict):
    CompilationJobArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateContextResponseTypeDef

```python
# CreateContextResponseTypeDef definition

class CreateContextResponseTypeDef(TypedDict):
    ContextArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDataQualityJobDefinitionResponseTypeDef

```python
# CreateDataQualityJobDefinitionResponseTypeDef definition

class CreateDataQualityJobDefinitionResponseTypeDef(TypedDict):
    JobDefinitionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDomainResponseTypeDef

```python
# CreateDomainResponseTypeDef definition

class CreateDomainResponseTypeDef(TypedDict):
    DomainArn: str,
    Url: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEdgeDeploymentPlanResponseTypeDef

```python
# CreateEdgeDeploymentPlanResponseTypeDef definition

class CreateEdgeDeploymentPlanResponseTypeDef(TypedDict):
    EdgeDeploymentPlanArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEndpointConfigOutputTypeDef

```python
# CreateEndpointConfigOutputTypeDef definition

class CreateEndpointConfigOutputTypeDef(TypedDict):
    EndpointConfigArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEndpointOutputTypeDef

```python
# CreateEndpointOutputTypeDef definition

class CreateEndpointOutputTypeDef(TypedDict):
    EndpointArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateExperimentResponseTypeDef

```python
# CreateExperimentResponseTypeDef definition

class CreateExperimentResponseTypeDef(TypedDict):
    ExperimentArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFeatureGroupResponseTypeDef

```python
# CreateFeatureGroupResponseTypeDef definition

class CreateFeatureGroupResponseTypeDef(TypedDict):
    FeatureGroupArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFlowDefinitionResponseTypeDef

```python
# CreateFlowDefinitionResponseTypeDef definition

class CreateFlowDefinitionResponseTypeDef(TypedDict):
    FlowDefinitionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateHubResponseTypeDef

```python
# CreateHubResponseTypeDef definition

class CreateHubResponseTypeDef(TypedDict):
    HubArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateHumanTaskUiResponseTypeDef

```python
# CreateHumanTaskUiResponseTypeDef definition

class CreateHumanTaskUiResponseTypeDef(TypedDict):
    HumanTaskUiArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateHyperParameterTuningJobResponseTypeDef

```python
# CreateHyperParameterTuningJobResponseTypeDef definition

class CreateHyperParameterTuningJobResponseTypeDef(TypedDict):
    HyperParameterTuningJobArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateImageResponseTypeDef

```python
# CreateImageResponseTypeDef definition

class CreateImageResponseTypeDef(TypedDict):
    ImageArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateImageVersionResponseTypeDef

```python
# CreateImageVersionResponseTypeDef definition

class CreateImageVersionResponseTypeDef(TypedDict):
    ImageVersionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateInferenceExperimentResponseTypeDef

```python
# CreateInferenceExperimentResponseTypeDef definition

class CreateInferenceExperimentResponseTypeDef(TypedDict):
    InferenceExperimentArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateInferenceRecommendationsJobResponseTypeDef

```python
# CreateInferenceRecommendationsJobResponseTypeDef definition

class CreateInferenceRecommendationsJobResponseTypeDef(TypedDict):
    JobArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLabelingJobResponseTypeDef

```python
# CreateLabelingJobResponseTypeDef definition

class CreateLabelingJobResponseTypeDef(TypedDict):
    LabelingJobArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateModelBiasJobDefinitionResponseTypeDef

```python
# CreateModelBiasJobDefinitionResponseTypeDef definition

class CreateModelBiasJobDefinitionResponseTypeDef(TypedDict):
    JobDefinitionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateModelCardExportJobResponseTypeDef

```python
# CreateModelCardExportJobResponseTypeDef definition

class CreateModelCardExportJobResponseTypeDef(TypedDict):
    ModelCardExportJobArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateModelCardResponseTypeDef

```python
# CreateModelCardResponseTypeDef definition

class CreateModelCardResponseTypeDef(TypedDict):
    ModelCardArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateModelExplainabilityJobDefinitionResponseTypeDef

```python
# CreateModelExplainabilityJobDefinitionResponseTypeDef definition

class CreateModelExplainabilityJobDefinitionResponseTypeDef(TypedDict):
    JobDefinitionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateModelOutputTypeDef

```python
# CreateModelOutputTypeDef definition

class CreateModelOutputTypeDef(TypedDict):
    ModelArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateModelPackageGroupOutputTypeDef

```python
# CreateModelPackageGroupOutputTypeDef definition

class CreateModelPackageGroupOutputTypeDef(TypedDict):
    ModelPackageGroupArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateModelPackageOutputTypeDef

```python
# CreateModelPackageOutputTypeDef definition

class CreateModelPackageOutputTypeDef(TypedDict):
    ModelPackageArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateModelQualityJobDefinitionResponseTypeDef

```python
# CreateModelQualityJobDefinitionResponseTypeDef definition

class CreateModelQualityJobDefinitionResponseTypeDef(TypedDict):
    JobDefinitionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMonitoringScheduleResponseTypeDef

```python
# CreateMonitoringScheduleResponseTypeDef definition

class CreateMonitoringScheduleResponseTypeDef(TypedDict):
    MonitoringScheduleArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateNotebookInstanceLifecycleConfigOutputTypeDef

```python
# CreateNotebookInstanceLifecycleConfigOutputTypeDef definition

class CreateNotebookInstanceLifecycleConfigOutputTypeDef(TypedDict):
    NotebookInstanceLifecycleConfigArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateNotebookInstanceOutputTypeDef

```python
# CreateNotebookInstanceOutputTypeDef definition

class CreateNotebookInstanceOutputTypeDef(TypedDict):
    NotebookInstanceArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePipelineResponseTypeDef

```python
# CreatePipelineResponseTypeDef definition

class CreatePipelineResponseTypeDef(TypedDict):
    PipelineArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePresignedDomainUrlResponseTypeDef

```python
# CreatePresignedDomainUrlResponseTypeDef definition

class CreatePresignedDomainUrlResponseTypeDef(TypedDict):
    AuthorizedUrl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePresignedNotebookInstanceUrlOutputTypeDef

```python
# CreatePresignedNotebookInstanceUrlOutputTypeDef definition

class CreatePresignedNotebookInstanceUrlOutputTypeDef(TypedDict):
    AuthorizedUrl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProcessingJobResponseTypeDef

```python
# CreateProcessingJobResponseTypeDef definition

class CreateProcessingJobResponseTypeDef(TypedDict):
    ProcessingJobArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProjectOutputTypeDef

```python
# CreateProjectOutputTypeDef definition

class CreateProjectOutputTypeDef(TypedDict):
    ProjectArn: str,
    ProjectId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSpaceResponseTypeDef

```python
# CreateSpaceResponseTypeDef definition

class CreateSpaceResponseTypeDef(TypedDict):
    SpaceArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStudioLifecycleConfigResponseTypeDef

```python
# CreateStudioLifecycleConfigResponseTypeDef definition

class CreateStudioLifecycleConfigResponseTypeDef(TypedDict):
    StudioLifecycleConfigArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTrainingJobResponseTypeDef

```python
# CreateTrainingJobResponseTypeDef definition

class CreateTrainingJobResponseTypeDef(TypedDict):
    TrainingJobArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTransformJobResponseTypeDef

```python
# CreateTransformJobResponseTypeDef definition

class CreateTransformJobResponseTypeDef(TypedDict):
    TransformJobArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTrialComponentResponseTypeDef

```python
# CreateTrialComponentResponseTypeDef definition

class CreateTrialComponentResponseTypeDef(TypedDict):
    TrialComponentArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTrialResponseTypeDef

```python
# CreateTrialResponseTypeDef definition

class CreateTrialResponseTypeDef(TypedDict):
    TrialArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUserProfileResponseTypeDef

```python
# CreateUserProfileResponseTypeDef definition

class CreateUserProfileResponseTypeDef(TypedDict):
    UserProfileArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkforceResponseTypeDef

```python
# CreateWorkforceResponseTypeDef definition

class CreateWorkforceResponseTypeDef(TypedDict):
    WorkforceArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkteamResponseTypeDef

```python
# CreateWorkteamResponseTypeDef definition

class CreateWorkteamResponseTypeDef(TypedDict):
    WorkteamArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteActionResponseTypeDef

```python
# DeleteActionResponseTypeDef definition

class DeleteActionResponseTypeDef(TypedDict):
    ActionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteArtifactResponseTypeDef

```python
# DeleteArtifactResponseTypeDef definition

class DeleteArtifactResponseTypeDef(TypedDict):
    ArtifactArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAssociationResponseTypeDef

```python
# DeleteAssociationResponseTypeDef definition

class DeleteAssociationResponseTypeDef(TypedDict):
    SourceArn: str,
    DestinationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteContextResponseTypeDef

```python
# DeleteContextResponseTypeDef definition

class DeleteContextResponseTypeDef(TypedDict):
    ContextArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteExperimentResponseTypeDef

```python
# DeleteExperimentResponseTypeDef definition

class DeleteExperimentResponseTypeDef(TypedDict):
    ExperimentArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteInferenceExperimentResponseTypeDef

```python
# DeleteInferenceExperimentResponseTypeDef definition

class DeleteInferenceExperimentResponseTypeDef(TypedDict):
    InferenceExperimentArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeletePipelineResponseTypeDef

```python
# DeletePipelineResponseTypeDef definition

class DeletePipelineResponseTypeDef(TypedDict):
    PipelineArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteTrialComponentResponseTypeDef

```python
# DeleteTrialComponentResponseTypeDef definition

class DeleteTrialComponentResponseTypeDef(TypedDict):
    TrialComponentArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteTrialResponseTypeDef

```python
# DeleteTrialResponseTypeDef definition

class DeleteTrialResponseTypeDef(TypedDict):
    TrialArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteWorkteamResponseTypeDef

```python
# DeleteWorkteamResponseTypeDef definition

class DeleteWorkteamResponseTypeDef(TypedDict):
    Success: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeImageResponseTypeDef

```python
# DescribeImageResponseTypeDef definition

class DescribeImageResponseTypeDef(TypedDict):
    CreationTime: datetime,
    Description: str,
    DisplayName: str,
    FailureReason: str,
    ImageArn: str,
    ImageName: str,
    ImageStatus: ImageStatusType,  # (1)
    LastModifiedTime: datetime,
    RoleArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ImageStatusType](./literals.md#imagestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeImageVersionResponseTypeDef

```python
# DescribeImageVersionResponseTypeDef definition

class DescribeImageVersionResponseTypeDef(TypedDict):
    BaseImage: str,
    ContainerImage: str,
    CreationTime: datetime,
    FailureReason: str,
    ImageArn: str,
    ImageVersionArn: str,
    ImageVersionStatus: ImageVersionStatusType,  # (1)
    LastModifiedTime: datetime,
    Version: int,
    VendorGuidance: VendorGuidanceType,  # (2)
    JobType: JobTypeType,  # (3)
    MLFramework: str,
    ProgrammingLang: str,
    Processor: ProcessorType,  # (4)
    Horovod: bool,
    ReleaseNotes: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: ImageVersionStatusType](./literals.md#imageversionstatustype) 
2. See [:material-code-brackets: VendorGuidanceType](./literals.md#vendorguidancetype) 
3. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
4. See [:material-code-brackets: ProcessorType](./literals.md#processortype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePipelineDefinitionForExecutionResponseTypeDef

```python
# DescribePipelineDefinitionForExecutionResponseTypeDef definition

class DescribePipelineDefinitionForExecutionResponseTypeDef(TypedDict):
    PipelineDefinition: str,
    CreationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeStudioLifecycleConfigResponseTypeDef

```python
# DescribeStudioLifecycleConfigResponseTypeDef definition

class DescribeStudioLifecycleConfigResponseTypeDef(TypedDict):
    StudioLifecycleConfigArn: str,
    StudioLifecycleConfigName: str,
    CreationTime: datetime,
    LastModifiedTime: datetime,
    StudioLifecycleConfigContent: str,
    StudioLifecycleConfigAppType: StudioLifecycleConfigAppTypeType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StudioLifecycleConfigAppTypeType](./literals.md#studiolifecycleconfigapptypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateTrialComponentResponseTypeDef

```python
# DisassociateTrialComponentResponseTypeDef definition

class DisassociateTrialComponentResponseTypeDef(TypedDict):
    TrialComponentArn: str,
    TrialArn: str,
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
## GetLineageGroupPolicyResponseTypeDef

```python
# GetLineageGroupPolicyResponseTypeDef definition

class GetLineageGroupPolicyResponseTypeDef(TypedDict):
    LineageGroupArn: str,
    ResourcePolicy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetModelPackageGroupPolicyOutputTypeDef

```python
# GetModelPackageGroupPolicyOutputTypeDef definition

class GetModelPackageGroupPolicyOutputTypeDef(TypedDict):
    ResourcePolicy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSagemakerServicecatalogPortfolioStatusOutputTypeDef

```python
# GetSagemakerServicecatalogPortfolioStatusOutputTypeDef definition

class GetSagemakerServicecatalogPortfolioStatusOutputTypeDef(TypedDict):
    Status: SagemakerServicecatalogStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: SagemakerServicecatalogStatusType](./literals.md#sagemakerservicecatalogstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportHubContentResponseTypeDef

```python
# ImportHubContentResponseTypeDef definition

class ImportHubContentResponseTypeDef(TypedDict):
    HubArn: str,
    HubContentArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAliasesResponseTypeDef

```python
# ListAliasesResponseTypeDef definition

class ListAliasesResponseTypeDef(TypedDict):
    SageMakerImageVersionAliases: List[str],
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutModelPackageGroupPolicyOutputTypeDef

```python
# PutModelPackageGroupPolicyOutputTypeDef definition

class PutModelPackageGroupPolicyOutputTypeDef(TypedDict):
    ModelPackageGroupArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RetryPipelineExecutionResponseTypeDef

```python
# RetryPipelineExecutionResponseTypeDef definition

class RetryPipelineExecutionResponseTypeDef(TypedDict):
    PipelineExecutionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendPipelineExecutionStepFailureResponseTypeDef

```python
# SendPipelineExecutionStepFailureResponseTypeDef definition

class SendPipelineExecutionStepFailureResponseTypeDef(TypedDict):
    PipelineExecutionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendPipelineExecutionStepSuccessResponseTypeDef

```python
# SendPipelineExecutionStepSuccessResponseTypeDef definition

class SendPipelineExecutionStepSuccessResponseTypeDef(TypedDict):
    PipelineExecutionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartInferenceExperimentResponseTypeDef

```python
# StartInferenceExperimentResponseTypeDef definition

class StartInferenceExperimentResponseTypeDef(TypedDict):
    InferenceExperimentArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartPipelineExecutionResponseTypeDef

```python
# StartPipelineExecutionResponseTypeDef definition

class StartPipelineExecutionResponseTypeDef(TypedDict):
    PipelineExecutionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopInferenceExperimentResponseTypeDef

```python
# StopInferenceExperimentResponseTypeDef definition

class StopInferenceExperimentResponseTypeDef(TypedDict):
    InferenceExperimentArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopPipelineExecutionResponseTypeDef

```python
# StopPipelineExecutionResponseTypeDef definition

class StopPipelineExecutionResponseTypeDef(TypedDict):
    PipelineExecutionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateActionResponseTypeDef

```python
# UpdateActionResponseTypeDef definition

class UpdateActionResponseTypeDef(TypedDict):
    ActionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAppImageConfigResponseTypeDef

```python
# UpdateAppImageConfigResponseTypeDef definition

class UpdateAppImageConfigResponseTypeDef(TypedDict):
    AppImageConfigArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateArtifactResponseTypeDef

```python
# UpdateArtifactResponseTypeDef definition

class UpdateArtifactResponseTypeDef(TypedDict):
    ArtifactArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCodeRepositoryOutputTypeDef

```python
# UpdateCodeRepositoryOutputTypeDef definition

class UpdateCodeRepositoryOutputTypeDef(TypedDict):
    CodeRepositoryArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateContextResponseTypeDef

```python
# UpdateContextResponseTypeDef definition

class UpdateContextResponseTypeDef(TypedDict):
    ContextArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDomainResponseTypeDef

```python
# UpdateDomainResponseTypeDef definition

class UpdateDomainResponseTypeDef(TypedDict):
    DomainArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEndpointOutputTypeDef

```python
# UpdateEndpointOutputTypeDef definition

class UpdateEndpointOutputTypeDef(TypedDict):
    EndpointArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEndpointWeightsAndCapacitiesOutputTypeDef

```python
# UpdateEndpointWeightsAndCapacitiesOutputTypeDef definition

class UpdateEndpointWeightsAndCapacitiesOutputTypeDef(TypedDict):
    EndpointArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateExperimentResponseTypeDef

```python
# UpdateExperimentResponseTypeDef definition

class UpdateExperimentResponseTypeDef(TypedDict):
    ExperimentArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFeatureGroupResponseTypeDef

```python
# UpdateFeatureGroupResponseTypeDef definition

class UpdateFeatureGroupResponseTypeDef(TypedDict):
    FeatureGroupArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateHubResponseTypeDef

```python
# UpdateHubResponseTypeDef definition

class UpdateHubResponseTypeDef(TypedDict):
    HubArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateImageResponseTypeDef

```python
# UpdateImageResponseTypeDef definition

class UpdateImageResponseTypeDef(TypedDict):
    ImageArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateImageVersionResponseTypeDef

```python
# UpdateImageVersionResponseTypeDef definition

class UpdateImageVersionResponseTypeDef(TypedDict):
    ImageVersionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateInferenceExperimentResponseTypeDef

```python
# UpdateInferenceExperimentResponseTypeDef definition

class UpdateInferenceExperimentResponseTypeDef(TypedDict):
    InferenceExperimentArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateModelCardResponseTypeDef

```python
# UpdateModelCardResponseTypeDef definition

class UpdateModelCardResponseTypeDef(TypedDict):
    ModelCardArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateModelPackageOutputTypeDef

```python
# UpdateModelPackageOutputTypeDef definition

class UpdateModelPackageOutputTypeDef(TypedDict):
    ModelPackageArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMonitoringAlertResponseTypeDef

```python
# UpdateMonitoringAlertResponseTypeDef definition

class UpdateMonitoringAlertResponseTypeDef(TypedDict):
    MonitoringScheduleArn: str,
    MonitoringAlertName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMonitoringScheduleResponseTypeDef

```python
# UpdateMonitoringScheduleResponseTypeDef definition

class UpdateMonitoringScheduleResponseTypeDef(TypedDict):
    MonitoringScheduleArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePipelineExecutionResponseTypeDef

```python
# UpdatePipelineExecutionResponseTypeDef definition

class UpdatePipelineExecutionResponseTypeDef(TypedDict):
    PipelineExecutionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePipelineResponseTypeDef

```python
# UpdatePipelineResponseTypeDef definition

class UpdatePipelineResponseTypeDef(TypedDict):
    PipelineArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProjectOutputTypeDef

```python
# UpdateProjectOutputTypeDef definition

class UpdateProjectOutputTypeDef(TypedDict):
    ProjectArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSpaceResponseTypeDef

```python
# UpdateSpaceResponseTypeDef definition

class UpdateSpaceResponseTypeDef(TypedDict):
    SpaceArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTrainingJobResponseTypeDef

```python
# UpdateTrainingJobResponseTypeDef definition

class UpdateTrainingJobResponseTypeDef(TypedDict):
    TrainingJobArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTrialComponentResponseTypeDef

```python
# UpdateTrialComponentResponseTypeDef definition

class UpdateTrialComponentResponseTypeDef(TypedDict):
    TrialComponentArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTrialResponseTypeDef

```python
# UpdateTrialResponseTypeDef definition

class UpdateTrialResponseTypeDef(TypedDict):
    TrialArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateUserProfileResponseTypeDef

```python
# UpdateUserProfileResponseTypeDef definition

class UpdateUserProfileResponseTypeDef(TypedDict):
    UserProfileArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddTagsInputRequestTypeDef

```python
# AddTagsInputRequestTypeDef definition

class AddTagsInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## AddTagsOutputTypeDef

```python
# AddTagsOutputTypeDef definition

class AddTagsOutputTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateExperimentRequestRequestTypeDef

```python
# CreateExperimentRequestRequestTypeDef definition

class CreateExperimentRequestRequestTypeDef(TypedDict):
    ExperimentName: str,
    DisplayName: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateImageRequestRequestTypeDef

```python
# CreateImageRequestRequestTypeDef definition

class CreateImageRequestRequestTypeDef(TypedDict):
    ImageName: str,
    RoleArn: str,
    Description: NotRequired[str],
    DisplayName: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateModelPackageGroupInputRequestTypeDef

```python
# CreateModelPackageGroupInputRequestTypeDef definition

class CreateModelPackageGroupInputRequestTypeDef(TypedDict):
    ModelPackageGroupName: str,
    ModelPackageGroupDescription: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateStudioLifecycleConfigRequestRequestTypeDef

```python
# CreateStudioLifecycleConfigRequestRequestTypeDef definition

class CreateStudioLifecycleConfigRequestRequestTypeDef(TypedDict):
    StudioLifecycleConfigName: str,
    StudioLifecycleConfigContent: str,
    StudioLifecycleConfigAppType: StudioLifecycleConfigAppTypeType,  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: StudioLifecycleConfigAppTypeType](./literals.md#studiolifecycleconfigapptypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ImportHubContentRequestRequestTypeDef

```python
# ImportHubContentRequestRequestTypeDef definition

class ImportHubContentRequestRequestTypeDef(TypedDict):
    HubContentName: str,
    HubContentType: HubContentTypeType,  # (1)
    DocumentSchemaVersion: str,
    HubName: str,
    HubContentDocument: str,
    HubContentVersion: NotRequired[str],
    HubContentDisplayName: NotRequired[str],
    HubContentDescription: NotRequired[str],
    HubContentMarkdown: NotRequired[str],
    HubContentSearchKeywords: NotRequired[Sequence[str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: HubContentTypeType](./literals.md#hubcontenttypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsOutputTypeDef

```python
# ListTagsOutputTypeDef definition

class ListTagsOutputTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AutoRollbackConfigTypeDef

```python
# AutoRollbackConfigTypeDef definition

class AutoRollbackConfigTypeDef(TypedDict):
    Alarms: NotRequired[Sequence[AlarmTypeDef]],  # (1)
```

1. See [:material-code-braces: AlarmTypeDef](./type_defs.md#alarmtypedef) 
## HyperParameterAlgorithmSpecificationTypeDef

```python
# HyperParameterAlgorithmSpecificationTypeDef definition

class HyperParameterAlgorithmSpecificationTypeDef(TypedDict):
    TrainingInputMode: TrainingInputModeType,  # (1)
    TrainingImage: NotRequired[str],
    AlgorithmName: NotRequired[str],
    MetricDefinitions: NotRequired[Sequence[MetricDefinitionTypeDef]],  # (2)
```

1. See [:material-code-brackets: TrainingInputModeType](./literals.md#traininginputmodetype) 
2. See [:material-code-braces: MetricDefinitionTypeDef](./type_defs.md#metricdefinitiontypedef) 
## AlgorithmStatusDetailsTypeDef

```python
# AlgorithmStatusDetailsTypeDef definition

class AlgorithmStatusDetailsTypeDef(TypedDict):
    ValidationStatuses: NotRequired[List[AlgorithmStatusItemTypeDef]],  # (1)
    ImageScanStatuses: NotRequired[List[AlgorithmStatusItemTypeDef]],  # (1)
```

1. See [:material-code-braces: AlgorithmStatusItemTypeDef](./type_defs.md#algorithmstatusitemtypedef) 
2. See [:material-code-braces: AlgorithmStatusItemTypeDef](./type_defs.md#algorithmstatusitemtypedef) 
## ListAlgorithmsOutputTypeDef

```python
# ListAlgorithmsOutputTypeDef definition

class ListAlgorithmsOutputTypeDef(TypedDict):
    AlgorithmSummaryList: List[AlgorithmSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AlgorithmSummaryTypeDef](./type_defs.md#algorithmsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAppsResponseTypeDef

```python
# ListAppsResponseTypeDef definition

class ListAppsResponseTypeDef(TypedDict):
    Apps: List[AppDetailsTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppDetailsTypeDef](./type_defs.md#appdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ArtifactSourceTypeDef

```python
# ArtifactSourceTypeDef definition

class ArtifactSourceTypeDef(TypedDict):
    SourceUri: str,
    SourceTypes: NotRequired[Sequence[ArtifactSourceTypeTypeDef]],  # (1)
```

1. See [:material-code-braces: ArtifactSourceTypeTypeDef](./type_defs.md#artifactsourcetypetypedef) 
## AsyncInferenceOutputConfigTypeDef

```python
# AsyncInferenceOutputConfigTypeDef definition

class AsyncInferenceOutputConfigTypeDef(TypedDict):
    KmsKeyId: NotRequired[str],
    S3OutputPath: NotRequired[str],
    NotificationConfig: NotRequired[AsyncInferenceNotificationConfigTypeDef],  # (1)
    S3FailurePath: NotRequired[str],
```

1. See [:material-code-braces: AsyncInferenceNotificationConfigTypeDef](./type_defs.md#asyncinferencenotificationconfigtypedef) 
## AutoMLCandidateGenerationConfigTypeDef

```python
# AutoMLCandidateGenerationConfigTypeDef definition

class AutoMLCandidateGenerationConfigTypeDef(TypedDict):
    FeatureSpecificationS3Uri: NotRequired[str],
    AlgorithmsConfig: NotRequired[Sequence[AutoMLAlgorithmConfigTypeDef]],  # (1)
```

1. See [:material-code-braces: AutoMLAlgorithmConfigTypeDef](./type_defs.md#automlalgorithmconfigtypedef) 
## CandidateGenerationConfigTypeDef

```python
# CandidateGenerationConfigTypeDef definition

class CandidateGenerationConfigTypeDef(TypedDict):
    AlgorithmsConfig: NotRequired[Sequence[AutoMLAlgorithmConfigTypeDef]],  # (1)
```

1. See [:material-code-braces: AutoMLAlgorithmConfigTypeDef](./type_defs.md#automlalgorithmconfigtypedef) 
## AutoMLDataSourceTypeDef

```python
# AutoMLDataSourceTypeDef definition

class AutoMLDataSourceTypeDef(TypedDict):
    S3DataSource: AutoMLS3DataSourceTypeDef,  # (1)
```

1. See [:material-code-braces: AutoMLS3DataSourceTypeDef](./type_defs.md#automls3datasourcetypedef) 
## ImageClassificationJobConfigTypeDef

```python
# ImageClassificationJobConfigTypeDef definition

class ImageClassificationJobConfigTypeDef(TypedDict):
    CompletionCriteria: NotRequired[AutoMLJobCompletionCriteriaTypeDef],  # (1)
```

1. See [:material-code-braces: AutoMLJobCompletionCriteriaTypeDef](./type_defs.md#automljobcompletioncriteriatypedef) 
## TextClassificationJobConfigTypeDef

```python
# TextClassificationJobConfigTypeDef definition

class TextClassificationJobConfigTypeDef(TypedDict):
    ContentColumn: str,
    TargetLabelColumn: str,
    CompletionCriteria: NotRequired[AutoMLJobCompletionCriteriaTypeDef],  # (1)
```

1. See [:material-code-braces: AutoMLJobCompletionCriteriaTypeDef](./type_defs.md#automljobcompletioncriteriatypedef) 
## ResolvedAttributesTypeDef

```python
# ResolvedAttributesTypeDef definition

class ResolvedAttributesTypeDef(TypedDict):
    AutoMLJobObjective: NotRequired[AutoMLJobObjectiveTypeDef],  # (1)
    ProblemType: NotRequired[ProblemTypeType],  # (2)
    CompletionCriteria: NotRequired[AutoMLJobCompletionCriteriaTypeDef],  # (3)
```

1. See [:material-code-braces: AutoMLJobObjectiveTypeDef](./type_defs.md#automljobobjectivetypedef) 
2. See [:material-code-brackets: ProblemTypeType](./literals.md#problemtypetype) 
3. See [:material-code-braces: AutoMLJobCompletionCriteriaTypeDef](./type_defs.md#automljobcompletioncriteriatypedef) 
## AutoMLJobSummaryTypeDef

```python
# AutoMLJobSummaryTypeDef definition

class AutoMLJobSummaryTypeDef(TypedDict):
    AutoMLJobName: str,
    AutoMLJobArn: str,
    AutoMLJobStatus: AutoMLJobStatusType,  # (1)
    AutoMLJobSecondaryStatus: AutoMLJobSecondaryStatusType,  # (2)
    CreationTime: datetime,
    LastModifiedTime: datetime,
    EndTime: NotRequired[datetime],
    FailureReason: NotRequired[str],
    PartialFailureReasons: NotRequired[List[AutoMLPartialFailureReasonTypeDef]],  # (3)
```

1. See [:material-code-brackets: AutoMLJobStatusType](./literals.md#automljobstatustype) 
2. See [:material-code-brackets: AutoMLJobSecondaryStatusType](./literals.md#automljobsecondarystatustype) 
3. See [:material-code-braces: AutoMLPartialFailureReasonTypeDef](./type_defs.md#automlpartialfailurereasontypedef) 
## AutoMLProblemTypeResolvedAttributesTypeDef

```python
# AutoMLProblemTypeResolvedAttributesTypeDef definition

class AutoMLProblemTypeResolvedAttributesTypeDef(TypedDict):
    TabularResolvedAttributes: NotRequired[TabularResolvedAttributesTypeDef],  # (1)
```

1. See [:material-code-braces: TabularResolvedAttributesTypeDef](./type_defs.md#tabularresolvedattributestypedef) 
## AutoMLSecurityConfigTypeDef

```python
# AutoMLSecurityConfigTypeDef definition

class AutoMLSecurityConfigTypeDef(TypedDict):
    VolumeKmsKeyId: NotRequired[str],
    EnableInterContainerTrafficEncryption: NotRequired[bool],
    VpcConfig: NotRequired[VpcConfigTypeDef],  # (1)
```

1. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
## LabelingJobResourceConfigTypeDef

```python
# LabelingJobResourceConfigTypeDef definition

class LabelingJobResourceConfigTypeDef(TypedDict):
    VolumeKmsKeyId: NotRequired[str],
    VpcConfig: NotRequired[VpcConfigTypeDef],  # (1)
```

1. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
## MonitoringNetworkConfigTypeDef

```python
# MonitoringNetworkConfigTypeDef definition

class MonitoringNetworkConfigTypeDef(TypedDict):
    EnableInterContainerTrafficEncryption: NotRequired[bool],
    EnableNetworkIsolation: NotRequired[bool],
    VpcConfig: NotRequired[VpcConfigTypeDef],  # (1)
```

1. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
## NetworkConfigTypeDef

```python
# NetworkConfigTypeDef definition

class NetworkConfigTypeDef(TypedDict):
    EnableInterContainerTrafficEncryption: NotRequired[bool],
    EnableNetworkIsolation: NotRequired[bool],
    VpcConfig: NotRequired[VpcConfigTypeDef],  # (1)
```

1. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
## BiasTypeDef

```python
# BiasTypeDef definition

class BiasTypeDef(TypedDict):
    Report: NotRequired[MetricsSourceTypeDef],  # (1)
    PreTrainingReport: NotRequired[MetricsSourceTypeDef],  # (1)
    PostTrainingReport: NotRequired[MetricsSourceTypeDef],  # (1)
```

1. See [:material-code-braces: MetricsSourceTypeDef](./type_defs.md#metricssourcetypedef) 
2. See [:material-code-braces: MetricsSourceTypeDef](./type_defs.md#metricssourcetypedef) 
3. See [:material-code-braces: MetricsSourceTypeDef](./type_defs.md#metricssourcetypedef) 
## DriftCheckModelDataQualityTypeDef

```python
# DriftCheckModelDataQualityTypeDef definition

class DriftCheckModelDataQualityTypeDef(TypedDict):
    Statistics: NotRequired[MetricsSourceTypeDef],  # (1)
    Constraints: NotRequired[MetricsSourceTypeDef],  # (1)
```

1. See [:material-code-braces: MetricsSourceTypeDef](./type_defs.md#metricssourcetypedef) 
2. See [:material-code-braces: MetricsSourceTypeDef](./type_defs.md#metricssourcetypedef) 
## DriftCheckModelQualityTypeDef

```python
# DriftCheckModelQualityTypeDef definition

class DriftCheckModelQualityTypeDef(TypedDict):
    Statistics: NotRequired[MetricsSourceTypeDef],  # (1)
    Constraints: NotRequired[MetricsSourceTypeDef],  # (1)
```

1. See [:material-code-braces: MetricsSourceTypeDef](./type_defs.md#metricssourcetypedef) 
2. See [:material-code-braces: MetricsSourceTypeDef](./type_defs.md#metricssourcetypedef) 
## ExplainabilityTypeDef

```python
# ExplainabilityTypeDef definition

class ExplainabilityTypeDef(TypedDict):
    Report: NotRequired[MetricsSourceTypeDef],  # (1)
```

1. See [:material-code-braces: MetricsSourceTypeDef](./type_defs.md#metricssourcetypedef) 
## ModelDataQualityTypeDef

```python
# ModelDataQualityTypeDef definition

class ModelDataQualityTypeDef(TypedDict):
    Statistics: NotRequired[MetricsSourceTypeDef],  # (1)
    Constraints: NotRequired[MetricsSourceTypeDef],  # (1)
```

1. See [:material-code-braces: MetricsSourceTypeDef](./type_defs.md#metricssourcetypedef) 
2. See [:material-code-braces: MetricsSourceTypeDef](./type_defs.md#metricssourcetypedef) 
## ModelQualityTypeDef

```python
# ModelQualityTypeDef definition

class ModelQualityTypeDef(TypedDict):
    Statistics: NotRequired[MetricsSourceTypeDef],  # (1)
    Constraints: NotRequired[MetricsSourceTypeDef],  # (1)
```

1. See [:material-code-braces: MetricsSourceTypeDef](./type_defs.md#metricssourcetypedef) 
2. See [:material-code-braces: MetricsSourceTypeDef](./type_defs.md#metricssourcetypedef) 
## CallbackStepMetadataTypeDef

```python
# CallbackStepMetadataTypeDef definition

class CallbackStepMetadataTypeDef(TypedDict):
    CallbackToken: NotRequired[str],
    SqsQueueUrl: NotRequired[str],
    OutputParameters: NotRequired[List[OutputParameterTypeDef]],  # (1)
```

1. See [:material-code-braces: OutputParameterTypeDef](./type_defs.md#outputparametertypedef) 
## LambdaStepMetadataTypeDef

```python
# LambdaStepMetadataTypeDef definition

class LambdaStepMetadataTypeDef(TypedDict):
    Arn: NotRequired[str],
    OutputParameters: NotRequired[List[OutputParameterTypeDef]],  # (1)
```

1. See [:material-code-braces: OutputParameterTypeDef](./type_defs.md#outputparametertypedef) 
## SendPipelineExecutionStepSuccessRequestRequestTypeDef

```python
# SendPipelineExecutionStepSuccessRequestRequestTypeDef definition

class SendPipelineExecutionStepSuccessRequestRequestTypeDef(TypedDict):
    CallbackToken: str,
    OutputParameters: NotRequired[Sequence[OutputParameterTypeDef]],  # (1)
    ClientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: OutputParameterTypeDef](./type_defs.md#outputparametertypedef) 
## CandidatePropertiesTypeDef

```python
# CandidatePropertiesTypeDef definition

class CandidatePropertiesTypeDef(TypedDict):
    CandidateArtifactLocations: NotRequired[CandidateArtifactLocationsTypeDef],  # (1)
    CandidateMetrics: NotRequired[List[MetricDatumTypeDef]],  # (2)
```

1. See [:material-code-braces: CandidateArtifactLocationsTypeDef](./type_defs.md#candidateartifactlocationstypedef) 
2. See [:material-code-braces: MetricDatumTypeDef](./type_defs.md#metricdatumtypedef) 
## CanvasAppSettingsTypeDef

```python
# CanvasAppSettingsTypeDef definition

class CanvasAppSettingsTypeDef(TypedDict):
    TimeSeriesForecastingSettings: NotRequired[TimeSeriesForecastingSettingsTypeDef],  # (1)
    ModelRegisterSettings: NotRequired[ModelRegisterSettingsTypeDef],  # (2)
    WorkspaceSettings: NotRequired[WorkspaceSettingsTypeDef],  # (3)
```

1. See [:material-code-braces: TimeSeriesForecastingSettingsTypeDef](./type_defs.md#timeseriesforecastingsettingstypedef) 
2. See [:material-code-braces: ModelRegisterSettingsTypeDef](./type_defs.md#modelregistersettingstypedef) 
3. See [:material-code-braces: WorkspaceSettingsTypeDef](./type_defs.md#workspacesettingstypedef) 
## RollingUpdatePolicyTypeDef

```python
# RollingUpdatePolicyTypeDef definition

class RollingUpdatePolicyTypeDef(TypedDict):
    MaximumBatchSize: CapacitySizeTypeDef,  # (1)
    WaitIntervalInSeconds: int,
    MaximumExecutionTimeoutInSeconds: NotRequired[int],
    RollbackMaximumBatchSize: NotRequired[CapacitySizeTypeDef],  # (1)
```

1. See [:material-code-braces: CapacitySizeTypeDef](./type_defs.md#capacitysizetypedef) 
2. See [:material-code-braces: CapacitySizeTypeDef](./type_defs.md#capacitysizetypedef) 
## TrafficRoutingConfigTypeDef

```python
# TrafficRoutingConfigTypeDef definition

class TrafficRoutingConfigTypeDef(TypedDict):
    Type: TrafficRoutingConfigTypeType,  # (1)
    WaitIntervalInSeconds: int,
    CanarySize: NotRequired[CapacitySizeTypeDef],  # (2)
    LinearStepSize: NotRequired[CapacitySizeTypeDef],  # (2)
```

1. See [:material-code-brackets: TrafficRoutingConfigTypeType](./literals.md#trafficroutingconfigtypetype) 
2. See [:material-code-braces: CapacitySizeTypeDef](./type_defs.md#capacitysizetypedef) 
3. See [:material-code-braces: CapacitySizeTypeDef](./type_defs.md#capacitysizetypedef) 
## InferenceExperimentDataStorageConfigTypeDef

```python
# InferenceExperimentDataStorageConfigTypeDef definition

class InferenceExperimentDataStorageConfigTypeDef(TypedDict):
    Destination: str,
    KmsKey: NotRequired[str],
    ContentType: NotRequired[CaptureContentTypeHeaderTypeDef],  # (1)
```

1. See [:material-code-braces: CaptureContentTypeHeaderTypeDef](./type_defs.md#capturecontenttypeheadertypedef) 
## DataCaptureConfigTypeDef

```python
# DataCaptureConfigTypeDef definition

class DataCaptureConfigTypeDef(TypedDict):
    InitialSamplingPercentage: int,
    DestinationS3Uri: str,
    CaptureOptions: Sequence[CaptureOptionTypeDef],  # (1)
    EnableCapture: NotRequired[bool],
    KmsKeyId: NotRequired[str],
    CaptureContentTypeHeader: NotRequired[CaptureContentTypeHeaderTypeDef],  # (2)
```

1. See [:material-code-braces: CaptureOptionTypeDef](./type_defs.md#captureoptiontypedef) 
2. See [:material-code-braces: CaptureContentTypeHeaderTypeDef](./type_defs.md#capturecontenttypeheadertypedef) 
## EnvironmentParameterRangesTypeDef

```python
# EnvironmentParameterRangesTypeDef definition

class EnvironmentParameterRangesTypeDef(TypedDict):
    CategoricalParameterRanges: NotRequired[Sequence[CategoricalParameterTypeDef]],  # (1)
```

1. See [:material-code-braces: CategoricalParameterTypeDef](./type_defs.md#categoricalparametertypedef) 
## ClarifyShapConfigTypeDef

```python
# ClarifyShapConfigTypeDef definition

class ClarifyShapConfigTypeDef(TypedDict):
    ShapBaselineConfig: ClarifyShapBaselineConfigTypeDef,  # (1)
    NumberOfSamples: NotRequired[int],
    UseLogit: NotRequired[bool],
    Seed: NotRequired[int],
    TextConfig: NotRequired[ClarifyTextConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ClarifyShapBaselineConfigTypeDef](./type_defs.md#clarifyshapbaselineconfigtypedef) 
2. See [:material-code-braces: ClarifyTextConfigTypeDef](./type_defs.md#clarifytextconfigtypedef) 
## CodeRepositorySummaryTypeDef

```python
# CodeRepositorySummaryTypeDef definition

class CodeRepositorySummaryTypeDef(TypedDict):
    CodeRepositoryName: str,
    CodeRepositoryArn: str,
    CreationTime: datetime,
    LastModifiedTime: datetime,
    GitConfig: NotRequired[GitConfigTypeDef],  # (1)
```

1. See [:material-code-braces: GitConfigTypeDef](./type_defs.md#gitconfigtypedef) 
## CreateCodeRepositoryInputRequestTypeDef

```python
# CreateCodeRepositoryInputRequestTypeDef definition

class CreateCodeRepositoryInputRequestTypeDef(TypedDict):
    CodeRepositoryName: str,
    GitConfig: GitConfigTypeDef,  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: GitConfigTypeDef](./type_defs.md#gitconfigtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeCodeRepositoryOutputTypeDef

```python
# DescribeCodeRepositoryOutputTypeDef definition

class DescribeCodeRepositoryOutputTypeDef(TypedDict):
    CodeRepositoryName: str,
    CodeRepositoryArn: str,
    CreationTime: datetime,
    LastModifiedTime: datetime,
    GitConfig: GitConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GitConfigTypeDef](./type_defs.md#gitconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DebugHookConfigTypeDef

```python
# DebugHookConfigTypeDef definition

class DebugHookConfigTypeDef(TypedDict):
    S3OutputPath: str,
    LocalPath: NotRequired[str],
    HookParameters: NotRequired[Mapping[str, str]],
    CollectionConfigurations: NotRequired[Sequence[CollectionConfigurationTypeDef]],  # (1)
```

1. See [:material-code-braces: CollectionConfigurationTypeDef](./type_defs.md#collectionconfigurationtypedef) 
## ListCompilationJobsResponseTypeDef

```python
# ListCompilationJobsResponseTypeDef definition

class ListCompilationJobsResponseTypeDef(TypedDict):
    CompilationJobSummaries: List[CompilationJobSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CompilationJobSummaryTypeDef](./type_defs.md#compilationjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ContextSummaryTypeDef

```python
# ContextSummaryTypeDef definition

class ContextSummaryTypeDef(TypedDict):
    ContextArn: NotRequired[str],
    ContextName: NotRequired[str],
    Source: NotRequired[ContextSourceTypeDef],  # (1)
    ContextType: NotRequired[str],
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
```

1. See [:material-code-braces: ContextSourceTypeDef](./type_defs.md#contextsourcetypedef) 
## CreateContextRequestRequestTypeDef

```python
# CreateContextRequestRequestTypeDef definition

class CreateContextRequestRequestTypeDef(TypedDict):
    ContextName: str,
    Source: ContextSourceTypeDef,  # (1)
    ContextType: str,
    Description: NotRequired[str],
    Properties: NotRequired[Mapping[str, str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: ContextSourceTypeDef](./type_defs.md#contextsourcetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TuningJobCompletionCriteriaTypeDef

```python
# TuningJobCompletionCriteriaTypeDef definition

class TuningJobCompletionCriteriaTypeDef(TypedDict):
    TargetObjectiveMetricValue: NotRequired[float],
    BestObjectiveNotImproving: NotRequired[BestObjectiveNotImprovingTypeDef],  # (1)
    ConvergenceDetected: NotRequired[ConvergenceDetectedTypeDef],  # (2)
```

1. See [:material-code-braces: BestObjectiveNotImprovingTypeDef](./type_defs.md#bestobjectivenotimprovingtypedef) 
2. See [:material-code-braces: ConvergenceDetectedTypeDef](./type_defs.md#convergencedetectedtypedef) 
## CreateActionRequestRequestTypeDef

```python
# CreateActionRequestRequestTypeDef definition

class CreateActionRequestRequestTypeDef(TypedDict):
    ActionName: str,
    Source: ActionSourceTypeDef,  # (1)
    ActionType: str,
    Description: NotRequired[str],
    Status: NotRequired[ActionStatusType],  # (2)
    Properties: NotRequired[Mapping[str, str]],
    MetadataProperties: NotRequired[MetadataPropertiesTypeDef],  # (3)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
```

1. See [:material-code-braces: ActionSourceTypeDef](./type_defs.md#actionsourcetypedef) 
2. See [:material-code-brackets: ActionStatusType](./literals.md#actionstatustype) 
3. See [:material-code-braces: MetadataPropertiesTypeDef](./type_defs.md#metadatapropertiestypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateTrialRequestRequestTypeDef

```python
# CreateTrialRequestRequestTypeDef definition

class CreateTrialRequestRequestTypeDef(TypedDict):
    TrialName: str,
    ExperimentName: str,
    DisplayName: NotRequired[str],
    MetadataProperties: NotRequired[MetadataPropertiesTypeDef],  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: MetadataPropertiesTypeDef](./type_defs.md#metadatapropertiestypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateAppRequestRequestTypeDef

```python
# CreateAppRequestRequestTypeDef definition

class CreateAppRequestRequestTypeDef(TypedDict):
    DomainId: str,
    AppType: AppTypeType,  # (1)
    AppName: str,
    UserProfileName: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    ResourceSpec: NotRequired[ResourceSpecTypeDef],  # (3)
    SpaceName: NotRequired[str],
```

1. See [:material-code-brackets: AppTypeType](./literals.md#apptypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ResourceSpecTypeDef](./type_defs.md#resourcespectypedef) 
## DescribeAppResponseTypeDef

```python
# DescribeAppResponseTypeDef definition

class DescribeAppResponseTypeDef(TypedDict):
    AppArn: str,
    AppType: AppTypeType,  # (1)
    AppName: str,
    DomainId: str,
    UserProfileName: str,
    Status: AppStatusType,  # (2)
    LastHealthCheckTimestamp: datetime,
    LastUserActivityTimestamp: datetime,
    CreationTime: datetime,
    FailureReason: str,
    ResourceSpec: ResourceSpecTypeDef,  # (3)
    SpaceName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: AppTypeType](./literals.md#apptypetype) 
2. See [:material-code-brackets: AppStatusType](./literals.md#appstatustype) 
3. See [:material-code-braces: ResourceSpecTypeDef](./type_defs.md#resourcespectypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## JupyterServerAppSettingsTypeDef

```python
# JupyterServerAppSettingsTypeDef definition

class JupyterServerAppSettingsTypeDef(TypedDict):
    DefaultResourceSpec: NotRequired[ResourceSpecTypeDef],  # (1)
    LifecycleConfigArns: NotRequired[Sequence[str]],
    CodeRepositories: NotRequired[Sequence[CodeRepositoryTypeDef]],  # (2)
```

1. See [:material-code-braces: ResourceSpecTypeDef](./type_defs.md#resourcespectypedef) 
2. See [:material-code-braces: CodeRepositoryTypeDef](./type_defs.md#coderepositorytypedef) 
## RStudioServerProDomainSettingsForUpdateTypeDef

```python
# RStudioServerProDomainSettingsForUpdateTypeDef definition

class RStudioServerProDomainSettingsForUpdateTypeDef(TypedDict):
    DomainExecutionRoleArn: str,
    DefaultResourceSpec: NotRequired[ResourceSpecTypeDef],  # (1)
    RStudioConnectUrl: NotRequired[str],
    RStudioPackageManagerUrl: NotRequired[str],
```

1. See [:material-code-braces: ResourceSpecTypeDef](./type_defs.md#resourcespectypedef) 
## RStudioServerProDomainSettingsTypeDef

```python
# RStudioServerProDomainSettingsTypeDef definition

class RStudioServerProDomainSettingsTypeDef(TypedDict):
    DomainExecutionRoleArn: str,
    RStudioConnectUrl: NotRequired[str],
    RStudioPackageManagerUrl: NotRequired[str],
    DefaultResourceSpec: NotRequired[ResourceSpecTypeDef],  # (1)
```

1. See [:material-code-braces: ResourceSpecTypeDef](./type_defs.md#resourcespectypedef) 
## TensorBoardAppSettingsTypeDef

```python
# TensorBoardAppSettingsTypeDef definition

class TensorBoardAppSettingsTypeDef(TypedDict):
    DefaultResourceSpec: NotRequired[ResourceSpecTypeDef],  # (1)
```

1. See [:material-code-braces: ResourceSpecTypeDef](./type_defs.md#resourcespectypedef) 
## CreateDeviceFleetRequestRequestTypeDef

```python
# CreateDeviceFleetRequestRequestTypeDef definition

class CreateDeviceFleetRequestRequestTypeDef(TypedDict):
    DeviceFleetName: str,
    OutputConfig: EdgeOutputConfigTypeDef,  # (1)
    RoleArn: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    EnableIotRoleAlias: NotRequired[bool],
```

1. See [:material-code-braces: EdgeOutputConfigTypeDef](./type_defs.md#edgeoutputconfigtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateEdgePackagingJobRequestRequestTypeDef

```python
# CreateEdgePackagingJobRequestRequestTypeDef definition

class CreateEdgePackagingJobRequestRequestTypeDef(TypedDict):
    EdgePackagingJobName: str,
    CompilationJobName: str,
    ModelName: str,
    ModelVersion: str,
    RoleArn: str,
    OutputConfig: EdgeOutputConfigTypeDef,  # (1)
    ResourceKey: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: EdgeOutputConfigTypeDef](./type_defs.md#edgeoutputconfigtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeDeviceFleetResponseTypeDef

```python
# DescribeDeviceFleetResponseTypeDef definition

class DescribeDeviceFleetResponseTypeDef(TypedDict):
    DeviceFleetName: str,
    DeviceFleetArn: str,
    OutputConfig: EdgeOutputConfigTypeDef,  # (1)
    Description: str,
    CreationTime: datetime,
    LastModifiedTime: datetime,
    RoleArn: str,
    IotRoleAlias: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EdgeOutputConfigTypeDef](./type_defs.md#edgeoutputconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDeviceFleetRequestRequestTypeDef

```python
# UpdateDeviceFleetRequestRequestTypeDef definition

class UpdateDeviceFleetRequestRequestTypeDef(TypedDict):
    DeviceFleetName: str,
    OutputConfig: EdgeOutputConfigTypeDef,  # (1)
    RoleArn: NotRequired[str],
    Description: NotRequired[str],
    EnableIotRoleAlias: NotRequired[bool],
```

1. See [:material-code-braces: EdgeOutputConfigTypeDef](./type_defs.md#edgeoutputconfigtypedef) 
## CreateHubRequestRequestTypeDef

```python
# CreateHubRequestRequestTypeDef definition

class CreateHubRequestRequestTypeDef(TypedDict):
    HubName: str,
    HubDescription: str,
    HubDisplayName: NotRequired[str],
    HubSearchKeywords: NotRequired[Sequence[str]],
    S3StorageConfig: NotRequired[HubS3StorageConfigTypeDef],  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: HubS3StorageConfigTypeDef](./type_defs.md#hubs3storageconfigtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeHubResponseTypeDef

```python
# DescribeHubResponseTypeDef definition

class DescribeHubResponseTypeDef(TypedDict):
    HubName: str,
    HubArn: str,
    HubDisplayName: str,
    HubDescription: str,
    HubSearchKeywords: List[str],
    S3StorageConfig: HubS3StorageConfigTypeDef,  # (1)
    HubStatus: HubStatusType,  # (2)
    FailureReason: str,
    CreationTime: datetime,
    LastModifiedTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: HubS3StorageConfigTypeDef](./type_defs.md#hubs3storageconfigtypedef) 
2. See [:material-code-brackets: HubStatusType](./literals.md#hubstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateHumanTaskUiRequestRequestTypeDef

```python
# CreateHumanTaskUiRequestRequestTypeDef definition

class CreateHumanTaskUiRequestRequestTypeDef(TypedDict):
    HumanTaskUiName: str,
    UiTemplate: UiTemplateTypeDef,  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: UiTemplateTypeDef](./type_defs.md#uitemplatetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateModelCardExportJobRequestRequestTypeDef

```python
# CreateModelCardExportJobRequestRequestTypeDef definition

class CreateModelCardExportJobRequestRequestTypeDef(TypedDict):
    ModelCardName: str,
    ModelCardExportJobName: str,
    OutputConfig: ModelCardExportOutputConfigTypeDef,  # (1)
    ModelCardVersion: NotRequired[int],
```

1. See [:material-code-braces: ModelCardExportOutputConfigTypeDef](./type_defs.md#modelcardexportoutputconfigtypedef) 
## CreateModelCardRequestRequestTypeDef

```python
# CreateModelCardRequestRequestTypeDef definition

class CreateModelCardRequestRequestTypeDef(TypedDict):
    ModelCardName: str,
    Content: str,
    ModelCardStatus: ModelCardStatusType,  # (1)
    SecurityConfig: NotRequired[ModelCardSecurityConfigTypeDef],  # (2)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-brackets: ModelCardStatusType](./literals.md#modelcardstatustype) 
2. See [:material-code-braces: ModelCardSecurityConfigTypeDef](./type_defs.md#modelcardsecurityconfigtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateNotebookInstanceInputRequestTypeDef

```python
# CreateNotebookInstanceInputRequestTypeDef definition

class CreateNotebookInstanceInputRequestTypeDef(TypedDict):
    NotebookInstanceName: str,
    InstanceType: InstanceTypeType,  # (1)
    RoleArn: str,
    SubnetId: NotRequired[str],
    SecurityGroupIds: NotRequired[Sequence[str]],
    KmsKeyId: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    LifecycleConfigName: NotRequired[str],
    DirectInternetAccess: NotRequired[DirectInternetAccessType],  # (3)
    VolumeSizeInGB: NotRequired[int],
    AcceleratorTypes: NotRequired[Sequence[NotebookInstanceAcceleratorTypeType]],  # (4)
    DefaultCodeRepository: NotRequired[str],
    AdditionalCodeRepositories: NotRequired[Sequence[str]],
    RootAccess: NotRequired[RootAccessType],  # (5)
    PlatformIdentifier: NotRequired[str],
    InstanceMetadataServiceConfiguration: NotRequired[InstanceMetadataServiceConfigurationTypeDef],  # (6)
```

1. See [:material-code-brackets: InstanceTypeType](./literals.md#instancetypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: DirectInternetAccessType](./literals.md#directinternetaccesstype) 
4. See [:material-code-brackets: NotebookInstanceAcceleratorTypeType](./literals.md#notebookinstanceacceleratortypetype) 
5. See [:material-code-brackets: RootAccessType](./literals.md#rootaccesstype) 
6. See [:material-code-braces: InstanceMetadataServiceConfigurationTypeDef](./type_defs.md#instancemetadataserviceconfigurationtypedef) 
## DescribeNotebookInstanceOutputTypeDef

```python
# DescribeNotebookInstanceOutputTypeDef definition

class DescribeNotebookInstanceOutputTypeDef(TypedDict):
    NotebookInstanceArn: str,
    NotebookInstanceName: str,
    NotebookInstanceStatus: NotebookInstanceStatusType,  # (1)
    FailureReason: str,
    Url: str,
    InstanceType: InstanceTypeType,  # (2)
    SubnetId: str,
    SecurityGroups: List[str],
    RoleArn: str,
    KmsKeyId: str,
    NetworkInterfaceId: str,
    LastModifiedTime: datetime,
    CreationTime: datetime,
    NotebookInstanceLifecycleConfigName: str,
    DirectInternetAccess: DirectInternetAccessType,  # (3)
    VolumeSizeInGB: int,
    AcceleratorTypes: List[NotebookInstanceAcceleratorTypeType],  # (4)
    DefaultCodeRepository: str,
    AdditionalCodeRepositories: List[str],
    RootAccess: RootAccessType,  # (5)
    PlatformIdentifier: str,
    InstanceMetadataServiceConfiguration: InstanceMetadataServiceConfigurationTypeDef,  # (6)
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-brackets: NotebookInstanceStatusType](./literals.md#notebookinstancestatustype) 
2. See [:material-code-brackets: InstanceTypeType](./literals.md#instancetypetype) 
3. See [:material-code-brackets: DirectInternetAccessType](./literals.md#directinternetaccesstype) 
4. See [:material-code-brackets: NotebookInstanceAcceleratorTypeType](./literals.md#notebookinstanceacceleratortypetype) 
5. See [:material-code-brackets: RootAccessType](./literals.md#rootaccesstype) 
6. See [:material-code-braces: InstanceMetadataServiceConfigurationTypeDef](./type_defs.md#instancemetadataserviceconfigurationtypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateNotebookInstanceInputRequestTypeDef

```python
# UpdateNotebookInstanceInputRequestTypeDef definition

class UpdateNotebookInstanceInputRequestTypeDef(TypedDict):
    NotebookInstanceName: str,
    InstanceType: NotRequired[InstanceTypeType],  # (1)
    RoleArn: NotRequired[str],
    LifecycleConfigName: NotRequired[str],
    DisassociateLifecycleConfig: NotRequired[bool],
    VolumeSizeInGB: NotRequired[int],
    DefaultCodeRepository: NotRequired[str],
    AdditionalCodeRepositories: NotRequired[Sequence[str]],
    AcceleratorTypes: NotRequired[Sequence[NotebookInstanceAcceleratorTypeType]],  # (2)
    DisassociateAcceleratorTypes: NotRequired[bool],
    DisassociateDefaultCodeRepository: NotRequired[bool],
    DisassociateAdditionalCodeRepositories: NotRequired[bool],
    RootAccess: NotRequired[RootAccessType],  # (3)
    InstanceMetadataServiceConfiguration: NotRequired[InstanceMetadataServiceConfigurationTypeDef],  # (4)
```

1. See [:material-code-brackets: InstanceTypeType](./literals.md#instancetypetype) 
2. See [:material-code-brackets: NotebookInstanceAcceleratorTypeType](./literals.md#notebookinstanceacceleratortypetype) 
3. See [:material-code-brackets: RootAccessType](./literals.md#rootaccesstype) 
4. See [:material-code-braces: InstanceMetadataServiceConfigurationTypeDef](./type_defs.md#instancemetadataserviceconfigurationtypedef) 
## CreateNotebookInstanceLifecycleConfigInputRequestTypeDef

```python
# CreateNotebookInstanceLifecycleConfigInputRequestTypeDef definition

class CreateNotebookInstanceLifecycleConfigInputRequestTypeDef(TypedDict):
    NotebookInstanceLifecycleConfigName: str,
    OnCreate: NotRequired[Sequence[NotebookInstanceLifecycleHookTypeDef]],  # (1)
    OnStart: NotRequired[Sequence[NotebookInstanceLifecycleHookTypeDef]],  # (1)
```

1. See [:material-code-braces: NotebookInstanceLifecycleHookTypeDef](./type_defs.md#notebookinstancelifecyclehooktypedef) 
2. See [:material-code-braces: NotebookInstanceLifecycleHookTypeDef](./type_defs.md#notebookinstancelifecyclehooktypedef) 
## DescribeNotebookInstanceLifecycleConfigOutputTypeDef

```python
# DescribeNotebookInstanceLifecycleConfigOutputTypeDef definition

class DescribeNotebookInstanceLifecycleConfigOutputTypeDef(TypedDict):
    NotebookInstanceLifecycleConfigArn: str,
    NotebookInstanceLifecycleConfigName: str,
    OnCreate: List[NotebookInstanceLifecycleHookTypeDef],  # (1)
    OnStart: List[NotebookInstanceLifecycleHookTypeDef],  # (1)
    LastModifiedTime: datetime,
    CreationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: NotebookInstanceLifecycleHookTypeDef](./type_defs.md#notebookinstancelifecyclehooktypedef) 
2. See [:material-code-braces: NotebookInstanceLifecycleHookTypeDef](./type_defs.md#notebookinstancelifecyclehooktypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateNotebookInstanceLifecycleConfigInputRequestTypeDef

```python
# UpdateNotebookInstanceLifecycleConfigInputRequestTypeDef definition

class UpdateNotebookInstanceLifecycleConfigInputRequestTypeDef(TypedDict):
    NotebookInstanceLifecycleConfigName: str,
    OnCreate: NotRequired[Sequence[NotebookInstanceLifecycleHookTypeDef]],  # (1)
    OnStart: NotRequired[Sequence[NotebookInstanceLifecycleHookTypeDef]],  # (1)
```

1. See [:material-code-braces: NotebookInstanceLifecycleHookTypeDef](./type_defs.md#notebookinstancelifecyclehooktypedef) 
2. See [:material-code-braces: NotebookInstanceLifecycleHookTypeDef](./type_defs.md#notebookinstancelifecyclehooktypedef) 
## RetryPipelineExecutionRequestRequestTypeDef

```python
# RetryPipelineExecutionRequestRequestTypeDef definition

class RetryPipelineExecutionRequestRequestTypeDef(TypedDict):
    PipelineExecutionArn: str,
    ClientRequestToken: str,
    ParallelismConfiguration: NotRequired[ParallelismConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ParallelismConfigurationTypeDef](./type_defs.md#parallelismconfigurationtypedef) 
## UpdatePipelineExecutionRequestRequestTypeDef

```python
# UpdatePipelineExecutionRequestRequestTypeDef definition

class UpdatePipelineExecutionRequestRequestTypeDef(TypedDict):
    PipelineExecutionArn: str,
    PipelineExecutionDescription: NotRequired[str],
    PipelineExecutionDisplayName: NotRequired[str],
    ParallelismConfiguration: NotRequired[ParallelismConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ParallelismConfigurationTypeDef](./type_defs.md#parallelismconfigurationtypedef) 
## CreatePipelineRequestRequestTypeDef

```python
# CreatePipelineRequestRequestTypeDef definition

class CreatePipelineRequestRequestTypeDef(TypedDict):
    PipelineName: str,
    ClientRequestToken: str,
    RoleArn: str,
    PipelineDisplayName: NotRequired[str],
    PipelineDefinition: NotRequired[str],
    PipelineDefinitionS3Location: NotRequired[PipelineDefinitionS3LocationTypeDef],  # (1)
    PipelineDescription: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    ParallelismConfiguration: NotRequired[ParallelismConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: PipelineDefinitionS3LocationTypeDef](./type_defs.md#pipelinedefinitions3locationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ParallelismConfigurationTypeDef](./type_defs.md#parallelismconfigurationtypedef) 
## UpdatePipelineRequestRequestTypeDef

```python
# UpdatePipelineRequestRequestTypeDef definition

class UpdatePipelineRequestRequestTypeDef(TypedDict):
    PipelineName: str,
    PipelineDisplayName: NotRequired[str],
    PipelineDefinition: NotRequired[str],
    PipelineDefinitionS3Location: NotRequired[PipelineDefinitionS3LocationTypeDef],  # (1)
    PipelineDescription: NotRequired[str],
    RoleArn: NotRequired[str],
    ParallelismConfiguration: NotRequired[ParallelismConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: PipelineDefinitionS3LocationTypeDef](./type_defs.md#pipelinedefinitions3locationtypedef) 
2. See [:material-code-braces: ParallelismConfigurationTypeDef](./type_defs.md#parallelismconfigurationtypedef) 
## InferenceExperimentScheduleTypeDef

```python
# InferenceExperimentScheduleTypeDef definition

class InferenceExperimentScheduleTypeDef(TypedDict):
    StartTime: NotRequired[Union[datetime, str]],
    EndTime: NotRequired[Union[datetime, str]],
```

## ListActionsRequestRequestTypeDef

```python
# ListActionsRequestRequestTypeDef definition

class ListActionsRequestRequestTypeDef(TypedDict):
    SourceUri: NotRequired[str],
    ActionType: NotRequired[str],
    CreatedAfter: NotRequired[Union[datetime, str]],
    CreatedBefore: NotRequired[Union[datetime, str]],
    SortBy: NotRequired[SortActionsByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: SortActionsByType](./literals.md#sortactionsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListAlgorithmsInputRequestTypeDef

```python
# ListAlgorithmsInputRequestTypeDef definition

class ListAlgorithmsInputRequestTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    MaxResults: NotRequired[int],
    NameContains: NotRequired[str],
    NextToken: NotRequired[str],
    SortBy: NotRequired[AlgorithmSortByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
```

1. See [:material-code-brackets: AlgorithmSortByType](./literals.md#algorithmsortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListAppImageConfigsRequestRequestTypeDef

```python
# ListAppImageConfigsRequestRequestTypeDef definition

class ListAppImageConfigsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    NameContains: NotRequired[str],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    ModifiedTimeBefore: NotRequired[Union[datetime, str]],
    ModifiedTimeAfter: NotRequired[Union[datetime, str]],
    SortBy: NotRequired[AppImageConfigSortKeyType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
```

1. See [:material-code-brackets: AppImageConfigSortKeyType](./literals.md#appimageconfigsortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListArtifactsRequestRequestTypeDef

```python
# ListArtifactsRequestRequestTypeDef definition

class ListArtifactsRequestRequestTypeDef(TypedDict):
    SourceUri: NotRequired[str],
    ArtifactType: NotRequired[str],
    CreatedAfter: NotRequired[Union[datetime, str]],
    CreatedBefore: NotRequired[Union[datetime, str]],
    SortBy: NotRequired[SortArtifactsByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: SortArtifactsByType](./literals.md#sortartifactsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListAssociationsRequestRequestTypeDef

```python
# ListAssociationsRequestRequestTypeDef definition

class ListAssociationsRequestRequestTypeDef(TypedDict):
    SourceArn: NotRequired[str],
    DestinationArn: NotRequired[str],
    SourceType: NotRequired[str],
    DestinationType: NotRequired[str],
    AssociationType: NotRequired[AssociationEdgeTypeType],  # (1)
    CreatedAfter: NotRequired[Union[datetime, str]],
    CreatedBefore: NotRequired[Union[datetime, str]],
    SortBy: NotRequired[SortAssociationsByType],  # (2)
    SortOrder: NotRequired[SortOrderType],  # (3)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: AssociationEdgeTypeType](./literals.md#associationedgetypetype) 
2. See [:material-code-brackets: SortAssociationsByType](./literals.md#sortassociationsbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListAutoMLJobsRequestRequestTypeDef

```python
# ListAutoMLJobsRequestRequestTypeDef definition

class ListAutoMLJobsRequestRequestTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    NameContains: NotRequired[str],
    StatusEquals: NotRequired[AutoMLJobStatusType],  # (1)
    SortOrder: NotRequired[AutoMLSortOrderType],  # (2)
    SortBy: NotRequired[AutoMLSortByType],  # (3)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: AutoMLJobStatusType](./literals.md#automljobstatustype) 
2. See [:material-code-brackets: AutoMLSortOrderType](./literals.md#automlsortordertype) 
3. See [:material-code-brackets: AutoMLSortByType](./literals.md#automlsortbytype) 
## ListCodeRepositoriesInputRequestTypeDef

```python
# ListCodeRepositoriesInputRequestTypeDef definition

class ListCodeRepositoriesInputRequestTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    MaxResults: NotRequired[int],
    NameContains: NotRequired[str],
    NextToken: NotRequired[str],
    SortBy: NotRequired[CodeRepositorySortByType],  # (1)
    SortOrder: NotRequired[CodeRepositorySortOrderType],  # (2)
```

1. See [:material-code-brackets: CodeRepositorySortByType](./literals.md#coderepositorysortbytype) 
2. See [:material-code-brackets: CodeRepositorySortOrderType](./literals.md#coderepositorysortordertype) 
## ListCompilationJobsRequestRequestTypeDef

```python
# ListCompilationJobsRequestRequestTypeDef definition

class ListCompilationJobsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    NameContains: NotRequired[str],
    StatusEquals: NotRequired[CompilationJobStatusType],  # (1)
    SortBy: NotRequired[ListCompilationJobsSortByType],  # (2)
    SortOrder: NotRequired[SortOrderType],  # (3)
```

1. See [:material-code-brackets: CompilationJobStatusType](./literals.md#compilationjobstatustype) 
2. See [:material-code-brackets: ListCompilationJobsSortByType](./literals.md#listcompilationjobssortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListContextsRequestRequestTypeDef

```python
# ListContextsRequestRequestTypeDef definition

class ListContextsRequestRequestTypeDef(TypedDict):
    SourceUri: NotRequired[str],
    ContextType: NotRequired[str],
    CreatedAfter: NotRequired[Union[datetime, str]],
    CreatedBefore: NotRequired[Union[datetime, str]],
    SortBy: NotRequired[SortContextsByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: SortContextsByType](./literals.md#sortcontextsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListDataQualityJobDefinitionsRequestRequestTypeDef

```python
# ListDataQualityJobDefinitionsRequestRequestTypeDef definition

class ListDataQualityJobDefinitionsRequestRequestTypeDef(TypedDict):
    EndpointName: NotRequired[str],
    SortBy: NotRequired[MonitoringJobDefinitionSortKeyType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    NameContains: NotRequired[str],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
```

1. See [:material-code-brackets: MonitoringJobDefinitionSortKeyType](./literals.md#monitoringjobdefinitionsortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListDeviceFleetsRequestRequestTypeDef

```python
# ListDeviceFleetsRequestRequestTypeDef definition

class ListDeviceFleetsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    NameContains: NotRequired[str],
    SortBy: NotRequired[ListDeviceFleetsSortByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
```

1. See [:material-code-brackets: ListDeviceFleetsSortByType](./literals.md#listdevicefleetssortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListDevicesRequestRequestTypeDef

```python
# ListDevicesRequestRequestTypeDef definition

class ListDevicesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    LatestHeartbeatAfter: NotRequired[Union[datetime, str]],
    ModelName: NotRequired[str],
    DeviceFleetName: NotRequired[str],
```

## ListEdgeDeploymentPlansRequestRequestTypeDef

```python
# ListEdgeDeploymentPlansRequestRequestTypeDef definition

class ListEdgeDeploymentPlansRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    NameContains: NotRequired[str],
    DeviceFleetNameContains: NotRequired[str],
    SortBy: NotRequired[ListEdgeDeploymentPlansSortByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
```

1. See [:material-code-brackets: ListEdgeDeploymentPlansSortByType](./literals.md#listedgedeploymentplanssortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListEdgePackagingJobsRequestRequestTypeDef

```python
# ListEdgePackagingJobsRequestRequestTypeDef definition

class ListEdgePackagingJobsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    NameContains: NotRequired[str],
    ModelNameContains: NotRequired[str],
    StatusEquals: NotRequired[EdgePackagingJobStatusType],  # (1)
    SortBy: NotRequired[ListEdgePackagingJobsSortByType],  # (2)
    SortOrder: NotRequired[SortOrderType],  # (3)
```

1. See [:material-code-brackets: EdgePackagingJobStatusType](./literals.md#edgepackagingjobstatustype) 
2. See [:material-code-brackets: ListEdgePackagingJobsSortByType](./literals.md#listedgepackagingjobssortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListEndpointConfigsInputRequestTypeDef

```python
# ListEndpointConfigsInputRequestTypeDef definition

class ListEndpointConfigsInputRequestTypeDef(TypedDict):
    SortBy: NotRequired[EndpointConfigSortKeyType],  # (1)
    SortOrder: NotRequired[OrderKeyType],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    NameContains: NotRequired[str],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
```

1. See [:material-code-brackets: EndpointConfigSortKeyType](./literals.md#endpointconfigsortkeytype) 
2. See [:material-code-brackets: OrderKeyType](./literals.md#orderkeytype) 
## ListEndpointsInputRequestTypeDef

```python
# ListEndpointsInputRequestTypeDef definition

class ListEndpointsInputRequestTypeDef(TypedDict):
    SortBy: NotRequired[EndpointSortKeyType],  # (1)
    SortOrder: NotRequired[OrderKeyType],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    NameContains: NotRequired[str],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    StatusEquals: NotRequired[EndpointStatusType],  # (3)
```

1. See [:material-code-brackets: EndpointSortKeyType](./literals.md#endpointsortkeytype) 
2. See [:material-code-brackets: OrderKeyType](./literals.md#orderkeytype) 
3. See [:material-code-brackets: EndpointStatusType](./literals.md#endpointstatustype) 
## ListExperimentsRequestRequestTypeDef

```python
# ListExperimentsRequestRequestTypeDef definition

class ListExperimentsRequestRequestTypeDef(TypedDict):
    CreatedAfter: NotRequired[Union[datetime, str]],
    CreatedBefore: NotRequired[Union[datetime, str]],
    SortBy: NotRequired[SortExperimentsByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: SortExperimentsByType](./literals.md#sortexperimentsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListFeatureGroupsRequestRequestTypeDef

```python
# ListFeatureGroupsRequestRequestTypeDef definition

class ListFeatureGroupsRequestRequestTypeDef(TypedDict):
    NameContains: NotRequired[str],
    FeatureGroupStatusEquals: NotRequired[FeatureGroupStatusType],  # (1)
    OfflineStoreStatusEquals: NotRequired[OfflineStoreStatusValueType],  # (2)
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    SortOrder: NotRequired[FeatureGroupSortOrderType],  # (3)
    SortBy: NotRequired[FeatureGroupSortByType],  # (4)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: FeatureGroupStatusType](./literals.md#featuregroupstatustype) 
2. See [:material-code-brackets: OfflineStoreStatusValueType](./literals.md#offlinestorestatusvaluetype) 
3. See [:material-code-brackets: FeatureGroupSortOrderType](./literals.md#featuregroupsortordertype) 
4. See [:material-code-brackets: FeatureGroupSortByType](./literals.md#featuregroupsortbytype) 
## ListFlowDefinitionsRequestRequestTypeDef

```python
# ListFlowDefinitionsRequestRequestTypeDef definition

class ListFlowDefinitionsRequestRequestTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    SortOrder: NotRequired[SortOrderType],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListHubContentVersionsRequestRequestTypeDef

```python
# ListHubContentVersionsRequestRequestTypeDef definition

class ListHubContentVersionsRequestRequestTypeDef(TypedDict):
    HubName: str,
    HubContentType: HubContentTypeType,  # (1)
    HubContentName: str,
    MinVersion: NotRequired[str],
    MaxSchemaVersion: NotRequired[str],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    SortBy: NotRequired[HubContentSortByType],  # (2)
    SortOrder: NotRequired[SortOrderType],  # (3)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: HubContentTypeType](./literals.md#hubcontenttypetype) 
2. See [:material-code-brackets: HubContentSortByType](./literals.md#hubcontentsortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListHubContentsRequestRequestTypeDef

```python
# ListHubContentsRequestRequestTypeDef definition

class ListHubContentsRequestRequestTypeDef(TypedDict):
    HubName: str,
    HubContentType: HubContentTypeType,  # (1)
    NameContains: NotRequired[str],
    MaxSchemaVersion: NotRequired[str],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    SortBy: NotRequired[HubContentSortByType],  # (2)
    SortOrder: NotRequired[SortOrderType],  # (3)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: HubContentTypeType](./literals.md#hubcontenttypetype) 
2. See [:material-code-brackets: HubContentSortByType](./literals.md#hubcontentsortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListHubsRequestRequestTypeDef

```python
# ListHubsRequestRequestTypeDef definition

class ListHubsRequestRequestTypeDef(TypedDict):
    NameContains: NotRequired[str],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    SortBy: NotRequired[HubSortByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: HubSortByType](./literals.md#hubsortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListHumanTaskUisRequestRequestTypeDef

```python
# ListHumanTaskUisRequestRequestTypeDef definition

class ListHumanTaskUisRequestRequestTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    SortOrder: NotRequired[SortOrderType],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListHyperParameterTuningJobsRequestRequestTypeDef

```python
# ListHyperParameterTuningJobsRequestRequestTypeDef definition

class ListHyperParameterTuningJobsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SortBy: NotRequired[HyperParameterTuningJobSortByOptionsType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    NameContains: NotRequired[str],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    StatusEquals: NotRequired[HyperParameterTuningJobStatusType],  # (3)
```

1. See [:material-code-brackets: HyperParameterTuningJobSortByOptionsType](./literals.md#hyperparametertuningjobsortbyoptionstype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: HyperParameterTuningJobStatusType](./literals.md#hyperparametertuningjobstatustype) 
## ListImageVersionsRequestRequestTypeDef

```python
# ListImageVersionsRequestRequestTypeDef definition

class ListImageVersionsRequestRequestTypeDef(TypedDict):
    ImageName: str,
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    SortBy: NotRequired[ImageVersionSortByType],  # (1)
    SortOrder: NotRequired[ImageVersionSortOrderType],  # (2)
```

1. See [:material-code-brackets: ImageVersionSortByType](./literals.md#imageversionsortbytype) 
2. See [:material-code-brackets: ImageVersionSortOrderType](./literals.md#imageversionsortordertype) 
## ListImagesRequestRequestTypeDef

```python
# ListImagesRequestRequestTypeDef definition

class ListImagesRequestRequestTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    MaxResults: NotRequired[int],
    NameContains: NotRequired[str],
    NextToken: NotRequired[str],
    SortBy: NotRequired[ImageSortByType],  # (1)
    SortOrder: NotRequired[ImageSortOrderType],  # (2)
```

1. See [:material-code-brackets: ImageSortByType](./literals.md#imagesortbytype) 
2. See [:material-code-brackets: ImageSortOrderType](./literals.md#imagesortordertype) 
## ListInferenceExperimentsRequestRequestTypeDef

```python
# ListInferenceExperimentsRequestRequestTypeDef definition

class ListInferenceExperimentsRequestRequestTypeDef(TypedDict):
    NameContains: NotRequired[str],
    Type: NotRequired[InferenceExperimentTypeType],  # (1)
    StatusEquals: NotRequired[InferenceExperimentStatusType],  # (2)
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    SortBy: NotRequired[SortInferenceExperimentsByType],  # (3)
    SortOrder: NotRequired[SortOrderType],  # (4)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: InferenceExperimentTypeType](./literals.md#inferenceexperimenttypetype) 
2. See [:material-code-brackets: InferenceExperimentStatusType](./literals.md#inferenceexperimentstatustype) 
3. See [:material-code-brackets: SortInferenceExperimentsByType](./literals.md#sortinferenceexperimentsbytype) 
4. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListInferenceRecommendationsJobsRequestRequestTypeDef

```python
# ListInferenceRecommendationsJobsRequestRequestTypeDef definition

class ListInferenceRecommendationsJobsRequestRequestTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    NameContains: NotRequired[str],
    StatusEquals: NotRequired[RecommendationJobStatusType],  # (1)
    SortBy: NotRequired[ListInferenceRecommendationsJobsSortByType],  # (2)
    SortOrder: NotRequired[SortOrderType],  # (3)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ModelNameEquals: NotRequired[str],
    ModelPackageVersionArnEquals: NotRequired[str],
```

1. See [:material-code-brackets: RecommendationJobStatusType](./literals.md#recommendationjobstatustype) 
2. See [:material-code-brackets: ListInferenceRecommendationsJobsSortByType](./literals.md#listinferencerecommendationsjobssortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListLabelingJobsForWorkteamRequestRequestTypeDef

```python
# ListLabelingJobsForWorkteamRequestRequestTypeDef definition

class ListLabelingJobsForWorkteamRequestRequestTypeDef(TypedDict):
    WorkteamArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    JobReferenceCodeContains: NotRequired[str],
    SortBy: NotRequired[ListLabelingJobsForWorkteamSortByOptionsType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
```

1. See [:material-code-brackets: ListLabelingJobsForWorkteamSortByOptionsType](./literals.md#listlabelingjobsforworkteamsortbyoptionstype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListLabelingJobsRequestRequestTypeDef

```python
# ListLabelingJobsRequestRequestTypeDef definition

class ListLabelingJobsRequestRequestTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    NameContains: NotRequired[str],
    SortBy: NotRequired[SortByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    StatusEquals: NotRequired[LabelingJobStatusType],  # (3)
```

1. See [:material-code-brackets: SortByType](./literals.md#sortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: LabelingJobStatusType](./literals.md#labelingjobstatustype) 
## ListLineageGroupsRequestRequestTypeDef

```python
# ListLineageGroupsRequestRequestTypeDef definition

class ListLineageGroupsRequestRequestTypeDef(TypedDict):
    CreatedAfter: NotRequired[Union[datetime, str]],
    CreatedBefore: NotRequired[Union[datetime, str]],
    SortBy: NotRequired[SortLineageGroupsByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: SortLineageGroupsByType](./literals.md#sortlineagegroupsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListModelBiasJobDefinitionsRequestRequestTypeDef

```python
# ListModelBiasJobDefinitionsRequestRequestTypeDef definition

class ListModelBiasJobDefinitionsRequestRequestTypeDef(TypedDict):
    EndpointName: NotRequired[str],
    SortBy: NotRequired[MonitoringJobDefinitionSortKeyType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    NameContains: NotRequired[str],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
```

1. See [:material-code-brackets: MonitoringJobDefinitionSortKeyType](./literals.md#monitoringjobdefinitionsortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListModelCardExportJobsRequestRequestTypeDef

```python
# ListModelCardExportJobsRequestRequestTypeDef definition

class ListModelCardExportJobsRequestRequestTypeDef(TypedDict):
    ModelCardName: str,
    ModelCardVersion: NotRequired[int],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    ModelCardExportJobNameContains: NotRequired[str],
    StatusEquals: NotRequired[ModelCardExportJobStatusType],  # (1)
    SortBy: NotRequired[ModelCardExportJobSortByType],  # (2)
    SortOrder: NotRequired[ModelCardExportJobSortOrderType],  # (3)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: ModelCardExportJobStatusType](./literals.md#modelcardexportjobstatustype) 
2. See [:material-code-brackets: ModelCardExportJobSortByType](./literals.md#modelcardexportjobsortbytype) 
3. See [:material-code-brackets: ModelCardExportJobSortOrderType](./literals.md#modelcardexportjobsortordertype) 
## ListModelCardVersionsRequestRequestTypeDef

```python
# ListModelCardVersionsRequestRequestTypeDef definition

class ListModelCardVersionsRequestRequestTypeDef(TypedDict):
    ModelCardName: str,
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    MaxResults: NotRequired[int],
    ModelCardStatus: NotRequired[ModelCardStatusType],  # (1)
    NextToken: NotRequired[str],
    SortBy: NotRequired[ModelCardVersionSortByType],  # (2)
    SortOrder: NotRequired[ModelCardSortOrderType],  # (3)
```

1. See [:material-code-brackets: ModelCardStatusType](./literals.md#modelcardstatustype) 
2. See [:material-code-brackets: ModelCardVersionSortByType](./literals.md#modelcardversionsortbytype) 
3. See [:material-code-brackets: ModelCardSortOrderType](./literals.md#modelcardsortordertype) 
## ListModelCardsRequestRequestTypeDef

```python
# ListModelCardsRequestRequestTypeDef definition

class ListModelCardsRequestRequestTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    MaxResults: NotRequired[int],
    NameContains: NotRequired[str],
    ModelCardStatus: NotRequired[ModelCardStatusType],  # (1)
    NextToken: NotRequired[str],
    SortBy: NotRequired[ModelCardSortByType],  # (2)
    SortOrder: NotRequired[ModelCardSortOrderType],  # (3)
```

1. See [:material-code-brackets: ModelCardStatusType](./literals.md#modelcardstatustype) 
2. See [:material-code-brackets: ModelCardSortByType](./literals.md#modelcardsortbytype) 
3. See [:material-code-brackets: ModelCardSortOrderType](./literals.md#modelcardsortordertype) 
## ListModelExplainabilityJobDefinitionsRequestRequestTypeDef

```python
# ListModelExplainabilityJobDefinitionsRequestRequestTypeDef definition

class ListModelExplainabilityJobDefinitionsRequestRequestTypeDef(TypedDict):
    EndpointName: NotRequired[str],
    SortBy: NotRequired[MonitoringJobDefinitionSortKeyType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    NameContains: NotRequired[str],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
```

1. See [:material-code-brackets: MonitoringJobDefinitionSortKeyType](./literals.md#monitoringjobdefinitionsortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListModelPackageGroupsInputRequestTypeDef

```python
# ListModelPackageGroupsInputRequestTypeDef definition

class ListModelPackageGroupsInputRequestTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    MaxResults: NotRequired[int],
    NameContains: NotRequired[str],
    NextToken: NotRequired[str],
    SortBy: NotRequired[ModelPackageGroupSortByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
```

1. See [:material-code-brackets: ModelPackageGroupSortByType](./literals.md#modelpackagegroupsortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListModelPackagesInputRequestTypeDef

```python
# ListModelPackagesInputRequestTypeDef definition

class ListModelPackagesInputRequestTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    MaxResults: NotRequired[int],
    NameContains: NotRequired[str],
    ModelApprovalStatus: NotRequired[ModelApprovalStatusType],  # (1)
    ModelPackageGroupName: NotRequired[str],
    ModelPackageType: NotRequired[ModelPackageTypeType],  # (2)
    NextToken: NotRequired[str],
    SortBy: NotRequired[ModelPackageSortByType],  # (3)
    SortOrder: NotRequired[SortOrderType],  # (4)
```

1. See [:material-code-brackets: ModelApprovalStatusType](./literals.md#modelapprovalstatustype) 
2. See [:material-code-brackets: ModelPackageTypeType](./literals.md#modelpackagetypetype) 
3. See [:material-code-brackets: ModelPackageSortByType](./literals.md#modelpackagesortbytype) 
4. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListModelQualityJobDefinitionsRequestRequestTypeDef

```python
# ListModelQualityJobDefinitionsRequestRequestTypeDef definition

class ListModelQualityJobDefinitionsRequestRequestTypeDef(TypedDict):
    EndpointName: NotRequired[str],
    SortBy: NotRequired[MonitoringJobDefinitionSortKeyType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    NameContains: NotRequired[str],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
```

1. See [:material-code-brackets: MonitoringJobDefinitionSortKeyType](./literals.md#monitoringjobdefinitionsortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListModelsInputRequestTypeDef

```python
# ListModelsInputRequestTypeDef definition

class ListModelsInputRequestTypeDef(TypedDict):
    SortBy: NotRequired[ModelSortKeyType],  # (1)
    SortOrder: NotRequired[OrderKeyType],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    NameContains: NotRequired[str],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
```

1. See [:material-code-brackets: ModelSortKeyType](./literals.md#modelsortkeytype) 
2. See [:material-code-brackets: OrderKeyType](./literals.md#orderkeytype) 
## ListMonitoringAlertHistoryRequestRequestTypeDef

```python
# ListMonitoringAlertHistoryRequestRequestTypeDef definition

class ListMonitoringAlertHistoryRequestRequestTypeDef(TypedDict):
    MonitoringScheduleName: NotRequired[str],
    MonitoringAlertName: NotRequired[str],
    SortBy: NotRequired[MonitoringAlertHistorySortKeyType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    StatusEquals: NotRequired[MonitoringAlertStatusType],  # (3)
```

1. See [:material-code-brackets: MonitoringAlertHistorySortKeyType](./literals.md#monitoringalerthistorysortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: MonitoringAlertStatusType](./literals.md#monitoringalertstatustype) 
## ListMonitoringExecutionsRequestRequestTypeDef

```python
# ListMonitoringExecutionsRequestRequestTypeDef definition

class ListMonitoringExecutionsRequestRequestTypeDef(TypedDict):
    MonitoringScheduleName: NotRequired[str],
    EndpointName: NotRequired[str],
    SortBy: NotRequired[MonitoringExecutionSortKeyType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ScheduledTimeBefore: NotRequired[Union[datetime, str]],
    ScheduledTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    StatusEquals: NotRequired[ExecutionStatusType],  # (3)
    MonitoringJobDefinitionName: NotRequired[str],
    MonitoringTypeEquals: NotRequired[MonitoringTypeType],  # (4)
```

1. See [:material-code-brackets: MonitoringExecutionSortKeyType](./literals.md#monitoringexecutionsortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: ExecutionStatusType](./literals.md#executionstatustype) 
4. See [:material-code-brackets: MonitoringTypeType](./literals.md#monitoringtypetype) 
## ListMonitoringSchedulesRequestRequestTypeDef

```python
# ListMonitoringSchedulesRequestRequestTypeDef definition

class ListMonitoringSchedulesRequestRequestTypeDef(TypedDict):
    EndpointName: NotRequired[str],
    SortBy: NotRequired[MonitoringScheduleSortKeyType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    NameContains: NotRequired[str],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    StatusEquals: NotRequired[ScheduleStatusType],  # (3)
    MonitoringJobDefinitionName: NotRequired[str],
    MonitoringTypeEquals: NotRequired[MonitoringTypeType],  # (4)
```

1. See [:material-code-brackets: MonitoringScheduleSortKeyType](./literals.md#monitoringschedulesortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: ScheduleStatusType](./literals.md#schedulestatustype) 
4. See [:material-code-brackets: MonitoringTypeType](./literals.md#monitoringtypetype) 
## ListNotebookInstanceLifecycleConfigsInputRequestTypeDef

```python
# ListNotebookInstanceLifecycleConfigsInputRequestTypeDef definition

class ListNotebookInstanceLifecycleConfigsInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SortBy: NotRequired[NotebookInstanceLifecycleConfigSortKeyType],  # (1)
    SortOrder: NotRequired[NotebookInstanceLifecycleConfigSortOrderType],  # (2)
    NameContains: NotRequired[str],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
```

1. See [:material-code-brackets: NotebookInstanceLifecycleConfigSortKeyType](./literals.md#notebookinstancelifecycleconfigsortkeytype) 
2. See [:material-code-brackets: NotebookInstanceLifecycleConfigSortOrderType](./literals.md#notebookinstancelifecycleconfigsortordertype) 
## ListNotebookInstancesInputRequestTypeDef

```python
# ListNotebookInstancesInputRequestTypeDef definition

class ListNotebookInstancesInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    SortBy: NotRequired[NotebookInstanceSortKeyType],  # (1)
    SortOrder: NotRequired[NotebookInstanceSortOrderType],  # (2)
    NameContains: NotRequired[str],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    StatusEquals: NotRequired[NotebookInstanceStatusType],  # (3)
    NotebookInstanceLifecycleConfigNameContains: NotRequired[str],
    DefaultCodeRepositoryContains: NotRequired[str],
    AdditionalCodeRepositoryEquals: NotRequired[str],
```

1. See [:material-code-brackets: NotebookInstanceSortKeyType](./literals.md#notebookinstancesortkeytype) 
2. See [:material-code-brackets: NotebookInstanceSortOrderType](./literals.md#notebookinstancesortordertype) 
3. See [:material-code-brackets: NotebookInstanceStatusType](./literals.md#notebookinstancestatustype) 
## ListPipelineExecutionsRequestRequestTypeDef

```python
# ListPipelineExecutionsRequestRequestTypeDef definition

class ListPipelineExecutionsRequestRequestTypeDef(TypedDict):
    PipelineName: str,
    CreatedAfter: NotRequired[Union[datetime, str]],
    CreatedBefore: NotRequired[Union[datetime, str]],
    SortBy: NotRequired[SortPipelineExecutionsByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: SortPipelineExecutionsByType](./literals.md#sortpipelineexecutionsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListPipelinesRequestRequestTypeDef

```python
# ListPipelinesRequestRequestTypeDef definition

class ListPipelinesRequestRequestTypeDef(TypedDict):
    PipelineNamePrefix: NotRequired[str],
    CreatedAfter: NotRequired[Union[datetime, str]],
    CreatedBefore: NotRequired[Union[datetime, str]],
    SortBy: NotRequired[SortPipelinesByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: SortPipelinesByType](./literals.md#sortpipelinesbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListProcessingJobsRequestRequestTypeDef

```python
# ListProcessingJobsRequestRequestTypeDef definition

class ListProcessingJobsRequestRequestTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    NameContains: NotRequired[str],
    StatusEquals: NotRequired[ProcessingJobStatusType],  # (1)
    SortBy: NotRequired[SortByType],  # (2)
    SortOrder: NotRequired[SortOrderType],  # (3)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: ProcessingJobStatusType](./literals.md#processingjobstatustype) 
2. See [:material-code-brackets: SortByType](./literals.md#sortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListProjectsInputRequestTypeDef

```python
# ListProjectsInputRequestTypeDef definition

class ListProjectsInputRequestTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    MaxResults: NotRequired[int],
    NameContains: NotRequired[str],
    NextToken: NotRequired[str],
    SortBy: NotRequired[ProjectSortByType],  # (1)
    SortOrder: NotRequired[ProjectSortOrderType],  # (2)
```

1. See [:material-code-brackets: ProjectSortByType](./literals.md#projectsortbytype) 
2. See [:material-code-brackets: ProjectSortOrderType](./literals.md#projectsortordertype) 
## ListResourceCatalogsRequestRequestTypeDef

```python
# ListResourceCatalogsRequestRequestTypeDef definition

class ListResourceCatalogsRequestRequestTypeDef(TypedDict):
    NameContains: NotRequired[str],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    SortOrder: NotRequired[ResourceCatalogSortOrderType],  # (1)
    SortBy: NotRequired[ResourceCatalogSortByType],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ResourceCatalogSortOrderType](./literals.md#resourcecatalogsortordertype) 
2. See [:material-code-brackets: ResourceCatalogSortByType](./literals.md#resourcecatalogsortbytype) 
## ListStudioLifecycleConfigsRequestRequestTypeDef

```python
# ListStudioLifecycleConfigsRequestRequestTypeDef definition

class ListStudioLifecycleConfigsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    NameContains: NotRequired[str],
    AppTypeEquals: NotRequired[StudioLifecycleConfigAppTypeType],  # (1)
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    ModifiedTimeBefore: NotRequired[Union[datetime, str]],
    ModifiedTimeAfter: NotRequired[Union[datetime, str]],
    SortBy: NotRequired[StudioLifecycleConfigSortKeyType],  # (2)
    SortOrder: NotRequired[SortOrderType],  # (3)
```

1. See [:material-code-brackets: StudioLifecycleConfigAppTypeType](./literals.md#studiolifecycleconfigapptypetype) 
2. See [:material-code-brackets: StudioLifecycleConfigSortKeyType](./literals.md#studiolifecycleconfigsortkeytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListTrainingJobsRequestRequestTypeDef

```python
# ListTrainingJobsRequestRequestTypeDef definition

class ListTrainingJobsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    NameContains: NotRequired[str],
    StatusEquals: NotRequired[TrainingJobStatusType],  # (1)
    SortBy: NotRequired[SortByType],  # (2)
    SortOrder: NotRequired[SortOrderType],  # (3)
    WarmPoolStatusEquals: NotRequired[WarmPoolResourceStatusType],  # (4)
```

1. See [:material-code-brackets: TrainingJobStatusType](./literals.md#trainingjobstatustype) 
2. See [:material-code-brackets: SortByType](./literals.md#sortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-brackets: WarmPoolResourceStatusType](./literals.md#warmpoolresourcestatustype) 
## ListTransformJobsRequestRequestTypeDef

```python
# ListTransformJobsRequestRequestTypeDef definition

class ListTransformJobsRequestRequestTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    NameContains: NotRequired[str],
    StatusEquals: NotRequired[TransformJobStatusType],  # (1)
    SortBy: NotRequired[SortByType],  # (2)
    SortOrder: NotRequired[SortOrderType],  # (3)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: TransformJobStatusType](./literals.md#transformjobstatustype) 
2. See [:material-code-brackets: SortByType](./literals.md#sortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListTrialComponentsRequestRequestTypeDef

```python
# ListTrialComponentsRequestRequestTypeDef definition

class ListTrialComponentsRequestRequestTypeDef(TypedDict):
    ExperimentName: NotRequired[str],
    TrialName: NotRequired[str],
    SourceArn: NotRequired[str],
    CreatedAfter: NotRequired[Union[datetime, str]],
    CreatedBefore: NotRequired[Union[datetime, str]],
    SortBy: NotRequired[SortTrialComponentsByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: SortTrialComponentsByType](./literals.md#sorttrialcomponentsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListTrialsRequestRequestTypeDef

```python
# ListTrialsRequestRequestTypeDef definition

class ListTrialsRequestRequestTypeDef(TypedDict):
    ExperimentName: NotRequired[str],
    TrialComponentName: NotRequired[str],
    CreatedAfter: NotRequired[Union[datetime, str]],
    CreatedBefore: NotRequired[Union[datetime, str]],
    SortBy: NotRequired[SortTrialsByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: SortTrialsByType](./literals.md#sorttrialsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## QueryFiltersTypeDef

```python
# QueryFiltersTypeDef definition

class QueryFiltersTypeDef(TypedDict):
    Types: NotRequired[Sequence[str]],
    LineageTypes: NotRequired[Sequence[LineageTypeType]],  # (1)
    CreatedBefore: NotRequired[Union[datetime, str]],
    CreatedAfter: NotRequired[Union[datetime, str]],
    ModifiedBefore: NotRequired[Union[datetime, str]],
    ModifiedAfter: NotRequired[Union[datetime, str]],
    Properties: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: LineageTypeType](./literals.md#lineagetypetype) 
## CreateTrialComponentRequestRequestTypeDef

```python
# CreateTrialComponentRequestRequestTypeDef definition

class CreateTrialComponentRequestRequestTypeDef(TypedDict):
    TrialComponentName: str,
    DisplayName: NotRequired[str],
    Status: NotRequired[TrialComponentStatusTypeDef],  # (1)
    StartTime: NotRequired[Union[datetime, str]],
    EndTime: NotRequired[Union[datetime, str]],
    Parameters: NotRequired[Mapping[str, TrialComponentParameterValueTypeDef]],  # (2)
    InputArtifacts: NotRequired[Mapping[str, TrialComponentArtifactTypeDef]],  # (3)
    OutputArtifacts: NotRequired[Mapping[str, TrialComponentArtifactTypeDef]],  # (3)
    MetadataProperties: NotRequired[MetadataPropertiesTypeDef],  # (5)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (6)
```

1. See [:material-code-braces: TrialComponentStatusTypeDef](./type_defs.md#trialcomponentstatustypedef) 
2. See [:material-code-braces: TrialComponentParameterValueTypeDef](./type_defs.md#trialcomponentparametervaluetypedef) 
3. See [:material-code-braces: TrialComponentArtifactTypeDef](./type_defs.md#trialcomponentartifacttypedef) 
4. See [:material-code-braces: TrialComponentArtifactTypeDef](./type_defs.md#trialcomponentartifacttypedef) 
5. See [:material-code-braces: MetadataPropertiesTypeDef](./type_defs.md#metadatapropertiestypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateTrialComponentRequestRequestTypeDef

```python
# UpdateTrialComponentRequestRequestTypeDef definition

class UpdateTrialComponentRequestRequestTypeDef(TypedDict):
    TrialComponentName: str,
    DisplayName: NotRequired[str],
    Status: NotRequired[TrialComponentStatusTypeDef],  # (1)
    StartTime: NotRequired[Union[datetime, str]],
    EndTime: NotRequired[Union[datetime, str]],
    Parameters: NotRequired[Mapping[str, TrialComponentParameterValueTypeDef]],  # (2)
    ParametersToRemove: NotRequired[Sequence[str]],
    InputArtifacts: NotRequired[Mapping[str, TrialComponentArtifactTypeDef]],  # (3)
    InputArtifactsToRemove: NotRequired[Sequence[str]],
    OutputArtifacts: NotRequired[Mapping[str, TrialComponentArtifactTypeDef]],  # (3)
    OutputArtifactsToRemove: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: TrialComponentStatusTypeDef](./type_defs.md#trialcomponentstatustypedef) 
2. See [:material-code-braces: TrialComponentParameterValueTypeDef](./type_defs.md#trialcomponentparametervaluetypedef) 
3. See [:material-code-braces: TrialComponentArtifactTypeDef](./type_defs.md#trialcomponentartifacttypedef) 
4. See [:material-code-braces: TrialComponentArtifactTypeDef](./type_defs.md#trialcomponentartifacttypedef) 
## CreateWorkforceRequestRequestTypeDef

```python
# CreateWorkforceRequestRequestTypeDef definition

class CreateWorkforceRequestRequestTypeDef(TypedDict):
    WorkforceName: str,
    CognitoConfig: NotRequired[CognitoConfigTypeDef],  # (1)
    OidcConfig: NotRequired[OidcConfigTypeDef],  # (2)
    SourceIpConfig: NotRequired[SourceIpConfigTypeDef],  # (3)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
    WorkforceVpcConfig: NotRequired[WorkforceVpcConfigRequestTypeDef],  # (5)
```

1. See [:material-code-braces: CognitoConfigTypeDef](./type_defs.md#cognitoconfigtypedef) 
2. See [:material-code-braces: OidcConfigTypeDef](./type_defs.md#oidcconfigtypedef) 
3. See [:material-code-braces: SourceIpConfigTypeDef](./type_defs.md#sourceipconfigtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: WorkforceVpcConfigRequestTypeDef](./type_defs.md#workforcevpcconfigrequesttypedef) 
## UpdateWorkforceRequestRequestTypeDef

```python
# UpdateWorkforceRequestRequestTypeDef definition

class UpdateWorkforceRequestRequestTypeDef(TypedDict):
    WorkforceName: str,
    SourceIpConfig: NotRequired[SourceIpConfigTypeDef],  # (1)
    OidcConfig: NotRequired[OidcConfigTypeDef],  # (2)
    WorkforceVpcConfig: NotRequired[WorkforceVpcConfigRequestTypeDef],  # (3)
```

1. See [:material-code-braces: SourceIpConfigTypeDef](./type_defs.md#sourceipconfigtypedef) 
2. See [:material-code-braces: OidcConfigTypeDef](./type_defs.md#oidcconfigtypedef) 
3. See [:material-code-braces: WorkforceVpcConfigRequestTypeDef](./type_defs.md#workforcevpcconfigrequesttypedef) 
## KernelGatewayAppSettingsTypeDef

```python
# KernelGatewayAppSettingsTypeDef definition

class KernelGatewayAppSettingsTypeDef(TypedDict):
    DefaultResourceSpec: NotRequired[ResourceSpecTypeDef],  # (1)
    CustomImages: NotRequired[Sequence[CustomImageTypeDef]],  # (2)
    LifecycleConfigArns: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: ResourceSpecTypeDef](./type_defs.md#resourcespectypedef) 
2. See [:material-code-braces: CustomImageTypeDef](./type_defs.md#customimagetypedef) 
## RSessionAppSettingsTypeDef

```python
# RSessionAppSettingsTypeDef definition

class RSessionAppSettingsTypeDef(TypedDict):
    DefaultResourceSpec: NotRequired[ResourceSpecTypeDef],  # (1)
    CustomImages: NotRequired[Sequence[CustomImageTypeDef]],  # (2)
```

1. See [:material-code-braces: ResourceSpecTypeDef](./type_defs.md#resourcespectypedef) 
2. See [:material-code-braces: CustomImageTypeDef](./type_defs.md#customimagetypedef) 
## ModelBiasBaselineConfigTypeDef

```python
# ModelBiasBaselineConfigTypeDef definition

class ModelBiasBaselineConfigTypeDef(TypedDict):
    BaseliningJobName: NotRequired[str],
    ConstraintsResource: NotRequired[MonitoringConstraintsResourceTypeDef],  # (1)
```

1. See [:material-code-braces: MonitoringConstraintsResourceTypeDef](./type_defs.md#monitoringconstraintsresourcetypedef) 
## ModelExplainabilityBaselineConfigTypeDef

```python
# ModelExplainabilityBaselineConfigTypeDef definition

class ModelExplainabilityBaselineConfigTypeDef(TypedDict):
    BaseliningJobName: NotRequired[str],
    ConstraintsResource: NotRequired[MonitoringConstraintsResourceTypeDef],  # (1)
```

1. See [:material-code-braces: MonitoringConstraintsResourceTypeDef](./type_defs.md#monitoringconstraintsresourcetypedef) 
## ModelQualityBaselineConfigTypeDef

```python
# ModelQualityBaselineConfigTypeDef definition

class ModelQualityBaselineConfigTypeDef(TypedDict):
    BaseliningJobName: NotRequired[str],
    ConstraintsResource: NotRequired[MonitoringConstraintsResourceTypeDef],  # (1)
```

1. See [:material-code-braces: MonitoringConstraintsResourceTypeDef](./type_defs.md#monitoringconstraintsresourcetypedef) 
## DataQualityBaselineConfigTypeDef

```python
# DataQualityBaselineConfigTypeDef definition

class DataQualityBaselineConfigTypeDef(TypedDict):
    BaseliningJobName: NotRequired[str],
    ConstraintsResource: NotRequired[MonitoringConstraintsResourceTypeDef],  # (1)
    StatisticsResource: NotRequired[MonitoringStatisticsResourceTypeDef],  # (2)
```

1. See [:material-code-braces: MonitoringConstraintsResourceTypeDef](./type_defs.md#monitoringconstraintsresourcetypedef) 
2. See [:material-code-braces: MonitoringStatisticsResourceTypeDef](./type_defs.md#monitoringstatisticsresourcetypedef) 
## MonitoringBaselineConfigTypeDef

```python
# MonitoringBaselineConfigTypeDef definition

class MonitoringBaselineConfigTypeDef(TypedDict):
    BaseliningJobName: NotRequired[str],
    ConstraintsResource: NotRequired[MonitoringConstraintsResourceTypeDef],  # (1)
    StatisticsResource: NotRequired[MonitoringStatisticsResourceTypeDef],  # (2)
```

1. See [:material-code-braces: MonitoringConstraintsResourceTypeDef](./type_defs.md#monitoringconstraintsresourcetypedef) 
2. See [:material-code-braces: MonitoringStatisticsResourceTypeDef](./type_defs.md#monitoringstatisticsresourcetypedef) 
## DataSourceTypeDef

```python
# DataSourceTypeDef definition

class DataSourceTypeDef(TypedDict):
    S3DataSource: NotRequired[S3DataSourceTypeDef],  # (1)
    FileSystemDataSource: NotRequired[FileSystemDataSourceTypeDef],  # (2)
```

1. See [:material-code-braces: S3DataSourceTypeDef](./type_defs.md#s3datasourcetypedef) 
2. See [:material-code-braces: FileSystemDataSourceTypeDef](./type_defs.md#filesystemdatasourcetypedef) 
## DatasetDefinitionTypeDef

```python
# DatasetDefinitionTypeDef definition

class DatasetDefinitionTypeDef(TypedDict):
    AthenaDatasetDefinition: NotRequired[AthenaDatasetDefinitionTypeDef],  # (1)
    RedshiftDatasetDefinition: NotRequired[RedshiftDatasetDefinitionTypeDef],  # (2)
    LocalPath: NotRequired[str],
    DataDistributionType: NotRequired[DataDistributionTypeType],  # (3)
    InputMode: NotRequired[InputModeType],  # (4)
```

1. See [:material-code-braces: AthenaDatasetDefinitionTypeDef](./type_defs.md#athenadatasetdefinitiontypedef) 
2. See [:material-code-braces: RedshiftDatasetDefinitionTypeDef](./type_defs.md#redshiftdatasetdefinitiontypedef) 
3. See [:material-code-brackets: DataDistributionTypeType](./literals.md#datadistributiontypetype) 
4. See [:material-code-brackets: InputModeType](./literals.md#inputmodetype) 
## DeleteDomainRequestRequestTypeDef

```python
# DeleteDomainRequestRequestTypeDef definition

class DeleteDomainRequestRequestTypeDef(TypedDict):
    DomainId: str,
    RetentionPolicy: NotRequired[RetentionPolicyTypeDef],  # (1)
```

1. See [:material-code-braces: RetentionPolicyTypeDef](./type_defs.md#retentionpolicytypedef) 
## DeploymentRecommendationTypeDef

```python
# DeploymentRecommendationTypeDef definition

class DeploymentRecommendationTypeDef(TypedDict):
    RecommendationStatus: RecommendationStatusType,  # (1)
    RealTimeInferenceRecommendations: NotRequired[List[RealTimeInferenceRecommendationTypeDef]],  # (2)
```

1. See [:material-code-brackets: RecommendationStatusType](./literals.md#recommendationstatustype) 
2. See [:material-code-braces: RealTimeInferenceRecommendationTypeDef](./type_defs.md#realtimeinferencerecommendationtypedef) 
## DeploymentStageTypeDef

```python
# DeploymentStageTypeDef definition

class DeploymentStageTypeDef(TypedDict):
    StageName: str,
    DeviceSelectionConfig: DeviceSelectionConfigTypeDef,  # (1)
    DeploymentConfig: NotRequired[EdgeDeploymentConfigTypeDef],  # (2)
```

1. See [:material-code-braces: DeviceSelectionConfigTypeDef](./type_defs.md#deviceselectionconfigtypedef) 
2. See [:material-code-braces: EdgeDeploymentConfigTypeDef](./type_defs.md#edgedeploymentconfigtypedef) 
## DeploymentStageStatusSummaryTypeDef

```python
# DeploymentStageStatusSummaryTypeDef definition

class DeploymentStageStatusSummaryTypeDef(TypedDict):
    StageName: str,
    DeviceSelectionConfig: DeviceSelectionConfigTypeDef,  # (1)
    DeploymentConfig: EdgeDeploymentConfigTypeDef,  # (2)
    DeploymentStatus: EdgeDeploymentStatusTypeDef,  # (3)
```

1. See [:material-code-braces: DeviceSelectionConfigTypeDef](./type_defs.md#deviceselectionconfigtypedef) 
2. See [:material-code-braces: EdgeDeploymentConfigTypeDef](./type_defs.md#edgedeploymentconfigtypedef) 
3. See [:material-code-braces: EdgeDeploymentStatusTypeDef](./type_defs.md#edgedeploymentstatustypedef) 
## DescribeDeviceResponseTypeDef

```python
# DescribeDeviceResponseTypeDef definition

class DescribeDeviceResponseTypeDef(TypedDict):
    DeviceArn: str,
    DeviceName: str,
    Description: str,
    DeviceFleetName: str,
    IotThingName: str,
    RegistrationTime: datetime,
    LatestHeartbeat: datetime,
    Models: List[EdgeModelTypeDef],  # (1)
    MaxModels: int,
    NextToken: str,
    AgentVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EdgeModelTypeDef](./type_defs.md#edgemodeltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEdgePackagingJobResponseTypeDef

```python
# DescribeEdgePackagingJobResponseTypeDef definition

class DescribeEdgePackagingJobResponseTypeDef(TypedDict):
    EdgePackagingJobArn: str,
    EdgePackagingJobName: str,
    CompilationJobName: str,
    ModelName: str,
    ModelVersion: str,
    RoleArn: str,
    OutputConfig: EdgeOutputConfigTypeDef,  # (1)
    ResourceKey: str,
    EdgePackagingJobStatus: EdgePackagingJobStatusType,  # (2)
    EdgePackagingJobStatusMessage: str,
    CreationTime: datetime,
    LastModifiedTime: datetime,
    ModelArtifact: str,
    ModelSignature: str,
    PresetDeploymentOutput: EdgePresetDeploymentOutputTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: EdgeOutputConfigTypeDef](./type_defs.md#edgeoutputconfigtypedef) 
2. See [:material-code-brackets: EdgePackagingJobStatusType](./literals.md#edgepackagingjobstatustype) 
3. See [:material-code-braces: EdgePresetDeploymentOutputTypeDef](./type_defs.md#edgepresetdeploymentoutputtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEndpointInputEndpointDeletedWaitTypeDef

```python
# DescribeEndpointInputEndpointDeletedWaitTypeDef definition

class DescribeEndpointInputEndpointDeletedWaitTypeDef(TypedDict):
    EndpointName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeEndpointInputEndpointInServiceWaitTypeDef

```python
# DescribeEndpointInputEndpointInServiceWaitTypeDef definition

class DescribeEndpointInputEndpointInServiceWaitTypeDef(TypedDict):
    EndpointName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeImageRequestImageCreatedWaitTypeDef

```python
# DescribeImageRequestImageCreatedWaitTypeDef definition

class DescribeImageRequestImageCreatedWaitTypeDef(TypedDict):
    ImageName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeImageRequestImageDeletedWaitTypeDef

```python
# DescribeImageRequestImageDeletedWaitTypeDef definition

class DescribeImageRequestImageDeletedWaitTypeDef(TypedDict):
    ImageName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeImageRequestImageUpdatedWaitTypeDef

```python
# DescribeImageRequestImageUpdatedWaitTypeDef definition

class DescribeImageRequestImageUpdatedWaitTypeDef(TypedDict):
    ImageName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeImageVersionRequestImageVersionCreatedWaitTypeDef

```python
# DescribeImageVersionRequestImageVersionCreatedWaitTypeDef definition

class DescribeImageVersionRequestImageVersionCreatedWaitTypeDef(TypedDict):
    ImageName: str,
    Version: NotRequired[int],
    Alias: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeImageVersionRequestImageVersionDeletedWaitTypeDef

```python
# DescribeImageVersionRequestImageVersionDeletedWaitTypeDef definition

class DescribeImageVersionRequestImageVersionDeletedWaitTypeDef(TypedDict):
    ImageName: str,
    Version: NotRequired[int],
    Alias: NotRequired[str],
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeNotebookInstanceInputNotebookInstanceDeletedWaitTypeDef

```python
# DescribeNotebookInstanceInputNotebookInstanceDeletedWaitTypeDef definition

class DescribeNotebookInstanceInputNotebookInstanceDeletedWaitTypeDef(TypedDict):
    NotebookInstanceName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeNotebookInstanceInputNotebookInstanceInServiceWaitTypeDef

```python
# DescribeNotebookInstanceInputNotebookInstanceInServiceWaitTypeDef definition

class DescribeNotebookInstanceInputNotebookInstanceInServiceWaitTypeDef(TypedDict):
    NotebookInstanceName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeNotebookInstanceInputNotebookInstanceStoppedWaitTypeDef

```python
# DescribeNotebookInstanceInputNotebookInstanceStoppedWaitTypeDef definition

class DescribeNotebookInstanceInputNotebookInstanceStoppedWaitTypeDef(TypedDict):
    NotebookInstanceName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeProcessingJobRequestProcessingJobCompletedOrStoppedWaitTypeDef

```python
# DescribeProcessingJobRequestProcessingJobCompletedOrStoppedWaitTypeDef definition

class DescribeProcessingJobRequestProcessingJobCompletedOrStoppedWaitTypeDef(TypedDict):
    ProcessingJobName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeTrainingJobRequestTrainingJobCompletedOrStoppedWaitTypeDef

```python
# DescribeTrainingJobRequestTrainingJobCompletedOrStoppedWaitTypeDef definition

class DescribeTrainingJobRequestTrainingJobCompletedOrStoppedWaitTypeDef(TypedDict):
    TrainingJobName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeTransformJobRequestTransformJobCompletedOrStoppedWaitTypeDef

```python
# DescribeTransformJobRequestTransformJobCompletedOrStoppedWaitTypeDef definition

class DescribeTransformJobRequestTransformJobCompletedOrStoppedWaitTypeDef(TypedDict):
    TransformJobName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## ExperimentSummaryTypeDef

```python
# ExperimentSummaryTypeDef definition

class ExperimentSummaryTypeDef(TypedDict):
    ExperimentArn: NotRequired[str],
    ExperimentName: NotRequired[str],
    DisplayName: NotRequired[str],
    ExperimentSource: NotRequired[ExperimentSourceTypeDef],  # (1)
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
```

1. See [:material-code-braces: ExperimentSourceTypeDef](./type_defs.md#experimentsourcetypedef) 
## FeatureGroupSummaryTypeDef

```python
# FeatureGroupSummaryTypeDef definition

class FeatureGroupSummaryTypeDef(TypedDict):
    FeatureGroupName: str,
    FeatureGroupArn: str,
    CreationTime: datetime,
    FeatureGroupStatus: NotRequired[FeatureGroupStatusType],  # (1)
    OfflineStoreStatus: NotRequired[OfflineStoreStatusTypeDef],  # (2)
```

1. See [:material-code-brackets: FeatureGroupStatusType](./literals.md#featuregroupstatustype) 
2. See [:material-code-braces: OfflineStoreStatusTypeDef](./type_defs.md#offlinestorestatustypedef) 
## DescribeFeatureMetadataResponseTypeDef

```python
# DescribeFeatureMetadataResponseTypeDef definition

class DescribeFeatureMetadataResponseTypeDef(TypedDict):
    FeatureGroupArn: str,
    FeatureGroupName: str,
    FeatureName: str,
    FeatureType: FeatureTypeType,  # (1)
    CreationTime: datetime,
    LastModifiedTime: datetime,
    Description: str,
    Parameters: List[FeatureParameterTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: FeatureTypeType](./literals.md#featuretypetype) 
2. See [:material-code-braces: FeatureParameterTypeDef](./type_defs.md#featureparametertypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FeatureMetadataTypeDef

```python
# FeatureMetadataTypeDef definition

class FeatureMetadataTypeDef(TypedDict):
    FeatureGroupArn: NotRequired[str],
    FeatureGroupName: NotRequired[str],
    FeatureName: NotRequired[str],
    FeatureType: NotRequired[FeatureTypeType],  # (1)
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
    Description: NotRequired[str],
    Parameters: NotRequired[List[FeatureParameterTypeDef]],  # (2)
```

1. See [:material-code-brackets: FeatureTypeType](./literals.md#featuretypetype) 
2. See [:material-code-braces: FeatureParameterTypeDef](./type_defs.md#featureparametertypedef) 
## UpdateFeatureMetadataRequestRequestTypeDef

```python
# UpdateFeatureMetadataRequestRequestTypeDef definition

class UpdateFeatureMetadataRequestRequestTypeDef(TypedDict):
    FeatureGroupName: str,
    FeatureName: str,
    Description: NotRequired[str],
    ParameterAdditions: NotRequired[Sequence[FeatureParameterTypeDef]],  # (1)
    ParameterRemovals: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: FeatureParameterTypeDef](./type_defs.md#featureparametertypedef) 
## DescribeHubContentResponseTypeDef

```python
# DescribeHubContentResponseTypeDef definition

class DescribeHubContentResponseTypeDef(TypedDict):
    HubContentName: str,
    HubContentArn: str,
    HubContentVersion: str,
    HubContentType: HubContentTypeType,  # (1)
    DocumentSchemaVersion: str,
    HubName: str,
    HubArn: str,
    HubContentDisplayName: str,
    HubContentDescription: str,
    HubContentMarkdown: str,
    HubContentDocument: str,
    HubContentSearchKeywords: List[str],
    HubContentDependencies: List[HubContentDependencyTypeDef],  # (2)
    HubContentStatus: HubContentStatusType,  # (3)
    FailureReason: str,
    CreationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: HubContentTypeType](./literals.md#hubcontenttypetype) 
2. See [:material-code-braces: HubContentDependencyTypeDef](./type_defs.md#hubcontentdependencytypedef) 
3. See [:material-code-brackets: HubContentStatusType](./literals.md#hubcontentstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeHumanTaskUiResponseTypeDef

```python
# DescribeHumanTaskUiResponseTypeDef definition

class DescribeHumanTaskUiResponseTypeDef(TypedDict):
    HumanTaskUiArn: str,
    HumanTaskUiName: str,
    HumanTaskUiStatus: HumanTaskUiStatusType,  # (1)
    CreationTime: datetime,
    UiTemplate: UiTemplateInfoTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: HumanTaskUiStatusType](./literals.md#humantaskuistatustype) 
2. See [:material-code-braces: UiTemplateInfoTypeDef](./type_defs.md#uitemplateinfotypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeModelCardExportJobResponseTypeDef

```python
# DescribeModelCardExportJobResponseTypeDef definition

class DescribeModelCardExportJobResponseTypeDef(TypedDict):
    ModelCardExportJobName: str,
    ModelCardExportJobArn: str,
    Status: ModelCardExportJobStatusType,  # (1)
    ModelCardName: str,
    ModelCardVersion: int,
    OutputConfig: ModelCardExportOutputConfigTypeDef,  # (2)
    CreatedAt: datetime,
    LastModifiedAt: datetime,
    FailureReason: str,
    ExportArtifacts: ModelCardExportArtifactsTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: ModelCardExportJobStatusType](./literals.md#modelcardexportjobstatustype) 
2. See [:material-code-braces: ModelCardExportOutputConfigTypeDef](./type_defs.md#modelcardexportoutputconfigtypedef) 
3. See [:material-code-braces: ModelCardExportArtifactsTypeDef](./type_defs.md#modelcardexportartifactstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMonitoringExecutionsResponseTypeDef

```python
# ListMonitoringExecutionsResponseTypeDef definition

class ListMonitoringExecutionsResponseTypeDef(TypedDict):
    MonitoringExecutionSummaries: List[MonitoringExecutionSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MonitoringExecutionSummaryTypeDef](./type_defs.md#monitoringexecutionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSubscribedWorkteamResponseTypeDef

```python
# DescribeSubscribedWorkteamResponseTypeDef definition

class DescribeSubscribedWorkteamResponseTypeDef(TypedDict):
    SubscribedWorkteam: SubscribedWorkteamTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SubscribedWorkteamTypeDef](./type_defs.md#subscribedworkteamtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSubscribedWorkteamsResponseTypeDef

```python
# ListSubscribedWorkteamsResponseTypeDef definition

class ListSubscribedWorkteamsResponseTypeDef(TypedDict):
    SubscribedWorkteams: List[SubscribedWorkteamTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SubscribedWorkteamTypeDef](./type_defs.md#subscribedworkteamtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TrainingJobSummaryTypeDef

```python
# TrainingJobSummaryTypeDef definition

class TrainingJobSummaryTypeDef(TypedDict):
    TrainingJobName: str,
    TrainingJobArn: str,
    CreationTime: datetime,
    TrainingJobStatus: TrainingJobStatusType,  # (1)
    TrainingEndTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
    WarmPoolStatus: NotRequired[WarmPoolStatusTypeDef],  # (2)
```

1. See [:material-code-brackets: TrainingJobStatusType](./literals.md#trainingjobstatustype) 
2. See [:material-code-braces: WarmPoolStatusTypeDef](./type_defs.md#warmpoolstatustypedef) 
## TrialSummaryTypeDef

```python
# TrialSummaryTypeDef definition

class TrialSummaryTypeDef(TypedDict):
    TrialArn: NotRequired[str],
    TrialName: NotRequired[str],
    DisplayName: NotRequired[str],
    TrialSource: NotRequired[TrialSourceTypeDef],  # (1)
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
```

1. See [:material-code-braces: TrialSourceTypeDef](./type_defs.md#trialsourcetypedef) 
## DesiredWeightAndCapacityTypeDef

```python
# DesiredWeightAndCapacityTypeDef definition

class DesiredWeightAndCapacityTypeDef(TypedDict):
    VariantName: str,
    DesiredWeight: NotRequired[float],
    DesiredInstanceCount: NotRequired[int],
    ServerlessUpdateConfig: NotRequired[ProductionVariantServerlessUpdateConfigTypeDef],  # (1)
```

1. See [:material-code-braces: ProductionVariantServerlessUpdateConfigTypeDef](./type_defs.md#productionvariantserverlessupdateconfigtypedef) 
## ListStageDevicesResponseTypeDef

```python
# ListStageDevicesResponseTypeDef definition

class ListStageDevicesResponseTypeDef(TypedDict):
    DeviceDeploymentSummaries: List[DeviceDeploymentSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeviceDeploymentSummaryTypeDef](./type_defs.md#devicedeploymentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDeviceFleetsResponseTypeDef

```python
# ListDeviceFleetsResponseTypeDef definition

class ListDeviceFleetsResponseTypeDef(TypedDict):
    DeviceFleetSummaries: List[DeviceFleetSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeviceFleetSummaryTypeDef](./type_defs.md#devicefleetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeviceSummaryTypeDef

```python
# DeviceSummaryTypeDef definition

class DeviceSummaryTypeDef(TypedDict):
    DeviceName: str,
    DeviceArn: str,
    Description: NotRequired[str],
    DeviceFleetName: NotRequired[str],
    IotThingName: NotRequired[str],
    RegistrationTime: NotRequired[datetime],
    LatestHeartbeat: NotRequired[datetime],
    Models: NotRequired[List[EdgeModelSummaryTypeDef]],  # (1)
    AgentVersion: NotRequired[str],
```

1. See [:material-code-braces: EdgeModelSummaryTypeDef](./type_defs.md#edgemodelsummarytypedef) 
## RegisterDevicesRequestRequestTypeDef

```python
# RegisterDevicesRequestRequestTypeDef definition

class RegisterDevicesRequestRequestTypeDef(TypedDict):
    DeviceFleetName: str,
    Devices: Sequence[DeviceTypeDef],  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: DeviceTypeDef](./type_defs.md#devicetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateDevicesRequestRequestTypeDef

```python
# UpdateDevicesRequestRequestTypeDef definition

class UpdateDevicesRequestRequestTypeDef(TypedDict):
    DeviceFleetName: str,
    Devices: Sequence[DeviceTypeDef],  # (1)
```

1. See [:material-code-braces: DeviceTypeDef](./type_defs.md#devicetypedef) 
## ListDomainsResponseTypeDef

```python
# ListDomainsResponseTypeDef definition

class ListDomainsResponseTypeDef(TypedDict):
    Domains: List[DomainDetailsTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainDetailsTypeDef](./type_defs.md#domaindetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DriftCheckBiasTypeDef

```python
# DriftCheckBiasTypeDef definition

class DriftCheckBiasTypeDef(TypedDict):
    ConfigFile: NotRequired[FileSourceTypeDef],  # (1)
    PreTrainingConstraints: NotRequired[MetricsSourceTypeDef],  # (2)
    PostTrainingConstraints: NotRequired[MetricsSourceTypeDef],  # (2)
```

1. See [:material-code-braces: FileSourceTypeDef](./type_defs.md#filesourcetypedef) 
2. See [:material-code-braces: MetricsSourceTypeDef](./type_defs.md#metricssourcetypedef) 
3. See [:material-code-braces: MetricsSourceTypeDef](./type_defs.md#metricssourcetypedef) 
## DriftCheckExplainabilityTypeDef

```python
# DriftCheckExplainabilityTypeDef definition

class DriftCheckExplainabilityTypeDef(TypedDict):
    Constraints: NotRequired[MetricsSourceTypeDef],  # (1)
    ConfigFile: NotRequired[FileSourceTypeDef],  # (2)
```

1. See [:material-code-braces: MetricsSourceTypeDef](./type_defs.md#metricssourcetypedef) 
2. See [:material-code-braces: FileSourceTypeDef](./type_defs.md#filesourcetypedef) 
## ListEdgeDeploymentPlansResponseTypeDef

```python
# ListEdgeDeploymentPlansResponseTypeDef definition

class ListEdgeDeploymentPlansResponseTypeDef(TypedDict):
    EdgeDeploymentPlanSummaries: List[EdgeDeploymentPlanSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EdgeDeploymentPlanSummaryTypeDef](./type_defs.md#edgedeploymentplansummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDeviceFleetReportResponseTypeDef

```python
# GetDeviceFleetReportResponseTypeDef definition

class GetDeviceFleetReportResponseTypeDef(TypedDict):
    DeviceFleetArn: str,
    DeviceFleetName: str,
    OutputConfig: EdgeOutputConfigTypeDef,  # (1)
    Description: str,
    ReportGenerated: datetime,
    DeviceStats: DeviceStatsTypeDef,  # (2)
    AgentVersions: List[AgentVersionTypeDef],  # (3)
    ModelStats: List[EdgeModelStatTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: EdgeOutputConfigTypeDef](./type_defs.md#edgeoutputconfigtypedef) 
2. See [:material-code-braces: DeviceStatsTypeDef](./type_defs.md#devicestatstypedef) 
3. See [:material-code-braces: AgentVersionTypeDef](./type_defs.md#agentversiontypedef) 
4. See [:material-code-braces: EdgeModelStatTypeDef](./type_defs.md#edgemodelstattypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEdgePackagingJobsResponseTypeDef

```python
# ListEdgePackagingJobsResponseTypeDef definition

class ListEdgePackagingJobsResponseTypeDef(TypedDict):
    EdgePackagingJobSummaries: List[EdgePackagingJobSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EdgePackagingJobSummaryTypeDef](./type_defs.md#edgepackagingjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEndpointConfigsOutputTypeDef

```python
# ListEndpointConfigsOutputTypeDef definition

class ListEndpointConfigsOutputTypeDef(TypedDict):
    EndpointConfigs: List[EndpointConfigSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointConfigSummaryTypeDef](./type_defs.md#endpointconfigsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EndpointOutputConfigurationTypeDef

```python
# EndpointOutputConfigurationTypeDef definition

class EndpointOutputConfigurationTypeDef(TypedDict):
    EndpointName: str,
    VariantName: str,
    InstanceType: NotRequired[ProductionVariantInstanceTypeType],  # (1)
    InitialInstanceCount: NotRequired[int],
    ServerlessConfig: NotRequired[ProductionVariantServerlessConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ProductionVariantInstanceTypeType](./literals.md#productionvariantinstancetypetype) 
2. See [:material-code-braces: ProductionVariantServerlessConfigTypeDef](./type_defs.md#productionvariantserverlessconfigtypedef) 
## EndpointPerformanceTypeDef

```python
# EndpointPerformanceTypeDef definition

class EndpointPerformanceTypeDef(TypedDict):
    Metrics: InferenceMetricsTypeDef,  # (1)
    EndpointInfo: EndpointInfoTypeDef,  # (2)
```

1. See [:material-code-braces: InferenceMetricsTypeDef](./type_defs.md#inferencemetricstypedef) 
2. See [:material-code-braces: EndpointInfoTypeDef](./type_defs.md#endpointinfotypedef) 
## ListEndpointsOutputTypeDef

```python
# ListEndpointsOutputTypeDef definition

class ListEndpointsOutputTypeDef(TypedDict):
    Endpoints: List[EndpointSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointSummaryTypeDef](./type_defs.md#endpointsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModelConfigurationTypeDef

```python
# ModelConfigurationTypeDef definition

class ModelConfigurationTypeDef(TypedDict):
    InferenceSpecificationName: NotRequired[str],
    EnvironmentParameters: NotRequired[List[EnvironmentParameterTypeDef]],  # (1)
    CompilationJobName: NotRequired[str],
```

1. See [:material-code-braces: EnvironmentParameterTypeDef](./type_defs.md#environmentparametertypedef) 
## NestedFiltersTypeDef

```python
# NestedFiltersTypeDef definition

class NestedFiltersTypeDef(TypedDict):
    NestedPropertyName: str,
    Filters: Sequence[FilterTypeDef],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## HyperParameterTrainingJobSummaryTypeDef

```python
# HyperParameterTrainingJobSummaryTypeDef definition

class HyperParameterTrainingJobSummaryTypeDef(TypedDict):
    TrainingJobName: str,
    TrainingJobArn: str,
    CreationTime: datetime,
    TrainingJobStatus: TrainingJobStatusType,  # (1)
    TunedHyperParameters: Dict[str, str],
    TrainingJobDefinitionName: NotRequired[str],
    TuningJobName: NotRequired[str],
    TrainingStartTime: NotRequired[datetime],
    TrainingEndTime: NotRequired[datetime],
    FailureReason: NotRequired[str],
    FinalHyperParameterTuningJobObjectiveMetric: NotRequired[FinalHyperParameterTuningJobObjectiveMetricTypeDef],  # (2)
    ObjectiveStatus: NotRequired[ObjectiveStatusType],  # (3)
```

1. See [:material-code-brackets: TrainingJobStatusType](./literals.md#trainingjobstatustype) 
2. See [:material-code-braces: FinalHyperParameterTuningJobObjectiveMetricTypeDef](./type_defs.md#finalhyperparametertuningjobobjectivemetrictypedef) 
3. See [:material-code-brackets: ObjectiveStatusType](./literals.md#objectivestatustype) 
## ListFlowDefinitionsResponseTypeDef

```python
# ListFlowDefinitionsResponseTypeDef definition

class ListFlowDefinitionsResponseTypeDef(TypedDict):
    FlowDefinitionSummaries: List[FlowDefinitionSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FlowDefinitionSummaryTypeDef](./type_defs.md#flowdefinitionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetScalingConfigurationRecommendationRequestRequestTypeDef

```python
# GetScalingConfigurationRecommendationRequestRequestTypeDef definition

class GetScalingConfigurationRecommendationRequestRequestTypeDef(TypedDict):
    InferenceRecommendationsJobName: str,
    RecommendationId: NotRequired[str],
    EndpointName: NotRequired[str],
    TargetCpuUtilizationPerCore: NotRequired[int],
    ScalingPolicyObjective: NotRequired[ScalingPolicyObjectiveTypeDef],  # (1)
```

1. See [:material-code-braces: ScalingPolicyObjectiveTypeDef](./type_defs.md#scalingpolicyobjectivetypedef) 
## GetSearchSuggestionsResponseTypeDef

```python
# GetSearchSuggestionsResponseTypeDef definition

class GetSearchSuggestionsResponseTypeDef(TypedDict):
    PropertyNameSuggestions: List[PropertyNameSuggestionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PropertyNameSuggestionTypeDef](./type_defs.md#propertynamesuggestiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCodeRepositoryInputRequestTypeDef

```python
# UpdateCodeRepositoryInputRequestTypeDef definition

class UpdateCodeRepositoryInputRequestTypeDef(TypedDict):
    CodeRepositoryName: str,
    GitConfig: NotRequired[GitConfigForUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: GitConfigForUpdateTypeDef](./type_defs.md#gitconfigforupdatetypedef) 
## ListHubContentVersionsResponseTypeDef

```python
# ListHubContentVersionsResponseTypeDef definition

class ListHubContentVersionsResponseTypeDef(TypedDict):
    HubContentSummaries: List[HubContentInfoTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HubContentInfoTypeDef](./type_defs.md#hubcontentinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListHubContentsResponseTypeDef

```python
# ListHubContentsResponseTypeDef definition

class ListHubContentsResponseTypeDef(TypedDict):
    HubContentSummaries: List[HubContentInfoTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HubContentInfoTypeDef](./type_defs.md#hubcontentinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListHubsResponseTypeDef

```python
# ListHubsResponseTypeDef definition

class ListHubsResponseTypeDef(TypedDict):
    HubSummaries: List[HubInfoTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HubInfoTypeDef](./type_defs.md#hubinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HumanLoopActivationConfigTypeDef

```python
# HumanLoopActivationConfigTypeDef definition

class HumanLoopActivationConfigTypeDef(TypedDict):
    HumanLoopActivationConditionsConfig: HumanLoopActivationConditionsConfigTypeDef,  # (1)
```

1. See [:material-code-braces: HumanLoopActivationConditionsConfigTypeDef](./type_defs.md#humanloopactivationconditionsconfigtypedef) 
## ListHumanTaskUisResponseTypeDef

```python
# ListHumanTaskUisResponseTypeDef definition

class ListHumanTaskUisResponseTypeDef(TypedDict):
    HumanTaskUiSummaries: List[HumanTaskUiSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HumanTaskUiSummaryTypeDef](./type_defs.md#humantaskuisummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HyperParameterTuningResourceConfigTypeDef

```python
# HyperParameterTuningResourceConfigTypeDef definition

class HyperParameterTuningResourceConfigTypeDef(TypedDict):
    InstanceType: NotRequired[TrainingInstanceTypeType],  # (1)
    InstanceCount: NotRequired[int],
    VolumeSizeInGB: NotRequired[int],
    VolumeKmsKeyId: NotRequired[str],
    AllocationStrategy: NotRequired[HyperParameterTuningAllocationStrategyType],  # (2)
    InstanceConfigs: NotRequired[Sequence[HyperParameterTuningInstanceConfigTypeDef]],  # (3)
```

1. See [:material-code-brackets: TrainingInstanceTypeType](./literals.md#traininginstancetypetype) 
2. See [:material-code-brackets: HyperParameterTuningAllocationStrategyType](./literals.md#hyperparametertuningallocationstrategytype) 
3. See [:material-code-braces: HyperParameterTuningInstanceConfigTypeDef](./type_defs.md#hyperparametertuninginstanceconfigtypedef) 
## HyperParameterTuningJobSummaryTypeDef

```python
# HyperParameterTuningJobSummaryTypeDef definition

class HyperParameterTuningJobSummaryTypeDef(TypedDict):
    HyperParameterTuningJobName: str,
    HyperParameterTuningJobArn: str,
    HyperParameterTuningJobStatus: HyperParameterTuningJobStatusType,  # (1)
    Strategy: HyperParameterTuningJobStrategyTypeType,  # (2)
    CreationTime: datetime,
    TrainingJobStatusCounters: TrainingJobStatusCountersTypeDef,  # (3)
    ObjectiveStatusCounters: ObjectiveStatusCountersTypeDef,  # (4)
    HyperParameterTuningEndTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
    ResourceLimits: NotRequired[ResourceLimitsTypeDef],  # (5)
```

1. See [:material-code-brackets: HyperParameterTuningJobStatusType](./literals.md#hyperparametertuningjobstatustype) 
2. See [:material-code-brackets: HyperParameterTuningJobStrategyTypeType](./literals.md#hyperparametertuningjobstrategytypetype) 
3. See [:material-code-braces: TrainingJobStatusCountersTypeDef](./type_defs.md#trainingjobstatuscounterstypedef) 
4. See [:material-code-braces: ObjectiveStatusCountersTypeDef](./type_defs.md#objectivestatuscounterstypedef) 
5. See [:material-code-braces: ResourceLimitsTypeDef](./type_defs.md#resourcelimitstypedef) 
## HyperParameterTuningJobStrategyConfigTypeDef

```python
# HyperParameterTuningJobStrategyConfigTypeDef definition

class HyperParameterTuningJobStrategyConfigTypeDef(TypedDict):
    HyperbandStrategyConfig: NotRequired[HyperbandStrategyConfigTypeDef],  # (1)
```

1. See [:material-code-braces: HyperbandStrategyConfigTypeDef](./type_defs.md#hyperbandstrategyconfigtypedef) 
## HyperParameterTuningJobWarmStartConfigTypeDef

```python
# HyperParameterTuningJobWarmStartConfigTypeDef definition

class HyperParameterTuningJobWarmStartConfigTypeDef(TypedDict):
    ParentHyperParameterTuningJobs: Sequence[ParentHyperParameterTuningJobTypeDef],  # (1)
    WarmStartType: HyperParameterTuningJobWarmStartTypeType,  # (2)
```

1. See [:material-code-braces: ParentHyperParameterTuningJobTypeDef](./type_defs.md#parenthyperparametertuningjobtypedef) 
2. See [:material-code-brackets: HyperParameterTuningJobWarmStartTypeType](./literals.md#hyperparametertuningjobwarmstarttypetype) 
## UserContextTypeDef

```python
# UserContextTypeDef definition

class UserContextTypeDef(TypedDict):
    UserProfileArn: NotRequired[str],
    UserProfileName: NotRequired[str],
    DomainId: NotRequired[str],
    IamIdentity: NotRequired[IamIdentityTypeDef],  # (1)
```

1. See [:material-code-braces: IamIdentityTypeDef](./type_defs.md#iamidentitytypedef) 
## ImageConfigTypeDef

```python
# ImageConfigTypeDef definition

class ImageConfigTypeDef(TypedDict):
    RepositoryAccessMode: RepositoryAccessModeType,  # (1)
    RepositoryAuthConfig: NotRequired[RepositoryAuthConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: RepositoryAccessModeType](./literals.md#repositoryaccessmodetype) 
2. See [:material-code-braces: RepositoryAuthConfigTypeDef](./type_defs.md#repositoryauthconfigtypedef) 
## ListImagesResponseTypeDef

```python
# ListImagesResponseTypeDef definition

class ListImagesResponseTypeDef(TypedDict):
    Images: List[ImageTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImageTypeDef](./type_defs.md#imagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListImageVersionsResponseTypeDef

```python
# ListImageVersionsResponseTypeDef definition

class ListImageVersionsResponseTypeDef(TypedDict):
    ImageVersions: List[ImageVersionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImageVersionTypeDef](./type_defs.md#imageversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInferenceRecommendationsJobsResponseTypeDef

```python
# ListInferenceRecommendationsJobsResponseTypeDef definition

class ListInferenceRecommendationsJobsResponseTypeDef(TypedDict):
    InferenceRecommendationsJobs: List[InferenceRecommendationsJobTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InferenceRecommendationsJobTypeDef](./type_defs.md#inferencerecommendationsjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResourceConfigTypeDef

```python
# ResourceConfigTypeDef definition

class ResourceConfigTypeDef(TypedDict):
    VolumeSizeInGB: int,
    InstanceType: NotRequired[TrainingInstanceTypeType],  # (1)
    InstanceCount: NotRequired[int],
    VolumeKmsKeyId: NotRequired[str],
    InstanceGroups: NotRequired[Sequence[InstanceGroupTypeDef]],  # (2)
    KeepAlivePeriodInSeconds: NotRequired[int],
```

1. See [:material-code-brackets: TrainingInstanceTypeType](./literals.md#traininginstancetypetype) 
2. See [:material-code-braces: InstanceGroupTypeDef](./type_defs.md#instancegrouptypedef) 
## ParameterRangeTypeDef

```python
# ParameterRangeTypeDef definition

class ParameterRangeTypeDef(TypedDict):
    IntegerParameterRangeSpecification: NotRequired[IntegerParameterRangeSpecificationTypeDef],  # (1)
    ContinuousParameterRangeSpecification: NotRequired[ContinuousParameterRangeSpecificationTypeDef],  # (2)
    CategoricalParameterRangeSpecification: NotRequired[CategoricalParameterRangeSpecificationTypeDef],  # (3)
```

1. See [:material-code-braces: IntegerParameterRangeSpecificationTypeDef](./type_defs.md#integerparameterrangespecificationtypedef) 
2. See [:material-code-braces: ContinuousParameterRangeSpecificationTypeDef](./type_defs.md#continuousparameterrangespecificationtypedef) 
3. See [:material-code-braces: CategoricalParameterRangeSpecificationTypeDef](./type_defs.md#categoricalparameterrangespecificationtypedef) 
## ParameterRangesTypeDef

```python
# ParameterRangesTypeDef definition

class ParameterRangesTypeDef(TypedDict):
    IntegerParameterRanges: NotRequired[Sequence[IntegerParameterRangeTypeDef]],  # (1)
    ContinuousParameterRanges: NotRequired[Sequence[ContinuousParameterRangeTypeDef]],  # (2)
    CategoricalParameterRanges: NotRequired[Sequence[CategoricalParameterRangeTypeDef]],  # (3)
    AutoParameters: NotRequired[Sequence[AutoParameterTypeDef]],  # (4)
```

1. See [:material-code-braces: IntegerParameterRangeTypeDef](./type_defs.md#integerparameterrangetypedef) 
2. See [:material-code-braces: ContinuousParameterRangeTypeDef](./type_defs.md#continuousparameterrangetypedef) 
3. See [:material-code-braces: CategoricalParameterRangeTypeDef](./type_defs.md#categoricalparameterrangetypedef) 
4. See [:material-code-braces: AutoParameterTypeDef](./type_defs.md#autoparametertypedef) 
## KernelGatewayImageConfigTypeDef

```python
# KernelGatewayImageConfigTypeDef definition

class KernelGatewayImageConfigTypeDef(TypedDict):
    KernelSpecs: Sequence[KernelSpecTypeDef],  # (1)
    FileSystemConfig: NotRequired[FileSystemConfigTypeDef],  # (2)
```

1. See [:material-code-braces: KernelSpecTypeDef](./type_defs.md#kernelspectypedef) 
2. See [:material-code-braces: FileSystemConfigTypeDef](./type_defs.md#filesystemconfigtypedef) 
## LabelingJobForWorkteamSummaryTypeDef

```python
# LabelingJobForWorkteamSummaryTypeDef definition

class LabelingJobForWorkteamSummaryTypeDef(TypedDict):
    JobReferenceCode: str,
    WorkRequesterAccountId: str,
    CreationTime: datetime,
    LabelingJobName: NotRequired[str],
    LabelCounters: NotRequired[LabelCountersForWorkteamTypeDef],  # (1)
    NumberOfHumanWorkersPerDataObject: NotRequired[int],
```

1. See [:material-code-braces: LabelCountersForWorkteamTypeDef](./type_defs.md#labelcountersforworkteamtypedef) 
## LabelingJobDataSourceTypeDef

```python
# LabelingJobDataSourceTypeDef definition

class LabelingJobDataSourceTypeDef(TypedDict):
    S3DataSource: NotRequired[LabelingJobS3DataSourceTypeDef],  # (1)
    SnsDataSource: NotRequired[LabelingJobSnsDataSourceTypeDef],  # (2)
```

1. See [:material-code-braces: LabelingJobS3DataSourceTypeDef](./type_defs.md#labelingjobs3datasourcetypedef) 
2. See [:material-code-braces: LabelingJobSnsDataSourceTypeDef](./type_defs.md#labelingjobsnsdatasourcetypedef) 
## ListLineageGroupsResponseTypeDef

```python
# ListLineageGroupsResponseTypeDef definition

class ListLineageGroupsResponseTypeDef(TypedDict):
    LineageGroupSummaries: List[LineageGroupSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LineageGroupSummaryTypeDef](./type_defs.md#lineagegroupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListActionsRequestListActionsPaginateTypeDef

```python
# ListActionsRequestListActionsPaginateTypeDef definition

class ListActionsRequestListActionsPaginateTypeDef(TypedDict):
    SourceUri: NotRequired[str],
    ActionType: NotRequired[str],
    CreatedAfter: NotRequired[Union[datetime, str]],
    CreatedBefore: NotRequired[Union[datetime, str]],
    SortBy: NotRequired[SortActionsByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SortActionsByType](./literals.md#sortactionsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAlgorithmsInputListAlgorithmsPaginateTypeDef

```python
# ListAlgorithmsInputListAlgorithmsPaginateTypeDef definition

class ListAlgorithmsInputListAlgorithmsPaginateTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    NameContains: NotRequired[str],
    SortBy: NotRequired[AlgorithmSortByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: AlgorithmSortByType](./literals.md#algorithmsortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAliasesRequestListAliasesPaginateTypeDef

```python
# ListAliasesRequestListAliasesPaginateTypeDef definition

class ListAliasesRequestListAliasesPaginateTypeDef(TypedDict):
    ImageName: str,
    Alias: NotRequired[str],
    Version: NotRequired[int],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAppImageConfigsRequestListAppImageConfigsPaginateTypeDef

```python
# ListAppImageConfigsRequestListAppImageConfigsPaginateTypeDef definition

class ListAppImageConfigsRequestListAppImageConfigsPaginateTypeDef(TypedDict):
    NameContains: NotRequired[str],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    ModifiedTimeBefore: NotRequired[Union[datetime, str]],
    ModifiedTimeAfter: NotRequired[Union[datetime, str]],
    SortBy: NotRequired[AppImageConfigSortKeyType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: AppImageConfigSortKeyType](./literals.md#appimageconfigsortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAppsRequestListAppsPaginateTypeDef

```python
# ListAppsRequestListAppsPaginateTypeDef definition

class ListAppsRequestListAppsPaginateTypeDef(TypedDict):
    SortOrder: NotRequired[SortOrderType],  # (1)
    SortBy: NotRequired[AppSortKeyType],  # (2)
    DomainIdEquals: NotRequired[str],
    UserProfileNameEquals: NotRequired[str],
    SpaceNameEquals: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-brackets: AppSortKeyType](./literals.md#appsortkeytype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListArtifactsRequestListArtifactsPaginateTypeDef

```python
# ListArtifactsRequestListArtifactsPaginateTypeDef definition

class ListArtifactsRequestListArtifactsPaginateTypeDef(TypedDict):
    SourceUri: NotRequired[str],
    ArtifactType: NotRequired[str],
    CreatedAfter: NotRequired[Union[datetime, str]],
    CreatedBefore: NotRequired[Union[datetime, str]],
    SortBy: NotRequired[SortArtifactsByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SortArtifactsByType](./literals.md#sortartifactsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssociationsRequestListAssociationsPaginateTypeDef

```python
# ListAssociationsRequestListAssociationsPaginateTypeDef definition

class ListAssociationsRequestListAssociationsPaginateTypeDef(TypedDict):
    SourceArn: NotRequired[str],
    DestinationArn: NotRequired[str],
    SourceType: NotRequired[str],
    DestinationType: NotRequired[str],
    AssociationType: NotRequired[AssociationEdgeTypeType],  # (1)
    CreatedAfter: NotRequired[Union[datetime, str]],
    CreatedBefore: NotRequired[Union[datetime, str]],
    SortBy: NotRequired[SortAssociationsByType],  # (2)
    SortOrder: NotRequired[SortOrderType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: AssociationEdgeTypeType](./literals.md#associationedgetypetype) 
2. See [:material-code-brackets: SortAssociationsByType](./literals.md#sortassociationsbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAutoMLJobsRequestListAutoMLJobsPaginateTypeDef

```python
# ListAutoMLJobsRequestListAutoMLJobsPaginateTypeDef definition

class ListAutoMLJobsRequestListAutoMLJobsPaginateTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    NameContains: NotRequired[str],
    StatusEquals: NotRequired[AutoMLJobStatusType],  # (1)
    SortOrder: NotRequired[AutoMLSortOrderType],  # (2)
    SortBy: NotRequired[AutoMLSortByType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: AutoMLJobStatusType](./literals.md#automljobstatustype) 
2. See [:material-code-brackets: AutoMLSortOrderType](./literals.md#automlsortordertype) 
3. See [:material-code-brackets: AutoMLSortByType](./literals.md#automlsortbytype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCandidatesForAutoMLJobRequestListCandidatesForAutoMLJobPaginateTypeDef

```python
# ListCandidatesForAutoMLJobRequestListCandidatesForAutoMLJobPaginateTypeDef definition

class ListCandidatesForAutoMLJobRequestListCandidatesForAutoMLJobPaginateTypeDef(TypedDict):
    AutoMLJobName: str,
    StatusEquals: NotRequired[CandidateStatusType],  # (1)
    CandidateNameEquals: NotRequired[str],
    SortOrder: NotRequired[AutoMLSortOrderType],  # (2)
    SortBy: NotRequired[CandidateSortByType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: CandidateStatusType](./literals.md#candidatestatustype) 
2. See [:material-code-brackets: AutoMLSortOrderType](./literals.md#automlsortordertype) 
3. See [:material-code-brackets: CandidateSortByType](./literals.md#candidatesortbytype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCodeRepositoriesInputListCodeRepositoriesPaginateTypeDef

```python
# ListCodeRepositoriesInputListCodeRepositoriesPaginateTypeDef definition

class ListCodeRepositoriesInputListCodeRepositoriesPaginateTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    NameContains: NotRequired[str],
    SortBy: NotRequired[CodeRepositorySortByType],  # (1)
    SortOrder: NotRequired[CodeRepositorySortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: CodeRepositorySortByType](./literals.md#coderepositorysortbytype) 
2. See [:material-code-brackets: CodeRepositorySortOrderType](./literals.md#coderepositorysortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCompilationJobsRequestListCompilationJobsPaginateTypeDef

```python
# ListCompilationJobsRequestListCompilationJobsPaginateTypeDef definition

class ListCompilationJobsRequestListCompilationJobsPaginateTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    NameContains: NotRequired[str],
    StatusEquals: NotRequired[CompilationJobStatusType],  # (1)
    SortBy: NotRequired[ListCompilationJobsSortByType],  # (2)
    SortOrder: NotRequired[SortOrderType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: CompilationJobStatusType](./literals.md#compilationjobstatustype) 
2. See [:material-code-brackets: ListCompilationJobsSortByType](./literals.md#listcompilationjobssortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListContextsRequestListContextsPaginateTypeDef

```python
# ListContextsRequestListContextsPaginateTypeDef definition

class ListContextsRequestListContextsPaginateTypeDef(TypedDict):
    SourceUri: NotRequired[str],
    ContextType: NotRequired[str],
    CreatedAfter: NotRequired[Union[datetime, str]],
    CreatedBefore: NotRequired[Union[datetime, str]],
    SortBy: NotRequired[SortContextsByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SortContextsByType](./literals.md#sortcontextsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataQualityJobDefinitionsRequestListDataQualityJobDefinitionsPaginateTypeDef

```python
# ListDataQualityJobDefinitionsRequestListDataQualityJobDefinitionsPaginateTypeDef definition

class ListDataQualityJobDefinitionsRequestListDataQualityJobDefinitionsPaginateTypeDef(TypedDict):
    EndpointName: NotRequired[str],
    SortBy: NotRequired[MonitoringJobDefinitionSortKeyType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    NameContains: NotRequired[str],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: MonitoringJobDefinitionSortKeyType](./literals.md#monitoringjobdefinitionsortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDeviceFleetsRequestListDeviceFleetsPaginateTypeDef

```python
# ListDeviceFleetsRequestListDeviceFleetsPaginateTypeDef definition

class ListDeviceFleetsRequestListDeviceFleetsPaginateTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    NameContains: NotRequired[str],
    SortBy: NotRequired[ListDeviceFleetsSortByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ListDeviceFleetsSortByType](./literals.md#listdevicefleetssortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDevicesRequestListDevicesPaginateTypeDef

```python
# ListDevicesRequestListDevicesPaginateTypeDef definition

class ListDevicesRequestListDevicesPaginateTypeDef(TypedDict):
    LatestHeartbeatAfter: NotRequired[Union[datetime, str]],
    ModelName: NotRequired[str],
    DeviceFleetName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDomainsRequestListDomainsPaginateTypeDef

```python
# ListDomainsRequestListDomainsPaginateTypeDef definition

class ListDomainsRequestListDomainsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEdgeDeploymentPlansRequestListEdgeDeploymentPlansPaginateTypeDef

```python
# ListEdgeDeploymentPlansRequestListEdgeDeploymentPlansPaginateTypeDef definition

class ListEdgeDeploymentPlansRequestListEdgeDeploymentPlansPaginateTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    NameContains: NotRequired[str],
    DeviceFleetNameContains: NotRequired[str],
    SortBy: NotRequired[ListEdgeDeploymentPlansSortByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ListEdgeDeploymentPlansSortByType](./literals.md#listedgedeploymentplanssortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEdgePackagingJobsRequestListEdgePackagingJobsPaginateTypeDef

```python
# ListEdgePackagingJobsRequestListEdgePackagingJobsPaginateTypeDef definition

class ListEdgePackagingJobsRequestListEdgePackagingJobsPaginateTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    NameContains: NotRequired[str],
    ModelNameContains: NotRequired[str],
    StatusEquals: NotRequired[EdgePackagingJobStatusType],  # (1)
    SortBy: NotRequired[ListEdgePackagingJobsSortByType],  # (2)
    SortOrder: NotRequired[SortOrderType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: EdgePackagingJobStatusType](./literals.md#edgepackagingjobstatustype) 
2. See [:material-code-brackets: ListEdgePackagingJobsSortByType](./literals.md#listedgepackagingjobssortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEndpointConfigsInputListEndpointConfigsPaginateTypeDef

```python
# ListEndpointConfigsInputListEndpointConfigsPaginateTypeDef definition

class ListEndpointConfigsInputListEndpointConfigsPaginateTypeDef(TypedDict):
    SortBy: NotRequired[EndpointConfigSortKeyType],  # (1)
    SortOrder: NotRequired[OrderKeyType],  # (2)
    NameContains: NotRequired[str],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: EndpointConfigSortKeyType](./literals.md#endpointconfigsortkeytype) 
2. See [:material-code-brackets: OrderKeyType](./literals.md#orderkeytype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEndpointsInputListEndpointsPaginateTypeDef

```python
# ListEndpointsInputListEndpointsPaginateTypeDef definition

class ListEndpointsInputListEndpointsPaginateTypeDef(TypedDict):
    SortBy: NotRequired[EndpointSortKeyType],  # (1)
    SortOrder: NotRequired[OrderKeyType],  # (2)
    NameContains: NotRequired[str],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    StatusEquals: NotRequired[EndpointStatusType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: EndpointSortKeyType](./literals.md#endpointsortkeytype) 
2. See [:material-code-brackets: OrderKeyType](./literals.md#orderkeytype) 
3. See [:material-code-brackets: EndpointStatusType](./literals.md#endpointstatustype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListExperimentsRequestListExperimentsPaginateTypeDef

```python
# ListExperimentsRequestListExperimentsPaginateTypeDef definition

class ListExperimentsRequestListExperimentsPaginateTypeDef(TypedDict):
    CreatedAfter: NotRequired[Union[datetime, str]],
    CreatedBefore: NotRequired[Union[datetime, str]],
    SortBy: NotRequired[SortExperimentsByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SortExperimentsByType](./literals.md#sortexperimentsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFeatureGroupsRequestListFeatureGroupsPaginateTypeDef

```python
# ListFeatureGroupsRequestListFeatureGroupsPaginateTypeDef definition

class ListFeatureGroupsRequestListFeatureGroupsPaginateTypeDef(TypedDict):
    NameContains: NotRequired[str],
    FeatureGroupStatusEquals: NotRequired[FeatureGroupStatusType],  # (1)
    OfflineStoreStatusEquals: NotRequired[OfflineStoreStatusValueType],  # (2)
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    SortOrder: NotRequired[FeatureGroupSortOrderType],  # (3)
    SortBy: NotRequired[FeatureGroupSortByType],  # (4)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (5)
```

1. See [:material-code-brackets: FeatureGroupStatusType](./literals.md#featuregroupstatustype) 
2. See [:material-code-brackets: OfflineStoreStatusValueType](./literals.md#offlinestorestatusvaluetype) 
3. See [:material-code-brackets: FeatureGroupSortOrderType](./literals.md#featuregroupsortordertype) 
4. See [:material-code-brackets: FeatureGroupSortByType](./literals.md#featuregroupsortbytype) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFlowDefinitionsRequestListFlowDefinitionsPaginateTypeDef

```python
# ListFlowDefinitionsRequestListFlowDefinitionsPaginateTypeDef definition

class ListFlowDefinitionsRequestListFlowDefinitionsPaginateTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    SortOrder: NotRequired[SortOrderType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListHumanTaskUisRequestListHumanTaskUisPaginateTypeDef

```python
# ListHumanTaskUisRequestListHumanTaskUisPaginateTypeDef definition

class ListHumanTaskUisRequestListHumanTaskUisPaginateTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    SortOrder: NotRequired[SortOrderType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListHyperParameterTuningJobsRequestListHyperParameterTuningJobsPaginateTypeDef

```python
# ListHyperParameterTuningJobsRequestListHyperParameterTuningJobsPaginateTypeDef definition

class ListHyperParameterTuningJobsRequestListHyperParameterTuningJobsPaginateTypeDef(TypedDict):
    SortBy: NotRequired[HyperParameterTuningJobSortByOptionsType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    NameContains: NotRequired[str],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    StatusEquals: NotRequired[HyperParameterTuningJobStatusType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: HyperParameterTuningJobSortByOptionsType](./literals.md#hyperparametertuningjobsortbyoptionstype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: HyperParameterTuningJobStatusType](./literals.md#hyperparametertuningjobstatustype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListImageVersionsRequestListImageVersionsPaginateTypeDef

```python
# ListImageVersionsRequestListImageVersionsPaginateTypeDef definition

class ListImageVersionsRequestListImageVersionsPaginateTypeDef(TypedDict):
    ImageName: str,
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    SortBy: NotRequired[ImageVersionSortByType],  # (1)
    SortOrder: NotRequired[ImageVersionSortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ImageVersionSortByType](./literals.md#imageversionsortbytype) 
2. See [:material-code-brackets: ImageVersionSortOrderType](./literals.md#imageversionsortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListImagesRequestListImagesPaginateTypeDef

```python
# ListImagesRequestListImagesPaginateTypeDef definition

class ListImagesRequestListImagesPaginateTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    NameContains: NotRequired[str],
    SortBy: NotRequired[ImageSortByType],  # (1)
    SortOrder: NotRequired[ImageSortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ImageSortByType](./literals.md#imagesortbytype) 
2. See [:material-code-brackets: ImageSortOrderType](./literals.md#imagesortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInferenceExperimentsRequestListInferenceExperimentsPaginateTypeDef

```python
# ListInferenceExperimentsRequestListInferenceExperimentsPaginateTypeDef definition

class ListInferenceExperimentsRequestListInferenceExperimentsPaginateTypeDef(TypedDict):
    NameContains: NotRequired[str],
    Type: NotRequired[InferenceExperimentTypeType],  # (1)
    StatusEquals: NotRequired[InferenceExperimentStatusType],  # (2)
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    SortBy: NotRequired[SortInferenceExperimentsByType],  # (3)
    SortOrder: NotRequired[SortOrderType],  # (4)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (5)
```

1. See [:material-code-brackets: InferenceExperimentTypeType](./literals.md#inferenceexperimenttypetype) 
2. See [:material-code-brackets: InferenceExperimentStatusType](./literals.md#inferenceexperimentstatustype) 
3. See [:material-code-brackets: SortInferenceExperimentsByType](./literals.md#sortinferenceexperimentsbytype) 
4. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInferenceRecommendationsJobStepsRequestListInferenceRecommendationsJobStepsPaginateTypeDef

```python
# ListInferenceRecommendationsJobStepsRequestListInferenceRecommendationsJobStepsPaginateTypeDef definition

class ListInferenceRecommendationsJobStepsRequestListInferenceRecommendationsJobStepsPaginateTypeDef(TypedDict):
    JobName: str,
    Status: NotRequired[RecommendationJobStatusType],  # (1)
    StepType: NotRequired[RecommendationStepTypeType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: RecommendationJobStatusType](./literals.md#recommendationjobstatustype) 
2. See [:material-code-brackets: RecommendationStepTypeType](./literals.md#recommendationsteptypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInferenceRecommendationsJobsRequestListInferenceRecommendationsJobsPaginateTypeDef

```python
# ListInferenceRecommendationsJobsRequestListInferenceRecommendationsJobsPaginateTypeDef definition

class ListInferenceRecommendationsJobsRequestListInferenceRecommendationsJobsPaginateTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    NameContains: NotRequired[str],
    StatusEquals: NotRequired[RecommendationJobStatusType],  # (1)
    SortBy: NotRequired[ListInferenceRecommendationsJobsSortByType],  # (2)
    SortOrder: NotRequired[SortOrderType],  # (3)
    ModelNameEquals: NotRequired[str],
    ModelPackageVersionArnEquals: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: RecommendationJobStatusType](./literals.md#recommendationjobstatustype) 
2. See [:material-code-brackets: ListInferenceRecommendationsJobsSortByType](./literals.md#listinferencerecommendationsjobssortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLabelingJobsForWorkteamRequestListLabelingJobsForWorkteamPaginateTypeDef

```python
# ListLabelingJobsForWorkteamRequestListLabelingJobsForWorkteamPaginateTypeDef definition

class ListLabelingJobsForWorkteamRequestListLabelingJobsForWorkteamPaginateTypeDef(TypedDict):
    WorkteamArn: str,
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    JobReferenceCodeContains: NotRequired[str],
    SortBy: NotRequired[ListLabelingJobsForWorkteamSortByOptionsType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ListLabelingJobsForWorkteamSortByOptionsType](./literals.md#listlabelingjobsforworkteamsortbyoptionstype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLabelingJobsRequestListLabelingJobsPaginateTypeDef

```python
# ListLabelingJobsRequestListLabelingJobsPaginateTypeDef definition

class ListLabelingJobsRequestListLabelingJobsPaginateTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    NameContains: NotRequired[str],
    SortBy: NotRequired[SortByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    StatusEquals: NotRequired[LabelingJobStatusType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: SortByType](./literals.md#sortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: LabelingJobStatusType](./literals.md#labelingjobstatustype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLineageGroupsRequestListLineageGroupsPaginateTypeDef

```python
# ListLineageGroupsRequestListLineageGroupsPaginateTypeDef definition

class ListLineageGroupsRequestListLineageGroupsPaginateTypeDef(TypedDict):
    CreatedAfter: NotRequired[Union[datetime, str]],
    CreatedBefore: NotRequired[Union[datetime, str]],
    SortBy: NotRequired[SortLineageGroupsByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SortLineageGroupsByType](./literals.md#sortlineagegroupsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListModelBiasJobDefinitionsRequestListModelBiasJobDefinitionsPaginateTypeDef

```python
# ListModelBiasJobDefinitionsRequestListModelBiasJobDefinitionsPaginateTypeDef definition

class ListModelBiasJobDefinitionsRequestListModelBiasJobDefinitionsPaginateTypeDef(TypedDict):
    EndpointName: NotRequired[str],
    SortBy: NotRequired[MonitoringJobDefinitionSortKeyType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    NameContains: NotRequired[str],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: MonitoringJobDefinitionSortKeyType](./literals.md#monitoringjobdefinitionsortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListModelCardExportJobsRequestListModelCardExportJobsPaginateTypeDef

```python
# ListModelCardExportJobsRequestListModelCardExportJobsPaginateTypeDef definition

class ListModelCardExportJobsRequestListModelCardExportJobsPaginateTypeDef(TypedDict):
    ModelCardName: str,
    ModelCardVersion: NotRequired[int],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    ModelCardExportJobNameContains: NotRequired[str],
    StatusEquals: NotRequired[ModelCardExportJobStatusType],  # (1)
    SortBy: NotRequired[ModelCardExportJobSortByType],  # (2)
    SortOrder: NotRequired[ModelCardExportJobSortOrderType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: ModelCardExportJobStatusType](./literals.md#modelcardexportjobstatustype) 
2. See [:material-code-brackets: ModelCardExportJobSortByType](./literals.md#modelcardexportjobsortbytype) 
3. See [:material-code-brackets: ModelCardExportJobSortOrderType](./literals.md#modelcardexportjobsortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListModelCardVersionsRequestListModelCardVersionsPaginateTypeDef

```python
# ListModelCardVersionsRequestListModelCardVersionsPaginateTypeDef definition

class ListModelCardVersionsRequestListModelCardVersionsPaginateTypeDef(TypedDict):
    ModelCardName: str,
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    ModelCardStatus: NotRequired[ModelCardStatusType],  # (1)
    SortBy: NotRequired[ModelCardVersionSortByType],  # (2)
    SortOrder: NotRequired[ModelCardSortOrderType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: ModelCardStatusType](./literals.md#modelcardstatustype) 
2. See [:material-code-brackets: ModelCardVersionSortByType](./literals.md#modelcardversionsortbytype) 
3. See [:material-code-brackets: ModelCardSortOrderType](./literals.md#modelcardsortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListModelCardsRequestListModelCardsPaginateTypeDef

```python
# ListModelCardsRequestListModelCardsPaginateTypeDef definition

class ListModelCardsRequestListModelCardsPaginateTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    NameContains: NotRequired[str],
    ModelCardStatus: NotRequired[ModelCardStatusType],  # (1)
    SortBy: NotRequired[ModelCardSortByType],  # (2)
    SortOrder: NotRequired[ModelCardSortOrderType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: ModelCardStatusType](./literals.md#modelcardstatustype) 
2. See [:material-code-brackets: ModelCardSortByType](./literals.md#modelcardsortbytype) 
3. See [:material-code-brackets: ModelCardSortOrderType](./literals.md#modelcardsortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListModelExplainabilityJobDefinitionsRequestListModelExplainabilityJobDefinitionsPaginateTypeDef

```python
# ListModelExplainabilityJobDefinitionsRequestListModelExplainabilityJobDefinitionsPaginateTypeDef definition

class ListModelExplainabilityJobDefinitionsRequestListModelExplainabilityJobDefinitionsPaginateTypeDef(TypedDict):
    EndpointName: NotRequired[str],
    SortBy: NotRequired[MonitoringJobDefinitionSortKeyType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    NameContains: NotRequired[str],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: MonitoringJobDefinitionSortKeyType](./literals.md#monitoringjobdefinitionsortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListModelPackageGroupsInputListModelPackageGroupsPaginateTypeDef

```python
# ListModelPackageGroupsInputListModelPackageGroupsPaginateTypeDef definition

class ListModelPackageGroupsInputListModelPackageGroupsPaginateTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    NameContains: NotRequired[str],
    SortBy: NotRequired[ModelPackageGroupSortByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ModelPackageGroupSortByType](./literals.md#modelpackagegroupsortbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListModelPackagesInputListModelPackagesPaginateTypeDef

```python
# ListModelPackagesInputListModelPackagesPaginateTypeDef definition

class ListModelPackagesInputListModelPackagesPaginateTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    NameContains: NotRequired[str],
    ModelApprovalStatus: NotRequired[ModelApprovalStatusType],  # (1)
    ModelPackageGroupName: NotRequired[str],
    ModelPackageType: NotRequired[ModelPackageTypeType],  # (2)
    SortBy: NotRequired[ModelPackageSortByType],  # (3)
    SortOrder: NotRequired[SortOrderType],  # (4)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (5)
```

1. See [:material-code-brackets: ModelApprovalStatusType](./literals.md#modelapprovalstatustype) 
2. See [:material-code-brackets: ModelPackageTypeType](./literals.md#modelpackagetypetype) 
3. See [:material-code-brackets: ModelPackageSortByType](./literals.md#modelpackagesortbytype) 
4. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListModelQualityJobDefinitionsRequestListModelQualityJobDefinitionsPaginateTypeDef

```python
# ListModelQualityJobDefinitionsRequestListModelQualityJobDefinitionsPaginateTypeDef definition

class ListModelQualityJobDefinitionsRequestListModelQualityJobDefinitionsPaginateTypeDef(TypedDict):
    EndpointName: NotRequired[str],
    SortBy: NotRequired[MonitoringJobDefinitionSortKeyType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    NameContains: NotRequired[str],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: MonitoringJobDefinitionSortKeyType](./literals.md#monitoringjobdefinitionsortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListModelsInputListModelsPaginateTypeDef

```python
# ListModelsInputListModelsPaginateTypeDef definition

class ListModelsInputListModelsPaginateTypeDef(TypedDict):
    SortBy: NotRequired[ModelSortKeyType],  # (1)
    SortOrder: NotRequired[OrderKeyType],  # (2)
    NameContains: NotRequired[str],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ModelSortKeyType](./literals.md#modelsortkeytype) 
2. See [:material-code-brackets: OrderKeyType](./literals.md#orderkeytype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMonitoringAlertHistoryRequestListMonitoringAlertHistoryPaginateTypeDef

```python
# ListMonitoringAlertHistoryRequestListMonitoringAlertHistoryPaginateTypeDef definition

class ListMonitoringAlertHistoryRequestListMonitoringAlertHistoryPaginateTypeDef(TypedDict):
    MonitoringScheduleName: NotRequired[str],
    MonitoringAlertName: NotRequired[str],
    SortBy: NotRequired[MonitoringAlertHistorySortKeyType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    StatusEquals: NotRequired[MonitoringAlertStatusType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: MonitoringAlertHistorySortKeyType](./literals.md#monitoringalerthistorysortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: MonitoringAlertStatusType](./literals.md#monitoringalertstatustype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMonitoringAlertsRequestListMonitoringAlertsPaginateTypeDef

```python
# ListMonitoringAlertsRequestListMonitoringAlertsPaginateTypeDef definition

class ListMonitoringAlertsRequestListMonitoringAlertsPaginateTypeDef(TypedDict):
    MonitoringScheduleName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMonitoringExecutionsRequestListMonitoringExecutionsPaginateTypeDef

```python
# ListMonitoringExecutionsRequestListMonitoringExecutionsPaginateTypeDef definition

class ListMonitoringExecutionsRequestListMonitoringExecutionsPaginateTypeDef(TypedDict):
    MonitoringScheduleName: NotRequired[str],
    EndpointName: NotRequired[str],
    SortBy: NotRequired[MonitoringExecutionSortKeyType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    ScheduledTimeBefore: NotRequired[Union[datetime, str]],
    ScheduledTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    StatusEquals: NotRequired[ExecutionStatusType],  # (3)
    MonitoringJobDefinitionName: NotRequired[str],
    MonitoringTypeEquals: NotRequired[MonitoringTypeType],  # (4)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (5)
```

1. See [:material-code-brackets: MonitoringExecutionSortKeyType](./literals.md#monitoringexecutionsortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: ExecutionStatusType](./literals.md#executionstatustype) 
4. See [:material-code-brackets: MonitoringTypeType](./literals.md#monitoringtypetype) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMonitoringSchedulesRequestListMonitoringSchedulesPaginateTypeDef

```python
# ListMonitoringSchedulesRequestListMonitoringSchedulesPaginateTypeDef definition

class ListMonitoringSchedulesRequestListMonitoringSchedulesPaginateTypeDef(TypedDict):
    EndpointName: NotRequired[str],
    SortBy: NotRequired[MonitoringScheduleSortKeyType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    NameContains: NotRequired[str],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    StatusEquals: NotRequired[ScheduleStatusType],  # (3)
    MonitoringJobDefinitionName: NotRequired[str],
    MonitoringTypeEquals: NotRequired[MonitoringTypeType],  # (4)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (5)
```

1. See [:material-code-brackets: MonitoringScheduleSortKeyType](./literals.md#monitoringschedulesortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: ScheduleStatusType](./literals.md#schedulestatustype) 
4. See [:material-code-brackets: MonitoringTypeType](./literals.md#monitoringtypetype) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNotebookInstanceLifecycleConfigsInputListNotebookInstanceLifecycleConfigsPaginateTypeDef

```python
# ListNotebookInstanceLifecycleConfigsInputListNotebookInstanceLifecycleConfigsPaginateTypeDef definition

class ListNotebookInstanceLifecycleConfigsInputListNotebookInstanceLifecycleConfigsPaginateTypeDef(TypedDict):
    SortBy: NotRequired[NotebookInstanceLifecycleConfigSortKeyType],  # (1)
    SortOrder: NotRequired[NotebookInstanceLifecycleConfigSortOrderType],  # (2)
    NameContains: NotRequired[str],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: NotebookInstanceLifecycleConfigSortKeyType](./literals.md#notebookinstancelifecycleconfigsortkeytype) 
2. See [:material-code-brackets: NotebookInstanceLifecycleConfigSortOrderType](./literals.md#notebookinstancelifecycleconfigsortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNotebookInstancesInputListNotebookInstancesPaginateTypeDef

```python
# ListNotebookInstancesInputListNotebookInstancesPaginateTypeDef definition

class ListNotebookInstancesInputListNotebookInstancesPaginateTypeDef(TypedDict):
    SortBy: NotRequired[NotebookInstanceSortKeyType],  # (1)
    SortOrder: NotRequired[NotebookInstanceSortOrderType],  # (2)
    NameContains: NotRequired[str],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    StatusEquals: NotRequired[NotebookInstanceStatusType],  # (3)
    NotebookInstanceLifecycleConfigNameContains: NotRequired[str],
    DefaultCodeRepositoryContains: NotRequired[str],
    AdditionalCodeRepositoryEquals: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: NotebookInstanceSortKeyType](./literals.md#notebookinstancesortkeytype) 
2. See [:material-code-brackets: NotebookInstanceSortOrderType](./literals.md#notebookinstancesortordertype) 
3. See [:material-code-brackets: NotebookInstanceStatusType](./literals.md#notebookinstancestatustype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPipelineExecutionStepsRequestListPipelineExecutionStepsPaginateTypeDef

```python
# ListPipelineExecutionStepsRequestListPipelineExecutionStepsPaginateTypeDef definition

class ListPipelineExecutionStepsRequestListPipelineExecutionStepsPaginateTypeDef(TypedDict):
    PipelineExecutionArn: NotRequired[str],
    SortOrder: NotRequired[SortOrderType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPipelineExecutionsRequestListPipelineExecutionsPaginateTypeDef

```python
# ListPipelineExecutionsRequestListPipelineExecutionsPaginateTypeDef definition

class ListPipelineExecutionsRequestListPipelineExecutionsPaginateTypeDef(TypedDict):
    PipelineName: str,
    CreatedAfter: NotRequired[Union[datetime, str]],
    CreatedBefore: NotRequired[Union[datetime, str]],
    SortBy: NotRequired[SortPipelineExecutionsByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SortPipelineExecutionsByType](./literals.md#sortpipelineexecutionsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPipelineParametersForExecutionRequestListPipelineParametersForExecutionPaginateTypeDef

```python
# ListPipelineParametersForExecutionRequestListPipelineParametersForExecutionPaginateTypeDef definition

class ListPipelineParametersForExecutionRequestListPipelineParametersForExecutionPaginateTypeDef(TypedDict):
    PipelineExecutionArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPipelinesRequestListPipelinesPaginateTypeDef

```python
# ListPipelinesRequestListPipelinesPaginateTypeDef definition

class ListPipelinesRequestListPipelinesPaginateTypeDef(TypedDict):
    PipelineNamePrefix: NotRequired[str],
    CreatedAfter: NotRequired[Union[datetime, str]],
    CreatedBefore: NotRequired[Union[datetime, str]],
    SortBy: NotRequired[SortPipelinesByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SortPipelinesByType](./literals.md#sortpipelinesbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProcessingJobsRequestListProcessingJobsPaginateTypeDef

```python
# ListProcessingJobsRequestListProcessingJobsPaginateTypeDef definition

class ListProcessingJobsRequestListProcessingJobsPaginateTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    NameContains: NotRequired[str],
    StatusEquals: NotRequired[ProcessingJobStatusType],  # (1)
    SortBy: NotRequired[SortByType],  # (2)
    SortOrder: NotRequired[SortOrderType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: ProcessingJobStatusType](./literals.md#processingjobstatustype) 
2. See [:material-code-brackets: SortByType](./literals.md#sortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourceCatalogsRequestListResourceCatalogsPaginateTypeDef

```python
# ListResourceCatalogsRequestListResourceCatalogsPaginateTypeDef definition

class ListResourceCatalogsRequestListResourceCatalogsPaginateTypeDef(TypedDict):
    NameContains: NotRequired[str],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    SortOrder: NotRequired[ResourceCatalogSortOrderType],  # (1)
    SortBy: NotRequired[ResourceCatalogSortByType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ResourceCatalogSortOrderType](./literals.md#resourcecatalogsortordertype) 
2. See [:material-code-brackets: ResourceCatalogSortByType](./literals.md#resourcecatalogsortbytype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSpacesRequestListSpacesPaginateTypeDef

```python
# ListSpacesRequestListSpacesPaginateTypeDef definition

class ListSpacesRequestListSpacesPaginateTypeDef(TypedDict):
    SortOrder: NotRequired[SortOrderType],  # (1)
    SortBy: NotRequired[SpaceSortKeyType],  # (2)
    DomainIdEquals: NotRequired[str],
    SpaceNameContains: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-brackets: SpaceSortKeyType](./literals.md#spacesortkeytype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStageDevicesRequestListStageDevicesPaginateTypeDef

```python
# ListStageDevicesRequestListStageDevicesPaginateTypeDef definition

class ListStageDevicesRequestListStageDevicesPaginateTypeDef(TypedDict):
    EdgeDeploymentPlanName: str,
    StageName: str,
    ExcludeDevicesDeployedInOtherStage: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStudioLifecycleConfigsRequestListStudioLifecycleConfigsPaginateTypeDef

```python
# ListStudioLifecycleConfigsRequestListStudioLifecycleConfigsPaginateTypeDef definition

class ListStudioLifecycleConfigsRequestListStudioLifecycleConfigsPaginateTypeDef(TypedDict):
    NameContains: NotRequired[str],
    AppTypeEquals: NotRequired[StudioLifecycleConfigAppTypeType],  # (1)
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    ModifiedTimeBefore: NotRequired[Union[datetime, str]],
    ModifiedTimeAfter: NotRequired[Union[datetime, str]],
    SortBy: NotRequired[StudioLifecycleConfigSortKeyType],  # (2)
    SortOrder: NotRequired[SortOrderType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: StudioLifecycleConfigAppTypeType](./literals.md#studiolifecycleconfigapptypetype) 
2. See [:material-code-brackets: StudioLifecycleConfigSortKeyType](./literals.md#studiolifecycleconfigsortkeytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSubscribedWorkteamsRequestListSubscribedWorkteamsPaginateTypeDef

```python
# ListSubscribedWorkteamsRequestListSubscribedWorkteamsPaginateTypeDef definition

class ListSubscribedWorkteamsRequestListSubscribedWorkteamsPaginateTypeDef(TypedDict):
    NameContains: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsInputListTagsPaginateTypeDef

```python
# ListTagsInputListTagsPaginateTypeDef definition

class ListTagsInputListTagsPaginateTypeDef(TypedDict):
    ResourceArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTrainingJobsForHyperParameterTuningJobRequestListTrainingJobsForHyperParameterTuningJobPaginateTypeDef

```python
# ListTrainingJobsForHyperParameterTuningJobRequestListTrainingJobsForHyperParameterTuningJobPaginateTypeDef definition

class ListTrainingJobsForHyperParameterTuningJobRequestListTrainingJobsForHyperParameterTuningJobPaginateTypeDef(TypedDict):
    HyperParameterTuningJobName: str,
    StatusEquals: NotRequired[TrainingJobStatusType],  # (1)
    SortBy: NotRequired[TrainingJobSortByOptionsType],  # (2)
    SortOrder: NotRequired[SortOrderType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: TrainingJobStatusType](./literals.md#trainingjobstatustype) 
2. See [:material-code-brackets: TrainingJobSortByOptionsType](./literals.md#trainingjobsortbyoptionstype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTrainingJobsRequestListTrainingJobsPaginateTypeDef

```python
# ListTrainingJobsRequestListTrainingJobsPaginateTypeDef definition

class ListTrainingJobsRequestListTrainingJobsPaginateTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    NameContains: NotRequired[str],
    StatusEquals: NotRequired[TrainingJobStatusType],  # (1)
    SortBy: NotRequired[SortByType],  # (2)
    SortOrder: NotRequired[SortOrderType],  # (3)
    WarmPoolStatusEquals: NotRequired[WarmPoolResourceStatusType],  # (4)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (5)
```

1. See [:material-code-brackets: TrainingJobStatusType](./literals.md#trainingjobstatustype) 
2. See [:material-code-brackets: SortByType](./literals.md#sortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-brackets: WarmPoolResourceStatusType](./literals.md#warmpoolresourcestatustype) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTransformJobsRequestListTransformJobsPaginateTypeDef

```python
# ListTransformJobsRequestListTransformJobsPaginateTypeDef definition

class ListTransformJobsRequestListTransformJobsPaginateTypeDef(TypedDict):
    CreationTimeAfter: NotRequired[Union[datetime, str]],
    CreationTimeBefore: NotRequired[Union[datetime, str]],
    LastModifiedTimeAfter: NotRequired[Union[datetime, str]],
    LastModifiedTimeBefore: NotRequired[Union[datetime, str]],
    NameContains: NotRequired[str],
    StatusEquals: NotRequired[TransformJobStatusType],  # (1)
    SortBy: NotRequired[SortByType],  # (2)
    SortOrder: NotRequired[SortOrderType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: TransformJobStatusType](./literals.md#transformjobstatustype) 
2. See [:material-code-brackets: SortByType](./literals.md#sortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTrialComponentsRequestListTrialComponentsPaginateTypeDef

```python
# ListTrialComponentsRequestListTrialComponentsPaginateTypeDef definition

class ListTrialComponentsRequestListTrialComponentsPaginateTypeDef(TypedDict):
    ExperimentName: NotRequired[str],
    TrialName: NotRequired[str],
    SourceArn: NotRequired[str],
    CreatedAfter: NotRequired[Union[datetime, str]],
    CreatedBefore: NotRequired[Union[datetime, str]],
    SortBy: NotRequired[SortTrialComponentsByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SortTrialComponentsByType](./literals.md#sorttrialcomponentsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTrialsRequestListTrialsPaginateTypeDef

```python
# ListTrialsRequestListTrialsPaginateTypeDef definition

class ListTrialsRequestListTrialsPaginateTypeDef(TypedDict):
    ExperimentName: NotRequired[str],
    TrialComponentName: NotRequired[str],
    CreatedAfter: NotRequired[Union[datetime, str]],
    CreatedBefore: NotRequired[Union[datetime, str]],
    SortBy: NotRequired[SortTrialsByType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SortTrialsByType](./literals.md#sorttrialsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUserProfilesRequestListUserProfilesPaginateTypeDef

```python
# ListUserProfilesRequestListUserProfilesPaginateTypeDef definition

class ListUserProfilesRequestListUserProfilesPaginateTypeDef(TypedDict):
    SortOrder: NotRequired[SortOrderType],  # (1)
    SortBy: NotRequired[UserProfileSortKeyType],  # (2)
    DomainIdEquals: NotRequired[str],
    UserProfileNameContains: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-brackets: UserProfileSortKeyType](./literals.md#userprofilesortkeytype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkforcesRequestListWorkforcesPaginateTypeDef

```python
# ListWorkforcesRequestListWorkforcesPaginateTypeDef definition

class ListWorkforcesRequestListWorkforcesPaginateTypeDef(TypedDict):
    SortBy: NotRequired[ListWorkforcesSortByOptionsType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    NameContains: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ListWorkforcesSortByOptionsType](./literals.md#listworkforcessortbyoptionstype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkteamsRequestListWorkteamsPaginateTypeDef

```python
# ListWorkteamsRequestListWorkteamsPaginateTypeDef definition

class ListWorkteamsRequestListWorkteamsPaginateTypeDef(TypedDict):
    SortBy: NotRequired[ListWorkteamsSortByOptionsType],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    NameContains: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ListWorkteamsSortByOptionsType](./literals.md#listworkteamssortbyoptionstype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchRequestSearchPaginateTypeDef

```python
# SearchRequestSearchPaginateTypeDef definition

class SearchRequestSearchPaginateTypeDef(TypedDict):
    Resource: ResourceTypeType,  # (1)
    SearchExpression: NotRequired[SearchExpressionTypeDef],  # (2)
    SortBy: NotRequired[str],
    SortOrder: NotRequired[SearchSortOrderType],  # (3)
    CrossAccountFilterOption: NotRequired[CrossAccountFilterOptionType],  # (4)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (5)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: SearchExpressionTypeDef](./type_defs.md#searchexpressiontypedef) 
3. See [:material-code-brackets: SearchSortOrderType](./literals.md#searchsortordertype) 
4. See [:material-code-brackets: CrossAccountFilterOptionType](./literals.md#crossaccountfilteroptiontype) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataQualityJobDefinitionsResponseTypeDef

```python
# ListDataQualityJobDefinitionsResponseTypeDef definition

class ListDataQualityJobDefinitionsResponseTypeDef(TypedDict):
    JobDefinitionSummaries: List[MonitoringJobDefinitionSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MonitoringJobDefinitionSummaryTypeDef](./type_defs.md#monitoringjobdefinitionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListModelBiasJobDefinitionsResponseTypeDef

```python
# ListModelBiasJobDefinitionsResponseTypeDef definition

class ListModelBiasJobDefinitionsResponseTypeDef(TypedDict):
    JobDefinitionSummaries: List[MonitoringJobDefinitionSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MonitoringJobDefinitionSummaryTypeDef](./type_defs.md#monitoringjobdefinitionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListModelExplainabilityJobDefinitionsResponseTypeDef

```python
# ListModelExplainabilityJobDefinitionsResponseTypeDef definition

class ListModelExplainabilityJobDefinitionsResponseTypeDef(TypedDict):
    JobDefinitionSummaries: List[MonitoringJobDefinitionSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MonitoringJobDefinitionSummaryTypeDef](./type_defs.md#monitoringjobdefinitionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListModelQualityJobDefinitionsResponseTypeDef

```python
# ListModelQualityJobDefinitionsResponseTypeDef definition

class ListModelQualityJobDefinitionsResponseTypeDef(TypedDict):
    JobDefinitionSummaries: List[MonitoringJobDefinitionSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MonitoringJobDefinitionSummaryTypeDef](./type_defs.md#monitoringjobdefinitionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListModelCardExportJobsResponseTypeDef

```python
# ListModelCardExportJobsResponseTypeDef definition

class ListModelCardExportJobsResponseTypeDef(TypedDict):
    ModelCardExportJobSummaries: List[ModelCardExportJobSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ModelCardExportJobSummaryTypeDef](./type_defs.md#modelcardexportjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListModelCardVersionsResponseTypeDef

```python
# ListModelCardVersionsResponseTypeDef definition

class ListModelCardVersionsResponseTypeDef(TypedDict):
    ModelCardVersionSummaryList: List[ModelCardVersionSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ModelCardVersionSummaryTypeDef](./type_defs.md#modelcardversionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListModelCardsResponseTypeDef

```python
# ListModelCardsResponseTypeDef definition

class ListModelCardsResponseTypeDef(TypedDict):
    ModelCardSummaries: List[ModelCardSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ModelCardSummaryTypeDef](./type_defs.md#modelcardsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListModelMetadataResponseTypeDef

```python
# ListModelMetadataResponseTypeDef definition

class ListModelMetadataResponseTypeDef(TypedDict):
    ModelMetadataSummaries: List[ModelMetadataSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ModelMetadataSummaryTypeDef](./type_defs.md#modelmetadatasummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListModelPackageGroupsOutputTypeDef

```python
# ListModelPackageGroupsOutputTypeDef definition

class ListModelPackageGroupsOutputTypeDef(TypedDict):
    ModelPackageGroupSummaryList: List[ModelPackageGroupSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ModelPackageGroupSummaryTypeDef](./type_defs.md#modelpackagegroupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListModelPackagesOutputTypeDef

```python
# ListModelPackagesOutputTypeDef definition

class ListModelPackagesOutputTypeDef(TypedDict):
    ModelPackageSummaryList: List[ModelPackageSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ModelPackageSummaryTypeDef](./type_defs.md#modelpackagesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListModelsOutputTypeDef

```python
# ListModelsOutputTypeDef definition

class ListModelsOutputTypeDef(TypedDict):
    Models: List[ModelSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ModelSummaryTypeDef](./type_defs.md#modelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMonitoringAlertHistoryResponseTypeDef

```python
# ListMonitoringAlertHistoryResponseTypeDef definition

class ListMonitoringAlertHistoryResponseTypeDef(TypedDict):
    MonitoringAlertHistory: List[MonitoringAlertHistorySummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MonitoringAlertHistorySummaryTypeDef](./type_defs.md#monitoringalerthistorysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMonitoringSchedulesResponseTypeDef

```python
# ListMonitoringSchedulesResponseTypeDef definition

class ListMonitoringSchedulesResponseTypeDef(TypedDict):
    MonitoringScheduleSummaries: List[MonitoringScheduleSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MonitoringScheduleSummaryTypeDef](./type_defs.md#monitoringschedulesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListNotebookInstanceLifecycleConfigsOutputTypeDef

```python
# ListNotebookInstanceLifecycleConfigsOutputTypeDef definition

class ListNotebookInstanceLifecycleConfigsOutputTypeDef(TypedDict):
    NextToken: str,
    NotebookInstanceLifecycleConfigs: List[NotebookInstanceLifecycleConfigSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NotebookInstanceLifecycleConfigSummaryTypeDef](./type_defs.md#notebookinstancelifecycleconfigsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListNotebookInstancesOutputTypeDef

```python
# ListNotebookInstancesOutputTypeDef definition

class ListNotebookInstancesOutputTypeDef(TypedDict):
    NextToken: str,
    NotebookInstances: List[NotebookInstanceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NotebookInstanceSummaryTypeDef](./type_defs.md#notebookinstancesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPipelineExecutionsResponseTypeDef

```python
# ListPipelineExecutionsResponseTypeDef definition

class ListPipelineExecutionsResponseTypeDef(TypedDict):
    PipelineExecutionSummaries: List[PipelineExecutionSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipelineExecutionSummaryTypeDef](./type_defs.md#pipelineexecutionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPipelineParametersForExecutionResponseTypeDef

```python
# ListPipelineParametersForExecutionResponseTypeDef definition

class ListPipelineParametersForExecutionResponseTypeDef(TypedDict):
    PipelineParameters: List[ParameterTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPipelinesResponseTypeDef

```python
# ListPipelinesResponseTypeDef definition

class ListPipelinesResponseTypeDef(TypedDict):
    PipelineSummaries: List[PipelineSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipelineSummaryTypeDef](./type_defs.md#pipelinesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProcessingJobsResponseTypeDef

```python
# ListProcessingJobsResponseTypeDef definition

class ListProcessingJobsResponseTypeDef(TypedDict):
    ProcessingJobSummaries: List[ProcessingJobSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProcessingJobSummaryTypeDef](./type_defs.md#processingjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProjectsOutputTypeDef

```python
# ListProjectsOutputTypeDef definition

class ListProjectsOutputTypeDef(TypedDict):
    ProjectSummaryList: List[ProjectSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProjectSummaryTypeDef](./type_defs.md#projectsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResourceCatalogsResponseTypeDef

```python
# ListResourceCatalogsResponseTypeDef definition

class ListResourceCatalogsResponseTypeDef(TypedDict):
    ResourceCatalogs: List[ResourceCatalogTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceCatalogTypeDef](./type_defs.md#resourcecatalogtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSpacesResponseTypeDef

```python
# ListSpacesResponseTypeDef definition

class ListSpacesResponseTypeDef(TypedDict):
    Spaces: List[SpaceDetailsTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SpaceDetailsTypeDef](./type_defs.md#spacedetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStudioLifecycleConfigsResponseTypeDef

```python
# ListStudioLifecycleConfigsResponseTypeDef definition

class ListStudioLifecycleConfigsResponseTypeDef(TypedDict):
    NextToken: str,
    StudioLifecycleConfigs: List[StudioLifecycleConfigDetailsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StudioLifecycleConfigDetailsTypeDef](./type_defs.md#studiolifecycleconfigdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTransformJobsResponseTypeDef

```python
# ListTransformJobsResponseTypeDef definition

class ListTransformJobsResponseTypeDef(TypedDict):
    TransformJobSummaries: List[TransformJobSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TransformJobSummaryTypeDef](./type_defs.md#transformjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUserProfilesResponseTypeDef

```python
# ListUserProfilesResponseTypeDef definition

class ListUserProfilesResponseTypeDef(TypedDict):
    UserProfiles: List[UserProfileDetailsTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserProfileDetailsTypeDef](./type_defs.md#userprofiledetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MemberDefinitionTypeDef

```python
# MemberDefinitionTypeDef definition

class MemberDefinitionTypeDef(TypedDict):
    CognitoMemberDefinition: NotRequired[CognitoMemberDefinitionTypeDef],  # (1)
    OidcMemberDefinition: NotRequired[OidcMemberDefinitionTypeDef],  # (2)
```

1. See [:material-code-braces: CognitoMemberDefinitionTypeDef](./type_defs.md#cognitomemberdefinitiontypedef) 
2. See [:material-code-braces: OidcMemberDefinitionTypeDef](./type_defs.md#oidcmemberdefinitiontypedef) 
## MetricSpecificationTypeDef

```python
# MetricSpecificationTypeDef definition

class MetricSpecificationTypeDef(TypedDict):
    Predefined: NotRequired[PredefinedMetricSpecificationTypeDef],  # (1)
    Customized: NotRequired[CustomizedMetricSpecificationTypeDef],  # (2)
```

1. See [:material-code-braces: PredefinedMetricSpecificationTypeDef](./type_defs.md#predefinedmetricspecificationtypedef) 
2. See [:material-code-braces: CustomizedMetricSpecificationTypeDef](./type_defs.md#customizedmetricspecificationtypedef) 
## MonitoringAlertActionsTypeDef

```python
# MonitoringAlertActionsTypeDef definition

class MonitoringAlertActionsTypeDef(TypedDict):
    ModelDashboardIndicator: NotRequired[ModelDashboardIndicatorActionTypeDef],  # (1)
```

1. See [:material-code-braces: ModelDashboardIndicatorActionTypeDef](./type_defs.md#modeldashboardindicatoractiontypedef) 
## ModelDataSourceTypeDef

```python
# ModelDataSourceTypeDef definition

class ModelDataSourceTypeDef(TypedDict):
    S3DataSource: S3ModelDataSourceTypeDef,  # (1)
```

1. See [:material-code-braces: S3ModelDataSourceTypeDef](./type_defs.md#s3modeldatasourcetypedef) 
## ModelInfrastructureConfigTypeDef

```python
# ModelInfrastructureConfigTypeDef definition

class ModelInfrastructureConfigTypeDef(TypedDict):
    InfrastructureType: ModelInfrastructureTypeType,  # (1)
    RealTimeInferenceConfig: RealTimeInferenceConfigTypeDef,  # (2)
```

1. See [:material-code-brackets: ModelInfrastructureTypeType](./literals.md#modelinfrastructuretypetype) 
2. See [:material-code-braces: RealTimeInferenceConfigTypeDef](./type_defs.md#realtimeinferenceconfigtypedef) 
## ModelPackageContainerDefinitionTypeDef

```python
# ModelPackageContainerDefinitionTypeDef definition

class ModelPackageContainerDefinitionTypeDef(TypedDict):
    Image: str,
    ContainerHostname: NotRequired[str],
    ImageDigest: NotRequired[str],
    ModelDataUrl: NotRequired[str],
    ProductId: NotRequired[str],
    Environment: NotRequired[Dict[str, str]],
    ModelInput: NotRequired[ModelInputTypeDef],  # (1)
    Framework: NotRequired[str],
    FrameworkVersion: NotRequired[str],
    NearestModelName: NotRequired[str],
```

1. See [:material-code-braces: ModelInputTypeDef](./type_defs.md#modelinputtypedef) 
## RecommendationJobStoppingConditionsTypeDef

```python
# RecommendationJobStoppingConditionsTypeDef definition

class RecommendationJobStoppingConditionsTypeDef(TypedDict):
    MaxInvocations: NotRequired[int],
    ModelLatencyThresholds: NotRequired[Sequence[ModelLatencyThresholdTypeDef]],  # (1)
    FlatInvocations: NotRequired[FlatInvocationsType],  # (2)
```

1. See [:material-code-braces: ModelLatencyThresholdTypeDef](./type_defs.md#modellatencythresholdtypedef) 
2. See [:material-code-brackets: FlatInvocationsType](./literals.md#flatinvocationstype) 
## ModelMetadataSearchExpressionTypeDef

```python
# ModelMetadataSearchExpressionTypeDef definition

class ModelMetadataSearchExpressionTypeDef(TypedDict):
    Filters: NotRequired[Sequence[ModelMetadataFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: ModelMetadataFilterTypeDef](./type_defs.md#modelmetadatafiltertypedef) 
## ModelPackageStatusDetailsTypeDef

```python
# ModelPackageStatusDetailsTypeDef definition

class ModelPackageStatusDetailsTypeDef(TypedDict):
    ValidationStatuses: List[ModelPackageStatusItemTypeDef],  # (1)
    ImageScanStatuses: NotRequired[List[ModelPackageStatusItemTypeDef]],  # (1)
```

1. See [:material-code-braces: ModelPackageStatusItemTypeDef](./type_defs.md#modelpackagestatusitemtypedef) 
2. See [:material-code-braces: ModelPackageStatusItemTypeDef](./type_defs.md#modelpackagestatusitemtypedef) 
## MonitoringResourcesTypeDef

```python
# MonitoringResourcesTypeDef definition

class MonitoringResourcesTypeDef(TypedDict):
    ClusterConfig: MonitoringClusterConfigTypeDef,  # (1)
```

1. See [:material-code-braces: MonitoringClusterConfigTypeDef](./type_defs.md#monitoringclusterconfigtypedef) 
## MonitoringDatasetFormatTypeDef

```python
# MonitoringDatasetFormatTypeDef definition

class MonitoringDatasetFormatTypeDef(TypedDict):
    Csv: NotRequired[MonitoringCsvDatasetFormatTypeDef],  # (1)
    Json: NotRequired[MonitoringJsonDatasetFormatTypeDef],  # (2)
    Parquet: NotRequired[Mapping[str, Any]],
```

1. See [:material-code-braces: MonitoringCsvDatasetFormatTypeDef](./type_defs.md#monitoringcsvdatasetformattypedef) 
2. See [:material-code-braces: MonitoringJsonDatasetFormatTypeDef](./type_defs.md#monitoringjsondatasetformattypedef) 
## MonitoringOutputTypeDef

```python
# MonitoringOutputTypeDef definition

class MonitoringOutputTypeDef(TypedDict):
    S3Output: MonitoringS3OutputTypeDef,  # (1)
```

1. See [:material-code-braces: MonitoringS3OutputTypeDef](./type_defs.md#monitorings3outputtypedef) 
## OfflineStoreConfigTypeDef

```python
# OfflineStoreConfigTypeDef definition

class OfflineStoreConfigTypeDef(TypedDict):
    S3StorageConfig: S3StorageConfigTypeDef,  # (1)
    DisableGlueTableCreation: NotRequired[bool],
    DataCatalogConfig: NotRequired[DataCatalogConfigTypeDef],  # (2)
    TableFormat: NotRequired[TableFormatType],  # (3)
```

1. See [:material-code-braces: S3StorageConfigTypeDef](./type_defs.md#s3storageconfigtypedef) 
2. See [:material-code-braces: DataCatalogConfigTypeDef](./type_defs.md#datacatalogconfigtypedef) 
3. See [:material-code-brackets: TableFormatType](./literals.md#tableformattype) 
## OnlineStoreConfigTypeDef

```python
# OnlineStoreConfigTypeDef definition

class OnlineStoreConfigTypeDef(TypedDict):
    SecurityConfig: NotRequired[OnlineStoreSecurityConfigTypeDef],  # (1)
    EnableOnlineStore: NotRequired[bool],
    TtlDuration: NotRequired[TtlDurationTypeDef],  # (2)
```

1. See [:material-code-braces: OnlineStoreSecurityConfigTypeDef](./type_defs.md#onlinestoresecurityconfigtypedef) 
2. See [:material-code-braces: TtlDurationTypeDef](./type_defs.md#ttldurationtypedef) 
## OnlineStoreConfigUpdateTypeDef

```python
# OnlineStoreConfigUpdateTypeDef definition

class OnlineStoreConfigUpdateTypeDef(TypedDict):
    TtlDuration: NotRequired[TtlDurationTypeDef],  # (1)
```

1. See [:material-code-braces: TtlDurationTypeDef](./type_defs.md#ttldurationtypedef) 
## OutputConfigTypeDef

```python
# OutputConfigTypeDef definition

class OutputConfigTypeDef(TypedDict):
    S3OutputLocation: str,
    TargetDevice: NotRequired[TargetDeviceType],  # (1)
    TargetPlatform: NotRequired[TargetPlatformTypeDef],  # (2)
    CompilerOptions: NotRequired[str],
    KmsKeyId: NotRequired[str],
```

1. See [:material-code-brackets: TargetDeviceType](./literals.md#targetdevicetype) 
2. See [:material-code-braces: TargetPlatformTypeDef](./type_defs.md#targetplatformtypedef) 
## PendingProductionVariantSummaryTypeDef

```python
# PendingProductionVariantSummaryTypeDef definition

class PendingProductionVariantSummaryTypeDef(TypedDict):
    VariantName: str,
    DeployedImages: NotRequired[List[DeployedImageTypeDef]],  # (1)
    CurrentWeight: NotRequired[float],
    DesiredWeight: NotRequired[float],
    CurrentInstanceCount: NotRequired[int],
    DesiredInstanceCount: NotRequired[int],
    InstanceType: NotRequired[ProductionVariantInstanceTypeType],  # (2)
    AcceleratorType: NotRequired[ProductionVariantAcceleratorTypeType],  # (3)
    VariantStatus: NotRequired[List[ProductionVariantStatusTypeDef]],  # (4)
    CurrentServerlessConfig: NotRequired[ProductionVariantServerlessConfigTypeDef],  # (5)
    DesiredServerlessConfig: NotRequired[ProductionVariantServerlessConfigTypeDef],  # (5)
```

1. See [:material-code-braces: DeployedImageTypeDef](./type_defs.md#deployedimagetypedef) 
2. See [:material-code-brackets: ProductionVariantInstanceTypeType](./literals.md#productionvariantinstancetypetype) 
3. See [:material-code-brackets: ProductionVariantAcceleratorTypeType](./literals.md#productionvariantacceleratortypetype) 
4. See [:material-code-braces: ProductionVariantStatusTypeDef](./type_defs.md#productionvariantstatustypedef) 
5. See [:material-code-braces: ProductionVariantServerlessConfigTypeDef](./type_defs.md#productionvariantserverlessconfigtypedef) 
6. See [:material-code-braces: ProductionVariantServerlessConfigTypeDef](./type_defs.md#productionvariantserverlessconfigtypedef) 
## ProductionVariantSummaryTypeDef

```python
# ProductionVariantSummaryTypeDef definition

class ProductionVariantSummaryTypeDef(TypedDict):
    VariantName: str,
    DeployedImages: NotRequired[List[DeployedImageTypeDef]],  # (1)
    CurrentWeight: NotRequired[float],
    DesiredWeight: NotRequired[float],
    CurrentInstanceCount: NotRequired[int],
    DesiredInstanceCount: NotRequired[int],
    VariantStatus: NotRequired[List[ProductionVariantStatusTypeDef]],  # (2)
    CurrentServerlessConfig: NotRequired[ProductionVariantServerlessConfigTypeDef],  # (3)
    DesiredServerlessConfig: NotRequired[ProductionVariantServerlessConfigTypeDef],  # (3)
```

1. See [:material-code-braces: DeployedImageTypeDef](./type_defs.md#deployedimagetypedef) 
2. See [:material-code-braces: ProductionVariantStatusTypeDef](./type_defs.md#productionvariantstatustypedef) 
3. See [:material-code-braces: ProductionVariantServerlessConfigTypeDef](./type_defs.md#productionvariantserverlessconfigtypedef) 
4. See [:material-code-braces: ProductionVariantServerlessConfigTypeDef](./type_defs.md#productionvariantserverlessconfigtypedef) 
## ProcessingResourcesTypeDef

```python
# ProcessingResourcesTypeDef definition

class ProcessingResourcesTypeDef(TypedDict):
    ClusterConfig: ProcessingClusterConfigTypeDef,  # (1)
```

1. See [:material-code-braces: ProcessingClusterConfigTypeDef](./type_defs.md#processingclusterconfigtypedef) 
## ProcessingOutputTypeDef

```python
# ProcessingOutputTypeDef definition

class ProcessingOutputTypeDef(TypedDict):
    OutputName: str,
    S3Output: NotRequired[ProcessingS3OutputTypeDef],  # (1)
    FeatureStoreOutput: NotRequired[ProcessingFeatureStoreOutputTypeDef],  # (2)
    AppManaged: NotRequired[bool],
```

1. See [:material-code-braces: ProcessingS3OutputTypeDef](./type_defs.md#processings3outputtypedef) 
2. See [:material-code-braces: ProcessingFeatureStoreOutputTypeDef](./type_defs.md#processingfeaturestoreoutputtypedef) 
## ProductionVariantTypeDef

```python
# ProductionVariantTypeDef definition

class ProductionVariantTypeDef(TypedDict):
    VariantName: str,
    ModelName: str,
    InitialInstanceCount: NotRequired[int],
    InstanceType: NotRequired[ProductionVariantInstanceTypeType],  # (1)
    InitialVariantWeight: NotRequired[float],
    AcceleratorType: NotRequired[ProductionVariantAcceleratorTypeType],  # (2)
    CoreDumpConfig: NotRequired[ProductionVariantCoreDumpConfigTypeDef],  # (3)
    ServerlessConfig: NotRequired[ProductionVariantServerlessConfigTypeDef],  # (4)
    VolumeSizeInGB: NotRequired[int],
    ModelDataDownloadTimeoutInSeconds: NotRequired[int],
    ContainerStartupHealthCheckTimeoutInSeconds: NotRequired[int],
    EnableSSMAccess: NotRequired[bool],
```

1. See [:material-code-brackets: ProductionVariantInstanceTypeType](./literals.md#productionvariantinstancetypetype) 
2. See [:material-code-brackets: ProductionVariantAcceleratorTypeType](./literals.md#productionvariantacceleratortypetype) 
3. See [:material-code-braces: ProductionVariantCoreDumpConfigTypeDef](./type_defs.md#productionvariantcoredumpconfigtypedef) 
4. See [:material-code-braces: ProductionVariantServerlessConfigTypeDef](./type_defs.md#productionvariantserverlessconfigtypedef) 
## SuggestionQueryTypeDef

```python
# SuggestionQueryTypeDef definition

class SuggestionQueryTypeDef(TypedDict):
    PropertyNameQuery: NotRequired[PropertyNameQueryTypeDef],  # (1)
```

1. See [:material-code-braces: PropertyNameQueryTypeDef](./type_defs.md#propertynamequerytypedef) 
## ServiceCatalogProvisioningDetailsTypeDef

```python
# ServiceCatalogProvisioningDetailsTypeDef definition

class ServiceCatalogProvisioningDetailsTypeDef(TypedDict):
    ProductId: str,
    ProvisioningArtifactId: NotRequired[str],
    PathId: NotRequired[str],
    ProvisioningParameters: NotRequired[Sequence[ProvisioningParameterTypeDef]],  # (1)
```

1. See [:material-code-braces: ProvisioningParameterTypeDef](./type_defs.md#provisioningparametertypedef) 
## ServiceCatalogProvisioningUpdateDetailsTypeDef

```python
# ServiceCatalogProvisioningUpdateDetailsTypeDef definition

class ServiceCatalogProvisioningUpdateDetailsTypeDef(TypedDict):
    ProvisioningArtifactId: NotRequired[str],
    ProvisioningParameters: NotRequired[Sequence[ProvisioningParameterTypeDef]],  # (1)
```

1. See [:material-code-braces: ProvisioningParameterTypeDef](./type_defs.md#provisioningparametertypedef) 
## PublicWorkforceTaskPriceTypeDef

```python
# PublicWorkforceTaskPriceTypeDef definition

class PublicWorkforceTaskPriceTypeDef(TypedDict):
    AmountInUsd: NotRequired[USDTypeDef],  # (1)
```

1. See [:material-code-braces: USDTypeDef](./type_defs.md#usdtypedef) 
## QueryLineageResponseTypeDef

```python
# QueryLineageResponseTypeDef definition

class QueryLineageResponseTypeDef(TypedDict):
    Vertices: List[VertexTypeDef],  # (1)
    Edges: List[EdgeTypeDef],  # (2)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: VertexTypeDef](./type_defs.md#vertextypedef) 
2. See [:material-code-braces: EdgeTypeDef](./type_defs.md#edgetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RecommendationJobOutputConfigTypeDef

```python
# RecommendationJobOutputConfigTypeDef definition

class RecommendationJobOutputConfigTypeDef(TypedDict):
    KmsKeyId: NotRequired[str],
    CompiledOutputConfig: NotRequired[RecommendationJobCompiledOutputConfigTypeDef],  # (1)
```

1. See [:material-code-braces: RecommendationJobCompiledOutputConfigTypeDef](./type_defs.md#recommendationjobcompiledoutputconfigtypedef) 
## RecommendationJobContainerConfigTypeDef

```python
# RecommendationJobContainerConfigTypeDef definition

class RecommendationJobContainerConfigTypeDef(TypedDict):
    Domain: NotRequired[str],
    Task: NotRequired[str],
    Framework: NotRequired[str],
    FrameworkVersion: NotRequired[str],
    PayloadConfig: NotRequired[RecommendationJobPayloadConfigTypeDef],  # (1)
    NearestModelName: NotRequired[str],
    SupportedInstanceTypes: NotRequired[Sequence[str]],
    DataInputConfig: NotRequired[str],
    SupportedEndpointType: NotRequired[RecommendationJobSupportedEndpointTypeType],  # (2)
```

1. See [:material-code-braces: RecommendationJobPayloadConfigTypeDef](./type_defs.md#recommendationjobpayloadconfigtypedef) 
2. See [:material-code-brackets: RecommendationJobSupportedEndpointTypeType](./literals.md#recommendationjobsupportedendpointtypetype) 
## RenderUiTemplateRequestRequestTypeDef

```python
# RenderUiTemplateRequestRequestTypeDef definition

class RenderUiTemplateRequestRequestTypeDef(TypedDict):
    Task: RenderableTaskTypeDef,  # (1)
    RoleArn: str,
    UiTemplate: NotRequired[UiTemplateTypeDef],  # (2)
    HumanTaskUiArn: NotRequired[str],
```

1. See [:material-code-braces: RenderableTaskTypeDef](./type_defs.md#renderabletasktypedef) 
2. See [:material-code-braces: UiTemplateTypeDef](./type_defs.md#uitemplatetypedef) 
## RenderUiTemplateResponseTypeDef

```python
# RenderUiTemplateResponseTypeDef definition

class RenderUiTemplateResponseTypeDef(TypedDict):
    RenderedContent: str,
    Errors: List[RenderingErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RenderingErrorTypeDef](./type_defs.md#renderingerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTrainingJobRequestRequestTypeDef

```python
# UpdateTrainingJobRequestRequestTypeDef definition

class UpdateTrainingJobRequestRequestTypeDef(TypedDict):
    TrainingJobName: str,
    ProfilerConfig: NotRequired[ProfilerConfigForUpdateTypeDef],  # (1)
    ProfilerRuleConfigurations: NotRequired[Sequence[ProfilerRuleConfigurationTypeDef]],  # (2)
    ResourceConfig: NotRequired[ResourceConfigForUpdateTypeDef],  # (3)
```

1. See [:material-code-braces: ProfilerConfigForUpdateTypeDef](./type_defs.md#profilerconfigforupdatetypedef) 
2. See [:material-code-braces: ProfilerRuleConfigurationTypeDef](./type_defs.md#profilerruleconfigurationtypedef) 
3. See [:material-code-braces: ResourceConfigForUpdateTypeDef](./type_defs.md#resourceconfigforupdatetypedef) 
## SelectiveExecutionConfigTypeDef

```python
# SelectiveExecutionConfigTypeDef definition

class SelectiveExecutionConfigTypeDef(TypedDict):
    SourcePipelineExecutionArn: str,
    SelectedSteps: List[SelectedStepTypeDef],  # (1)
```

1. See [:material-code-braces: SelectedStepTypeDef](./type_defs.md#selectedsteptypedef) 
## ShadowModeConfigTypeDef

```python
# ShadowModeConfigTypeDef definition

class ShadowModeConfigTypeDef(TypedDict):
    SourceModelVariantName: str,
    ShadowModelVariants: Sequence[ShadowModelVariantConfigTypeDef],  # (1)
```

1. See [:material-code-braces: ShadowModelVariantConfigTypeDef](./type_defs.md#shadowmodelvariantconfigtypedef) 
## SourceAlgorithmSpecificationTypeDef

```python
# SourceAlgorithmSpecificationTypeDef definition

class SourceAlgorithmSpecificationTypeDef(TypedDict):
    SourceAlgorithms: Sequence[SourceAlgorithmTypeDef],  # (1)
```

1. See [:material-code-braces: SourceAlgorithmTypeDef](./type_defs.md#sourcealgorithmtypedef) 
## TrafficPatternTypeDef

```python
# TrafficPatternTypeDef definition

class TrafficPatternTypeDef(TypedDict):
    TrafficType: NotRequired[TrafficTypeType],  # (1)
    Phases: NotRequired[Sequence[PhaseTypeDef]],  # (2)
    Stairs: NotRequired[StairsTypeDef],  # (3)
```

1. See [:material-code-brackets: TrafficTypeType](./literals.md#traffictypetype) 
2. See [:material-code-braces: PhaseTypeDef](./type_defs.md#phasetypedef) 
3. See [:material-code-braces: StairsTypeDef](./type_defs.md#stairstypedef) 
## TimeSeriesForecastingJobConfigTypeDef

```python
# TimeSeriesForecastingJobConfigTypeDef definition

class TimeSeriesForecastingJobConfigTypeDef(TypedDict):
    ForecastFrequency: str,
    ForecastHorizon: int,
    TimeSeriesConfig: TimeSeriesConfigTypeDef,  # (3)
    FeatureSpecificationS3Uri: NotRequired[str],
    CompletionCriteria: NotRequired[AutoMLJobCompletionCriteriaTypeDef],  # (1)
    ForecastQuantiles: NotRequired[Sequence[str]],
    Transformations: NotRequired[TimeSeriesTransformationsTypeDef],  # (2)
```

1. See [:material-code-braces: AutoMLJobCompletionCriteriaTypeDef](./type_defs.md#automljobcompletioncriteriatypedef) 
2. See [:material-code-braces: TimeSeriesTransformationsTypeDef](./type_defs.md#timeseriestransformationstypedef) 
3. See [:material-code-braces: TimeSeriesConfigTypeDef](./type_defs.md#timeseriesconfigtypedef) 
## TrainingImageConfigTypeDef

```python
# TrainingImageConfigTypeDef definition

class TrainingImageConfigTypeDef(TypedDict):
    TrainingRepositoryAccessMode: TrainingRepositoryAccessModeType,  # (1)
    TrainingRepositoryAuthConfig: NotRequired[TrainingRepositoryAuthConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: TrainingRepositoryAccessModeType](./literals.md#trainingrepositoryaccessmodetype) 
2. See [:material-code-braces: TrainingRepositoryAuthConfigTypeDef](./type_defs.md#trainingrepositoryauthconfigtypedef) 
## TransformDataSourceTypeDef

```python
# TransformDataSourceTypeDef definition

class TransformDataSourceTypeDef(TypedDict):
    S3DataSource: TransformS3DataSourceTypeDef,  # (1)
```

1. See [:material-code-braces: TransformS3DataSourceTypeDef](./type_defs.md#transforms3datasourcetypedef) 
## WorkforceTypeDef

```python
# WorkforceTypeDef definition

class WorkforceTypeDef(TypedDict):
    WorkforceName: str,
    WorkforceArn: str,
    LastUpdatedDate: NotRequired[datetime],
    SourceIpConfig: NotRequired[SourceIpConfigTypeDef],  # (1)
    SubDomain: NotRequired[str],
    CognitoConfig: NotRequired[CognitoConfigTypeDef],  # (2)
    OidcConfig: NotRequired[OidcConfigForResponseTypeDef],  # (3)
    CreateDate: NotRequired[datetime],
    WorkforceVpcConfig: NotRequired[WorkforceVpcConfigResponseTypeDef],  # (4)
    Status: NotRequired[WorkforceStatusType],  # (5)
    FailureReason: NotRequired[str],
```

1. See [:material-code-braces: SourceIpConfigTypeDef](./type_defs.md#sourceipconfigtypedef) 
2. See [:material-code-braces: CognitoConfigTypeDef](./type_defs.md#cognitoconfigtypedef) 
3. See [:material-code-braces: OidcConfigForResponseTypeDef](./type_defs.md#oidcconfigforresponsetypedef) 
4. See [:material-code-braces: WorkforceVpcConfigResponseTypeDef](./type_defs.md#workforcevpcconfigresponsetypedef) 
5. See [:material-code-brackets: WorkforceStatusType](./literals.md#workforcestatustype) 
## ListActionsResponseTypeDef

```python
# ListActionsResponseTypeDef definition

class ListActionsResponseTypeDef(TypedDict):
    ActionSummaries: List[ActionSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ActionSummaryTypeDef](./type_defs.md#actionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ArtifactSummaryTypeDef

```python
# ArtifactSummaryTypeDef definition

class ArtifactSummaryTypeDef(TypedDict):
    ArtifactArn: NotRequired[str],
    ArtifactName: NotRequired[str],
    Source: NotRequired[ArtifactSourceTypeDef],  # (1)
    ArtifactType: NotRequired[str],
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
```

1. See [:material-code-braces: ArtifactSourceTypeDef](./type_defs.md#artifactsourcetypedef) 
## CreateArtifactRequestRequestTypeDef

```python
# CreateArtifactRequestRequestTypeDef definition

class CreateArtifactRequestRequestTypeDef(TypedDict):
    Source: ArtifactSourceTypeDef,  # (1)
    ArtifactType: str,
    ArtifactName: NotRequired[str],
    Properties: NotRequired[Mapping[str, str]],
    MetadataProperties: NotRequired[MetadataPropertiesTypeDef],  # (2)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: ArtifactSourceTypeDef](./type_defs.md#artifactsourcetypedef) 
2. See [:material-code-braces: MetadataPropertiesTypeDef](./type_defs.md#metadatapropertiestypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DeleteArtifactRequestRequestTypeDef

```python
# DeleteArtifactRequestRequestTypeDef definition

class DeleteArtifactRequestRequestTypeDef(TypedDict):
    ArtifactArn: NotRequired[str],
    Source: NotRequired[ArtifactSourceTypeDef],  # (1)
```

1. See [:material-code-braces: ArtifactSourceTypeDef](./type_defs.md#artifactsourcetypedef) 
## AsyncInferenceConfigTypeDef

```python
# AsyncInferenceConfigTypeDef definition

class AsyncInferenceConfigTypeDef(TypedDict):
    OutputConfig: AsyncInferenceOutputConfigTypeDef,  # (2)
    ClientConfig: NotRequired[AsyncInferenceClientConfigTypeDef],  # (1)
```

1. See [:material-code-braces: AsyncInferenceClientConfigTypeDef](./type_defs.md#asyncinferenceclientconfigtypedef) 
2. See [:material-code-braces: AsyncInferenceOutputConfigTypeDef](./type_defs.md#asyncinferenceoutputconfigtypedef) 
## TabularJobConfigTypeDef

```python
# TabularJobConfigTypeDef definition

class TabularJobConfigTypeDef(TypedDict):
    TargetAttributeName: str,
    CandidateGenerationConfig: NotRequired[CandidateGenerationConfigTypeDef],  # (1)
    CompletionCriteria: NotRequired[AutoMLJobCompletionCriteriaTypeDef],  # (2)
    FeatureSpecificationS3Uri: NotRequired[str],
    Mode: NotRequired[AutoMLModeType],  # (3)
    GenerateCandidateDefinitionsOnly: NotRequired[bool],
    ProblemType: NotRequired[ProblemTypeType],  # (4)
    SampleWeightAttributeName: NotRequired[str],
```

1. See [:material-code-braces: CandidateGenerationConfigTypeDef](./type_defs.md#candidategenerationconfigtypedef) 
2. See [:material-code-braces: AutoMLJobCompletionCriteriaTypeDef](./type_defs.md#automljobcompletioncriteriatypedef) 
3. See [:material-code-brackets: AutoMLModeType](./literals.md#automlmodetype) 
4. See [:material-code-brackets: ProblemTypeType](./literals.md#problemtypetype) 
## AutoMLChannelTypeDef

```python
# AutoMLChannelTypeDef definition

class AutoMLChannelTypeDef(TypedDict):
    DataSource: AutoMLDataSourceTypeDef,  # (1)
    TargetAttributeName: str,
    CompressionType: NotRequired[CompressionTypeType],  # (2)
    ContentType: NotRequired[str],
    ChannelType: NotRequired[AutoMLChannelTypeType],  # (3)
    SampleWeightAttributeName: NotRequired[str],
```

1. See [:material-code-braces: AutoMLDataSourceTypeDef](./type_defs.md#automldatasourcetypedef) 
2. See [:material-code-brackets: CompressionTypeType](./literals.md#compressiontypetype) 
3. See [:material-code-brackets: AutoMLChannelTypeType](./literals.md#automlchanneltypetype) 
## AutoMLJobChannelTypeDef

```python
# AutoMLJobChannelTypeDef definition

class AutoMLJobChannelTypeDef(TypedDict):
    ChannelType: NotRequired[AutoMLChannelTypeType],  # (1)
    ContentType: NotRequired[str],
    CompressionType: NotRequired[CompressionTypeType],  # (2)
    DataSource: NotRequired[AutoMLDataSourceTypeDef],  # (3)
```

1. See [:material-code-brackets: AutoMLChannelTypeType](./literals.md#automlchanneltypetype) 
2. See [:material-code-brackets: CompressionTypeType](./literals.md#compressiontypetype) 
3. See [:material-code-braces: AutoMLDataSourceTypeDef](./type_defs.md#automldatasourcetypedef) 
## ListAutoMLJobsResponseTypeDef

```python
# ListAutoMLJobsResponseTypeDef definition

class ListAutoMLJobsResponseTypeDef(TypedDict):
    AutoMLJobSummaries: List[AutoMLJobSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AutoMLJobSummaryTypeDef](./type_defs.md#automljobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AutoMLResolvedAttributesTypeDef

```python
# AutoMLResolvedAttributesTypeDef definition

class AutoMLResolvedAttributesTypeDef(TypedDict):
    AutoMLJobObjective: NotRequired[AutoMLJobObjectiveTypeDef],  # (1)
    CompletionCriteria: NotRequired[AutoMLJobCompletionCriteriaTypeDef],  # (2)
    AutoMLProblemTypeResolvedAttributes: NotRequired[AutoMLProblemTypeResolvedAttributesTypeDef],  # (3)
```

1. See [:material-code-braces: AutoMLJobObjectiveTypeDef](./type_defs.md#automljobobjectivetypedef) 
2. See [:material-code-braces: AutoMLJobCompletionCriteriaTypeDef](./type_defs.md#automljobcompletioncriteriatypedef) 
3. See [:material-code-braces: AutoMLProblemTypeResolvedAttributesTypeDef](./type_defs.md#automlproblemtyperesolvedattributestypedef) 
## AutoMLJobConfigTypeDef

```python
# AutoMLJobConfigTypeDef definition

class AutoMLJobConfigTypeDef(TypedDict):
    CompletionCriteria: NotRequired[AutoMLJobCompletionCriteriaTypeDef],  # (1)
    SecurityConfig: NotRequired[AutoMLSecurityConfigTypeDef],  # (2)
    DataSplitConfig: NotRequired[AutoMLDataSplitConfigTypeDef],  # (3)
    CandidateGenerationConfig: NotRequired[AutoMLCandidateGenerationConfigTypeDef],  # (4)
    Mode: NotRequired[AutoMLModeType],  # (5)
```

1. See [:material-code-braces: AutoMLJobCompletionCriteriaTypeDef](./type_defs.md#automljobcompletioncriteriatypedef) 
2. See [:material-code-braces: AutoMLSecurityConfigTypeDef](./type_defs.md#automlsecurityconfigtypedef) 
3. See [:material-code-braces: AutoMLDataSplitConfigTypeDef](./type_defs.md#automldatasplitconfigtypedef) 
4. See [:material-code-braces: AutoMLCandidateGenerationConfigTypeDef](./type_defs.md#automlcandidategenerationconfigtypedef) 
5. See [:material-code-brackets: AutoMLModeType](./literals.md#automlmodetype) 
## LabelingJobAlgorithmsConfigTypeDef

```python
# LabelingJobAlgorithmsConfigTypeDef definition

class LabelingJobAlgorithmsConfigTypeDef(TypedDict):
    LabelingJobAlgorithmSpecificationArn: str,
    InitialActiveLearningModelArn: NotRequired[str],
    LabelingJobResourceConfig: NotRequired[LabelingJobResourceConfigTypeDef],  # (1)
```

1. See [:material-code-braces: LabelingJobResourceConfigTypeDef](./type_defs.md#labelingjobresourceconfigtypedef) 
## ModelMetricsTypeDef

```python
# ModelMetricsTypeDef definition

class ModelMetricsTypeDef(TypedDict):
    ModelQuality: NotRequired[ModelQualityTypeDef],  # (1)
    ModelDataQuality: NotRequired[ModelDataQualityTypeDef],  # (2)
    Bias: NotRequired[BiasTypeDef],  # (3)
    Explainability: NotRequired[ExplainabilityTypeDef],  # (4)
```

1. See [:material-code-braces: ModelQualityTypeDef](./type_defs.md#modelqualitytypedef) 
2. See [:material-code-braces: ModelDataQualityTypeDef](./type_defs.md#modeldataqualitytypedef) 
3. See [:material-code-braces: BiasTypeDef](./type_defs.md#biastypedef) 
4. See [:material-code-braces: ExplainabilityTypeDef](./type_defs.md#explainabilitytypedef) 
## PipelineExecutionStepMetadataTypeDef

```python
# PipelineExecutionStepMetadataTypeDef definition

class PipelineExecutionStepMetadataTypeDef(TypedDict):
    TrainingJob: NotRequired[TrainingJobStepMetadataTypeDef],  # (1)
    ProcessingJob: NotRequired[ProcessingJobStepMetadataTypeDef],  # (2)
    TransformJob: NotRequired[TransformJobStepMetadataTypeDef],  # (3)
    TuningJob: NotRequired[TuningJobStepMetaDataTypeDef],  # (4)
    Model: NotRequired[ModelStepMetadataTypeDef],  # (5)
    RegisterModel: NotRequired[RegisterModelStepMetadataTypeDef],  # (6)
    Condition: NotRequired[ConditionStepMetadataTypeDef],  # (7)
    Callback: NotRequired[CallbackStepMetadataTypeDef],  # (8)
    Lambda: NotRequired[LambdaStepMetadataTypeDef],  # (9)
    QualityCheck: NotRequired[QualityCheckStepMetadataTypeDef],  # (10)
    ClarifyCheck: NotRequired[ClarifyCheckStepMetadataTypeDef],  # (11)
    EMR: NotRequired[EMRStepMetadataTypeDef],  # (12)
    Fail: NotRequired[FailStepMetadataTypeDef],  # (13)
    AutoMLJob: NotRequired[AutoMLJobStepMetadataTypeDef],  # (14)
```

1. See [:material-code-braces: TrainingJobStepMetadataTypeDef](./type_defs.md#trainingjobstepmetadatatypedef) 
2. See [:material-code-braces: ProcessingJobStepMetadataTypeDef](./type_defs.md#processingjobstepmetadatatypedef) 
3. See [:material-code-braces: TransformJobStepMetadataTypeDef](./type_defs.md#transformjobstepmetadatatypedef) 
4. See [:material-code-braces: TuningJobStepMetaDataTypeDef](./type_defs.md#tuningjobstepmetadatatypedef) 
5. See [:material-code-braces: ModelStepMetadataTypeDef](./type_defs.md#modelstepmetadatatypedef) 
6. See [:material-code-braces: RegisterModelStepMetadataTypeDef](./type_defs.md#registermodelstepmetadatatypedef) 
7. See [:material-code-braces: ConditionStepMetadataTypeDef](./type_defs.md#conditionstepmetadatatypedef) 
8. See [:material-code-braces: CallbackStepMetadataTypeDef](./type_defs.md#callbackstepmetadatatypedef) 
9. See [:material-code-braces: LambdaStepMetadataTypeDef](./type_defs.md#lambdastepmetadatatypedef) 
10. See [:material-code-braces: QualityCheckStepMetadataTypeDef](./type_defs.md#qualitycheckstepmetadatatypedef) 
11. See [:material-code-braces: ClarifyCheckStepMetadataTypeDef](./type_defs.md#clarifycheckstepmetadatatypedef) 
12. See [:material-code-braces: EMRStepMetadataTypeDef](./type_defs.md#emrstepmetadatatypedef) 
13. See [:material-code-braces: FailStepMetadataTypeDef](./type_defs.md#failstepmetadatatypedef) 
14. See [:material-code-braces: AutoMLJobStepMetadataTypeDef](./type_defs.md#automljobstepmetadatatypedef) 
## AutoMLCandidateTypeDef

```python
# AutoMLCandidateTypeDef definition

class AutoMLCandidateTypeDef(TypedDict):
    CandidateName: str,
    ObjectiveStatus: ObjectiveStatusType,  # (2)
    CandidateSteps: List[AutoMLCandidateStepTypeDef],  # (3)
    CandidateStatus: CandidateStatusType,  # (4)
    CreationTime: datetime,
    LastModifiedTime: datetime,
    FinalAutoMLJobObjectiveMetric: NotRequired[FinalAutoMLJobObjectiveMetricTypeDef],  # (1)
    InferenceContainers: NotRequired[List[AutoMLContainerDefinitionTypeDef]],  # (5)
    EndTime: NotRequired[datetime],
    FailureReason: NotRequired[str],
    CandidateProperties: NotRequired[CandidatePropertiesTypeDef],  # (6)
    InferenceContainerDefinitions: NotRequired[Dict[AutoMLProcessingUnitType, List[AutoMLContainerDefinitionTypeDef]]],  # (7)
```

1. See [:material-code-braces: FinalAutoMLJobObjectiveMetricTypeDef](./type_defs.md#finalautomljobobjectivemetrictypedef) 
2. See [:material-code-brackets: ObjectiveStatusType](./literals.md#objectivestatustype) 
3. See [:material-code-braces: AutoMLCandidateStepTypeDef](./type_defs.md#automlcandidatesteptypedef) 
4. See [:material-code-brackets: CandidateStatusType](./literals.md#candidatestatustype) 
5. See [:material-code-braces: AutoMLContainerDefinitionTypeDef](./type_defs.md#automlcontainerdefinitiontypedef) 
6. See [:material-code-braces: CandidatePropertiesTypeDef](./type_defs.md#candidatepropertiestypedef) 
7. See [:material-code-brackets: AutoMLProcessingUnitType](./literals.md#automlprocessingunittype) [:material-code-braces: AutoMLContainerDefinitionTypeDef](./type_defs.md#automlcontainerdefinitiontypedef) 
## BlueGreenUpdatePolicyTypeDef

```python
# BlueGreenUpdatePolicyTypeDef definition

class BlueGreenUpdatePolicyTypeDef(TypedDict):
    TrafficRoutingConfiguration: TrafficRoutingConfigTypeDef,  # (1)
    TerminationWaitInSeconds: NotRequired[int],
    MaximumExecutionTimeoutInSeconds: NotRequired[int],
```

1. See [:material-code-braces: TrafficRoutingConfigTypeDef](./type_defs.md#trafficroutingconfigtypedef) 
## EndpointInputConfigurationTypeDef

```python
# EndpointInputConfigurationTypeDef definition

class EndpointInputConfigurationTypeDef(TypedDict):
    InstanceType: NotRequired[ProductionVariantInstanceTypeType],  # (1)
    InferenceSpecificationName: NotRequired[str],
    EnvironmentParameterRanges: NotRequired[EnvironmentParameterRangesTypeDef],  # (2)
    ServerlessConfig: NotRequired[ProductionVariantServerlessConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ProductionVariantInstanceTypeType](./literals.md#productionvariantinstancetypetype) 
2. See [:material-code-braces: EnvironmentParameterRangesTypeDef](./type_defs.md#environmentparameterrangestypedef) 
3. See [:material-code-braces: ProductionVariantServerlessConfigTypeDef](./type_defs.md#productionvariantserverlessconfigtypedef) 
## ClarifyExplainerConfigTypeDef

```python
# ClarifyExplainerConfigTypeDef definition

class ClarifyExplainerConfigTypeDef(TypedDict):
    ShapConfig: ClarifyShapConfigTypeDef,  # (2)
    EnableExplanations: NotRequired[str],
    InferenceConfig: NotRequired[ClarifyInferenceConfigTypeDef],  # (1)
```

1. See [:material-code-braces: ClarifyInferenceConfigTypeDef](./type_defs.md#clarifyinferenceconfigtypedef) 
2. See [:material-code-braces: ClarifyShapConfigTypeDef](./type_defs.md#clarifyshapconfigtypedef) 
## ListCodeRepositoriesOutputTypeDef

```python
# ListCodeRepositoriesOutputTypeDef definition

class ListCodeRepositoriesOutputTypeDef(TypedDict):
    CodeRepositorySummaryList: List[CodeRepositorySummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CodeRepositorySummaryTypeDef](./type_defs.md#coderepositorysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListContextsResponseTypeDef

```python
# ListContextsResponseTypeDef definition

class ListContextsResponseTypeDef(TypedDict):
    ContextSummaries: List[ContextSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContextSummaryTypeDef](./type_defs.md#contextsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DomainSettingsForUpdateTypeDef

```python
# DomainSettingsForUpdateTypeDef definition

class DomainSettingsForUpdateTypeDef(TypedDict):
    RStudioServerProDomainSettingsForUpdate: NotRequired[RStudioServerProDomainSettingsForUpdateTypeDef],  # (1)
    ExecutionRoleIdentityConfig: NotRequired[ExecutionRoleIdentityConfigType],  # (2)
    SecurityGroupIds: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: RStudioServerProDomainSettingsForUpdateTypeDef](./type_defs.md#rstudioserverprodomainsettingsforupdatetypedef) 
2. See [:material-code-brackets: ExecutionRoleIdentityConfigType](./literals.md#executionroleidentityconfigtype) 
## DomainSettingsTypeDef

```python
# DomainSettingsTypeDef definition

class DomainSettingsTypeDef(TypedDict):
    SecurityGroupIds: NotRequired[Sequence[str]],
    RStudioServerProDomainSettings: NotRequired[RStudioServerProDomainSettingsTypeDef],  # (1)
    ExecutionRoleIdentityConfig: NotRequired[ExecutionRoleIdentityConfigType],  # (2)
```

1. See [:material-code-braces: RStudioServerProDomainSettingsTypeDef](./type_defs.md#rstudioserverprodomainsettingstypedef) 
2. See [:material-code-brackets: ExecutionRoleIdentityConfigType](./literals.md#executionroleidentityconfigtype) 
## InferenceExperimentSummaryTypeDef

```python
# InferenceExperimentSummaryTypeDef definition

class InferenceExperimentSummaryTypeDef(TypedDict):
    Name: str,
    Type: InferenceExperimentTypeType,  # (1)
    Status: InferenceExperimentStatusType,  # (3)
    CreationTime: datetime,
    LastModifiedTime: datetime,
    Schedule: NotRequired[InferenceExperimentScheduleTypeDef],  # (2)
    StatusReason: NotRequired[str],
    Description: NotRequired[str],
    CompletionTime: NotRequired[datetime],
    RoleArn: NotRequired[str],
```

1. See [:material-code-brackets: InferenceExperimentTypeType](./literals.md#inferenceexperimenttypetype) 
2. See [:material-code-braces: InferenceExperimentScheduleTypeDef](./type_defs.md#inferenceexperimentscheduletypedef) 
3. See [:material-code-brackets: InferenceExperimentStatusType](./literals.md#inferenceexperimentstatustype) 
## QueryLineageRequestRequestTypeDef

```python
# QueryLineageRequestRequestTypeDef definition

class QueryLineageRequestRequestTypeDef(TypedDict):
    StartArns: NotRequired[Sequence[str]],
    Direction: NotRequired[DirectionType],  # (1)
    IncludeEdges: NotRequired[bool],
    Filters: NotRequired[QueryFiltersTypeDef],  # (2)
    MaxDepth: NotRequired[int],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: DirectionType](./literals.md#directiontype) 
2. See [:material-code-braces: QueryFiltersTypeDef](./type_defs.md#queryfilterstypedef) 
## DefaultSpaceSettingsTypeDef

```python
# DefaultSpaceSettingsTypeDef definition

class DefaultSpaceSettingsTypeDef(TypedDict):
    ExecutionRole: NotRequired[str],
    SecurityGroups: NotRequired[Sequence[str]],
    JupyterServerAppSettings: NotRequired[JupyterServerAppSettingsTypeDef],  # (1)
    KernelGatewayAppSettings: NotRequired[KernelGatewayAppSettingsTypeDef],  # (2)
```

1. See [:material-code-braces: JupyterServerAppSettingsTypeDef](./type_defs.md#jupyterserverappsettingstypedef) 
2. See [:material-code-braces: KernelGatewayAppSettingsTypeDef](./type_defs.md#kernelgatewayappsettingstypedef) 
## SpaceSettingsTypeDef

```python
# SpaceSettingsTypeDef definition

class SpaceSettingsTypeDef(TypedDict):
    JupyterServerAppSettings: NotRequired[JupyterServerAppSettingsTypeDef],  # (1)
    KernelGatewayAppSettings: NotRequired[KernelGatewayAppSettingsTypeDef],  # (2)
```

1. See [:material-code-braces: JupyterServerAppSettingsTypeDef](./type_defs.md#jupyterserverappsettingstypedef) 
2. See [:material-code-braces: KernelGatewayAppSettingsTypeDef](./type_defs.md#kernelgatewayappsettingstypedef) 
## UserSettingsTypeDef

```python
# UserSettingsTypeDef definition

class UserSettingsTypeDef(TypedDict):
    ExecutionRole: NotRequired[str],
    SecurityGroups: NotRequired[Sequence[str]],
    SharingSettings: NotRequired[SharingSettingsTypeDef],  # (1)
    JupyterServerAppSettings: NotRequired[JupyterServerAppSettingsTypeDef],  # (2)
    KernelGatewayAppSettings: NotRequired[KernelGatewayAppSettingsTypeDef],  # (3)
    TensorBoardAppSettings: NotRequired[TensorBoardAppSettingsTypeDef],  # (4)
    RStudioServerProAppSettings: NotRequired[RStudioServerProAppSettingsTypeDef],  # (5)
    RSessionAppSettings: NotRequired[RSessionAppSettingsTypeDef],  # (6)
    CanvasAppSettings: NotRequired[CanvasAppSettingsTypeDef],  # (7)
```

1. See [:material-code-braces: SharingSettingsTypeDef](./type_defs.md#sharingsettingstypedef) 
2. See [:material-code-braces: JupyterServerAppSettingsTypeDef](./type_defs.md#jupyterserverappsettingstypedef) 
3. See [:material-code-braces: KernelGatewayAppSettingsTypeDef](./type_defs.md#kernelgatewayappsettingstypedef) 
4. See [:material-code-braces: TensorBoardAppSettingsTypeDef](./type_defs.md#tensorboardappsettingstypedef) 
5. See [:material-code-braces: RStudioServerProAppSettingsTypeDef](./type_defs.md#rstudioserverproappsettingstypedef) 
6. See [:material-code-braces: RSessionAppSettingsTypeDef](./type_defs.md#rsessionappsettingstypedef) 
7. See [:material-code-braces: CanvasAppSettingsTypeDef](./type_defs.md#canvasappsettingstypedef) 
## ChannelTypeDef

```python
# ChannelTypeDef definition

class ChannelTypeDef(TypedDict):
    ChannelName: str,
    DataSource: DataSourceTypeDef,  # (1)
    ContentType: NotRequired[str],
    CompressionType: NotRequired[CompressionTypeType],  # (2)
    RecordWrapperType: NotRequired[RecordWrapperType],  # (3)
    InputMode: NotRequired[TrainingInputModeType],  # (4)
    ShuffleConfig: NotRequired[ShuffleConfigTypeDef],  # (5)
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
2. See [:material-code-brackets: CompressionTypeType](./literals.md#compressiontypetype) 
3. See [:material-code-brackets: RecordWrapperType](./literals.md#recordwrappertype) 
4. See [:material-code-brackets: TrainingInputModeType](./literals.md#traininginputmodetype) 
5. See [:material-code-braces: ShuffleConfigTypeDef](./type_defs.md#shuffleconfigtypedef) 
## ProcessingInputTypeDef

```python
# ProcessingInputTypeDef definition

class ProcessingInputTypeDef(TypedDict):
    InputName: str,
    AppManaged: NotRequired[bool],
    S3Input: NotRequired[ProcessingS3InputTypeDef],  # (1)
    DatasetDefinition: NotRequired[DatasetDefinitionTypeDef],  # (2)
```

1. See [:material-code-braces: ProcessingS3InputTypeDef](./type_defs.md#processings3inputtypedef) 
2. See [:material-code-braces: DatasetDefinitionTypeDef](./type_defs.md#datasetdefinitiontypedef) 
## CreateEdgeDeploymentPlanRequestRequestTypeDef

```python
# CreateEdgeDeploymentPlanRequestRequestTypeDef definition

class CreateEdgeDeploymentPlanRequestRequestTypeDef(TypedDict):
    EdgeDeploymentPlanName: str,
    ModelConfigs: Sequence[EdgeDeploymentModelConfigTypeDef],  # (1)
    DeviceFleetName: str,
    Stages: NotRequired[Sequence[DeploymentStageTypeDef]],  # (2)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: EdgeDeploymentModelConfigTypeDef](./type_defs.md#edgedeploymentmodelconfigtypedef) 
2. See [:material-code-braces: DeploymentStageTypeDef](./type_defs.md#deploymentstagetypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateEdgeDeploymentStageRequestRequestTypeDef

```python
# CreateEdgeDeploymentStageRequestRequestTypeDef definition

class CreateEdgeDeploymentStageRequestRequestTypeDef(TypedDict):
    EdgeDeploymentPlanName: str,
    Stages: Sequence[DeploymentStageTypeDef],  # (1)
```

1. See [:material-code-braces: DeploymentStageTypeDef](./type_defs.md#deploymentstagetypedef) 
## DescribeEdgeDeploymentPlanResponseTypeDef

```python
# DescribeEdgeDeploymentPlanResponseTypeDef definition

class DescribeEdgeDeploymentPlanResponseTypeDef(TypedDict):
    EdgeDeploymentPlanArn: str,
    EdgeDeploymentPlanName: str,
    ModelConfigs: List[EdgeDeploymentModelConfigTypeDef],  # (1)
    DeviceFleetName: str,
    EdgeDeploymentSuccess: int,
    EdgeDeploymentPending: int,
    EdgeDeploymentFailed: int,
    Stages: List[DeploymentStageStatusSummaryTypeDef],  # (2)
    NextToken: str,
    CreationTime: datetime,
    LastModifiedTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: EdgeDeploymentModelConfigTypeDef](./type_defs.md#edgedeploymentmodelconfigtypedef) 
2. See [:material-code-braces: DeploymentStageStatusSummaryTypeDef](./type_defs.md#deploymentstagestatussummarytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListExperimentsResponseTypeDef

```python
# ListExperimentsResponseTypeDef definition

class ListExperimentsResponseTypeDef(TypedDict):
    ExperimentSummaries: List[ExperimentSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExperimentSummaryTypeDef](./type_defs.md#experimentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFeatureGroupsResponseTypeDef

```python
# ListFeatureGroupsResponseTypeDef definition

class ListFeatureGroupsResponseTypeDef(TypedDict):
    FeatureGroupSummaries: List[FeatureGroupSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FeatureGroupSummaryTypeDef](./type_defs.md#featuregroupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTrainingJobsResponseTypeDef

```python
# ListTrainingJobsResponseTypeDef definition

class ListTrainingJobsResponseTypeDef(TypedDict):
    TrainingJobSummaries: List[TrainingJobSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrainingJobSummaryTypeDef](./type_defs.md#trainingjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTrialsResponseTypeDef

```python
# ListTrialsResponseTypeDef definition

class ListTrialsResponseTypeDef(TypedDict):
    TrialSummaries: List[TrialSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrialSummaryTypeDef](./type_defs.md#trialsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEndpointWeightsAndCapacitiesInputRequestTypeDef

```python
# UpdateEndpointWeightsAndCapacitiesInputRequestTypeDef definition

class UpdateEndpointWeightsAndCapacitiesInputRequestTypeDef(TypedDict):
    EndpointName: str,
    DesiredWeightsAndCapacities: Sequence[DesiredWeightAndCapacityTypeDef],  # (1)
```

1. See [:material-code-braces: DesiredWeightAndCapacityTypeDef](./type_defs.md#desiredweightandcapacitytypedef) 
## ListDevicesResponseTypeDef

```python
# ListDevicesResponseTypeDef definition

class ListDevicesResponseTypeDef(TypedDict):
    DeviceSummaries: List[DeviceSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeviceSummaryTypeDef](./type_defs.md#devicesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DriftCheckBaselinesTypeDef

```python
# DriftCheckBaselinesTypeDef definition

class DriftCheckBaselinesTypeDef(TypedDict):
    Bias: NotRequired[DriftCheckBiasTypeDef],  # (1)
    Explainability: NotRequired[DriftCheckExplainabilityTypeDef],  # (2)
    ModelQuality: NotRequired[DriftCheckModelQualityTypeDef],  # (3)
    ModelDataQuality: NotRequired[DriftCheckModelDataQualityTypeDef],  # (4)
```

1. See [:material-code-braces: DriftCheckBiasTypeDef](./type_defs.md#driftcheckbiastypedef) 
2. See [:material-code-braces: DriftCheckExplainabilityTypeDef](./type_defs.md#driftcheckexplainabilitytypedef) 
3. See [:material-code-braces: DriftCheckModelQualityTypeDef](./type_defs.md#driftcheckmodelqualitytypedef) 
4. See [:material-code-braces: DriftCheckModelDataQualityTypeDef](./type_defs.md#driftcheckmodeldataqualitytypedef) 
## InferenceRecommendationTypeDef

```python
# InferenceRecommendationTypeDef definition

class InferenceRecommendationTypeDef(TypedDict):
    Metrics: RecommendationMetricsTypeDef,  # (1)
    EndpointConfiguration: EndpointOutputConfigurationTypeDef,  # (2)
    ModelConfiguration: ModelConfigurationTypeDef,  # (3)
    RecommendationId: NotRequired[str],
    InvocationEndTime: NotRequired[datetime],
    InvocationStartTime: NotRequired[datetime],
```

1. See [:material-code-braces: RecommendationMetricsTypeDef](./type_defs.md#recommendationmetricstypedef) 
2. See [:material-code-braces: EndpointOutputConfigurationTypeDef](./type_defs.md#endpointoutputconfigurationtypedef) 
3. See [:material-code-braces: ModelConfigurationTypeDef](./type_defs.md#modelconfigurationtypedef) 
## RecommendationJobInferenceBenchmarkTypeDef

```python
# RecommendationJobInferenceBenchmarkTypeDef definition

class RecommendationJobInferenceBenchmarkTypeDef(TypedDict):
    ModelConfiguration: ModelConfigurationTypeDef,  # (3)
    Metrics: NotRequired[RecommendationMetricsTypeDef],  # (1)
    EndpointConfiguration: NotRequired[EndpointOutputConfigurationTypeDef],  # (2)
    FailureReason: NotRequired[str],
    EndpointMetrics: NotRequired[InferenceMetricsTypeDef],  # (4)
    InvocationEndTime: NotRequired[datetime],
    InvocationStartTime: NotRequired[datetime],
```

1. See [:material-code-braces: RecommendationMetricsTypeDef](./type_defs.md#recommendationmetricstypedef) 
2. See [:material-code-braces: EndpointOutputConfigurationTypeDef](./type_defs.md#endpointoutputconfigurationtypedef) 
3. See [:material-code-braces: ModelConfigurationTypeDef](./type_defs.md#modelconfigurationtypedef) 
4. See [:material-code-braces: InferenceMetricsTypeDef](./type_defs.md#inferencemetricstypedef) 
## SearchExpressionTypeDef

```python
# SearchExpressionTypeDef definition

class SearchExpressionTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    NestedFilters: NotRequired[Sequence[NestedFiltersTypeDef]],  # (2)
    SubExpressions: NotRequired[Sequence[SearchExpressionTypeDef]],  # (3)
    Operator: NotRequired[BooleanOperatorType],  # (4)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: NestedFiltersTypeDef](./type_defs.md#nestedfilterstypedef) 
3. See [:material-code-braces: SearchExpressionTypeDef](./type_defs.md#searchexpressiontypedef) 
4. See [:material-code-brackets: BooleanOperatorType](./literals.md#booleanoperatortype) 
## ListTrainingJobsForHyperParameterTuningJobResponseTypeDef

```python
# ListTrainingJobsForHyperParameterTuningJobResponseTypeDef definition

class ListTrainingJobsForHyperParameterTuningJobResponseTypeDef(TypedDict):
    TrainingJobSummaries: List[HyperParameterTrainingJobSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HyperParameterTrainingJobSummaryTypeDef](./type_defs.md#hyperparametertrainingjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListHyperParameterTuningJobsResponseTypeDef

```python
# ListHyperParameterTuningJobsResponseTypeDef definition

class ListHyperParameterTuningJobsResponseTypeDef(TypedDict):
    HyperParameterTuningJobSummaries: List[HyperParameterTuningJobSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HyperParameterTuningJobSummaryTypeDef](./type_defs.md#hyperparametertuningjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociationSummaryTypeDef

```python
# AssociationSummaryTypeDef definition

class AssociationSummaryTypeDef(TypedDict):
    SourceArn: NotRequired[str],
    DestinationArn: NotRequired[str],
    SourceType: NotRequired[str],
    DestinationType: NotRequired[str],
    AssociationType: NotRequired[AssociationEdgeTypeType],  # (1)
    SourceName: NotRequired[str],
    DestinationName: NotRequired[str],
    CreationTime: NotRequired[datetime],
    CreatedBy: NotRequired[UserContextTypeDef],  # (2)
```

1. See [:material-code-brackets: AssociationEdgeTypeType](./literals.md#associationedgetypetype) 
2. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
## DescribeActionResponseTypeDef

```python
# DescribeActionResponseTypeDef definition

class DescribeActionResponseTypeDef(TypedDict):
    ActionName: str,
    ActionArn: str,
    Source: ActionSourceTypeDef,  # (1)
    ActionType: str,
    Description: str,
    Status: ActionStatusType,  # (2)
    Properties: Dict[str, str],
    CreationTime: datetime,
    CreatedBy: UserContextTypeDef,  # (3)
    LastModifiedTime: datetime,
    LastModifiedBy: UserContextTypeDef,  # (3)
    MetadataProperties: MetadataPropertiesTypeDef,  # (5)
    LineageGroupArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: ActionSourceTypeDef](./type_defs.md#actionsourcetypedef) 
2. See [:material-code-brackets: ActionStatusType](./literals.md#actionstatustype) 
3. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
4. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
5. See [:material-code-braces: MetadataPropertiesTypeDef](./type_defs.md#metadatapropertiestypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeArtifactResponseTypeDef

```python
# DescribeArtifactResponseTypeDef definition

class DescribeArtifactResponseTypeDef(TypedDict):
    ArtifactName: str,
    ArtifactArn: str,
    Source: ArtifactSourceTypeDef,  # (1)
    ArtifactType: str,
    Properties: Dict[str, str],
    CreationTime: datetime,
    CreatedBy: UserContextTypeDef,  # (2)
    LastModifiedTime: datetime,
    LastModifiedBy: UserContextTypeDef,  # (2)
    MetadataProperties: MetadataPropertiesTypeDef,  # (4)
    LineageGroupArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: ArtifactSourceTypeDef](./type_defs.md#artifactsourcetypedef) 
2. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
3. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
4. See [:material-code-braces: MetadataPropertiesTypeDef](./type_defs.md#metadatapropertiestypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeContextResponseTypeDef

```python
# DescribeContextResponseTypeDef definition

class DescribeContextResponseTypeDef(TypedDict):
    ContextName: str,
    ContextArn: str,
    Source: ContextSourceTypeDef,  # (1)
    ContextType: str,
    Description: str,
    Properties: Dict[str, str],
    CreationTime: datetime,
    CreatedBy: UserContextTypeDef,  # (2)
    LastModifiedTime: datetime,
    LastModifiedBy: UserContextTypeDef,  # (2)
    LineageGroupArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ContextSourceTypeDef](./type_defs.md#contextsourcetypedef) 
2. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
3. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeExperimentResponseTypeDef

```python
# DescribeExperimentResponseTypeDef definition

class DescribeExperimentResponseTypeDef(TypedDict):
    ExperimentName: str,
    ExperimentArn: str,
    DisplayName: str,
    Source: ExperimentSourceTypeDef,  # (1)
    Description: str,
    CreationTime: datetime,
    CreatedBy: UserContextTypeDef,  # (2)
    LastModifiedTime: datetime,
    LastModifiedBy: UserContextTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ExperimentSourceTypeDef](./type_defs.md#experimentsourcetypedef) 
2. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
3. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLineageGroupResponseTypeDef

```python
# DescribeLineageGroupResponseTypeDef definition

class DescribeLineageGroupResponseTypeDef(TypedDict):
    LineageGroupName: str,
    LineageGroupArn: str,
    DisplayName: str,
    Description: str,
    CreationTime: datetime,
    CreatedBy: UserContextTypeDef,  # (1)
    LastModifiedTime: datetime,
    LastModifiedBy: UserContextTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
2. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeModelCardResponseTypeDef

```python
# DescribeModelCardResponseTypeDef definition

class DescribeModelCardResponseTypeDef(TypedDict):
    ModelCardArn: str,
    ModelCardName: str,
    ModelCardVersion: int,
    Content: str,
    ModelCardStatus: ModelCardStatusType,  # (1)
    SecurityConfig: ModelCardSecurityConfigTypeDef,  # (2)
    CreationTime: datetime,
    CreatedBy: UserContextTypeDef,  # (3)
    LastModifiedTime: datetime,
    LastModifiedBy: UserContextTypeDef,  # (3)
    ModelCardProcessingStatus: ModelCardProcessingStatusType,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: ModelCardStatusType](./literals.md#modelcardstatustype) 
2. See [:material-code-braces: ModelCardSecurityConfigTypeDef](./type_defs.md#modelcardsecurityconfigtypedef) 
3. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
4. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
5. See [:material-code-brackets: ModelCardProcessingStatusType](./literals.md#modelcardprocessingstatustype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeModelPackageGroupOutputTypeDef

```python
# DescribeModelPackageGroupOutputTypeDef definition

class DescribeModelPackageGroupOutputTypeDef(TypedDict):
    ModelPackageGroupName: str,
    ModelPackageGroupArn: str,
    ModelPackageGroupDescription: str,
    CreationTime: datetime,
    CreatedBy: UserContextTypeDef,  # (1)
    ModelPackageGroupStatus: ModelPackageGroupStatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
2. See [:material-code-brackets: ModelPackageGroupStatusType](./literals.md#modelpackagegroupstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePipelineResponseTypeDef

```python
# DescribePipelineResponseTypeDef definition

class DescribePipelineResponseTypeDef(TypedDict):
    PipelineArn: str,
    PipelineName: str,
    PipelineDisplayName: str,
    PipelineDefinition: str,
    PipelineDescription: str,
    RoleArn: str,
    PipelineStatus: PipelineStatusType,  # (1)
    CreationTime: datetime,
    LastModifiedTime: datetime,
    LastRunTime: datetime,
    CreatedBy: UserContextTypeDef,  # (2)
    LastModifiedBy: UserContextTypeDef,  # (2)
    ParallelismConfiguration: ParallelismConfigurationTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: PipelineStatusType](./literals.md#pipelinestatustype) 
2. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
3. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
4. See [:material-code-braces: ParallelismConfigurationTypeDef](./type_defs.md#parallelismconfigurationtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTrialComponentResponseTypeDef

```python
# DescribeTrialComponentResponseTypeDef definition

class DescribeTrialComponentResponseTypeDef(TypedDict):
    TrialComponentName: str,
    TrialComponentArn: str,
    DisplayName: str,
    Source: TrialComponentSourceTypeDef,  # (1)
    Status: TrialComponentStatusTypeDef,  # (2)
    StartTime: datetime,
    EndTime: datetime,
    CreationTime: datetime,
    CreatedBy: UserContextTypeDef,  # (3)
    LastModifiedTime: datetime,
    LastModifiedBy: UserContextTypeDef,  # (3)
    Parameters: Dict[str, TrialComponentParameterValueTypeDef],  # (5)
    InputArtifacts: Dict[str, TrialComponentArtifactTypeDef],  # (6)
    OutputArtifacts: Dict[str, TrialComponentArtifactTypeDef],  # (6)
    MetadataProperties: MetadataPropertiesTypeDef,  # (8)
    Metrics: List[TrialComponentMetricSummaryTypeDef],  # (9)
    LineageGroupArn: str,
    Sources: List[TrialComponentSourceTypeDef],  # (10)
    ResponseMetadata: ResponseMetadataTypeDef,  # (11)
```

1. See [:material-code-braces: TrialComponentSourceTypeDef](./type_defs.md#trialcomponentsourcetypedef) 
2. See [:material-code-braces: TrialComponentStatusTypeDef](./type_defs.md#trialcomponentstatustypedef) 
3. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
4. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
5. See [:material-code-braces: TrialComponentParameterValueTypeDef](./type_defs.md#trialcomponentparametervaluetypedef) 
6. See [:material-code-braces: TrialComponentArtifactTypeDef](./type_defs.md#trialcomponentartifacttypedef) 
7. See [:material-code-braces: TrialComponentArtifactTypeDef](./type_defs.md#trialcomponentartifacttypedef) 
8. See [:material-code-braces: MetadataPropertiesTypeDef](./type_defs.md#metadatapropertiestypedef) 
9. See [:material-code-braces: TrialComponentMetricSummaryTypeDef](./type_defs.md#trialcomponentmetricsummarytypedef) 
10. See [:material-code-braces: TrialComponentSourceTypeDef](./type_defs.md#trialcomponentsourcetypedef) 
11. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTrialResponseTypeDef

```python
# DescribeTrialResponseTypeDef definition

class DescribeTrialResponseTypeDef(TypedDict):
    TrialName: str,
    TrialArn: str,
    DisplayName: str,
    ExperimentName: str,
    Source: TrialSourceTypeDef,  # (1)
    CreationTime: datetime,
    CreatedBy: UserContextTypeDef,  # (2)
    LastModifiedTime: datetime,
    LastModifiedBy: UserContextTypeDef,  # (2)
    MetadataProperties: MetadataPropertiesTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: TrialSourceTypeDef](./type_defs.md#trialsourcetypedef) 
2. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
3. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
4. See [:material-code-braces: MetadataPropertiesTypeDef](./type_defs.md#metadatapropertiestypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExperimentTypeDef

```python
# ExperimentTypeDef definition

class ExperimentTypeDef(TypedDict):
    ExperimentName: NotRequired[str],
    ExperimentArn: NotRequired[str],
    DisplayName: NotRequired[str],
    Source: NotRequired[ExperimentSourceTypeDef],  # (1)
    Description: NotRequired[str],
    CreationTime: NotRequired[datetime],
    CreatedBy: NotRequired[UserContextTypeDef],  # (2)
    LastModifiedTime: NotRequired[datetime],
    LastModifiedBy: NotRequired[UserContextTypeDef],  # (2)
    Tags: NotRequired[List[TagTypeDef]],  # (4)
```

1. See [:material-code-braces: ExperimentSourceTypeDef](./type_defs.md#experimentsourcetypedef) 
2. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
3. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ModelCardTypeDef

```python
# ModelCardTypeDef definition

class ModelCardTypeDef(TypedDict):
    ModelCardArn: NotRequired[str],
    ModelCardName: NotRequired[str],
    ModelCardVersion: NotRequired[int],
    Content: NotRequired[str],
    ModelCardStatus: NotRequired[ModelCardStatusType],  # (1)
    SecurityConfig: NotRequired[ModelCardSecurityConfigTypeDef],  # (2)
    CreationTime: NotRequired[datetime],
    CreatedBy: NotRequired[UserContextTypeDef],  # (3)
    LastModifiedTime: NotRequired[datetime],
    LastModifiedBy: NotRequired[UserContextTypeDef],  # (3)
    Tags: NotRequired[List[TagTypeDef]],  # (5)
    ModelId: NotRequired[str],
    RiskRating: NotRequired[str],
    ModelPackageGroupName: NotRequired[str],
```

1. See [:material-code-brackets: ModelCardStatusType](./literals.md#modelcardstatustype) 
2. See [:material-code-braces: ModelCardSecurityConfigTypeDef](./type_defs.md#modelcardsecurityconfigtypedef) 
3. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
4. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ModelDashboardModelCardTypeDef

```python
# ModelDashboardModelCardTypeDef definition

class ModelDashboardModelCardTypeDef(TypedDict):
    ModelCardArn: NotRequired[str],
    ModelCardName: NotRequired[str],
    ModelCardVersion: NotRequired[int],
    ModelCardStatus: NotRequired[ModelCardStatusType],  # (1)
    SecurityConfig: NotRequired[ModelCardSecurityConfigTypeDef],  # (2)
    CreationTime: NotRequired[datetime],
    CreatedBy: NotRequired[UserContextTypeDef],  # (3)
    LastModifiedTime: NotRequired[datetime],
    LastModifiedBy: NotRequired[UserContextTypeDef],  # (3)
    Tags: NotRequired[List[TagTypeDef]],  # (5)
    ModelId: NotRequired[str],
    RiskRating: NotRequired[str],
```

1. See [:material-code-brackets: ModelCardStatusType](./literals.md#modelcardstatustype) 
2. See [:material-code-braces: ModelCardSecurityConfigTypeDef](./type_defs.md#modelcardsecurityconfigtypedef) 
3. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
4. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ModelPackageGroupTypeDef

```python
# ModelPackageGroupTypeDef definition

class ModelPackageGroupTypeDef(TypedDict):
    ModelPackageGroupName: NotRequired[str],
    ModelPackageGroupArn: NotRequired[str],
    ModelPackageGroupDescription: NotRequired[str],
    CreationTime: NotRequired[datetime],
    CreatedBy: NotRequired[UserContextTypeDef],  # (1)
    ModelPackageGroupStatus: NotRequired[ModelPackageGroupStatusType],  # (2)
    Tags: NotRequired[List[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
2. See [:material-code-brackets: ModelPackageGroupStatusType](./literals.md#modelpackagegroupstatustype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## PipelineTypeDef

```python
# PipelineTypeDef definition

class PipelineTypeDef(TypedDict):
    PipelineArn: NotRequired[str],
    PipelineName: NotRequired[str],
    PipelineDisplayName: NotRequired[str],
    PipelineDescription: NotRequired[str],
    RoleArn: NotRequired[str],
    PipelineStatus: NotRequired[PipelineStatusType],  # (1)
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
    LastRunTime: NotRequired[datetime],
    CreatedBy: NotRequired[UserContextTypeDef],  # (2)
    LastModifiedBy: NotRequired[UserContextTypeDef],  # (2)
    ParallelismConfiguration: NotRequired[ParallelismConfigurationTypeDef],  # (4)
    Tags: NotRequired[List[TagTypeDef]],  # (5)
```

1. See [:material-code-brackets: PipelineStatusType](./literals.md#pipelinestatustype) 
2. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
3. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
4. See [:material-code-braces: ParallelismConfigurationTypeDef](./type_defs.md#parallelismconfigurationtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TrialComponentSimpleSummaryTypeDef

```python
# TrialComponentSimpleSummaryTypeDef definition

class TrialComponentSimpleSummaryTypeDef(TypedDict):
    TrialComponentName: NotRequired[str],
    TrialComponentArn: NotRequired[str],
    TrialComponentSource: NotRequired[TrialComponentSourceTypeDef],  # (1)
    CreationTime: NotRequired[datetime],
    CreatedBy: NotRequired[UserContextTypeDef],  # (2)
```

1. See [:material-code-braces: TrialComponentSourceTypeDef](./type_defs.md#trialcomponentsourcetypedef) 
2. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
## TrialComponentSummaryTypeDef

```python
# TrialComponentSummaryTypeDef definition

class TrialComponentSummaryTypeDef(TypedDict):
    TrialComponentName: NotRequired[str],
    TrialComponentArn: NotRequired[str],
    DisplayName: NotRequired[str],
    TrialComponentSource: NotRequired[TrialComponentSourceTypeDef],  # (1)
    Status: NotRequired[TrialComponentStatusTypeDef],  # (2)
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    CreationTime: NotRequired[datetime],
    CreatedBy: NotRequired[UserContextTypeDef],  # (3)
    LastModifiedTime: NotRequired[datetime],
    LastModifiedBy: NotRequired[UserContextTypeDef],  # (3)
```

1. See [:material-code-braces: TrialComponentSourceTypeDef](./type_defs.md#trialcomponentsourcetypedef) 
2. See [:material-code-braces: TrialComponentStatusTypeDef](./type_defs.md#trialcomponentstatustypedef) 
3. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
4. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
## HyperParameterSpecificationTypeDef

```python
# HyperParameterSpecificationTypeDef definition

class HyperParameterSpecificationTypeDef(TypedDict):
    Name: str,
    Type: ParameterTypeType,  # (1)
    Description: NotRequired[str],
    Range: NotRequired[ParameterRangeTypeDef],  # (2)
    IsTunable: NotRequired[bool],
    IsRequired: NotRequired[bool],
    DefaultValue: NotRequired[str],
```

1. See [:material-code-brackets: ParameterTypeType](./literals.md#parametertypetype) 
2. See [:material-code-braces: ParameterRangeTypeDef](./type_defs.md#parameterrangetypedef) 
## HyperParameterTuningJobConfigTypeDef

```python
# HyperParameterTuningJobConfigTypeDef definition

class HyperParameterTuningJobConfigTypeDef(TypedDict):
    Strategy: HyperParameterTuningJobStrategyTypeType,  # (1)
    ResourceLimits: ResourceLimitsTypeDef,  # (4)
    StrategyConfig: NotRequired[HyperParameterTuningJobStrategyConfigTypeDef],  # (2)
    HyperParameterTuningJobObjective: NotRequired[HyperParameterTuningJobObjectiveTypeDef],  # (3)
    ParameterRanges: NotRequired[ParameterRangesTypeDef],  # (5)
    TrainingJobEarlyStoppingType: NotRequired[TrainingJobEarlyStoppingTypeType],  # (6)
    TuningJobCompletionCriteria: NotRequired[TuningJobCompletionCriteriaTypeDef],  # (7)
    RandomSeed: NotRequired[int],
```

1. See [:material-code-brackets: HyperParameterTuningJobStrategyTypeType](./literals.md#hyperparametertuningjobstrategytypetype) 
2. See [:material-code-braces: HyperParameterTuningJobStrategyConfigTypeDef](./type_defs.md#hyperparametertuningjobstrategyconfigtypedef) 
3. See [:material-code-braces: HyperParameterTuningJobObjectiveTypeDef](./type_defs.md#hyperparametertuningjobobjectivetypedef) 
4. See [:material-code-braces: ResourceLimitsTypeDef](./type_defs.md#resourcelimitstypedef) 
5. See [:material-code-braces: ParameterRangesTypeDef](./type_defs.md#parameterrangestypedef) 
6. See [:material-code-brackets: TrainingJobEarlyStoppingTypeType](./literals.md#trainingjobearlystoppingtypetype) 
7. See [:material-code-braces: TuningJobCompletionCriteriaTypeDef](./type_defs.md#tuningjobcompletioncriteriatypedef) 
## AppImageConfigDetailsTypeDef

```python
# AppImageConfigDetailsTypeDef definition

class AppImageConfigDetailsTypeDef(TypedDict):
    AppImageConfigArn: NotRequired[str],
    AppImageConfigName: NotRequired[str],
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
    KernelGatewayImageConfig: NotRequired[KernelGatewayImageConfigTypeDef],  # (1)
```

1. See [:material-code-braces: KernelGatewayImageConfigTypeDef](./type_defs.md#kernelgatewayimageconfigtypedef) 
## CreateAppImageConfigRequestRequestTypeDef

```python
# CreateAppImageConfigRequestRequestTypeDef definition

class CreateAppImageConfigRequestRequestTypeDef(TypedDict):
    AppImageConfigName: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    KernelGatewayImageConfig: NotRequired[KernelGatewayImageConfigTypeDef],  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: KernelGatewayImageConfigTypeDef](./type_defs.md#kernelgatewayimageconfigtypedef) 
## DescribeAppImageConfigResponseTypeDef

```python
# DescribeAppImageConfigResponseTypeDef definition

class DescribeAppImageConfigResponseTypeDef(TypedDict):
    AppImageConfigArn: str,
    AppImageConfigName: str,
    CreationTime: datetime,
    LastModifiedTime: datetime,
    KernelGatewayImageConfig: KernelGatewayImageConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KernelGatewayImageConfigTypeDef](./type_defs.md#kernelgatewayimageconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAppImageConfigRequestRequestTypeDef

```python
# UpdateAppImageConfigRequestRequestTypeDef definition

class UpdateAppImageConfigRequestRequestTypeDef(TypedDict):
    AppImageConfigName: str,
    KernelGatewayImageConfig: NotRequired[KernelGatewayImageConfigTypeDef],  # (1)
```

1. See [:material-code-braces: KernelGatewayImageConfigTypeDef](./type_defs.md#kernelgatewayimageconfigtypedef) 
## ListLabelingJobsForWorkteamResponseTypeDef

```python
# ListLabelingJobsForWorkteamResponseTypeDef definition

class ListLabelingJobsForWorkteamResponseTypeDef(TypedDict):
    LabelingJobSummaryList: List[LabelingJobForWorkteamSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LabelingJobForWorkteamSummaryTypeDef](./type_defs.md#labelingjobforworkteamsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LabelingJobInputConfigTypeDef

```python
# LabelingJobInputConfigTypeDef definition

class LabelingJobInputConfigTypeDef(TypedDict):
    DataSource: LabelingJobDataSourceTypeDef,  # (1)
    DataAttributes: NotRequired[LabelingJobDataAttributesTypeDef],  # (2)
```

1. See [:material-code-braces: LabelingJobDataSourceTypeDef](./type_defs.md#labelingjobdatasourcetypedef) 
2. See [:material-code-braces: LabelingJobDataAttributesTypeDef](./type_defs.md#labelingjobdataattributestypedef) 
## CreateWorkteamRequestRequestTypeDef

```python
# CreateWorkteamRequestRequestTypeDef definition

class CreateWorkteamRequestRequestTypeDef(TypedDict):
    WorkteamName: str,
    MemberDefinitions: Sequence[MemberDefinitionTypeDef],  # (1)
    Description: str,
    WorkforceName: NotRequired[str],
    NotificationConfiguration: NotRequired[NotificationConfigurationTypeDef],  # (2)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: MemberDefinitionTypeDef](./type_defs.md#memberdefinitiontypedef) 
2. See [:material-code-braces: NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateWorkteamRequestRequestTypeDef

```python
# UpdateWorkteamRequestRequestTypeDef definition

class UpdateWorkteamRequestRequestTypeDef(TypedDict):
    WorkteamName: str,
    MemberDefinitions: NotRequired[Sequence[MemberDefinitionTypeDef]],  # (1)
    Description: NotRequired[str],
    NotificationConfiguration: NotRequired[NotificationConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: MemberDefinitionTypeDef](./type_defs.md#memberdefinitiontypedef) 
2. See [:material-code-braces: NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef) 
## WorkteamTypeDef

```python
# WorkteamTypeDef definition

class WorkteamTypeDef(TypedDict):
    WorkteamName: str,
    MemberDefinitions: List[MemberDefinitionTypeDef],  # (1)
    WorkteamArn: str,
    Description: str,
    WorkforceArn: NotRequired[str],
    ProductListingIds: NotRequired[List[str]],
    SubDomain: NotRequired[str],
    CreateDate: NotRequired[datetime],
    LastUpdatedDate: NotRequired[datetime],
    NotificationConfiguration: NotRequired[NotificationConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: MemberDefinitionTypeDef](./type_defs.md#memberdefinitiontypedef) 
2. See [:material-code-braces: NotificationConfigurationTypeDef](./type_defs.md#notificationconfigurationtypedef) 
## TargetTrackingScalingPolicyConfigurationTypeDef

```python
# TargetTrackingScalingPolicyConfigurationTypeDef definition

class TargetTrackingScalingPolicyConfigurationTypeDef(TypedDict):
    MetricSpecification: NotRequired[MetricSpecificationTypeDef],  # (1)
    TargetValue: NotRequired[float],
```

1. See [:material-code-braces: MetricSpecificationTypeDef](./type_defs.md#metricspecificationtypedef) 
## MonitoringAlertSummaryTypeDef

```python
# MonitoringAlertSummaryTypeDef definition

class MonitoringAlertSummaryTypeDef(TypedDict):
    MonitoringAlertName: str,
    CreationTime: datetime,
    LastModifiedTime: datetime,
    AlertStatus: MonitoringAlertStatusType,  # (1)
    DatapointsToAlert: int,
    EvaluationPeriod: int,
    Actions: MonitoringAlertActionsTypeDef,  # (2)
```

1. See [:material-code-brackets: MonitoringAlertStatusType](./literals.md#monitoringalertstatustype) 
2. See [:material-code-braces: MonitoringAlertActionsTypeDef](./type_defs.md#monitoringalertactionstypedef) 
## ContainerDefinitionTypeDef

```python
# ContainerDefinitionTypeDef definition

class ContainerDefinitionTypeDef(TypedDict):
    ContainerHostname: NotRequired[str],
    Image: NotRequired[str],
    ImageConfig: NotRequired[ImageConfigTypeDef],  # (1)
    Mode: NotRequired[ContainerModeType],  # (2)
    ModelDataUrl: NotRequired[str],
    Environment: NotRequired[Mapping[str, str]],
    ModelPackageName: NotRequired[str],
    InferenceSpecificationName: NotRequired[str],
    MultiModelConfig: NotRequired[MultiModelConfigTypeDef],  # (3)
    ModelDataSource: NotRequired[ModelDataSourceTypeDef],  # (4)
```

1. See [:material-code-braces: ImageConfigTypeDef](./type_defs.md#imageconfigtypedef) 
2. See [:material-code-brackets: ContainerModeType](./literals.md#containermodetype) 
3. See [:material-code-braces: MultiModelConfigTypeDef](./type_defs.md#multimodelconfigtypedef) 
4. See [:material-code-braces: ModelDataSourceTypeDef](./type_defs.md#modeldatasourcetypedef) 
## ModelVariantConfigSummaryTypeDef

```python
# ModelVariantConfigSummaryTypeDef definition

class ModelVariantConfigSummaryTypeDef(TypedDict):
    ModelName: str,
    VariantName: str,
    InfrastructureConfig: ModelInfrastructureConfigTypeDef,  # (1)
    Status: ModelVariantStatusType,  # (2)
```

1. See [:material-code-braces: ModelInfrastructureConfigTypeDef](./type_defs.md#modelinfrastructureconfigtypedef) 
2. See [:material-code-brackets: ModelVariantStatusType](./literals.md#modelvariantstatustype) 
## ModelVariantConfigTypeDef

```python
# ModelVariantConfigTypeDef definition

class ModelVariantConfigTypeDef(TypedDict):
    ModelName: str,
    VariantName: str,
    InfrastructureConfig: ModelInfrastructureConfigTypeDef,  # (1)
```

1. See [:material-code-braces: ModelInfrastructureConfigTypeDef](./type_defs.md#modelinfrastructureconfigtypedef) 
## AdditionalInferenceSpecificationDefinitionTypeDef

```python
# AdditionalInferenceSpecificationDefinitionTypeDef definition

class AdditionalInferenceSpecificationDefinitionTypeDef(TypedDict):
    Name: str,
    Containers: Sequence[ModelPackageContainerDefinitionTypeDef],  # (1)
    Description: NotRequired[str],
    SupportedTransformInstanceTypes: NotRequired[Sequence[TransformInstanceTypeType]],  # (2)
    SupportedRealtimeInferenceInstanceTypes: NotRequired[Sequence[ProductionVariantInstanceTypeType]],  # (3)
    SupportedContentTypes: NotRequired[Sequence[str]],
    SupportedResponseMIMETypes: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: ModelPackageContainerDefinitionTypeDef](./type_defs.md#modelpackagecontainerdefinitiontypedef) 
2. See [:material-code-brackets: TransformInstanceTypeType](./literals.md#transforminstancetypetype) 
3. See [:material-code-brackets: ProductionVariantInstanceTypeType](./literals.md#productionvariantinstancetypetype) 
## InferenceSpecificationTypeDef

```python
# InferenceSpecificationTypeDef definition

class InferenceSpecificationTypeDef(TypedDict):
    Containers: List[ModelPackageContainerDefinitionTypeDef],  # (1)
    SupportedContentTypes: List[str],
    SupportedResponseMIMETypes: List[str],
    SupportedTransformInstanceTypes: NotRequired[List[TransformInstanceTypeType]],  # (2)
    SupportedRealtimeInferenceInstanceTypes: NotRequired[List[ProductionVariantInstanceTypeType]],  # (3)
```

1. See [:material-code-braces: ModelPackageContainerDefinitionTypeDef](./type_defs.md#modelpackagecontainerdefinitiontypedef) 
2. See [:material-code-brackets: TransformInstanceTypeType](./literals.md#transforminstancetypetype) 
3. See [:material-code-brackets: ProductionVariantInstanceTypeType](./literals.md#productionvariantinstancetypetype) 
## ListModelMetadataRequestListModelMetadataPaginateTypeDef

```python
# ListModelMetadataRequestListModelMetadataPaginateTypeDef definition

class ListModelMetadataRequestListModelMetadataPaginateTypeDef(TypedDict):
    SearchExpression: NotRequired[ModelMetadataSearchExpressionTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ModelMetadataSearchExpressionTypeDef](./type_defs.md#modelmetadatasearchexpressiontypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListModelMetadataRequestRequestTypeDef

```python
# ListModelMetadataRequestRequestTypeDef definition

class ListModelMetadataRequestRequestTypeDef(TypedDict):
    SearchExpression: NotRequired[ModelMetadataSearchExpressionTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: ModelMetadataSearchExpressionTypeDef](./type_defs.md#modelmetadatasearchexpressiontypedef) 
## BatchTransformInputTypeDef

```python
# BatchTransformInputTypeDef definition

class BatchTransformInputTypeDef(TypedDict):
    DataCapturedDestinationS3Uri: str,
    DatasetFormat: MonitoringDatasetFormatTypeDef,  # (1)
    LocalPath: str,
    S3InputMode: NotRequired[ProcessingS3InputModeType],  # (2)
    S3DataDistributionType: NotRequired[ProcessingS3DataDistributionTypeType],  # (3)
    FeaturesAttribute: NotRequired[str],
    InferenceAttribute: NotRequired[str],
    ProbabilityAttribute: NotRequired[str],
    ProbabilityThresholdAttribute: NotRequired[float],
    StartTimeOffset: NotRequired[str],
    EndTimeOffset: NotRequired[str],
```

1. See [:material-code-braces: MonitoringDatasetFormatTypeDef](./type_defs.md#monitoringdatasetformattypedef) 
2. See [:material-code-brackets: ProcessingS3InputModeType](./literals.md#processings3inputmodetype) 
3. See [:material-code-brackets: ProcessingS3DataDistributionTypeType](./literals.md#processings3datadistributiontypetype) 
## MonitoringOutputConfigTypeDef

```python
# MonitoringOutputConfigTypeDef definition

class MonitoringOutputConfigTypeDef(TypedDict):
    MonitoringOutputs: Sequence[MonitoringOutputTypeDef],  # (1)
    KmsKeyId: NotRequired[str],
```

1. See [:material-code-braces: MonitoringOutputTypeDef](./type_defs.md#monitoringoutputtypedef) 
## CreateFeatureGroupRequestRequestTypeDef

```python
# CreateFeatureGroupRequestRequestTypeDef definition

class CreateFeatureGroupRequestRequestTypeDef(TypedDict):
    FeatureGroupName: str,
    RecordIdentifierFeatureName: str,
    EventTimeFeatureName: str,
    FeatureDefinitions: Sequence[FeatureDefinitionTypeDef],  # (1)
    OnlineStoreConfig: NotRequired[OnlineStoreConfigTypeDef],  # (2)
    OfflineStoreConfig: NotRequired[OfflineStoreConfigTypeDef],  # (3)
    RoleArn: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
```

1. See [:material-code-braces: FeatureDefinitionTypeDef](./type_defs.md#featuredefinitiontypedef) 
2. See [:material-code-braces: OnlineStoreConfigTypeDef](./type_defs.md#onlinestoreconfigtypedef) 
3. See [:material-code-braces: OfflineStoreConfigTypeDef](./type_defs.md#offlinestoreconfigtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeFeatureGroupResponseTypeDef

```python
# DescribeFeatureGroupResponseTypeDef definition

class DescribeFeatureGroupResponseTypeDef(TypedDict):
    FeatureGroupArn: str,
    FeatureGroupName: str,
    RecordIdentifierFeatureName: str,
    EventTimeFeatureName: str,
    FeatureDefinitions: List[FeatureDefinitionTypeDef],  # (1)
    CreationTime: datetime,
    LastModifiedTime: datetime,
    OnlineStoreConfig: OnlineStoreConfigTypeDef,  # (2)
    OfflineStoreConfig: OfflineStoreConfigTypeDef,  # (3)
    RoleArn: str,
    FeatureGroupStatus: FeatureGroupStatusType,  # (4)
    OfflineStoreStatus: OfflineStoreStatusTypeDef,  # (5)
    LastUpdateStatus: LastUpdateStatusTypeDef,  # (6)
    FailureReason: str,
    Description: str,
    NextToken: str,
    OnlineStoreTotalSizeBytes: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-braces: FeatureDefinitionTypeDef](./type_defs.md#featuredefinitiontypedef) 
2. See [:material-code-braces: OnlineStoreConfigTypeDef](./type_defs.md#onlinestoreconfigtypedef) 
3. See [:material-code-braces: OfflineStoreConfigTypeDef](./type_defs.md#offlinestoreconfigtypedef) 
4. See [:material-code-brackets: FeatureGroupStatusType](./literals.md#featuregroupstatustype) 
5. See [:material-code-braces: OfflineStoreStatusTypeDef](./type_defs.md#offlinestorestatustypedef) 
6. See [:material-code-braces: LastUpdateStatusTypeDef](./type_defs.md#lastupdatestatustypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FeatureGroupTypeDef

```python
# FeatureGroupTypeDef definition

class FeatureGroupTypeDef(TypedDict):
    FeatureGroupArn: NotRequired[str],
    FeatureGroupName: NotRequired[str],
    RecordIdentifierFeatureName: NotRequired[str],
    EventTimeFeatureName: NotRequired[str],
    FeatureDefinitions: NotRequired[List[FeatureDefinitionTypeDef]],  # (1)
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
    OnlineStoreConfig: NotRequired[OnlineStoreConfigTypeDef],  # (2)
    OfflineStoreConfig: NotRequired[OfflineStoreConfigTypeDef],  # (3)
    RoleArn: NotRequired[str],
    FeatureGroupStatus: NotRequired[FeatureGroupStatusType],  # (4)
    OfflineStoreStatus: NotRequired[OfflineStoreStatusTypeDef],  # (5)
    LastUpdateStatus: NotRequired[LastUpdateStatusTypeDef],  # (6)
    FailureReason: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (7)
```

1. See [:material-code-braces: FeatureDefinitionTypeDef](./type_defs.md#featuredefinitiontypedef) 
2. See [:material-code-braces: OnlineStoreConfigTypeDef](./type_defs.md#onlinestoreconfigtypedef) 
3. See [:material-code-braces: OfflineStoreConfigTypeDef](./type_defs.md#offlinestoreconfigtypedef) 
4. See [:material-code-brackets: FeatureGroupStatusType](./literals.md#featuregroupstatustype) 
5. See [:material-code-braces: OfflineStoreStatusTypeDef](./type_defs.md#offlinestorestatustypedef) 
6. See [:material-code-braces: LastUpdateStatusTypeDef](./type_defs.md#lastupdatestatustypedef) 
7. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateFeatureGroupRequestRequestTypeDef

```python
# UpdateFeatureGroupRequestRequestTypeDef definition

class UpdateFeatureGroupRequestRequestTypeDef(TypedDict):
    FeatureGroupName: str,
    FeatureAdditions: NotRequired[Sequence[FeatureDefinitionTypeDef]],  # (1)
    OnlineStoreConfig: NotRequired[OnlineStoreConfigUpdateTypeDef],  # (2)
```

1. See [:material-code-braces: FeatureDefinitionTypeDef](./type_defs.md#featuredefinitiontypedef) 
2. See [:material-code-braces: OnlineStoreConfigUpdateTypeDef](./type_defs.md#onlinestoreconfigupdatetypedef) 
## CreateCompilationJobRequestRequestTypeDef

```python
# CreateCompilationJobRequestRequestTypeDef definition

class CreateCompilationJobRequestRequestTypeDef(TypedDict):
    CompilationJobName: str,
    RoleArn: str,
    OutputConfig: OutputConfigTypeDef,  # (1)
    StoppingCondition: StoppingConditionTypeDef,  # (2)
    ModelPackageVersionArn: NotRequired[str],
    InputConfig: NotRequired[InputConfigTypeDef],  # (3)
    VpcConfig: NotRequired[NeoVpcConfigTypeDef],  # (4)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (5)
```

1. See [:material-code-braces: OutputConfigTypeDef](./type_defs.md#outputconfigtypedef) 
2. See [:material-code-braces: StoppingConditionTypeDef](./type_defs.md#stoppingconditiontypedef) 
3. See [:material-code-braces: InputConfigTypeDef](./type_defs.md#inputconfigtypedef) 
4. See [:material-code-braces: NeoVpcConfigTypeDef](./type_defs.md#neovpcconfigtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeCompilationJobResponseTypeDef

```python
# DescribeCompilationJobResponseTypeDef definition

class DescribeCompilationJobResponseTypeDef(TypedDict):
    CompilationJobName: str,
    CompilationJobArn: str,
    CompilationJobStatus: CompilationJobStatusType,  # (1)
    CompilationStartTime: datetime,
    CompilationEndTime: datetime,
    StoppingCondition: StoppingConditionTypeDef,  # (2)
    InferenceImage: str,
    ModelPackageVersionArn: str,
    CreationTime: datetime,
    LastModifiedTime: datetime,
    FailureReason: str,
    ModelArtifacts: ModelArtifactsTypeDef,  # (3)
    ModelDigests: ModelDigestsTypeDef,  # (4)
    RoleArn: str,
    InputConfig: InputConfigTypeDef,  # (5)
    OutputConfig: OutputConfigTypeDef,  # (6)
    VpcConfig: NeoVpcConfigTypeDef,  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-brackets: CompilationJobStatusType](./literals.md#compilationjobstatustype) 
2. See [:material-code-braces: StoppingConditionTypeDef](./type_defs.md#stoppingconditiontypedef) 
3. See [:material-code-braces: ModelArtifactsTypeDef](./type_defs.md#modelartifactstypedef) 
4. See [:material-code-braces: ModelDigestsTypeDef](./type_defs.md#modeldigeststypedef) 
5. See [:material-code-braces: InputConfigTypeDef](./type_defs.md#inputconfigtypedef) 
6. See [:material-code-braces: OutputConfigTypeDef](./type_defs.md#outputconfigtypedef) 
7. See [:material-code-braces: NeoVpcConfigTypeDef](./type_defs.md#neovpcconfigtypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PendingDeploymentSummaryTypeDef

```python
# PendingDeploymentSummaryTypeDef definition

class PendingDeploymentSummaryTypeDef(TypedDict):
    EndpointConfigName: str,
    ProductionVariants: NotRequired[List[PendingProductionVariantSummaryTypeDef]],  # (1)
    StartTime: NotRequired[datetime],
    ShadowProductionVariants: NotRequired[List[PendingProductionVariantSummaryTypeDef]],  # (1)
```

1. See [:material-code-braces: PendingProductionVariantSummaryTypeDef](./type_defs.md#pendingproductionvariantsummarytypedef) 
2. See [:material-code-braces: PendingProductionVariantSummaryTypeDef](./type_defs.md#pendingproductionvariantsummarytypedef) 
## ProcessingOutputConfigTypeDef

```python
# ProcessingOutputConfigTypeDef definition

class ProcessingOutputConfigTypeDef(TypedDict):
    Outputs: Sequence[ProcessingOutputTypeDef],  # (1)
    KmsKeyId: NotRequired[str],
```

1. See [:material-code-braces: ProcessingOutputTypeDef](./type_defs.md#processingoutputtypedef) 
## GetSearchSuggestionsRequestRequestTypeDef

```python
# GetSearchSuggestionsRequestRequestTypeDef definition

class GetSearchSuggestionsRequestRequestTypeDef(TypedDict):
    Resource: ResourceTypeType,  # (1)
    SuggestionQuery: NotRequired[SuggestionQueryTypeDef],  # (2)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: SuggestionQueryTypeDef](./type_defs.md#suggestionquerytypedef) 
## CreateProjectInputRequestTypeDef

```python
# CreateProjectInputRequestTypeDef definition

class CreateProjectInputRequestTypeDef(TypedDict):
    ProjectName: str,
    ServiceCatalogProvisioningDetails: ServiceCatalogProvisioningDetailsTypeDef,  # (1)
    ProjectDescription: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: ServiceCatalogProvisioningDetailsTypeDef](./type_defs.md#servicecatalogprovisioningdetailstypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeProjectOutputTypeDef

```python
# DescribeProjectOutputTypeDef definition

class DescribeProjectOutputTypeDef(TypedDict):
    ProjectArn: str,
    ProjectName: str,
    ProjectId: str,
    ProjectDescription: str,
    ServiceCatalogProvisioningDetails: ServiceCatalogProvisioningDetailsTypeDef,  # (1)
    ServiceCatalogProvisionedProductDetails: ServiceCatalogProvisionedProductDetailsTypeDef,  # (2)
    ProjectStatus: ProjectStatusType,  # (3)
    CreatedBy: UserContextTypeDef,  # (4)
    CreationTime: datetime,
    LastModifiedTime: datetime,
    LastModifiedBy: UserContextTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: ServiceCatalogProvisioningDetailsTypeDef](./type_defs.md#servicecatalogprovisioningdetailstypedef) 
2. See [:material-code-braces: ServiceCatalogProvisionedProductDetailsTypeDef](./type_defs.md#servicecatalogprovisionedproductdetailstypedef) 
3. See [:material-code-brackets: ProjectStatusType](./literals.md#projectstatustype) 
4. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
5. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProjectTypeDef

```python
# ProjectTypeDef definition

class ProjectTypeDef(TypedDict):
    ProjectArn: NotRequired[str],
    ProjectName: NotRequired[str],
    ProjectId: NotRequired[str],
    ProjectDescription: NotRequired[str],
    ServiceCatalogProvisioningDetails: NotRequired[ServiceCatalogProvisioningDetailsTypeDef],  # (1)
    ServiceCatalogProvisionedProductDetails: NotRequired[ServiceCatalogProvisionedProductDetailsTypeDef],  # (2)
    ProjectStatus: NotRequired[ProjectStatusType],  # (3)
    CreatedBy: NotRequired[UserContextTypeDef],  # (4)
    CreationTime: NotRequired[datetime],
    Tags: NotRequired[List[TagTypeDef]],  # (5)
    LastModifiedTime: NotRequired[datetime],
    LastModifiedBy: NotRequired[UserContextTypeDef],  # (4)
```

1. See [:material-code-braces: ServiceCatalogProvisioningDetailsTypeDef](./type_defs.md#servicecatalogprovisioningdetailstypedef) 
2. See [:material-code-braces: ServiceCatalogProvisionedProductDetailsTypeDef](./type_defs.md#servicecatalogprovisionedproductdetailstypedef) 
3. See [:material-code-brackets: ProjectStatusType](./literals.md#projectstatustype) 
4. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
## UpdateProjectInputRequestTypeDef

```python
# UpdateProjectInputRequestTypeDef definition

class UpdateProjectInputRequestTypeDef(TypedDict):
    ProjectName: str,
    ProjectDescription: NotRequired[str],
    ServiceCatalogProvisioningUpdateDetails: NotRequired[ServiceCatalogProvisioningUpdateDetailsTypeDef],  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: ServiceCatalogProvisioningUpdateDetailsTypeDef](./type_defs.md#servicecatalogprovisioningupdatedetailstypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## HumanLoopConfigTypeDef

```python
# HumanLoopConfigTypeDef definition

class HumanLoopConfigTypeDef(TypedDict):
    WorkteamArn: str,
    HumanTaskUiArn: str,
    TaskTitle: str,
    TaskDescription: str,
    TaskCount: int,
    TaskAvailabilityLifetimeInSeconds: NotRequired[int],
    TaskTimeLimitInSeconds: NotRequired[int],
    TaskKeywords: NotRequired[Sequence[str]],
    PublicWorkforceTaskPrice: NotRequired[PublicWorkforceTaskPriceTypeDef],  # (1)
```

1. See [:material-code-braces: PublicWorkforceTaskPriceTypeDef](./type_defs.md#publicworkforcetaskpricetypedef) 
## HumanTaskConfigTypeDef

```python
# HumanTaskConfigTypeDef definition

class HumanTaskConfigTypeDef(TypedDict):
    WorkteamArn: str,
    UiConfig: UiConfigTypeDef,  # (1)
    PreHumanTaskLambdaArn: str,
    TaskTitle: str,
    TaskDescription: str,
    NumberOfHumanWorkersPerDataObject: int,
    TaskTimeLimitInSeconds: int,
    AnnotationConsolidationConfig: AnnotationConsolidationConfigTypeDef,  # (2)
    TaskKeywords: NotRequired[Sequence[str]],
    TaskAvailabilityLifetimeInSeconds: NotRequired[int],
    MaxConcurrentTaskCount: NotRequired[int],
    PublicWorkforceTaskPrice: NotRequired[PublicWorkforceTaskPriceTypeDef],  # (3)
```

1. See [:material-code-braces: UiConfigTypeDef](./type_defs.md#uiconfigtypedef) 
2. See [:material-code-braces: AnnotationConsolidationConfigTypeDef](./type_defs.md#annotationconsolidationconfigtypedef) 
3. See [:material-code-braces: PublicWorkforceTaskPriceTypeDef](./type_defs.md#publicworkforcetaskpricetypedef) 
## DescribePipelineExecutionResponseTypeDef

```python
# DescribePipelineExecutionResponseTypeDef definition

class DescribePipelineExecutionResponseTypeDef(TypedDict):
    PipelineArn: str,
    PipelineExecutionArn: str,
    PipelineExecutionDisplayName: str,
    PipelineExecutionStatus: PipelineExecutionStatusType,  # (1)
    PipelineExecutionDescription: str,
    PipelineExperimentConfig: PipelineExperimentConfigTypeDef,  # (2)
    FailureReason: str,
    CreationTime: datetime,
    LastModifiedTime: datetime,
    CreatedBy: UserContextTypeDef,  # (3)
    LastModifiedBy: UserContextTypeDef,  # (3)
    ParallelismConfiguration: ParallelismConfigurationTypeDef,  # (5)
    SelectiveExecutionConfig: SelectiveExecutionConfigTypeDef,  # (6)
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-brackets: PipelineExecutionStatusType](./literals.md#pipelineexecutionstatustype) 
2. See [:material-code-braces: PipelineExperimentConfigTypeDef](./type_defs.md#pipelineexperimentconfigtypedef) 
3. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
4. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
5. See [:material-code-braces: ParallelismConfigurationTypeDef](./type_defs.md#parallelismconfigurationtypedef) 
6. See [:material-code-braces: SelectiveExecutionConfigTypeDef](./type_defs.md#selectiveexecutionconfigtypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PipelineExecutionTypeDef

```python
# PipelineExecutionTypeDef definition

class PipelineExecutionTypeDef(TypedDict):
    PipelineArn: NotRequired[str],
    PipelineExecutionArn: NotRequired[str],
    PipelineExecutionDisplayName: NotRequired[str],
    PipelineExecutionStatus: NotRequired[PipelineExecutionStatusType],  # (1)
    PipelineExecutionDescription: NotRequired[str],
    PipelineExperimentConfig: NotRequired[PipelineExperimentConfigTypeDef],  # (2)
    FailureReason: NotRequired[str],
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
    CreatedBy: NotRequired[UserContextTypeDef],  # (3)
    LastModifiedBy: NotRequired[UserContextTypeDef],  # (3)
    ParallelismConfiguration: NotRequired[ParallelismConfigurationTypeDef],  # (5)
    PipelineParameters: NotRequired[List[ParameterTypeDef]],  # (6)
    SelectiveExecutionConfig: NotRequired[SelectiveExecutionConfigTypeDef],  # (7)
```

1. See [:material-code-brackets: PipelineExecutionStatusType](./literals.md#pipelineexecutionstatustype) 
2. See [:material-code-braces: PipelineExperimentConfigTypeDef](./type_defs.md#pipelineexperimentconfigtypedef) 
3. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
4. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
5. See [:material-code-braces: ParallelismConfigurationTypeDef](./type_defs.md#parallelismconfigurationtypedef) 
6. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
7. See [:material-code-braces: SelectiveExecutionConfigTypeDef](./type_defs.md#selectiveexecutionconfigtypedef) 
## StartPipelineExecutionRequestRequestTypeDef

```python
# StartPipelineExecutionRequestRequestTypeDef definition

class StartPipelineExecutionRequestRequestTypeDef(TypedDict):
    PipelineName: str,
    ClientRequestToken: str,
    PipelineExecutionDisplayName: NotRequired[str],
    PipelineParameters: NotRequired[Sequence[ParameterTypeDef]],  # (1)
    PipelineExecutionDescription: NotRequired[str],
    ParallelismConfiguration: NotRequired[ParallelismConfigurationTypeDef],  # (2)
    SelectiveExecutionConfig: NotRequired[SelectiveExecutionConfigTypeDef],  # (3)
```

1. See [:material-code-braces: ParameterTypeDef](./type_defs.md#parametertypedef) 
2. See [:material-code-braces: ParallelismConfigurationTypeDef](./type_defs.md#parallelismconfigurationtypedef) 
3. See [:material-code-braces: SelectiveExecutionConfigTypeDef](./type_defs.md#selectiveexecutionconfigtypedef) 
## AlgorithmSpecificationTypeDef

```python
# AlgorithmSpecificationTypeDef definition

class AlgorithmSpecificationTypeDef(TypedDict):
    TrainingInputMode: TrainingInputModeType,  # (1)
    TrainingImage: NotRequired[str],
    AlgorithmName: NotRequired[str],
    MetricDefinitions: NotRequired[Sequence[MetricDefinitionTypeDef]],  # (2)
    EnableSageMakerMetricsTimeSeries: NotRequired[bool],
    ContainerEntrypoint: NotRequired[Sequence[str]],
    ContainerArguments: NotRequired[Sequence[str]],
    TrainingImageConfig: NotRequired[TrainingImageConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: TrainingInputModeType](./literals.md#traininginputmodetype) 
2. See [:material-code-braces: MetricDefinitionTypeDef](./type_defs.md#metricdefinitiontypedef) 
3. See [:material-code-braces: TrainingImageConfigTypeDef](./type_defs.md#trainingimageconfigtypedef) 
## TransformInputTypeDef

```python
# TransformInputTypeDef definition

class TransformInputTypeDef(TypedDict):
    DataSource: TransformDataSourceTypeDef,  # (1)
    ContentType: NotRequired[str],
    CompressionType: NotRequired[CompressionTypeType],  # (2)
    SplitType: NotRequired[SplitTypeType],  # (3)
```

1. See [:material-code-braces: TransformDataSourceTypeDef](./type_defs.md#transformdatasourcetypedef) 
2. See [:material-code-brackets: CompressionTypeType](./literals.md#compressiontypetype) 
3. See [:material-code-brackets: SplitTypeType](./literals.md#splittypetype) 
## DescribeWorkforceResponseTypeDef

```python
# DescribeWorkforceResponseTypeDef definition

class DescribeWorkforceResponseTypeDef(TypedDict):
    Workforce: WorkforceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkforceTypeDef](./type_defs.md#workforcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWorkforcesResponseTypeDef

```python
# ListWorkforcesResponseTypeDef definition

class ListWorkforcesResponseTypeDef(TypedDict):
    Workforces: List[WorkforceTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkforceTypeDef](./type_defs.md#workforcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWorkforceResponseTypeDef

```python
# UpdateWorkforceResponseTypeDef definition

class UpdateWorkforceResponseTypeDef(TypedDict):
    Workforce: WorkforceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkforceTypeDef](./type_defs.md#workforcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListArtifactsResponseTypeDef

```python
# ListArtifactsResponseTypeDef definition

class ListArtifactsResponseTypeDef(TypedDict):
    ArtifactSummaries: List[ArtifactSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ArtifactSummaryTypeDef](./type_defs.md#artifactsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AutoMLProblemTypeConfigTypeDef

```python
# AutoMLProblemTypeConfigTypeDef definition

class AutoMLProblemTypeConfigTypeDef(TypedDict):
    ImageClassificationJobConfig: NotRequired[ImageClassificationJobConfigTypeDef],  # (1)
    TextClassificationJobConfig: NotRequired[TextClassificationJobConfigTypeDef],  # (2)
    TabularJobConfig: NotRequired[TabularJobConfigTypeDef],  # (3)
    TimeSeriesForecastingJobConfig: NotRequired[TimeSeriesForecastingJobConfigTypeDef],  # (4)
```

1. See [:material-code-braces: ImageClassificationJobConfigTypeDef](./type_defs.md#imageclassificationjobconfigtypedef) 
2. See [:material-code-braces: TextClassificationJobConfigTypeDef](./type_defs.md#textclassificationjobconfigtypedef) 
3. See [:material-code-braces: TabularJobConfigTypeDef](./type_defs.md#tabularjobconfigtypedef) 
4. See [:material-code-braces: TimeSeriesForecastingJobConfigTypeDef](./type_defs.md#timeseriesforecastingjobconfigtypedef) 
## CreateAutoMLJobRequestRequestTypeDef

```python
# CreateAutoMLJobRequestRequestTypeDef definition

class CreateAutoMLJobRequestRequestTypeDef(TypedDict):
    AutoMLJobName: str,
    InputDataConfig: Sequence[AutoMLChannelTypeDef],  # (1)
    OutputDataConfig: AutoMLOutputDataConfigTypeDef,  # (2)
    RoleArn: str,
    ProblemType: NotRequired[ProblemTypeType],  # (3)
    AutoMLJobObjective: NotRequired[AutoMLJobObjectiveTypeDef],  # (4)
    AutoMLJobConfig: NotRequired[AutoMLJobConfigTypeDef],  # (5)
    GenerateCandidateDefinitionsOnly: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (6)
    ModelDeployConfig: NotRequired[ModelDeployConfigTypeDef],  # (7)
```

1. See [:material-code-braces: AutoMLChannelTypeDef](./type_defs.md#automlchanneltypedef) 
2. See [:material-code-braces: AutoMLOutputDataConfigTypeDef](./type_defs.md#automloutputdataconfigtypedef) 
3. See [:material-code-brackets: ProblemTypeType](./literals.md#problemtypetype) 
4. See [:material-code-braces: AutoMLJobObjectiveTypeDef](./type_defs.md#automljobobjectivetypedef) 
5. See [:material-code-braces: AutoMLJobConfigTypeDef](./type_defs.md#automljobconfigtypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
7. See [:material-code-braces: ModelDeployConfigTypeDef](./type_defs.md#modeldeployconfigtypedef) 
## PipelineExecutionStepTypeDef

```python
# PipelineExecutionStepTypeDef definition

class PipelineExecutionStepTypeDef(TypedDict):
    StepName: NotRequired[str],
    StepDisplayName: NotRequired[str],
    StepDescription: NotRequired[str],
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    StepStatus: NotRequired[StepStatusType],  # (1)
    CacheHitResult: NotRequired[CacheHitResultTypeDef],  # (2)
    AttemptCount: NotRequired[int],
    FailureReason: NotRequired[str],
    Metadata: NotRequired[PipelineExecutionStepMetadataTypeDef],  # (3)
    SelectiveExecutionResult: NotRequired[SelectiveExecutionResultTypeDef],  # (4)
```

1. See [:material-code-brackets: StepStatusType](./literals.md#stepstatustype) 
2. See [:material-code-braces: CacheHitResultTypeDef](./type_defs.md#cachehitresulttypedef) 
3. See [:material-code-braces: PipelineExecutionStepMetadataTypeDef](./type_defs.md#pipelineexecutionstepmetadatatypedef) 
4. See [:material-code-braces: SelectiveExecutionResultTypeDef](./type_defs.md#selectiveexecutionresulttypedef) 
## DescribeAutoMLJobResponseTypeDef

```python
# DescribeAutoMLJobResponseTypeDef definition

class DescribeAutoMLJobResponseTypeDef(TypedDict):
    AutoMLJobName: str,
    AutoMLJobArn: str,
    InputDataConfig: List[AutoMLChannelTypeDef],  # (1)
    OutputDataConfig: AutoMLOutputDataConfigTypeDef,  # (2)
    RoleArn: str,
    AutoMLJobObjective: AutoMLJobObjectiveTypeDef,  # (3)
    ProblemType: ProblemTypeType,  # (4)
    AutoMLJobConfig: AutoMLJobConfigTypeDef,  # (5)
    CreationTime: datetime,
    EndTime: datetime,
    LastModifiedTime: datetime,
    FailureReason: str,
    PartialFailureReasons: List[AutoMLPartialFailureReasonTypeDef],  # (6)
    BestCandidate: AutoMLCandidateTypeDef,  # (7)
    AutoMLJobStatus: AutoMLJobStatusType,  # (8)
    AutoMLJobSecondaryStatus: AutoMLJobSecondaryStatusType,  # (9)
    GenerateCandidateDefinitionsOnly: bool,
    AutoMLJobArtifacts: AutoMLJobArtifactsTypeDef,  # (10)
    ResolvedAttributes: ResolvedAttributesTypeDef,  # (11)
    ModelDeployConfig: ModelDeployConfigTypeDef,  # (12)
    ModelDeployResult: ModelDeployResultTypeDef,  # (13)
    ResponseMetadata: ResponseMetadataTypeDef,  # (14)
```

1. See [:material-code-braces: AutoMLChannelTypeDef](./type_defs.md#automlchanneltypedef) 
2. See [:material-code-braces: AutoMLOutputDataConfigTypeDef](./type_defs.md#automloutputdataconfigtypedef) 
3. See [:material-code-braces: AutoMLJobObjectiveTypeDef](./type_defs.md#automljobobjectivetypedef) 
4. See [:material-code-brackets: ProblemTypeType](./literals.md#problemtypetype) 
5. See [:material-code-braces: AutoMLJobConfigTypeDef](./type_defs.md#automljobconfigtypedef) 
6. See [:material-code-braces: AutoMLPartialFailureReasonTypeDef](./type_defs.md#automlpartialfailurereasontypedef) 
7. See [:material-code-braces: AutoMLCandidateTypeDef](./type_defs.md#automlcandidatetypedef) 
8. See [:material-code-brackets: AutoMLJobStatusType](./literals.md#automljobstatustype) 
9. See [:material-code-brackets: AutoMLJobSecondaryStatusType](./literals.md#automljobsecondarystatustype) 
10. See [:material-code-braces: AutoMLJobArtifactsTypeDef](./type_defs.md#automljobartifactstypedef) 
11. See [:material-code-braces: ResolvedAttributesTypeDef](./type_defs.md#resolvedattributestypedef) 
12. See [:material-code-braces: ModelDeployConfigTypeDef](./type_defs.md#modeldeployconfigtypedef) 
13. See [:material-code-braces: ModelDeployResultTypeDef](./type_defs.md#modeldeployresulttypedef) 
14. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCandidatesForAutoMLJobResponseTypeDef

```python
# ListCandidatesForAutoMLJobResponseTypeDef definition

class ListCandidatesForAutoMLJobResponseTypeDef(TypedDict):
    Candidates: List[AutoMLCandidateTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AutoMLCandidateTypeDef](./type_defs.md#automlcandidatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeploymentConfigTypeDef

```python
# DeploymentConfigTypeDef definition

class DeploymentConfigTypeDef(TypedDict):
    BlueGreenUpdatePolicy: NotRequired[BlueGreenUpdatePolicyTypeDef],  # (1)
    AutoRollbackConfiguration: NotRequired[AutoRollbackConfigTypeDef],  # (2)
    RollingUpdatePolicy: NotRequired[RollingUpdatePolicyTypeDef],  # (3)
```

1. See [:material-code-braces: BlueGreenUpdatePolicyTypeDef](./type_defs.md#bluegreenupdatepolicytypedef) 
2. See [:material-code-braces: AutoRollbackConfigTypeDef](./type_defs.md#autorollbackconfigtypedef) 
3. See [:material-code-braces: RollingUpdatePolicyTypeDef](./type_defs.md#rollingupdatepolicytypedef) 
## RecommendationJobInputConfigTypeDef

```python
# RecommendationJobInputConfigTypeDef definition

class RecommendationJobInputConfigTypeDef(TypedDict):
    ModelPackageVersionArn: NotRequired[str],
    JobDurationInSeconds: NotRequired[int],
    TrafficPattern: NotRequired[TrafficPatternTypeDef],  # (1)
    ResourceLimit: NotRequired[RecommendationJobResourceLimitTypeDef],  # (2)
    EndpointConfigurations: NotRequired[Sequence[EndpointInputConfigurationTypeDef]],  # (3)
    VolumeKmsKeyId: NotRequired[str],
    ContainerConfig: NotRequired[RecommendationJobContainerConfigTypeDef],  # (4)
    Endpoints: NotRequired[Sequence[EndpointInfoTypeDef]],  # (5)
    VpcConfig: NotRequired[RecommendationJobVpcConfigTypeDef],  # (6)
    ModelName: NotRequired[str],
```

1. See [:material-code-braces: TrafficPatternTypeDef](./type_defs.md#trafficpatterntypedef) 
2. See [:material-code-braces: RecommendationJobResourceLimitTypeDef](./type_defs.md#recommendationjobresourcelimittypedef) 
3. See [:material-code-braces: EndpointInputConfigurationTypeDef](./type_defs.md#endpointinputconfigurationtypedef) 
4. See [:material-code-braces: RecommendationJobContainerConfigTypeDef](./type_defs.md#recommendationjobcontainerconfigtypedef) 
5. See [:material-code-braces: EndpointInfoTypeDef](./type_defs.md#endpointinfotypedef) 
6. See [:material-code-braces: RecommendationJobVpcConfigTypeDef](./type_defs.md#recommendationjobvpcconfigtypedef) 
## ExplainerConfigTypeDef

```python
# ExplainerConfigTypeDef definition

class ExplainerConfigTypeDef(TypedDict):
    ClarifyExplainerConfig: NotRequired[ClarifyExplainerConfigTypeDef],  # (1)
```

1. See [:material-code-braces: ClarifyExplainerConfigTypeDef](./type_defs.md#clarifyexplainerconfigtypedef) 
## ListInferenceExperimentsResponseTypeDef

```python
# ListInferenceExperimentsResponseTypeDef definition

class ListInferenceExperimentsResponseTypeDef(TypedDict):
    InferenceExperiments: List[InferenceExperimentSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InferenceExperimentSummaryTypeDef](./type_defs.md#inferenceexperimentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSpaceRequestRequestTypeDef

```python
# CreateSpaceRequestRequestTypeDef definition

class CreateSpaceRequestRequestTypeDef(TypedDict):
    DomainId: str,
    SpaceName: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    SpaceSettings: NotRequired[SpaceSettingsTypeDef],  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: SpaceSettingsTypeDef](./type_defs.md#spacesettingstypedef) 
## DescribeSpaceResponseTypeDef

```python
# DescribeSpaceResponseTypeDef definition

class DescribeSpaceResponseTypeDef(TypedDict):
    DomainId: str,
    SpaceArn: str,
    SpaceName: str,
    HomeEfsFileSystemUid: str,
    Status: SpaceStatusType,  # (1)
    LastModifiedTime: datetime,
    CreationTime: datetime,
    FailureReason: str,
    SpaceSettings: SpaceSettingsTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: SpaceStatusType](./literals.md#spacestatustype) 
2. See [:material-code-braces: SpaceSettingsTypeDef](./type_defs.md#spacesettingstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSpaceRequestRequestTypeDef

```python
# UpdateSpaceRequestRequestTypeDef definition

class UpdateSpaceRequestRequestTypeDef(TypedDict):
    DomainId: str,
    SpaceName: str,
    SpaceSettings: NotRequired[SpaceSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: SpaceSettingsTypeDef](./type_defs.md#spacesettingstypedef) 
## CreateDomainRequestRequestTypeDef

```python
# CreateDomainRequestRequestTypeDef definition

class CreateDomainRequestRequestTypeDef(TypedDict):
    DomainName: str,
    AuthMode: AuthModeType,  # (1)
    DefaultUserSettings: UserSettingsTypeDef,  # (2)
    SubnetIds: Sequence[str],
    VpcId: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
    AppNetworkAccessType: NotRequired[AppNetworkAccessTypeType],  # (4)
    HomeEfsFileSystemKmsKeyId: NotRequired[str],
    KmsKeyId: NotRequired[str],
    AppSecurityGroupManagement: NotRequired[AppSecurityGroupManagementType],  # (5)
    DomainSettings: NotRequired[DomainSettingsTypeDef],  # (6)
    DefaultSpaceSettings: NotRequired[DefaultSpaceSettingsTypeDef],  # (7)
```

1. See [:material-code-brackets: AuthModeType](./literals.md#authmodetype) 
2. See [:material-code-braces: UserSettingsTypeDef](./type_defs.md#usersettingstypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-brackets: AppNetworkAccessTypeType](./literals.md#appnetworkaccesstypetype) 
5. See [:material-code-brackets: AppSecurityGroupManagementType](./literals.md#appsecuritygroupmanagementtype) 
6. See [:material-code-braces: DomainSettingsTypeDef](./type_defs.md#domainsettingstypedef) 
7. See [:material-code-braces: DefaultSpaceSettingsTypeDef](./type_defs.md#defaultspacesettingstypedef) 
## CreateUserProfileRequestRequestTypeDef

```python
# CreateUserProfileRequestRequestTypeDef definition

class CreateUserProfileRequestRequestTypeDef(TypedDict):
    DomainId: str,
    UserProfileName: str,
    SingleSignOnUserIdentifier: NotRequired[str],
    SingleSignOnUserValue: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    UserSettings: NotRequired[UserSettingsTypeDef],  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: UserSettingsTypeDef](./type_defs.md#usersettingstypedef) 
## DescribeDomainResponseTypeDef

```python
# DescribeDomainResponseTypeDef definition

class DescribeDomainResponseTypeDef(TypedDict):
    DomainArn: str,
    DomainId: str,
    DomainName: str,
    HomeEfsFileSystemId: str,
    SingleSignOnManagedApplicationInstanceId: str,
    Status: DomainStatusType,  # (1)
    CreationTime: datetime,
    LastModifiedTime: datetime,
    FailureReason: str,
    AuthMode: AuthModeType,  # (2)
    DefaultUserSettings: UserSettingsTypeDef,  # (3)
    AppNetworkAccessType: AppNetworkAccessTypeType,  # (4)
    HomeEfsFileSystemKmsKeyId: str,
    SubnetIds: List[str],
    Url: str,
    VpcId: str,
    KmsKeyId: str,
    DomainSettings: DomainSettingsTypeDef,  # (5)
    AppSecurityGroupManagement: AppSecurityGroupManagementType,  # (6)
    SecurityGroupIdForDomainBoundary: str,
    DefaultSpaceSettings: DefaultSpaceSettingsTypeDef,  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-brackets: DomainStatusType](./literals.md#domainstatustype) 
2. See [:material-code-brackets: AuthModeType](./literals.md#authmodetype) 
3. See [:material-code-braces: UserSettingsTypeDef](./type_defs.md#usersettingstypedef) 
4. See [:material-code-brackets: AppNetworkAccessTypeType](./literals.md#appnetworkaccesstypetype) 
5. See [:material-code-braces: DomainSettingsTypeDef](./type_defs.md#domainsettingstypedef) 
6. See [:material-code-brackets: AppSecurityGroupManagementType](./literals.md#appsecuritygroupmanagementtype) 
7. See [:material-code-braces: DefaultSpaceSettingsTypeDef](./type_defs.md#defaultspacesettingstypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeUserProfileResponseTypeDef

```python
# DescribeUserProfileResponseTypeDef definition

class DescribeUserProfileResponseTypeDef(TypedDict):
    DomainId: str,
    UserProfileArn: str,
    UserProfileName: str,
    HomeEfsFileSystemUid: str,
    Status: UserProfileStatusType,  # (1)
    LastModifiedTime: datetime,
    CreationTime: datetime,
    FailureReason: str,
    SingleSignOnUserIdentifier: str,
    SingleSignOnUserValue: str,
    UserSettings: UserSettingsTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: UserProfileStatusType](./literals.md#userprofilestatustype) 
2. See [:material-code-braces: UserSettingsTypeDef](./type_defs.md#usersettingstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDomainRequestRequestTypeDef

```python
# UpdateDomainRequestRequestTypeDef definition

class UpdateDomainRequestRequestTypeDef(TypedDict):
    DomainId: str,
    DefaultUserSettings: NotRequired[UserSettingsTypeDef],  # (1)
    DomainSettingsForUpdate: NotRequired[DomainSettingsForUpdateTypeDef],  # (2)
    DefaultSpaceSettings: NotRequired[DefaultSpaceSettingsTypeDef],  # (3)
    AppSecurityGroupManagement: NotRequired[AppSecurityGroupManagementType],  # (4)
```

1. See [:material-code-braces: UserSettingsTypeDef](./type_defs.md#usersettingstypedef) 
2. See [:material-code-braces: DomainSettingsForUpdateTypeDef](./type_defs.md#domainsettingsforupdatetypedef) 
3. See [:material-code-braces: DefaultSpaceSettingsTypeDef](./type_defs.md#defaultspacesettingstypedef) 
4. See [:material-code-brackets: AppSecurityGroupManagementType](./literals.md#appsecuritygroupmanagementtype) 
## UpdateUserProfileRequestRequestTypeDef

```python
# UpdateUserProfileRequestRequestTypeDef definition

class UpdateUserProfileRequestRequestTypeDef(TypedDict):
    DomainId: str,
    UserProfileName: str,
    UserSettings: NotRequired[UserSettingsTypeDef],  # (1)
```

1. See [:material-code-braces: UserSettingsTypeDef](./type_defs.md#usersettingstypedef) 
## HyperParameterTrainingJobDefinitionTypeDef

```python
# HyperParameterTrainingJobDefinitionTypeDef definition

class HyperParameterTrainingJobDefinitionTypeDef(TypedDict):
    AlgorithmSpecification: HyperParameterAlgorithmSpecificationTypeDef,  # (3)
    RoleArn: str,
    OutputDataConfig: OutputDataConfigTypeDef,  # (6)
    StoppingCondition: StoppingConditionTypeDef,  # (8)
    DefinitionName: NotRequired[str],
    TuningObjective: NotRequired[HyperParameterTuningJobObjectiveTypeDef],  # (1)
    HyperParameterRanges: NotRequired[ParameterRangesTypeDef],  # (2)
    StaticHyperParameters: NotRequired[Mapping[str, str]],
    InputDataConfig: NotRequired[Sequence[ChannelTypeDef]],  # (4)
    VpcConfig: NotRequired[VpcConfigTypeDef],  # (5)
    ResourceConfig: NotRequired[ResourceConfigTypeDef],  # (7)
    EnableNetworkIsolation: NotRequired[bool],
    EnableInterContainerTrafficEncryption: NotRequired[bool],
    EnableManagedSpotTraining: NotRequired[bool],
    CheckpointConfig: NotRequired[CheckpointConfigTypeDef],  # (9)
    RetryStrategy: NotRequired[RetryStrategyTypeDef],  # (10)
    HyperParameterTuningResourceConfig: NotRequired[HyperParameterTuningResourceConfigTypeDef],  # (11)
    Environment: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: HyperParameterTuningJobObjectiveTypeDef](./type_defs.md#hyperparametertuningjobobjectivetypedef) 
2. See [:material-code-braces: ParameterRangesTypeDef](./type_defs.md#parameterrangestypedef) 
3. See [:material-code-braces: HyperParameterAlgorithmSpecificationTypeDef](./type_defs.md#hyperparameteralgorithmspecificationtypedef) 
4. See [:material-code-braces: ChannelTypeDef](./type_defs.md#channeltypedef) 
5. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
6. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
7. See [:material-code-braces: ResourceConfigTypeDef](./type_defs.md#resourceconfigtypedef) 
8. See [:material-code-braces: StoppingConditionTypeDef](./type_defs.md#stoppingconditiontypedef) 
9. See [:material-code-braces: CheckpointConfigTypeDef](./type_defs.md#checkpointconfigtypedef) 
10. See [:material-code-braces: RetryStrategyTypeDef](./type_defs.md#retrystrategytypedef) 
11. See [:material-code-braces: HyperParameterTuningResourceConfigTypeDef](./type_defs.md#hyperparametertuningresourceconfigtypedef) 
## TrainingJobDefinitionTypeDef

```python
# TrainingJobDefinitionTypeDef definition

class TrainingJobDefinitionTypeDef(TypedDict):
    TrainingInputMode: TrainingInputModeType,  # (1)
    InputDataConfig: Sequence[ChannelTypeDef],  # (2)
    OutputDataConfig: OutputDataConfigTypeDef,  # (3)
    ResourceConfig: ResourceConfigTypeDef,  # (4)
    StoppingCondition: StoppingConditionTypeDef,  # (5)
    HyperParameters: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: TrainingInputModeType](./literals.md#traininginputmodetype) 
2. See [:material-code-braces: ChannelTypeDef](./type_defs.md#channeltypedef) 
3. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
4. See [:material-code-braces: ResourceConfigTypeDef](./type_defs.md#resourceconfigtypedef) 
5. See [:material-code-braces: StoppingConditionTypeDef](./type_defs.md#stoppingconditiontypedef) 
## InferenceRecommendationsJobStepTypeDef

```python
# InferenceRecommendationsJobStepTypeDef definition

class InferenceRecommendationsJobStepTypeDef(TypedDict):
    StepType: RecommendationStepTypeType,  # (1)
    JobName: str,
    Status: RecommendationJobStatusType,  # (2)
    InferenceBenchmark: NotRequired[RecommendationJobInferenceBenchmarkTypeDef],  # (3)
```

1. See [:material-code-brackets: RecommendationStepTypeType](./literals.md#recommendationsteptypetype) 
2. See [:material-code-brackets: RecommendationJobStatusType](./literals.md#recommendationjobstatustype) 
3. See [:material-code-braces: RecommendationJobInferenceBenchmarkTypeDef](./type_defs.md#recommendationjobinferencebenchmarktypedef) 
## ListAssociationsResponseTypeDef

```python
# ListAssociationsResponseTypeDef definition

class ListAssociationsResponseTypeDef(TypedDict):
    AssociationSummaries: List[AssociationSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssociationSummaryTypeDef](./type_defs.md#associationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TrialTypeDef

```python
# TrialTypeDef definition

class TrialTypeDef(TypedDict):
    TrialName: NotRequired[str],
    TrialArn: NotRequired[str],
    DisplayName: NotRequired[str],
    ExperimentName: NotRequired[str],
    Source: NotRequired[TrialSourceTypeDef],  # (1)
    CreationTime: NotRequired[datetime],
    CreatedBy: NotRequired[UserContextTypeDef],  # (2)
    LastModifiedTime: NotRequired[datetime],
    LastModifiedBy: NotRequired[UserContextTypeDef],  # (2)
    MetadataProperties: NotRequired[MetadataPropertiesTypeDef],  # (4)
    Tags: NotRequired[List[TagTypeDef]],  # (5)
    TrialComponentSummaries: NotRequired[List[TrialComponentSimpleSummaryTypeDef]],  # (6)
```

1. See [:material-code-braces: TrialSourceTypeDef](./type_defs.md#trialsourcetypedef) 
2. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
3. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
4. See [:material-code-braces: MetadataPropertiesTypeDef](./type_defs.md#metadatapropertiestypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: TrialComponentSimpleSummaryTypeDef](./type_defs.md#trialcomponentsimplesummarytypedef) 
## ListTrialComponentsResponseTypeDef

```python
# ListTrialComponentsResponseTypeDef definition

class ListTrialComponentsResponseTypeDef(TypedDict):
    TrialComponentSummaries: List[TrialComponentSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrialComponentSummaryTypeDef](./type_defs.md#trialcomponentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TrainingSpecificationTypeDef

```python
# TrainingSpecificationTypeDef definition

class TrainingSpecificationTypeDef(TypedDict):
    TrainingImage: str,
    SupportedTrainingInstanceTypes: Sequence[TrainingInstanceTypeType],  # (2)
    TrainingChannels: Sequence[ChannelSpecificationTypeDef],  # (4)
    TrainingImageDigest: NotRequired[str],
    SupportedHyperParameters: NotRequired[Sequence[HyperParameterSpecificationTypeDef]],  # (1)
    SupportsDistributedTraining: NotRequired[bool],
    MetricDefinitions: NotRequired[Sequence[MetricDefinitionTypeDef]],  # (3)
    SupportedTuningJobObjectiveMetrics: NotRequired[Sequence[HyperParameterTuningJobObjectiveTypeDef]],  # (5)
```

1. See [:material-code-braces: HyperParameterSpecificationTypeDef](./type_defs.md#hyperparameterspecificationtypedef) 
2. See [:material-code-brackets: TrainingInstanceTypeType](./literals.md#traininginstancetypetype) 
3. See [:material-code-braces: MetricDefinitionTypeDef](./type_defs.md#metricdefinitiontypedef) 
4. See [:material-code-braces: ChannelSpecificationTypeDef](./type_defs.md#channelspecificationtypedef) 
5. See [:material-code-braces: HyperParameterTuningJobObjectiveTypeDef](./type_defs.md#hyperparametertuningjobobjectivetypedef) 
## ListAppImageConfigsResponseTypeDef

```python
# ListAppImageConfigsResponseTypeDef definition

class ListAppImageConfigsResponseTypeDef(TypedDict):
    NextToken: str,
    AppImageConfigs: List[AppImageConfigDetailsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppImageConfigDetailsTypeDef](./type_defs.md#appimageconfigdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LabelingJobSummaryTypeDef

```python
# LabelingJobSummaryTypeDef definition

class LabelingJobSummaryTypeDef(TypedDict):
    LabelingJobName: str,
    LabelingJobArn: str,
    CreationTime: datetime,
    LastModifiedTime: datetime,
    LabelingJobStatus: LabelingJobStatusType,  # (1)
    LabelCounters: LabelCountersTypeDef,  # (2)
    WorkteamArn: str,
    PreHumanTaskLambdaArn: str,
    AnnotationConsolidationLambdaArn: NotRequired[str],
    FailureReason: NotRequired[str],
    LabelingJobOutput: NotRequired[LabelingJobOutputTypeDef],  # (3)
    InputConfig: NotRequired[LabelingJobInputConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: LabelingJobStatusType](./literals.md#labelingjobstatustype) 
2. See [:material-code-braces: LabelCountersTypeDef](./type_defs.md#labelcounterstypedef) 
3. See [:material-code-braces: LabelingJobOutputTypeDef](./type_defs.md#labelingjoboutputtypedef) 
4. See [:material-code-braces: LabelingJobInputConfigTypeDef](./type_defs.md#labelingjobinputconfigtypedef) 
## DescribeWorkteamResponseTypeDef

```python
# DescribeWorkteamResponseTypeDef definition

class DescribeWorkteamResponseTypeDef(TypedDict):
    Workteam: WorkteamTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkteamTypeDef](./type_defs.md#workteamtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWorkteamsResponseTypeDef

```python
# ListWorkteamsResponseTypeDef definition

class ListWorkteamsResponseTypeDef(TypedDict):
    Workteams: List[WorkteamTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkteamTypeDef](./type_defs.md#workteamtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWorkteamResponseTypeDef

```python
# UpdateWorkteamResponseTypeDef definition

class UpdateWorkteamResponseTypeDef(TypedDict):
    Workteam: WorkteamTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkteamTypeDef](./type_defs.md#workteamtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ScalingPolicyTypeDef

```python
# ScalingPolicyTypeDef definition

class ScalingPolicyTypeDef(TypedDict):
    TargetTracking: NotRequired[TargetTrackingScalingPolicyConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: TargetTrackingScalingPolicyConfigurationTypeDef](./type_defs.md#targettrackingscalingpolicyconfigurationtypedef) 
## ListMonitoringAlertsResponseTypeDef

```python
# ListMonitoringAlertsResponseTypeDef definition

class ListMonitoringAlertsResponseTypeDef(TypedDict):
    MonitoringAlertSummaries: List[MonitoringAlertSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MonitoringAlertSummaryTypeDef](./type_defs.md#monitoringalertsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateModelInputRequestTypeDef

```python
# CreateModelInputRequestTypeDef definition

class CreateModelInputRequestTypeDef(TypedDict):
    ModelName: str,
    ExecutionRoleArn: str,
    PrimaryContainer: NotRequired[ContainerDefinitionTypeDef],  # (1)
    Containers: NotRequired[Sequence[ContainerDefinitionTypeDef]],  # (2)
    InferenceExecutionConfig: NotRequired[InferenceExecutionConfigTypeDef],  # (3)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
    VpcConfig: NotRequired[VpcConfigTypeDef],  # (5)
    EnableNetworkIsolation: NotRequired[bool],
```

1. See [:material-code-braces: ContainerDefinitionTypeDef](./type_defs.md#containerdefinitiontypedef) 
2. See [:material-code-braces: ContainerDefinitionTypeDef](./type_defs.md#containerdefinitiontypedef) 
3. See [:material-code-braces: InferenceExecutionConfigTypeDef](./type_defs.md#inferenceexecutionconfigtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
## DescribeModelOutputTypeDef

```python
# DescribeModelOutputTypeDef definition

class DescribeModelOutputTypeDef(TypedDict):
    ModelName: str,
    PrimaryContainer: ContainerDefinitionTypeDef,  # (1)
    Containers: List[ContainerDefinitionTypeDef],  # (2)
    InferenceExecutionConfig: InferenceExecutionConfigTypeDef,  # (3)
    ExecutionRoleArn: str,
    VpcConfig: VpcConfigTypeDef,  # (4)
    CreationTime: datetime,
    ModelArn: str,
    EnableNetworkIsolation: bool,
    DeploymentRecommendation: DeploymentRecommendationTypeDef,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: ContainerDefinitionTypeDef](./type_defs.md#containerdefinitiontypedef) 
2. See [:material-code-braces: ContainerDefinitionTypeDef](./type_defs.md#containerdefinitiontypedef) 
3. See [:material-code-braces: InferenceExecutionConfigTypeDef](./type_defs.md#inferenceexecutionconfigtypedef) 
4. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
5. See [:material-code-braces: DeploymentRecommendationTypeDef](./type_defs.md#deploymentrecommendationtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModelTypeDef

```python
# ModelTypeDef definition

class ModelTypeDef(TypedDict):
    ModelName: NotRequired[str],
    PrimaryContainer: NotRequired[ContainerDefinitionTypeDef],  # (1)
    Containers: NotRequired[List[ContainerDefinitionTypeDef]],  # (2)
    InferenceExecutionConfig: NotRequired[InferenceExecutionConfigTypeDef],  # (3)
    ExecutionRoleArn: NotRequired[str],
    VpcConfig: NotRequired[VpcConfigTypeDef],  # (4)
    CreationTime: NotRequired[datetime],
    ModelArn: NotRequired[str],
    EnableNetworkIsolation: NotRequired[bool],
    Tags: NotRequired[List[TagTypeDef]],  # (5)
    DeploymentRecommendation: NotRequired[DeploymentRecommendationTypeDef],  # (6)
```

1. See [:material-code-braces: ContainerDefinitionTypeDef](./type_defs.md#containerdefinitiontypedef) 
2. See [:material-code-braces: ContainerDefinitionTypeDef](./type_defs.md#containerdefinitiontypedef) 
3. See [:material-code-braces: InferenceExecutionConfigTypeDef](./type_defs.md#inferenceexecutionconfigtypedef) 
4. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: DeploymentRecommendationTypeDef](./type_defs.md#deploymentrecommendationtypedef) 
## DescribeInferenceExperimentResponseTypeDef

```python
# DescribeInferenceExperimentResponseTypeDef definition

class DescribeInferenceExperimentResponseTypeDef(TypedDict):
    Arn: str,
    Name: str,
    Type: InferenceExperimentTypeType,  # (1)
    Schedule: InferenceExperimentScheduleTypeDef,  # (2)
    Status: InferenceExperimentStatusType,  # (3)
    StatusReason: str,
    Description: str,
    CreationTime: datetime,
    CompletionTime: datetime,
    LastModifiedTime: datetime,
    RoleArn: str,
    EndpointMetadata: EndpointMetadataTypeDef,  # (4)
    ModelVariants: List[ModelVariantConfigSummaryTypeDef],  # (5)
    DataStorageConfig: InferenceExperimentDataStorageConfigTypeDef,  # (6)
    ShadowModeConfig: ShadowModeConfigTypeDef,  # (7)
    KmsKey: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-brackets: InferenceExperimentTypeType](./literals.md#inferenceexperimenttypetype) 
2. See [:material-code-braces: InferenceExperimentScheduleTypeDef](./type_defs.md#inferenceexperimentscheduletypedef) 
3. See [:material-code-brackets: InferenceExperimentStatusType](./literals.md#inferenceexperimentstatustype) 
4. See [:material-code-braces: EndpointMetadataTypeDef](./type_defs.md#endpointmetadatatypedef) 
5. See [:material-code-braces: ModelVariantConfigSummaryTypeDef](./type_defs.md#modelvariantconfigsummarytypedef) 
6. See [:material-code-braces: InferenceExperimentDataStorageConfigTypeDef](./type_defs.md#inferenceexperimentdatastorageconfigtypedef) 
7. See [:material-code-braces: ShadowModeConfigTypeDef](./type_defs.md#shadowmodeconfigtypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateInferenceExperimentRequestRequestTypeDef

```python
# CreateInferenceExperimentRequestRequestTypeDef definition

class CreateInferenceExperimentRequestRequestTypeDef(TypedDict):
    Name: str,
    Type: InferenceExperimentTypeType,  # (1)
    RoleArn: str,
    EndpointName: str,
    ModelVariants: Sequence[ModelVariantConfigTypeDef],  # (2)
    ShadowModeConfig: ShadowModeConfigTypeDef,  # (3)
    Schedule: NotRequired[InferenceExperimentScheduleTypeDef],  # (4)
    Description: NotRequired[str],
    DataStorageConfig: NotRequired[InferenceExperimentDataStorageConfigTypeDef],  # (5)
    KmsKey: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (6)
```

1. See [:material-code-brackets: InferenceExperimentTypeType](./literals.md#inferenceexperimenttypetype) 
2. See [:material-code-braces: ModelVariantConfigTypeDef](./type_defs.md#modelvariantconfigtypedef) 
3. See [:material-code-braces: ShadowModeConfigTypeDef](./type_defs.md#shadowmodeconfigtypedef) 
4. See [:material-code-braces: InferenceExperimentScheduleTypeDef](./type_defs.md#inferenceexperimentscheduletypedef) 
5. See [:material-code-braces: InferenceExperimentDataStorageConfigTypeDef](./type_defs.md#inferenceexperimentdatastorageconfigtypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## StopInferenceExperimentRequestRequestTypeDef

```python
# StopInferenceExperimentRequestRequestTypeDef definition

class StopInferenceExperimentRequestRequestTypeDef(TypedDict):
    Name: str,
    ModelVariantActions: Mapping[str, ModelVariantActionType],  # (1)
    DesiredModelVariants: NotRequired[Sequence[ModelVariantConfigTypeDef]],  # (2)
    DesiredState: NotRequired[InferenceExperimentStopDesiredStateType],  # (3)
    Reason: NotRequired[str],
```

1. See [:material-code-brackets: ModelVariantActionType](./literals.md#modelvariantactiontype) 
2. See [:material-code-braces: ModelVariantConfigTypeDef](./type_defs.md#modelvariantconfigtypedef) 
3. See [:material-code-brackets: InferenceExperimentStopDesiredStateType](./literals.md#inferenceexperimentstopdesiredstatetype) 
## UpdateInferenceExperimentRequestRequestTypeDef

```python
# UpdateInferenceExperimentRequestRequestTypeDef definition

class UpdateInferenceExperimentRequestRequestTypeDef(TypedDict):
    Name: str,
    Schedule: NotRequired[InferenceExperimentScheduleTypeDef],  # (1)
    Description: NotRequired[str],
    ModelVariants: NotRequired[Sequence[ModelVariantConfigTypeDef]],  # (2)
    DataStorageConfig: NotRequired[InferenceExperimentDataStorageConfigTypeDef],  # (3)
    ShadowModeConfig: NotRequired[ShadowModeConfigTypeDef],  # (4)
```

1. See [:material-code-braces: InferenceExperimentScheduleTypeDef](./type_defs.md#inferenceexperimentscheduletypedef) 
2. See [:material-code-braces: ModelVariantConfigTypeDef](./type_defs.md#modelvariantconfigtypedef) 
3. See [:material-code-braces: InferenceExperimentDataStorageConfigTypeDef](./type_defs.md#inferenceexperimentdatastorageconfigtypedef) 
4. See [:material-code-braces: ShadowModeConfigTypeDef](./type_defs.md#shadowmodeconfigtypedef) 
## UpdateModelPackageInputRequestTypeDef

```python
# UpdateModelPackageInputRequestTypeDef definition

class UpdateModelPackageInputRequestTypeDef(TypedDict):
    ModelPackageArn: str,
    ModelApprovalStatus: NotRequired[ModelApprovalStatusType],  # (1)
    ApprovalDescription: NotRequired[str],
    CustomerMetadataProperties: NotRequired[Mapping[str, str]],
    CustomerMetadataPropertiesToRemove: NotRequired[Sequence[str]],
    AdditionalInferenceSpecificationsToAdd: NotRequired[Sequence[AdditionalInferenceSpecificationDefinitionTypeDef]],  # (2)
```

1. See [:material-code-brackets: ModelApprovalStatusType](./literals.md#modelapprovalstatustype) 
2. See [:material-code-braces: AdditionalInferenceSpecificationDefinitionTypeDef](./type_defs.md#additionalinferencespecificationdefinitiontypedef) 
## BatchDescribeModelPackageSummaryTypeDef

```python
# BatchDescribeModelPackageSummaryTypeDef definition

class BatchDescribeModelPackageSummaryTypeDef(TypedDict):
    ModelPackageGroupName: str,
    ModelPackageArn: str,
    CreationTime: datetime,
    InferenceSpecification: InferenceSpecificationTypeDef,  # (1)
    ModelPackageStatus: ModelPackageStatusType,  # (2)
    ModelPackageVersion: NotRequired[int],
    ModelPackageDescription: NotRequired[str],
    ModelApprovalStatus: NotRequired[ModelApprovalStatusType],  # (3)
```

1. See [:material-code-braces: InferenceSpecificationTypeDef](./type_defs.md#inferencespecificationtypedef) 
2. See [:material-code-brackets: ModelPackageStatusType](./literals.md#modelpackagestatustype) 
3. See [:material-code-brackets: ModelApprovalStatusType](./literals.md#modelapprovalstatustype) 
## DataQualityJobInputTypeDef

```python
# DataQualityJobInputTypeDef definition

class DataQualityJobInputTypeDef(TypedDict):
    EndpointInput: NotRequired[EndpointInputTypeDef],  # (1)
    BatchTransformInput: NotRequired[BatchTransformInputTypeDef],  # (2)
```

1. See [:material-code-braces: EndpointInputTypeDef](./type_defs.md#endpointinputtypedef) 
2. See [:material-code-braces: BatchTransformInputTypeDef](./type_defs.md#batchtransforminputtypedef) 
## ModelBiasJobInputTypeDef

```python
# ModelBiasJobInputTypeDef definition

class ModelBiasJobInputTypeDef(TypedDict):
    GroundTruthS3Input: MonitoringGroundTruthS3InputTypeDef,  # (3)
    EndpointInput: NotRequired[EndpointInputTypeDef],  # (1)
    BatchTransformInput: NotRequired[BatchTransformInputTypeDef],  # (2)
```

1. See [:material-code-braces: EndpointInputTypeDef](./type_defs.md#endpointinputtypedef) 
2. See [:material-code-braces: BatchTransformInputTypeDef](./type_defs.md#batchtransforminputtypedef) 
3. See [:material-code-braces: MonitoringGroundTruthS3InputTypeDef](./type_defs.md#monitoringgroundtruths3inputtypedef) 
## ModelExplainabilityJobInputTypeDef

```python
# ModelExplainabilityJobInputTypeDef definition

class ModelExplainabilityJobInputTypeDef(TypedDict):
    EndpointInput: NotRequired[EndpointInputTypeDef],  # (1)
    BatchTransformInput: NotRequired[BatchTransformInputTypeDef],  # (2)
```

1. See [:material-code-braces: EndpointInputTypeDef](./type_defs.md#endpointinputtypedef) 
2. See [:material-code-braces: BatchTransformInputTypeDef](./type_defs.md#batchtransforminputtypedef) 
## ModelQualityJobInputTypeDef

```python
# ModelQualityJobInputTypeDef definition

class ModelQualityJobInputTypeDef(TypedDict):
    GroundTruthS3Input: MonitoringGroundTruthS3InputTypeDef,  # (3)
    EndpointInput: NotRequired[EndpointInputTypeDef],  # (1)
    BatchTransformInput: NotRequired[BatchTransformInputTypeDef],  # (2)
```

1. See [:material-code-braces: EndpointInputTypeDef](./type_defs.md#endpointinputtypedef) 
2. See [:material-code-braces: BatchTransformInputTypeDef](./type_defs.md#batchtransforminputtypedef) 
3. See [:material-code-braces: MonitoringGroundTruthS3InputTypeDef](./type_defs.md#monitoringgroundtruths3inputtypedef) 
## MonitoringInputTypeDef

```python
# MonitoringInputTypeDef definition

class MonitoringInputTypeDef(TypedDict):
    EndpointInput: NotRequired[EndpointInputTypeDef],  # (1)
    BatchTransformInput: NotRequired[BatchTransformInputTypeDef],  # (2)
```

1. See [:material-code-braces: EndpointInputTypeDef](./type_defs.md#endpointinputtypedef) 
2. See [:material-code-braces: BatchTransformInputTypeDef](./type_defs.md#batchtransforminputtypedef) 
## CreateProcessingJobRequestRequestTypeDef

```python
# CreateProcessingJobRequestRequestTypeDef definition

class CreateProcessingJobRequestRequestTypeDef(TypedDict):
    ProcessingJobName: str,
    ProcessingResources: ProcessingResourcesTypeDef,  # (1)
    AppSpecification: AppSpecificationTypeDef,  # (2)
    RoleArn: str,
    ProcessingInputs: NotRequired[Sequence[ProcessingInputTypeDef]],  # (3)
    ProcessingOutputConfig: NotRequired[ProcessingOutputConfigTypeDef],  # (4)
    StoppingCondition: NotRequired[ProcessingStoppingConditionTypeDef],  # (5)
    Environment: NotRequired[Mapping[str, str]],
    NetworkConfig: NotRequired[NetworkConfigTypeDef],  # (6)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (7)
    ExperimentConfig: NotRequired[ExperimentConfigTypeDef],  # (8)
```

1. See [:material-code-braces: ProcessingResourcesTypeDef](./type_defs.md#processingresourcestypedef) 
2. See [:material-code-braces: AppSpecificationTypeDef](./type_defs.md#appspecificationtypedef) 
3. See [:material-code-braces: ProcessingInputTypeDef](./type_defs.md#processinginputtypedef) 
4. See [:material-code-braces: ProcessingOutputConfigTypeDef](./type_defs.md#processingoutputconfigtypedef) 
5. See [:material-code-braces: ProcessingStoppingConditionTypeDef](./type_defs.md#processingstoppingconditiontypedef) 
6. See [:material-code-braces: NetworkConfigTypeDef](./type_defs.md#networkconfigtypedef) 
7. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
8. See [:material-code-braces: ExperimentConfigTypeDef](./type_defs.md#experimentconfigtypedef) 
## DescribeProcessingJobResponseTypeDef

```python
# DescribeProcessingJobResponseTypeDef definition

class DescribeProcessingJobResponseTypeDef(TypedDict):
    ProcessingInputs: List[ProcessingInputTypeDef],  # (1)
    ProcessingOutputConfig: ProcessingOutputConfigTypeDef,  # (2)
    ProcessingJobName: str,
    ProcessingResources: ProcessingResourcesTypeDef,  # (3)
    StoppingCondition: ProcessingStoppingConditionTypeDef,  # (4)
    AppSpecification: AppSpecificationTypeDef,  # (5)
    Environment: Dict[str, str],
    NetworkConfig: NetworkConfigTypeDef,  # (6)
    RoleArn: str,
    ExperimentConfig: ExperimentConfigTypeDef,  # (7)
    ProcessingJobArn: str,
    ProcessingJobStatus: ProcessingJobStatusType,  # (8)
    ExitMessage: str,
    FailureReason: str,
    ProcessingEndTime: datetime,
    ProcessingStartTime: datetime,
    LastModifiedTime: datetime,
    CreationTime: datetime,
    MonitoringScheduleArn: str,
    AutoMLJobArn: str,
    TrainingJobArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (9)
```

1. See [:material-code-braces: ProcessingInputTypeDef](./type_defs.md#processinginputtypedef) 
2. See [:material-code-braces: ProcessingOutputConfigTypeDef](./type_defs.md#processingoutputconfigtypedef) 
3. See [:material-code-braces: ProcessingResourcesTypeDef](./type_defs.md#processingresourcestypedef) 
4. See [:material-code-braces: ProcessingStoppingConditionTypeDef](./type_defs.md#processingstoppingconditiontypedef) 
5. See [:material-code-braces: AppSpecificationTypeDef](./type_defs.md#appspecificationtypedef) 
6. See [:material-code-braces: NetworkConfigTypeDef](./type_defs.md#networkconfigtypedef) 
7. See [:material-code-braces: ExperimentConfigTypeDef](./type_defs.md#experimentconfigtypedef) 
8. See [:material-code-brackets: ProcessingJobStatusType](./literals.md#processingjobstatustype) 
9. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProcessingJobTypeDef

```python
# ProcessingJobTypeDef definition

class ProcessingJobTypeDef(TypedDict):
    ProcessingInputs: NotRequired[List[ProcessingInputTypeDef]],  # (1)
    ProcessingOutputConfig: NotRequired[ProcessingOutputConfigTypeDef],  # (2)
    ProcessingJobName: NotRequired[str],
    ProcessingResources: NotRequired[ProcessingResourcesTypeDef],  # (3)
    StoppingCondition: NotRequired[ProcessingStoppingConditionTypeDef],  # (4)
    AppSpecification: NotRequired[AppSpecificationTypeDef],  # (5)
    Environment: NotRequired[Dict[str, str]],
    NetworkConfig: NotRequired[NetworkConfigTypeDef],  # (6)
    RoleArn: NotRequired[str],
    ExperimentConfig: NotRequired[ExperimentConfigTypeDef],  # (7)
    ProcessingJobArn: NotRequired[str],
    ProcessingJobStatus: NotRequired[ProcessingJobStatusType],  # (8)
    ExitMessage: NotRequired[str],
    FailureReason: NotRequired[str],
    ProcessingEndTime: NotRequired[datetime],
    ProcessingStartTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
    CreationTime: NotRequired[datetime],
    MonitoringScheduleArn: NotRequired[str],
    AutoMLJobArn: NotRequired[str],
    TrainingJobArn: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (9)
```

1. See [:material-code-braces: ProcessingInputTypeDef](./type_defs.md#processinginputtypedef) 
2. See [:material-code-braces: ProcessingOutputConfigTypeDef](./type_defs.md#processingoutputconfigtypedef) 
3. See [:material-code-braces: ProcessingResourcesTypeDef](./type_defs.md#processingresourcestypedef) 
4. See [:material-code-braces: ProcessingStoppingConditionTypeDef](./type_defs.md#processingstoppingconditiontypedef) 
5. See [:material-code-braces: AppSpecificationTypeDef](./type_defs.md#appspecificationtypedef) 
6. See [:material-code-braces: NetworkConfigTypeDef](./type_defs.md#networkconfigtypedef) 
7. See [:material-code-braces: ExperimentConfigTypeDef](./type_defs.md#experimentconfigtypedef) 
8. See [:material-code-brackets: ProcessingJobStatusType](./literals.md#processingjobstatustype) 
9. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateFlowDefinitionRequestRequestTypeDef

```python
# CreateFlowDefinitionRequestRequestTypeDef definition

class CreateFlowDefinitionRequestRequestTypeDef(TypedDict):
    FlowDefinitionName: str,
    HumanLoopConfig: HumanLoopConfigTypeDef,  # (1)
    OutputConfig: FlowDefinitionOutputConfigTypeDef,  # (2)
    RoleArn: str,
    HumanLoopRequestSource: NotRequired[HumanLoopRequestSourceTypeDef],  # (3)
    HumanLoopActivationConfig: NotRequired[HumanLoopActivationConfigTypeDef],  # (4)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (5)
```

1. See [:material-code-braces: HumanLoopConfigTypeDef](./type_defs.md#humanloopconfigtypedef) 
2. See [:material-code-braces: FlowDefinitionOutputConfigTypeDef](./type_defs.md#flowdefinitionoutputconfigtypedef) 
3. See [:material-code-braces: HumanLoopRequestSourceTypeDef](./type_defs.md#humanlooprequestsourcetypedef) 
4. See [:material-code-braces: HumanLoopActivationConfigTypeDef](./type_defs.md#humanloopactivationconfigtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeFlowDefinitionResponseTypeDef

```python
# DescribeFlowDefinitionResponseTypeDef definition

class DescribeFlowDefinitionResponseTypeDef(TypedDict):
    FlowDefinitionArn: str,
    FlowDefinitionName: str,
    FlowDefinitionStatus: FlowDefinitionStatusType,  # (1)
    CreationTime: datetime,
    HumanLoopRequestSource: HumanLoopRequestSourceTypeDef,  # (2)
    HumanLoopActivationConfig: HumanLoopActivationConfigTypeDef,  # (3)
    HumanLoopConfig: HumanLoopConfigTypeDef,  # (4)
    OutputConfig: FlowDefinitionOutputConfigTypeDef,  # (5)
    RoleArn: str,
    FailureReason: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: FlowDefinitionStatusType](./literals.md#flowdefinitionstatustype) 
2. See [:material-code-braces: HumanLoopRequestSourceTypeDef](./type_defs.md#humanlooprequestsourcetypedef) 
3. See [:material-code-braces: HumanLoopActivationConfigTypeDef](./type_defs.md#humanloopactivationconfigtypedef) 
4. See [:material-code-braces: HumanLoopConfigTypeDef](./type_defs.md#humanloopconfigtypedef) 
5. See [:material-code-braces: FlowDefinitionOutputConfigTypeDef](./type_defs.md#flowdefinitionoutputconfigtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLabelingJobRequestRequestTypeDef

```python
# CreateLabelingJobRequestRequestTypeDef definition

class CreateLabelingJobRequestRequestTypeDef(TypedDict):
    LabelingJobName: str,
    LabelAttributeName: str,
    InputConfig: LabelingJobInputConfigTypeDef,  # (1)
    OutputConfig: LabelingJobOutputConfigTypeDef,  # (2)
    RoleArn: str,
    HumanTaskConfig: HumanTaskConfigTypeDef,  # (3)
    LabelCategoryConfigS3Uri: NotRequired[str],
    StoppingConditions: NotRequired[LabelingJobStoppingConditionsTypeDef],  # (4)
    LabelingJobAlgorithmsConfig: NotRequired[LabelingJobAlgorithmsConfigTypeDef],  # (5)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (6)
```

1. See [:material-code-braces: LabelingJobInputConfigTypeDef](./type_defs.md#labelingjobinputconfigtypedef) 
2. See [:material-code-braces: LabelingJobOutputConfigTypeDef](./type_defs.md#labelingjoboutputconfigtypedef) 
3. See [:material-code-braces: HumanTaskConfigTypeDef](./type_defs.md#humantaskconfigtypedef) 
4. See [:material-code-braces: LabelingJobStoppingConditionsTypeDef](./type_defs.md#labelingjobstoppingconditionstypedef) 
5. See [:material-code-braces: LabelingJobAlgorithmsConfigTypeDef](./type_defs.md#labelingjobalgorithmsconfigtypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeLabelingJobResponseTypeDef

```python
# DescribeLabelingJobResponseTypeDef definition

class DescribeLabelingJobResponseTypeDef(TypedDict):
    LabelingJobStatus: LabelingJobStatusType,  # (1)
    LabelCounters: LabelCountersTypeDef,  # (2)
    FailureReason: str,
    CreationTime: datetime,
    LastModifiedTime: datetime,
    JobReferenceCode: str,
    LabelingJobName: str,
    LabelingJobArn: str,
    LabelAttributeName: str,
    InputConfig: LabelingJobInputConfigTypeDef,  # (3)
    OutputConfig: LabelingJobOutputConfigTypeDef,  # (4)
    RoleArn: str,
    LabelCategoryConfigS3Uri: str,
    StoppingConditions: LabelingJobStoppingConditionsTypeDef,  # (5)
    LabelingJobAlgorithmsConfig: LabelingJobAlgorithmsConfigTypeDef,  # (6)
    HumanTaskConfig: HumanTaskConfigTypeDef,  # (7)
    Tags: List[TagTypeDef],  # (8)
    LabelingJobOutput: LabelingJobOutputTypeDef,  # (9)
    ResponseMetadata: ResponseMetadataTypeDef,  # (10)
```

1. See [:material-code-brackets: LabelingJobStatusType](./literals.md#labelingjobstatustype) 
2. See [:material-code-braces: LabelCountersTypeDef](./type_defs.md#labelcounterstypedef) 
3. See [:material-code-braces: LabelingJobInputConfigTypeDef](./type_defs.md#labelingjobinputconfigtypedef) 
4. See [:material-code-braces: LabelingJobOutputConfigTypeDef](./type_defs.md#labelingjoboutputconfigtypedef) 
5. See [:material-code-braces: LabelingJobStoppingConditionsTypeDef](./type_defs.md#labelingjobstoppingconditionstypedef) 
6. See [:material-code-braces: LabelingJobAlgorithmsConfigTypeDef](./type_defs.md#labelingjobalgorithmsconfigtypedef) 
7. See [:material-code-braces: HumanTaskConfigTypeDef](./type_defs.md#humantaskconfigtypedef) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
9. See [:material-code-braces: LabelingJobOutputTypeDef](./type_defs.md#labelingjoboutputtypedef) 
10. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTrainingJobRequestRequestTypeDef

```python
# CreateTrainingJobRequestRequestTypeDef definition

class CreateTrainingJobRequestRequestTypeDef(TypedDict):
    TrainingJobName: str,
    AlgorithmSpecification: AlgorithmSpecificationTypeDef,  # (1)
    RoleArn: str,
    OutputDataConfig: OutputDataConfigTypeDef,  # (2)
    ResourceConfig: ResourceConfigTypeDef,  # (3)
    StoppingCondition: StoppingConditionTypeDef,  # (4)
    HyperParameters: NotRequired[Mapping[str, str]],
    InputDataConfig: NotRequired[Sequence[ChannelTypeDef]],  # (5)
    VpcConfig: NotRequired[VpcConfigTypeDef],  # (6)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (7)
    EnableNetworkIsolation: NotRequired[bool],
    EnableInterContainerTrafficEncryption: NotRequired[bool],
    EnableManagedSpotTraining: NotRequired[bool],
    CheckpointConfig: NotRequired[CheckpointConfigTypeDef],  # (8)
    DebugHookConfig: NotRequired[DebugHookConfigTypeDef],  # (9)
    DebugRuleConfigurations: NotRequired[Sequence[DebugRuleConfigurationTypeDef]],  # (10)
    TensorBoardOutputConfig: NotRequired[TensorBoardOutputConfigTypeDef],  # (11)
    ExperimentConfig: NotRequired[ExperimentConfigTypeDef],  # (12)
    ProfilerConfig: NotRequired[ProfilerConfigTypeDef],  # (13)
    ProfilerRuleConfigurations: NotRequired[Sequence[ProfilerRuleConfigurationTypeDef]],  # (14)
    Environment: NotRequired[Mapping[str, str]],
    RetryStrategy: NotRequired[RetryStrategyTypeDef],  # (15)
```

1. See [:material-code-braces: AlgorithmSpecificationTypeDef](./type_defs.md#algorithmspecificationtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-braces: ResourceConfigTypeDef](./type_defs.md#resourceconfigtypedef) 
4. See [:material-code-braces: StoppingConditionTypeDef](./type_defs.md#stoppingconditiontypedef) 
5. See [:material-code-braces: ChannelTypeDef](./type_defs.md#channeltypedef) 
6. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
7. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
8. See [:material-code-braces: CheckpointConfigTypeDef](./type_defs.md#checkpointconfigtypedef) 
9. See [:material-code-braces: DebugHookConfigTypeDef](./type_defs.md#debughookconfigtypedef) 
10. See [:material-code-braces: DebugRuleConfigurationTypeDef](./type_defs.md#debugruleconfigurationtypedef) 
11. See [:material-code-braces: TensorBoardOutputConfigTypeDef](./type_defs.md#tensorboardoutputconfigtypedef) 
12. See [:material-code-braces: ExperimentConfigTypeDef](./type_defs.md#experimentconfigtypedef) 
13. See [:material-code-braces: ProfilerConfigTypeDef](./type_defs.md#profilerconfigtypedef) 
14. See [:material-code-braces: ProfilerRuleConfigurationTypeDef](./type_defs.md#profilerruleconfigurationtypedef) 
15. See [:material-code-braces: RetryStrategyTypeDef](./type_defs.md#retrystrategytypedef) 
## DescribeTrainingJobResponseTypeDef

```python
# DescribeTrainingJobResponseTypeDef definition

class DescribeTrainingJobResponseTypeDef(TypedDict):
    TrainingJobName: str,
    TrainingJobArn: str,
    TuningJobArn: str,
    LabelingJobArn: str,
    AutoMLJobArn: str,
    ModelArtifacts: ModelArtifactsTypeDef,  # (1)
    TrainingJobStatus: TrainingJobStatusType,  # (2)
    SecondaryStatus: SecondaryStatusType,  # (3)
    FailureReason: str,
    HyperParameters: Dict[str, str],
    AlgorithmSpecification: AlgorithmSpecificationTypeDef,  # (4)
    RoleArn: str,
    InputDataConfig: List[ChannelTypeDef],  # (5)
    OutputDataConfig: OutputDataConfigTypeDef,  # (6)
    ResourceConfig: ResourceConfigTypeDef,  # (7)
    VpcConfig: VpcConfigTypeDef,  # (8)
    StoppingCondition: StoppingConditionTypeDef,  # (9)
    CreationTime: datetime,
    TrainingStartTime: datetime,
    TrainingEndTime: datetime,
    LastModifiedTime: datetime,
    SecondaryStatusTransitions: List[SecondaryStatusTransitionTypeDef],  # (10)
    FinalMetricDataList: List[MetricDataTypeDef],  # (11)
    EnableNetworkIsolation: bool,
    EnableInterContainerTrafficEncryption: bool,
    EnableManagedSpotTraining: bool,
    CheckpointConfig: CheckpointConfigTypeDef,  # (12)
    TrainingTimeInSeconds: int,
    BillableTimeInSeconds: int,
    DebugHookConfig: DebugHookConfigTypeDef,  # (13)
    ExperimentConfig: ExperimentConfigTypeDef,  # (14)
    DebugRuleConfigurations: List[DebugRuleConfigurationTypeDef],  # (15)
    TensorBoardOutputConfig: TensorBoardOutputConfigTypeDef,  # (16)
    DebugRuleEvaluationStatuses: List[DebugRuleEvaluationStatusTypeDef],  # (17)
    ProfilerConfig: ProfilerConfigTypeDef,  # (18)
    ProfilerRuleConfigurations: List[ProfilerRuleConfigurationTypeDef],  # (19)
    ProfilerRuleEvaluationStatuses: List[ProfilerRuleEvaluationStatusTypeDef],  # (20)
    ProfilingStatus: ProfilingStatusType,  # (21)
    RetryStrategy: RetryStrategyTypeDef,  # (22)
    Environment: Dict[str, str],
    WarmPoolStatus: WarmPoolStatusTypeDef,  # (23)
    ResponseMetadata: ResponseMetadataTypeDef,  # (24)
```

1. See [:material-code-braces: ModelArtifactsTypeDef](./type_defs.md#modelartifactstypedef) 
2. See [:material-code-brackets: TrainingJobStatusType](./literals.md#trainingjobstatustype) 
3. See [:material-code-brackets: SecondaryStatusType](./literals.md#secondarystatustype) 
4. See [:material-code-braces: AlgorithmSpecificationTypeDef](./type_defs.md#algorithmspecificationtypedef) 
5. See [:material-code-braces: ChannelTypeDef](./type_defs.md#channeltypedef) 
6. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
7. See [:material-code-braces: ResourceConfigTypeDef](./type_defs.md#resourceconfigtypedef) 
8. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
9. See [:material-code-braces: StoppingConditionTypeDef](./type_defs.md#stoppingconditiontypedef) 
10. See [:material-code-braces: SecondaryStatusTransitionTypeDef](./type_defs.md#secondarystatustransitiontypedef) 
11. See [:material-code-braces: MetricDataTypeDef](./type_defs.md#metricdatatypedef) 
12. See [:material-code-braces: CheckpointConfigTypeDef](./type_defs.md#checkpointconfigtypedef) 
13. See [:material-code-braces: DebugHookConfigTypeDef](./type_defs.md#debughookconfigtypedef) 
14. See [:material-code-braces: ExperimentConfigTypeDef](./type_defs.md#experimentconfigtypedef) 
15. See [:material-code-braces: DebugRuleConfigurationTypeDef](./type_defs.md#debugruleconfigurationtypedef) 
16. See [:material-code-braces: TensorBoardOutputConfigTypeDef](./type_defs.md#tensorboardoutputconfigtypedef) 
17. See [:material-code-braces: DebugRuleEvaluationStatusTypeDef](./type_defs.md#debugruleevaluationstatustypedef) 
18. See [:material-code-braces: ProfilerConfigTypeDef](./type_defs.md#profilerconfigtypedef) 
19. See [:material-code-braces: ProfilerRuleConfigurationTypeDef](./type_defs.md#profilerruleconfigurationtypedef) 
20. See [:material-code-braces: ProfilerRuleEvaluationStatusTypeDef](./type_defs.md#profilerruleevaluationstatustypedef) 
21. See [:material-code-brackets: ProfilingStatusType](./literals.md#profilingstatustype) 
22. See [:material-code-braces: RetryStrategyTypeDef](./type_defs.md#retrystrategytypedef) 
23. See [:material-code-braces: WarmPoolStatusTypeDef](./type_defs.md#warmpoolstatustypedef) 
24. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TrainingJobTypeDef

```python
# TrainingJobTypeDef definition

class TrainingJobTypeDef(TypedDict):
    TrainingJobName: NotRequired[str],
    TrainingJobArn: NotRequired[str],
    TuningJobArn: NotRequired[str],
    LabelingJobArn: NotRequired[str],
    AutoMLJobArn: NotRequired[str],
    ModelArtifacts: NotRequired[ModelArtifactsTypeDef],  # (1)
    TrainingJobStatus: NotRequired[TrainingJobStatusType],  # (2)
    SecondaryStatus: NotRequired[SecondaryStatusType],  # (3)
    FailureReason: NotRequired[str],
    HyperParameters: NotRequired[Dict[str, str]],
    AlgorithmSpecification: NotRequired[AlgorithmSpecificationTypeDef],  # (4)
    RoleArn: NotRequired[str],
    InputDataConfig: NotRequired[List[ChannelTypeDef]],  # (5)
    OutputDataConfig: NotRequired[OutputDataConfigTypeDef],  # (6)
    ResourceConfig: NotRequired[ResourceConfigTypeDef],  # (7)
    VpcConfig: NotRequired[VpcConfigTypeDef],  # (8)
    StoppingCondition: NotRequired[StoppingConditionTypeDef],  # (9)
    CreationTime: NotRequired[datetime],
    TrainingStartTime: NotRequired[datetime],
    TrainingEndTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
    SecondaryStatusTransitions: NotRequired[List[SecondaryStatusTransitionTypeDef]],  # (10)
    FinalMetricDataList: NotRequired[List[MetricDataTypeDef]],  # (11)
    EnableNetworkIsolation: NotRequired[bool],
    EnableInterContainerTrafficEncryption: NotRequired[bool],
    EnableManagedSpotTraining: NotRequired[bool],
    CheckpointConfig: NotRequired[CheckpointConfigTypeDef],  # (12)
    TrainingTimeInSeconds: NotRequired[int],
    BillableTimeInSeconds: NotRequired[int],
    DebugHookConfig: NotRequired[DebugHookConfigTypeDef],  # (13)
    ExperimentConfig: NotRequired[ExperimentConfigTypeDef],  # (14)
    DebugRuleConfigurations: NotRequired[List[DebugRuleConfigurationTypeDef]],  # (15)
    TensorBoardOutputConfig: NotRequired[TensorBoardOutputConfigTypeDef],  # (16)
    DebugRuleEvaluationStatuses: NotRequired[List[DebugRuleEvaluationStatusTypeDef]],  # (17)
    ProfilerConfig: NotRequired[ProfilerConfigTypeDef],  # (18)
    Environment: NotRequired[Dict[str, str]],
    RetryStrategy: NotRequired[RetryStrategyTypeDef],  # (19)
    Tags: NotRequired[List[TagTypeDef]],  # (20)
```

1. See [:material-code-braces: ModelArtifactsTypeDef](./type_defs.md#modelartifactstypedef) 
2. See [:material-code-brackets: TrainingJobStatusType](./literals.md#trainingjobstatustype) 
3. See [:material-code-brackets: SecondaryStatusType](./literals.md#secondarystatustype) 
4. See [:material-code-braces: AlgorithmSpecificationTypeDef](./type_defs.md#algorithmspecificationtypedef) 
5. See [:material-code-braces: ChannelTypeDef](./type_defs.md#channeltypedef) 
6. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
7. See [:material-code-braces: ResourceConfigTypeDef](./type_defs.md#resourceconfigtypedef) 
8. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
9. See [:material-code-braces: StoppingConditionTypeDef](./type_defs.md#stoppingconditiontypedef) 
10. See [:material-code-braces: SecondaryStatusTransitionTypeDef](./type_defs.md#secondarystatustransitiontypedef) 
11. See [:material-code-braces: MetricDataTypeDef](./type_defs.md#metricdatatypedef) 
12. See [:material-code-braces: CheckpointConfigTypeDef](./type_defs.md#checkpointconfigtypedef) 
13. See [:material-code-braces: DebugHookConfigTypeDef](./type_defs.md#debughookconfigtypedef) 
14. See [:material-code-braces: ExperimentConfigTypeDef](./type_defs.md#experimentconfigtypedef) 
15. See [:material-code-braces: DebugRuleConfigurationTypeDef](./type_defs.md#debugruleconfigurationtypedef) 
16. See [:material-code-braces: TensorBoardOutputConfigTypeDef](./type_defs.md#tensorboardoutputconfigtypedef) 
17. See [:material-code-braces: DebugRuleEvaluationStatusTypeDef](./type_defs.md#debugruleevaluationstatustypedef) 
18. See [:material-code-braces: ProfilerConfigTypeDef](./type_defs.md#profilerconfigtypedef) 
19. See [:material-code-braces: RetryStrategyTypeDef](./type_defs.md#retrystrategytypedef) 
20. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateTransformJobRequestRequestTypeDef

```python
# CreateTransformJobRequestRequestTypeDef definition

class CreateTransformJobRequestRequestTypeDef(TypedDict):
    TransformJobName: str,
    ModelName: str,
    TransformInput: TransformInputTypeDef,  # (1)
    TransformOutput: TransformOutputTypeDef,  # (2)
    TransformResources: TransformResourcesTypeDef,  # (3)
    MaxConcurrentTransforms: NotRequired[int],
    ModelClientConfig: NotRequired[ModelClientConfigTypeDef],  # (4)
    MaxPayloadInMB: NotRequired[int],
    BatchStrategy: NotRequired[BatchStrategyType],  # (5)
    Environment: NotRequired[Mapping[str, str]],
    DataCaptureConfig: NotRequired[BatchDataCaptureConfigTypeDef],  # (6)
    DataProcessing: NotRequired[DataProcessingTypeDef],  # (7)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (8)
    ExperimentConfig: NotRequired[ExperimentConfigTypeDef],  # (9)
```

1. See [:material-code-braces: TransformInputTypeDef](./type_defs.md#transforminputtypedef) 
2. See [:material-code-braces: TransformOutputTypeDef](./type_defs.md#transformoutputtypedef) 
3. See [:material-code-braces: TransformResourcesTypeDef](./type_defs.md#transformresourcestypedef) 
4. See [:material-code-braces: ModelClientConfigTypeDef](./type_defs.md#modelclientconfigtypedef) 
5. See [:material-code-brackets: BatchStrategyType](./literals.md#batchstrategytype) 
6. See [:material-code-braces: BatchDataCaptureConfigTypeDef](./type_defs.md#batchdatacaptureconfigtypedef) 
7. See [:material-code-braces: DataProcessingTypeDef](./type_defs.md#dataprocessingtypedef) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
9. See [:material-code-braces: ExperimentConfigTypeDef](./type_defs.md#experimentconfigtypedef) 
## DescribeTransformJobResponseTypeDef

```python
# DescribeTransformJobResponseTypeDef definition

class DescribeTransformJobResponseTypeDef(TypedDict):
    TransformJobName: str,
    TransformJobArn: str,
    TransformJobStatus: TransformJobStatusType,  # (1)
    FailureReason: str,
    ModelName: str,
    MaxConcurrentTransforms: int,
    ModelClientConfig: ModelClientConfigTypeDef,  # (2)
    MaxPayloadInMB: int,
    BatchStrategy: BatchStrategyType,  # (3)
    Environment: Dict[str, str],
    TransformInput: TransformInputTypeDef,  # (4)
    TransformOutput: TransformOutputTypeDef,  # (5)
    DataCaptureConfig: BatchDataCaptureConfigTypeDef,  # (6)
    TransformResources: TransformResourcesTypeDef,  # (7)
    CreationTime: datetime,
    TransformStartTime: datetime,
    TransformEndTime: datetime,
    LabelingJobArn: str,
    AutoMLJobArn: str,
    DataProcessing: DataProcessingTypeDef,  # (8)
    ExperimentConfig: ExperimentConfigTypeDef,  # (9)
    ResponseMetadata: ResponseMetadataTypeDef,  # (10)
```

1. See [:material-code-brackets: TransformJobStatusType](./literals.md#transformjobstatustype) 
2. See [:material-code-braces: ModelClientConfigTypeDef](./type_defs.md#modelclientconfigtypedef) 
3. See [:material-code-brackets: BatchStrategyType](./literals.md#batchstrategytype) 
4. See [:material-code-braces: TransformInputTypeDef](./type_defs.md#transforminputtypedef) 
5. See [:material-code-braces: TransformOutputTypeDef](./type_defs.md#transformoutputtypedef) 
6. See [:material-code-braces: BatchDataCaptureConfigTypeDef](./type_defs.md#batchdatacaptureconfigtypedef) 
7. See [:material-code-braces: TransformResourcesTypeDef](./type_defs.md#transformresourcestypedef) 
8. See [:material-code-braces: DataProcessingTypeDef](./type_defs.md#dataprocessingtypedef) 
9. See [:material-code-braces: ExperimentConfigTypeDef](./type_defs.md#experimentconfigtypedef) 
10. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TransformJobDefinitionTypeDef

```python
# TransformJobDefinitionTypeDef definition

class TransformJobDefinitionTypeDef(TypedDict):
    TransformInput: TransformInputTypeDef,  # (2)
    TransformOutput: TransformOutputTypeDef,  # (3)
    TransformResources: TransformResourcesTypeDef,  # (4)
    MaxConcurrentTransforms: NotRequired[int],
    MaxPayloadInMB: NotRequired[int],
    BatchStrategy: NotRequired[BatchStrategyType],  # (1)
    Environment: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: BatchStrategyType](./literals.md#batchstrategytype) 
2. See [:material-code-braces: TransformInputTypeDef](./type_defs.md#transforminputtypedef) 
3. See [:material-code-braces: TransformOutputTypeDef](./type_defs.md#transformoutputtypedef) 
4. See [:material-code-braces: TransformResourcesTypeDef](./type_defs.md#transformresourcestypedef) 
## TransformJobTypeDef

```python
# TransformJobTypeDef definition

class TransformJobTypeDef(TypedDict):
    TransformJobName: NotRequired[str],
    TransformJobArn: NotRequired[str],
    TransformJobStatus: NotRequired[TransformJobStatusType],  # (1)
    FailureReason: NotRequired[str],
    ModelName: NotRequired[str],
    MaxConcurrentTransforms: NotRequired[int],
    ModelClientConfig: NotRequired[ModelClientConfigTypeDef],  # (2)
    MaxPayloadInMB: NotRequired[int],
    BatchStrategy: NotRequired[BatchStrategyType],  # (3)
    Environment: NotRequired[Dict[str, str]],
    TransformInput: NotRequired[TransformInputTypeDef],  # (4)
    TransformOutput: NotRequired[TransformOutputTypeDef],  # (5)
    TransformResources: NotRequired[TransformResourcesTypeDef],  # (6)
    CreationTime: NotRequired[datetime],
    TransformStartTime: NotRequired[datetime],
    TransformEndTime: NotRequired[datetime],
    LabelingJobArn: NotRequired[str],
    AutoMLJobArn: NotRequired[str],
    DataProcessing: NotRequired[DataProcessingTypeDef],  # (7)
    ExperimentConfig: NotRequired[ExperimentConfigTypeDef],  # (8)
    Tags: NotRequired[List[TagTypeDef]],  # (9)
    DataCaptureConfig: NotRequired[BatchDataCaptureConfigTypeDef],  # (10)
```

1. See [:material-code-brackets: TransformJobStatusType](./literals.md#transformjobstatustype) 
2. See [:material-code-braces: ModelClientConfigTypeDef](./type_defs.md#modelclientconfigtypedef) 
3. See [:material-code-brackets: BatchStrategyType](./literals.md#batchstrategytype) 
4. See [:material-code-braces: TransformInputTypeDef](./type_defs.md#transforminputtypedef) 
5. See [:material-code-braces: TransformOutputTypeDef](./type_defs.md#transformoutputtypedef) 
6. See [:material-code-braces: TransformResourcesTypeDef](./type_defs.md#transformresourcestypedef) 
7. See [:material-code-braces: DataProcessingTypeDef](./type_defs.md#dataprocessingtypedef) 
8. See [:material-code-braces: ExperimentConfigTypeDef](./type_defs.md#experimentconfigtypedef) 
9. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
10. See [:material-code-braces: BatchDataCaptureConfigTypeDef](./type_defs.md#batchdatacaptureconfigtypedef) 
## CreateAutoMLJobV2RequestRequestTypeDef

```python
# CreateAutoMLJobV2RequestRequestTypeDef definition

class CreateAutoMLJobV2RequestRequestTypeDef(TypedDict):
    AutoMLJobName: str,
    AutoMLJobInputDataConfig: Sequence[AutoMLJobChannelTypeDef],  # (1)
    OutputDataConfig: AutoMLOutputDataConfigTypeDef,  # (2)
    AutoMLProblemTypeConfig: AutoMLProblemTypeConfigTypeDef,  # (3)
    RoleArn: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
    SecurityConfig: NotRequired[AutoMLSecurityConfigTypeDef],  # (5)
    AutoMLJobObjective: NotRequired[AutoMLJobObjectiveTypeDef],  # (6)
    ModelDeployConfig: NotRequired[ModelDeployConfigTypeDef],  # (7)
    DataSplitConfig: NotRequired[AutoMLDataSplitConfigTypeDef],  # (8)
```

1. See [:material-code-braces: AutoMLJobChannelTypeDef](./type_defs.md#automljobchanneltypedef) 
2. See [:material-code-braces: AutoMLOutputDataConfigTypeDef](./type_defs.md#automloutputdataconfigtypedef) 
3. See [:material-code-braces: AutoMLProblemTypeConfigTypeDef](./type_defs.md#automlproblemtypeconfigtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: AutoMLSecurityConfigTypeDef](./type_defs.md#automlsecurityconfigtypedef) 
6. See [:material-code-braces: AutoMLJobObjectiveTypeDef](./type_defs.md#automljobobjectivetypedef) 
7. See [:material-code-braces: ModelDeployConfigTypeDef](./type_defs.md#modeldeployconfigtypedef) 
8. See [:material-code-braces: AutoMLDataSplitConfigTypeDef](./type_defs.md#automldatasplitconfigtypedef) 
## DescribeAutoMLJobV2ResponseTypeDef

```python
# DescribeAutoMLJobV2ResponseTypeDef definition

class DescribeAutoMLJobV2ResponseTypeDef(TypedDict):
    AutoMLJobName: str,
    AutoMLJobArn: str,
    AutoMLJobInputDataConfig: List[AutoMLJobChannelTypeDef],  # (1)
    OutputDataConfig: AutoMLOutputDataConfigTypeDef,  # (2)
    RoleArn: str,
    AutoMLJobObjective: AutoMLJobObjectiveTypeDef,  # (3)
    AutoMLProblemTypeConfig: AutoMLProblemTypeConfigTypeDef,  # (4)
    CreationTime: datetime,
    EndTime: datetime,
    LastModifiedTime: datetime,
    FailureReason: str,
    PartialFailureReasons: List[AutoMLPartialFailureReasonTypeDef],  # (5)
    BestCandidate: AutoMLCandidateTypeDef,  # (6)
    AutoMLJobStatus: AutoMLJobStatusType,  # (7)
    AutoMLJobSecondaryStatus: AutoMLJobSecondaryStatusType,  # (8)
    ModelDeployConfig: ModelDeployConfigTypeDef,  # (9)
    ModelDeployResult: ModelDeployResultTypeDef,  # (10)
    DataSplitConfig: AutoMLDataSplitConfigTypeDef,  # (11)
    SecurityConfig: AutoMLSecurityConfigTypeDef,  # (12)
    AutoMLJobArtifacts: AutoMLJobArtifactsTypeDef,  # (13)
    ResolvedAttributes: AutoMLResolvedAttributesTypeDef,  # (14)
    AutoMLProblemTypeConfigName: AutoMLProblemTypeConfigNameType,  # (15)
    ResponseMetadata: ResponseMetadataTypeDef,  # (16)
```

1. See [:material-code-braces: AutoMLJobChannelTypeDef](./type_defs.md#automljobchanneltypedef) 
2. See [:material-code-braces: AutoMLOutputDataConfigTypeDef](./type_defs.md#automloutputdataconfigtypedef) 
3. See [:material-code-braces: AutoMLJobObjectiveTypeDef](./type_defs.md#automljobobjectivetypedef) 
4. See [:material-code-braces: AutoMLProblemTypeConfigTypeDef](./type_defs.md#automlproblemtypeconfigtypedef) 
5. See [:material-code-braces: AutoMLPartialFailureReasonTypeDef](./type_defs.md#automlpartialfailurereasontypedef) 
6. See [:material-code-braces: AutoMLCandidateTypeDef](./type_defs.md#automlcandidatetypedef) 
7. See [:material-code-brackets: AutoMLJobStatusType](./literals.md#automljobstatustype) 
8. See [:material-code-brackets: AutoMLJobSecondaryStatusType](./literals.md#automljobsecondarystatustype) 
9. See [:material-code-braces: ModelDeployConfigTypeDef](./type_defs.md#modeldeployconfigtypedef) 
10. See [:material-code-braces: ModelDeployResultTypeDef](./type_defs.md#modeldeployresulttypedef) 
11. See [:material-code-braces: AutoMLDataSplitConfigTypeDef](./type_defs.md#automldatasplitconfigtypedef) 
12. See [:material-code-braces: AutoMLSecurityConfigTypeDef](./type_defs.md#automlsecurityconfigtypedef) 
13. See [:material-code-braces: AutoMLJobArtifactsTypeDef](./type_defs.md#automljobartifactstypedef) 
14. See [:material-code-braces: AutoMLResolvedAttributesTypeDef](./type_defs.md#automlresolvedattributestypedef) 
15. See [:material-code-brackets: AutoMLProblemTypeConfigNameType](./literals.md#automlproblemtypeconfignametype) 
16. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPipelineExecutionStepsResponseTypeDef

```python
# ListPipelineExecutionStepsResponseTypeDef definition

class ListPipelineExecutionStepsResponseTypeDef(TypedDict):
    PipelineExecutionSteps: List[PipelineExecutionStepTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PipelineExecutionStepTypeDef](./type_defs.md#pipelineexecutionsteptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEndpointInputRequestTypeDef

```python
# CreateEndpointInputRequestTypeDef definition

class CreateEndpointInputRequestTypeDef(TypedDict):
    EndpointName: str,
    EndpointConfigName: str,
    DeploymentConfig: NotRequired[DeploymentConfigTypeDef],  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: DeploymentConfigTypeDef](./type_defs.md#deploymentconfigtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateEndpointInputRequestTypeDef

```python
# UpdateEndpointInputRequestTypeDef definition

class UpdateEndpointInputRequestTypeDef(TypedDict):
    EndpointName: str,
    EndpointConfigName: str,
    RetainAllVariantProperties: NotRequired[bool],
    ExcludeRetainedVariantProperties: NotRequired[Sequence[VariantPropertyTypeDef]],  # (1)
    DeploymentConfig: NotRequired[DeploymentConfigTypeDef],  # (2)
    RetainDeploymentConfig: NotRequired[bool],
```

1. See [:material-code-braces: VariantPropertyTypeDef](./type_defs.md#variantpropertytypedef) 
2. See [:material-code-braces: DeploymentConfigTypeDef](./type_defs.md#deploymentconfigtypedef) 
## CreateInferenceRecommendationsJobRequestRequestTypeDef

```python
# CreateInferenceRecommendationsJobRequestRequestTypeDef definition

class CreateInferenceRecommendationsJobRequestRequestTypeDef(TypedDict):
    JobName: str,
    JobType: RecommendationJobTypeType,  # (1)
    RoleArn: str,
    InputConfig: RecommendationJobInputConfigTypeDef,  # (2)
    JobDescription: NotRequired[str],
    StoppingConditions: NotRequired[RecommendationJobStoppingConditionsTypeDef],  # (3)
    OutputConfig: NotRequired[RecommendationJobOutputConfigTypeDef],  # (4)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (5)
```

1. See [:material-code-brackets: RecommendationJobTypeType](./literals.md#recommendationjobtypetype) 
2. See [:material-code-braces: RecommendationJobInputConfigTypeDef](./type_defs.md#recommendationjobinputconfigtypedef) 
3. See [:material-code-braces: RecommendationJobStoppingConditionsTypeDef](./type_defs.md#recommendationjobstoppingconditionstypedef) 
4. See [:material-code-braces: RecommendationJobOutputConfigTypeDef](./type_defs.md#recommendationjoboutputconfigtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeInferenceRecommendationsJobResponseTypeDef

```python
# DescribeInferenceRecommendationsJobResponseTypeDef definition

class DescribeInferenceRecommendationsJobResponseTypeDef(TypedDict):
    JobName: str,
    JobDescription: str,
    JobType: RecommendationJobTypeType,  # (1)
    JobArn: str,
    RoleArn: str,
    Status: RecommendationJobStatusType,  # (2)
    CreationTime: datetime,
    CompletionTime: datetime,
    LastModifiedTime: datetime,
    FailureReason: str,
    InputConfig: RecommendationJobInputConfigTypeDef,  # (3)
    StoppingConditions: RecommendationJobStoppingConditionsTypeDef,  # (4)
    InferenceRecommendations: List[InferenceRecommendationTypeDef],  # (5)
    EndpointPerformances: List[EndpointPerformanceTypeDef],  # (6)
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-brackets: RecommendationJobTypeType](./literals.md#recommendationjobtypetype) 
2. See [:material-code-brackets: RecommendationJobStatusType](./literals.md#recommendationjobstatustype) 
3. See [:material-code-braces: RecommendationJobInputConfigTypeDef](./type_defs.md#recommendationjobinputconfigtypedef) 
4. See [:material-code-braces: RecommendationJobStoppingConditionsTypeDef](./type_defs.md#recommendationjobstoppingconditionstypedef) 
5. See [:material-code-braces: InferenceRecommendationTypeDef](./type_defs.md#inferencerecommendationtypedef) 
6. See [:material-code-braces: EndpointPerformanceTypeDef](./type_defs.md#endpointperformancetypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEndpointConfigInputRequestTypeDef

```python
# CreateEndpointConfigInputRequestTypeDef definition

class CreateEndpointConfigInputRequestTypeDef(TypedDict):
    EndpointConfigName: str,
    ProductionVariants: Sequence[ProductionVariantTypeDef],  # (1)
    DataCaptureConfig: NotRequired[DataCaptureConfigTypeDef],  # (2)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
    KmsKeyId: NotRequired[str],
    AsyncInferenceConfig: NotRequired[AsyncInferenceConfigTypeDef],  # (4)
    ExplainerConfig: NotRequired[ExplainerConfigTypeDef],  # (5)
    ShadowProductionVariants: NotRequired[Sequence[ProductionVariantTypeDef]],  # (1)
```

1. See [:material-code-braces: ProductionVariantTypeDef](./type_defs.md#productionvarianttypedef) 
2. See [:material-code-braces: DataCaptureConfigTypeDef](./type_defs.md#datacaptureconfigtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: AsyncInferenceConfigTypeDef](./type_defs.md#asyncinferenceconfigtypedef) 
5. See [:material-code-braces: ExplainerConfigTypeDef](./type_defs.md#explainerconfigtypedef) 
6. See [:material-code-braces: ProductionVariantTypeDef](./type_defs.md#productionvarianttypedef) 
## DescribeEndpointConfigOutputTypeDef

```python
# DescribeEndpointConfigOutputTypeDef definition

class DescribeEndpointConfigOutputTypeDef(TypedDict):
    EndpointConfigName: str,
    EndpointConfigArn: str,
    ProductionVariants: List[ProductionVariantTypeDef],  # (1)
    DataCaptureConfig: DataCaptureConfigTypeDef,  # (2)
    KmsKeyId: str,
    CreationTime: datetime,
    AsyncInferenceConfig: AsyncInferenceConfigTypeDef,  # (3)
    ExplainerConfig: ExplainerConfigTypeDef,  # (4)
    ShadowProductionVariants: List[ProductionVariantTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: ProductionVariantTypeDef](./type_defs.md#productionvarianttypedef) 
2. See [:material-code-braces: DataCaptureConfigTypeDef](./type_defs.md#datacaptureconfigtypedef) 
3. See [:material-code-braces: AsyncInferenceConfigTypeDef](./type_defs.md#asyncinferenceconfigtypedef) 
4. See [:material-code-braces: ExplainerConfigTypeDef](./type_defs.md#explainerconfigtypedef) 
5. See [:material-code-braces: ProductionVariantTypeDef](./type_defs.md#productionvarianttypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEndpointOutputTypeDef

```python
# DescribeEndpointOutputTypeDef definition

class DescribeEndpointOutputTypeDef(TypedDict):
    EndpointName: str,
    EndpointArn: str,
    EndpointConfigName: str,
    ProductionVariants: List[ProductionVariantSummaryTypeDef],  # (1)
    DataCaptureConfig: DataCaptureConfigSummaryTypeDef,  # (2)
    EndpointStatus: EndpointStatusType,  # (3)
    FailureReason: str,
    CreationTime: datetime,
    LastModifiedTime: datetime,
    LastDeploymentConfig: DeploymentConfigTypeDef,  # (4)
    AsyncInferenceConfig: AsyncInferenceConfigTypeDef,  # (5)
    PendingDeploymentSummary: PendingDeploymentSummaryTypeDef,  # (6)
    ExplainerConfig: ExplainerConfigTypeDef,  # (7)
    ShadowProductionVariants: List[ProductionVariantSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (9)
```

1. See [:material-code-braces: ProductionVariantSummaryTypeDef](./type_defs.md#productionvariantsummarytypedef) 
2. See [:material-code-braces: DataCaptureConfigSummaryTypeDef](./type_defs.md#datacaptureconfigsummarytypedef) 
3. See [:material-code-brackets: EndpointStatusType](./literals.md#endpointstatustype) 
4. See [:material-code-braces: DeploymentConfigTypeDef](./type_defs.md#deploymentconfigtypedef) 
5. See [:material-code-braces: AsyncInferenceConfigTypeDef](./type_defs.md#asyncinferenceconfigtypedef) 
6. See [:material-code-braces: PendingDeploymentSummaryTypeDef](./type_defs.md#pendingdeploymentsummarytypedef) 
7. See [:material-code-braces: ExplainerConfigTypeDef](./type_defs.md#explainerconfigtypedef) 
8. See [:material-code-braces: ProductionVariantSummaryTypeDef](./type_defs.md#productionvariantsummarytypedef) 
9. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateHyperParameterTuningJobRequestRequestTypeDef

```python
# CreateHyperParameterTuningJobRequestRequestTypeDef definition

class CreateHyperParameterTuningJobRequestRequestTypeDef(TypedDict):
    HyperParameterTuningJobName: str,
    HyperParameterTuningJobConfig: HyperParameterTuningJobConfigTypeDef,  # (1)
    TrainingJobDefinition: NotRequired[HyperParameterTrainingJobDefinitionTypeDef],  # (2)
    TrainingJobDefinitions: NotRequired[Sequence[HyperParameterTrainingJobDefinitionTypeDef]],  # (3)
    WarmStartConfig: NotRequired[HyperParameterTuningJobWarmStartConfigTypeDef],  # (4)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (5)
    Autotune: NotRequired[AutotuneTypeDef],  # (6)
```

1. See [:material-code-braces: HyperParameterTuningJobConfigTypeDef](./type_defs.md#hyperparametertuningjobconfigtypedef) 
2. See [:material-code-braces: HyperParameterTrainingJobDefinitionTypeDef](./type_defs.md#hyperparametertrainingjobdefinitiontypedef) 
3. See [:material-code-braces: HyperParameterTrainingJobDefinitionTypeDef](./type_defs.md#hyperparametertrainingjobdefinitiontypedef) 
4. See [:material-code-braces: HyperParameterTuningJobWarmStartConfigTypeDef](./type_defs.md#hyperparametertuningjobwarmstartconfigtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: AutotuneTypeDef](./type_defs.md#autotunetypedef) 
## DescribeHyperParameterTuningJobResponseTypeDef

```python
# DescribeHyperParameterTuningJobResponseTypeDef definition

class DescribeHyperParameterTuningJobResponseTypeDef(TypedDict):
    HyperParameterTuningJobName: str,
    HyperParameterTuningJobArn: str,
    HyperParameterTuningJobConfig: HyperParameterTuningJobConfigTypeDef,  # (1)
    TrainingJobDefinition: HyperParameterTrainingJobDefinitionTypeDef,  # (2)
    TrainingJobDefinitions: List[HyperParameterTrainingJobDefinitionTypeDef],  # (3)
    HyperParameterTuningJobStatus: HyperParameterTuningJobStatusType,  # (4)
    CreationTime: datetime,
    HyperParameterTuningEndTime: datetime,
    LastModifiedTime: datetime,
    TrainingJobStatusCounters: TrainingJobStatusCountersTypeDef,  # (5)
    ObjectiveStatusCounters: ObjectiveStatusCountersTypeDef,  # (6)
    BestTrainingJob: HyperParameterTrainingJobSummaryTypeDef,  # (7)
    OverallBestTrainingJob: HyperParameterTrainingJobSummaryTypeDef,  # (7)
    WarmStartConfig: HyperParameterTuningJobWarmStartConfigTypeDef,  # (9)
    FailureReason: str,
    TuningJobCompletionDetails: HyperParameterTuningJobCompletionDetailsTypeDef,  # (10)
    ConsumedResources: HyperParameterTuningJobConsumedResourcesTypeDef,  # (11)
    Autotune: AutotuneTypeDef,  # (12)
    ResponseMetadata: ResponseMetadataTypeDef,  # (13)
```

1. See [:material-code-braces: HyperParameterTuningJobConfigTypeDef](./type_defs.md#hyperparametertuningjobconfigtypedef) 
2. See [:material-code-braces: HyperParameterTrainingJobDefinitionTypeDef](./type_defs.md#hyperparametertrainingjobdefinitiontypedef) 
3. See [:material-code-braces: HyperParameterTrainingJobDefinitionTypeDef](./type_defs.md#hyperparametertrainingjobdefinitiontypedef) 
4. See [:material-code-brackets: HyperParameterTuningJobStatusType](./literals.md#hyperparametertuningjobstatustype) 
5. See [:material-code-braces: TrainingJobStatusCountersTypeDef](./type_defs.md#trainingjobstatuscounterstypedef) 
6. See [:material-code-braces: ObjectiveStatusCountersTypeDef](./type_defs.md#objectivestatuscounterstypedef) 
7. See [:material-code-braces: HyperParameterTrainingJobSummaryTypeDef](./type_defs.md#hyperparametertrainingjobsummarytypedef) 
8. See [:material-code-braces: HyperParameterTrainingJobSummaryTypeDef](./type_defs.md#hyperparametertrainingjobsummarytypedef) 
9. See [:material-code-braces: HyperParameterTuningJobWarmStartConfigTypeDef](./type_defs.md#hyperparametertuningjobwarmstartconfigtypedef) 
10. See [:material-code-braces: HyperParameterTuningJobCompletionDetailsTypeDef](./type_defs.md#hyperparametertuningjobcompletiondetailstypedef) 
11. See [:material-code-braces: HyperParameterTuningJobConsumedResourcesTypeDef](./type_defs.md#hyperparametertuningjobconsumedresourcestypedef) 
12. See [:material-code-braces: AutotuneTypeDef](./type_defs.md#autotunetypedef) 
13. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HyperParameterTuningJobSearchEntityTypeDef

```python
# HyperParameterTuningJobSearchEntityTypeDef definition

class HyperParameterTuningJobSearchEntityTypeDef(TypedDict):
    HyperParameterTuningJobName: NotRequired[str],
    HyperParameterTuningJobArn: NotRequired[str],
    HyperParameterTuningJobConfig: NotRequired[HyperParameterTuningJobConfigTypeDef],  # (1)
    TrainingJobDefinition: NotRequired[HyperParameterTrainingJobDefinitionTypeDef],  # (2)
    TrainingJobDefinitions: NotRequired[List[HyperParameterTrainingJobDefinitionTypeDef]],  # (3)
    HyperParameterTuningJobStatus: NotRequired[HyperParameterTuningJobStatusType],  # (4)
    CreationTime: NotRequired[datetime],
    HyperParameterTuningEndTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
    TrainingJobStatusCounters: NotRequired[TrainingJobStatusCountersTypeDef],  # (5)
    ObjectiveStatusCounters: NotRequired[ObjectiveStatusCountersTypeDef],  # (6)
    BestTrainingJob: NotRequired[HyperParameterTrainingJobSummaryTypeDef],  # (7)
    OverallBestTrainingJob: NotRequired[HyperParameterTrainingJobSummaryTypeDef],  # (7)
    WarmStartConfig: NotRequired[HyperParameterTuningJobWarmStartConfigTypeDef],  # (9)
    FailureReason: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (10)
    TuningJobCompletionDetails: NotRequired[HyperParameterTuningJobCompletionDetailsTypeDef],  # (11)
    ConsumedResources: NotRequired[HyperParameterTuningJobConsumedResourcesTypeDef],  # (12)
```

1. See [:material-code-braces: HyperParameterTuningJobConfigTypeDef](./type_defs.md#hyperparametertuningjobconfigtypedef) 
2. See [:material-code-braces: HyperParameterTrainingJobDefinitionTypeDef](./type_defs.md#hyperparametertrainingjobdefinitiontypedef) 
3. See [:material-code-braces: HyperParameterTrainingJobDefinitionTypeDef](./type_defs.md#hyperparametertrainingjobdefinitiontypedef) 
4. See [:material-code-brackets: HyperParameterTuningJobStatusType](./literals.md#hyperparametertuningjobstatustype) 
5. See [:material-code-braces: TrainingJobStatusCountersTypeDef](./type_defs.md#trainingjobstatuscounterstypedef) 
6. See [:material-code-braces: ObjectiveStatusCountersTypeDef](./type_defs.md#objectivestatuscounterstypedef) 
7. See [:material-code-braces: HyperParameterTrainingJobSummaryTypeDef](./type_defs.md#hyperparametertrainingjobsummarytypedef) 
8. See [:material-code-braces: HyperParameterTrainingJobSummaryTypeDef](./type_defs.md#hyperparametertrainingjobsummarytypedef) 
9. See [:material-code-braces: HyperParameterTuningJobWarmStartConfigTypeDef](./type_defs.md#hyperparametertuningjobwarmstartconfigtypedef) 
10. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
11. See [:material-code-braces: HyperParameterTuningJobCompletionDetailsTypeDef](./type_defs.md#hyperparametertuningjobcompletiondetailstypedef) 
12. See [:material-code-braces: HyperParameterTuningJobConsumedResourcesTypeDef](./type_defs.md#hyperparametertuningjobconsumedresourcestypedef) 
## ListInferenceRecommendationsJobStepsResponseTypeDef

```python
# ListInferenceRecommendationsJobStepsResponseTypeDef definition

class ListInferenceRecommendationsJobStepsResponseTypeDef(TypedDict):
    Steps: List[InferenceRecommendationsJobStepTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InferenceRecommendationsJobStepTypeDef](./type_defs.md#inferencerecommendationsjobsteptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLabelingJobsResponseTypeDef

```python
# ListLabelingJobsResponseTypeDef definition

class ListLabelingJobsResponseTypeDef(TypedDict):
    LabelingJobSummaryList: List[LabelingJobSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LabelingJobSummaryTypeDef](./type_defs.md#labelingjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DynamicScalingConfigurationTypeDef

```python
# DynamicScalingConfigurationTypeDef definition

class DynamicScalingConfigurationTypeDef(TypedDict):
    MinCapacity: NotRequired[int],
    MaxCapacity: NotRequired[int],
    ScaleInCooldown: NotRequired[int],
    ScaleOutCooldown: NotRequired[int],
    ScalingPolicies: NotRequired[List[ScalingPolicyTypeDef]],  # (1)
```

1. See [:material-code-braces: ScalingPolicyTypeDef](./type_defs.md#scalingpolicytypedef) 
## BatchDescribeModelPackageOutputTypeDef

```python
# BatchDescribeModelPackageOutputTypeDef definition

class BatchDescribeModelPackageOutputTypeDef(TypedDict):
    ModelPackageSummaries: Dict[str, BatchDescribeModelPackageSummaryTypeDef],  # (1)
    BatchDescribeModelPackageErrorMap: Dict[str, BatchDescribeModelPackageErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchDescribeModelPackageSummaryTypeDef](./type_defs.md#batchdescribemodelpackagesummarytypedef) 
2. See [:material-code-braces: BatchDescribeModelPackageErrorTypeDef](./type_defs.md#batchdescribemodelpackageerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDataQualityJobDefinitionRequestRequestTypeDef

```python
# CreateDataQualityJobDefinitionRequestRequestTypeDef definition

class CreateDataQualityJobDefinitionRequestRequestTypeDef(TypedDict):
    JobDefinitionName: str,
    DataQualityAppSpecification: DataQualityAppSpecificationTypeDef,  # (1)
    DataQualityJobInput: DataQualityJobInputTypeDef,  # (2)
    DataQualityJobOutputConfig: MonitoringOutputConfigTypeDef,  # (3)
    JobResources: MonitoringResourcesTypeDef,  # (4)
    RoleArn: str,
    DataQualityBaselineConfig: NotRequired[DataQualityBaselineConfigTypeDef],  # (5)
    NetworkConfig: NotRequired[MonitoringNetworkConfigTypeDef],  # (6)
    StoppingCondition: NotRequired[MonitoringStoppingConditionTypeDef],  # (7)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (8)
```

1. See [:material-code-braces: DataQualityAppSpecificationTypeDef](./type_defs.md#dataqualityappspecificationtypedef) 
2. See [:material-code-braces: DataQualityJobInputTypeDef](./type_defs.md#dataqualityjobinputtypedef) 
3. See [:material-code-braces: MonitoringOutputConfigTypeDef](./type_defs.md#monitoringoutputconfigtypedef) 
4. See [:material-code-braces: MonitoringResourcesTypeDef](./type_defs.md#monitoringresourcestypedef) 
5. See [:material-code-braces: DataQualityBaselineConfigTypeDef](./type_defs.md#dataqualitybaselineconfigtypedef) 
6. See [:material-code-braces: MonitoringNetworkConfigTypeDef](./type_defs.md#monitoringnetworkconfigtypedef) 
7. See [:material-code-braces: MonitoringStoppingConditionTypeDef](./type_defs.md#monitoringstoppingconditiontypedef) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeDataQualityJobDefinitionResponseTypeDef

```python
# DescribeDataQualityJobDefinitionResponseTypeDef definition

class DescribeDataQualityJobDefinitionResponseTypeDef(TypedDict):
    JobDefinitionArn: str,
    JobDefinitionName: str,
    CreationTime: datetime,
    DataQualityBaselineConfig: DataQualityBaselineConfigTypeDef,  # (1)
    DataQualityAppSpecification: DataQualityAppSpecificationTypeDef,  # (2)
    DataQualityJobInput: DataQualityJobInputTypeDef,  # (3)
    DataQualityJobOutputConfig: MonitoringOutputConfigTypeDef,  # (4)
    JobResources: MonitoringResourcesTypeDef,  # (5)
    NetworkConfig: MonitoringNetworkConfigTypeDef,  # (6)
    RoleArn: str,
    StoppingCondition: MonitoringStoppingConditionTypeDef,  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-braces: DataQualityBaselineConfigTypeDef](./type_defs.md#dataqualitybaselineconfigtypedef) 
2. See [:material-code-braces: DataQualityAppSpecificationTypeDef](./type_defs.md#dataqualityappspecificationtypedef) 
3. See [:material-code-braces: DataQualityJobInputTypeDef](./type_defs.md#dataqualityjobinputtypedef) 
4. See [:material-code-braces: MonitoringOutputConfigTypeDef](./type_defs.md#monitoringoutputconfigtypedef) 
5. See [:material-code-braces: MonitoringResourcesTypeDef](./type_defs.md#monitoringresourcestypedef) 
6. See [:material-code-braces: MonitoringNetworkConfigTypeDef](./type_defs.md#monitoringnetworkconfigtypedef) 
7. See [:material-code-braces: MonitoringStoppingConditionTypeDef](./type_defs.md#monitoringstoppingconditiontypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateModelBiasJobDefinitionRequestRequestTypeDef

```python
# CreateModelBiasJobDefinitionRequestRequestTypeDef definition

class CreateModelBiasJobDefinitionRequestRequestTypeDef(TypedDict):
    JobDefinitionName: str,
    ModelBiasAppSpecification: ModelBiasAppSpecificationTypeDef,  # (1)
    ModelBiasJobInput: ModelBiasJobInputTypeDef,  # (2)
    ModelBiasJobOutputConfig: MonitoringOutputConfigTypeDef,  # (3)
    JobResources: MonitoringResourcesTypeDef,  # (4)
    RoleArn: str,
    ModelBiasBaselineConfig: NotRequired[ModelBiasBaselineConfigTypeDef],  # (5)
    NetworkConfig: NotRequired[MonitoringNetworkConfigTypeDef],  # (6)
    StoppingCondition: NotRequired[MonitoringStoppingConditionTypeDef],  # (7)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (8)
```

1. See [:material-code-braces: ModelBiasAppSpecificationTypeDef](./type_defs.md#modelbiasappspecificationtypedef) 
2. See [:material-code-braces: ModelBiasJobInputTypeDef](./type_defs.md#modelbiasjobinputtypedef) 
3. See [:material-code-braces: MonitoringOutputConfigTypeDef](./type_defs.md#monitoringoutputconfigtypedef) 
4. See [:material-code-braces: MonitoringResourcesTypeDef](./type_defs.md#monitoringresourcestypedef) 
5. See [:material-code-braces: ModelBiasBaselineConfigTypeDef](./type_defs.md#modelbiasbaselineconfigtypedef) 
6. See [:material-code-braces: MonitoringNetworkConfigTypeDef](./type_defs.md#monitoringnetworkconfigtypedef) 
7. See [:material-code-braces: MonitoringStoppingConditionTypeDef](./type_defs.md#monitoringstoppingconditiontypedef) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeModelBiasJobDefinitionResponseTypeDef

```python
# DescribeModelBiasJobDefinitionResponseTypeDef definition

class DescribeModelBiasJobDefinitionResponseTypeDef(TypedDict):
    JobDefinitionArn: str,
    JobDefinitionName: str,
    CreationTime: datetime,
    ModelBiasBaselineConfig: ModelBiasBaselineConfigTypeDef,  # (1)
    ModelBiasAppSpecification: ModelBiasAppSpecificationTypeDef,  # (2)
    ModelBiasJobInput: ModelBiasJobInputTypeDef,  # (3)
    ModelBiasJobOutputConfig: MonitoringOutputConfigTypeDef,  # (4)
    JobResources: MonitoringResourcesTypeDef,  # (5)
    NetworkConfig: MonitoringNetworkConfigTypeDef,  # (6)
    RoleArn: str,
    StoppingCondition: MonitoringStoppingConditionTypeDef,  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-braces: ModelBiasBaselineConfigTypeDef](./type_defs.md#modelbiasbaselineconfigtypedef) 
2. See [:material-code-braces: ModelBiasAppSpecificationTypeDef](./type_defs.md#modelbiasappspecificationtypedef) 
3. See [:material-code-braces: ModelBiasJobInputTypeDef](./type_defs.md#modelbiasjobinputtypedef) 
4. See [:material-code-braces: MonitoringOutputConfigTypeDef](./type_defs.md#monitoringoutputconfigtypedef) 
5. See [:material-code-braces: MonitoringResourcesTypeDef](./type_defs.md#monitoringresourcestypedef) 
6. See [:material-code-braces: MonitoringNetworkConfigTypeDef](./type_defs.md#monitoringnetworkconfigtypedef) 
7. See [:material-code-braces: MonitoringStoppingConditionTypeDef](./type_defs.md#monitoringstoppingconditiontypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateModelExplainabilityJobDefinitionRequestRequestTypeDef

```python
# CreateModelExplainabilityJobDefinitionRequestRequestTypeDef definition

class CreateModelExplainabilityJobDefinitionRequestRequestTypeDef(TypedDict):
    JobDefinitionName: str,
    ModelExplainabilityAppSpecification: ModelExplainabilityAppSpecificationTypeDef,  # (1)
    ModelExplainabilityJobInput: ModelExplainabilityJobInputTypeDef,  # (2)
    ModelExplainabilityJobOutputConfig: MonitoringOutputConfigTypeDef,  # (3)
    JobResources: MonitoringResourcesTypeDef,  # (4)
    RoleArn: str,
    ModelExplainabilityBaselineConfig: NotRequired[ModelExplainabilityBaselineConfigTypeDef],  # (5)
    NetworkConfig: NotRequired[MonitoringNetworkConfigTypeDef],  # (6)
    StoppingCondition: NotRequired[MonitoringStoppingConditionTypeDef],  # (7)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (8)
```

1. See [:material-code-braces: ModelExplainabilityAppSpecificationTypeDef](./type_defs.md#modelexplainabilityappspecificationtypedef) 
2. See [:material-code-braces: ModelExplainabilityJobInputTypeDef](./type_defs.md#modelexplainabilityjobinputtypedef) 
3. See [:material-code-braces: MonitoringOutputConfigTypeDef](./type_defs.md#monitoringoutputconfigtypedef) 
4. See [:material-code-braces: MonitoringResourcesTypeDef](./type_defs.md#monitoringresourcestypedef) 
5. See [:material-code-braces: ModelExplainabilityBaselineConfigTypeDef](./type_defs.md#modelexplainabilitybaselineconfigtypedef) 
6. See [:material-code-braces: MonitoringNetworkConfigTypeDef](./type_defs.md#monitoringnetworkconfigtypedef) 
7. See [:material-code-braces: MonitoringStoppingConditionTypeDef](./type_defs.md#monitoringstoppingconditiontypedef) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeModelExplainabilityJobDefinitionResponseTypeDef

```python
# DescribeModelExplainabilityJobDefinitionResponseTypeDef definition

class DescribeModelExplainabilityJobDefinitionResponseTypeDef(TypedDict):
    JobDefinitionArn: str,
    JobDefinitionName: str,
    CreationTime: datetime,
    ModelExplainabilityBaselineConfig: ModelExplainabilityBaselineConfigTypeDef,  # (1)
    ModelExplainabilityAppSpecification: ModelExplainabilityAppSpecificationTypeDef,  # (2)
    ModelExplainabilityJobInput: ModelExplainabilityJobInputTypeDef,  # (3)
    ModelExplainabilityJobOutputConfig: MonitoringOutputConfigTypeDef,  # (4)
    JobResources: MonitoringResourcesTypeDef,  # (5)
    NetworkConfig: MonitoringNetworkConfigTypeDef,  # (6)
    RoleArn: str,
    StoppingCondition: MonitoringStoppingConditionTypeDef,  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-braces: ModelExplainabilityBaselineConfigTypeDef](./type_defs.md#modelexplainabilitybaselineconfigtypedef) 
2. See [:material-code-braces: ModelExplainabilityAppSpecificationTypeDef](./type_defs.md#modelexplainabilityappspecificationtypedef) 
3. See [:material-code-braces: ModelExplainabilityJobInputTypeDef](./type_defs.md#modelexplainabilityjobinputtypedef) 
4. See [:material-code-braces: MonitoringOutputConfigTypeDef](./type_defs.md#monitoringoutputconfigtypedef) 
5. See [:material-code-braces: MonitoringResourcesTypeDef](./type_defs.md#monitoringresourcestypedef) 
6. See [:material-code-braces: MonitoringNetworkConfigTypeDef](./type_defs.md#monitoringnetworkconfigtypedef) 
7. See [:material-code-braces: MonitoringStoppingConditionTypeDef](./type_defs.md#monitoringstoppingconditiontypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateModelQualityJobDefinitionRequestRequestTypeDef

```python
# CreateModelQualityJobDefinitionRequestRequestTypeDef definition

class CreateModelQualityJobDefinitionRequestRequestTypeDef(TypedDict):
    JobDefinitionName: str,
    ModelQualityAppSpecification: ModelQualityAppSpecificationTypeDef,  # (1)
    ModelQualityJobInput: ModelQualityJobInputTypeDef,  # (2)
    ModelQualityJobOutputConfig: MonitoringOutputConfigTypeDef,  # (3)
    JobResources: MonitoringResourcesTypeDef,  # (4)
    RoleArn: str,
    ModelQualityBaselineConfig: NotRequired[ModelQualityBaselineConfigTypeDef],  # (5)
    NetworkConfig: NotRequired[MonitoringNetworkConfigTypeDef],  # (6)
    StoppingCondition: NotRequired[MonitoringStoppingConditionTypeDef],  # (7)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (8)
```

1. See [:material-code-braces: ModelQualityAppSpecificationTypeDef](./type_defs.md#modelqualityappspecificationtypedef) 
2. See [:material-code-braces: ModelQualityJobInputTypeDef](./type_defs.md#modelqualityjobinputtypedef) 
3. See [:material-code-braces: MonitoringOutputConfigTypeDef](./type_defs.md#monitoringoutputconfigtypedef) 
4. See [:material-code-braces: MonitoringResourcesTypeDef](./type_defs.md#monitoringresourcestypedef) 
5. See [:material-code-braces: ModelQualityBaselineConfigTypeDef](./type_defs.md#modelqualitybaselineconfigtypedef) 
6. See [:material-code-braces: MonitoringNetworkConfigTypeDef](./type_defs.md#monitoringnetworkconfigtypedef) 
7. See [:material-code-braces: MonitoringStoppingConditionTypeDef](./type_defs.md#monitoringstoppingconditiontypedef) 
8. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeModelQualityJobDefinitionResponseTypeDef

```python
# DescribeModelQualityJobDefinitionResponseTypeDef definition

class DescribeModelQualityJobDefinitionResponseTypeDef(TypedDict):
    JobDefinitionArn: str,
    JobDefinitionName: str,
    CreationTime: datetime,
    ModelQualityBaselineConfig: ModelQualityBaselineConfigTypeDef,  # (1)
    ModelQualityAppSpecification: ModelQualityAppSpecificationTypeDef,  # (2)
    ModelQualityJobInput: ModelQualityJobInputTypeDef,  # (3)
    ModelQualityJobOutputConfig: MonitoringOutputConfigTypeDef,  # (4)
    JobResources: MonitoringResourcesTypeDef,  # (5)
    NetworkConfig: MonitoringNetworkConfigTypeDef,  # (6)
    RoleArn: str,
    StoppingCondition: MonitoringStoppingConditionTypeDef,  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-braces: ModelQualityBaselineConfigTypeDef](./type_defs.md#modelqualitybaselineconfigtypedef) 
2. See [:material-code-braces: ModelQualityAppSpecificationTypeDef](./type_defs.md#modelqualityappspecificationtypedef) 
3. See [:material-code-braces: ModelQualityJobInputTypeDef](./type_defs.md#modelqualityjobinputtypedef) 
4. See [:material-code-braces: MonitoringOutputConfigTypeDef](./type_defs.md#monitoringoutputconfigtypedef) 
5. See [:material-code-braces: MonitoringResourcesTypeDef](./type_defs.md#monitoringresourcestypedef) 
6. See [:material-code-braces: MonitoringNetworkConfigTypeDef](./type_defs.md#monitoringnetworkconfigtypedef) 
7. See [:material-code-braces: MonitoringStoppingConditionTypeDef](./type_defs.md#monitoringstoppingconditiontypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MonitoringJobDefinitionTypeDef

```python
# MonitoringJobDefinitionTypeDef definition

class MonitoringJobDefinitionTypeDef(TypedDict):
    MonitoringInputs: Sequence[MonitoringInputTypeDef],  # (2)
    MonitoringOutputConfig: MonitoringOutputConfigTypeDef,  # (3)
    MonitoringResources: MonitoringResourcesTypeDef,  # (4)
    MonitoringAppSpecification: MonitoringAppSpecificationTypeDef,  # (5)
    RoleArn: str,
    BaselineConfig: NotRequired[MonitoringBaselineConfigTypeDef],  # (1)
    StoppingCondition: NotRequired[MonitoringStoppingConditionTypeDef],  # (6)
    Environment: NotRequired[Mapping[str, str]],
    NetworkConfig: NotRequired[NetworkConfigTypeDef],  # (7)
```

1. See [:material-code-braces: MonitoringBaselineConfigTypeDef](./type_defs.md#monitoringbaselineconfigtypedef) 
2. See [:material-code-braces: MonitoringInputTypeDef](./type_defs.md#monitoringinputtypedef) 
3. See [:material-code-braces: MonitoringOutputConfigTypeDef](./type_defs.md#monitoringoutputconfigtypedef) 
4. See [:material-code-braces: MonitoringResourcesTypeDef](./type_defs.md#monitoringresourcestypedef) 
5. See [:material-code-braces: MonitoringAppSpecificationTypeDef](./type_defs.md#monitoringappspecificationtypedef) 
6. See [:material-code-braces: MonitoringStoppingConditionTypeDef](./type_defs.md#monitoringstoppingconditiontypedef) 
7. See [:material-code-braces: NetworkConfigTypeDef](./type_defs.md#networkconfigtypedef) 
## AlgorithmValidationProfileTypeDef

```python
# AlgorithmValidationProfileTypeDef definition

class AlgorithmValidationProfileTypeDef(TypedDict):
    ProfileName: str,
    TrainingJobDefinition: TrainingJobDefinitionTypeDef,  # (1)
    TransformJobDefinition: NotRequired[TransformJobDefinitionTypeDef],  # (2)
```

1. See [:material-code-braces: TrainingJobDefinitionTypeDef](./type_defs.md#trainingjobdefinitiontypedef) 
2. See [:material-code-braces: TransformJobDefinitionTypeDef](./type_defs.md#transformjobdefinitiontypedef) 
## ModelPackageValidationProfileTypeDef

```python
# ModelPackageValidationProfileTypeDef definition

class ModelPackageValidationProfileTypeDef(TypedDict):
    ProfileName: str,
    TransformJobDefinition: TransformJobDefinitionTypeDef,  # (1)
```

1. See [:material-code-braces: TransformJobDefinitionTypeDef](./type_defs.md#transformjobdefinitiontypedef) 
## TrialComponentSourceDetailTypeDef

```python
# TrialComponentSourceDetailTypeDef definition

class TrialComponentSourceDetailTypeDef(TypedDict):
    SourceArn: NotRequired[str],
    TrainingJob: NotRequired[TrainingJobTypeDef],  # (1)
    ProcessingJob: NotRequired[ProcessingJobTypeDef],  # (2)
    TransformJob: NotRequired[TransformJobTypeDef],  # (3)
```

1. See [:material-code-braces: TrainingJobTypeDef](./type_defs.md#trainingjobtypedef) 
2. See [:material-code-braces: ProcessingJobTypeDef](./type_defs.md#processingjobtypedef) 
3. See [:material-code-braces: TransformJobTypeDef](./type_defs.md#transformjobtypedef) 
## GetScalingConfigurationRecommendationResponseTypeDef

```python
# GetScalingConfigurationRecommendationResponseTypeDef definition

class GetScalingConfigurationRecommendationResponseTypeDef(TypedDict):
    InferenceRecommendationsJobName: str,
    RecommendationId: str,
    EndpointName: str,
    TargetCpuUtilizationPerCore: int,
    ScalingPolicyObjective: ScalingPolicyObjectiveTypeDef,  # (1)
    Metric: ScalingPolicyMetricTypeDef,  # (2)
    DynamicScalingConfiguration: DynamicScalingConfigurationTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ScalingPolicyObjectiveTypeDef](./type_defs.md#scalingpolicyobjectivetypedef) 
2. See [:material-code-braces: ScalingPolicyMetricTypeDef](./type_defs.md#scalingpolicymetrictypedef) 
3. See [:material-code-braces: DynamicScalingConfigurationTypeDef](./type_defs.md#dynamicscalingconfigurationtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MonitoringScheduleConfigTypeDef

```python
# MonitoringScheduleConfigTypeDef definition

class MonitoringScheduleConfigTypeDef(TypedDict):
    ScheduleConfig: NotRequired[ScheduleConfigTypeDef],  # (1)
    MonitoringJobDefinition: NotRequired[MonitoringJobDefinitionTypeDef],  # (2)
    MonitoringJobDefinitionName: NotRequired[str],
    MonitoringType: NotRequired[MonitoringTypeType],  # (3)
```

1. See [:material-code-braces: ScheduleConfigTypeDef](./type_defs.md#scheduleconfigtypedef) 
2. See [:material-code-braces: MonitoringJobDefinitionTypeDef](./type_defs.md#monitoringjobdefinitiontypedef) 
3. See [:material-code-brackets: MonitoringTypeType](./literals.md#monitoringtypetype) 
## AlgorithmValidationSpecificationTypeDef

```python
# AlgorithmValidationSpecificationTypeDef definition

class AlgorithmValidationSpecificationTypeDef(TypedDict):
    ValidationRole: str,
    ValidationProfiles: Sequence[AlgorithmValidationProfileTypeDef],  # (1)
```

1. See [:material-code-braces: AlgorithmValidationProfileTypeDef](./type_defs.md#algorithmvalidationprofiletypedef) 
## ModelPackageValidationSpecificationTypeDef

```python
# ModelPackageValidationSpecificationTypeDef definition

class ModelPackageValidationSpecificationTypeDef(TypedDict):
    ValidationRole: str,
    ValidationProfiles: Sequence[ModelPackageValidationProfileTypeDef],  # (1)
```

1. See [:material-code-braces: ModelPackageValidationProfileTypeDef](./type_defs.md#modelpackagevalidationprofiletypedef) 
## TrialComponentTypeDef

```python
# TrialComponentTypeDef definition

class TrialComponentTypeDef(TypedDict):
    TrialComponentName: NotRequired[str],
    DisplayName: NotRequired[str],
    TrialComponentArn: NotRequired[str],
    Source: NotRequired[TrialComponentSourceTypeDef],  # (1)
    Status: NotRequired[TrialComponentStatusTypeDef],  # (2)
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    CreationTime: NotRequired[datetime],
    CreatedBy: NotRequired[UserContextTypeDef],  # (3)
    LastModifiedTime: NotRequired[datetime],
    LastModifiedBy: NotRequired[UserContextTypeDef],  # (3)
    Parameters: NotRequired[Dict[str, TrialComponentParameterValueTypeDef]],  # (5)
    InputArtifacts: NotRequired[Dict[str, TrialComponentArtifactTypeDef]],  # (6)
    OutputArtifacts: NotRequired[Dict[str, TrialComponentArtifactTypeDef]],  # (6)
    Metrics: NotRequired[List[TrialComponentMetricSummaryTypeDef]],  # (8)
    MetadataProperties: NotRequired[MetadataPropertiesTypeDef],  # (9)
    SourceDetail: NotRequired[TrialComponentSourceDetailTypeDef],  # (10)
    LineageGroupArn: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (11)
    Parents: NotRequired[List[ParentTypeDef]],  # (12)
    RunName: NotRequired[str],
```

1. See [:material-code-braces: TrialComponentSourceTypeDef](./type_defs.md#trialcomponentsourcetypedef) 
2. See [:material-code-braces: TrialComponentStatusTypeDef](./type_defs.md#trialcomponentstatustypedef) 
3. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
4. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
5. See [:material-code-braces: TrialComponentParameterValueTypeDef](./type_defs.md#trialcomponentparametervaluetypedef) 
6. See [:material-code-braces: TrialComponentArtifactTypeDef](./type_defs.md#trialcomponentartifacttypedef) 
7. See [:material-code-braces: TrialComponentArtifactTypeDef](./type_defs.md#trialcomponentartifacttypedef) 
8. See [:material-code-braces: TrialComponentMetricSummaryTypeDef](./type_defs.md#trialcomponentmetricsummarytypedef) 
9. See [:material-code-braces: MetadataPropertiesTypeDef](./type_defs.md#metadatapropertiestypedef) 
10. See [:material-code-braces: TrialComponentSourceDetailTypeDef](./type_defs.md#trialcomponentsourcedetailtypedef) 
11. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
12. See [:material-code-braces: ParentTypeDef](./type_defs.md#parenttypedef) 
## CreateMonitoringScheduleRequestRequestTypeDef

```python
# CreateMonitoringScheduleRequestRequestTypeDef definition

class CreateMonitoringScheduleRequestRequestTypeDef(TypedDict):
    MonitoringScheduleName: str,
    MonitoringScheduleConfig: MonitoringScheduleConfigTypeDef,  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: MonitoringScheduleConfigTypeDef](./type_defs.md#monitoringscheduleconfigtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeMonitoringScheduleResponseTypeDef

```python
# DescribeMonitoringScheduleResponseTypeDef definition

class DescribeMonitoringScheduleResponseTypeDef(TypedDict):
    MonitoringScheduleArn: str,
    MonitoringScheduleName: str,
    MonitoringScheduleStatus: ScheduleStatusType,  # (1)
    MonitoringType: MonitoringTypeType,  # (2)
    FailureReason: str,
    CreationTime: datetime,
    LastModifiedTime: datetime,
    MonitoringScheduleConfig: MonitoringScheduleConfigTypeDef,  # (3)
    EndpointName: str,
    LastMonitoringExecutionSummary: MonitoringExecutionSummaryTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: ScheduleStatusType](./literals.md#schedulestatustype) 
2. See [:material-code-brackets: MonitoringTypeType](./literals.md#monitoringtypetype) 
3. See [:material-code-braces: MonitoringScheduleConfigTypeDef](./type_defs.md#monitoringscheduleconfigtypedef) 
4. See [:material-code-braces: MonitoringExecutionSummaryTypeDef](./type_defs.md#monitoringexecutionsummarytypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModelDashboardMonitoringScheduleTypeDef

```python
# ModelDashboardMonitoringScheduleTypeDef definition

class ModelDashboardMonitoringScheduleTypeDef(TypedDict):
    MonitoringScheduleArn: NotRequired[str],
    MonitoringScheduleName: NotRequired[str],
    MonitoringScheduleStatus: NotRequired[ScheduleStatusType],  # (1)
    MonitoringType: NotRequired[MonitoringTypeType],  # (2)
    FailureReason: NotRequired[str],
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
    MonitoringScheduleConfig: NotRequired[MonitoringScheduleConfigTypeDef],  # (3)
    EndpointName: NotRequired[str],
    MonitoringAlertSummaries: NotRequired[List[MonitoringAlertSummaryTypeDef]],  # (4)
    LastMonitoringExecutionSummary: NotRequired[MonitoringExecutionSummaryTypeDef],  # (5)
```

1. See [:material-code-brackets: ScheduleStatusType](./literals.md#schedulestatustype) 
2. See [:material-code-brackets: MonitoringTypeType](./literals.md#monitoringtypetype) 
3. See [:material-code-braces: MonitoringScheduleConfigTypeDef](./type_defs.md#monitoringscheduleconfigtypedef) 
4. See [:material-code-braces: MonitoringAlertSummaryTypeDef](./type_defs.md#monitoringalertsummarytypedef) 
5. See [:material-code-braces: MonitoringExecutionSummaryTypeDef](./type_defs.md#monitoringexecutionsummarytypedef) 
## MonitoringScheduleTypeDef

```python
# MonitoringScheduleTypeDef definition

class MonitoringScheduleTypeDef(TypedDict):
    MonitoringScheduleArn: NotRequired[str],
    MonitoringScheduleName: NotRequired[str],
    MonitoringScheduleStatus: NotRequired[ScheduleStatusType],  # (1)
    MonitoringType: NotRequired[MonitoringTypeType],  # (2)
    FailureReason: NotRequired[str],
    CreationTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
    MonitoringScheduleConfig: NotRequired[MonitoringScheduleConfigTypeDef],  # (3)
    EndpointName: NotRequired[str],
    LastMonitoringExecutionSummary: NotRequired[MonitoringExecutionSummaryTypeDef],  # (4)
    Tags: NotRequired[List[TagTypeDef]],  # (5)
```

1. See [:material-code-brackets: ScheduleStatusType](./literals.md#schedulestatustype) 
2. See [:material-code-brackets: MonitoringTypeType](./literals.md#monitoringtypetype) 
3. See [:material-code-braces: MonitoringScheduleConfigTypeDef](./type_defs.md#monitoringscheduleconfigtypedef) 
4. See [:material-code-braces: MonitoringExecutionSummaryTypeDef](./type_defs.md#monitoringexecutionsummarytypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateMonitoringScheduleRequestRequestTypeDef

```python
# UpdateMonitoringScheduleRequestRequestTypeDef definition

class UpdateMonitoringScheduleRequestRequestTypeDef(TypedDict):
    MonitoringScheduleName: str,
    MonitoringScheduleConfig: MonitoringScheduleConfigTypeDef,  # (1)
```

1. See [:material-code-braces: MonitoringScheduleConfigTypeDef](./type_defs.md#monitoringscheduleconfigtypedef) 
## CreateAlgorithmInputRequestTypeDef

```python
# CreateAlgorithmInputRequestTypeDef definition

class CreateAlgorithmInputRequestTypeDef(TypedDict):
    AlgorithmName: str,
    TrainingSpecification: TrainingSpecificationTypeDef,  # (1)
    AlgorithmDescription: NotRequired[str],
    InferenceSpecification: NotRequired[InferenceSpecificationTypeDef],  # (2)
    ValidationSpecification: NotRequired[AlgorithmValidationSpecificationTypeDef],  # (3)
    CertifyForMarketplace: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
```

1. See [:material-code-braces: TrainingSpecificationTypeDef](./type_defs.md#trainingspecificationtypedef) 
2. See [:material-code-braces: InferenceSpecificationTypeDef](./type_defs.md#inferencespecificationtypedef) 
3. See [:material-code-braces: AlgorithmValidationSpecificationTypeDef](./type_defs.md#algorithmvalidationspecificationtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DescribeAlgorithmOutputTypeDef

```python
# DescribeAlgorithmOutputTypeDef definition

class DescribeAlgorithmOutputTypeDef(TypedDict):
    AlgorithmName: str,
    AlgorithmArn: str,
    AlgorithmDescription: str,
    CreationTime: datetime,
    TrainingSpecification: TrainingSpecificationTypeDef,  # (1)
    InferenceSpecification: InferenceSpecificationTypeDef,  # (2)
    ValidationSpecification: AlgorithmValidationSpecificationTypeDef,  # (3)
    AlgorithmStatus: AlgorithmStatusType,  # (4)
    AlgorithmStatusDetails: AlgorithmStatusDetailsTypeDef,  # (5)
    ProductId: str,
    CertifyForMarketplace: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: TrainingSpecificationTypeDef](./type_defs.md#trainingspecificationtypedef) 
2. See [:material-code-braces: InferenceSpecificationTypeDef](./type_defs.md#inferencespecificationtypedef) 
3. See [:material-code-braces: AlgorithmValidationSpecificationTypeDef](./type_defs.md#algorithmvalidationspecificationtypedef) 
4. See [:material-code-brackets: AlgorithmStatusType](./literals.md#algorithmstatustype) 
5. See [:material-code-braces: AlgorithmStatusDetailsTypeDef](./type_defs.md#algorithmstatusdetailstypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateModelPackageInputRequestTypeDef

```python
# CreateModelPackageInputRequestTypeDef definition

class CreateModelPackageInputRequestTypeDef(TypedDict):
    ModelPackageName: NotRequired[str],
    ModelPackageGroupName: NotRequired[str],
    ModelPackageDescription: NotRequired[str],
    InferenceSpecification: NotRequired[InferenceSpecificationTypeDef],  # (1)
    ValidationSpecification: NotRequired[ModelPackageValidationSpecificationTypeDef],  # (2)
    SourceAlgorithmSpecification: NotRequired[SourceAlgorithmSpecificationTypeDef],  # (3)
    CertifyForMarketplace: NotRequired[bool],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
    ModelApprovalStatus: NotRequired[ModelApprovalStatusType],  # (5)
    MetadataProperties: NotRequired[MetadataPropertiesTypeDef],  # (6)
    ModelMetrics: NotRequired[ModelMetricsTypeDef],  # (7)
    ClientToken: NotRequired[str],
    CustomerMetadataProperties: NotRequired[Mapping[str, str]],
    DriftCheckBaselines: NotRequired[DriftCheckBaselinesTypeDef],  # (8)
    Domain: NotRequired[str],
    Task: NotRequired[str],
    SamplePayloadUrl: NotRequired[str],
    AdditionalInferenceSpecifications: NotRequired[Sequence[AdditionalInferenceSpecificationDefinitionTypeDef]],  # (9)
```

1. See [:material-code-braces: InferenceSpecificationTypeDef](./type_defs.md#inferencespecificationtypedef) 
2. See [:material-code-braces: ModelPackageValidationSpecificationTypeDef](./type_defs.md#modelpackagevalidationspecificationtypedef) 
3. See [:material-code-braces: SourceAlgorithmSpecificationTypeDef](./type_defs.md#sourcealgorithmspecificationtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-brackets: ModelApprovalStatusType](./literals.md#modelapprovalstatustype) 
6. See [:material-code-braces: MetadataPropertiesTypeDef](./type_defs.md#metadatapropertiestypedef) 
7. See [:material-code-braces: ModelMetricsTypeDef](./type_defs.md#modelmetricstypedef) 
8. See [:material-code-braces: DriftCheckBaselinesTypeDef](./type_defs.md#driftcheckbaselinestypedef) 
9. See [:material-code-braces: AdditionalInferenceSpecificationDefinitionTypeDef](./type_defs.md#additionalinferencespecificationdefinitiontypedef) 
## DescribeModelPackageOutputTypeDef

```python
# DescribeModelPackageOutputTypeDef definition

class DescribeModelPackageOutputTypeDef(TypedDict):
    ModelPackageName: str,
    ModelPackageGroupName: str,
    ModelPackageVersion: int,
    ModelPackageArn: str,
    ModelPackageDescription: str,
    CreationTime: datetime,
    InferenceSpecification: InferenceSpecificationTypeDef,  # (1)
    SourceAlgorithmSpecification: SourceAlgorithmSpecificationTypeDef,  # (2)
    ValidationSpecification: ModelPackageValidationSpecificationTypeDef,  # (3)
    ModelPackageStatus: ModelPackageStatusType,  # (4)
    ModelPackageStatusDetails: ModelPackageStatusDetailsTypeDef,  # (5)
    CertifyForMarketplace: bool,
    ModelApprovalStatus: ModelApprovalStatusType,  # (6)
    CreatedBy: UserContextTypeDef,  # (7)
    MetadataProperties: MetadataPropertiesTypeDef,  # (8)
    ModelMetrics: ModelMetricsTypeDef,  # (9)
    LastModifiedTime: datetime,
    LastModifiedBy: UserContextTypeDef,  # (7)
    ApprovalDescription: str,
    CustomerMetadataProperties: Dict[str, str],
    DriftCheckBaselines: DriftCheckBaselinesTypeDef,  # (11)
    Domain: str,
    Task: str,
    SamplePayloadUrl: str,
    AdditionalInferenceSpecifications: List[AdditionalInferenceSpecificationDefinitionTypeDef],  # (12)
    ResponseMetadata: ResponseMetadataTypeDef,  # (13)
```

1. See [:material-code-braces: InferenceSpecificationTypeDef](./type_defs.md#inferencespecificationtypedef) 
2. See [:material-code-braces: SourceAlgorithmSpecificationTypeDef](./type_defs.md#sourcealgorithmspecificationtypedef) 
3. See [:material-code-braces: ModelPackageValidationSpecificationTypeDef](./type_defs.md#modelpackagevalidationspecificationtypedef) 
4. See [:material-code-brackets: ModelPackageStatusType](./literals.md#modelpackagestatustype) 
5. See [:material-code-braces: ModelPackageStatusDetailsTypeDef](./type_defs.md#modelpackagestatusdetailstypedef) 
6. See [:material-code-brackets: ModelApprovalStatusType](./literals.md#modelapprovalstatustype) 
7. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
8. See [:material-code-braces: MetadataPropertiesTypeDef](./type_defs.md#metadatapropertiestypedef) 
9. See [:material-code-braces: ModelMetricsTypeDef](./type_defs.md#modelmetricstypedef) 
10. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
11. See [:material-code-braces: DriftCheckBaselinesTypeDef](./type_defs.md#driftcheckbaselinestypedef) 
12. See [:material-code-braces: AdditionalInferenceSpecificationDefinitionTypeDef](./type_defs.md#additionalinferencespecificationdefinitiontypedef) 
13. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModelPackageTypeDef

```python
# ModelPackageTypeDef definition

class ModelPackageTypeDef(TypedDict):
    ModelPackageName: NotRequired[str],
    ModelPackageGroupName: NotRequired[str],
    ModelPackageVersion: NotRequired[int],
    ModelPackageArn: NotRequired[str],
    ModelPackageDescription: NotRequired[str],
    CreationTime: NotRequired[datetime],
    InferenceSpecification: NotRequired[InferenceSpecificationTypeDef],  # (1)
    SourceAlgorithmSpecification: NotRequired[SourceAlgorithmSpecificationTypeDef],  # (2)
    ValidationSpecification: NotRequired[ModelPackageValidationSpecificationTypeDef],  # (3)
    ModelPackageStatus: NotRequired[ModelPackageStatusType],  # (4)
    ModelPackageStatusDetails: NotRequired[ModelPackageStatusDetailsTypeDef],  # (5)
    CertifyForMarketplace: NotRequired[bool],
    ModelApprovalStatus: NotRequired[ModelApprovalStatusType],  # (6)
    CreatedBy: NotRequired[UserContextTypeDef],  # (7)
    MetadataProperties: NotRequired[MetadataPropertiesTypeDef],  # (8)
    ModelMetrics: NotRequired[ModelMetricsTypeDef],  # (9)
    LastModifiedTime: NotRequired[datetime],
    LastModifiedBy: NotRequired[UserContextTypeDef],  # (7)
    ApprovalDescription: NotRequired[str],
    Domain: NotRequired[str],
    Task: NotRequired[str],
    SamplePayloadUrl: NotRequired[str],
    AdditionalInferenceSpecifications: NotRequired[List[AdditionalInferenceSpecificationDefinitionTypeDef]],  # (11)
    Tags: NotRequired[List[TagTypeDef]],  # (12)
    CustomerMetadataProperties: NotRequired[Dict[str, str]],
    DriftCheckBaselines: NotRequired[DriftCheckBaselinesTypeDef],  # (13)
```

1. See [:material-code-braces: InferenceSpecificationTypeDef](./type_defs.md#inferencespecificationtypedef) 
2. See [:material-code-braces: SourceAlgorithmSpecificationTypeDef](./type_defs.md#sourcealgorithmspecificationtypedef) 
3. See [:material-code-braces: ModelPackageValidationSpecificationTypeDef](./type_defs.md#modelpackagevalidationspecificationtypedef) 
4. See [:material-code-brackets: ModelPackageStatusType](./literals.md#modelpackagestatustype) 
5. See [:material-code-braces: ModelPackageStatusDetailsTypeDef](./type_defs.md#modelpackagestatusdetailstypedef) 
6. See [:material-code-brackets: ModelApprovalStatusType](./literals.md#modelapprovalstatustype) 
7. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
8. See [:material-code-braces: MetadataPropertiesTypeDef](./type_defs.md#metadatapropertiestypedef) 
9. See [:material-code-braces: ModelMetricsTypeDef](./type_defs.md#modelmetricstypedef) 
10. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
11. See [:material-code-braces: AdditionalInferenceSpecificationDefinitionTypeDef](./type_defs.md#additionalinferencespecificationdefinitiontypedef) 
12. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
13. See [:material-code-braces: DriftCheckBaselinesTypeDef](./type_defs.md#driftcheckbaselinestypedef) 
## ModelDashboardModelTypeDef

```python
# ModelDashboardModelTypeDef definition

class ModelDashboardModelTypeDef(TypedDict):
    Model: NotRequired[ModelTypeDef],  # (1)
    Endpoints: NotRequired[List[ModelDashboardEndpointTypeDef]],  # (2)
    LastBatchTransformJob: NotRequired[TransformJobTypeDef],  # (3)
    MonitoringSchedules: NotRequired[List[ModelDashboardMonitoringScheduleTypeDef]],  # (4)
    ModelCard: NotRequired[ModelDashboardModelCardTypeDef],  # (5)
```

1. See [:material-code-braces: ModelTypeDef](./type_defs.md#modeltypedef) 
2. See [:material-code-braces: ModelDashboardEndpointTypeDef](./type_defs.md#modeldashboardendpointtypedef) 
3. See [:material-code-braces: TransformJobTypeDef](./type_defs.md#transformjobtypedef) 
4. See [:material-code-braces: ModelDashboardMonitoringScheduleTypeDef](./type_defs.md#modeldashboardmonitoringscheduletypedef) 
5. See [:material-code-braces: ModelDashboardModelCardTypeDef](./type_defs.md#modeldashboardmodelcardtypedef) 
## EndpointTypeDef

```python
# EndpointTypeDef definition

class EndpointTypeDef(TypedDict):
    EndpointName: str,
    EndpointArn: str,
    EndpointConfigName: str,
    EndpointStatus: EndpointStatusType,  # (3)
    CreationTime: datetime,
    LastModifiedTime: datetime,
    ProductionVariants: NotRequired[List[ProductionVariantSummaryTypeDef]],  # (1)
    DataCaptureConfig: NotRequired[DataCaptureConfigSummaryTypeDef],  # (2)
    FailureReason: NotRequired[str],
    MonitoringSchedules: NotRequired[List[MonitoringScheduleTypeDef]],  # (4)
    Tags: NotRequired[List[TagTypeDef]],  # (5)
    ShadowProductionVariants: NotRequired[List[ProductionVariantSummaryTypeDef]],  # (1)
```

1. See [:material-code-braces: ProductionVariantSummaryTypeDef](./type_defs.md#productionvariantsummarytypedef) 
2. See [:material-code-braces: DataCaptureConfigSummaryTypeDef](./type_defs.md#datacaptureconfigsummarytypedef) 
3. See [:material-code-brackets: EndpointStatusType](./literals.md#endpointstatustype) 
4. See [:material-code-braces: MonitoringScheduleTypeDef](./type_defs.md#monitoringscheduletypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: ProductionVariantSummaryTypeDef](./type_defs.md#productionvariantsummarytypedef) 
## SearchRecordTypeDef

```python
# SearchRecordTypeDef definition

class SearchRecordTypeDef(TypedDict):
    TrainingJob: NotRequired[TrainingJobTypeDef],  # (1)
    Experiment: NotRequired[ExperimentTypeDef],  # (2)
    Trial: NotRequired[TrialTypeDef],  # (3)
    TrialComponent: NotRequired[TrialComponentTypeDef],  # (4)
    Endpoint: NotRequired[EndpointTypeDef],  # (5)
    ModelPackage: NotRequired[ModelPackageTypeDef],  # (6)
    ModelPackageGroup: NotRequired[ModelPackageGroupTypeDef],  # (7)
    Pipeline: NotRequired[PipelineTypeDef],  # (8)
    PipelineExecution: NotRequired[PipelineExecutionTypeDef],  # (9)
    FeatureGroup: NotRequired[FeatureGroupTypeDef],  # (10)
    Project: NotRequired[ProjectTypeDef],  # (11)
    FeatureMetadata: NotRequired[FeatureMetadataTypeDef],  # (12)
    HyperParameterTuningJob: NotRequired[HyperParameterTuningJobSearchEntityTypeDef],  # (13)
    Model: NotRequired[ModelDashboardModelTypeDef],  # (14)
    ModelCard: NotRequired[ModelCardTypeDef],  # (15)
```

1. See [:material-code-braces: TrainingJobTypeDef](./type_defs.md#trainingjobtypedef) 
2. See [:material-code-braces: ExperimentTypeDef](./type_defs.md#experimenttypedef) 
3. See [:material-code-braces: TrialTypeDef](./type_defs.md#trialtypedef) 
4. See [:material-code-braces: TrialComponentTypeDef](./type_defs.md#trialcomponenttypedef) 
5. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
6. See [:material-code-braces: ModelPackageTypeDef](./type_defs.md#modelpackagetypedef) 
7. See [:material-code-braces: ModelPackageGroupTypeDef](./type_defs.md#modelpackagegrouptypedef) 
8. See [:material-code-braces: PipelineTypeDef](./type_defs.md#pipelinetypedef) 
9. See [:material-code-braces: PipelineExecutionTypeDef](./type_defs.md#pipelineexecutiontypedef) 
10. See [:material-code-braces: FeatureGroupTypeDef](./type_defs.md#featuregrouptypedef) 
11. See [:material-code-braces: ProjectTypeDef](./type_defs.md#projecttypedef) 
12. See [:material-code-braces: FeatureMetadataTypeDef](./type_defs.md#featuremetadatatypedef) 
13. See [:material-code-braces: HyperParameterTuningJobSearchEntityTypeDef](./type_defs.md#hyperparametertuningjobsearchentitytypedef) 
14. See [:material-code-braces: ModelDashboardModelTypeDef](./type_defs.md#modeldashboardmodeltypedef) 
15. See [:material-code-braces: ModelCardTypeDef](./type_defs.md#modelcardtypedef) 
## SearchResponseTypeDef

```python
# SearchResponseTypeDef definition

class SearchResponseTypeDef(TypedDict):
    Results: List[SearchRecordTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SearchRecordTypeDef](./type_defs.md#searchrecordtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
