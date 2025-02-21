# Type definitions

> [Index](../README.md) > [CleanRoomsML](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CleanRoomsML](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#cleanroomsml)
    type annotations stubs module [types-aiobotocore-cleanroomsml](https://pypi.org/project/types-aiobotocore-cleanroomsml/).

## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_cleanroomsml.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## AudienceSizeConfigUnionTypeDef

```python
# AudienceSizeConfigUnionTypeDef Union usage example

from types_aiobotocore_cleanroomsml.type_defs import AudienceSizeConfigUnionTypeDef


def get_value() -> AudienceSizeConfigUnionTypeDef:
    return ...


# AudienceSizeConfigUnionTypeDef definition

AudienceSizeConfigUnionTypeDef = Union[
    AudienceSizeConfigTypeDef,  # (1)
    AudienceSizeConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AudienceSizeConfigTypeDef](./type_defs.md#audiencesizeconfigtypedef) 
2. See [:material-code-braces: AudienceSizeConfigOutputTypeDef](./type_defs.md#audiencesizeconfigoutputtypedef) 

## ColumnSchemaUnionTypeDef

```python
# ColumnSchemaUnionTypeDef Union usage example

from types_aiobotocore_cleanroomsml.type_defs import ColumnSchemaUnionTypeDef


def get_value() -> ColumnSchemaUnionTypeDef:
    return ...


# ColumnSchemaUnionTypeDef definition

ColumnSchemaUnionTypeDef = Union[
    ColumnSchemaTypeDef,  # (1)
    ColumnSchemaOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ColumnSchemaTypeDef](./type_defs.md#columnschematypedef) 
2. See [:material-code-braces: ColumnSchemaOutputTypeDef](./type_defs.md#columnschemaoutputtypedef) 

## ContainerConfigUnionTypeDef

```python
# ContainerConfigUnionTypeDef Union usage example

from types_aiobotocore_cleanroomsml.type_defs import ContainerConfigUnionTypeDef


def get_value() -> ContainerConfigUnionTypeDef:
    return ...


# ContainerConfigUnionTypeDef definition

ContainerConfigUnionTypeDef = Union[
    ContainerConfigTypeDef,  # (1)
    ContainerConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ContainerConfigTypeDef](./type_defs.md#containerconfigtypedef) 
2. See [:material-code-braces: ContainerConfigOutputTypeDef](./type_defs.md#containerconfigoutputtypedef) 

## InferenceOutputConfigurationUnionTypeDef

```python
# InferenceOutputConfigurationUnionTypeDef Union usage example

from types_aiobotocore_cleanroomsml.type_defs import InferenceOutputConfigurationUnionTypeDef


def get_value() -> InferenceOutputConfigurationUnionTypeDef:
    return ...


# InferenceOutputConfigurationUnionTypeDef definition

InferenceOutputConfigurationUnionTypeDef = Union[
    InferenceOutputConfigurationTypeDef,  # (1)
    InferenceOutputConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: InferenceOutputConfigurationTypeDef](./type_defs.md#inferenceoutputconfigurationtypedef) 
2. See [:material-code-braces: InferenceOutputConfigurationOutputTypeDef](./type_defs.md#inferenceoutputconfigurationoutputtypedef) 

## TrainedModelExportOutputConfigurationUnionTypeDef

```python
# TrainedModelExportOutputConfigurationUnionTypeDef Union usage example

from types_aiobotocore_cleanroomsml.type_defs import TrainedModelExportOutputConfigurationUnionTypeDef


def get_value() -> TrainedModelExportOutputConfigurationUnionTypeDef:
    return ...


# TrainedModelExportOutputConfigurationUnionTypeDef definition

TrainedModelExportOutputConfigurationUnionTypeDef = Union[
    TrainedModelExportOutputConfigurationTypeDef,  # (1)
    TrainedModelExportOutputConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TrainedModelExportOutputConfigurationTypeDef](./type_defs.md#trainedmodelexportoutputconfigurationtypedef) 
2. See [:material-code-braces: TrainedModelExportOutputConfigurationOutputTypeDef](./type_defs.md#trainedmodelexportoutputconfigurationoutputtypedef) 

## AudienceGenerationJobDataSourceUnionTypeDef

```python
# AudienceGenerationJobDataSourceUnionTypeDef Union usage example

from types_aiobotocore_cleanroomsml.type_defs import AudienceGenerationJobDataSourceUnionTypeDef


def get_value() -> AudienceGenerationJobDataSourceUnionTypeDef:
    return ...


# AudienceGenerationJobDataSourceUnionTypeDef definition

AudienceGenerationJobDataSourceUnionTypeDef = Union[
    AudienceGenerationJobDataSourceTypeDef,  # (1)
    AudienceGenerationJobDataSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AudienceGenerationJobDataSourceTypeDef](./type_defs.md#audiencegenerationjobdatasourcetypedef) 
2. See [:material-code-braces: AudienceGenerationJobDataSourceOutputTypeDef](./type_defs.md#audiencegenerationjobdatasourceoutputtypedef) 

## DatasetInputConfigUnionTypeDef

```python
# DatasetInputConfigUnionTypeDef Union usage example

from types_aiobotocore_cleanroomsml.type_defs import DatasetInputConfigUnionTypeDef


def get_value() -> DatasetInputConfigUnionTypeDef:
    return ...


# DatasetInputConfigUnionTypeDef definition

DatasetInputConfigUnionTypeDef = Union[
    DatasetInputConfigTypeDef,  # (1)
    DatasetInputConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DatasetInputConfigTypeDef](./type_defs.md#datasetinputconfigtypedef) 
2. See [:material-code-braces: DatasetInputConfigOutputTypeDef](./type_defs.md#datasetinputconfigoutputtypedef) 

## PrivacyConfigurationUnionTypeDef

```python
# PrivacyConfigurationUnionTypeDef Union usage example

from types_aiobotocore_cleanroomsml.type_defs import PrivacyConfigurationUnionTypeDef


def get_value() -> PrivacyConfigurationUnionTypeDef:
    return ...


# PrivacyConfigurationUnionTypeDef definition

PrivacyConfigurationUnionTypeDef = Union[
    PrivacyConfigurationTypeDef,  # (1)
    PrivacyConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PrivacyConfigurationTypeDef](./type_defs.md#privacyconfigurationtypedef) 
2. See [:material-code-braces: PrivacyConfigurationOutputTypeDef](./type_defs.md#privacyconfigurationoutputtypedef) 

## InputChannelUnionTypeDef

```python
# InputChannelUnionTypeDef Union usage example

from types_aiobotocore_cleanroomsml.type_defs import InputChannelUnionTypeDef


def get_value() -> InputChannelUnionTypeDef:
    return ...


# InputChannelUnionTypeDef definition

InputChannelUnionTypeDef = Union[
    InputChannelTypeDef,  # (1)
    InputChannelOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: InputChannelTypeDef](./type_defs.md#inputchanneltypedef) 
2. See [:material-code-braces: InputChannelOutputTypeDef](./type_defs.md#inputchanneloutputtypedef) 

## DatasetUnionTypeDef

```python
# DatasetUnionTypeDef Union usage example

from types_aiobotocore_cleanroomsml.type_defs import DatasetUnionTypeDef


def get_value() -> DatasetUnionTypeDef:
    return ...


# DatasetUnionTypeDef definition

DatasetUnionTypeDef = Union[
    DatasetTypeDef,  # (1)
    DatasetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DatasetTypeDef](./type_defs.md#datasettypedef) 
2. See [:material-code-braces: DatasetOutputTypeDef](./type_defs.md#datasetoutputtypedef) 



## S3ConfigMapTypeDef

```python
# S3ConfigMapTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import S3ConfigMapTypeDef


def get_value() -> S3ConfigMapTypeDef:
    return {
        "s3Uri": ...,
    }


# S3ConfigMapTypeDef definition

class S3ConfigMapTypeDef(TypedDict):
    s3Uri: str,
```

## AudienceSizeTypeDef

```python
# AudienceSizeTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import AudienceSizeTypeDef


def get_value() -> AudienceSizeTypeDef:
    return {
        "type": ...,
    }


# AudienceSizeTypeDef definition

class AudienceSizeTypeDef(TypedDict):
    type: AudienceSizeTypeType,  # (1)
    value: int,
```

1. See [:material-code-brackets: AudienceSizeTypeType](./literals.md#audiencesizetypetype) 
## StatusDetailsTypeDef

```python
# StatusDetailsTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import StatusDetailsTypeDef


def get_value() -> StatusDetailsTypeDef:
    return {
        "statusCode": ...,
    }


# StatusDetailsTypeDef definition

class StatusDetailsTypeDef(TypedDict):
    statusCode: NotRequired[str],
    message: NotRequired[str],
```

## ProtectedQuerySQLParametersOutputTypeDef

```python
# ProtectedQuerySQLParametersOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ProtectedQuerySQLParametersOutputTypeDef


def get_value() -> ProtectedQuerySQLParametersOutputTypeDef:
    return {
        "queryString": ...,
    }


# ProtectedQuerySQLParametersOutputTypeDef definition

class ProtectedQuerySQLParametersOutputTypeDef(TypedDict):
    queryString: NotRequired[str],
    analysisTemplateArn: NotRequired[str],
    parameters: NotRequired[Dict[str, str]],
```

## ProtectedQuerySQLParametersTypeDef

```python
# ProtectedQuerySQLParametersTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ProtectedQuerySQLParametersTypeDef


def get_value() -> ProtectedQuerySQLParametersTypeDef:
    return {
        "queryString": ...,
    }


# ProtectedQuerySQLParametersTypeDef definition

class ProtectedQuerySQLParametersTypeDef(TypedDict):
    queryString: NotRequired[str],
    analysisTemplateArn: NotRequired[str],
    parameters: NotRequired[Mapping[str, str]],
```

## AudienceGenerationJobSummaryTypeDef

```python
# AudienceGenerationJobSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import AudienceGenerationJobSummaryTypeDef


def get_value() -> AudienceGenerationJobSummaryTypeDef:
    return {
        "createTime": ...,
    }


# AudienceGenerationJobSummaryTypeDef definition

class AudienceGenerationJobSummaryTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    audienceGenerationJobArn: str,
    name: str,
    status: AudienceGenerationJobStatusType,  # (1)
    configuredAudienceModelArn: str,
    description: NotRequired[str],
    collaborationId: NotRequired[str],
    startedBy: NotRequired[str],
```

1. See [:material-code-brackets: AudienceGenerationJobStatusType](./literals.md#audiencegenerationjobstatustype) 
## AudienceModelSummaryTypeDef

```python
# AudienceModelSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import AudienceModelSummaryTypeDef


def get_value() -> AudienceModelSummaryTypeDef:
    return {
        "createTime": ...,
    }


# AudienceModelSummaryTypeDef definition

class AudienceModelSummaryTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    audienceModelArn: str,
    name: str,
    trainingDatasetArn: str,
    status: AudienceModelStatusType,  # (1)
    description: NotRequired[str],
```

1. See [:material-code-brackets: AudienceModelStatusType](./literals.md#audiencemodelstatustype) 
## AudienceSizeConfigOutputTypeDef

```python
# AudienceSizeConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import AudienceSizeConfigOutputTypeDef


def get_value() -> AudienceSizeConfigOutputTypeDef:
    return {
        "audienceSizeType": ...,
    }


# AudienceSizeConfigOutputTypeDef definition

class AudienceSizeConfigOutputTypeDef(TypedDict):
    audienceSizeType: AudienceSizeTypeType,  # (1)
    audienceSizeBins: List[int],
```

1. See [:material-code-brackets: AudienceSizeTypeType](./literals.md#audiencesizetypetype) 
## AudienceSizeConfigTypeDef

```python
# AudienceSizeConfigTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import AudienceSizeConfigTypeDef


def get_value() -> AudienceSizeConfigTypeDef:
    return {
        "audienceSizeType": ...,
    }


# AudienceSizeConfigTypeDef definition

class AudienceSizeConfigTypeDef(TypedDict):
    audienceSizeType: AudienceSizeTypeType,  # (1)
    audienceSizeBins: Sequence[int],
```

1. See [:material-code-brackets: AudienceSizeTypeType](./literals.md#audiencesizetypetype) 
## CancelTrainedModelInferenceJobRequestTypeDef

```python
# CancelTrainedModelInferenceJobRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import CancelTrainedModelInferenceJobRequestTypeDef


def get_value() -> CancelTrainedModelInferenceJobRequestTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# CancelTrainedModelInferenceJobRequestTypeDef definition

class CancelTrainedModelInferenceJobRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    trainedModelInferenceJobArn: str,
```

## CancelTrainedModelRequestTypeDef

```python
# CancelTrainedModelRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import CancelTrainedModelRequestTypeDef


def get_value() -> CancelTrainedModelRequestTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# CancelTrainedModelRequestTypeDef definition

class CancelTrainedModelRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    trainedModelArn: str,
```

## CollaborationConfiguredModelAlgorithmAssociationSummaryTypeDef

```python
# CollaborationConfiguredModelAlgorithmAssociationSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import CollaborationConfiguredModelAlgorithmAssociationSummaryTypeDef


def get_value() -> CollaborationConfiguredModelAlgorithmAssociationSummaryTypeDef:
    return {
        "createTime": ...,
    }


# CollaborationConfiguredModelAlgorithmAssociationSummaryTypeDef definition

class CollaborationConfiguredModelAlgorithmAssociationSummaryTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    configuredModelAlgorithmAssociationArn: str,
    name: str,
    membershipIdentifier: str,
    collaborationIdentifier: str,
    configuredModelAlgorithmArn: str,
    creatorAccountId: str,
    description: NotRequired[str],
```

## CollaborationMLInputChannelSummaryTypeDef

```python
# CollaborationMLInputChannelSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import CollaborationMLInputChannelSummaryTypeDef


def get_value() -> CollaborationMLInputChannelSummaryTypeDef:
    return {
        "createTime": ...,
    }


# CollaborationMLInputChannelSummaryTypeDef definition

class CollaborationMLInputChannelSummaryTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    membershipIdentifier: str,
    collaborationIdentifier: str,
    name: str,
    configuredModelAlgorithmAssociations: List[str],
    mlInputChannelArn: str,
    status: MLInputChannelStatusType,  # (1)
    creatorAccountId: str,
    description: NotRequired[str],
```

1. See [:material-code-brackets: MLInputChannelStatusType](./literals.md#mlinputchannelstatustype) 
## CollaborationTrainedModelSummaryTypeDef

```python
# CollaborationTrainedModelSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import CollaborationTrainedModelSummaryTypeDef


def get_value() -> CollaborationTrainedModelSummaryTypeDef:
    return {
        "createTime": ...,
    }


# CollaborationTrainedModelSummaryTypeDef definition

class CollaborationTrainedModelSummaryTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    trainedModelArn: str,
    name: str,
    membershipIdentifier: str,
    collaborationIdentifier: str,
    status: TrainedModelStatusType,  # (1)
    configuredModelAlgorithmAssociationArn: str,
    creatorAccountId: str,
    description: NotRequired[str],
```

1. See [:material-code-brackets: TrainedModelStatusType](./literals.md#trainedmodelstatustype) 
## ColumnSchemaOutputTypeDef

```python
# ColumnSchemaOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ColumnSchemaOutputTypeDef


def get_value() -> ColumnSchemaOutputTypeDef:
    return {
        "columnName": ...,
    }


# ColumnSchemaOutputTypeDef definition

class ColumnSchemaOutputTypeDef(TypedDict):
    columnName: str,
    columnTypes: List[ColumnTypeType],  # (1)
```

1. See [:material-code-brackets: ColumnTypeType](./literals.md#columntypetype) 
## ColumnSchemaTypeDef

```python
# ColumnSchemaTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ColumnSchemaTypeDef


def get_value() -> ColumnSchemaTypeDef:
    return {
        "columnName": ...,
    }


# ColumnSchemaTypeDef definition

class ColumnSchemaTypeDef(TypedDict):
    columnName: str,
    columnTypes: Sequence[ColumnTypeType],  # (1)
```

1. See [:material-code-brackets: ColumnTypeType](./literals.md#columntypetype) 
## WorkerComputeConfigurationTypeDef

```python
# WorkerComputeConfigurationTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import WorkerComputeConfigurationTypeDef


def get_value() -> WorkerComputeConfigurationTypeDef:
    return {
        "type": ...,
    }


# WorkerComputeConfigurationTypeDef definition

class WorkerComputeConfigurationTypeDef(TypedDict):
    type: NotRequired[WorkerComputeTypeType],  # (1)
    number: NotRequired[int],
```

1. See [:material-code-brackets: WorkerComputeTypeType](./literals.md#workercomputetypetype) 
## ConfiguredModelAlgorithmAssociationSummaryTypeDef

```python
# ConfiguredModelAlgorithmAssociationSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ConfiguredModelAlgorithmAssociationSummaryTypeDef


def get_value() -> ConfiguredModelAlgorithmAssociationSummaryTypeDef:
    return {
        "createTime": ...,
    }


# ConfiguredModelAlgorithmAssociationSummaryTypeDef definition

class ConfiguredModelAlgorithmAssociationSummaryTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    configuredModelAlgorithmAssociationArn: str,
    configuredModelAlgorithmArn: str,
    name: str,
    membershipIdentifier: str,
    collaborationIdentifier: str,
    description: NotRequired[str],
```

## ConfiguredModelAlgorithmSummaryTypeDef

```python
# ConfiguredModelAlgorithmSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ConfiguredModelAlgorithmSummaryTypeDef


def get_value() -> ConfiguredModelAlgorithmSummaryTypeDef:
    return {
        "createTime": ...,
    }


# ConfiguredModelAlgorithmSummaryTypeDef definition

class ConfiguredModelAlgorithmSummaryTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    configuredModelAlgorithmArn: str,
    name: str,
    description: NotRequired[str],
```

## MetricDefinitionTypeDef

```python
# MetricDefinitionTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import MetricDefinitionTypeDef


def get_value() -> MetricDefinitionTypeDef:
    return {
        "name": ...,
    }


# MetricDefinitionTypeDef definition

class MetricDefinitionTypeDef(TypedDict):
    name: str,
    regex: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ResponseMetadataTypeDef


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

## InferenceContainerConfigTypeDef

```python
# InferenceContainerConfigTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import InferenceContainerConfigTypeDef


def get_value() -> InferenceContainerConfigTypeDef:
    return {
        "imageUri": ...,
    }


# InferenceContainerConfigTypeDef definition

class InferenceContainerConfigTypeDef(TypedDict):
    imageUri: str,
```

## ModelTrainingDataChannelTypeDef

```python
# ModelTrainingDataChannelTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ModelTrainingDataChannelTypeDef


def get_value() -> ModelTrainingDataChannelTypeDef:
    return {
        "mlInputChannelArn": ...,
    }


# ModelTrainingDataChannelTypeDef definition

class ModelTrainingDataChannelTypeDef(TypedDict):
    mlInputChannelArn: str,
    channelName: str,
```

## ResourceConfigTypeDef

```python
# ResourceConfigTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ResourceConfigTypeDef


def get_value() -> ResourceConfigTypeDef:
    return {
        "instanceCount": ...,
    }


# ResourceConfigTypeDef definition

class ResourceConfigTypeDef(TypedDict):
    instanceType: InstanceTypeType,  # (1)
    volumeSizeInGB: int,
    instanceCount: NotRequired[int],
```

1. See [:material-code-brackets: InstanceTypeType](./literals.md#instancetypetype) 
## StoppingConditionTypeDef

```python
# StoppingConditionTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import StoppingConditionTypeDef


def get_value() -> StoppingConditionTypeDef:
    return {
        "maxRuntimeInSeconds": ...,
    }


# StoppingConditionTypeDef definition

class StoppingConditionTypeDef(TypedDict):
    maxRuntimeInSeconds: NotRequired[int],
```

## GlueDataSourceTypeDef

```python
# GlueDataSourceTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import GlueDataSourceTypeDef


def get_value() -> GlueDataSourceTypeDef:
    return {
        "tableName": ...,
    }


# GlueDataSourceTypeDef definition

class GlueDataSourceTypeDef(TypedDict):
    tableName: str,
    databaseName: str,
    catalogId: NotRequired[str],
```

## DeleteAudienceGenerationJobRequestTypeDef

```python
# DeleteAudienceGenerationJobRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import DeleteAudienceGenerationJobRequestTypeDef


def get_value() -> DeleteAudienceGenerationJobRequestTypeDef:
    return {
        "audienceGenerationJobArn": ...,
    }


# DeleteAudienceGenerationJobRequestTypeDef definition

class DeleteAudienceGenerationJobRequestTypeDef(TypedDict):
    audienceGenerationJobArn: str,
```

## DeleteAudienceModelRequestTypeDef

```python
# DeleteAudienceModelRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import DeleteAudienceModelRequestTypeDef


def get_value() -> DeleteAudienceModelRequestTypeDef:
    return {
        "audienceModelArn": ...,
    }


# DeleteAudienceModelRequestTypeDef definition

class DeleteAudienceModelRequestTypeDef(TypedDict):
    audienceModelArn: str,
```

## DeleteConfiguredAudienceModelPolicyRequestTypeDef

```python
# DeleteConfiguredAudienceModelPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import DeleteConfiguredAudienceModelPolicyRequestTypeDef


def get_value() -> DeleteConfiguredAudienceModelPolicyRequestTypeDef:
    return {
        "configuredAudienceModelArn": ...,
    }


# DeleteConfiguredAudienceModelPolicyRequestTypeDef definition

class DeleteConfiguredAudienceModelPolicyRequestTypeDef(TypedDict):
    configuredAudienceModelArn: str,
```

## DeleteConfiguredAudienceModelRequestTypeDef

```python
# DeleteConfiguredAudienceModelRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import DeleteConfiguredAudienceModelRequestTypeDef


def get_value() -> DeleteConfiguredAudienceModelRequestTypeDef:
    return {
        "configuredAudienceModelArn": ...,
    }


# DeleteConfiguredAudienceModelRequestTypeDef definition

class DeleteConfiguredAudienceModelRequestTypeDef(TypedDict):
    configuredAudienceModelArn: str,
```

## DeleteConfiguredModelAlgorithmAssociationRequestTypeDef

```python
# DeleteConfiguredModelAlgorithmAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import DeleteConfiguredModelAlgorithmAssociationRequestTypeDef


def get_value() -> DeleteConfiguredModelAlgorithmAssociationRequestTypeDef:
    return {
        "configuredModelAlgorithmAssociationArn": ...,
    }


# DeleteConfiguredModelAlgorithmAssociationRequestTypeDef definition

class DeleteConfiguredModelAlgorithmAssociationRequestTypeDef(TypedDict):
    configuredModelAlgorithmAssociationArn: str,
    membershipIdentifier: str,
```

## DeleteConfiguredModelAlgorithmRequestTypeDef

```python
# DeleteConfiguredModelAlgorithmRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import DeleteConfiguredModelAlgorithmRequestTypeDef


def get_value() -> DeleteConfiguredModelAlgorithmRequestTypeDef:
    return {
        "configuredModelAlgorithmArn": ...,
    }


# DeleteConfiguredModelAlgorithmRequestTypeDef definition

class DeleteConfiguredModelAlgorithmRequestTypeDef(TypedDict):
    configuredModelAlgorithmArn: str,
```

## DeleteMLConfigurationRequestTypeDef

```python
# DeleteMLConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import DeleteMLConfigurationRequestTypeDef


def get_value() -> DeleteMLConfigurationRequestTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# DeleteMLConfigurationRequestTypeDef definition

class DeleteMLConfigurationRequestTypeDef(TypedDict):
    membershipIdentifier: str,
```

## DeleteMLInputChannelDataRequestTypeDef

```python
# DeleteMLInputChannelDataRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import DeleteMLInputChannelDataRequestTypeDef


def get_value() -> DeleteMLInputChannelDataRequestTypeDef:
    return {
        "mlInputChannelArn": ...,
    }


# DeleteMLInputChannelDataRequestTypeDef definition

class DeleteMLInputChannelDataRequestTypeDef(TypedDict):
    mlInputChannelArn: str,
    membershipIdentifier: str,
```

## DeleteTrainedModelOutputRequestTypeDef

```python
# DeleteTrainedModelOutputRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import DeleteTrainedModelOutputRequestTypeDef


def get_value() -> DeleteTrainedModelOutputRequestTypeDef:
    return {
        "trainedModelArn": ...,
    }


# DeleteTrainedModelOutputRequestTypeDef definition

class DeleteTrainedModelOutputRequestTypeDef(TypedDict):
    trainedModelArn: str,
    membershipIdentifier: str,
```

## DeleteTrainingDatasetRequestTypeDef

```python
# DeleteTrainingDatasetRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import DeleteTrainingDatasetRequestTypeDef


def get_value() -> DeleteTrainingDatasetRequestTypeDef:
    return {
        "trainingDatasetArn": ...,
    }


# DeleteTrainingDatasetRequestTypeDef definition

class DeleteTrainingDatasetRequestTypeDef(TypedDict):
    trainingDatasetArn: str,
```

## GetAudienceGenerationJobRequestTypeDef

```python
# GetAudienceGenerationJobRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import GetAudienceGenerationJobRequestTypeDef


def get_value() -> GetAudienceGenerationJobRequestTypeDef:
    return {
        "audienceGenerationJobArn": ...,
    }


# GetAudienceGenerationJobRequestTypeDef definition

class GetAudienceGenerationJobRequestTypeDef(TypedDict):
    audienceGenerationJobArn: str,
```

## GetAudienceModelRequestTypeDef

```python
# GetAudienceModelRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import GetAudienceModelRequestTypeDef


def get_value() -> GetAudienceModelRequestTypeDef:
    return {
        "audienceModelArn": ...,
    }


# GetAudienceModelRequestTypeDef definition

class GetAudienceModelRequestTypeDef(TypedDict):
    audienceModelArn: str,
```

## GetCollaborationConfiguredModelAlgorithmAssociationRequestTypeDef

```python
# GetCollaborationConfiguredModelAlgorithmAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import GetCollaborationConfiguredModelAlgorithmAssociationRequestTypeDef


def get_value() -> GetCollaborationConfiguredModelAlgorithmAssociationRequestTypeDef:
    return {
        "configuredModelAlgorithmAssociationArn": ...,
    }


# GetCollaborationConfiguredModelAlgorithmAssociationRequestTypeDef definition

class GetCollaborationConfiguredModelAlgorithmAssociationRequestTypeDef(TypedDict):
    configuredModelAlgorithmAssociationArn: str,
    collaborationIdentifier: str,
```

## GetCollaborationMLInputChannelRequestTypeDef

```python
# GetCollaborationMLInputChannelRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import GetCollaborationMLInputChannelRequestTypeDef


def get_value() -> GetCollaborationMLInputChannelRequestTypeDef:
    return {
        "mlInputChannelArn": ...,
    }


# GetCollaborationMLInputChannelRequestTypeDef definition

class GetCollaborationMLInputChannelRequestTypeDef(TypedDict):
    mlInputChannelArn: str,
    collaborationIdentifier: str,
```

## GetCollaborationTrainedModelRequestTypeDef

```python
# GetCollaborationTrainedModelRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import GetCollaborationTrainedModelRequestTypeDef


def get_value() -> GetCollaborationTrainedModelRequestTypeDef:
    return {
        "trainedModelArn": ...,
    }


# GetCollaborationTrainedModelRequestTypeDef definition

class GetCollaborationTrainedModelRequestTypeDef(TypedDict):
    trainedModelArn: str,
    collaborationIdentifier: str,
```

## GetConfiguredAudienceModelPolicyRequestTypeDef

```python
# GetConfiguredAudienceModelPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import GetConfiguredAudienceModelPolicyRequestTypeDef


def get_value() -> GetConfiguredAudienceModelPolicyRequestTypeDef:
    return {
        "configuredAudienceModelArn": ...,
    }


# GetConfiguredAudienceModelPolicyRequestTypeDef definition

class GetConfiguredAudienceModelPolicyRequestTypeDef(TypedDict):
    configuredAudienceModelArn: str,
```

## GetConfiguredAudienceModelRequestTypeDef

```python
# GetConfiguredAudienceModelRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import GetConfiguredAudienceModelRequestTypeDef


def get_value() -> GetConfiguredAudienceModelRequestTypeDef:
    return {
        "configuredAudienceModelArn": ...,
    }


# GetConfiguredAudienceModelRequestTypeDef definition

class GetConfiguredAudienceModelRequestTypeDef(TypedDict):
    configuredAudienceModelArn: str,
```

## GetConfiguredModelAlgorithmAssociationRequestTypeDef

```python
# GetConfiguredModelAlgorithmAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import GetConfiguredModelAlgorithmAssociationRequestTypeDef


def get_value() -> GetConfiguredModelAlgorithmAssociationRequestTypeDef:
    return {
        "configuredModelAlgorithmAssociationArn": ...,
    }


# GetConfiguredModelAlgorithmAssociationRequestTypeDef definition

class GetConfiguredModelAlgorithmAssociationRequestTypeDef(TypedDict):
    configuredModelAlgorithmAssociationArn: str,
    membershipIdentifier: str,
```

## GetConfiguredModelAlgorithmRequestTypeDef

```python
# GetConfiguredModelAlgorithmRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import GetConfiguredModelAlgorithmRequestTypeDef


def get_value() -> GetConfiguredModelAlgorithmRequestTypeDef:
    return {
        "configuredModelAlgorithmArn": ...,
    }


# GetConfiguredModelAlgorithmRequestTypeDef definition

class GetConfiguredModelAlgorithmRequestTypeDef(TypedDict):
    configuredModelAlgorithmArn: str,
```

## GetMLConfigurationRequestTypeDef

```python
# GetMLConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import GetMLConfigurationRequestTypeDef


def get_value() -> GetMLConfigurationRequestTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# GetMLConfigurationRequestTypeDef definition

class GetMLConfigurationRequestTypeDef(TypedDict):
    membershipIdentifier: str,
```

## GetMLInputChannelRequestTypeDef

```python
# GetMLInputChannelRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import GetMLInputChannelRequestTypeDef


def get_value() -> GetMLInputChannelRequestTypeDef:
    return {
        "mlInputChannelArn": ...,
    }


# GetMLInputChannelRequestTypeDef definition

class GetMLInputChannelRequestTypeDef(TypedDict):
    mlInputChannelArn: str,
    membershipIdentifier: str,
```

## GetTrainedModelInferenceJobRequestTypeDef

```python
# GetTrainedModelInferenceJobRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import GetTrainedModelInferenceJobRequestTypeDef


def get_value() -> GetTrainedModelInferenceJobRequestTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# GetTrainedModelInferenceJobRequestTypeDef definition

class GetTrainedModelInferenceJobRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    trainedModelInferenceJobArn: str,
```

## InferenceContainerExecutionParametersTypeDef

```python
# InferenceContainerExecutionParametersTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import InferenceContainerExecutionParametersTypeDef


def get_value() -> InferenceContainerExecutionParametersTypeDef:
    return {
        "maxPayloadInMB": ...,
    }


# InferenceContainerExecutionParametersTypeDef definition

class InferenceContainerExecutionParametersTypeDef(TypedDict):
    maxPayloadInMB: NotRequired[int],
```

## InferenceResourceConfigTypeDef

```python
# InferenceResourceConfigTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import InferenceResourceConfigTypeDef


def get_value() -> InferenceResourceConfigTypeDef:
    return {
        "instanceType": ...,
    }


# InferenceResourceConfigTypeDef definition

class InferenceResourceConfigTypeDef(TypedDict):
    instanceType: InferenceInstanceTypeType,  # (1)
    instanceCount: NotRequired[int],
```

1. See [:material-code-brackets: InferenceInstanceTypeType](./literals.md#inferenceinstancetypetype) 
## ModelInferenceDataSourceTypeDef

```python
# ModelInferenceDataSourceTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ModelInferenceDataSourceTypeDef


def get_value() -> ModelInferenceDataSourceTypeDef:
    return {
        "mlInputChannelArn": ...,
    }


# ModelInferenceDataSourceTypeDef definition

class ModelInferenceDataSourceTypeDef(TypedDict):
    mlInputChannelArn: str,
```

## GetTrainedModelRequestTypeDef

```python
# GetTrainedModelRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import GetTrainedModelRequestTypeDef


def get_value() -> GetTrainedModelRequestTypeDef:
    return {
        "trainedModelArn": ...,
    }


# GetTrainedModelRequestTypeDef definition

class GetTrainedModelRequestTypeDef(TypedDict):
    trainedModelArn: str,
    membershipIdentifier: str,
```

## GetTrainingDatasetRequestTypeDef

```python
# GetTrainingDatasetRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import GetTrainingDatasetRequestTypeDef


def get_value() -> GetTrainingDatasetRequestTypeDef:
    return {
        "trainingDatasetArn": ...,
    }


# GetTrainingDatasetRequestTypeDef definition

class GetTrainingDatasetRequestTypeDef(TypedDict):
    trainingDatasetArn: str,
```

## InferenceReceiverMemberTypeDef

```python
# InferenceReceiverMemberTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import InferenceReceiverMemberTypeDef


def get_value() -> InferenceReceiverMemberTypeDef:
    return {
        "accountId": ...,
    }


# InferenceReceiverMemberTypeDef definition

class InferenceReceiverMemberTypeDef(TypedDict):
    accountId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import PaginatorConfigTypeDef


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

## ListAudienceExportJobsRequestTypeDef

```python
# ListAudienceExportJobsRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListAudienceExportJobsRequestTypeDef


def get_value() -> ListAudienceExportJobsRequestTypeDef:
    return {
        "nextToken": ...,
    }


# ListAudienceExportJobsRequestTypeDef definition

class ListAudienceExportJobsRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    audienceGenerationJobArn: NotRequired[str],
```

## ListAudienceGenerationJobsRequestTypeDef

```python
# ListAudienceGenerationJobsRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListAudienceGenerationJobsRequestTypeDef


def get_value() -> ListAudienceGenerationJobsRequestTypeDef:
    return {
        "nextToken": ...,
    }


# ListAudienceGenerationJobsRequestTypeDef definition

class ListAudienceGenerationJobsRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    configuredAudienceModelArn: NotRequired[str],
    collaborationId: NotRequired[str],
```

## ListAudienceModelsRequestTypeDef

```python
# ListAudienceModelsRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListAudienceModelsRequestTypeDef


def get_value() -> ListAudienceModelsRequestTypeDef:
    return {
        "nextToken": ...,
    }


# ListAudienceModelsRequestTypeDef definition

class ListAudienceModelsRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListCollaborationConfiguredModelAlgorithmAssociationsRequestTypeDef

```python
# ListCollaborationConfiguredModelAlgorithmAssociationsRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListCollaborationConfiguredModelAlgorithmAssociationsRequestTypeDef


def get_value() -> ListCollaborationConfiguredModelAlgorithmAssociationsRequestTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# ListCollaborationConfiguredModelAlgorithmAssociationsRequestTypeDef definition

class ListCollaborationConfiguredModelAlgorithmAssociationsRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListCollaborationMLInputChannelsRequestTypeDef

```python
# ListCollaborationMLInputChannelsRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListCollaborationMLInputChannelsRequestTypeDef


def get_value() -> ListCollaborationMLInputChannelsRequestTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# ListCollaborationMLInputChannelsRequestTypeDef definition

class ListCollaborationMLInputChannelsRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListCollaborationTrainedModelExportJobsRequestTypeDef

```python
# ListCollaborationTrainedModelExportJobsRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListCollaborationTrainedModelExportJobsRequestTypeDef


def get_value() -> ListCollaborationTrainedModelExportJobsRequestTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# ListCollaborationTrainedModelExportJobsRequestTypeDef definition

class ListCollaborationTrainedModelExportJobsRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    trainedModelArn: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListCollaborationTrainedModelInferenceJobsRequestTypeDef

```python
# ListCollaborationTrainedModelInferenceJobsRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListCollaborationTrainedModelInferenceJobsRequestTypeDef


def get_value() -> ListCollaborationTrainedModelInferenceJobsRequestTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# ListCollaborationTrainedModelInferenceJobsRequestTypeDef definition

class ListCollaborationTrainedModelInferenceJobsRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    trainedModelArn: NotRequired[str],
```

## ListCollaborationTrainedModelsRequestTypeDef

```python
# ListCollaborationTrainedModelsRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListCollaborationTrainedModelsRequestTypeDef


def get_value() -> ListCollaborationTrainedModelsRequestTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# ListCollaborationTrainedModelsRequestTypeDef definition

class ListCollaborationTrainedModelsRequestTypeDef(TypedDict):
    collaborationIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListConfiguredAudienceModelsRequestTypeDef

```python
# ListConfiguredAudienceModelsRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListConfiguredAudienceModelsRequestTypeDef


def get_value() -> ListConfiguredAudienceModelsRequestTypeDef:
    return {
        "nextToken": ...,
    }


# ListConfiguredAudienceModelsRequestTypeDef definition

class ListConfiguredAudienceModelsRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListConfiguredModelAlgorithmAssociationsRequestTypeDef

```python
# ListConfiguredModelAlgorithmAssociationsRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListConfiguredModelAlgorithmAssociationsRequestTypeDef


def get_value() -> ListConfiguredModelAlgorithmAssociationsRequestTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# ListConfiguredModelAlgorithmAssociationsRequestTypeDef definition

class ListConfiguredModelAlgorithmAssociationsRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListConfiguredModelAlgorithmsRequestTypeDef

```python
# ListConfiguredModelAlgorithmsRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListConfiguredModelAlgorithmsRequestTypeDef


def get_value() -> ListConfiguredModelAlgorithmsRequestTypeDef:
    return {
        "nextToken": ...,
    }


# ListConfiguredModelAlgorithmsRequestTypeDef definition

class ListConfiguredModelAlgorithmsRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListMLInputChannelsRequestTypeDef

```python
# ListMLInputChannelsRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListMLInputChannelsRequestTypeDef


def get_value() -> ListMLInputChannelsRequestTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# ListMLInputChannelsRequestTypeDef definition

class ListMLInputChannelsRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## MLInputChannelSummaryTypeDef

```python
# MLInputChannelSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import MLInputChannelSummaryTypeDef


def get_value() -> MLInputChannelSummaryTypeDef:
    return {
        "createTime": ...,
    }


# MLInputChannelSummaryTypeDef definition

class MLInputChannelSummaryTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    membershipIdentifier: str,
    collaborationIdentifier: str,
    name: str,
    configuredModelAlgorithmAssociations: List[str],
    mlInputChannelArn: str,
    status: MLInputChannelStatusType,  # (1)
    protectedQueryIdentifier: NotRequired[str],
    description: NotRequired[str],
```

1. See [:material-code-brackets: MLInputChannelStatusType](./literals.md#mlinputchannelstatustype) 
## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListTrainedModelInferenceJobsRequestTypeDef

```python
# ListTrainedModelInferenceJobsRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListTrainedModelInferenceJobsRequestTypeDef


def get_value() -> ListTrainedModelInferenceJobsRequestTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# ListTrainedModelInferenceJobsRequestTypeDef definition

class ListTrainedModelInferenceJobsRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    trainedModelArn: NotRequired[str],
```

## ListTrainedModelsRequestTypeDef

```python
# ListTrainedModelsRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListTrainedModelsRequestTypeDef


def get_value() -> ListTrainedModelsRequestTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# ListTrainedModelsRequestTypeDef definition

class ListTrainedModelsRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## TrainedModelSummaryTypeDef

```python
# TrainedModelSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import TrainedModelSummaryTypeDef


def get_value() -> TrainedModelSummaryTypeDef:
    return {
        "createTime": ...,
    }


# TrainedModelSummaryTypeDef definition

class TrainedModelSummaryTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    trainedModelArn: str,
    name: str,
    membershipIdentifier: str,
    collaborationIdentifier: str,
    status: TrainedModelStatusType,  # (1)
    configuredModelAlgorithmAssociationArn: str,
    description: NotRequired[str],
```

1. See [:material-code-brackets: TrainedModelStatusType](./literals.md#trainedmodelstatustype) 
## ListTrainingDatasetsRequestTypeDef

```python
# ListTrainingDatasetsRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListTrainingDatasetsRequestTypeDef


def get_value() -> ListTrainingDatasetsRequestTypeDef:
    return {
        "nextToken": ...,
    }


# ListTrainingDatasetsRequestTypeDef definition

class ListTrainingDatasetsRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## TrainingDatasetSummaryTypeDef

```python
# TrainingDatasetSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import TrainingDatasetSummaryTypeDef


def get_value() -> TrainingDatasetSummaryTypeDef:
    return {
        "createTime": ...,
    }


# TrainingDatasetSummaryTypeDef definition

class TrainingDatasetSummaryTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    trainingDatasetArn: str,
    name: str,
    status: TrainingDatasetStatusType,  # (1)
    description: NotRequired[str],
```

1. See [:material-code-brackets: TrainingDatasetStatusType](./literals.md#trainingdatasetstatustype) 
## LogsConfigurationPolicyOutputTypeDef

```python
# LogsConfigurationPolicyOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import LogsConfigurationPolicyOutputTypeDef


def get_value() -> LogsConfigurationPolicyOutputTypeDef:
    return {
        "allowedAccountIds": ...,
    }


# LogsConfigurationPolicyOutputTypeDef definition

class LogsConfigurationPolicyOutputTypeDef(TypedDict):
    allowedAccountIds: List[str],
    filterPattern: NotRequired[str],
```

## LogsConfigurationPolicyTypeDef

```python
# LogsConfigurationPolicyTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import LogsConfigurationPolicyTypeDef


def get_value() -> LogsConfigurationPolicyTypeDef:
    return {
        "allowedAccountIds": ...,
    }


# LogsConfigurationPolicyTypeDef definition

class LogsConfigurationPolicyTypeDef(TypedDict):
    allowedAccountIds: Sequence[str],
    filterPattern: NotRequired[str],
```

## MetricsConfigurationPolicyTypeDef

```python
# MetricsConfigurationPolicyTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import MetricsConfigurationPolicyTypeDef


def get_value() -> MetricsConfigurationPolicyTypeDef:
    return {
        "noiseLevel": ...,
    }


# MetricsConfigurationPolicyTypeDef definition

class MetricsConfigurationPolicyTypeDef(TypedDict):
    noiseLevel: NoiseLevelTypeType,  # (1)
```

1. See [:material-code-brackets: NoiseLevelTypeType](./literals.md#noiseleveltypetype) 
## PutConfiguredAudienceModelPolicyRequestTypeDef

```python
# PutConfiguredAudienceModelPolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import PutConfiguredAudienceModelPolicyRequestTypeDef


def get_value() -> PutConfiguredAudienceModelPolicyRequestTypeDef:
    return {
        "configuredAudienceModelArn": ...,
    }


# PutConfiguredAudienceModelPolicyRequestTypeDef definition

class PutConfiguredAudienceModelPolicyRequestTypeDef(TypedDict):
    configuredAudienceModelArn: str,
    configuredAudienceModelPolicy: str,
    previousPolicyHash: NotRequired[str],
    policyExistenceCondition: NotRequired[PolicyExistenceConditionType],  # (1)
```

1. See [:material-code-brackets: PolicyExistenceConditionType](./literals.md#policyexistenceconditiontype) 
## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## TrainedModelExportReceiverMemberTypeDef

```python
# TrainedModelExportReceiverMemberTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import TrainedModelExportReceiverMemberTypeDef


def get_value() -> TrainedModelExportReceiverMemberTypeDef:
    return {
        "accountId": ...,
    }


# TrainedModelExportReceiverMemberTypeDef definition

class TrainedModelExportReceiverMemberTypeDef(TypedDict):
    accountId: str,
```

## TrainedModelExportsMaxSizeTypeDef

```python
# TrainedModelExportsMaxSizeTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import TrainedModelExportsMaxSizeTypeDef


def get_value() -> TrainedModelExportsMaxSizeTypeDef:
    return {
        "unit": ...,
    }


# TrainedModelExportsMaxSizeTypeDef definition

class TrainedModelExportsMaxSizeTypeDef(TypedDict):
    unit: TrainedModelExportsMaxSizeUnitTypeType,  # (1)
    value: float,
```

1. See [:material-code-brackets: TrainedModelExportsMaxSizeUnitTypeType](./literals.md#trainedmodelexportsmaxsizeunittypetype) 
## TrainedModelInferenceMaxOutputSizeTypeDef

```python
# TrainedModelInferenceMaxOutputSizeTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import TrainedModelInferenceMaxOutputSizeTypeDef


def get_value() -> TrainedModelInferenceMaxOutputSizeTypeDef:
    return {
        "unit": ...,
    }


# TrainedModelInferenceMaxOutputSizeTypeDef definition

class TrainedModelInferenceMaxOutputSizeTypeDef(TypedDict):
    unit: TrainedModelInferenceMaxOutputSizeUnitTypeType,  # (1)
    value: float,
```

1. See [:material-code-brackets: TrainedModelInferenceMaxOutputSizeUnitTypeType](./literals.md#trainedmodelinferencemaxoutputsizeunittypetype) 
## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## AudienceDestinationTypeDef

```python
# AudienceDestinationTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import AudienceDestinationTypeDef


def get_value() -> AudienceDestinationTypeDef:
    return {
        "s3Destination": ...,
    }


# AudienceDestinationTypeDef definition

class AudienceDestinationTypeDef(TypedDict):
    s3Destination: S3ConfigMapTypeDef,  # (1)
```

1. See [:material-code-braces: S3ConfigMapTypeDef](./type_defs.md#s3configmaptypedef) 
## DestinationTypeDef

```python
# DestinationTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import DestinationTypeDef


def get_value() -> DestinationTypeDef:
    return {
        "s3Destination": ...,
    }


# DestinationTypeDef definition

class DestinationTypeDef(TypedDict):
    s3Destination: S3ConfigMapTypeDef,  # (1)
```

1. See [:material-code-braces: S3ConfigMapTypeDef](./type_defs.md#s3configmaptypedef) 
## RelevanceMetricTypeDef

```python
# RelevanceMetricTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import RelevanceMetricTypeDef


def get_value() -> RelevanceMetricTypeDef:
    return {
        "audienceSize": ...,
    }


# RelevanceMetricTypeDef definition

class RelevanceMetricTypeDef(TypedDict):
    audienceSize: AudienceSizeTypeDef,  # (1)
    score: NotRequired[float],
```

1. See [:material-code-braces: AudienceSizeTypeDef](./type_defs.md#audiencesizetypedef) 
## StartAudienceExportJobRequestTypeDef

```python
# StartAudienceExportJobRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import StartAudienceExportJobRequestTypeDef


def get_value() -> StartAudienceExportJobRequestTypeDef:
    return {
        "name": ...,
    }


# StartAudienceExportJobRequestTypeDef definition

class StartAudienceExportJobRequestTypeDef(TypedDict):
    name: str,
    audienceGenerationJobArn: str,
    audienceSize: AudienceSizeTypeDef,  # (1)
    description: NotRequired[str],
```

1. See [:material-code-braces: AudienceSizeTypeDef](./type_defs.md#audiencesizetypedef) 
## AudienceExportJobSummaryTypeDef

```python
# AudienceExportJobSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import AudienceExportJobSummaryTypeDef


def get_value() -> AudienceExportJobSummaryTypeDef:
    return {
        "createTime": ...,
    }


# AudienceExportJobSummaryTypeDef definition

class AudienceExportJobSummaryTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    name: str,
    audienceGenerationJobArn: str,
    audienceSize: AudienceSizeTypeDef,  # (1)
    status: AudienceExportJobStatusType,  # (2)
    description: NotRequired[str],
    statusDetails: NotRequired[StatusDetailsTypeDef],  # (3)
    outputLocation: NotRequired[str],
```

1. See [:material-code-braces: AudienceSizeTypeDef](./type_defs.md#audiencesizetypedef) 
2. See [:material-code-brackets: AudienceExportJobStatusType](./literals.md#audienceexportjobstatustype) 
3. See [:material-code-braces: StatusDetailsTypeDef](./type_defs.md#statusdetailstypedef) 
## ComputeConfigurationTypeDef

```python
# ComputeConfigurationTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ComputeConfigurationTypeDef


def get_value() -> ComputeConfigurationTypeDef:
    return {
        "worker": ...,
    }


# ComputeConfigurationTypeDef definition

class ComputeConfigurationTypeDef(TypedDict):
    worker: NotRequired[WorkerComputeConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: WorkerComputeConfigurationTypeDef](./type_defs.md#workercomputeconfigurationtypedef) 
## ContainerConfigOutputTypeDef

```python
# ContainerConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ContainerConfigOutputTypeDef


def get_value() -> ContainerConfigOutputTypeDef:
    return {
        "imageUri": ...,
    }


# ContainerConfigOutputTypeDef definition

class ContainerConfigOutputTypeDef(TypedDict):
    imageUri: str,
    entrypoint: NotRequired[List[str]],
    arguments: NotRequired[List[str]],
    metricDefinitions: NotRequired[List[MetricDefinitionTypeDef]],  # (1)
```

1. See [:material-code-braces: MetricDefinitionTypeDef](./type_defs.md#metricdefinitiontypedef) 
## ContainerConfigTypeDef

```python
# ContainerConfigTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ContainerConfigTypeDef


def get_value() -> ContainerConfigTypeDef:
    return {
        "imageUri": ...,
    }


# ContainerConfigTypeDef definition

class ContainerConfigTypeDef(TypedDict):
    imageUri: str,
    entrypoint: NotRequired[Sequence[str]],
    arguments: NotRequired[Sequence[str]],
    metricDefinitions: NotRequired[Sequence[MetricDefinitionTypeDef]],  # (1)
```

1. See [:material-code-braces: MetricDefinitionTypeDef](./type_defs.md#metricdefinitiontypedef) 
## CreateAudienceModelRequestTypeDef

```python
# CreateAudienceModelRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import CreateAudienceModelRequestTypeDef


def get_value() -> CreateAudienceModelRequestTypeDef:
    return {
        "name": ...,
    }


# CreateAudienceModelRequestTypeDef definition

class CreateAudienceModelRequestTypeDef(TypedDict):
    name: str,
    trainingDatasetArn: str,
    trainingDataStartTime: NotRequired[TimestampTypeDef],
    trainingDataEndTime: NotRequired[TimestampTypeDef],
    kmsKeyArn: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    description: NotRequired[str],
```

## CreateAudienceModelResponseTypeDef

```python
# CreateAudienceModelResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import CreateAudienceModelResponseTypeDef


def get_value() -> CreateAudienceModelResponseTypeDef:
    return {
        "audienceModelArn": ...,
    }


# CreateAudienceModelResponseTypeDef definition

class CreateAudienceModelResponseTypeDef(TypedDict):
    audienceModelArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConfiguredAudienceModelResponseTypeDef

```python
# CreateConfiguredAudienceModelResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import CreateConfiguredAudienceModelResponseTypeDef


def get_value() -> CreateConfiguredAudienceModelResponseTypeDef:
    return {
        "configuredAudienceModelArn": ...,
    }


# CreateConfiguredAudienceModelResponseTypeDef definition

class CreateConfiguredAudienceModelResponseTypeDef(TypedDict):
    configuredAudienceModelArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConfiguredModelAlgorithmAssociationResponseTypeDef

```python
# CreateConfiguredModelAlgorithmAssociationResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import CreateConfiguredModelAlgorithmAssociationResponseTypeDef


def get_value() -> CreateConfiguredModelAlgorithmAssociationResponseTypeDef:
    return {
        "configuredModelAlgorithmAssociationArn": ...,
    }


# CreateConfiguredModelAlgorithmAssociationResponseTypeDef definition

class CreateConfiguredModelAlgorithmAssociationResponseTypeDef(TypedDict):
    configuredModelAlgorithmAssociationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConfiguredModelAlgorithmResponseTypeDef

```python
# CreateConfiguredModelAlgorithmResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import CreateConfiguredModelAlgorithmResponseTypeDef


def get_value() -> CreateConfiguredModelAlgorithmResponseTypeDef:
    return {
        "configuredModelAlgorithmArn": ...,
    }


# CreateConfiguredModelAlgorithmResponseTypeDef definition

class CreateConfiguredModelAlgorithmResponseTypeDef(TypedDict):
    configuredModelAlgorithmArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMLInputChannelResponseTypeDef

```python
# CreateMLInputChannelResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import CreateMLInputChannelResponseTypeDef


def get_value() -> CreateMLInputChannelResponseTypeDef:
    return {
        "mlInputChannelArn": ...,
    }


# CreateMLInputChannelResponseTypeDef definition

class CreateMLInputChannelResponseTypeDef(TypedDict):
    mlInputChannelArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTrainedModelResponseTypeDef

```python
# CreateTrainedModelResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import CreateTrainedModelResponseTypeDef


def get_value() -> CreateTrainedModelResponseTypeDef:
    return {
        "trainedModelArn": ...,
    }


# CreateTrainedModelResponseTypeDef definition

class CreateTrainedModelResponseTypeDef(TypedDict):
    trainedModelArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTrainingDatasetResponseTypeDef

```python
# CreateTrainingDatasetResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import CreateTrainingDatasetResponseTypeDef


def get_value() -> CreateTrainingDatasetResponseTypeDef:
    return {
        "trainingDatasetArn": ...,
    }


# CreateTrainingDatasetResponseTypeDef definition

class CreateTrainingDatasetResponseTypeDef(TypedDict):
    trainingDatasetArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAudienceModelResponseTypeDef

```python
# GetAudienceModelResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import GetAudienceModelResponseTypeDef


def get_value() -> GetAudienceModelResponseTypeDef:
    return {
        "createTime": ...,
    }


# GetAudienceModelResponseTypeDef definition

class GetAudienceModelResponseTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    trainingDataStartTime: datetime,
    trainingDataEndTime: datetime,
    audienceModelArn: str,
    name: str,
    trainingDatasetArn: str,
    status: AudienceModelStatusType,  # (1)
    statusDetails: StatusDetailsTypeDef,  # (2)
    kmsKeyArn: str,
    tags: Dict[str, str],
    description: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: AudienceModelStatusType](./literals.md#audiencemodelstatustype) 
2. See [:material-code-braces: StatusDetailsTypeDef](./type_defs.md#statusdetailstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCollaborationMLInputChannelResponseTypeDef

```python
# GetCollaborationMLInputChannelResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import GetCollaborationMLInputChannelResponseTypeDef


def get_value() -> GetCollaborationMLInputChannelResponseTypeDef:
    return {
        "createTime": ...,
    }


# GetCollaborationMLInputChannelResponseTypeDef definition

class GetCollaborationMLInputChannelResponseTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    creatorAccountId: str,
    membershipIdentifier: str,
    collaborationIdentifier: str,
    mlInputChannelArn: str,
    name: str,
    configuredModelAlgorithmAssociations: List[str],
    status: MLInputChannelStatusType,  # (1)
    statusDetails: StatusDetailsTypeDef,  # (2)
    retentionInDays: int,
    numberOfRecords: int,
    description: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: MLInputChannelStatusType](./literals.md#mlinputchannelstatustype) 
2. See [:material-code-braces: StatusDetailsTypeDef](./type_defs.md#statusdetailstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConfiguredAudienceModelPolicyResponseTypeDef

```python
# GetConfiguredAudienceModelPolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import GetConfiguredAudienceModelPolicyResponseTypeDef


def get_value() -> GetConfiguredAudienceModelPolicyResponseTypeDef:
    return {
        "configuredAudienceModelArn": ...,
    }


# GetConfiguredAudienceModelPolicyResponseTypeDef definition

class GetConfiguredAudienceModelPolicyResponseTypeDef(TypedDict):
    configuredAudienceModelArn: str,
    configuredAudienceModelPolicy: str,
    policyHash: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAudienceGenerationJobsResponseTypeDef

```python
# ListAudienceGenerationJobsResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListAudienceGenerationJobsResponseTypeDef


def get_value() -> ListAudienceGenerationJobsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListAudienceGenerationJobsResponseTypeDef definition

class ListAudienceGenerationJobsResponseTypeDef(TypedDict):
    audienceGenerationJobs: List[AudienceGenerationJobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AudienceGenerationJobSummaryTypeDef](./type_defs.md#audiencegenerationjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAudienceModelsResponseTypeDef

```python
# ListAudienceModelsResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListAudienceModelsResponseTypeDef


def get_value() -> ListAudienceModelsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListAudienceModelsResponseTypeDef definition

class ListAudienceModelsResponseTypeDef(TypedDict):
    audienceModels: List[AudienceModelSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AudienceModelSummaryTypeDef](./type_defs.md#audiencemodelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCollaborationConfiguredModelAlgorithmAssociationsResponseTypeDef

```python
# ListCollaborationConfiguredModelAlgorithmAssociationsResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListCollaborationConfiguredModelAlgorithmAssociationsResponseTypeDef


def get_value() -> ListCollaborationConfiguredModelAlgorithmAssociationsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListCollaborationConfiguredModelAlgorithmAssociationsResponseTypeDef definition

class ListCollaborationConfiguredModelAlgorithmAssociationsResponseTypeDef(TypedDict):
    collaborationConfiguredModelAlgorithmAssociations: List[CollaborationConfiguredModelAlgorithmAssociationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CollaborationConfiguredModelAlgorithmAssociationSummaryTypeDef](./type_defs.md#collaborationconfiguredmodelalgorithmassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCollaborationMLInputChannelsResponseTypeDef

```python
# ListCollaborationMLInputChannelsResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListCollaborationMLInputChannelsResponseTypeDef


def get_value() -> ListCollaborationMLInputChannelsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListCollaborationMLInputChannelsResponseTypeDef definition

class ListCollaborationMLInputChannelsResponseTypeDef(TypedDict):
    collaborationMLInputChannelsList: List[CollaborationMLInputChannelSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CollaborationMLInputChannelSummaryTypeDef](./type_defs.md#collaborationmlinputchannelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCollaborationTrainedModelsResponseTypeDef

```python
# ListCollaborationTrainedModelsResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListCollaborationTrainedModelsResponseTypeDef


def get_value() -> ListCollaborationTrainedModelsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListCollaborationTrainedModelsResponseTypeDef definition

class ListCollaborationTrainedModelsResponseTypeDef(TypedDict):
    collaborationTrainedModels: List[CollaborationTrainedModelSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CollaborationTrainedModelSummaryTypeDef](./type_defs.md#collaborationtrainedmodelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConfiguredModelAlgorithmAssociationsResponseTypeDef

```python
# ListConfiguredModelAlgorithmAssociationsResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListConfiguredModelAlgorithmAssociationsResponseTypeDef


def get_value() -> ListConfiguredModelAlgorithmAssociationsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListConfiguredModelAlgorithmAssociationsResponseTypeDef definition

class ListConfiguredModelAlgorithmAssociationsResponseTypeDef(TypedDict):
    configuredModelAlgorithmAssociations: List[ConfiguredModelAlgorithmAssociationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ConfiguredModelAlgorithmAssociationSummaryTypeDef](./type_defs.md#configuredmodelalgorithmassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConfiguredModelAlgorithmsResponseTypeDef

```python
# ListConfiguredModelAlgorithmsResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListConfiguredModelAlgorithmsResponseTypeDef


def get_value() -> ListConfiguredModelAlgorithmsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListConfiguredModelAlgorithmsResponseTypeDef definition

class ListConfiguredModelAlgorithmsResponseTypeDef(TypedDict):
    configuredModelAlgorithms: List[ConfiguredModelAlgorithmSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ConfiguredModelAlgorithmSummaryTypeDef](./type_defs.md#configuredmodelalgorithmsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListTagsForResourceResponseTypeDef


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
## PutConfiguredAudienceModelPolicyResponseTypeDef

```python
# PutConfiguredAudienceModelPolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import PutConfiguredAudienceModelPolicyResponseTypeDef


def get_value() -> PutConfiguredAudienceModelPolicyResponseTypeDef:
    return {
        "configuredAudienceModelPolicy": ...,
    }


# PutConfiguredAudienceModelPolicyResponseTypeDef definition

class PutConfiguredAudienceModelPolicyResponseTypeDef(TypedDict):
    configuredAudienceModelPolicy: str,
    policyHash: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartAudienceGenerationJobResponseTypeDef

```python
# StartAudienceGenerationJobResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import StartAudienceGenerationJobResponseTypeDef


def get_value() -> StartAudienceGenerationJobResponseTypeDef:
    return {
        "audienceGenerationJobArn": ...,
    }


# StartAudienceGenerationJobResponseTypeDef definition

class StartAudienceGenerationJobResponseTypeDef(TypedDict):
    audienceGenerationJobArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartTrainedModelInferenceJobResponseTypeDef

```python
# StartTrainedModelInferenceJobResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import StartTrainedModelInferenceJobResponseTypeDef


def get_value() -> StartTrainedModelInferenceJobResponseTypeDef:
    return {
        "trainedModelInferenceJobArn": ...,
    }


# StartTrainedModelInferenceJobResponseTypeDef definition

class StartTrainedModelInferenceJobResponseTypeDef(TypedDict):
    trainedModelInferenceJobArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateConfiguredAudienceModelResponseTypeDef

```python
# UpdateConfiguredAudienceModelResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import UpdateConfiguredAudienceModelResponseTypeDef


def get_value() -> UpdateConfiguredAudienceModelResponseTypeDef:
    return {
        "configuredAudienceModelArn": ...,
    }


# UpdateConfiguredAudienceModelResponseTypeDef definition

class UpdateConfiguredAudienceModelResponseTypeDef(TypedDict):
    configuredAudienceModelArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTrainedModelRequestTypeDef

```python
# CreateTrainedModelRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import CreateTrainedModelRequestTypeDef


def get_value() -> CreateTrainedModelRequestTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# CreateTrainedModelRequestTypeDef definition

class CreateTrainedModelRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    name: str,
    configuredModelAlgorithmAssociationArn: str,
    resourceConfig: ResourceConfigTypeDef,  # (1)
    dataChannels: Sequence[ModelTrainingDataChannelTypeDef],  # (2)
    hyperparameters: NotRequired[Mapping[str, str]],
    environment: NotRequired[Mapping[str, str]],
    stoppingCondition: NotRequired[StoppingConditionTypeDef],  # (3)
    description: NotRequired[str],
    kmsKeyArn: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ResourceConfigTypeDef](./type_defs.md#resourceconfigtypedef) 
2. See [:material-code-braces: ModelTrainingDataChannelTypeDef](./type_defs.md#modeltrainingdatachanneltypedef) 
3. See [:material-code-braces: StoppingConditionTypeDef](./type_defs.md#stoppingconditiontypedef) 
## GetCollaborationTrainedModelResponseTypeDef

```python
# GetCollaborationTrainedModelResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import GetCollaborationTrainedModelResponseTypeDef


def get_value() -> GetCollaborationTrainedModelResponseTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# GetCollaborationTrainedModelResponseTypeDef definition

class GetCollaborationTrainedModelResponseTypeDef(TypedDict):
    membershipIdentifier: str,
    collaborationIdentifier: str,
    trainedModelArn: str,
    name: str,
    description: str,
    status: TrainedModelStatusType,  # (1)
    statusDetails: StatusDetailsTypeDef,  # (2)
    configuredModelAlgorithmAssociationArn: str,
    resourceConfig: ResourceConfigTypeDef,  # (3)
    stoppingCondition: StoppingConditionTypeDef,  # (4)
    metricsStatus: MetricsStatusType,  # (5)
    metricsStatusDetails: str,
    logsStatus: LogsStatusType,  # (6)
    logsStatusDetails: str,
    trainingContainerImageDigest: str,
    createTime: datetime,
    updateTime: datetime,
    creatorAccountId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-brackets: TrainedModelStatusType](./literals.md#trainedmodelstatustype) 
2. See [:material-code-braces: StatusDetailsTypeDef](./type_defs.md#statusdetailstypedef) 
3. See [:material-code-braces: ResourceConfigTypeDef](./type_defs.md#resourceconfigtypedef) 
4. See [:material-code-braces: StoppingConditionTypeDef](./type_defs.md#stoppingconditiontypedef) 
5. See [:material-code-brackets: MetricsStatusType](./literals.md#metricsstatustype) 
6. See [:material-code-brackets: LogsStatusType](./literals.md#logsstatustype) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTrainedModelResponseTypeDef

```python
# GetTrainedModelResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import GetTrainedModelResponseTypeDef


def get_value() -> GetTrainedModelResponseTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# GetTrainedModelResponseTypeDef definition

class GetTrainedModelResponseTypeDef(TypedDict):
    membershipIdentifier: str,
    collaborationIdentifier: str,
    trainedModelArn: str,
    name: str,
    description: str,
    status: TrainedModelStatusType,  # (1)
    statusDetails: StatusDetailsTypeDef,  # (2)
    configuredModelAlgorithmAssociationArn: str,
    resourceConfig: ResourceConfigTypeDef,  # (3)
    stoppingCondition: StoppingConditionTypeDef,  # (4)
    metricsStatus: MetricsStatusType,  # (5)
    metricsStatusDetails: str,
    logsStatus: LogsStatusType,  # (6)
    logsStatusDetails: str,
    trainingContainerImageDigest: str,
    createTime: datetime,
    updateTime: datetime,
    hyperparameters: Dict[str, str],
    environment: Dict[str, str],
    kmsKeyArn: str,
    tags: Dict[str, str],
    dataChannels: List[ModelTrainingDataChannelTypeDef],  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-brackets: TrainedModelStatusType](./literals.md#trainedmodelstatustype) 
2. See [:material-code-braces: StatusDetailsTypeDef](./type_defs.md#statusdetailstypedef) 
3. See [:material-code-braces: ResourceConfigTypeDef](./type_defs.md#resourceconfigtypedef) 
4. See [:material-code-braces: StoppingConditionTypeDef](./type_defs.md#stoppingconditiontypedef) 
5. See [:material-code-brackets: MetricsStatusType](./literals.md#metricsstatustype) 
6. See [:material-code-brackets: LogsStatusType](./literals.md#logsstatustype) 
7. See [:material-code-braces: ModelTrainingDataChannelTypeDef](./type_defs.md#modeltrainingdatachanneltypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataSourceTypeDef

```python
# DataSourceTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import DataSourceTypeDef


def get_value() -> DataSourceTypeDef:
    return {
        "glueDataSource": ...,
    }


# DataSourceTypeDef definition

class DataSourceTypeDef(TypedDict):
    glueDataSource: GlueDataSourceTypeDef,  # (1)
```

1. See [:material-code-braces: GlueDataSourceTypeDef](./type_defs.md#gluedatasourcetypedef) 
## InferenceOutputConfigurationOutputTypeDef

```python
# InferenceOutputConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import InferenceOutputConfigurationOutputTypeDef


def get_value() -> InferenceOutputConfigurationOutputTypeDef:
    return {
        "accept": ...,
    }


# InferenceOutputConfigurationOutputTypeDef definition

class InferenceOutputConfigurationOutputTypeDef(TypedDict):
    members: List[InferenceReceiverMemberTypeDef],  # (1)
    accept: NotRequired[str],
```

1. See [:material-code-braces: InferenceReceiverMemberTypeDef](./type_defs.md#inferencereceivermembertypedef) 
## InferenceOutputConfigurationTypeDef

```python
# InferenceOutputConfigurationTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import InferenceOutputConfigurationTypeDef


def get_value() -> InferenceOutputConfigurationTypeDef:
    return {
        "accept": ...,
    }


# InferenceOutputConfigurationTypeDef definition

class InferenceOutputConfigurationTypeDef(TypedDict):
    members: Sequence[InferenceReceiverMemberTypeDef],  # (1)
    accept: NotRequired[str],
```

1. See [:material-code-braces: InferenceReceiverMemberTypeDef](./type_defs.md#inferencereceivermembertypedef) 
## ListAudienceExportJobsRequestPaginateTypeDef

```python
# ListAudienceExportJobsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListAudienceExportJobsRequestPaginateTypeDef


def get_value() -> ListAudienceExportJobsRequestPaginateTypeDef:
    return {
        "audienceGenerationJobArn": ...,
    }


# ListAudienceExportJobsRequestPaginateTypeDef definition

class ListAudienceExportJobsRequestPaginateTypeDef(TypedDict):
    audienceGenerationJobArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAudienceGenerationJobsRequestPaginateTypeDef

```python
# ListAudienceGenerationJobsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListAudienceGenerationJobsRequestPaginateTypeDef


def get_value() -> ListAudienceGenerationJobsRequestPaginateTypeDef:
    return {
        "configuredAudienceModelArn": ...,
    }


# ListAudienceGenerationJobsRequestPaginateTypeDef definition

class ListAudienceGenerationJobsRequestPaginateTypeDef(TypedDict):
    configuredAudienceModelArn: NotRequired[str],
    collaborationId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAudienceModelsRequestPaginateTypeDef

```python
# ListAudienceModelsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListAudienceModelsRequestPaginateTypeDef


def get_value() -> ListAudienceModelsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListAudienceModelsRequestPaginateTypeDef definition

class ListAudienceModelsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCollaborationConfiguredModelAlgorithmAssociationsRequestPaginateTypeDef

```python
# ListCollaborationConfiguredModelAlgorithmAssociationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListCollaborationConfiguredModelAlgorithmAssociationsRequestPaginateTypeDef


def get_value() -> ListCollaborationConfiguredModelAlgorithmAssociationsRequestPaginateTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# ListCollaborationConfiguredModelAlgorithmAssociationsRequestPaginateTypeDef definition

class ListCollaborationConfiguredModelAlgorithmAssociationsRequestPaginateTypeDef(TypedDict):
    collaborationIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCollaborationMLInputChannelsRequestPaginateTypeDef

```python
# ListCollaborationMLInputChannelsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListCollaborationMLInputChannelsRequestPaginateTypeDef


def get_value() -> ListCollaborationMLInputChannelsRequestPaginateTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# ListCollaborationMLInputChannelsRequestPaginateTypeDef definition

class ListCollaborationMLInputChannelsRequestPaginateTypeDef(TypedDict):
    collaborationIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCollaborationTrainedModelExportJobsRequestPaginateTypeDef

```python
# ListCollaborationTrainedModelExportJobsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListCollaborationTrainedModelExportJobsRequestPaginateTypeDef


def get_value() -> ListCollaborationTrainedModelExportJobsRequestPaginateTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# ListCollaborationTrainedModelExportJobsRequestPaginateTypeDef definition

class ListCollaborationTrainedModelExportJobsRequestPaginateTypeDef(TypedDict):
    collaborationIdentifier: str,
    trainedModelArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCollaborationTrainedModelInferenceJobsRequestPaginateTypeDef

```python
# ListCollaborationTrainedModelInferenceJobsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListCollaborationTrainedModelInferenceJobsRequestPaginateTypeDef


def get_value() -> ListCollaborationTrainedModelInferenceJobsRequestPaginateTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# ListCollaborationTrainedModelInferenceJobsRequestPaginateTypeDef definition

class ListCollaborationTrainedModelInferenceJobsRequestPaginateTypeDef(TypedDict):
    collaborationIdentifier: str,
    trainedModelArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCollaborationTrainedModelsRequestPaginateTypeDef

```python
# ListCollaborationTrainedModelsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListCollaborationTrainedModelsRequestPaginateTypeDef


def get_value() -> ListCollaborationTrainedModelsRequestPaginateTypeDef:
    return {
        "collaborationIdentifier": ...,
    }


# ListCollaborationTrainedModelsRequestPaginateTypeDef definition

class ListCollaborationTrainedModelsRequestPaginateTypeDef(TypedDict):
    collaborationIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConfiguredAudienceModelsRequestPaginateTypeDef

```python
# ListConfiguredAudienceModelsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListConfiguredAudienceModelsRequestPaginateTypeDef


def get_value() -> ListConfiguredAudienceModelsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListConfiguredAudienceModelsRequestPaginateTypeDef definition

class ListConfiguredAudienceModelsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConfiguredModelAlgorithmAssociationsRequestPaginateTypeDef

```python
# ListConfiguredModelAlgorithmAssociationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListConfiguredModelAlgorithmAssociationsRequestPaginateTypeDef


def get_value() -> ListConfiguredModelAlgorithmAssociationsRequestPaginateTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# ListConfiguredModelAlgorithmAssociationsRequestPaginateTypeDef definition

class ListConfiguredModelAlgorithmAssociationsRequestPaginateTypeDef(TypedDict):
    membershipIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConfiguredModelAlgorithmsRequestPaginateTypeDef

```python
# ListConfiguredModelAlgorithmsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListConfiguredModelAlgorithmsRequestPaginateTypeDef


def get_value() -> ListConfiguredModelAlgorithmsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListConfiguredModelAlgorithmsRequestPaginateTypeDef definition

class ListConfiguredModelAlgorithmsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMLInputChannelsRequestPaginateTypeDef

```python
# ListMLInputChannelsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListMLInputChannelsRequestPaginateTypeDef


def get_value() -> ListMLInputChannelsRequestPaginateTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# ListMLInputChannelsRequestPaginateTypeDef definition

class ListMLInputChannelsRequestPaginateTypeDef(TypedDict):
    membershipIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTrainedModelInferenceJobsRequestPaginateTypeDef

```python
# ListTrainedModelInferenceJobsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListTrainedModelInferenceJobsRequestPaginateTypeDef


def get_value() -> ListTrainedModelInferenceJobsRequestPaginateTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# ListTrainedModelInferenceJobsRequestPaginateTypeDef definition

class ListTrainedModelInferenceJobsRequestPaginateTypeDef(TypedDict):
    membershipIdentifier: str,
    trainedModelArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTrainedModelsRequestPaginateTypeDef

```python
# ListTrainedModelsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListTrainedModelsRequestPaginateTypeDef


def get_value() -> ListTrainedModelsRequestPaginateTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# ListTrainedModelsRequestPaginateTypeDef definition

class ListTrainedModelsRequestPaginateTypeDef(TypedDict):
    membershipIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTrainingDatasetsRequestPaginateTypeDef

```python
# ListTrainingDatasetsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListTrainingDatasetsRequestPaginateTypeDef


def get_value() -> ListTrainingDatasetsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListTrainingDatasetsRequestPaginateTypeDef definition

class ListTrainingDatasetsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMLInputChannelsResponseTypeDef

```python
# ListMLInputChannelsResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListMLInputChannelsResponseTypeDef


def get_value() -> ListMLInputChannelsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListMLInputChannelsResponseTypeDef definition

class ListMLInputChannelsResponseTypeDef(TypedDict):
    mlInputChannelsList: List[MLInputChannelSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: MLInputChannelSummaryTypeDef](./type_defs.md#mlinputchannelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTrainedModelsResponseTypeDef

```python
# ListTrainedModelsResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListTrainedModelsResponseTypeDef


def get_value() -> ListTrainedModelsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListTrainedModelsResponseTypeDef definition

class ListTrainedModelsResponseTypeDef(TypedDict):
    trainedModels: List[TrainedModelSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TrainedModelSummaryTypeDef](./type_defs.md#trainedmodelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTrainingDatasetsResponseTypeDef

```python
# ListTrainingDatasetsResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListTrainingDatasetsResponseTypeDef


def get_value() -> ListTrainingDatasetsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListTrainingDatasetsResponseTypeDef definition

class ListTrainingDatasetsResponseTypeDef(TypedDict):
    trainingDatasets: List[TrainingDatasetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TrainingDatasetSummaryTypeDef](./type_defs.md#trainingdatasetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TrainedModelsConfigurationPolicyOutputTypeDef

```python
# TrainedModelsConfigurationPolicyOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import TrainedModelsConfigurationPolicyOutputTypeDef


def get_value() -> TrainedModelsConfigurationPolicyOutputTypeDef:
    return {
        "containerLogs": ...,
    }


# TrainedModelsConfigurationPolicyOutputTypeDef definition

class TrainedModelsConfigurationPolicyOutputTypeDef(TypedDict):
    containerLogs: NotRequired[List[LogsConfigurationPolicyOutputTypeDef]],  # (1)
    containerMetrics: NotRequired[MetricsConfigurationPolicyTypeDef],  # (2)
```

1. See [:material-code-braces: LogsConfigurationPolicyOutputTypeDef](./type_defs.md#logsconfigurationpolicyoutputtypedef) 
2. See [:material-code-braces: MetricsConfigurationPolicyTypeDef](./type_defs.md#metricsconfigurationpolicytypedef) 
## TrainedModelsConfigurationPolicyTypeDef

```python
# TrainedModelsConfigurationPolicyTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import TrainedModelsConfigurationPolicyTypeDef


def get_value() -> TrainedModelsConfigurationPolicyTypeDef:
    return {
        "containerLogs": ...,
    }


# TrainedModelsConfigurationPolicyTypeDef definition

class TrainedModelsConfigurationPolicyTypeDef(TypedDict):
    containerLogs: NotRequired[Sequence[LogsConfigurationPolicyTypeDef]],  # (1)
    containerMetrics: NotRequired[MetricsConfigurationPolicyTypeDef],  # (2)
```

1. See [:material-code-braces: LogsConfigurationPolicyTypeDef](./type_defs.md#logsconfigurationpolicytypedef) 
2. See [:material-code-braces: MetricsConfigurationPolicyTypeDef](./type_defs.md#metricsconfigurationpolicytypedef) 
## TrainedModelExportOutputConfigurationOutputTypeDef

```python
# TrainedModelExportOutputConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import TrainedModelExportOutputConfigurationOutputTypeDef


def get_value() -> TrainedModelExportOutputConfigurationOutputTypeDef:
    return {
        "members": ...,
    }


# TrainedModelExportOutputConfigurationOutputTypeDef definition

class TrainedModelExportOutputConfigurationOutputTypeDef(TypedDict):
    members: List[TrainedModelExportReceiverMemberTypeDef],  # (1)
```

1. See [:material-code-braces: TrainedModelExportReceiverMemberTypeDef](./type_defs.md#trainedmodelexportreceivermembertypedef) 
## TrainedModelExportOutputConfigurationTypeDef

```python
# TrainedModelExportOutputConfigurationTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import TrainedModelExportOutputConfigurationTypeDef


def get_value() -> TrainedModelExportOutputConfigurationTypeDef:
    return {
        "members": ...,
    }


# TrainedModelExportOutputConfigurationTypeDef definition

class TrainedModelExportOutputConfigurationTypeDef(TypedDict):
    members: Sequence[TrainedModelExportReceiverMemberTypeDef],  # (1)
```

1. See [:material-code-braces: TrainedModelExportReceiverMemberTypeDef](./type_defs.md#trainedmodelexportreceivermembertypedef) 
## TrainedModelExportsConfigurationPolicyOutputTypeDef

```python
# TrainedModelExportsConfigurationPolicyOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import TrainedModelExportsConfigurationPolicyOutputTypeDef


def get_value() -> TrainedModelExportsConfigurationPolicyOutputTypeDef:
    return {
        "maxSize": ...,
    }


# TrainedModelExportsConfigurationPolicyOutputTypeDef definition

class TrainedModelExportsConfigurationPolicyOutputTypeDef(TypedDict):
    maxSize: TrainedModelExportsMaxSizeTypeDef,  # (1)
    filesToExport: List[TrainedModelExportFileTypeType],  # (2)
```

1. See [:material-code-braces: TrainedModelExportsMaxSizeTypeDef](./type_defs.md#trainedmodelexportsmaxsizetypedef) 
2. See [:material-code-brackets: TrainedModelExportFileTypeType](./literals.md#trainedmodelexportfiletypetype) 
## TrainedModelExportsConfigurationPolicyTypeDef

```python
# TrainedModelExportsConfigurationPolicyTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import TrainedModelExportsConfigurationPolicyTypeDef


def get_value() -> TrainedModelExportsConfigurationPolicyTypeDef:
    return {
        "maxSize": ...,
    }


# TrainedModelExportsConfigurationPolicyTypeDef definition

class TrainedModelExportsConfigurationPolicyTypeDef(TypedDict):
    maxSize: TrainedModelExportsMaxSizeTypeDef,  # (1)
    filesToExport: Sequence[TrainedModelExportFileTypeType],  # (2)
```

1. See [:material-code-braces: TrainedModelExportsMaxSizeTypeDef](./type_defs.md#trainedmodelexportsmaxsizetypedef) 
2. See [:material-code-brackets: TrainedModelExportFileTypeType](./literals.md#trainedmodelexportfiletypetype) 
## TrainedModelInferenceJobsConfigurationPolicyOutputTypeDef

```python
# TrainedModelInferenceJobsConfigurationPolicyOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import TrainedModelInferenceJobsConfigurationPolicyOutputTypeDef


def get_value() -> TrainedModelInferenceJobsConfigurationPolicyOutputTypeDef:
    return {
        "containerLogs": ...,
    }


# TrainedModelInferenceJobsConfigurationPolicyOutputTypeDef definition

class TrainedModelInferenceJobsConfigurationPolicyOutputTypeDef(TypedDict):
    containerLogs: NotRequired[List[LogsConfigurationPolicyOutputTypeDef]],  # (1)
    maxOutputSize: NotRequired[TrainedModelInferenceMaxOutputSizeTypeDef],  # (2)
```

1. See [:material-code-braces: LogsConfigurationPolicyOutputTypeDef](./type_defs.md#logsconfigurationpolicyoutputtypedef) 
2. See [:material-code-braces: TrainedModelInferenceMaxOutputSizeTypeDef](./type_defs.md#trainedmodelinferencemaxoutputsizetypedef) 
## TrainedModelInferenceJobsConfigurationPolicyTypeDef

```python
# TrainedModelInferenceJobsConfigurationPolicyTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import TrainedModelInferenceJobsConfigurationPolicyTypeDef


def get_value() -> TrainedModelInferenceJobsConfigurationPolicyTypeDef:
    return {
        "containerLogs": ...,
    }


# TrainedModelInferenceJobsConfigurationPolicyTypeDef definition

class TrainedModelInferenceJobsConfigurationPolicyTypeDef(TypedDict):
    containerLogs: NotRequired[Sequence[LogsConfigurationPolicyTypeDef]],  # (1)
    maxOutputSize: NotRequired[TrainedModelInferenceMaxOutputSizeTypeDef],  # (2)
```

1. See [:material-code-braces: LogsConfigurationPolicyTypeDef](./type_defs.md#logsconfigurationpolicytypedef) 
2. See [:material-code-braces: TrainedModelInferenceMaxOutputSizeTypeDef](./type_defs.md#trainedmodelinferencemaxoutputsizetypedef) 
## ConfiguredAudienceModelOutputConfigTypeDef

```python
# ConfiguredAudienceModelOutputConfigTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ConfiguredAudienceModelOutputConfigTypeDef


def get_value() -> ConfiguredAudienceModelOutputConfigTypeDef:
    return {
        "destination": ...,
    }


# ConfiguredAudienceModelOutputConfigTypeDef definition

class ConfiguredAudienceModelOutputConfigTypeDef(TypedDict):
    destination: AudienceDestinationTypeDef,  # (1)
    roleArn: str,
```

1. See [:material-code-braces: AudienceDestinationTypeDef](./type_defs.md#audiencedestinationtypedef) 
## MLOutputConfigurationTypeDef

```python
# MLOutputConfigurationTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import MLOutputConfigurationTypeDef


def get_value() -> MLOutputConfigurationTypeDef:
    return {
        "destination": ...,
    }


# MLOutputConfigurationTypeDef definition

class MLOutputConfigurationTypeDef(TypedDict):
    roleArn: str,
    destination: NotRequired[DestinationTypeDef],  # (1)
```

1. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
## AudienceQualityMetricsTypeDef

```python
# AudienceQualityMetricsTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import AudienceQualityMetricsTypeDef


def get_value() -> AudienceQualityMetricsTypeDef:
    return {
        "relevanceMetrics": ...,
    }


# AudienceQualityMetricsTypeDef definition

class AudienceQualityMetricsTypeDef(TypedDict):
    relevanceMetrics: List[RelevanceMetricTypeDef],  # (1)
    recallMetric: NotRequired[float],
```

1. See [:material-code-braces: RelevanceMetricTypeDef](./type_defs.md#relevancemetrictypedef) 
## ListAudienceExportJobsResponseTypeDef

```python
# ListAudienceExportJobsResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListAudienceExportJobsResponseTypeDef


def get_value() -> ListAudienceExportJobsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListAudienceExportJobsResponseTypeDef definition

class ListAudienceExportJobsResponseTypeDef(TypedDict):
    audienceExportJobs: List[AudienceExportJobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AudienceExportJobSummaryTypeDef](./type_defs.md#audienceexportjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AudienceGenerationJobDataSourceOutputTypeDef

```python
# AudienceGenerationJobDataSourceOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import AudienceGenerationJobDataSourceOutputTypeDef


def get_value() -> AudienceGenerationJobDataSourceOutputTypeDef:
    return {
        "dataSource": ...,
    }


# AudienceGenerationJobDataSourceOutputTypeDef definition

class AudienceGenerationJobDataSourceOutputTypeDef(TypedDict):
    roleArn: str,
    dataSource: NotRequired[S3ConfigMapTypeDef],  # (1)
    sqlParameters: NotRequired[ProtectedQuerySQLParametersOutputTypeDef],  # (2)
    sqlComputeConfiguration: NotRequired[ComputeConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: S3ConfigMapTypeDef](./type_defs.md#s3configmaptypedef) 
2. See [:material-code-braces: ProtectedQuerySQLParametersOutputTypeDef](./type_defs.md#protectedquerysqlparametersoutputtypedef) 
3. See [:material-code-braces: ComputeConfigurationTypeDef](./type_defs.md#computeconfigurationtypedef) 
## AudienceGenerationJobDataSourceTypeDef

```python
# AudienceGenerationJobDataSourceTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import AudienceGenerationJobDataSourceTypeDef


def get_value() -> AudienceGenerationJobDataSourceTypeDef:
    return {
        "dataSource": ...,
    }


# AudienceGenerationJobDataSourceTypeDef definition

class AudienceGenerationJobDataSourceTypeDef(TypedDict):
    roleArn: str,
    dataSource: NotRequired[S3ConfigMapTypeDef],  # (1)
    sqlParameters: NotRequired[ProtectedQuerySQLParametersTypeDef],  # (2)
    sqlComputeConfiguration: NotRequired[ComputeConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: S3ConfigMapTypeDef](./type_defs.md#s3configmaptypedef) 
2. See [:material-code-braces: ProtectedQuerySQLParametersTypeDef](./type_defs.md#protectedquerysqlparameterstypedef) 
3. See [:material-code-braces: ComputeConfigurationTypeDef](./type_defs.md#computeconfigurationtypedef) 
## ProtectedQueryInputParametersOutputTypeDef

```python
# ProtectedQueryInputParametersOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ProtectedQueryInputParametersOutputTypeDef


def get_value() -> ProtectedQueryInputParametersOutputTypeDef:
    return {
        "sqlParameters": ...,
    }


# ProtectedQueryInputParametersOutputTypeDef definition

class ProtectedQueryInputParametersOutputTypeDef(TypedDict):
    sqlParameters: ProtectedQuerySQLParametersOutputTypeDef,  # (1)
    computeConfiguration: NotRequired[ComputeConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: ProtectedQuerySQLParametersOutputTypeDef](./type_defs.md#protectedquerysqlparametersoutputtypedef) 
2. See [:material-code-braces: ComputeConfigurationTypeDef](./type_defs.md#computeconfigurationtypedef) 
## ProtectedQueryInputParametersTypeDef

```python
# ProtectedQueryInputParametersTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ProtectedQueryInputParametersTypeDef


def get_value() -> ProtectedQueryInputParametersTypeDef:
    return {
        "sqlParameters": ...,
    }


# ProtectedQueryInputParametersTypeDef definition

class ProtectedQueryInputParametersTypeDef(TypedDict):
    sqlParameters: ProtectedQuerySQLParametersTypeDef,  # (1)
    computeConfiguration: NotRequired[ComputeConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: ProtectedQuerySQLParametersTypeDef](./type_defs.md#protectedquerysqlparameterstypedef) 
2. See [:material-code-braces: ComputeConfigurationTypeDef](./type_defs.md#computeconfigurationtypedef) 
## GetConfiguredModelAlgorithmResponseTypeDef

```python
# GetConfiguredModelAlgorithmResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import GetConfiguredModelAlgorithmResponseTypeDef


def get_value() -> GetConfiguredModelAlgorithmResponseTypeDef:
    return {
        "createTime": ...,
    }


# GetConfiguredModelAlgorithmResponseTypeDef definition

class GetConfiguredModelAlgorithmResponseTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    configuredModelAlgorithmArn: str,
    name: str,
    trainingContainerConfig: ContainerConfigOutputTypeDef,  # (1)
    inferenceContainerConfig: InferenceContainerConfigTypeDef,  # (2)
    roleArn: str,
    description: str,
    tags: Dict[str, str],
    kmsKeyArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ContainerConfigOutputTypeDef](./type_defs.md#containerconfigoutputtypedef) 
2. See [:material-code-braces: InferenceContainerConfigTypeDef](./type_defs.md#inferencecontainerconfigtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DatasetInputConfigOutputTypeDef

```python
# DatasetInputConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import DatasetInputConfigOutputTypeDef


def get_value() -> DatasetInputConfigOutputTypeDef:
    return {
        "schema": ...,
    }


# DatasetInputConfigOutputTypeDef definition

class DatasetInputConfigOutputTypeDef(TypedDict):
    schema: List[ColumnSchemaOutputTypeDef],  # (1)
    dataSource: DataSourceTypeDef,  # (2)
```

1. See [:material-code-braces: ColumnSchemaOutputTypeDef](./type_defs.md#columnschemaoutputtypedef) 
2. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
## DatasetInputConfigTypeDef

```python
# DatasetInputConfigTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import DatasetInputConfigTypeDef


def get_value() -> DatasetInputConfigTypeDef:
    return {
        "schema": ...,
    }


# DatasetInputConfigTypeDef definition

class DatasetInputConfigTypeDef(TypedDict):
    schema: Sequence[ColumnSchemaUnionTypeDef],  # (1)
    dataSource: DataSourceTypeDef,  # (2)
```

1. See [:material-code-braces: ColumnSchemaTypeDef](./type_defs.md#columnschematypedef) [:material-code-braces: ColumnSchemaOutputTypeDef](./type_defs.md#columnschemaoutputtypedef) 
2. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
## CollaborationTrainedModelInferenceJobSummaryTypeDef

```python
# CollaborationTrainedModelInferenceJobSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import CollaborationTrainedModelInferenceJobSummaryTypeDef


def get_value() -> CollaborationTrainedModelInferenceJobSummaryTypeDef:
    return {
        "trainedModelInferenceJobArn": ...,
    }


# CollaborationTrainedModelInferenceJobSummaryTypeDef definition

class CollaborationTrainedModelInferenceJobSummaryTypeDef(TypedDict):
    trainedModelInferenceJobArn: str,
    membershipIdentifier: str,
    trainedModelArn: str,
    collaborationIdentifier: str,
    status: TrainedModelInferenceJobStatusType,  # (1)
    outputConfiguration: InferenceOutputConfigurationOutputTypeDef,  # (2)
    name: str,
    createTime: datetime,
    updateTime: datetime,
    creatorAccountId: str,
    configuredModelAlgorithmAssociationArn: NotRequired[str],
    description: NotRequired[str],
    metricsStatus: NotRequired[MetricsStatusType],  # (3)
    metricsStatusDetails: NotRequired[str],
    logsStatus: NotRequired[LogsStatusType],  # (4)
    logsStatusDetails: NotRequired[str],
```

1. See [:material-code-brackets: TrainedModelInferenceJobStatusType](./literals.md#trainedmodelinferencejobstatustype) 
2. See [:material-code-braces: InferenceOutputConfigurationOutputTypeDef](./type_defs.md#inferenceoutputconfigurationoutputtypedef) 
3. See [:material-code-brackets: MetricsStatusType](./literals.md#metricsstatustype) 
4. See [:material-code-brackets: LogsStatusType](./literals.md#logsstatustype) 
## GetTrainedModelInferenceJobResponseTypeDef

```python
# GetTrainedModelInferenceJobResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import GetTrainedModelInferenceJobResponseTypeDef


def get_value() -> GetTrainedModelInferenceJobResponseTypeDef:
    return {
        "createTime": ...,
    }


# GetTrainedModelInferenceJobResponseTypeDef definition

class GetTrainedModelInferenceJobResponseTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    trainedModelInferenceJobArn: str,
    configuredModelAlgorithmAssociationArn: str,
    name: str,
    status: TrainedModelInferenceJobStatusType,  # (1)
    trainedModelArn: str,
    resourceConfig: InferenceResourceConfigTypeDef,  # (2)
    outputConfiguration: InferenceOutputConfigurationOutputTypeDef,  # (3)
    membershipIdentifier: str,
    dataSource: ModelInferenceDataSourceTypeDef,  # (4)
    containerExecutionParameters: InferenceContainerExecutionParametersTypeDef,  # (5)
    statusDetails: StatusDetailsTypeDef,  # (6)
    description: str,
    inferenceContainerImageDigest: str,
    environment: Dict[str, str],
    kmsKeyArn: str,
    metricsStatus: MetricsStatusType,  # (7)
    metricsStatusDetails: str,
    logsStatus: LogsStatusType,  # (8)
    logsStatusDetails: str,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (9)
```

1. See [:material-code-brackets: TrainedModelInferenceJobStatusType](./literals.md#trainedmodelinferencejobstatustype) 
2. See [:material-code-braces: InferenceResourceConfigTypeDef](./type_defs.md#inferenceresourceconfigtypedef) 
3. See [:material-code-braces: InferenceOutputConfigurationOutputTypeDef](./type_defs.md#inferenceoutputconfigurationoutputtypedef) 
4. See [:material-code-braces: ModelInferenceDataSourceTypeDef](./type_defs.md#modelinferencedatasourcetypedef) 
5. See [:material-code-braces: InferenceContainerExecutionParametersTypeDef](./type_defs.md#inferencecontainerexecutionparameterstypedef) 
6. See [:material-code-braces: StatusDetailsTypeDef](./type_defs.md#statusdetailstypedef) 
7. See [:material-code-brackets: MetricsStatusType](./literals.md#metricsstatustype) 
8. See [:material-code-brackets: LogsStatusType](./literals.md#logsstatustype) 
9. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TrainedModelInferenceJobSummaryTypeDef

```python
# TrainedModelInferenceJobSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import TrainedModelInferenceJobSummaryTypeDef


def get_value() -> TrainedModelInferenceJobSummaryTypeDef:
    return {
        "trainedModelInferenceJobArn": ...,
    }


# TrainedModelInferenceJobSummaryTypeDef definition

class TrainedModelInferenceJobSummaryTypeDef(TypedDict):
    trainedModelInferenceJobArn: str,
    membershipIdentifier: str,
    trainedModelArn: str,
    collaborationIdentifier: str,
    status: TrainedModelInferenceJobStatusType,  # (1)
    outputConfiguration: InferenceOutputConfigurationOutputTypeDef,  # (2)
    name: str,
    createTime: datetime,
    updateTime: datetime,
    configuredModelAlgorithmAssociationArn: NotRequired[str],
    description: NotRequired[str],
    metricsStatus: NotRequired[MetricsStatusType],  # (3)
    metricsStatusDetails: NotRequired[str],
    logsStatus: NotRequired[LogsStatusType],  # (4)
    logsStatusDetails: NotRequired[str],
```

1. See [:material-code-brackets: TrainedModelInferenceJobStatusType](./literals.md#trainedmodelinferencejobstatustype) 
2. See [:material-code-braces: InferenceOutputConfigurationOutputTypeDef](./type_defs.md#inferenceoutputconfigurationoutputtypedef) 
3. See [:material-code-brackets: MetricsStatusType](./literals.md#metricsstatustype) 
4. See [:material-code-brackets: LogsStatusType](./literals.md#logsstatustype) 
## CollaborationTrainedModelExportJobSummaryTypeDef

```python
# CollaborationTrainedModelExportJobSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import CollaborationTrainedModelExportJobSummaryTypeDef


def get_value() -> CollaborationTrainedModelExportJobSummaryTypeDef:
    return {
        "createTime": ...,
    }


# CollaborationTrainedModelExportJobSummaryTypeDef definition

class CollaborationTrainedModelExportJobSummaryTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    name: str,
    outputConfiguration: TrainedModelExportOutputConfigurationOutputTypeDef,  # (1)
    status: TrainedModelExportJobStatusType,  # (2)
    creatorAccountId: str,
    trainedModelArn: str,
    membershipIdentifier: str,
    collaborationIdentifier: str,
    statusDetails: NotRequired[StatusDetailsTypeDef],  # (3)
    description: NotRequired[str],
```

1. See [:material-code-braces: TrainedModelExportOutputConfigurationOutputTypeDef](./type_defs.md#trainedmodelexportoutputconfigurationoutputtypedef) 
2. See [:material-code-brackets: TrainedModelExportJobStatusType](./literals.md#trainedmodelexportjobstatustype) 
3. See [:material-code-braces: StatusDetailsTypeDef](./type_defs.md#statusdetailstypedef) 
## PrivacyConfigurationPoliciesOutputTypeDef

```python
# PrivacyConfigurationPoliciesOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import PrivacyConfigurationPoliciesOutputTypeDef


def get_value() -> PrivacyConfigurationPoliciesOutputTypeDef:
    return {
        "trainedModels": ...,
    }


# PrivacyConfigurationPoliciesOutputTypeDef definition

class PrivacyConfigurationPoliciesOutputTypeDef(TypedDict):
    trainedModels: NotRequired[TrainedModelsConfigurationPolicyOutputTypeDef],  # (1)
    trainedModelExports: NotRequired[TrainedModelExportsConfigurationPolicyOutputTypeDef],  # (2)
    trainedModelInferenceJobs: NotRequired[TrainedModelInferenceJobsConfigurationPolicyOutputTypeDef],  # (3)
```

1. See [:material-code-braces: TrainedModelsConfigurationPolicyOutputTypeDef](./type_defs.md#trainedmodelsconfigurationpolicyoutputtypedef) 
2. See [:material-code-braces: TrainedModelExportsConfigurationPolicyOutputTypeDef](./type_defs.md#trainedmodelexportsconfigurationpolicyoutputtypedef) 
3. See [:material-code-braces: TrainedModelInferenceJobsConfigurationPolicyOutputTypeDef](./type_defs.md#trainedmodelinferencejobsconfigurationpolicyoutputtypedef) 
## PrivacyConfigurationPoliciesTypeDef

```python
# PrivacyConfigurationPoliciesTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import PrivacyConfigurationPoliciesTypeDef


def get_value() -> PrivacyConfigurationPoliciesTypeDef:
    return {
        "trainedModels": ...,
    }


# PrivacyConfigurationPoliciesTypeDef definition

class PrivacyConfigurationPoliciesTypeDef(TypedDict):
    trainedModels: NotRequired[TrainedModelsConfigurationPolicyTypeDef],  # (1)
    trainedModelExports: NotRequired[TrainedModelExportsConfigurationPolicyTypeDef],  # (2)
    trainedModelInferenceJobs: NotRequired[TrainedModelInferenceJobsConfigurationPolicyTypeDef],  # (3)
```

1. See [:material-code-braces: TrainedModelsConfigurationPolicyTypeDef](./type_defs.md#trainedmodelsconfigurationpolicytypedef) 
2. See [:material-code-braces: TrainedModelExportsConfigurationPolicyTypeDef](./type_defs.md#trainedmodelexportsconfigurationpolicytypedef) 
3. See [:material-code-braces: TrainedModelInferenceJobsConfigurationPolicyTypeDef](./type_defs.md#trainedmodelinferencejobsconfigurationpolicytypedef) 
## ConfiguredAudienceModelSummaryTypeDef

```python
# ConfiguredAudienceModelSummaryTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ConfiguredAudienceModelSummaryTypeDef


def get_value() -> ConfiguredAudienceModelSummaryTypeDef:
    return {
        "createTime": ...,
    }


# ConfiguredAudienceModelSummaryTypeDef definition

class ConfiguredAudienceModelSummaryTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    name: str,
    audienceModelArn: str,
    outputConfig: ConfiguredAudienceModelOutputConfigTypeDef,  # (1)
    configuredAudienceModelArn: str,
    status: ConfiguredAudienceModelStatusType,  # (2)
    description: NotRequired[str],
```

1. See [:material-code-braces: ConfiguredAudienceModelOutputConfigTypeDef](./type_defs.md#configuredaudiencemodeloutputconfigtypedef) 
2. See [:material-code-brackets: ConfiguredAudienceModelStatusType](./literals.md#configuredaudiencemodelstatustype) 
## CreateConfiguredAudienceModelRequestTypeDef

```python
# CreateConfiguredAudienceModelRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import CreateConfiguredAudienceModelRequestTypeDef


def get_value() -> CreateConfiguredAudienceModelRequestTypeDef:
    return {
        "name": ...,
    }


# CreateConfiguredAudienceModelRequestTypeDef definition

class CreateConfiguredAudienceModelRequestTypeDef(TypedDict):
    name: str,
    audienceModelArn: str,
    outputConfig: ConfiguredAudienceModelOutputConfigTypeDef,  # (1)
    sharedAudienceMetrics: Sequence[SharedAudienceMetricsType],  # (2)
    description: NotRequired[str],
    minMatchingSeedSize: NotRequired[int],
    audienceSizeConfig: NotRequired[AudienceSizeConfigUnionTypeDef],  # (3)
    tags: NotRequired[Mapping[str, str]],
    childResourceTagOnCreatePolicy: NotRequired[TagOnCreatePolicyType],  # (4)
```

1. See [:material-code-braces: ConfiguredAudienceModelOutputConfigTypeDef](./type_defs.md#configuredaudiencemodeloutputconfigtypedef) 
2. See [:material-code-brackets: SharedAudienceMetricsType](./literals.md#sharedaudiencemetricstype) 
3. See [:material-code-braces: AudienceSizeConfigTypeDef](./type_defs.md#audiencesizeconfigtypedef) [:material-code-braces: AudienceSizeConfigOutputTypeDef](./type_defs.md#audiencesizeconfigoutputtypedef) 
4. See [:material-code-brackets: TagOnCreatePolicyType](./literals.md#tagoncreatepolicytype) 
## GetConfiguredAudienceModelResponseTypeDef

```python
# GetConfiguredAudienceModelResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import GetConfiguredAudienceModelResponseTypeDef


def get_value() -> GetConfiguredAudienceModelResponseTypeDef:
    return {
        "createTime": ...,
    }


# GetConfiguredAudienceModelResponseTypeDef definition

class GetConfiguredAudienceModelResponseTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    configuredAudienceModelArn: str,
    name: str,
    audienceModelArn: str,
    outputConfig: ConfiguredAudienceModelOutputConfigTypeDef,  # (1)
    description: str,
    status: ConfiguredAudienceModelStatusType,  # (2)
    sharedAudienceMetrics: List[SharedAudienceMetricsType],  # (3)
    minMatchingSeedSize: int,
    audienceSizeConfig: AudienceSizeConfigOutputTypeDef,  # (4)
    tags: Dict[str, str],
    childResourceTagOnCreatePolicy: TagOnCreatePolicyType,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: ConfiguredAudienceModelOutputConfigTypeDef](./type_defs.md#configuredaudiencemodeloutputconfigtypedef) 
2. See [:material-code-brackets: ConfiguredAudienceModelStatusType](./literals.md#configuredaudiencemodelstatustype) 
3. See [:material-code-brackets: SharedAudienceMetricsType](./literals.md#sharedaudiencemetricstype) 
4. See [:material-code-braces: AudienceSizeConfigOutputTypeDef](./type_defs.md#audiencesizeconfigoutputtypedef) 
5. See [:material-code-brackets: TagOnCreatePolicyType](./literals.md#tagoncreatepolicytype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateConfiguredAudienceModelRequestTypeDef

```python
# UpdateConfiguredAudienceModelRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import UpdateConfiguredAudienceModelRequestTypeDef


def get_value() -> UpdateConfiguredAudienceModelRequestTypeDef:
    return {
        "configuredAudienceModelArn": ...,
    }


# UpdateConfiguredAudienceModelRequestTypeDef definition

class UpdateConfiguredAudienceModelRequestTypeDef(TypedDict):
    configuredAudienceModelArn: str,
    outputConfig: NotRequired[ConfiguredAudienceModelOutputConfigTypeDef],  # (1)
    audienceModelArn: NotRequired[str],
    sharedAudienceMetrics: NotRequired[Sequence[SharedAudienceMetricsType]],  # (2)
    minMatchingSeedSize: NotRequired[int],
    audienceSizeConfig: NotRequired[AudienceSizeConfigUnionTypeDef],  # (3)
    description: NotRequired[str],
```

1. See [:material-code-braces: ConfiguredAudienceModelOutputConfigTypeDef](./type_defs.md#configuredaudiencemodeloutputconfigtypedef) 
2. See [:material-code-brackets: SharedAudienceMetricsType](./literals.md#sharedaudiencemetricstype) 
3. See [:material-code-braces: AudienceSizeConfigTypeDef](./type_defs.md#audiencesizeconfigtypedef) [:material-code-braces: AudienceSizeConfigOutputTypeDef](./type_defs.md#audiencesizeconfigoutputtypedef) 
## GetMLConfigurationResponseTypeDef

```python
# GetMLConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import GetMLConfigurationResponseTypeDef


def get_value() -> GetMLConfigurationResponseTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# GetMLConfigurationResponseTypeDef definition

class GetMLConfigurationResponseTypeDef(TypedDict):
    membershipIdentifier: str,
    defaultOutputLocation: MLOutputConfigurationTypeDef,  # (1)
    createTime: datetime,
    updateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MLOutputConfigurationTypeDef](./type_defs.md#mloutputconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutMLConfigurationRequestTypeDef

```python
# PutMLConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import PutMLConfigurationRequestTypeDef


def get_value() -> PutMLConfigurationRequestTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# PutMLConfigurationRequestTypeDef definition

class PutMLConfigurationRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    defaultOutputLocation: MLOutputConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: MLOutputConfigurationTypeDef](./type_defs.md#mloutputconfigurationtypedef) 
## GetAudienceGenerationJobResponseTypeDef

```python
# GetAudienceGenerationJobResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import GetAudienceGenerationJobResponseTypeDef


def get_value() -> GetAudienceGenerationJobResponseTypeDef:
    return {
        "createTime": ...,
    }


# GetAudienceGenerationJobResponseTypeDef definition

class GetAudienceGenerationJobResponseTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    audienceGenerationJobArn: str,
    name: str,
    description: str,
    status: AudienceGenerationJobStatusType,  # (1)
    statusDetails: StatusDetailsTypeDef,  # (2)
    configuredAudienceModelArn: str,
    seedAudience: AudienceGenerationJobDataSourceOutputTypeDef,  # (3)
    includeSeedInOutput: bool,
    collaborationId: str,
    metrics: AudienceQualityMetricsTypeDef,  # (4)
    startedBy: str,
    tags: Dict[str, str],
    protectedQueryIdentifier: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: AudienceGenerationJobStatusType](./literals.md#audiencegenerationjobstatustype) 
2. See [:material-code-braces: StatusDetailsTypeDef](./type_defs.md#statusdetailstypedef) 
3. See [:material-code-braces: AudienceGenerationJobDataSourceOutputTypeDef](./type_defs.md#audiencegenerationjobdatasourceoutputtypedef) 
4. See [:material-code-braces: AudienceQualityMetricsTypeDef](./type_defs.md#audiencequalitymetricstypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InputChannelDataSourceOutputTypeDef

```python
# InputChannelDataSourceOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import InputChannelDataSourceOutputTypeDef


def get_value() -> InputChannelDataSourceOutputTypeDef:
    return {
        "protectedQueryInputParameters": ...,
    }


# InputChannelDataSourceOutputTypeDef definition

class InputChannelDataSourceOutputTypeDef(TypedDict):
    protectedQueryInputParameters: NotRequired[ProtectedQueryInputParametersOutputTypeDef],  # (1)
```

1. See [:material-code-braces: ProtectedQueryInputParametersOutputTypeDef](./type_defs.md#protectedqueryinputparametersoutputtypedef) 
## InputChannelDataSourceTypeDef

```python
# InputChannelDataSourceTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import InputChannelDataSourceTypeDef


def get_value() -> InputChannelDataSourceTypeDef:
    return {
        "protectedQueryInputParameters": ...,
    }


# InputChannelDataSourceTypeDef definition

class InputChannelDataSourceTypeDef(TypedDict):
    protectedQueryInputParameters: NotRequired[ProtectedQueryInputParametersTypeDef],  # (1)
```

1. See [:material-code-braces: ProtectedQueryInputParametersTypeDef](./type_defs.md#protectedqueryinputparameterstypedef) 
## CreateConfiguredModelAlgorithmRequestTypeDef

```python
# CreateConfiguredModelAlgorithmRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import CreateConfiguredModelAlgorithmRequestTypeDef


def get_value() -> CreateConfiguredModelAlgorithmRequestTypeDef:
    return {
        "name": ...,
    }


# CreateConfiguredModelAlgorithmRequestTypeDef definition

class CreateConfiguredModelAlgorithmRequestTypeDef(TypedDict):
    name: str,
    roleArn: str,
    description: NotRequired[str],
    trainingContainerConfig: NotRequired[ContainerConfigUnionTypeDef],  # (1)
    inferenceContainerConfig: NotRequired[InferenceContainerConfigTypeDef],  # (2)
    tags: NotRequired[Mapping[str, str]],
    kmsKeyArn: NotRequired[str],
```

1. See [:material-code-braces: ContainerConfigTypeDef](./type_defs.md#containerconfigtypedef) [:material-code-braces: ContainerConfigOutputTypeDef](./type_defs.md#containerconfigoutputtypedef) 
2. See [:material-code-braces: InferenceContainerConfigTypeDef](./type_defs.md#inferencecontainerconfigtypedef) 
## DatasetOutputTypeDef

```python
# DatasetOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import DatasetOutputTypeDef


def get_value() -> DatasetOutputTypeDef:
    return {
        "type": ...,
    }


# DatasetOutputTypeDef definition

class DatasetOutputTypeDef(TypedDict):
    type: DatasetTypeType,  # (1)
    inputConfig: DatasetInputConfigOutputTypeDef,  # (2)
```

1. See [:material-code-brackets: DatasetTypeType](./literals.md#datasettypetype) 
2. See [:material-code-braces: DatasetInputConfigOutputTypeDef](./type_defs.md#datasetinputconfigoutputtypedef) 
## ListCollaborationTrainedModelInferenceJobsResponseTypeDef

```python
# ListCollaborationTrainedModelInferenceJobsResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListCollaborationTrainedModelInferenceJobsResponseTypeDef


def get_value() -> ListCollaborationTrainedModelInferenceJobsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListCollaborationTrainedModelInferenceJobsResponseTypeDef definition

class ListCollaborationTrainedModelInferenceJobsResponseTypeDef(TypedDict):
    collaborationTrainedModelInferenceJobs: List[CollaborationTrainedModelInferenceJobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CollaborationTrainedModelInferenceJobSummaryTypeDef](./type_defs.md#collaborationtrainedmodelinferencejobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTrainedModelInferenceJobsResponseTypeDef

```python
# ListTrainedModelInferenceJobsResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListTrainedModelInferenceJobsResponseTypeDef


def get_value() -> ListTrainedModelInferenceJobsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListTrainedModelInferenceJobsResponseTypeDef definition

class ListTrainedModelInferenceJobsResponseTypeDef(TypedDict):
    trainedModelInferenceJobs: List[TrainedModelInferenceJobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TrainedModelInferenceJobSummaryTypeDef](./type_defs.md#trainedmodelinferencejobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartTrainedModelInferenceJobRequestTypeDef

```python
# StartTrainedModelInferenceJobRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import StartTrainedModelInferenceJobRequestTypeDef


def get_value() -> StartTrainedModelInferenceJobRequestTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# StartTrainedModelInferenceJobRequestTypeDef definition

class StartTrainedModelInferenceJobRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    name: str,
    trainedModelArn: str,
    resourceConfig: InferenceResourceConfigTypeDef,  # (1)
    outputConfiguration: InferenceOutputConfigurationUnionTypeDef,  # (2)
    dataSource: ModelInferenceDataSourceTypeDef,  # (3)
    configuredModelAlgorithmAssociationArn: NotRequired[str],
    description: NotRequired[str],
    containerExecutionParameters: NotRequired[InferenceContainerExecutionParametersTypeDef],  # (4)
    environment: NotRequired[Mapping[str, str]],
    kmsKeyArn: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: InferenceResourceConfigTypeDef](./type_defs.md#inferenceresourceconfigtypedef) 
2. See [:material-code-braces: InferenceOutputConfigurationTypeDef](./type_defs.md#inferenceoutputconfigurationtypedef) [:material-code-braces: InferenceOutputConfigurationOutputTypeDef](./type_defs.md#inferenceoutputconfigurationoutputtypedef) 
3. See [:material-code-braces: ModelInferenceDataSourceTypeDef](./type_defs.md#modelinferencedatasourcetypedef) 
4. See [:material-code-braces: InferenceContainerExecutionParametersTypeDef](./type_defs.md#inferencecontainerexecutionparameterstypedef) 
## ListCollaborationTrainedModelExportJobsResponseTypeDef

```python
# ListCollaborationTrainedModelExportJobsResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListCollaborationTrainedModelExportJobsResponseTypeDef


def get_value() -> ListCollaborationTrainedModelExportJobsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListCollaborationTrainedModelExportJobsResponseTypeDef definition

class ListCollaborationTrainedModelExportJobsResponseTypeDef(TypedDict):
    collaborationTrainedModelExportJobs: List[CollaborationTrainedModelExportJobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CollaborationTrainedModelExportJobSummaryTypeDef](./type_defs.md#collaborationtrainedmodelexportjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartTrainedModelExportJobRequestTypeDef

```python
# StartTrainedModelExportJobRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import StartTrainedModelExportJobRequestTypeDef


def get_value() -> StartTrainedModelExportJobRequestTypeDef:
    return {
        "name": ...,
    }


# StartTrainedModelExportJobRequestTypeDef definition

class StartTrainedModelExportJobRequestTypeDef(TypedDict):
    name: str,
    trainedModelArn: str,
    membershipIdentifier: str,
    outputConfiguration: TrainedModelExportOutputConfigurationUnionTypeDef,  # (1)
    description: NotRequired[str],
```

1. See [:material-code-braces: TrainedModelExportOutputConfigurationTypeDef](./type_defs.md#trainedmodelexportoutputconfigurationtypedef) [:material-code-braces: TrainedModelExportOutputConfigurationOutputTypeDef](./type_defs.md#trainedmodelexportoutputconfigurationoutputtypedef) 
## PrivacyConfigurationOutputTypeDef

```python
# PrivacyConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import PrivacyConfigurationOutputTypeDef


def get_value() -> PrivacyConfigurationOutputTypeDef:
    return {
        "policies": ...,
    }


# PrivacyConfigurationOutputTypeDef definition

class PrivacyConfigurationOutputTypeDef(TypedDict):
    policies: PrivacyConfigurationPoliciesOutputTypeDef,  # (1)
```

1. See [:material-code-braces: PrivacyConfigurationPoliciesOutputTypeDef](./type_defs.md#privacyconfigurationpoliciesoutputtypedef) 
## PrivacyConfigurationTypeDef

```python
# PrivacyConfigurationTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import PrivacyConfigurationTypeDef


def get_value() -> PrivacyConfigurationTypeDef:
    return {
        "policies": ...,
    }


# PrivacyConfigurationTypeDef definition

class PrivacyConfigurationTypeDef(TypedDict):
    policies: PrivacyConfigurationPoliciesTypeDef,  # (1)
```

1. See [:material-code-braces: PrivacyConfigurationPoliciesTypeDef](./type_defs.md#privacyconfigurationpoliciestypedef) 
## ListConfiguredAudienceModelsResponseTypeDef

```python
# ListConfiguredAudienceModelsResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import ListConfiguredAudienceModelsResponseTypeDef


def get_value() -> ListConfiguredAudienceModelsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListConfiguredAudienceModelsResponseTypeDef definition

class ListConfiguredAudienceModelsResponseTypeDef(TypedDict):
    configuredAudienceModels: List[ConfiguredAudienceModelSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ConfiguredAudienceModelSummaryTypeDef](./type_defs.md#configuredaudiencemodelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartAudienceGenerationJobRequestTypeDef

```python
# StartAudienceGenerationJobRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import StartAudienceGenerationJobRequestTypeDef


def get_value() -> StartAudienceGenerationJobRequestTypeDef:
    return {
        "name": ...,
    }


# StartAudienceGenerationJobRequestTypeDef definition

class StartAudienceGenerationJobRequestTypeDef(TypedDict):
    name: str,
    configuredAudienceModelArn: str,
    seedAudience: AudienceGenerationJobDataSourceUnionTypeDef,  # (1)
    includeSeedInOutput: NotRequired[bool],
    collaborationId: NotRequired[str],
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AudienceGenerationJobDataSourceTypeDef](./type_defs.md#audiencegenerationjobdatasourcetypedef) [:material-code-braces: AudienceGenerationJobDataSourceOutputTypeDef](./type_defs.md#audiencegenerationjobdatasourceoutputtypedef) 
## InputChannelOutputTypeDef

```python
# InputChannelOutputTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import InputChannelOutputTypeDef


def get_value() -> InputChannelOutputTypeDef:
    return {
        "dataSource": ...,
    }


# InputChannelOutputTypeDef definition

class InputChannelOutputTypeDef(TypedDict):
    dataSource: InputChannelDataSourceOutputTypeDef,  # (1)
    roleArn: str,
```

1. See [:material-code-braces: InputChannelDataSourceOutputTypeDef](./type_defs.md#inputchanneldatasourceoutputtypedef) 
## InputChannelTypeDef

```python
# InputChannelTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import InputChannelTypeDef


def get_value() -> InputChannelTypeDef:
    return {
        "dataSource": ...,
    }


# InputChannelTypeDef definition

class InputChannelTypeDef(TypedDict):
    dataSource: InputChannelDataSourceTypeDef,  # (1)
    roleArn: str,
```

1. See [:material-code-braces: InputChannelDataSourceTypeDef](./type_defs.md#inputchanneldatasourcetypedef) 
## GetTrainingDatasetResponseTypeDef

```python
# GetTrainingDatasetResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import GetTrainingDatasetResponseTypeDef


def get_value() -> GetTrainingDatasetResponseTypeDef:
    return {
        "createTime": ...,
    }


# GetTrainingDatasetResponseTypeDef definition

class GetTrainingDatasetResponseTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    trainingDatasetArn: str,
    name: str,
    trainingData: List[DatasetOutputTypeDef],  # (1)
    status: TrainingDatasetStatusType,  # (2)
    roleArn: str,
    tags: Dict[str, str],
    description: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: DatasetOutputTypeDef](./type_defs.md#datasetoutputtypedef) 
2. See [:material-code-brackets: TrainingDatasetStatusType](./literals.md#trainingdatasetstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DatasetTypeDef

```python
# DatasetTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import DatasetTypeDef


def get_value() -> DatasetTypeDef:
    return {
        "type": ...,
    }


# DatasetTypeDef definition

class DatasetTypeDef(TypedDict):
    type: DatasetTypeType,  # (1)
    inputConfig: DatasetInputConfigUnionTypeDef,  # (2)
```

1. See [:material-code-brackets: DatasetTypeType](./literals.md#datasettypetype) 
2. See [:material-code-braces: DatasetInputConfigTypeDef](./type_defs.md#datasetinputconfigtypedef) [:material-code-braces: DatasetInputConfigOutputTypeDef](./type_defs.md#datasetinputconfigoutputtypedef) 
## GetCollaborationConfiguredModelAlgorithmAssociationResponseTypeDef

```python
# GetCollaborationConfiguredModelAlgorithmAssociationResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import GetCollaborationConfiguredModelAlgorithmAssociationResponseTypeDef


def get_value() -> GetCollaborationConfiguredModelAlgorithmAssociationResponseTypeDef:
    return {
        "createTime": ...,
    }


# GetCollaborationConfiguredModelAlgorithmAssociationResponseTypeDef definition

class GetCollaborationConfiguredModelAlgorithmAssociationResponseTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    configuredModelAlgorithmAssociationArn: str,
    membershipIdentifier: str,
    collaborationIdentifier: str,
    configuredModelAlgorithmArn: str,
    name: str,
    description: str,
    creatorAccountId: str,
    privacyConfiguration: PrivacyConfigurationOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PrivacyConfigurationOutputTypeDef](./type_defs.md#privacyconfigurationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConfiguredModelAlgorithmAssociationResponseTypeDef

```python
# GetConfiguredModelAlgorithmAssociationResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import GetConfiguredModelAlgorithmAssociationResponseTypeDef


def get_value() -> GetConfiguredModelAlgorithmAssociationResponseTypeDef:
    return {
        "createTime": ...,
    }


# GetConfiguredModelAlgorithmAssociationResponseTypeDef definition

class GetConfiguredModelAlgorithmAssociationResponseTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    configuredModelAlgorithmAssociationArn: str,
    membershipIdentifier: str,
    collaborationIdentifier: str,
    configuredModelAlgorithmArn: str,
    name: str,
    privacyConfiguration: PrivacyConfigurationOutputTypeDef,  # (1)
    description: str,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PrivacyConfigurationOutputTypeDef](./type_defs.md#privacyconfigurationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMLInputChannelResponseTypeDef

```python
# GetMLInputChannelResponseTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import GetMLInputChannelResponseTypeDef


def get_value() -> GetMLInputChannelResponseTypeDef:
    return {
        "createTime": ...,
    }


# GetMLInputChannelResponseTypeDef definition

class GetMLInputChannelResponseTypeDef(TypedDict):
    createTime: datetime,
    updateTime: datetime,
    membershipIdentifier: str,
    collaborationIdentifier: str,
    inputChannel: InputChannelOutputTypeDef,  # (1)
    protectedQueryIdentifier: str,
    mlInputChannelArn: str,
    name: str,
    configuredModelAlgorithmAssociations: List[str],
    status: MLInputChannelStatusType,  # (2)
    statusDetails: StatusDetailsTypeDef,  # (3)
    retentionInDays: int,
    numberOfRecords: int,
    numberOfFiles: float,
    sizeInGb: float,
    description: str,
    kmsKeyArn: str,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: InputChannelOutputTypeDef](./type_defs.md#inputchanneloutputtypedef) 
2. See [:material-code-brackets: MLInputChannelStatusType](./literals.md#mlinputchannelstatustype) 
3. See [:material-code-braces: StatusDetailsTypeDef](./type_defs.md#statusdetailstypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConfiguredModelAlgorithmAssociationRequestTypeDef

```python
# CreateConfiguredModelAlgorithmAssociationRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import CreateConfiguredModelAlgorithmAssociationRequestTypeDef


def get_value() -> CreateConfiguredModelAlgorithmAssociationRequestTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# CreateConfiguredModelAlgorithmAssociationRequestTypeDef definition

class CreateConfiguredModelAlgorithmAssociationRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    configuredModelAlgorithmArn: str,
    name: str,
    description: NotRequired[str],
    privacyConfiguration: NotRequired[PrivacyConfigurationUnionTypeDef],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: PrivacyConfigurationTypeDef](./type_defs.md#privacyconfigurationtypedef) [:material-code-braces: PrivacyConfigurationOutputTypeDef](./type_defs.md#privacyconfigurationoutputtypedef) 
## CreateMLInputChannelRequestTypeDef

```python
# CreateMLInputChannelRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import CreateMLInputChannelRequestTypeDef


def get_value() -> CreateMLInputChannelRequestTypeDef:
    return {
        "membershipIdentifier": ...,
    }


# CreateMLInputChannelRequestTypeDef definition

class CreateMLInputChannelRequestTypeDef(TypedDict):
    membershipIdentifier: str,
    configuredModelAlgorithmAssociations: Sequence[str],
    inputChannel: InputChannelUnionTypeDef,  # (1)
    name: str,
    retentionInDays: int,
    description: NotRequired[str],
    kmsKeyArn: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: InputChannelTypeDef](./type_defs.md#inputchanneltypedef) [:material-code-braces: InputChannelOutputTypeDef](./type_defs.md#inputchanneloutputtypedef) 
## CreateTrainingDatasetRequestTypeDef

```python
# CreateTrainingDatasetRequestTypeDef TypedDict usage example

from types_aiobotocore_cleanroomsml.type_defs import CreateTrainingDatasetRequestTypeDef


def get_value() -> CreateTrainingDatasetRequestTypeDef:
    return {
        "name": ...,
    }


# CreateTrainingDatasetRequestTypeDef definition

class CreateTrainingDatasetRequestTypeDef(TypedDict):
    name: str,
    roleArn: str,
    trainingData: Sequence[DatasetUnionTypeDef],  # (1)
    tags: NotRequired[Mapping[str, str]],
    description: NotRequired[str],
```

1. See [:material-code-braces: DatasetTypeDef](./type_defs.md#datasettypedef) [:material-code-braces: DatasetOutputTypeDef](./type_defs.md#datasetoutputtypedef) 
