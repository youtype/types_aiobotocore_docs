# Type definitions

> [Index](../README.md) > [Bedrock](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Bedrock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#bedrock)
    type annotations stubs module [types-aiobotocore-bedrock](https://pypi.org/project/types-aiobotocore-bedrock/).

## BlobTypeDef

```python
# BlobTypeDef Union usage example

from types_aiobotocore_bedrock.type_defs import BlobTypeDef


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


## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_bedrock.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## VpcConfigUnionTypeDef

```python
# VpcConfigUnionTypeDef Union usage example

from types_aiobotocore_bedrock.type_defs import VpcConfigUnionTypeDef


def get_value() -> VpcConfigUnionTypeDef:
    return ...


# VpcConfigUnionTypeDef definition

VpcConfigUnionTypeDef = Union[
    VpcConfigTypeDef,  # (1)
    VpcConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
2. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 

## ValidationDataConfigUnionTypeDef

```python
# ValidationDataConfigUnionTypeDef Union usage example

from types_aiobotocore_bedrock.type_defs import ValidationDataConfigUnionTypeDef


def get_value() -> ValidationDataConfigUnionTypeDef:
    return ...


# ValidationDataConfigUnionTypeDef definition

ValidationDataConfigUnionTypeDef = Union[
    ValidationDataConfigTypeDef,  # (1)
    ValidationDataConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ValidationDataConfigTypeDef](./type_defs.md#validationdataconfigtypedef) 
2. See [:material-code-braces: ValidationDataConfigOutputTypeDef](./type_defs.md#validationdataconfigoutputtypedef) 

## EndpointConfigUnionTypeDef

```python
# EndpointConfigUnionTypeDef Union usage example

from types_aiobotocore_bedrock.type_defs import EndpointConfigUnionTypeDef


def get_value() -> EndpointConfigUnionTypeDef:
    return ...


# EndpointConfigUnionTypeDef definition

EndpointConfigUnionTypeDef = Union[
    EndpointConfigTypeDef,  # (1)
    EndpointConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EndpointConfigTypeDef](./type_defs.md#endpointconfigtypedef) 
2. See [:material-code-braces: EndpointConfigOutputTypeDef](./type_defs.md#endpointconfigoutputtypedef) 

## TrainingDataConfigUnionTypeDef

```python
# TrainingDataConfigUnionTypeDef Union usage example

from types_aiobotocore_bedrock.type_defs import TrainingDataConfigUnionTypeDef


def get_value() -> TrainingDataConfigUnionTypeDef:
    return ...


# TrainingDataConfigUnionTypeDef definition

TrainingDataConfigUnionTypeDef = Union[
    TrainingDataConfigTypeDef,  # (1)
    TrainingDataConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TrainingDataConfigTypeDef](./type_defs.md#trainingdataconfigtypedef) 
2. See [:material-code-braces: TrainingDataConfigOutputTypeDef](./type_defs.md#trainingdataconfigoutputtypedef) 

## EvaluationConfigUnionTypeDef

```python
# EvaluationConfigUnionTypeDef Union usage example

from types_aiobotocore_bedrock.type_defs import EvaluationConfigUnionTypeDef


def get_value() -> EvaluationConfigUnionTypeDef:
    return ...


# EvaluationConfigUnionTypeDef definition

EvaluationConfigUnionTypeDef = Union[
    EvaluationConfigTypeDef,  # (1)
    EvaluationConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EvaluationConfigTypeDef](./type_defs.md#evaluationconfigtypedef) 
2. See [:material-code-braces: EvaluationConfigOutputTypeDef](./type_defs.md#evaluationconfigoutputtypedef) 

## EvaluationInferenceConfigUnionTypeDef

```python
# EvaluationInferenceConfigUnionTypeDef Union usage example

from types_aiobotocore_bedrock.type_defs import EvaluationInferenceConfigUnionTypeDef


def get_value() -> EvaluationInferenceConfigUnionTypeDef:
    return ...


# EvaluationInferenceConfigUnionTypeDef definition

EvaluationInferenceConfigUnionTypeDef = Union[
    EvaluationInferenceConfigTypeDef,  # (1)
    EvaluationInferenceConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EvaluationInferenceConfigTypeDef](./type_defs.md#evaluationinferenceconfigtypedef) 
2. See [:material-code-braces: EvaluationInferenceConfigOutputTypeDef](./type_defs.md#evaluationinferenceconfigoutputtypedef) 



## BatchDeleteEvaluationJobErrorTypeDef

```python
# BatchDeleteEvaluationJobErrorTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import BatchDeleteEvaluationJobErrorTypeDef


def get_value() -> BatchDeleteEvaluationJobErrorTypeDef:
    return {
        "jobIdentifier": ...,
    }


# BatchDeleteEvaluationJobErrorTypeDef definition

class BatchDeleteEvaluationJobErrorTypeDef(TypedDict):
    jobIdentifier: str,
    code: str,
    message: NotRequired[str],
```

## BatchDeleteEvaluationJobItemTypeDef

```python
# BatchDeleteEvaluationJobItemTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import BatchDeleteEvaluationJobItemTypeDef


def get_value() -> BatchDeleteEvaluationJobItemTypeDef:
    return {
        "jobIdentifier": ...,
    }


# BatchDeleteEvaluationJobItemTypeDef definition

class BatchDeleteEvaluationJobItemTypeDef(TypedDict):
    jobIdentifier: str,
    jobStatus: EvaluationJobStatusType,  # (1)
```

1. See [:material-code-brackets: EvaluationJobStatusType](./literals.md#evaluationjobstatustype) 
## BatchDeleteEvaluationJobRequestTypeDef

```python
# BatchDeleteEvaluationJobRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import BatchDeleteEvaluationJobRequestTypeDef


def get_value() -> BatchDeleteEvaluationJobRequestTypeDef:
    return {
        "jobIdentifiers": ...,
    }


# BatchDeleteEvaluationJobRequestTypeDef definition

class BatchDeleteEvaluationJobRequestTypeDef(TypedDict):
    jobIdentifiers: Sequence[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ResponseMetadataTypeDef


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

## BedrockEvaluatorModelTypeDef

```python
# BedrockEvaluatorModelTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import BedrockEvaluatorModelTypeDef


def get_value() -> BedrockEvaluatorModelTypeDef:
    return {
        "modelIdentifier": ...,
    }


# BedrockEvaluatorModelTypeDef definition

class BedrockEvaluatorModelTypeDef(TypedDict):
    modelIdentifier: str,
```

## ByteContentDocOutputTypeDef

```python
# ByteContentDocOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ByteContentDocOutputTypeDef


def get_value() -> ByteContentDocOutputTypeDef:
    return {
        "identifier": ...,
    }


# ByteContentDocOutputTypeDef definition

class ByteContentDocOutputTypeDef(TypedDict):
    identifier: str,
    contentType: str,
    data: bytes,
```

## S3ConfigTypeDef

```python
# S3ConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import S3ConfigTypeDef


def get_value() -> S3ConfigTypeDef:
    return {
        "bucketName": ...,
    }


# S3ConfigTypeDef definition

class S3ConfigTypeDef(TypedDict):
    bucketName: str,
    keyPrefix: NotRequired[str],
```

## EvaluationOutputDataConfigTypeDef

```python
# EvaluationOutputDataConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import EvaluationOutputDataConfigTypeDef


def get_value() -> EvaluationOutputDataConfigTypeDef:
    return {
        "s3Uri": ...,
    }


# EvaluationOutputDataConfigTypeDef definition

class EvaluationOutputDataConfigTypeDef(TypedDict):
    s3Uri: str,
```

## TagTypeDef

```python
# TagTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import TagTypeDef


def get_value() -> TagTypeDef:
    return {
        "key": ...,
    }


# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: str,
    value: str,
```

## CreateGuardrailVersionRequestTypeDef

```python
# CreateGuardrailVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import CreateGuardrailVersionRequestTypeDef


def get_value() -> CreateGuardrailVersionRequestTypeDef:
    return {
        "guardrailIdentifier": ...,
    }


# CreateGuardrailVersionRequestTypeDef definition

class CreateGuardrailVersionRequestTypeDef(TypedDict):
    guardrailIdentifier: str,
    description: NotRequired[str],
    clientRequestToken: NotRequired[str],
```

## InferenceProfileModelSourceTypeDef

```python
# InferenceProfileModelSourceTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import InferenceProfileModelSourceTypeDef


def get_value() -> InferenceProfileModelSourceTypeDef:
    return {
        "copyFrom": ...,
    }


# InferenceProfileModelSourceTypeDef definition

class InferenceProfileModelSourceTypeDef(TypedDict):
    copyFrom: NotRequired[str],
```

## OutputDataConfigTypeDef

```python
# OutputDataConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import OutputDataConfigTypeDef


def get_value() -> OutputDataConfigTypeDef:
    return {
        "s3Uri": ...,
    }


# OutputDataConfigTypeDef definition

class OutputDataConfigTypeDef(TypedDict):
    s3Uri: str,
```

## CustomModelSummaryTypeDef

```python
# CustomModelSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import CustomModelSummaryTypeDef


def get_value() -> CustomModelSummaryTypeDef:
    return {
        "modelArn": ...,
    }


# CustomModelSummaryTypeDef definition

class CustomModelSummaryTypeDef(TypedDict):
    modelArn: str,
    modelName: str,
    creationTime: datetime,
    baseModelArn: str,
    baseModelName: str,
    customizationType: NotRequired[CustomizationTypeType],  # (1)
    ownerAccountId: NotRequired[str],
```

1. See [:material-code-brackets: CustomizationTypeType](./literals.md#customizationtypetype) 
## DeleteCustomModelRequestTypeDef

```python
# DeleteCustomModelRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import DeleteCustomModelRequestTypeDef


def get_value() -> DeleteCustomModelRequestTypeDef:
    return {
        "modelIdentifier": ...,
    }


# DeleteCustomModelRequestTypeDef definition

class DeleteCustomModelRequestTypeDef(TypedDict):
    modelIdentifier: str,
```

## DeleteGuardrailRequestTypeDef

```python
# DeleteGuardrailRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import DeleteGuardrailRequestTypeDef


def get_value() -> DeleteGuardrailRequestTypeDef:
    return {
        "guardrailIdentifier": ...,
    }


# DeleteGuardrailRequestTypeDef definition

class DeleteGuardrailRequestTypeDef(TypedDict):
    guardrailIdentifier: str,
    guardrailVersion: NotRequired[str],
```

## DeleteImportedModelRequestTypeDef

```python
# DeleteImportedModelRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import DeleteImportedModelRequestTypeDef


def get_value() -> DeleteImportedModelRequestTypeDef:
    return {
        "modelIdentifier": ...,
    }


# DeleteImportedModelRequestTypeDef definition

class DeleteImportedModelRequestTypeDef(TypedDict):
    modelIdentifier: str,
```

## DeleteInferenceProfileRequestTypeDef

```python
# DeleteInferenceProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import DeleteInferenceProfileRequestTypeDef


def get_value() -> DeleteInferenceProfileRequestTypeDef:
    return {
        "inferenceProfileIdentifier": ...,
    }


# DeleteInferenceProfileRequestTypeDef definition

class DeleteInferenceProfileRequestTypeDef(TypedDict):
    inferenceProfileIdentifier: str,
```

## DeleteMarketplaceModelEndpointRequestTypeDef

```python
# DeleteMarketplaceModelEndpointRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import DeleteMarketplaceModelEndpointRequestTypeDef


def get_value() -> DeleteMarketplaceModelEndpointRequestTypeDef:
    return {
        "endpointArn": ...,
    }


# DeleteMarketplaceModelEndpointRequestTypeDef definition

class DeleteMarketplaceModelEndpointRequestTypeDef(TypedDict):
    endpointArn: str,
```

## DeleteProvisionedModelThroughputRequestTypeDef

```python
# DeleteProvisionedModelThroughputRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import DeleteProvisionedModelThroughputRequestTypeDef


def get_value() -> DeleteProvisionedModelThroughputRequestTypeDef:
    return {
        "provisionedModelId": ...,
    }


# DeleteProvisionedModelThroughputRequestTypeDef definition

class DeleteProvisionedModelThroughputRequestTypeDef(TypedDict):
    provisionedModelId: str,
```

## DeregisterMarketplaceModelEndpointRequestTypeDef

```python
# DeregisterMarketplaceModelEndpointRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import DeregisterMarketplaceModelEndpointRequestTypeDef


def get_value() -> DeregisterMarketplaceModelEndpointRequestTypeDef:
    return {
        "endpointArn": ...,
    }


# DeregisterMarketplaceModelEndpointRequestTypeDef definition

class DeregisterMarketplaceModelEndpointRequestTypeDef(TypedDict):
    endpointArn: str,
```

## TeacherModelConfigTypeDef

```python
# TeacherModelConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import TeacherModelConfigTypeDef


def get_value() -> TeacherModelConfigTypeDef:
    return {
        "teacherModelIdentifier": ...,
    }


# TeacherModelConfigTypeDef definition

class TeacherModelConfigTypeDef(TypedDict):
    teacherModelIdentifier: str,
    maxResponseLengthForInference: NotRequired[int],
```

## PerformanceConfigurationTypeDef

```python
# PerformanceConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import PerformanceConfigurationTypeDef


def get_value() -> PerformanceConfigurationTypeDef:
    return {
        "latency": ...,
    }


# PerformanceConfigurationTypeDef definition

class PerformanceConfigurationTypeDef(TypedDict):
    latency: NotRequired[PerformanceConfigLatencyType],  # (1)
```

1. See [:material-code-brackets: PerformanceConfigLatencyType](./literals.md#performanceconfiglatencytype) 
## EvaluationDatasetLocationTypeDef

```python
# EvaluationDatasetLocationTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import EvaluationDatasetLocationTypeDef


def get_value() -> EvaluationDatasetLocationTypeDef:
    return {
        "s3Uri": ...,
    }


# EvaluationDatasetLocationTypeDef definition

class EvaluationDatasetLocationTypeDef(TypedDict):
    s3Uri: NotRequired[str],
```

## EvaluationSummaryTypeDef

```python
# EvaluationSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import EvaluationSummaryTypeDef


def get_value() -> EvaluationSummaryTypeDef:
    return {
        "jobArn": ...,
    }


# EvaluationSummaryTypeDef definition

class EvaluationSummaryTypeDef(TypedDict):
    jobArn: str,
    jobName: str,
    status: EvaluationJobStatusType,  # (1)
    creationTime: datetime,
    jobType: EvaluationJobTypeType,  # (2)
    evaluationTaskTypes: List[EvaluationTaskTypeType],  # (3)
    modelIdentifiers: NotRequired[List[str]],
    ragIdentifiers: NotRequired[List[str]],
    evaluatorModelIdentifiers: NotRequired[List[str]],
    applicationType: NotRequired[ApplicationTypeType],  # (4)
```

1. See [:material-code-brackets: EvaluationJobStatusType](./literals.md#evaluationjobstatustype) 
2. See [:material-code-brackets: EvaluationJobTypeType](./literals.md#evaluationjobtypetype) 
3. See [:material-code-brackets: EvaluationTaskTypeType](./literals.md#evaluationtasktypetype) 
4. See [:material-code-brackets: ApplicationTypeType](./literals.md#applicationtypetype) 
## S3ObjectDocTypeDef

```python
# S3ObjectDocTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import S3ObjectDocTypeDef


def get_value() -> S3ObjectDocTypeDef:
    return {
        "uri": ...,
    }


# S3ObjectDocTypeDef definition

class S3ObjectDocTypeDef(TypedDict):
    uri: str,
```

## GuardrailConfigurationTypeDef

```python
# GuardrailConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GuardrailConfigurationTypeDef


def get_value() -> GuardrailConfigurationTypeDef:
    return {
        "guardrailId": ...,
    }


# GuardrailConfigurationTypeDef definition

class GuardrailConfigurationTypeDef(TypedDict):
    guardrailId: str,
    guardrailVersion: str,
```

## PromptTemplateTypeDef

```python
# PromptTemplateTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import PromptTemplateTypeDef


def get_value() -> PromptTemplateTypeDef:
    return {
        "textPromptTemplate": ...,
    }


# PromptTemplateTypeDef definition

class PromptTemplateTypeDef(TypedDict):
    textPromptTemplate: NotRequired[str],
```

## FilterAttributeOutputTypeDef

```python
# FilterAttributeOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import FilterAttributeOutputTypeDef


def get_value() -> FilterAttributeOutputTypeDef:
    return {
        "key": ...,
    }


# FilterAttributeOutputTypeDef definition

class FilterAttributeOutputTypeDef(TypedDict):
    key: str,
    value: Dict[str, Any],
```

## FilterAttributeTypeDef

```python
# FilterAttributeTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import FilterAttributeTypeDef


def get_value() -> FilterAttributeTypeDef:
    return {
        "key": ...,
    }


# FilterAttributeTypeDef definition

class FilterAttributeTypeDef(TypedDict):
    key: str,
    value: Mapping[str, Any],
```

## FoundationModelLifecycleTypeDef

```python
# FoundationModelLifecycleTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import FoundationModelLifecycleTypeDef


def get_value() -> FoundationModelLifecycleTypeDef:
    return {
        "status": ...,
    }


# FoundationModelLifecycleTypeDef definition

class FoundationModelLifecycleTypeDef(TypedDict):
    status: FoundationModelLifecycleStatusType,  # (1)
```

1. See [:material-code-brackets: FoundationModelLifecycleStatusType](./literals.md#foundationmodellifecyclestatustype) 
## GetCustomModelRequestTypeDef

```python
# GetCustomModelRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GetCustomModelRequestTypeDef


def get_value() -> GetCustomModelRequestTypeDef:
    return {
        "modelIdentifier": ...,
    }


# GetCustomModelRequestTypeDef definition

class GetCustomModelRequestTypeDef(TypedDict):
    modelIdentifier: str,
```

## TrainingMetricsTypeDef

```python
# TrainingMetricsTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import TrainingMetricsTypeDef


def get_value() -> TrainingMetricsTypeDef:
    return {
        "trainingLoss": ...,
    }


# TrainingMetricsTypeDef definition

class TrainingMetricsTypeDef(TypedDict):
    trainingLoss: NotRequired[float],
```

## ValidatorMetricTypeDef

```python
# ValidatorMetricTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ValidatorMetricTypeDef


def get_value() -> ValidatorMetricTypeDef:
    return {
        "validationLoss": ...,
    }


# ValidatorMetricTypeDef definition

class ValidatorMetricTypeDef(TypedDict):
    validationLoss: NotRequired[float],
```

## GetEvaluationJobRequestTypeDef

```python
# GetEvaluationJobRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GetEvaluationJobRequestTypeDef


def get_value() -> GetEvaluationJobRequestTypeDef:
    return {
        "jobIdentifier": ...,
    }


# GetEvaluationJobRequestTypeDef definition

class GetEvaluationJobRequestTypeDef(TypedDict):
    jobIdentifier: str,
```

## GetFoundationModelRequestTypeDef

```python
# GetFoundationModelRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GetFoundationModelRequestTypeDef


def get_value() -> GetFoundationModelRequestTypeDef:
    return {
        "modelIdentifier": ...,
    }


# GetFoundationModelRequestTypeDef definition

class GetFoundationModelRequestTypeDef(TypedDict):
    modelIdentifier: str,
```

## GetGuardrailRequestTypeDef

```python
# GetGuardrailRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GetGuardrailRequestTypeDef


def get_value() -> GetGuardrailRequestTypeDef:
    return {
        "guardrailIdentifier": ...,
    }


# GetGuardrailRequestTypeDef definition

class GetGuardrailRequestTypeDef(TypedDict):
    guardrailIdentifier: str,
    guardrailVersion: NotRequired[str],
```

## GetImportedModelRequestTypeDef

```python
# GetImportedModelRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GetImportedModelRequestTypeDef


def get_value() -> GetImportedModelRequestTypeDef:
    return {
        "modelIdentifier": ...,
    }


# GetImportedModelRequestTypeDef definition

class GetImportedModelRequestTypeDef(TypedDict):
    modelIdentifier: str,
```

## GetInferenceProfileRequestTypeDef

```python
# GetInferenceProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GetInferenceProfileRequestTypeDef


def get_value() -> GetInferenceProfileRequestTypeDef:
    return {
        "inferenceProfileIdentifier": ...,
    }


# GetInferenceProfileRequestTypeDef definition

class GetInferenceProfileRequestTypeDef(TypedDict):
    inferenceProfileIdentifier: str,
```

## InferenceProfileModelTypeDef

```python
# InferenceProfileModelTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import InferenceProfileModelTypeDef


def get_value() -> InferenceProfileModelTypeDef:
    return {
        "modelArn": ...,
    }


# InferenceProfileModelTypeDef definition

class InferenceProfileModelTypeDef(TypedDict):
    modelArn: NotRequired[str],
```

## GetMarketplaceModelEndpointRequestTypeDef

```python
# GetMarketplaceModelEndpointRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GetMarketplaceModelEndpointRequestTypeDef


def get_value() -> GetMarketplaceModelEndpointRequestTypeDef:
    return {
        "endpointArn": ...,
    }


# GetMarketplaceModelEndpointRequestTypeDef definition

class GetMarketplaceModelEndpointRequestTypeDef(TypedDict):
    endpointArn: str,
```

## GetModelCopyJobRequestTypeDef

```python
# GetModelCopyJobRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GetModelCopyJobRequestTypeDef


def get_value() -> GetModelCopyJobRequestTypeDef:
    return {
        "jobArn": ...,
    }


# GetModelCopyJobRequestTypeDef definition

class GetModelCopyJobRequestTypeDef(TypedDict):
    jobArn: str,
```

## GetModelCustomizationJobRequestTypeDef

```python
# GetModelCustomizationJobRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GetModelCustomizationJobRequestTypeDef


def get_value() -> GetModelCustomizationJobRequestTypeDef:
    return {
        "jobIdentifier": ...,
    }


# GetModelCustomizationJobRequestTypeDef definition

class GetModelCustomizationJobRequestTypeDef(TypedDict):
    jobIdentifier: str,
```

## VpcConfigOutputTypeDef

```python
# VpcConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import VpcConfigOutputTypeDef


def get_value() -> VpcConfigOutputTypeDef:
    return {
        "subnetIds": ...,
    }


# VpcConfigOutputTypeDef definition

class VpcConfigOutputTypeDef(TypedDict):
    subnetIds: List[str],
    securityGroupIds: List[str],
```

## GetModelImportJobRequestTypeDef

```python
# GetModelImportJobRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GetModelImportJobRequestTypeDef


def get_value() -> GetModelImportJobRequestTypeDef:
    return {
        "jobIdentifier": ...,
    }


# GetModelImportJobRequestTypeDef definition

class GetModelImportJobRequestTypeDef(TypedDict):
    jobIdentifier: str,
```

## GetModelInvocationJobRequestTypeDef

```python
# GetModelInvocationJobRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GetModelInvocationJobRequestTypeDef


def get_value() -> GetModelInvocationJobRequestTypeDef:
    return {
        "jobIdentifier": ...,
    }


# GetModelInvocationJobRequestTypeDef definition

class GetModelInvocationJobRequestTypeDef(TypedDict):
    jobIdentifier: str,
```

## GetPromptRouterRequestTypeDef

```python
# GetPromptRouterRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GetPromptRouterRequestTypeDef


def get_value() -> GetPromptRouterRequestTypeDef:
    return {
        "promptRouterArn": ...,
    }


# GetPromptRouterRequestTypeDef definition

class GetPromptRouterRequestTypeDef(TypedDict):
    promptRouterArn: str,
```

## PromptRouterTargetModelTypeDef

```python
# PromptRouterTargetModelTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import PromptRouterTargetModelTypeDef


def get_value() -> PromptRouterTargetModelTypeDef:
    return {
        "modelArn": ...,
    }


# PromptRouterTargetModelTypeDef definition

class PromptRouterTargetModelTypeDef(TypedDict):
    modelArn: NotRequired[str],
```

## RoutingCriteriaTypeDef

```python
# RoutingCriteriaTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import RoutingCriteriaTypeDef


def get_value() -> RoutingCriteriaTypeDef:
    return {
        "responseQualityDifference": ...,
    }


# RoutingCriteriaTypeDef definition

class RoutingCriteriaTypeDef(TypedDict):
    responseQualityDifference: float,
```

## GetProvisionedModelThroughputRequestTypeDef

```python
# GetProvisionedModelThroughputRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GetProvisionedModelThroughputRequestTypeDef


def get_value() -> GetProvisionedModelThroughputRequestTypeDef:
    return {
        "provisionedModelId": ...,
    }


# GetProvisionedModelThroughputRequestTypeDef definition

class GetProvisionedModelThroughputRequestTypeDef(TypedDict):
    provisionedModelId: str,
```

## GuardrailContentFilterConfigTypeDef

```python
# GuardrailContentFilterConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GuardrailContentFilterConfigTypeDef


def get_value() -> GuardrailContentFilterConfigTypeDef:
    return {
        "type": ...,
    }


# GuardrailContentFilterConfigTypeDef definition

class GuardrailContentFilterConfigTypeDef(TypedDict):
    type: GuardrailContentFilterTypeType,  # (1)
    inputStrength: GuardrailFilterStrengthType,  # (2)
    outputStrength: GuardrailFilterStrengthType,  # (2)
    inputModalities: NotRequired[Sequence[GuardrailModalityType]],  # (4)
    outputModalities: NotRequired[Sequence[GuardrailModalityType]],  # (4)
```

1. See [:material-code-brackets: GuardrailContentFilterTypeType](./literals.md#guardrailcontentfiltertypetype) 
2. See [:material-code-brackets: GuardrailFilterStrengthType](./literals.md#guardrailfilterstrengthtype) 
3. See [:material-code-brackets: GuardrailFilterStrengthType](./literals.md#guardrailfilterstrengthtype) 
4. See [:material-code-brackets: GuardrailModalityType](./literals.md#guardrailmodalitytype) 
5. See [:material-code-brackets: GuardrailModalityType](./literals.md#guardrailmodalitytype) 
## GuardrailContentFilterTypeDef

```python
# GuardrailContentFilterTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GuardrailContentFilterTypeDef


def get_value() -> GuardrailContentFilterTypeDef:
    return {
        "type": ...,
    }


# GuardrailContentFilterTypeDef definition

class GuardrailContentFilterTypeDef(TypedDict):
    type: GuardrailContentFilterTypeType,  # (1)
    inputStrength: GuardrailFilterStrengthType,  # (2)
    outputStrength: GuardrailFilterStrengthType,  # (2)
    inputModalities: NotRequired[List[GuardrailModalityType]],  # (4)
    outputModalities: NotRequired[List[GuardrailModalityType]],  # (4)
```

1. See [:material-code-brackets: GuardrailContentFilterTypeType](./literals.md#guardrailcontentfiltertypetype) 
2. See [:material-code-brackets: GuardrailFilterStrengthType](./literals.md#guardrailfilterstrengthtype) 
3. See [:material-code-brackets: GuardrailFilterStrengthType](./literals.md#guardrailfilterstrengthtype) 
4. See [:material-code-brackets: GuardrailModalityType](./literals.md#guardrailmodalitytype) 
5. See [:material-code-brackets: GuardrailModalityType](./literals.md#guardrailmodalitytype) 
## GuardrailContextualGroundingFilterConfigTypeDef

```python
# GuardrailContextualGroundingFilterConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GuardrailContextualGroundingFilterConfigTypeDef


def get_value() -> GuardrailContextualGroundingFilterConfigTypeDef:
    return {
        "type": ...,
    }


# GuardrailContextualGroundingFilterConfigTypeDef definition

class GuardrailContextualGroundingFilterConfigTypeDef(TypedDict):
    type: GuardrailContextualGroundingFilterTypeType,  # (1)
    threshold: float,
```

1. See [:material-code-brackets: GuardrailContextualGroundingFilterTypeType](./literals.md#guardrailcontextualgroundingfiltertypetype) 
## GuardrailContextualGroundingFilterTypeDef

```python
# GuardrailContextualGroundingFilterTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GuardrailContextualGroundingFilterTypeDef


def get_value() -> GuardrailContextualGroundingFilterTypeDef:
    return {
        "type": ...,
    }


# GuardrailContextualGroundingFilterTypeDef definition

class GuardrailContextualGroundingFilterTypeDef(TypedDict):
    type: GuardrailContextualGroundingFilterTypeType,  # (1)
    threshold: float,
```

1. See [:material-code-brackets: GuardrailContextualGroundingFilterTypeType](./literals.md#guardrailcontextualgroundingfiltertypetype) 
## GuardrailManagedWordsConfigTypeDef

```python
# GuardrailManagedWordsConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GuardrailManagedWordsConfigTypeDef


def get_value() -> GuardrailManagedWordsConfigTypeDef:
    return {
        "type": ...,
    }


# GuardrailManagedWordsConfigTypeDef definition

class GuardrailManagedWordsConfigTypeDef(TypedDict):
    type: GuardrailManagedWordsTypeType,  # (1)
```

1. See [:material-code-brackets: GuardrailManagedWordsTypeType](./literals.md#guardrailmanagedwordstypetype) 
## GuardrailManagedWordsTypeDef

```python
# GuardrailManagedWordsTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GuardrailManagedWordsTypeDef


def get_value() -> GuardrailManagedWordsTypeDef:
    return {
        "type": ...,
    }


# GuardrailManagedWordsTypeDef definition

class GuardrailManagedWordsTypeDef(TypedDict):
    type: GuardrailManagedWordsTypeType,  # (1)
```

1. See [:material-code-brackets: GuardrailManagedWordsTypeType](./literals.md#guardrailmanagedwordstypetype) 
## GuardrailPiiEntityConfigTypeDef

```python
# GuardrailPiiEntityConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GuardrailPiiEntityConfigTypeDef


def get_value() -> GuardrailPiiEntityConfigTypeDef:
    return {
        "type": ...,
    }


# GuardrailPiiEntityConfigTypeDef definition

class GuardrailPiiEntityConfigTypeDef(TypedDict):
    type: GuardrailPiiEntityTypeType,  # (1)
    action: GuardrailSensitiveInformationActionType,  # (2)
```

1. See [:material-code-brackets: GuardrailPiiEntityTypeType](./literals.md#guardrailpiientitytypetype) 
2. See [:material-code-brackets: GuardrailSensitiveInformationActionType](./literals.md#guardrailsensitiveinformationactiontype) 
## GuardrailPiiEntityTypeDef

```python
# GuardrailPiiEntityTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GuardrailPiiEntityTypeDef


def get_value() -> GuardrailPiiEntityTypeDef:
    return {
        "type": ...,
    }


# GuardrailPiiEntityTypeDef definition

class GuardrailPiiEntityTypeDef(TypedDict):
    type: GuardrailPiiEntityTypeType,  # (1)
    action: GuardrailSensitiveInformationActionType,  # (2)
```

1. See [:material-code-brackets: GuardrailPiiEntityTypeType](./literals.md#guardrailpiientitytypetype) 
2. See [:material-code-brackets: GuardrailSensitiveInformationActionType](./literals.md#guardrailsensitiveinformationactiontype) 
## GuardrailRegexConfigTypeDef

```python
# GuardrailRegexConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GuardrailRegexConfigTypeDef


def get_value() -> GuardrailRegexConfigTypeDef:
    return {
        "name": ...,
    }


# GuardrailRegexConfigTypeDef definition

class GuardrailRegexConfigTypeDef(TypedDict):
    name: str,
    pattern: str,
    action: GuardrailSensitiveInformationActionType,  # (1)
    description: NotRequired[str],
```

1. See [:material-code-brackets: GuardrailSensitiveInformationActionType](./literals.md#guardrailsensitiveinformationactiontype) 
## GuardrailRegexTypeDef

```python
# GuardrailRegexTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GuardrailRegexTypeDef


def get_value() -> GuardrailRegexTypeDef:
    return {
        "name": ...,
    }


# GuardrailRegexTypeDef definition

class GuardrailRegexTypeDef(TypedDict):
    name: str,
    pattern: str,
    action: GuardrailSensitiveInformationActionType,  # (1)
    description: NotRequired[str],
```

1. See [:material-code-brackets: GuardrailSensitiveInformationActionType](./literals.md#guardrailsensitiveinformationactiontype) 
## GuardrailSummaryTypeDef

```python
# GuardrailSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GuardrailSummaryTypeDef


def get_value() -> GuardrailSummaryTypeDef:
    return {
        "id": ...,
    }


# GuardrailSummaryTypeDef definition

class GuardrailSummaryTypeDef(TypedDict):
    id: str,
    arn: str,
    status: GuardrailStatusType,  # (1)
    name: str,
    version: str,
    createdAt: datetime,
    updatedAt: datetime,
    description: NotRequired[str],
```

1. See [:material-code-brackets: GuardrailStatusType](./literals.md#guardrailstatustype) 
## GuardrailTopicConfigTypeDef

```python
# GuardrailTopicConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GuardrailTopicConfigTypeDef


def get_value() -> GuardrailTopicConfigTypeDef:
    return {
        "name": ...,
    }


# GuardrailTopicConfigTypeDef definition

class GuardrailTopicConfigTypeDef(TypedDict):
    name: str,
    definition: str,
    type: GuardrailTopicTypeType,  # (1)
    examples: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: GuardrailTopicTypeType](./literals.md#guardrailtopictypetype) 
## GuardrailTopicTypeDef

```python
# GuardrailTopicTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GuardrailTopicTypeDef


def get_value() -> GuardrailTopicTypeDef:
    return {
        "name": ...,
    }


# GuardrailTopicTypeDef definition

class GuardrailTopicTypeDef(TypedDict):
    name: str,
    definition: str,
    examples: NotRequired[List[str]],
    type: NotRequired[GuardrailTopicTypeType],  # (1)
```

1. See [:material-code-brackets: GuardrailTopicTypeType](./literals.md#guardrailtopictypetype) 
## GuardrailWordConfigTypeDef

```python
# GuardrailWordConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GuardrailWordConfigTypeDef


def get_value() -> GuardrailWordConfigTypeDef:
    return {
        "text": ...,
    }


# GuardrailWordConfigTypeDef definition

class GuardrailWordConfigTypeDef(TypedDict):
    text: str,
```

## GuardrailWordTypeDef

```python
# GuardrailWordTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GuardrailWordTypeDef


def get_value() -> GuardrailWordTypeDef:
    return {
        "text": ...,
    }


# GuardrailWordTypeDef definition

class GuardrailWordTypeDef(TypedDict):
    text: str,
```

## HumanEvaluationCustomMetricTypeDef

```python
# HumanEvaluationCustomMetricTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import HumanEvaluationCustomMetricTypeDef


def get_value() -> HumanEvaluationCustomMetricTypeDef:
    return {
        "name": ...,
    }


# HumanEvaluationCustomMetricTypeDef definition

class HumanEvaluationCustomMetricTypeDef(TypedDict):
    name: str,
    ratingMethod: str,
    description: NotRequired[str],
```

## HumanWorkflowConfigTypeDef

```python
# HumanWorkflowConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import HumanWorkflowConfigTypeDef


def get_value() -> HumanWorkflowConfigTypeDef:
    return {
        "flowDefinitionArn": ...,
    }


# HumanWorkflowConfigTypeDef definition

class HumanWorkflowConfigTypeDef(TypedDict):
    flowDefinitionArn: str,
    instructions: NotRequired[str],
```

## ImportedModelSummaryTypeDef

```python
# ImportedModelSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ImportedModelSummaryTypeDef


def get_value() -> ImportedModelSummaryTypeDef:
    return {
        "modelArn": ...,
    }


# ImportedModelSummaryTypeDef definition

class ImportedModelSummaryTypeDef(TypedDict):
    modelArn: str,
    modelName: str,
    creationTime: datetime,
    instructSupported: NotRequired[bool],
    modelArchitecture: NotRequired[str],
```

## InvocationLogSourceTypeDef

```python
# InvocationLogSourceTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import InvocationLogSourceTypeDef


def get_value() -> InvocationLogSourceTypeDef:
    return {
        "s3Uri": ...,
    }


# InvocationLogSourceTypeDef definition

class InvocationLogSourceTypeDef(TypedDict):
    s3Uri: NotRequired[str],
```

## TextInferenceConfigOutputTypeDef

```python
# TextInferenceConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import TextInferenceConfigOutputTypeDef


def get_value() -> TextInferenceConfigOutputTypeDef:
    return {
        "temperature": ...,
    }


# TextInferenceConfigOutputTypeDef definition

class TextInferenceConfigOutputTypeDef(TypedDict):
    temperature: NotRequired[float],
    topP: NotRequired[float],
    maxTokens: NotRequired[int],
    stopSequences: NotRequired[List[str]],
```

## TextInferenceConfigTypeDef

```python
# TextInferenceConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import TextInferenceConfigTypeDef


def get_value() -> TextInferenceConfigTypeDef:
    return {
        "temperature": ...,
    }


# TextInferenceConfigTypeDef definition

class TextInferenceConfigTypeDef(TypedDict):
    temperature: NotRequired[float],
    topP: NotRequired[float],
    maxTokens: NotRequired[int],
    stopSequences: NotRequired[Sequence[str]],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import PaginatorConfigTypeDef


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

## ListFoundationModelsRequestTypeDef

```python
# ListFoundationModelsRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListFoundationModelsRequestTypeDef


def get_value() -> ListFoundationModelsRequestTypeDef:
    return {
        "byProvider": ...,
    }


# ListFoundationModelsRequestTypeDef definition

class ListFoundationModelsRequestTypeDef(TypedDict):
    byProvider: NotRequired[str],
    byCustomizationType: NotRequired[ModelCustomizationType],  # (1)
    byOutputModality: NotRequired[ModelModalityType],  # (2)
    byInferenceType: NotRequired[InferenceTypeType],  # (3)
```

1. See [:material-code-brackets: ModelCustomizationType](./literals.md#modelcustomizationtype) 
2. See [:material-code-brackets: ModelModalityType](./literals.md#modelmodalitytype) 
3. See [:material-code-brackets: InferenceTypeType](./literals.md#inferencetypetype) 
## ListGuardrailsRequestTypeDef

```python
# ListGuardrailsRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListGuardrailsRequestTypeDef


def get_value() -> ListGuardrailsRequestTypeDef:
    return {
        "guardrailIdentifier": ...,
    }


# ListGuardrailsRequestTypeDef definition

class ListGuardrailsRequestTypeDef(TypedDict):
    guardrailIdentifier: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListInferenceProfilesRequestTypeDef

```python
# ListInferenceProfilesRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListInferenceProfilesRequestTypeDef


def get_value() -> ListInferenceProfilesRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListInferenceProfilesRequestTypeDef definition

class ListInferenceProfilesRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    typeEquals: NotRequired[InferenceProfileTypeType],  # (1)
```

1. See [:material-code-brackets: InferenceProfileTypeType](./literals.md#inferenceprofiletypetype) 
## ListMarketplaceModelEndpointsRequestTypeDef

```python
# ListMarketplaceModelEndpointsRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListMarketplaceModelEndpointsRequestTypeDef


def get_value() -> ListMarketplaceModelEndpointsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListMarketplaceModelEndpointsRequestTypeDef definition

class ListMarketplaceModelEndpointsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    modelSourceEquals: NotRequired[str],
```

## MarketplaceModelEndpointSummaryTypeDef

```python
# MarketplaceModelEndpointSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import MarketplaceModelEndpointSummaryTypeDef


def get_value() -> MarketplaceModelEndpointSummaryTypeDef:
    return {
        "endpointArn": ...,
    }


# MarketplaceModelEndpointSummaryTypeDef definition

class MarketplaceModelEndpointSummaryTypeDef(TypedDict):
    endpointArn: str,
    modelSourceIdentifier: str,
    createdAt: datetime,
    updatedAt: datetime,
    status: NotRequired[StatusType],  # (1)
    statusMessage: NotRequired[str],
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## ModelCustomizationJobSummaryTypeDef

```python
# ModelCustomizationJobSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ModelCustomizationJobSummaryTypeDef


def get_value() -> ModelCustomizationJobSummaryTypeDef:
    return {
        "jobArn": ...,
    }


# ModelCustomizationJobSummaryTypeDef definition

class ModelCustomizationJobSummaryTypeDef(TypedDict):
    jobArn: str,
    baseModelArn: str,
    jobName: str,
    status: ModelCustomizationJobStatusType,  # (1)
    creationTime: datetime,
    lastModifiedTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
    customModelArn: NotRequired[str],
    customModelName: NotRequired[str],
    customizationType: NotRequired[CustomizationTypeType],  # (2)
```

1. See [:material-code-brackets: ModelCustomizationJobStatusType](./literals.md#modelcustomizationjobstatustype) 
2. See [:material-code-brackets: CustomizationTypeType](./literals.md#customizationtypetype) 
## ModelImportJobSummaryTypeDef

```python
# ModelImportJobSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ModelImportJobSummaryTypeDef


def get_value() -> ModelImportJobSummaryTypeDef:
    return {
        "jobArn": ...,
    }


# ModelImportJobSummaryTypeDef definition

class ModelImportJobSummaryTypeDef(TypedDict):
    jobArn: str,
    jobName: str,
    status: ModelImportJobStatusType,  # (1)
    creationTime: datetime,
    lastModifiedTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
    importedModelArn: NotRequired[str],
    importedModelName: NotRequired[str],
```

1. See [:material-code-brackets: ModelImportJobStatusType](./literals.md#modelimportjobstatustype) 
## ListPromptRoutersRequestTypeDef

```python
# ListPromptRoutersRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListPromptRoutersRequestTypeDef


def get_value() -> ListPromptRoutersRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListPromptRoutersRequestTypeDef definition

class ListPromptRoutersRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ProvisionedModelSummaryTypeDef

```python
# ProvisionedModelSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ProvisionedModelSummaryTypeDef


def get_value() -> ProvisionedModelSummaryTypeDef:
    return {
        "provisionedModelName": ...,
    }


# ProvisionedModelSummaryTypeDef definition

class ProvisionedModelSummaryTypeDef(TypedDict):
    provisionedModelName: str,
    provisionedModelArn: str,
    modelArn: str,
    desiredModelArn: str,
    foundationModelArn: str,
    modelUnits: int,
    desiredModelUnits: int,
    status: ProvisionedModelStatusType,  # (1)
    creationTime: datetime,
    lastModifiedTime: datetime,
    commitmentDuration: NotRequired[CommitmentDurationType],  # (2)
    commitmentExpirationTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ProvisionedModelStatusType](./literals.md#provisionedmodelstatustype) 
2. See [:material-code-brackets: CommitmentDurationType](./literals.md#commitmentdurationtype) 
## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceARN": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceARN: str,
```

## S3DataSourceTypeDef

```python
# S3DataSourceTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import S3DataSourceTypeDef


def get_value() -> S3DataSourceTypeDef:
    return {
        "s3Uri": ...,
    }


# S3DataSourceTypeDef definition

class S3DataSourceTypeDef(TypedDict):
    s3Uri: str,
```

## ModelInvocationJobS3InputDataConfigTypeDef

```python
# ModelInvocationJobS3InputDataConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ModelInvocationJobS3InputDataConfigTypeDef


def get_value() -> ModelInvocationJobS3InputDataConfigTypeDef:
    return {
        "s3InputFormat": ...,
    }


# ModelInvocationJobS3InputDataConfigTypeDef definition

class ModelInvocationJobS3InputDataConfigTypeDef(TypedDict):
    s3Uri: str,
    s3InputFormat: NotRequired[S3InputFormatType],  # (1)
    s3BucketOwner: NotRequired[str],
```

1. See [:material-code-brackets: S3InputFormatType](./literals.md#s3inputformattype) 
## ModelInvocationJobS3OutputDataConfigTypeDef

```python
# ModelInvocationJobS3OutputDataConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ModelInvocationJobS3OutputDataConfigTypeDef


def get_value() -> ModelInvocationJobS3OutputDataConfigTypeDef:
    return {
        "s3Uri": ...,
    }


# ModelInvocationJobS3OutputDataConfigTypeDef definition

class ModelInvocationJobS3OutputDataConfigTypeDef(TypedDict):
    s3Uri: str,
    s3EncryptionKeyId: NotRequired[str],
    s3BucketOwner: NotRequired[str],
```

## QueryTransformationConfigurationTypeDef

```python
# QueryTransformationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import QueryTransformationConfigurationTypeDef


def get_value() -> QueryTransformationConfigurationTypeDef:
    return {
        "type": ...,
    }


# QueryTransformationConfigurationTypeDef definition

class QueryTransformationConfigurationTypeDef(TypedDict):
    type: QueryTransformationTypeType,  # (1)
```

1. See [:material-code-brackets: QueryTransformationTypeType](./literals.md#querytransformationtypetype) 
## RegisterMarketplaceModelEndpointRequestTypeDef

```python
# RegisterMarketplaceModelEndpointRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import RegisterMarketplaceModelEndpointRequestTypeDef


def get_value() -> RegisterMarketplaceModelEndpointRequestTypeDef:
    return {
        "endpointIdentifier": ...,
    }


# RegisterMarketplaceModelEndpointRequestTypeDef definition

class RegisterMarketplaceModelEndpointRequestTypeDef(TypedDict):
    endpointIdentifier: str,
    modelSourceIdentifier: str,
```

## RequestMetadataBaseFiltersOutputTypeDef

```python
# RequestMetadataBaseFiltersOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import RequestMetadataBaseFiltersOutputTypeDef


def get_value() -> RequestMetadataBaseFiltersOutputTypeDef:
    return {
        "equals": ...,
    }


# RequestMetadataBaseFiltersOutputTypeDef definition

class RequestMetadataBaseFiltersOutputTypeDef(TypedDict):
    equals: NotRequired[Dict[str, str]],
    notEquals: NotRequired[Dict[str, str]],
```

## RequestMetadataBaseFiltersTypeDef

```python
# RequestMetadataBaseFiltersTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import RequestMetadataBaseFiltersTypeDef


def get_value() -> RequestMetadataBaseFiltersTypeDef:
    return {
        "equals": ...,
    }


# RequestMetadataBaseFiltersTypeDef definition

class RequestMetadataBaseFiltersTypeDef(TypedDict):
    equals: NotRequired[Mapping[str, str]],
    notEquals: NotRequired[Mapping[str, str]],
```

## VpcConfigTypeDef

```python
# VpcConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import VpcConfigTypeDef


def get_value() -> VpcConfigTypeDef:
    return {
        "subnetIds": ...,
    }


# VpcConfigTypeDef definition

class VpcConfigTypeDef(TypedDict):
    subnetIds: Sequence[str],
    securityGroupIds: Sequence[str],
```

## StopEvaluationJobRequestTypeDef

```python
# StopEvaluationJobRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import StopEvaluationJobRequestTypeDef


def get_value() -> StopEvaluationJobRequestTypeDef:
    return {
        "jobIdentifier": ...,
    }


# StopEvaluationJobRequestTypeDef definition

class StopEvaluationJobRequestTypeDef(TypedDict):
    jobIdentifier: str,
```

## StopModelCustomizationJobRequestTypeDef

```python
# StopModelCustomizationJobRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import StopModelCustomizationJobRequestTypeDef


def get_value() -> StopModelCustomizationJobRequestTypeDef:
    return {
        "jobIdentifier": ...,
    }


# StopModelCustomizationJobRequestTypeDef definition

class StopModelCustomizationJobRequestTypeDef(TypedDict):
    jobIdentifier: str,
```

## StopModelInvocationJobRequestTypeDef

```python
# StopModelInvocationJobRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import StopModelInvocationJobRequestTypeDef


def get_value() -> StopModelInvocationJobRequestTypeDef:
    return {
        "jobIdentifier": ...,
    }


# StopModelInvocationJobRequestTypeDef definition

class StopModelInvocationJobRequestTypeDef(TypedDict):
    jobIdentifier: str,
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceARN": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceARN: str,
    tagKeys: Sequence[str],
```

## UpdateProvisionedModelThroughputRequestTypeDef

```python
# UpdateProvisionedModelThroughputRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import UpdateProvisionedModelThroughputRequestTypeDef


def get_value() -> UpdateProvisionedModelThroughputRequestTypeDef:
    return {
        "provisionedModelId": ...,
    }


# UpdateProvisionedModelThroughputRequestTypeDef definition

class UpdateProvisionedModelThroughputRequestTypeDef(TypedDict):
    provisionedModelId: str,
    desiredProvisionedModelName: NotRequired[str],
    desiredModelId: NotRequired[str],
```

## ValidatorTypeDef

```python
# ValidatorTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ValidatorTypeDef


def get_value() -> ValidatorTypeDef:
    return {
        "s3Uri": ...,
    }


# ValidatorTypeDef definition

class ValidatorTypeDef(TypedDict):
    s3Uri: str,
```

## BatchDeleteEvaluationJobResponseTypeDef

```python
# BatchDeleteEvaluationJobResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import BatchDeleteEvaluationJobResponseTypeDef


def get_value() -> BatchDeleteEvaluationJobResponseTypeDef:
    return {
        "errors": ...,
    }


# BatchDeleteEvaluationJobResponseTypeDef definition

class BatchDeleteEvaluationJobResponseTypeDef(TypedDict):
    errors: List[BatchDeleteEvaluationJobErrorTypeDef],  # (1)
    evaluationJobs: List[BatchDeleteEvaluationJobItemTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchDeleteEvaluationJobErrorTypeDef](./type_defs.md#batchdeleteevaluationjoberrortypedef) 
2. See [:material-code-braces: BatchDeleteEvaluationJobItemTypeDef](./type_defs.md#batchdeleteevaluationjobitemtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEvaluationJobResponseTypeDef

```python
# CreateEvaluationJobResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import CreateEvaluationJobResponseTypeDef


def get_value() -> CreateEvaluationJobResponseTypeDef:
    return {
        "jobArn": ...,
    }


# CreateEvaluationJobResponseTypeDef definition

class CreateEvaluationJobResponseTypeDef(TypedDict):
    jobArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGuardrailResponseTypeDef

```python
# CreateGuardrailResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import CreateGuardrailResponseTypeDef


def get_value() -> CreateGuardrailResponseTypeDef:
    return {
        "guardrailId": ...,
    }


# CreateGuardrailResponseTypeDef definition

class CreateGuardrailResponseTypeDef(TypedDict):
    guardrailId: str,
    guardrailArn: str,
    version: str,
    createdAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGuardrailVersionResponseTypeDef

```python
# CreateGuardrailVersionResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import CreateGuardrailVersionResponseTypeDef


def get_value() -> CreateGuardrailVersionResponseTypeDef:
    return {
        "guardrailId": ...,
    }


# CreateGuardrailVersionResponseTypeDef definition

class CreateGuardrailVersionResponseTypeDef(TypedDict):
    guardrailId: str,
    version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateInferenceProfileResponseTypeDef

```python
# CreateInferenceProfileResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import CreateInferenceProfileResponseTypeDef


def get_value() -> CreateInferenceProfileResponseTypeDef:
    return {
        "inferenceProfileArn": ...,
    }


# CreateInferenceProfileResponseTypeDef definition

class CreateInferenceProfileResponseTypeDef(TypedDict):
    inferenceProfileArn: str,
    status: InferenceProfileStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: InferenceProfileStatusType](./literals.md#inferenceprofilestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateModelCopyJobResponseTypeDef

```python
# CreateModelCopyJobResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import CreateModelCopyJobResponseTypeDef


def get_value() -> CreateModelCopyJobResponseTypeDef:
    return {
        "jobArn": ...,
    }


# CreateModelCopyJobResponseTypeDef definition

class CreateModelCopyJobResponseTypeDef(TypedDict):
    jobArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateModelCustomizationJobResponseTypeDef

```python
# CreateModelCustomizationJobResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import CreateModelCustomizationJobResponseTypeDef


def get_value() -> CreateModelCustomizationJobResponseTypeDef:
    return {
        "jobArn": ...,
    }


# CreateModelCustomizationJobResponseTypeDef definition

class CreateModelCustomizationJobResponseTypeDef(TypedDict):
    jobArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateModelImportJobResponseTypeDef

```python
# CreateModelImportJobResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import CreateModelImportJobResponseTypeDef


def get_value() -> CreateModelImportJobResponseTypeDef:
    return {
        "jobArn": ...,
    }


# CreateModelImportJobResponseTypeDef definition

class CreateModelImportJobResponseTypeDef(TypedDict):
    jobArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateModelInvocationJobResponseTypeDef

```python
# CreateModelInvocationJobResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import CreateModelInvocationJobResponseTypeDef


def get_value() -> CreateModelInvocationJobResponseTypeDef:
    return {
        "jobArn": ...,
    }


# CreateModelInvocationJobResponseTypeDef definition

class CreateModelInvocationJobResponseTypeDef(TypedDict):
    jobArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProvisionedModelThroughputResponseTypeDef

```python
# CreateProvisionedModelThroughputResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import CreateProvisionedModelThroughputResponseTypeDef


def get_value() -> CreateProvisionedModelThroughputResponseTypeDef:
    return {
        "provisionedModelArn": ...,
    }


# CreateProvisionedModelThroughputResponseTypeDef definition

class CreateProvisionedModelThroughputResponseTypeDef(TypedDict):
    provisionedModelArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetProvisionedModelThroughputResponseTypeDef

```python
# GetProvisionedModelThroughputResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GetProvisionedModelThroughputResponseTypeDef


def get_value() -> GetProvisionedModelThroughputResponseTypeDef:
    return {
        "modelUnits": ...,
    }


# GetProvisionedModelThroughputResponseTypeDef definition

class GetProvisionedModelThroughputResponseTypeDef(TypedDict):
    modelUnits: int,
    desiredModelUnits: int,
    provisionedModelName: str,
    provisionedModelArn: str,
    modelArn: str,
    desiredModelArn: str,
    foundationModelArn: str,
    status: ProvisionedModelStatusType,  # (1)
    creationTime: datetime,
    lastModifiedTime: datetime,
    failureMessage: str,
    commitmentDuration: CommitmentDurationType,  # (2)
    commitmentExpirationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ProvisionedModelStatusType](./literals.md#provisionedmodelstatustype) 
2. See [:material-code-brackets: CommitmentDurationType](./literals.md#commitmentdurationtype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGuardrailResponseTypeDef

```python
# UpdateGuardrailResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import UpdateGuardrailResponseTypeDef


def get_value() -> UpdateGuardrailResponseTypeDef:
    return {
        "guardrailId": ...,
    }


# UpdateGuardrailResponseTypeDef definition

class UpdateGuardrailResponseTypeDef(TypedDict):
    guardrailId: str,
    guardrailArn: str,
    version: str,
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EvaluatorModelConfigOutputTypeDef

```python
# EvaluatorModelConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import EvaluatorModelConfigOutputTypeDef


def get_value() -> EvaluatorModelConfigOutputTypeDef:
    return {
        "bedrockEvaluatorModels": ...,
    }


# EvaluatorModelConfigOutputTypeDef definition

class EvaluatorModelConfigOutputTypeDef(TypedDict):
    bedrockEvaluatorModels: NotRequired[List[BedrockEvaluatorModelTypeDef]],  # (1)
```

1. See [:material-code-braces: BedrockEvaluatorModelTypeDef](./type_defs.md#bedrockevaluatormodeltypedef) 
## EvaluatorModelConfigTypeDef

```python
# EvaluatorModelConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import EvaluatorModelConfigTypeDef


def get_value() -> EvaluatorModelConfigTypeDef:
    return {
        "bedrockEvaluatorModels": ...,
    }


# EvaluatorModelConfigTypeDef definition

class EvaluatorModelConfigTypeDef(TypedDict):
    bedrockEvaluatorModels: NotRequired[Sequence[BedrockEvaluatorModelTypeDef]],  # (1)
```

1. See [:material-code-braces: BedrockEvaluatorModelTypeDef](./type_defs.md#bedrockevaluatormodeltypedef) 
## ByteContentDocTypeDef

```python
# ByteContentDocTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ByteContentDocTypeDef


def get_value() -> ByteContentDocTypeDef:
    return {
        "identifier": ...,
    }


# ByteContentDocTypeDef definition

class ByteContentDocTypeDef(TypedDict):
    identifier: str,
    contentType: str,
    data: BlobTypeDef,
```

## CloudWatchConfigTypeDef

```python
# CloudWatchConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import CloudWatchConfigTypeDef


def get_value() -> CloudWatchConfigTypeDef:
    return {
        "logGroupName": ...,
    }


# CloudWatchConfigTypeDef definition

class CloudWatchConfigTypeDef(TypedDict):
    logGroupName: str,
    roleArn: str,
    largeDataDeliveryS3Config: NotRequired[S3ConfigTypeDef],  # (1)
```

1. See [:material-code-braces: S3ConfigTypeDef](./type_defs.md#s3configtypedef) 
## CreateModelCopyJobRequestTypeDef

```python
# CreateModelCopyJobRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import CreateModelCopyJobRequestTypeDef


def get_value() -> CreateModelCopyJobRequestTypeDef:
    return {
        "sourceModelArn": ...,
    }


# CreateModelCopyJobRequestTypeDef definition

class CreateModelCopyJobRequestTypeDef(TypedDict):
    sourceModelArn: str,
    targetModelName: str,
    modelKmsKeyId: NotRequired[str],
    targetModelTags: NotRequired[Sequence[TagTypeDef]],  # (1)
    clientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateProvisionedModelThroughputRequestTypeDef

```python
# CreateProvisionedModelThroughputRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import CreateProvisionedModelThroughputRequestTypeDef


def get_value() -> CreateProvisionedModelThroughputRequestTypeDef:
    return {
        "modelUnits": ...,
    }


# CreateProvisionedModelThroughputRequestTypeDef definition

class CreateProvisionedModelThroughputRequestTypeDef(TypedDict):
    modelUnits: int,
    provisionedModelName: str,
    modelId: str,
    clientRequestToken: NotRequired[str],
    commitmentDuration: NotRequired[CommitmentDurationType],  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: CommitmentDurationType](./literals.md#commitmentdurationtype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetModelCopyJobResponseTypeDef

```python
# GetModelCopyJobResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GetModelCopyJobResponseTypeDef


def get_value() -> GetModelCopyJobResponseTypeDef:
    return {
        "jobArn": ...,
    }


# GetModelCopyJobResponseTypeDef definition

class GetModelCopyJobResponseTypeDef(TypedDict):
    jobArn: str,
    status: ModelCopyJobStatusType,  # (1)
    creationTime: datetime,
    targetModelArn: str,
    targetModelName: str,
    sourceAccountId: str,
    sourceModelArn: str,
    targetModelKmsKeyArn: str,
    targetModelTags: List[TagTypeDef],  # (2)
    failureMessage: str,
    sourceModelName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ModelCopyJobStatusType](./literals.md#modelcopyjobstatustype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModelCopyJobSummaryTypeDef

```python
# ModelCopyJobSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ModelCopyJobSummaryTypeDef


def get_value() -> ModelCopyJobSummaryTypeDef:
    return {
        "jobArn": ...,
    }


# ModelCopyJobSummaryTypeDef definition

class ModelCopyJobSummaryTypeDef(TypedDict):
    jobArn: str,
    status: ModelCopyJobStatusType,  # (1)
    creationTime: datetime,
    targetModelArn: str,
    sourceAccountId: str,
    sourceModelArn: str,
    targetModelName: NotRequired[str],
    targetModelKmsKeyArn: NotRequired[str],
    targetModelTags: NotRequired[List[TagTypeDef]],  # (2)
    failureMessage: NotRequired[str],
    sourceModelName: NotRequired[str],
```

1. See [:material-code-brackets: ModelCopyJobStatusType](./literals.md#modelcopyjobstatustype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceARN": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceARN: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateInferenceProfileRequestTypeDef

```python
# CreateInferenceProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import CreateInferenceProfileRequestTypeDef


def get_value() -> CreateInferenceProfileRequestTypeDef:
    return {
        "inferenceProfileName": ...,
    }


# CreateInferenceProfileRequestTypeDef definition

class CreateInferenceProfileRequestTypeDef(TypedDict):
    inferenceProfileName: str,
    modelSource: InferenceProfileModelSourceTypeDef,  # (1)
    description: NotRequired[str],
    clientRequestToken: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: InferenceProfileModelSourceTypeDef](./type_defs.md#inferenceprofilemodelsourcetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListCustomModelsResponseTypeDef

```python
# ListCustomModelsResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListCustomModelsResponseTypeDef


def get_value() -> ListCustomModelsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListCustomModelsResponseTypeDef definition

class ListCustomModelsResponseTypeDef(TypedDict):
    modelSummaries: List[CustomModelSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CustomModelSummaryTypeDef](./type_defs.md#custommodelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DistillationConfigTypeDef

```python
# DistillationConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import DistillationConfigTypeDef


def get_value() -> DistillationConfigTypeDef:
    return {
        "teacherModelConfig": ...,
    }


# DistillationConfigTypeDef definition

class DistillationConfigTypeDef(TypedDict):
    teacherModelConfig: TeacherModelConfigTypeDef,  # (1)
```

1. See [:material-code-braces: TeacherModelConfigTypeDef](./type_defs.md#teachermodelconfigtypedef) 
## EvaluationBedrockModelTypeDef

```python
# EvaluationBedrockModelTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import EvaluationBedrockModelTypeDef


def get_value() -> EvaluationBedrockModelTypeDef:
    return {
        "modelIdentifier": ...,
    }


# EvaluationBedrockModelTypeDef definition

class EvaluationBedrockModelTypeDef(TypedDict):
    modelIdentifier: str,
    inferenceParams: NotRequired[str],
    performanceConfig: NotRequired[PerformanceConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: PerformanceConfigurationTypeDef](./type_defs.md#performanceconfigurationtypedef) 
## EvaluationDatasetTypeDef

```python
# EvaluationDatasetTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import EvaluationDatasetTypeDef


def get_value() -> EvaluationDatasetTypeDef:
    return {
        "name": ...,
    }


# EvaluationDatasetTypeDef definition

class EvaluationDatasetTypeDef(TypedDict):
    name: str,
    datasetLocation: NotRequired[EvaluationDatasetLocationTypeDef],  # (1)
```

1. See [:material-code-braces: EvaluationDatasetLocationTypeDef](./type_defs.md#evaluationdatasetlocationtypedef) 
## ListEvaluationJobsResponseTypeDef

```python
# ListEvaluationJobsResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListEvaluationJobsResponseTypeDef


def get_value() -> ListEvaluationJobsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListEvaluationJobsResponseTypeDef definition

class ListEvaluationJobsResponseTypeDef(TypedDict):
    jobSummaries: List[EvaluationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: EvaluationSummaryTypeDef](./type_defs.md#evaluationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExternalSourceOutputTypeDef

```python
# ExternalSourceOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ExternalSourceOutputTypeDef


def get_value() -> ExternalSourceOutputTypeDef:
    return {
        "sourceType": ...,
    }


# ExternalSourceOutputTypeDef definition

class ExternalSourceOutputTypeDef(TypedDict):
    sourceType: ExternalSourceTypeType,  # (1)
    s3Location: NotRequired[S3ObjectDocTypeDef],  # (2)
    byteContent: NotRequired[ByteContentDocOutputTypeDef],  # (3)
```

1. See [:material-code-brackets: ExternalSourceTypeType](./literals.md#externalsourcetypetype) 
2. See [:material-code-braces: S3ObjectDocTypeDef](./type_defs.md#s3objectdoctypedef) 
3. See [:material-code-braces: ByteContentDocOutputTypeDef](./type_defs.md#bytecontentdocoutputtypedef) 
## RetrievalFilterOutputTypeDef

```python
# RetrievalFilterOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import RetrievalFilterOutputTypeDef


def get_value() -> RetrievalFilterOutputTypeDef:
    return {
        "equals": ...,
    }


# RetrievalFilterOutputTypeDef definition

class RetrievalFilterOutputTypeDef(TypedDict):
    equals: NotRequired[FilterAttributeOutputTypeDef],  # (1)
    notEquals: NotRequired[FilterAttributeOutputTypeDef],  # (1)
    greaterThan: NotRequired[FilterAttributeOutputTypeDef],  # (1)
    greaterThanOrEquals: NotRequired[FilterAttributeOutputTypeDef],  # (1)
    lessThan: NotRequired[FilterAttributeOutputTypeDef],  # (1)
    lessThanOrEquals: NotRequired[FilterAttributeOutputTypeDef],  # (1)
    in: NotRequired[FilterAttributeOutputTypeDef],  # (1)
    notIn: NotRequired[FilterAttributeOutputTypeDef],  # (1)
    startsWith: NotRequired[FilterAttributeOutputTypeDef],  # (1)
    listContains: NotRequired[FilterAttributeOutputTypeDef],  # (1)
    stringContains: NotRequired[FilterAttributeOutputTypeDef],  # (1)
    andAll: NotRequired[List[Dict[str, Any]]],
    orAll: NotRequired[List[Dict[str, Any]]],
```

1. See [:material-code-braces: FilterAttributeOutputTypeDef](./type_defs.md#filterattributeoutputtypedef) 
2. See [:material-code-braces: FilterAttributeOutputTypeDef](./type_defs.md#filterattributeoutputtypedef) 
3. See [:material-code-braces: FilterAttributeOutputTypeDef](./type_defs.md#filterattributeoutputtypedef) 
4. See [:material-code-braces: FilterAttributeOutputTypeDef](./type_defs.md#filterattributeoutputtypedef) 
5. See [:material-code-braces: FilterAttributeOutputTypeDef](./type_defs.md#filterattributeoutputtypedef) 
6. See [:material-code-braces: FilterAttributeOutputTypeDef](./type_defs.md#filterattributeoutputtypedef) 
7. See [:material-code-braces: FilterAttributeOutputTypeDef](./type_defs.md#filterattributeoutputtypedef) 
8. See [:material-code-braces: FilterAttributeOutputTypeDef](./type_defs.md#filterattributeoutputtypedef) 
9. See [:material-code-braces: FilterAttributeOutputTypeDef](./type_defs.md#filterattributeoutputtypedef) 
10. See [:material-code-braces: FilterAttributeOutputTypeDef](./type_defs.md#filterattributeoutputtypedef) 
11. See [:material-code-braces: FilterAttributeOutputTypeDef](./type_defs.md#filterattributeoutputtypedef) 
## RetrievalFilterTypeDef

```python
# RetrievalFilterTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import RetrievalFilterTypeDef


def get_value() -> RetrievalFilterTypeDef:
    return {
        "equals": ...,
    }


# RetrievalFilterTypeDef definition

class RetrievalFilterTypeDef(TypedDict):
    equals: NotRequired[FilterAttributeTypeDef],  # (1)
    notEquals: NotRequired[FilterAttributeTypeDef],  # (1)
    greaterThan: NotRequired[FilterAttributeTypeDef],  # (1)
    greaterThanOrEquals: NotRequired[FilterAttributeTypeDef],  # (1)
    lessThan: NotRequired[FilterAttributeTypeDef],  # (1)
    lessThanOrEquals: NotRequired[FilterAttributeTypeDef],  # (1)
    in: NotRequired[FilterAttributeTypeDef],  # (1)
    notIn: NotRequired[FilterAttributeTypeDef],  # (1)
    startsWith: NotRequired[FilterAttributeTypeDef],  # (1)
    listContains: NotRequired[FilterAttributeTypeDef],  # (1)
    stringContains: NotRequired[FilterAttributeTypeDef],  # (1)
    andAll: NotRequired[Sequence[Mapping[str, Any]]],
    orAll: NotRequired[Sequence[Mapping[str, Any]]],
```

1. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
2. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
3. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
4. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
5. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
6. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
7. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
8. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
9. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
10. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
11. See [:material-code-braces: FilterAttributeTypeDef](./type_defs.md#filterattributetypedef) 
## FoundationModelDetailsTypeDef

```python
# FoundationModelDetailsTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import FoundationModelDetailsTypeDef


def get_value() -> FoundationModelDetailsTypeDef:
    return {
        "modelArn": ...,
    }


# FoundationModelDetailsTypeDef definition

class FoundationModelDetailsTypeDef(TypedDict):
    modelArn: str,
    modelId: str,
    modelName: NotRequired[str],
    providerName: NotRequired[str],
    inputModalities: NotRequired[List[ModelModalityType]],  # (1)
    outputModalities: NotRequired[List[ModelModalityType]],  # (1)
    responseStreamingSupported: NotRequired[bool],
    customizationsSupported: NotRequired[List[ModelCustomizationType]],  # (3)
    inferenceTypesSupported: NotRequired[List[InferenceTypeType]],  # (4)
    modelLifecycle: NotRequired[FoundationModelLifecycleTypeDef],  # (5)
```

1. See [:material-code-brackets: ModelModalityType](./literals.md#modelmodalitytype) 
2. See [:material-code-brackets: ModelModalityType](./literals.md#modelmodalitytype) 
3. See [:material-code-brackets: ModelCustomizationType](./literals.md#modelcustomizationtype) 
4. See [:material-code-brackets: InferenceTypeType](./literals.md#inferencetypetype) 
5. See [:material-code-braces: FoundationModelLifecycleTypeDef](./type_defs.md#foundationmodellifecycletypedef) 
## FoundationModelSummaryTypeDef

```python
# FoundationModelSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import FoundationModelSummaryTypeDef


def get_value() -> FoundationModelSummaryTypeDef:
    return {
        "modelArn": ...,
    }


# FoundationModelSummaryTypeDef definition

class FoundationModelSummaryTypeDef(TypedDict):
    modelArn: str,
    modelId: str,
    modelName: NotRequired[str],
    providerName: NotRequired[str],
    inputModalities: NotRequired[List[ModelModalityType]],  # (1)
    outputModalities: NotRequired[List[ModelModalityType]],  # (1)
    responseStreamingSupported: NotRequired[bool],
    customizationsSupported: NotRequired[List[ModelCustomizationType]],  # (3)
    inferenceTypesSupported: NotRequired[List[InferenceTypeType]],  # (4)
    modelLifecycle: NotRequired[FoundationModelLifecycleTypeDef],  # (5)
```

1. See [:material-code-brackets: ModelModalityType](./literals.md#modelmodalitytype) 
2. See [:material-code-brackets: ModelModalityType](./literals.md#modelmodalitytype) 
3. See [:material-code-brackets: ModelCustomizationType](./literals.md#modelcustomizationtype) 
4. See [:material-code-brackets: InferenceTypeType](./literals.md#inferencetypetype) 
5. See [:material-code-braces: FoundationModelLifecycleTypeDef](./type_defs.md#foundationmodellifecycletypedef) 
## GetInferenceProfileResponseTypeDef

```python
# GetInferenceProfileResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GetInferenceProfileResponseTypeDef


def get_value() -> GetInferenceProfileResponseTypeDef:
    return {
        "inferenceProfileName": ...,
    }


# GetInferenceProfileResponseTypeDef definition

class GetInferenceProfileResponseTypeDef(TypedDict):
    inferenceProfileName: str,
    description: str,
    createdAt: datetime,
    updatedAt: datetime,
    inferenceProfileArn: str,
    models: List[InferenceProfileModelTypeDef],  # (1)
    inferenceProfileId: str,
    status: InferenceProfileStatusType,  # (2)
    type: InferenceProfileTypeType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: InferenceProfileModelTypeDef](./type_defs.md#inferenceprofilemodeltypedef) 
2. See [:material-code-brackets: InferenceProfileStatusType](./literals.md#inferenceprofilestatustype) 
3. See [:material-code-brackets: InferenceProfileTypeType](./literals.md#inferenceprofiletypetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InferenceProfileSummaryTypeDef

```python
# InferenceProfileSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import InferenceProfileSummaryTypeDef


def get_value() -> InferenceProfileSummaryTypeDef:
    return {
        "inferenceProfileName": ...,
    }


# InferenceProfileSummaryTypeDef definition

class InferenceProfileSummaryTypeDef(TypedDict):
    inferenceProfileName: str,
    inferenceProfileArn: str,
    models: List[InferenceProfileModelTypeDef],  # (1)
    inferenceProfileId: str,
    status: InferenceProfileStatusType,  # (2)
    type: InferenceProfileTypeType,  # (3)
    description: NotRequired[str],
    createdAt: NotRequired[datetime],
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-braces: InferenceProfileModelTypeDef](./type_defs.md#inferenceprofilemodeltypedef) 
2. See [:material-code-brackets: InferenceProfileStatusType](./literals.md#inferenceprofilestatustype) 
3. See [:material-code-brackets: InferenceProfileTypeType](./literals.md#inferenceprofiletypetype) 
## SageMakerEndpointOutputTypeDef

```python
# SageMakerEndpointOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import SageMakerEndpointOutputTypeDef


def get_value() -> SageMakerEndpointOutputTypeDef:
    return {
        "initialInstanceCount": ...,
    }


# SageMakerEndpointOutputTypeDef definition

class SageMakerEndpointOutputTypeDef(TypedDict):
    initialInstanceCount: int,
    instanceType: str,
    executionRole: str,
    kmsEncryptionKey: NotRequired[str],
    vpc: NotRequired[VpcConfigOutputTypeDef],  # (1)
```

1. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
## GetPromptRouterResponseTypeDef

```python
# GetPromptRouterResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GetPromptRouterResponseTypeDef


def get_value() -> GetPromptRouterResponseTypeDef:
    return {
        "promptRouterName": ...,
    }


# GetPromptRouterResponseTypeDef definition

class GetPromptRouterResponseTypeDef(TypedDict):
    promptRouterName: str,
    routingCriteria: RoutingCriteriaTypeDef,  # (1)
    description: str,
    createdAt: datetime,
    updatedAt: datetime,
    promptRouterArn: str,
    models: List[PromptRouterTargetModelTypeDef],  # (2)
    fallbackModel: PromptRouterTargetModelTypeDef,  # (3)
    status: PromptRouterStatusType,  # (4)
    type: PromptRouterTypeType,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: RoutingCriteriaTypeDef](./type_defs.md#routingcriteriatypedef) 
2. See [:material-code-braces: PromptRouterTargetModelTypeDef](./type_defs.md#promptroutertargetmodeltypedef) 
3. See [:material-code-braces: PromptRouterTargetModelTypeDef](./type_defs.md#promptroutertargetmodeltypedef) 
4. See [:material-code-brackets: PromptRouterStatusType](./literals.md#promptrouterstatustype) 
5. See [:material-code-brackets: PromptRouterTypeType](./literals.md#promptroutertypetype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PromptRouterSummaryTypeDef

```python
# PromptRouterSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import PromptRouterSummaryTypeDef


def get_value() -> PromptRouterSummaryTypeDef:
    return {
        "promptRouterName": ...,
    }


# PromptRouterSummaryTypeDef definition

class PromptRouterSummaryTypeDef(TypedDict):
    promptRouterName: str,
    routingCriteria: RoutingCriteriaTypeDef,  # (1)
    promptRouterArn: str,
    models: List[PromptRouterTargetModelTypeDef],  # (2)
    fallbackModel: PromptRouterTargetModelTypeDef,  # (3)
    status: PromptRouterStatusType,  # (4)
    type: PromptRouterTypeType,  # (5)
    description: NotRequired[str],
    createdAt: NotRequired[datetime],
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-braces: RoutingCriteriaTypeDef](./type_defs.md#routingcriteriatypedef) 
2. See [:material-code-braces: PromptRouterTargetModelTypeDef](./type_defs.md#promptroutertargetmodeltypedef) 
3. See [:material-code-braces: PromptRouterTargetModelTypeDef](./type_defs.md#promptroutertargetmodeltypedef) 
4. See [:material-code-brackets: PromptRouterStatusType](./literals.md#promptrouterstatustype) 
5. See [:material-code-brackets: PromptRouterTypeType](./literals.md#promptroutertypetype) 
## GuardrailContentPolicyConfigTypeDef

```python
# GuardrailContentPolicyConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GuardrailContentPolicyConfigTypeDef


def get_value() -> GuardrailContentPolicyConfigTypeDef:
    return {
        "filtersConfig": ...,
    }


# GuardrailContentPolicyConfigTypeDef definition

class GuardrailContentPolicyConfigTypeDef(TypedDict):
    filtersConfig: Sequence[GuardrailContentFilterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: GuardrailContentFilterConfigTypeDef](./type_defs.md#guardrailcontentfilterconfigtypedef) 
## GuardrailContentPolicyTypeDef

```python
# GuardrailContentPolicyTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GuardrailContentPolicyTypeDef


def get_value() -> GuardrailContentPolicyTypeDef:
    return {
        "filters": ...,
    }


# GuardrailContentPolicyTypeDef definition

class GuardrailContentPolicyTypeDef(TypedDict):
    filters: NotRequired[List[GuardrailContentFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: GuardrailContentFilterTypeDef](./type_defs.md#guardrailcontentfiltertypedef) 
## GuardrailContextualGroundingPolicyConfigTypeDef

```python
# GuardrailContextualGroundingPolicyConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GuardrailContextualGroundingPolicyConfigTypeDef


def get_value() -> GuardrailContextualGroundingPolicyConfigTypeDef:
    return {
        "filtersConfig": ...,
    }


# GuardrailContextualGroundingPolicyConfigTypeDef definition

class GuardrailContextualGroundingPolicyConfigTypeDef(TypedDict):
    filtersConfig: Sequence[GuardrailContextualGroundingFilterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: GuardrailContextualGroundingFilterConfigTypeDef](./type_defs.md#guardrailcontextualgroundingfilterconfigtypedef) 
## GuardrailContextualGroundingPolicyTypeDef

```python
# GuardrailContextualGroundingPolicyTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GuardrailContextualGroundingPolicyTypeDef


def get_value() -> GuardrailContextualGroundingPolicyTypeDef:
    return {
        "filters": ...,
    }


# GuardrailContextualGroundingPolicyTypeDef definition

class GuardrailContextualGroundingPolicyTypeDef(TypedDict):
    filters: List[GuardrailContextualGroundingFilterTypeDef],  # (1)
```

1. See [:material-code-braces: GuardrailContextualGroundingFilterTypeDef](./type_defs.md#guardrailcontextualgroundingfiltertypedef) 
## GuardrailSensitiveInformationPolicyConfigTypeDef

```python
# GuardrailSensitiveInformationPolicyConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GuardrailSensitiveInformationPolicyConfigTypeDef


def get_value() -> GuardrailSensitiveInformationPolicyConfigTypeDef:
    return {
        "piiEntitiesConfig": ...,
    }


# GuardrailSensitiveInformationPolicyConfigTypeDef definition

class GuardrailSensitiveInformationPolicyConfigTypeDef(TypedDict):
    piiEntitiesConfig: NotRequired[Sequence[GuardrailPiiEntityConfigTypeDef]],  # (1)
    regexesConfig: NotRequired[Sequence[GuardrailRegexConfigTypeDef]],  # (2)
```

1. See [:material-code-braces: GuardrailPiiEntityConfigTypeDef](./type_defs.md#guardrailpiientityconfigtypedef) 
2. See [:material-code-braces: GuardrailRegexConfigTypeDef](./type_defs.md#guardrailregexconfigtypedef) 
## GuardrailSensitiveInformationPolicyTypeDef

```python
# GuardrailSensitiveInformationPolicyTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GuardrailSensitiveInformationPolicyTypeDef


def get_value() -> GuardrailSensitiveInformationPolicyTypeDef:
    return {
        "piiEntities": ...,
    }


# GuardrailSensitiveInformationPolicyTypeDef definition

class GuardrailSensitiveInformationPolicyTypeDef(TypedDict):
    piiEntities: NotRequired[List[GuardrailPiiEntityTypeDef]],  # (1)
    regexes: NotRequired[List[GuardrailRegexTypeDef]],  # (2)
```

1. See [:material-code-braces: GuardrailPiiEntityTypeDef](./type_defs.md#guardrailpiientitytypedef) 
2. See [:material-code-braces: GuardrailRegexTypeDef](./type_defs.md#guardrailregextypedef) 
## ListGuardrailsResponseTypeDef

```python
# ListGuardrailsResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListGuardrailsResponseTypeDef


def get_value() -> ListGuardrailsResponseTypeDef:
    return {
        "guardrails": ...,
    }


# ListGuardrailsResponseTypeDef definition

class ListGuardrailsResponseTypeDef(TypedDict):
    guardrails: List[GuardrailSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: GuardrailSummaryTypeDef](./type_defs.md#guardrailsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GuardrailTopicPolicyConfigTypeDef

```python
# GuardrailTopicPolicyConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GuardrailTopicPolicyConfigTypeDef


def get_value() -> GuardrailTopicPolicyConfigTypeDef:
    return {
        "topicsConfig": ...,
    }


# GuardrailTopicPolicyConfigTypeDef definition

class GuardrailTopicPolicyConfigTypeDef(TypedDict):
    topicsConfig: Sequence[GuardrailTopicConfigTypeDef],  # (1)
```

1. See [:material-code-braces: GuardrailTopicConfigTypeDef](./type_defs.md#guardrailtopicconfigtypedef) 
## GuardrailTopicPolicyTypeDef

```python
# GuardrailTopicPolicyTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GuardrailTopicPolicyTypeDef


def get_value() -> GuardrailTopicPolicyTypeDef:
    return {
        "topics": ...,
    }


# GuardrailTopicPolicyTypeDef definition

class GuardrailTopicPolicyTypeDef(TypedDict):
    topics: List[GuardrailTopicTypeDef],  # (1)
```

1. See [:material-code-braces: GuardrailTopicTypeDef](./type_defs.md#guardrailtopictypedef) 
## GuardrailWordPolicyConfigTypeDef

```python
# GuardrailWordPolicyConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GuardrailWordPolicyConfigTypeDef


def get_value() -> GuardrailWordPolicyConfigTypeDef:
    return {
        "wordsConfig": ...,
    }


# GuardrailWordPolicyConfigTypeDef definition

class GuardrailWordPolicyConfigTypeDef(TypedDict):
    wordsConfig: NotRequired[Sequence[GuardrailWordConfigTypeDef]],  # (1)
    managedWordListsConfig: NotRequired[Sequence[GuardrailManagedWordsConfigTypeDef]],  # (2)
```

1. See [:material-code-braces: GuardrailWordConfigTypeDef](./type_defs.md#guardrailwordconfigtypedef) 
2. See [:material-code-braces: GuardrailManagedWordsConfigTypeDef](./type_defs.md#guardrailmanagedwordsconfigtypedef) 
## GuardrailWordPolicyTypeDef

```python
# GuardrailWordPolicyTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GuardrailWordPolicyTypeDef


def get_value() -> GuardrailWordPolicyTypeDef:
    return {
        "words": ...,
    }


# GuardrailWordPolicyTypeDef definition

class GuardrailWordPolicyTypeDef(TypedDict):
    words: NotRequired[List[GuardrailWordTypeDef]],  # (1)
    managedWordLists: NotRequired[List[GuardrailManagedWordsTypeDef]],  # (2)
```

1. See [:material-code-braces: GuardrailWordTypeDef](./type_defs.md#guardrailwordtypedef) 
2. See [:material-code-braces: GuardrailManagedWordsTypeDef](./type_defs.md#guardrailmanagedwordstypedef) 
## ListImportedModelsResponseTypeDef

```python
# ListImportedModelsResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListImportedModelsResponseTypeDef


def get_value() -> ListImportedModelsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListImportedModelsResponseTypeDef definition

class ListImportedModelsResponseTypeDef(TypedDict):
    modelSummaries: List[ImportedModelSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ImportedModelSummaryTypeDef](./type_defs.md#importedmodelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## KbInferenceConfigOutputTypeDef

```python
# KbInferenceConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import KbInferenceConfigOutputTypeDef


def get_value() -> KbInferenceConfigOutputTypeDef:
    return {
        "textInferenceConfig": ...,
    }


# KbInferenceConfigOutputTypeDef definition

class KbInferenceConfigOutputTypeDef(TypedDict):
    textInferenceConfig: NotRequired[TextInferenceConfigOutputTypeDef],  # (1)
```

1. See [:material-code-braces: TextInferenceConfigOutputTypeDef](./type_defs.md#textinferenceconfigoutputtypedef) 
## KbInferenceConfigTypeDef

```python
# KbInferenceConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import KbInferenceConfigTypeDef


def get_value() -> KbInferenceConfigTypeDef:
    return {
        "textInferenceConfig": ...,
    }


# KbInferenceConfigTypeDef definition

class KbInferenceConfigTypeDef(TypedDict):
    textInferenceConfig: NotRequired[TextInferenceConfigTypeDef],  # (1)
```

1. See [:material-code-braces: TextInferenceConfigTypeDef](./type_defs.md#textinferenceconfigtypedef) 
## ListGuardrailsRequestPaginateTypeDef

```python
# ListGuardrailsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListGuardrailsRequestPaginateTypeDef


def get_value() -> ListGuardrailsRequestPaginateTypeDef:
    return {
        "guardrailIdentifier": ...,
    }


# ListGuardrailsRequestPaginateTypeDef definition

class ListGuardrailsRequestPaginateTypeDef(TypedDict):
    guardrailIdentifier: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInferenceProfilesRequestPaginateTypeDef

```python
# ListInferenceProfilesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListInferenceProfilesRequestPaginateTypeDef


def get_value() -> ListInferenceProfilesRequestPaginateTypeDef:
    return {
        "typeEquals": ...,
    }


# ListInferenceProfilesRequestPaginateTypeDef definition

class ListInferenceProfilesRequestPaginateTypeDef(TypedDict):
    typeEquals: NotRequired[InferenceProfileTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: InferenceProfileTypeType](./literals.md#inferenceprofiletypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMarketplaceModelEndpointsRequestPaginateTypeDef

```python
# ListMarketplaceModelEndpointsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListMarketplaceModelEndpointsRequestPaginateTypeDef


def get_value() -> ListMarketplaceModelEndpointsRequestPaginateTypeDef:
    return {
        "modelSourceEquals": ...,
    }


# ListMarketplaceModelEndpointsRequestPaginateTypeDef definition

class ListMarketplaceModelEndpointsRequestPaginateTypeDef(TypedDict):
    modelSourceEquals: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPromptRoutersRequestPaginateTypeDef

```python
# ListPromptRoutersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListPromptRoutersRequestPaginateTypeDef


def get_value() -> ListPromptRoutersRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListPromptRoutersRequestPaginateTypeDef definition

class ListPromptRoutersRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCustomModelsRequestPaginateTypeDef

```python
# ListCustomModelsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListCustomModelsRequestPaginateTypeDef


def get_value() -> ListCustomModelsRequestPaginateTypeDef:
    return {
        "creationTimeBefore": ...,
    }


# ListCustomModelsRequestPaginateTypeDef definition

class ListCustomModelsRequestPaginateTypeDef(TypedDict):
    creationTimeBefore: NotRequired[TimestampTypeDef],
    creationTimeAfter: NotRequired[TimestampTypeDef],
    nameContains: NotRequired[str],
    baseModelArnEquals: NotRequired[str],
    foundationModelArnEquals: NotRequired[str],
    sortBy: NotRequired[SortModelsByType],  # (1)
    sortOrder: NotRequired[SortOrderType],  # (2)
    isOwned: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SortModelsByType](./literals.md#sortmodelsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCustomModelsRequestTypeDef

```python
# ListCustomModelsRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListCustomModelsRequestTypeDef


def get_value() -> ListCustomModelsRequestTypeDef:
    return {
        "creationTimeBefore": ...,
    }


# ListCustomModelsRequestTypeDef definition

class ListCustomModelsRequestTypeDef(TypedDict):
    creationTimeBefore: NotRequired[TimestampTypeDef],
    creationTimeAfter: NotRequired[TimestampTypeDef],
    nameContains: NotRequired[str],
    baseModelArnEquals: NotRequired[str],
    foundationModelArnEquals: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    sortBy: NotRequired[SortModelsByType],  # (1)
    sortOrder: NotRequired[SortOrderType],  # (2)
    isOwned: NotRequired[bool],
```

1. See [:material-code-brackets: SortModelsByType](./literals.md#sortmodelsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListEvaluationJobsRequestPaginateTypeDef

```python
# ListEvaluationJobsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListEvaluationJobsRequestPaginateTypeDef


def get_value() -> ListEvaluationJobsRequestPaginateTypeDef:
    return {
        "creationTimeAfter": ...,
    }


# ListEvaluationJobsRequestPaginateTypeDef definition

class ListEvaluationJobsRequestPaginateTypeDef(TypedDict):
    creationTimeAfter: NotRequired[TimestampTypeDef],
    creationTimeBefore: NotRequired[TimestampTypeDef],
    statusEquals: NotRequired[EvaluationJobStatusType],  # (1)
    applicationTypeEquals: NotRequired[ApplicationTypeType],  # (2)
    nameContains: NotRequired[str],
    sortBy: NotRequired[SortJobsByType],  # (3)
    sortOrder: NotRequired[SortOrderType],  # (4)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (5)
```

1. See [:material-code-brackets: EvaluationJobStatusType](./literals.md#evaluationjobstatustype) 
2. See [:material-code-brackets: ApplicationTypeType](./literals.md#applicationtypetype) 
3. See [:material-code-brackets: SortJobsByType](./literals.md#sortjobsbytype) 
4. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEvaluationJobsRequestTypeDef

```python
# ListEvaluationJobsRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListEvaluationJobsRequestTypeDef


def get_value() -> ListEvaluationJobsRequestTypeDef:
    return {
        "creationTimeAfter": ...,
    }


# ListEvaluationJobsRequestTypeDef definition

class ListEvaluationJobsRequestTypeDef(TypedDict):
    creationTimeAfter: NotRequired[TimestampTypeDef],
    creationTimeBefore: NotRequired[TimestampTypeDef],
    statusEquals: NotRequired[EvaluationJobStatusType],  # (1)
    applicationTypeEquals: NotRequired[ApplicationTypeType],  # (2)
    nameContains: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    sortBy: NotRequired[SortJobsByType],  # (3)
    sortOrder: NotRequired[SortOrderType],  # (4)
```

1. See [:material-code-brackets: EvaluationJobStatusType](./literals.md#evaluationjobstatustype) 
2. See [:material-code-brackets: ApplicationTypeType](./literals.md#applicationtypetype) 
3. See [:material-code-brackets: SortJobsByType](./literals.md#sortjobsbytype) 
4. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListImportedModelsRequestPaginateTypeDef

```python
# ListImportedModelsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListImportedModelsRequestPaginateTypeDef


def get_value() -> ListImportedModelsRequestPaginateTypeDef:
    return {
        "creationTimeBefore": ...,
    }


# ListImportedModelsRequestPaginateTypeDef definition

class ListImportedModelsRequestPaginateTypeDef(TypedDict):
    creationTimeBefore: NotRequired[TimestampTypeDef],
    creationTimeAfter: NotRequired[TimestampTypeDef],
    nameContains: NotRequired[str],
    sortBy: NotRequired[SortModelsByType],  # (1)
    sortOrder: NotRequired[SortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SortModelsByType](./literals.md#sortmodelsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListImportedModelsRequestTypeDef

```python
# ListImportedModelsRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListImportedModelsRequestTypeDef


def get_value() -> ListImportedModelsRequestTypeDef:
    return {
        "creationTimeBefore": ...,
    }


# ListImportedModelsRequestTypeDef definition

class ListImportedModelsRequestTypeDef(TypedDict):
    creationTimeBefore: NotRequired[TimestampTypeDef],
    creationTimeAfter: NotRequired[TimestampTypeDef],
    nameContains: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    sortBy: NotRequired[SortModelsByType],  # (1)
    sortOrder: NotRequired[SortOrderType],  # (2)
```

1. See [:material-code-brackets: SortModelsByType](./literals.md#sortmodelsbytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListModelCopyJobsRequestPaginateTypeDef

```python
# ListModelCopyJobsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListModelCopyJobsRequestPaginateTypeDef


def get_value() -> ListModelCopyJobsRequestPaginateTypeDef:
    return {
        "creationTimeAfter": ...,
    }


# ListModelCopyJobsRequestPaginateTypeDef definition

class ListModelCopyJobsRequestPaginateTypeDef(TypedDict):
    creationTimeAfter: NotRequired[TimestampTypeDef],
    creationTimeBefore: NotRequired[TimestampTypeDef],
    statusEquals: NotRequired[ModelCopyJobStatusType],  # (1)
    sourceAccountEquals: NotRequired[str],
    sourceModelArnEquals: NotRequired[str],
    targetModelNameContains: NotRequired[str],
    sortBy: NotRequired[SortJobsByType],  # (2)
    sortOrder: NotRequired[SortOrderType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: ModelCopyJobStatusType](./literals.md#modelcopyjobstatustype) 
2. See [:material-code-brackets: SortJobsByType](./literals.md#sortjobsbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListModelCopyJobsRequestTypeDef

```python
# ListModelCopyJobsRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListModelCopyJobsRequestTypeDef


def get_value() -> ListModelCopyJobsRequestTypeDef:
    return {
        "creationTimeAfter": ...,
    }


# ListModelCopyJobsRequestTypeDef definition

class ListModelCopyJobsRequestTypeDef(TypedDict):
    creationTimeAfter: NotRequired[TimestampTypeDef],
    creationTimeBefore: NotRequired[TimestampTypeDef],
    statusEquals: NotRequired[ModelCopyJobStatusType],  # (1)
    sourceAccountEquals: NotRequired[str],
    sourceModelArnEquals: NotRequired[str],
    targetModelNameContains: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    sortBy: NotRequired[SortJobsByType],  # (2)
    sortOrder: NotRequired[SortOrderType],  # (3)
```

1. See [:material-code-brackets: ModelCopyJobStatusType](./literals.md#modelcopyjobstatustype) 
2. See [:material-code-brackets: SortJobsByType](./literals.md#sortjobsbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListModelCustomizationJobsRequestPaginateTypeDef

```python
# ListModelCustomizationJobsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListModelCustomizationJobsRequestPaginateTypeDef


def get_value() -> ListModelCustomizationJobsRequestPaginateTypeDef:
    return {
        "creationTimeAfter": ...,
    }


# ListModelCustomizationJobsRequestPaginateTypeDef definition

class ListModelCustomizationJobsRequestPaginateTypeDef(TypedDict):
    creationTimeAfter: NotRequired[TimestampTypeDef],
    creationTimeBefore: NotRequired[TimestampTypeDef],
    statusEquals: NotRequired[FineTuningJobStatusType],  # (1)
    nameContains: NotRequired[str],
    sortBy: NotRequired[SortJobsByType],  # (2)
    sortOrder: NotRequired[SortOrderType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: FineTuningJobStatusType](./literals.md#finetuningjobstatustype) 
2. See [:material-code-brackets: SortJobsByType](./literals.md#sortjobsbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListModelCustomizationJobsRequestTypeDef

```python
# ListModelCustomizationJobsRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListModelCustomizationJobsRequestTypeDef


def get_value() -> ListModelCustomizationJobsRequestTypeDef:
    return {
        "creationTimeAfter": ...,
    }


# ListModelCustomizationJobsRequestTypeDef definition

class ListModelCustomizationJobsRequestTypeDef(TypedDict):
    creationTimeAfter: NotRequired[TimestampTypeDef],
    creationTimeBefore: NotRequired[TimestampTypeDef],
    statusEquals: NotRequired[FineTuningJobStatusType],  # (1)
    nameContains: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    sortBy: NotRequired[SortJobsByType],  # (2)
    sortOrder: NotRequired[SortOrderType],  # (3)
```

1. See [:material-code-brackets: FineTuningJobStatusType](./literals.md#finetuningjobstatustype) 
2. See [:material-code-brackets: SortJobsByType](./literals.md#sortjobsbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListModelImportJobsRequestPaginateTypeDef

```python
# ListModelImportJobsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListModelImportJobsRequestPaginateTypeDef


def get_value() -> ListModelImportJobsRequestPaginateTypeDef:
    return {
        "creationTimeAfter": ...,
    }


# ListModelImportJobsRequestPaginateTypeDef definition

class ListModelImportJobsRequestPaginateTypeDef(TypedDict):
    creationTimeAfter: NotRequired[TimestampTypeDef],
    creationTimeBefore: NotRequired[TimestampTypeDef],
    statusEquals: NotRequired[ModelImportJobStatusType],  # (1)
    nameContains: NotRequired[str],
    sortBy: NotRequired[SortJobsByType],  # (2)
    sortOrder: NotRequired[SortOrderType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: ModelImportJobStatusType](./literals.md#modelimportjobstatustype) 
2. See [:material-code-brackets: SortJobsByType](./literals.md#sortjobsbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListModelImportJobsRequestTypeDef

```python
# ListModelImportJobsRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListModelImportJobsRequestTypeDef


def get_value() -> ListModelImportJobsRequestTypeDef:
    return {
        "creationTimeAfter": ...,
    }


# ListModelImportJobsRequestTypeDef definition

class ListModelImportJobsRequestTypeDef(TypedDict):
    creationTimeAfter: NotRequired[TimestampTypeDef],
    creationTimeBefore: NotRequired[TimestampTypeDef],
    statusEquals: NotRequired[ModelImportJobStatusType],  # (1)
    nameContains: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    sortBy: NotRequired[SortJobsByType],  # (2)
    sortOrder: NotRequired[SortOrderType],  # (3)
```

1. See [:material-code-brackets: ModelImportJobStatusType](./literals.md#modelimportjobstatustype) 
2. See [:material-code-brackets: SortJobsByType](./literals.md#sortjobsbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListModelInvocationJobsRequestPaginateTypeDef

```python
# ListModelInvocationJobsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListModelInvocationJobsRequestPaginateTypeDef


def get_value() -> ListModelInvocationJobsRequestPaginateTypeDef:
    return {
        "submitTimeAfter": ...,
    }


# ListModelInvocationJobsRequestPaginateTypeDef definition

class ListModelInvocationJobsRequestPaginateTypeDef(TypedDict):
    submitTimeAfter: NotRequired[TimestampTypeDef],
    submitTimeBefore: NotRequired[TimestampTypeDef],
    statusEquals: NotRequired[ModelInvocationJobStatusType],  # (1)
    nameContains: NotRequired[str],
    sortBy: NotRequired[SortJobsByType],  # (2)
    sortOrder: NotRequired[SortOrderType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: ModelInvocationJobStatusType](./literals.md#modelinvocationjobstatustype) 
2. See [:material-code-brackets: SortJobsByType](./literals.md#sortjobsbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListModelInvocationJobsRequestTypeDef

```python
# ListModelInvocationJobsRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListModelInvocationJobsRequestTypeDef


def get_value() -> ListModelInvocationJobsRequestTypeDef:
    return {
        "submitTimeAfter": ...,
    }


# ListModelInvocationJobsRequestTypeDef definition

class ListModelInvocationJobsRequestTypeDef(TypedDict):
    submitTimeAfter: NotRequired[TimestampTypeDef],
    submitTimeBefore: NotRequired[TimestampTypeDef],
    statusEquals: NotRequired[ModelInvocationJobStatusType],  # (1)
    nameContains: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    sortBy: NotRequired[SortJobsByType],  # (2)
    sortOrder: NotRequired[SortOrderType],  # (3)
```

1. See [:material-code-brackets: ModelInvocationJobStatusType](./literals.md#modelinvocationjobstatustype) 
2. See [:material-code-brackets: SortJobsByType](./literals.md#sortjobsbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListProvisionedModelThroughputsRequestPaginateTypeDef

```python
# ListProvisionedModelThroughputsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListProvisionedModelThroughputsRequestPaginateTypeDef


def get_value() -> ListProvisionedModelThroughputsRequestPaginateTypeDef:
    return {
        "creationTimeAfter": ...,
    }


# ListProvisionedModelThroughputsRequestPaginateTypeDef definition

class ListProvisionedModelThroughputsRequestPaginateTypeDef(TypedDict):
    creationTimeAfter: NotRequired[TimestampTypeDef],
    creationTimeBefore: NotRequired[TimestampTypeDef],
    statusEquals: NotRequired[ProvisionedModelStatusType],  # (1)
    modelArnEquals: NotRequired[str],
    nameContains: NotRequired[str],
    sortBy: NotRequired[SortByProvisionedModelsType],  # (2)
    sortOrder: NotRequired[SortOrderType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: ProvisionedModelStatusType](./literals.md#provisionedmodelstatustype) 
2. See [:material-code-brackets: SortByProvisionedModelsType](./literals.md#sortbyprovisionedmodelstype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProvisionedModelThroughputsRequestTypeDef

```python
# ListProvisionedModelThroughputsRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListProvisionedModelThroughputsRequestTypeDef


def get_value() -> ListProvisionedModelThroughputsRequestTypeDef:
    return {
        "creationTimeAfter": ...,
    }


# ListProvisionedModelThroughputsRequestTypeDef definition

class ListProvisionedModelThroughputsRequestTypeDef(TypedDict):
    creationTimeAfter: NotRequired[TimestampTypeDef],
    creationTimeBefore: NotRequired[TimestampTypeDef],
    statusEquals: NotRequired[ProvisionedModelStatusType],  # (1)
    modelArnEquals: NotRequired[str],
    nameContains: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    sortBy: NotRequired[SortByProvisionedModelsType],  # (2)
    sortOrder: NotRequired[SortOrderType],  # (3)
```

1. See [:material-code-brackets: ProvisionedModelStatusType](./literals.md#provisionedmodelstatustype) 
2. See [:material-code-brackets: SortByProvisionedModelsType](./literals.md#sortbyprovisionedmodelstype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListMarketplaceModelEndpointsResponseTypeDef

```python
# ListMarketplaceModelEndpointsResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListMarketplaceModelEndpointsResponseTypeDef


def get_value() -> ListMarketplaceModelEndpointsResponseTypeDef:
    return {
        "marketplaceModelEndpoints": ...,
    }


# ListMarketplaceModelEndpointsResponseTypeDef definition

class ListMarketplaceModelEndpointsResponseTypeDef(TypedDict):
    marketplaceModelEndpoints: List[MarketplaceModelEndpointSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: MarketplaceModelEndpointSummaryTypeDef](./type_defs.md#marketplacemodelendpointsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListModelCustomizationJobsResponseTypeDef

```python
# ListModelCustomizationJobsResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListModelCustomizationJobsResponseTypeDef


def get_value() -> ListModelCustomizationJobsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListModelCustomizationJobsResponseTypeDef definition

class ListModelCustomizationJobsResponseTypeDef(TypedDict):
    modelCustomizationJobSummaries: List[ModelCustomizationJobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ModelCustomizationJobSummaryTypeDef](./type_defs.md#modelcustomizationjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListModelImportJobsResponseTypeDef

```python
# ListModelImportJobsResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListModelImportJobsResponseTypeDef


def get_value() -> ListModelImportJobsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListModelImportJobsResponseTypeDef definition

class ListModelImportJobsResponseTypeDef(TypedDict):
    modelImportJobSummaries: List[ModelImportJobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ModelImportJobSummaryTypeDef](./type_defs.md#modelimportjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProvisionedModelThroughputsResponseTypeDef

```python
# ListProvisionedModelThroughputsResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListProvisionedModelThroughputsResponseTypeDef


def get_value() -> ListProvisionedModelThroughputsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListProvisionedModelThroughputsResponseTypeDef definition

class ListProvisionedModelThroughputsResponseTypeDef(TypedDict):
    provisionedModelSummaries: List[ProvisionedModelSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ProvisionedModelSummaryTypeDef](./type_defs.md#provisionedmodelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModelDataSourceTypeDef

```python
# ModelDataSourceTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ModelDataSourceTypeDef


def get_value() -> ModelDataSourceTypeDef:
    return {
        "s3DataSource": ...,
    }


# ModelDataSourceTypeDef definition

class ModelDataSourceTypeDef(TypedDict):
    s3DataSource: NotRequired[S3DataSourceTypeDef],  # (1)
```

1. See [:material-code-braces: S3DataSourceTypeDef](./type_defs.md#s3datasourcetypedef) 
## ModelInvocationJobInputDataConfigTypeDef

```python
# ModelInvocationJobInputDataConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ModelInvocationJobInputDataConfigTypeDef


def get_value() -> ModelInvocationJobInputDataConfigTypeDef:
    return {
        "s3InputDataConfig": ...,
    }


# ModelInvocationJobInputDataConfigTypeDef definition

class ModelInvocationJobInputDataConfigTypeDef(TypedDict):
    s3InputDataConfig: NotRequired[ModelInvocationJobS3InputDataConfigTypeDef],  # (1)
```

1. See [:material-code-braces: ModelInvocationJobS3InputDataConfigTypeDef](./type_defs.md#modelinvocationjobs3inputdataconfigtypedef) 
## ModelInvocationJobOutputDataConfigTypeDef

```python
# ModelInvocationJobOutputDataConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ModelInvocationJobOutputDataConfigTypeDef


def get_value() -> ModelInvocationJobOutputDataConfigTypeDef:
    return {
        "s3OutputDataConfig": ...,
    }


# ModelInvocationJobOutputDataConfigTypeDef definition

class ModelInvocationJobOutputDataConfigTypeDef(TypedDict):
    s3OutputDataConfig: NotRequired[ModelInvocationJobS3OutputDataConfigTypeDef],  # (1)
```

1. See [:material-code-braces: ModelInvocationJobS3OutputDataConfigTypeDef](./type_defs.md#modelinvocationjobs3outputdataconfigtypedef) 
## OrchestrationConfigurationTypeDef

```python
# OrchestrationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import OrchestrationConfigurationTypeDef


def get_value() -> OrchestrationConfigurationTypeDef:
    return {
        "queryTransformationConfiguration": ...,
    }


# OrchestrationConfigurationTypeDef definition

class OrchestrationConfigurationTypeDef(TypedDict):
    queryTransformationConfiguration: QueryTransformationConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: QueryTransformationConfigurationTypeDef](./type_defs.md#querytransformationconfigurationtypedef) 
## RequestMetadataFiltersOutputTypeDef

```python
# RequestMetadataFiltersOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import RequestMetadataFiltersOutputTypeDef


def get_value() -> RequestMetadataFiltersOutputTypeDef:
    return {
        "equals": ...,
    }


# RequestMetadataFiltersOutputTypeDef definition

class RequestMetadataFiltersOutputTypeDef(TypedDict):
    equals: NotRequired[Dict[str, str]],
    notEquals: NotRequired[Dict[str, str]],
    andAll: NotRequired[List[RequestMetadataBaseFiltersOutputTypeDef]],  # (1)
    orAll: NotRequired[List[RequestMetadataBaseFiltersOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: RequestMetadataBaseFiltersOutputTypeDef](./type_defs.md#requestmetadatabasefiltersoutputtypedef) 
2. See [:material-code-braces: RequestMetadataBaseFiltersOutputTypeDef](./type_defs.md#requestmetadatabasefiltersoutputtypedef) 
## RequestMetadataFiltersTypeDef

```python
# RequestMetadataFiltersTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import RequestMetadataFiltersTypeDef


def get_value() -> RequestMetadataFiltersTypeDef:
    return {
        "equals": ...,
    }


# RequestMetadataFiltersTypeDef definition

class RequestMetadataFiltersTypeDef(TypedDict):
    equals: NotRequired[Mapping[str, str]],
    notEquals: NotRequired[Mapping[str, str]],
    andAll: NotRequired[Sequence[RequestMetadataBaseFiltersTypeDef]],  # (1)
    orAll: NotRequired[Sequence[RequestMetadataBaseFiltersTypeDef]],  # (1)
```

1. See [:material-code-braces: RequestMetadataBaseFiltersTypeDef](./type_defs.md#requestmetadatabasefilterstypedef) 
2. See [:material-code-braces: RequestMetadataBaseFiltersTypeDef](./type_defs.md#requestmetadatabasefilterstypedef) 
## SageMakerEndpointTypeDef

```python
# SageMakerEndpointTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import SageMakerEndpointTypeDef


def get_value() -> SageMakerEndpointTypeDef:
    return {
        "initialInstanceCount": ...,
    }


# SageMakerEndpointTypeDef definition

class SageMakerEndpointTypeDef(TypedDict):
    initialInstanceCount: int,
    instanceType: str,
    executionRole: str,
    kmsEncryptionKey: NotRequired[str],
    vpc: NotRequired[VpcConfigTypeDef],  # (1)
```

1. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
## ValidationDataConfigOutputTypeDef

```python
# ValidationDataConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ValidationDataConfigOutputTypeDef


def get_value() -> ValidationDataConfigOutputTypeDef:
    return {
        "validators": ...,
    }


# ValidationDataConfigOutputTypeDef definition

class ValidationDataConfigOutputTypeDef(TypedDict):
    validators: List[ValidatorTypeDef],  # (1)
```

1. See [:material-code-braces: ValidatorTypeDef](./type_defs.md#validatortypedef) 
## ValidationDataConfigTypeDef

```python
# ValidationDataConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ValidationDataConfigTypeDef


def get_value() -> ValidationDataConfigTypeDef:
    return {
        "validators": ...,
    }


# ValidationDataConfigTypeDef definition

class ValidationDataConfigTypeDef(TypedDict):
    validators: Sequence[ValidatorTypeDef],  # (1)
```

1. See [:material-code-braces: ValidatorTypeDef](./type_defs.md#validatortypedef) 
## ExternalSourceTypeDef

```python
# ExternalSourceTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ExternalSourceTypeDef


def get_value() -> ExternalSourceTypeDef:
    return {
        "sourceType": ...,
    }


# ExternalSourceTypeDef definition

class ExternalSourceTypeDef(TypedDict):
    sourceType: ExternalSourceTypeType,  # (1)
    s3Location: NotRequired[S3ObjectDocTypeDef],  # (2)
    byteContent: NotRequired[ByteContentDocTypeDef],  # (3)
```

1. See [:material-code-brackets: ExternalSourceTypeType](./literals.md#externalsourcetypetype) 
2. See [:material-code-braces: S3ObjectDocTypeDef](./type_defs.md#s3objectdoctypedef) 
3. See [:material-code-braces: ByteContentDocTypeDef](./type_defs.md#bytecontentdoctypedef) 
## LoggingConfigTypeDef

```python
# LoggingConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import LoggingConfigTypeDef


def get_value() -> LoggingConfigTypeDef:
    return {
        "cloudWatchConfig": ...,
    }


# LoggingConfigTypeDef definition

class LoggingConfigTypeDef(TypedDict):
    cloudWatchConfig: NotRequired[CloudWatchConfigTypeDef],  # (1)
    s3Config: NotRequired[S3ConfigTypeDef],  # (2)
    textDataDeliveryEnabled: NotRequired[bool],
    imageDataDeliveryEnabled: NotRequired[bool],
    embeddingDataDeliveryEnabled: NotRequired[bool],
    videoDataDeliveryEnabled: NotRequired[bool],
```

1. See [:material-code-braces: CloudWatchConfigTypeDef](./type_defs.md#cloudwatchconfigtypedef) 
2. See [:material-code-braces: S3ConfigTypeDef](./type_defs.md#s3configtypedef) 
## ListModelCopyJobsResponseTypeDef

```python
# ListModelCopyJobsResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListModelCopyJobsResponseTypeDef


def get_value() -> ListModelCopyJobsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListModelCopyJobsResponseTypeDef definition

class ListModelCopyJobsResponseTypeDef(TypedDict):
    modelCopyJobSummaries: List[ModelCopyJobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ModelCopyJobSummaryTypeDef](./type_defs.md#modelcopyjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CustomizationConfigTypeDef

```python
# CustomizationConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import CustomizationConfigTypeDef


def get_value() -> CustomizationConfigTypeDef:
    return {
        "distillationConfig": ...,
    }


# CustomizationConfigTypeDef definition

class CustomizationConfigTypeDef(TypedDict):
    distillationConfig: NotRequired[DistillationConfigTypeDef],  # (1)
```

1. See [:material-code-braces: DistillationConfigTypeDef](./type_defs.md#distillationconfigtypedef) 
## EvaluationModelConfigTypeDef

```python
# EvaluationModelConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import EvaluationModelConfigTypeDef


def get_value() -> EvaluationModelConfigTypeDef:
    return {
        "bedrockModel": ...,
    }


# EvaluationModelConfigTypeDef definition

class EvaluationModelConfigTypeDef(TypedDict):
    bedrockModel: NotRequired[EvaluationBedrockModelTypeDef],  # (1)
```

1. See [:material-code-braces: EvaluationBedrockModelTypeDef](./type_defs.md#evaluationbedrockmodeltypedef) 
## EvaluationDatasetMetricConfigOutputTypeDef

```python
# EvaluationDatasetMetricConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import EvaluationDatasetMetricConfigOutputTypeDef


def get_value() -> EvaluationDatasetMetricConfigOutputTypeDef:
    return {
        "taskType": ...,
    }


# EvaluationDatasetMetricConfigOutputTypeDef definition

class EvaluationDatasetMetricConfigOutputTypeDef(TypedDict):
    taskType: EvaluationTaskTypeType,  # (1)
    dataset: EvaluationDatasetTypeDef,  # (2)
    metricNames: List[str],
```

1. See [:material-code-brackets: EvaluationTaskTypeType](./literals.md#evaluationtasktypetype) 
2. See [:material-code-braces: EvaluationDatasetTypeDef](./type_defs.md#evaluationdatasettypedef) 
## EvaluationDatasetMetricConfigTypeDef

```python
# EvaluationDatasetMetricConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import EvaluationDatasetMetricConfigTypeDef


def get_value() -> EvaluationDatasetMetricConfigTypeDef:
    return {
        "taskType": ...,
    }


# EvaluationDatasetMetricConfigTypeDef definition

class EvaluationDatasetMetricConfigTypeDef(TypedDict):
    taskType: EvaluationTaskTypeType,  # (1)
    dataset: EvaluationDatasetTypeDef,  # (2)
    metricNames: Sequence[str],
```

1. See [:material-code-brackets: EvaluationTaskTypeType](./literals.md#evaluationtasktypetype) 
2. See [:material-code-braces: EvaluationDatasetTypeDef](./type_defs.md#evaluationdatasettypedef) 
## KnowledgeBaseVectorSearchConfigurationOutputTypeDef

```python
# KnowledgeBaseVectorSearchConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import KnowledgeBaseVectorSearchConfigurationOutputTypeDef


def get_value() -> KnowledgeBaseVectorSearchConfigurationOutputTypeDef:
    return {
        "numberOfResults": ...,
    }


# KnowledgeBaseVectorSearchConfigurationOutputTypeDef definition

class KnowledgeBaseVectorSearchConfigurationOutputTypeDef(TypedDict):
    numberOfResults: NotRequired[int],
    overrideSearchType: NotRequired[SearchTypeType],  # (1)
    filter: NotRequired[RetrievalFilterOutputTypeDef],  # (2)
```

1. See [:material-code-brackets: SearchTypeType](./literals.md#searchtypetype) 
2. See [:material-code-braces: RetrievalFilterOutputTypeDef](./type_defs.md#retrievalfilteroutputtypedef) 
## KnowledgeBaseVectorSearchConfigurationTypeDef

```python
# KnowledgeBaseVectorSearchConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import KnowledgeBaseVectorSearchConfigurationTypeDef


def get_value() -> KnowledgeBaseVectorSearchConfigurationTypeDef:
    return {
        "numberOfResults": ...,
    }


# KnowledgeBaseVectorSearchConfigurationTypeDef definition

class KnowledgeBaseVectorSearchConfigurationTypeDef(TypedDict):
    numberOfResults: NotRequired[int],
    overrideSearchType: NotRequired[SearchTypeType],  # (1)
    filter: NotRequired[RetrievalFilterTypeDef],  # (2)
```

1. See [:material-code-brackets: SearchTypeType](./literals.md#searchtypetype) 
2. See [:material-code-braces: RetrievalFilterTypeDef](./type_defs.md#retrievalfiltertypedef) 
## GetFoundationModelResponseTypeDef

```python
# GetFoundationModelResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GetFoundationModelResponseTypeDef


def get_value() -> GetFoundationModelResponseTypeDef:
    return {
        "modelDetails": ...,
    }


# GetFoundationModelResponseTypeDef definition

class GetFoundationModelResponseTypeDef(TypedDict):
    modelDetails: FoundationModelDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FoundationModelDetailsTypeDef](./type_defs.md#foundationmodeldetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFoundationModelsResponseTypeDef

```python
# ListFoundationModelsResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListFoundationModelsResponseTypeDef


def get_value() -> ListFoundationModelsResponseTypeDef:
    return {
        "modelSummaries": ...,
    }


# ListFoundationModelsResponseTypeDef definition

class ListFoundationModelsResponseTypeDef(TypedDict):
    modelSummaries: List[FoundationModelSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FoundationModelSummaryTypeDef](./type_defs.md#foundationmodelsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListInferenceProfilesResponseTypeDef

```python
# ListInferenceProfilesResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListInferenceProfilesResponseTypeDef


def get_value() -> ListInferenceProfilesResponseTypeDef:
    return {
        "inferenceProfileSummaries": ...,
    }


# ListInferenceProfilesResponseTypeDef definition

class ListInferenceProfilesResponseTypeDef(TypedDict):
    inferenceProfileSummaries: List[InferenceProfileSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: InferenceProfileSummaryTypeDef](./type_defs.md#inferenceprofilesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EndpointConfigOutputTypeDef

```python
# EndpointConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import EndpointConfigOutputTypeDef


def get_value() -> EndpointConfigOutputTypeDef:
    return {
        "sageMaker": ...,
    }


# EndpointConfigOutputTypeDef definition

class EndpointConfigOutputTypeDef(TypedDict):
    sageMaker: NotRequired[SageMakerEndpointOutputTypeDef],  # (1)
```

1. See [:material-code-braces: SageMakerEndpointOutputTypeDef](./type_defs.md#sagemakerendpointoutputtypedef) 
## ListPromptRoutersResponseTypeDef

```python
# ListPromptRoutersResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListPromptRoutersResponseTypeDef


def get_value() -> ListPromptRoutersResponseTypeDef:
    return {
        "promptRouterSummaries": ...,
    }


# ListPromptRoutersResponseTypeDef definition

class ListPromptRoutersResponseTypeDef(TypedDict):
    promptRouterSummaries: List[PromptRouterSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PromptRouterSummaryTypeDef](./type_defs.md#promptroutersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGuardrailRequestTypeDef

```python
# CreateGuardrailRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import CreateGuardrailRequestTypeDef


def get_value() -> CreateGuardrailRequestTypeDef:
    return {
        "name": ...,
    }


# CreateGuardrailRequestTypeDef definition

class CreateGuardrailRequestTypeDef(TypedDict):
    name: str,
    blockedInputMessaging: str,
    blockedOutputsMessaging: str,
    description: NotRequired[str],
    topicPolicyConfig: NotRequired[GuardrailTopicPolicyConfigTypeDef],  # (1)
    contentPolicyConfig: NotRequired[GuardrailContentPolicyConfigTypeDef],  # (2)
    wordPolicyConfig: NotRequired[GuardrailWordPolicyConfigTypeDef],  # (3)
    sensitiveInformationPolicyConfig: NotRequired[GuardrailSensitiveInformationPolicyConfigTypeDef],  # (4)
    contextualGroundingPolicyConfig: NotRequired[GuardrailContextualGroundingPolicyConfigTypeDef],  # (5)
    kmsKeyId: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (6)
    clientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: GuardrailTopicPolicyConfigTypeDef](./type_defs.md#guardrailtopicpolicyconfigtypedef) 
2. See [:material-code-braces: GuardrailContentPolicyConfigTypeDef](./type_defs.md#guardrailcontentpolicyconfigtypedef) 
3. See [:material-code-braces: GuardrailWordPolicyConfigTypeDef](./type_defs.md#guardrailwordpolicyconfigtypedef) 
4. See [:material-code-braces: GuardrailSensitiveInformationPolicyConfigTypeDef](./type_defs.md#guardrailsensitiveinformationpolicyconfigtypedef) 
5. See [:material-code-braces: GuardrailContextualGroundingPolicyConfigTypeDef](./type_defs.md#guardrailcontextualgroundingpolicyconfigtypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateGuardrailRequestTypeDef

```python
# UpdateGuardrailRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import UpdateGuardrailRequestTypeDef


def get_value() -> UpdateGuardrailRequestTypeDef:
    return {
        "guardrailIdentifier": ...,
    }


# UpdateGuardrailRequestTypeDef definition

class UpdateGuardrailRequestTypeDef(TypedDict):
    guardrailIdentifier: str,
    name: str,
    blockedInputMessaging: str,
    blockedOutputsMessaging: str,
    description: NotRequired[str],
    topicPolicyConfig: NotRequired[GuardrailTopicPolicyConfigTypeDef],  # (1)
    contentPolicyConfig: NotRequired[GuardrailContentPolicyConfigTypeDef],  # (2)
    wordPolicyConfig: NotRequired[GuardrailWordPolicyConfigTypeDef],  # (3)
    sensitiveInformationPolicyConfig: NotRequired[GuardrailSensitiveInformationPolicyConfigTypeDef],  # (4)
    contextualGroundingPolicyConfig: NotRequired[GuardrailContextualGroundingPolicyConfigTypeDef],  # (5)
    kmsKeyId: NotRequired[str],
```

1. See [:material-code-braces: GuardrailTopicPolicyConfigTypeDef](./type_defs.md#guardrailtopicpolicyconfigtypedef) 
2. See [:material-code-braces: GuardrailContentPolicyConfigTypeDef](./type_defs.md#guardrailcontentpolicyconfigtypedef) 
3. See [:material-code-braces: GuardrailWordPolicyConfigTypeDef](./type_defs.md#guardrailwordpolicyconfigtypedef) 
4. See [:material-code-braces: GuardrailSensitiveInformationPolicyConfigTypeDef](./type_defs.md#guardrailsensitiveinformationpolicyconfigtypedef) 
5. See [:material-code-braces: GuardrailContextualGroundingPolicyConfigTypeDef](./type_defs.md#guardrailcontextualgroundingpolicyconfigtypedef) 
## GetGuardrailResponseTypeDef

```python
# GetGuardrailResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GetGuardrailResponseTypeDef


def get_value() -> GetGuardrailResponseTypeDef:
    return {
        "name": ...,
    }


# GetGuardrailResponseTypeDef definition

class GetGuardrailResponseTypeDef(TypedDict):
    name: str,
    description: str,
    guardrailId: str,
    guardrailArn: str,
    version: str,
    status: GuardrailStatusType,  # (1)
    topicPolicy: GuardrailTopicPolicyTypeDef,  # (2)
    contentPolicy: GuardrailContentPolicyTypeDef,  # (3)
    wordPolicy: GuardrailWordPolicyTypeDef,  # (4)
    sensitiveInformationPolicy: GuardrailSensitiveInformationPolicyTypeDef,  # (5)
    contextualGroundingPolicy: GuardrailContextualGroundingPolicyTypeDef,  # (6)
    createdAt: datetime,
    updatedAt: datetime,
    statusReasons: List[str],
    failureRecommendations: List[str],
    blockedInputMessaging: str,
    blockedOutputsMessaging: str,
    kmsKeyArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-brackets: GuardrailStatusType](./literals.md#guardrailstatustype) 
2. See [:material-code-braces: GuardrailTopicPolicyTypeDef](./type_defs.md#guardrailtopicpolicytypedef) 
3. See [:material-code-braces: GuardrailContentPolicyTypeDef](./type_defs.md#guardrailcontentpolicytypedef) 
4. See [:material-code-braces: GuardrailWordPolicyTypeDef](./type_defs.md#guardrailwordpolicytypedef) 
5. See [:material-code-braces: GuardrailSensitiveInformationPolicyTypeDef](./type_defs.md#guardrailsensitiveinformationpolicytypedef) 
6. See [:material-code-braces: GuardrailContextualGroundingPolicyTypeDef](./type_defs.md#guardrailcontextualgroundingpolicytypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExternalSourcesGenerationConfigurationOutputTypeDef

```python
# ExternalSourcesGenerationConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ExternalSourcesGenerationConfigurationOutputTypeDef


def get_value() -> ExternalSourcesGenerationConfigurationOutputTypeDef:
    return {
        "promptTemplate": ...,
    }


# ExternalSourcesGenerationConfigurationOutputTypeDef definition

class ExternalSourcesGenerationConfigurationOutputTypeDef(TypedDict):
    promptTemplate: NotRequired[PromptTemplateTypeDef],  # (1)
    guardrailConfiguration: NotRequired[GuardrailConfigurationTypeDef],  # (2)
    kbInferenceConfig: NotRequired[KbInferenceConfigOutputTypeDef],  # (3)
    additionalModelRequestFields: NotRequired[Dict[str, Dict[str, Any]]],
```

1. See [:material-code-braces: PromptTemplateTypeDef](./type_defs.md#prompttemplatetypedef) 
2. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef) 
3. See [:material-code-braces: KbInferenceConfigOutputTypeDef](./type_defs.md#kbinferenceconfigoutputtypedef) 
## GenerationConfigurationOutputTypeDef

```python
# GenerationConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GenerationConfigurationOutputTypeDef


def get_value() -> GenerationConfigurationOutputTypeDef:
    return {
        "promptTemplate": ...,
    }


# GenerationConfigurationOutputTypeDef definition

class GenerationConfigurationOutputTypeDef(TypedDict):
    promptTemplate: NotRequired[PromptTemplateTypeDef],  # (1)
    guardrailConfiguration: NotRequired[GuardrailConfigurationTypeDef],  # (2)
    kbInferenceConfig: NotRequired[KbInferenceConfigOutputTypeDef],  # (3)
    additionalModelRequestFields: NotRequired[Dict[str, Dict[str, Any]]],
```

1. See [:material-code-braces: PromptTemplateTypeDef](./type_defs.md#prompttemplatetypedef) 
2. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef) 
3. See [:material-code-braces: KbInferenceConfigOutputTypeDef](./type_defs.md#kbinferenceconfigoutputtypedef) 
## ExternalSourcesGenerationConfigurationTypeDef

```python
# ExternalSourcesGenerationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ExternalSourcesGenerationConfigurationTypeDef


def get_value() -> ExternalSourcesGenerationConfigurationTypeDef:
    return {
        "promptTemplate": ...,
    }


# ExternalSourcesGenerationConfigurationTypeDef definition

class ExternalSourcesGenerationConfigurationTypeDef(TypedDict):
    promptTemplate: NotRequired[PromptTemplateTypeDef],  # (1)
    guardrailConfiguration: NotRequired[GuardrailConfigurationTypeDef],  # (2)
    kbInferenceConfig: NotRequired[KbInferenceConfigTypeDef],  # (3)
    additionalModelRequestFields: NotRequired[Mapping[str, Mapping[str, Any]]],
```

1. See [:material-code-braces: PromptTemplateTypeDef](./type_defs.md#prompttemplatetypedef) 
2. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef) 
3. See [:material-code-braces: KbInferenceConfigTypeDef](./type_defs.md#kbinferenceconfigtypedef) 
## GenerationConfigurationTypeDef

```python
# GenerationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GenerationConfigurationTypeDef


def get_value() -> GenerationConfigurationTypeDef:
    return {
        "promptTemplate": ...,
    }


# GenerationConfigurationTypeDef definition

class GenerationConfigurationTypeDef(TypedDict):
    promptTemplate: NotRequired[PromptTemplateTypeDef],  # (1)
    guardrailConfiguration: NotRequired[GuardrailConfigurationTypeDef],  # (2)
    kbInferenceConfig: NotRequired[KbInferenceConfigTypeDef],  # (3)
    additionalModelRequestFields: NotRequired[Mapping[str, Mapping[str, Any]]],
```

1. See [:material-code-braces: PromptTemplateTypeDef](./type_defs.md#prompttemplatetypedef) 
2. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef) 
3. See [:material-code-braces: KbInferenceConfigTypeDef](./type_defs.md#kbinferenceconfigtypedef) 
## GetImportedModelResponseTypeDef

```python
# GetImportedModelResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GetImportedModelResponseTypeDef


def get_value() -> GetImportedModelResponseTypeDef:
    return {
        "modelArn": ...,
    }


# GetImportedModelResponseTypeDef definition

class GetImportedModelResponseTypeDef(TypedDict):
    modelArn: str,
    modelName: str,
    jobName: str,
    jobArn: str,
    modelDataSource: ModelDataSourceTypeDef,  # (1)
    creationTime: datetime,
    modelArchitecture: str,
    modelKmsKeyArn: str,
    instructSupported: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ModelDataSourceTypeDef](./type_defs.md#modeldatasourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetModelImportJobResponseTypeDef

```python
# GetModelImportJobResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GetModelImportJobResponseTypeDef


def get_value() -> GetModelImportJobResponseTypeDef:
    return {
        "jobArn": ...,
    }


# GetModelImportJobResponseTypeDef definition

class GetModelImportJobResponseTypeDef(TypedDict):
    jobArn: str,
    jobName: str,
    importedModelName: str,
    importedModelArn: str,
    roleArn: str,
    modelDataSource: ModelDataSourceTypeDef,  # (1)
    status: ModelImportJobStatusType,  # (2)
    failureMessage: str,
    creationTime: datetime,
    lastModifiedTime: datetime,
    endTime: datetime,
    vpcConfig: VpcConfigOutputTypeDef,  # (3)
    importedModelKmsKeyArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ModelDataSourceTypeDef](./type_defs.md#modeldatasourcetypedef) 
2. See [:material-code-brackets: ModelImportJobStatusType](./literals.md#modelimportjobstatustype) 
3. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetModelInvocationJobResponseTypeDef

```python
# GetModelInvocationJobResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GetModelInvocationJobResponseTypeDef


def get_value() -> GetModelInvocationJobResponseTypeDef:
    return {
        "jobArn": ...,
    }


# GetModelInvocationJobResponseTypeDef definition

class GetModelInvocationJobResponseTypeDef(TypedDict):
    jobArn: str,
    jobName: str,
    modelId: str,
    clientRequestToken: str,
    roleArn: str,
    status: ModelInvocationJobStatusType,  # (1)
    message: str,
    submitTime: datetime,
    lastModifiedTime: datetime,
    endTime: datetime,
    inputDataConfig: ModelInvocationJobInputDataConfigTypeDef,  # (2)
    outputDataConfig: ModelInvocationJobOutputDataConfigTypeDef,  # (3)
    vpcConfig: VpcConfigOutputTypeDef,  # (4)
    timeoutDurationInHours: int,
    jobExpirationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: ModelInvocationJobStatusType](./literals.md#modelinvocationjobstatustype) 
2. See [:material-code-braces: ModelInvocationJobInputDataConfigTypeDef](./type_defs.md#modelinvocationjobinputdataconfigtypedef) 
3. See [:material-code-braces: ModelInvocationJobOutputDataConfigTypeDef](./type_defs.md#modelinvocationjoboutputdataconfigtypedef) 
4. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ModelInvocationJobSummaryTypeDef

```python
# ModelInvocationJobSummaryTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ModelInvocationJobSummaryTypeDef


def get_value() -> ModelInvocationJobSummaryTypeDef:
    return {
        "jobArn": ...,
    }


# ModelInvocationJobSummaryTypeDef definition

class ModelInvocationJobSummaryTypeDef(TypedDict):
    jobArn: str,
    jobName: str,
    modelId: str,
    roleArn: str,
    submitTime: datetime,
    inputDataConfig: ModelInvocationJobInputDataConfigTypeDef,  # (2)
    outputDataConfig: ModelInvocationJobOutputDataConfigTypeDef,  # (3)
    clientRequestToken: NotRequired[str],
    status: NotRequired[ModelInvocationJobStatusType],  # (1)
    message: NotRequired[str],
    lastModifiedTime: NotRequired[datetime],
    endTime: NotRequired[datetime],
    vpcConfig: NotRequired[VpcConfigOutputTypeDef],  # (4)
    timeoutDurationInHours: NotRequired[int],
    jobExpirationTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ModelInvocationJobStatusType](./literals.md#modelinvocationjobstatustype) 
2. See [:material-code-braces: ModelInvocationJobInputDataConfigTypeDef](./type_defs.md#modelinvocationjobinputdataconfigtypedef) 
3. See [:material-code-braces: ModelInvocationJobOutputDataConfigTypeDef](./type_defs.md#modelinvocationjoboutputdataconfigtypedef) 
4. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
## InvocationLogsConfigOutputTypeDef

```python
# InvocationLogsConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import InvocationLogsConfigOutputTypeDef


def get_value() -> InvocationLogsConfigOutputTypeDef:
    return {
        "usePromptResponse": ...,
    }


# InvocationLogsConfigOutputTypeDef definition

class InvocationLogsConfigOutputTypeDef(TypedDict):
    invocationLogSource: InvocationLogSourceTypeDef,  # (1)
    usePromptResponse: NotRequired[bool],
    requestMetadataFilters: NotRequired[RequestMetadataFiltersOutputTypeDef],  # (2)
```

1. See [:material-code-braces: InvocationLogSourceTypeDef](./type_defs.md#invocationlogsourcetypedef) 
2. See [:material-code-braces: RequestMetadataFiltersOutputTypeDef](./type_defs.md#requestmetadatafiltersoutputtypedef) 
## InvocationLogsConfigTypeDef

```python
# InvocationLogsConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import InvocationLogsConfigTypeDef


def get_value() -> InvocationLogsConfigTypeDef:
    return {
        "usePromptResponse": ...,
    }


# InvocationLogsConfigTypeDef definition

class InvocationLogsConfigTypeDef(TypedDict):
    invocationLogSource: InvocationLogSourceTypeDef,  # (1)
    usePromptResponse: NotRequired[bool],
    requestMetadataFilters: NotRequired[RequestMetadataFiltersTypeDef],  # (2)
```

1. See [:material-code-braces: InvocationLogSourceTypeDef](./type_defs.md#invocationlogsourcetypedef) 
2. See [:material-code-braces: RequestMetadataFiltersTypeDef](./type_defs.md#requestmetadatafilterstypedef) 
## EndpointConfigTypeDef

```python
# EndpointConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import EndpointConfigTypeDef


def get_value() -> EndpointConfigTypeDef:
    return {
        "sageMaker": ...,
    }


# EndpointConfigTypeDef definition

class EndpointConfigTypeDef(TypedDict):
    sageMaker: NotRequired[SageMakerEndpointTypeDef],  # (1)
```

1. See [:material-code-braces: SageMakerEndpointTypeDef](./type_defs.md#sagemakerendpointtypedef) 
## CreateModelImportJobRequestTypeDef

```python
# CreateModelImportJobRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import CreateModelImportJobRequestTypeDef


def get_value() -> CreateModelImportJobRequestTypeDef:
    return {
        "jobName": ...,
    }


# CreateModelImportJobRequestTypeDef definition

class CreateModelImportJobRequestTypeDef(TypedDict):
    jobName: str,
    importedModelName: str,
    roleArn: str,
    modelDataSource: ModelDataSourceTypeDef,  # (1)
    jobTags: NotRequired[Sequence[TagTypeDef]],  # (2)
    importedModelTags: NotRequired[Sequence[TagTypeDef]],  # (2)
    clientRequestToken: NotRequired[str],
    vpcConfig: NotRequired[VpcConfigUnionTypeDef],  # (4)
    importedModelKmsKeyId: NotRequired[str],
```

1. See [:material-code-braces: ModelDataSourceTypeDef](./type_defs.md#modeldatasourcetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
## CreateModelInvocationJobRequestTypeDef

```python
# CreateModelInvocationJobRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import CreateModelInvocationJobRequestTypeDef


def get_value() -> CreateModelInvocationJobRequestTypeDef:
    return {
        "jobName": ...,
    }


# CreateModelInvocationJobRequestTypeDef definition

class CreateModelInvocationJobRequestTypeDef(TypedDict):
    jobName: str,
    roleArn: str,
    modelId: str,
    inputDataConfig: ModelInvocationJobInputDataConfigTypeDef,  # (1)
    outputDataConfig: ModelInvocationJobOutputDataConfigTypeDef,  # (2)
    clientRequestToken: NotRequired[str],
    vpcConfig: NotRequired[VpcConfigUnionTypeDef],  # (3)
    timeoutDurationInHours: NotRequired[int],
    tags: NotRequired[Sequence[TagTypeDef]],  # (4)
```

1. See [:material-code-braces: ModelInvocationJobInputDataConfigTypeDef](./type_defs.md#modelinvocationjobinputdataconfigtypedef) 
2. See [:material-code-braces: ModelInvocationJobOutputDataConfigTypeDef](./type_defs.md#modelinvocationjoboutputdataconfigtypedef) 
3. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetModelInvocationLoggingConfigurationResponseTypeDef

```python
# GetModelInvocationLoggingConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GetModelInvocationLoggingConfigurationResponseTypeDef


def get_value() -> GetModelInvocationLoggingConfigurationResponseTypeDef:
    return {
        "loggingConfig": ...,
    }


# GetModelInvocationLoggingConfigurationResponseTypeDef definition

class GetModelInvocationLoggingConfigurationResponseTypeDef(TypedDict):
    loggingConfig: LoggingConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LoggingConfigTypeDef](./type_defs.md#loggingconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutModelInvocationLoggingConfigurationRequestTypeDef

```python
# PutModelInvocationLoggingConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import PutModelInvocationLoggingConfigurationRequestTypeDef


def get_value() -> PutModelInvocationLoggingConfigurationRequestTypeDef:
    return {
        "loggingConfig": ...,
    }


# PutModelInvocationLoggingConfigurationRequestTypeDef definition

class PutModelInvocationLoggingConfigurationRequestTypeDef(TypedDict):
    loggingConfig: LoggingConfigTypeDef,  # (1)
```

1. See [:material-code-braces: LoggingConfigTypeDef](./type_defs.md#loggingconfigtypedef) 
## AutomatedEvaluationConfigOutputTypeDef

```python
# AutomatedEvaluationConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import AutomatedEvaluationConfigOutputTypeDef


def get_value() -> AutomatedEvaluationConfigOutputTypeDef:
    return {
        "datasetMetricConfigs": ...,
    }


# AutomatedEvaluationConfigOutputTypeDef definition

class AutomatedEvaluationConfigOutputTypeDef(TypedDict):
    datasetMetricConfigs: List[EvaluationDatasetMetricConfigOutputTypeDef],  # (1)
    evaluatorModelConfig: NotRequired[EvaluatorModelConfigOutputTypeDef],  # (2)
```

1. See [:material-code-braces: EvaluationDatasetMetricConfigOutputTypeDef](./type_defs.md#evaluationdatasetmetricconfigoutputtypedef) 
2. See [:material-code-braces: EvaluatorModelConfigOutputTypeDef](./type_defs.md#evaluatormodelconfigoutputtypedef) 
## HumanEvaluationConfigOutputTypeDef

```python
# HumanEvaluationConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import HumanEvaluationConfigOutputTypeDef


def get_value() -> HumanEvaluationConfigOutputTypeDef:
    return {
        "humanWorkflowConfig": ...,
    }


# HumanEvaluationConfigOutputTypeDef definition

class HumanEvaluationConfigOutputTypeDef(TypedDict):
    datasetMetricConfigs: List[EvaluationDatasetMetricConfigOutputTypeDef],  # (3)
    humanWorkflowConfig: NotRequired[HumanWorkflowConfigTypeDef],  # (1)
    customMetrics: NotRequired[List[HumanEvaluationCustomMetricTypeDef]],  # (2)
```

1. See [:material-code-braces: HumanWorkflowConfigTypeDef](./type_defs.md#humanworkflowconfigtypedef) 
2. See [:material-code-braces: HumanEvaluationCustomMetricTypeDef](./type_defs.md#humanevaluationcustommetrictypedef) 
3. See [:material-code-braces: EvaluationDatasetMetricConfigOutputTypeDef](./type_defs.md#evaluationdatasetmetricconfigoutputtypedef) 
## AutomatedEvaluationConfigTypeDef

```python
# AutomatedEvaluationConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import AutomatedEvaluationConfigTypeDef


def get_value() -> AutomatedEvaluationConfigTypeDef:
    return {
        "datasetMetricConfigs": ...,
    }


# AutomatedEvaluationConfigTypeDef definition

class AutomatedEvaluationConfigTypeDef(TypedDict):
    datasetMetricConfigs: Sequence[EvaluationDatasetMetricConfigTypeDef],  # (1)
    evaluatorModelConfig: NotRequired[EvaluatorModelConfigTypeDef],  # (2)
```

1. See [:material-code-braces: EvaluationDatasetMetricConfigTypeDef](./type_defs.md#evaluationdatasetmetricconfigtypedef) 
2. See [:material-code-braces: EvaluatorModelConfigTypeDef](./type_defs.md#evaluatormodelconfigtypedef) 
## HumanEvaluationConfigTypeDef

```python
# HumanEvaluationConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import HumanEvaluationConfigTypeDef


def get_value() -> HumanEvaluationConfigTypeDef:
    return {
        "humanWorkflowConfig": ...,
    }


# HumanEvaluationConfigTypeDef definition

class HumanEvaluationConfigTypeDef(TypedDict):
    datasetMetricConfigs: Sequence[EvaluationDatasetMetricConfigTypeDef],  # (3)
    humanWorkflowConfig: NotRequired[HumanWorkflowConfigTypeDef],  # (1)
    customMetrics: NotRequired[Sequence[HumanEvaluationCustomMetricTypeDef]],  # (2)
```

1. See [:material-code-braces: HumanWorkflowConfigTypeDef](./type_defs.md#humanworkflowconfigtypedef) 
2. See [:material-code-braces: HumanEvaluationCustomMetricTypeDef](./type_defs.md#humanevaluationcustommetrictypedef) 
3. See [:material-code-braces: EvaluationDatasetMetricConfigTypeDef](./type_defs.md#evaluationdatasetmetricconfigtypedef) 
## KnowledgeBaseRetrievalConfigurationOutputTypeDef

```python
# KnowledgeBaseRetrievalConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import KnowledgeBaseRetrievalConfigurationOutputTypeDef


def get_value() -> KnowledgeBaseRetrievalConfigurationOutputTypeDef:
    return {
        "vectorSearchConfiguration": ...,
    }


# KnowledgeBaseRetrievalConfigurationOutputTypeDef definition

class KnowledgeBaseRetrievalConfigurationOutputTypeDef(TypedDict):
    vectorSearchConfiguration: KnowledgeBaseVectorSearchConfigurationOutputTypeDef,  # (1)
```

1. See [:material-code-braces: KnowledgeBaseVectorSearchConfigurationOutputTypeDef](./type_defs.md#knowledgebasevectorsearchconfigurationoutputtypedef) 
## KnowledgeBaseRetrievalConfigurationTypeDef

```python
# KnowledgeBaseRetrievalConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import KnowledgeBaseRetrievalConfigurationTypeDef


def get_value() -> KnowledgeBaseRetrievalConfigurationTypeDef:
    return {
        "vectorSearchConfiguration": ...,
    }


# KnowledgeBaseRetrievalConfigurationTypeDef definition

class KnowledgeBaseRetrievalConfigurationTypeDef(TypedDict):
    vectorSearchConfiguration: KnowledgeBaseVectorSearchConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: KnowledgeBaseVectorSearchConfigurationTypeDef](./type_defs.md#knowledgebasevectorsearchconfigurationtypedef) 
## MarketplaceModelEndpointTypeDef

```python
# MarketplaceModelEndpointTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import MarketplaceModelEndpointTypeDef


def get_value() -> MarketplaceModelEndpointTypeDef:
    return {
        "endpointArn": ...,
    }


# MarketplaceModelEndpointTypeDef definition

class MarketplaceModelEndpointTypeDef(TypedDict):
    endpointArn: str,
    modelSourceIdentifier: str,
    createdAt: datetime,
    updatedAt: datetime,
    endpointConfig: EndpointConfigOutputTypeDef,  # (2)
    endpointStatus: str,
    status: NotRequired[StatusType],  # (1)
    statusMessage: NotRequired[str],
    endpointStatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-braces: EndpointConfigOutputTypeDef](./type_defs.md#endpointconfigoutputtypedef) 
## ExternalSourcesRetrieveAndGenerateConfigurationOutputTypeDef

```python
# ExternalSourcesRetrieveAndGenerateConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ExternalSourcesRetrieveAndGenerateConfigurationOutputTypeDef


def get_value() -> ExternalSourcesRetrieveAndGenerateConfigurationOutputTypeDef:
    return {
        "modelArn": ...,
    }


# ExternalSourcesRetrieveAndGenerateConfigurationOutputTypeDef definition

class ExternalSourcesRetrieveAndGenerateConfigurationOutputTypeDef(TypedDict):
    modelArn: str,
    sources: List[ExternalSourceOutputTypeDef],  # (1)
    generationConfiguration: NotRequired[ExternalSourcesGenerationConfigurationOutputTypeDef],  # (2)
```

1. See [:material-code-braces: ExternalSourceOutputTypeDef](./type_defs.md#externalsourceoutputtypedef) 
2. See [:material-code-braces: ExternalSourcesGenerationConfigurationOutputTypeDef](./type_defs.md#externalsourcesgenerationconfigurationoutputtypedef) 
## ExternalSourcesRetrieveAndGenerateConfigurationTypeDef

```python
# ExternalSourcesRetrieveAndGenerateConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ExternalSourcesRetrieveAndGenerateConfigurationTypeDef


def get_value() -> ExternalSourcesRetrieveAndGenerateConfigurationTypeDef:
    return {
        "modelArn": ...,
    }


# ExternalSourcesRetrieveAndGenerateConfigurationTypeDef definition

class ExternalSourcesRetrieveAndGenerateConfigurationTypeDef(TypedDict):
    modelArn: str,
    sources: Sequence[ExternalSourceTypeDef],  # (1)
    generationConfiguration: NotRequired[ExternalSourcesGenerationConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: ExternalSourceTypeDef](./type_defs.md#externalsourcetypedef) 
2. See [:material-code-braces: ExternalSourcesGenerationConfigurationTypeDef](./type_defs.md#externalsourcesgenerationconfigurationtypedef) 
## ListModelInvocationJobsResponseTypeDef

```python
# ListModelInvocationJobsResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import ListModelInvocationJobsResponseTypeDef


def get_value() -> ListModelInvocationJobsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListModelInvocationJobsResponseTypeDef definition

class ListModelInvocationJobsResponseTypeDef(TypedDict):
    invocationJobSummaries: List[ModelInvocationJobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ModelInvocationJobSummaryTypeDef](./type_defs.md#modelinvocationjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TrainingDataConfigOutputTypeDef

```python
# TrainingDataConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import TrainingDataConfigOutputTypeDef


def get_value() -> TrainingDataConfigOutputTypeDef:
    return {
        "s3Uri": ...,
    }


# TrainingDataConfigOutputTypeDef definition

class TrainingDataConfigOutputTypeDef(TypedDict):
    s3Uri: NotRequired[str],
    invocationLogsConfig: NotRequired[InvocationLogsConfigOutputTypeDef],  # (1)
```

1. See [:material-code-braces: InvocationLogsConfigOutputTypeDef](./type_defs.md#invocationlogsconfigoutputtypedef) 
## TrainingDataConfigTypeDef

```python
# TrainingDataConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import TrainingDataConfigTypeDef


def get_value() -> TrainingDataConfigTypeDef:
    return {
        "s3Uri": ...,
    }


# TrainingDataConfigTypeDef definition

class TrainingDataConfigTypeDef(TypedDict):
    s3Uri: NotRequired[str],
    invocationLogsConfig: NotRequired[InvocationLogsConfigTypeDef],  # (1)
```

1. See [:material-code-braces: InvocationLogsConfigTypeDef](./type_defs.md#invocationlogsconfigtypedef) 
## EvaluationConfigOutputTypeDef

```python
# EvaluationConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import EvaluationConfigOutputTypeDef


def get_value() -> EvaluationConfigOutputTypeDef:
    return {
        "automated": ...,
    }


# EvaluationConfigOutputTypeDef definition

class EvaluationConfigOutputTypeDef(TypedDict):
    automated: NotRequired[AutomatedEvaluationConfigOutputTypeDef],  # (1)
    human: NotRequired[HumanEvaluationConfigOutputTypeDef],  # (2)
```

1. See [:material-code-braces: AutomatedEvaluationConfigOutputTypeDef](./type_defs.md#automatedevaluationconfigoutputtypedef) 
2. See [:material-code-braces: HumanEvaluationConfigOutputTypeDef](./type_defs.md#humanevaluationconfigoutputtypedef) 
## EvaluationConfigTypeDef

```python
# EvaluationConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import EvaluationConfigTypeDef


def get_value() -> EvaluationConfigTypeDef:
    return {
        "automated": ...,
    }


# EvaluationConfigTypeDef definition

class EvaluationConfigTypeDef(TypedDict):
    automated: NotRequired[AutomatedEvaluationConfigTypeDef],  # (1)
    human: NotRequired[HumanEvaluationConfigTypeDef],  # (2)
```

1. See [:material-code-braces: AutomatedEvaluationConfigTypeDef](./type_defs.md#automatedevaluationconfigtypedef) 
2. See [:material-code-braces: HumanEvaluationConfigTypeDef](./type_defs.md#humanevaluationconfigtypedef) 
## KnowledgeBaseRetrieveAndGenerateConfigurationOutputTypeDef

```python
# KnowledgeBaseRetrieveAndGenerateConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import KnowledgeBaseRetrieveAndGenerateConfigurationOutputTypeDef


def get_value() -> KnowledgeBaseRetrieveAndGenerateConfigurationOutputTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# KnowledgeBaseRetrieveAndGenerateConfigurationOutputTypeDef definition

class KnowledgeBaseRetrieveAndGenerateConfigurationOutputTypeDef(TypedDict):
    knowledgeBaseId: str,
    modelArn: str,
    retrievalConfiguration: NotRequired[KnowledgeBaseRetrievalConfigurationOutputTypeDef],  # (1)
    generationConfiguration: NotRequired[GenerationConfigurationOutputTypeDef],  # (2)
    orchestrationConfiguration: NotRequired[OrchestrationConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: KnowledgeBaseRetrievalConfigurationOutputTypeDef](./type_defs.md#knowledgebaseretrievalconfigurationoutputtypedef) 
2. See [:material-code-braces: GenerationConfigurationOutputTypeDef](./type_defs.md#generationconfigurationoutputtypedef) 
3. See [:material-code-braces: OrchestrationConfigurationTypeDef](./type_defs.md#orchestrationconfigurationtypedef) 
## RetrieveConfigOutputTypeDef

```python
# RetrieveConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import RetrieveConfigOutputTypeDef


def get_value() -> RetrieveConfigOutputTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# RetrieveConfigOutputTypeDef definition

class RetrieveConfigOutputTypeDef(TypedDict):
    knowledgeBaseId: str,
    knowledgeBaseRetrievalConfiguration: KnowledgeBaseRetrievalConfigurationOutputTypeDef,  # (1)
```

1. See [:material-code-braces: KnowledgeBaseRetrievalConfigurationOutputTypeDef](./type_defs.md#knowledgebaseretrievalconfigurationoutputtypedef) 
## KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef

```python
# KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef


def get_value() -> KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef definition

class KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef(TypedDict):
    knowledgeBaseId: str,
    modelArn: str,
    retrievalConfiguration: NotRequired[KnowledgeBaseRetrievalConfigurationTypeDef],  # (1)
    generationConfiguration: NotRequired[GenerationConfigurationTypeDef],  # (2)
    orchestrationConfiguration: NotRequired[OrchestrationConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: KnowledgeBaseRetrievalConfigurationTypeDef](./type_defs.md#knowledgebaseretrievalconfigurationtypedef) 
2. See [:material-code-braces: GenerationConfigurationTypeDef](./type_defs.md#generationconfigurationtypedef) 
3. See [:material-code-braces: OrchestrationConfigurationTypeDef](./type_defs.md#orchestrationconfigurationtypedef) 
## RetrieveConfigTypeDef

```python
# RetrieveConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import RetrieveConfigTypeDef


def get_value() -> RetrieveConfigTypeDef:
    return {
        "knowledgeBaseId": ...,
    }


# RetrieveConfigTypeDef definition

class RetrieveConfigTypeDef(TypedDict):
    knowledgeBaseId: str,
    knowledgeBaseRetrievalConfiguration: KnowledgeBaseRetrievalConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: KnowledgeBaseRetrievalConfigurationTypeDef](./type_defs.md#knowledgebaseretrievalconfigurationtypedef) 
## CreateMarketplaceModelEndpointResponseTypeDef

```python
# CreateMarketplaceModelEndpointResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import CreateMarketplaceModelEndpointResponseTypeDef


def get_value() -> CreateMarketplaceModelEndpointResponseTypeDef:
    return {
        "marketplaceModelEndpoint": ...,
    }


# CreateMarketplaceModelEndpointResponseTypeDef definition

class CreateMarketplaceModelEndpointResponseTypeDef(TypedDict):
    marketplaceModelEndpoint: MarketplaceModelEndpointTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MarketplaceModelEndpointTypeDef](./type_defs.md#marketplacemodelendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMarketplaceModelEndpointResponseTypeDef

```python
# GetMarketplaceModelEndpointResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GetMarketplaceModelEndpointResponseTypeDef


def get_value() -> GetMarketplaceModelEndpointResponseTypeDef:
    return {
        "marketplaceModelEndpoint": ...,
    }


# GetMarketplaceModelEndpointResponseTypeDef definition

class GetMarketplaceModelEndpointResponseTypeDef(TypedDict):
    marketplaceModelEndpoint: MarketplaceModelEndpointTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MarketplaceModelEndpointTypeDef](./type_defs.md#marketplacemodelendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterMarketplaceModelEndpointResponseTypeDef

```python
# RegisterMarketplaceModelEndpointResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import RegisterMarketplaceModelEndpointResponseTypeDef


def get_value() -> RegisterMarketplaceModelEndpointResponseTypeDef:
    return {
        "marketplaceModelEndpoint": ...,
    }


# RegisterMarketplaceModelEndpointResponseTypeDef definition

class RegisterMarketplaceModelEndpointResponseTypeDef(TypedDict):
    marketplaceModelEndpoint: MarketplaceModelEndpointTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MarketplaceModelEndpointTypeDef](./type_defs.md#marketplacemodelendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMarketplaceModelEndpointResponseTypeDef

```python
# UpdateMarketplaceModelEndpointResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import UpdateMarketplaceModelEndpointResponseTypeDef


def get_value() -> UpdateMarketplaceModelEndpointResponseTypeDef:
    return {
        "marketplaceModelEndpoint": ...,
    }


# UpdateMarketplaceModelEndpointResponseTypeDef definition

class UpdateMarketplaceModelEndpointResponseTypeDef(TypedDict):
    marketplaceModelEndpoint: MarketplaceModelEndpointTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MarketplaceModelEndpointTypeDef](./type_defs.md#marketplacemodelendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCustomModelResponseTypeDef

```python
# GetCustomModelResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GetCustomModelResponseTypeDef


def get_value() -> GetCustomModelResponseTypeDef:
    return {
        "modelArn": ...,
    }


# GetCustomModelResponseTypeDef definition

class GetCustomModelResponseTypeDef(TypedDict):
    modelArn: str,
    modelName: str,
    jobName: str,
    jobArn: str,
    baseModelArn: str,
    customizationType: CustomizationTypeType,  # (1)
    modelKmsKeyArn: str,
    hyperParameters: Dict[str, str],
    trainingDataConfig: TrainingDataConfigOutputTypeDef,  # (2)
    validationDataConfig: ValidationDataConfigOutputTypeDef,  # (3)
    outputDataConfig: OutputDataConfigTypeDef,  # (4)
    trainingMetrics: TrainingMetricsTypeDef,  # (5)
    validationMetrics: List[ValidatorMetricTypeDef],  # (6)
    creationTime: datetime,
    customizationConfig: CustomizationConfigTypeDef,  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-brackets: CustomizationTypeType](./literals.md#customizationtypetype) 
2. See [:material-code-braces: TrainingDataConfigOutputTypeDef](./type_defs.md#trainingdataconfigoutputtypedef) 
3. See [:material-code-braces: ValidationDataConfigOutputTypeDef](./type_defs.md#validationdataconfigoutputtypedef) 
4. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
5. See [:material-code-braces: TrainingMetricsTypeDef](./type_defs.md#trainingmetricstypedef) 
6. See [:material-code-braces: ValidatorMetricTypeDef](./type_defs.md#validatormetrictypedef) 
7. See [:material-code-braces: CustomizationConfigTypeDef](./type_defs.md#customizationconfigtypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetModelCustomizationJobResponseTypeDef

```python
# GetModelCustomizationJobResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GetModelCustomizationJobResponseTypeDef


def get_value() -> GetModelCustomizationJobResponseTypeDef:
    return {
        "jobArn": ...,
    }


# GetModelCustomizationJobResponseTypeDef definition

class GetModelCustomizationJobResponseTypeDef(TypedDict):
    jobArn: str,
    jobName: str,
    outputModelName: str,
    outputModelArn: str,
    clientRequestToken: str,
    roleArn: str,
    status: ModelCustomizationJobStatusType,  # (1)
    failureMessage: str,
    creationTime: datetime,
    lastModifiedTime: datetime,
    endTime: datetime,
    baseModelArn: str,
    hyperParameters: Dict[str, str],
    trainingDataConfig: TrainingDataConfigOutputTypeDef,  # (2)
    validationDataConfig: ValidationDataConfigOutputTypeDef,  # (3)
    outputDataConfig: OutputDataConfigTypeDef,  # (4)
    customizationType: CustomizationTypeType,  # (5)
    outputModelKmsKeyArn: str,
    trainingMetrics: TrainingMetricsTypeDef,  # (6)
    validationMetrics: List[ValidatorMetricTypeDef],  # (7)
    vpcConfig: VpcConfigOutputTypeDef,  # (8)
    customizationConfig: CustomizationConfigTypeDef,  # (9)
    ResponseMetadata: ResponseMetadataTypeDef,  # (10)
```

1. See [:material-code-brackets: ModelCustomizationJobStatusType](./literals.md#modelcustomizationjobstatustype) 
2. See [:material-code-braces: TrainingDataConfigOutputTypeDef](./type_defs.md#trainingdataconfigoutputtypedef) 
3. See [:material-code-braces: ValidationDataConfigOutputTypeDef](./type_defs.md#validationdataconfigoutputtypedef) 
4. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
5. See [:material-code-brackets: CustomizationTypeType](./literals.md#customizationtypetype) 
6. See [:material-code-braces: TrainingMetricsTypeDef](./type_defs.md#trainingmetricstypedef) 
7. See [:material-code-braces: ValidatorMetricTypeDef](./type_defs.md#validatormetrictypedef) 
8. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
9. See [:material-code-braces: CustomizationConfigTypeDef](./type_defs.md#customizationconfigtypedef) 
10. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMarketplaceModelEndpointRequestTypeDef

```python
# CreateMarketplaceModelEndpointRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import CreateMarketplaceModelEndpointRequestTypeDef


def get_value() -> CreateMarketplaceModelEndpointRequestTypeDef:
    return {
        "modelSourceIdentifier": ...,
    }


# CreateMarketplaceModelEndpointRequestTypeDef definition

class CreateMarketplaceModelEndpointRequestTypeDef(TypedDict):
    modelSourceIdentifier: str,
    endpointConfig: EndpointConfigUnionTypeDef,  # (1)
    endpointName: str,
    acceptEula: NotRequired[bool],
    clientRequestToken: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: EndpointConfigTypeDef](./type_defs.md#endpointconfigtypedef) [:material-code-braces: EndpointConfigOutputTypeDef](./type_defs.md#endpointconfigoutputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateMarketplaceModelEndpointRequestTypeDef

```python
# UpdateMarketplaceModelEndpointRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import UpdateMarketplaceModelEndpointRequestTypeDef


def get_value() -> UpdateMarketplaceModelEndpointRequestTypeDef:
    return {
        "endpointArn": ...,
    }


# UpdateMarketplaceModelEndpointRequestTypeDef definition

class UpdateMarketplaceModelEndpointRequestTypeDef(TypedDict):
    endpointArn: str,
    endpointConfig: EndpointConfigUnionTypeDef,  # (1)
    clientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: EndpointConfigTypeDef](./type_defs.md#endpointconfigtypedef) [:material-code-braces: EndpointConfigOutputTypeDef](./type_defs.md#endpointconfigoutputtypedef) 
## RetrieveAndGenerateConfigurationOutputTypeDef

```python
# RetrieveAndGenerateConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import RetrieveAndGenerateConfigurationOutputTypeDef


def get_value() -> RetrieveAndGenerateConfigurationOutputTypeDef:
    return {
        "type": ...,
    }


# RetrieveAndGenerateConfigurationOutputTypeDef definition

class RetrieveAndGenerateConfigurationOutputTypeDef(TypedDict):
    type: RetrieveAndGenerateTypeType,  # (1)
    knowledgeBaseConfiguration: NotRequired[KnowledgeBaseRetrieveAndGenerateConfigurationOutputTypeDef],  # (2)
    externalSourcesConfiguration: NotRequired[ExternalSourcesRetrieveAndGenerateConfigurationOutputTypeDef],  # (3)
```

1. See [:material-code-brackets: RetrieveAndGenerateTypeType](./literals.md#retrieveandgeneratetypetype) 
2. See [:material-code-braces: KnowledgeBaseRetrieveAndGenerateConfigurationOutputTypeDef](./type_defs.md#knowledgebaseretrieveandgenerateconfigurationoutputtypedef) 
3. See [:material-code-braces: ExternalSourcesRetrieveAndGenerateConfigurationOutputTypeDef](./type_defs.md#externalsourcesretrieveandgenerateconfigurationoutputtypedef) 
## RetrieveAndGenerateConfigurationTypeDef

```python
# RetrieveAndGenerateConfigurationTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import RetrieveAndGenerateConfigurationTypeDef


def get_value() -> RetrieveAndGenerateConfigurationTypeDef:
    return {
        "type": ...,
    }


# RetrieveAndGenerateConfigurationTypeDef definition

class RetrieveAndGenerateConfigurationTypeDef(TypedDict):
    type: RetrieveAndGenerateTypeType,  # (1)
    knowledgeBaseConfiguration: NotRequired[KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef],  # (2)
    externalSourcesConfiguration: NotRequired[ExternalSourcesRetrieveAndGenerateConfigurationTypeDef],  # (3)
```

1. See [:material-code-brackets: RetrieveAndGenerateTypeType](./literals.md#retrieveandgeneratetypetype) 
2. See [:material-code-braces: KnowledgeBaseRetrieveAndGenerateConfigurationTypeDef](./type_defs.md#knowledgebaseretrieveandgenerateconfigurationtypedef) 
3. See [:material-code-braces: ExternalSourcesRetrieveAndGenerateConfigurationTypeDef](./type_defs.md#externalsourcesretrieveandgenerateconfigurationtypedef) 
## CreateModelCustomizationJobRequestTypeDef

```python
# CreateModelCustomizationJobRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import CreateModelCustomizationJobRequestTypeDef


def get_value() -> CreateModelCustomizationJobRequestTypeDef:
    return {
        "jobName": ...,
    }


# CreateModelCustomizationJobRequestTypeDef definition

class CreateModelCustomizationJobRequestTypeDef(TypedDict):
    jobName: str,
    customModelName: str,
    roleArn: str,
    baseModelIdentifier: str,
    trainingDataConfig: TrainingDataConfigUnionTypeDef,  # (1)
    outputDataConfig: OutputDataConfigTypeDef,  # (2)
    clientRequestToken: NotRequired[str],
    customizationType: NotRequired[CustomizationTypeType],  # (3)
    customModelKmsKeyId: NotRequired[str],
    jobTags: NotRequired[Sequence[TagTypeDef]],  # (4)
    customModelTags: NotRequired[Sequence[TagTypeDef]],  # (4)
    validationDataConfig: NotRequired[ValidationDataConfigUnionTypeDef],  # (6)
    hyperParameters: NotRequired[Mapping[str, str]],
    vpcConfig: NotRequired[VpcConfigUnionTypeDef],  # (7)
    customizationConfig: NotRequired[CustomizationConfigTypeDef],  # (8)
```

1. See [:material-code-braces: TrainingDataConfigTypeDef](./type_defs.md#trainingdataconfigtypedef) [:material-code-braces: TrainingDataConfigOutputTypeDef](./type_defs.md#trainingdataconfigoutputtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-brackets: CustomizationTypeType](./literals.md#customizationtypetype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: ValidationDataConfigTypeDef](./type_defs.md#validationdataconfigtypedef) [:material-code-braces: ValidationDataConfigOutputTypeDef](./type_defs.md#validationdataconfigoutputtypedef) 
7. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
8. See [:material-code-braces: CustomizationConfigTypeDef](./type_defs.md#customizationconfigtypedef) 
## KnowledgeBaseConfigOutputTypeDef

```python
# KnowledgeBaseConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import KnowledgeBaseConfigOutputTypeDef


def get_value() -> KnowledgeBaseConfigOutputTypeDef:
    return {
        "retrieveConfig": ...,
    }


# KnowledgeBaseConfigOutputTypeDef definition

class KnowledgeBaseConfigOutputTypeDef(TypedDict):
    retrieveConfig: NotRequired[RetrieveConfigOutputTypeDef],  # (1)
    retrieveAndGenerateConfig: NotRequired[RetrieveAndGenerateConfigurationOutputTypeDef],  # (2)
```

1. See [:material-code-braces: RetrieveConfigOutputTypeDef](./type_defs.md#retrieveconfigoutputtypedef) 
2. See [:material-code-braces: RetrieveAndGenerateConfigurationOutputTypeDef](./type_defs.md#retrieveandgenerateconfigurationoutputtypedef) 
## KnowledgeBaseConfigTypeDef

```python
# KnowledgeBaseConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import KnowledgeBaseConfigTypeDef


def get_value() -> KnowledgeBaseConfigTypeDef:
    return {
        "retrieveConfig": ...,
    }


# KnowledgeBaseConfigTypeDef definition

class KnowledgeBaseConfigTypeDef(TypedDict):
    retrieveConfig: NotRequired[RetrieveConfigTypeDef],  # (1)
    retrieveAndGenerateConfig: NotRequired[RetrieveAndGenerateConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: RetrieveConfigTypeDef](./type_defs.md#retrieveconfigtypedef) 
2. See [:material-code-braces: RetrieveAndGenerateConfigurationTypeDef](./type_defs.md#retrieveandgenerateconfigurationtypedef) 
## RAGConfigOutputTypeDef

```python
# RAGConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import RAGConfigOutputTypeDef


def get_value() -> RAGConfigOutputTypeDef:
    return {
        "knowledgeBaseConfig": ...,
    }


# RAGConfigOutputTypeDef definition

class RAGConfigOutputTypeDef(TypedDict):
    knowledgeBaseConfig: NotRequired[KnowledgeBaseConfigOutputTypeDef],  # (1)
```

1. See [:material-code-braces: KnowledgeBaseConfigOutputTypeDef](./type_defs.md#knowledgebaseconfigoutputtypedef) 
## RAGConfigTypeDef

```python
# RAGConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import RAGConfigTypeDef


def get_value() -> RAGConfigTypeDef:
    return {
        "knowledgeBaseConfig": ...,
    }


# RAGConfigTypeDef definition

class RAGConfigTypeDef(TypedDict):
    knowledgeBaseConfig: NotRequired[KnowledgeBaseConfigTypeDef],  # (1)
```

1. See [:material-code-braces: KnowledgeBaseConfigTypeDef](./type_defs.md#knowledgebaseconfigtypedef) 
## EvaluationInferenceConfigOutputTypeDef

```python
# EvaluationInferenceConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import EvaluationInferenceConfigOutputTypeDef


def get_value() -> EvaluationInferenceConfigOutputTypeDef:
    return {
        "models": ...,
    }


# EvaluationInferenceConfigOutputTypeDef definition

class EvaluationInferenceConfigOutputTypeDef(TypedDict):
    models: NotRequired[List[EvaluationModelConfigTypeDef]],  # (1)
    ragConfigs: NotRequired[List[RAGConfigOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: EvaluationModelConfigTypeDef](./type_defs.md#evaluationmodelconfigtypedef) 
2. See [:material-code-braces: RAGConfigOutputTypeDef](./type_defs.md#ragconfigoutputtypedef) 
## EvaluationInferenceConfigTypeDef

```python
# EvaluationInferenceConfigTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import EvaluationInferenceConfigTypeDef


def get_value() -> EvaluationInferenceConfigTypeDef:
    return {
        "models": ...,
    }


# EvaluationInferenceConfigTypeDef definition

class EvaluationInferenceConfigTypeDef(TypedDict):
    models: NotRequired[Sequence[EvaluationModelConfigTypeDef]],  # (1)
    ragConfigs: NotRequired[Sequence[RAGConfigTypeDef]],  # (2)
```

1. See [:material-code-braces: EvaluationModelConfigTypeDef](./type_defs.md#evaluationmodelconfigtypedef) 
2. See [:material-code-braces: RAGConfigTypeDef](./type_defs.md#ragconfigtypedef) 
## GetEvaluationJobResponseTypeDef

```python
# GetEvaluationJobResponseTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import GetEvaluationJobResponseTypeDef


def get_value() -> GetEvaluationJobResponseTypeDef:
    return {
        "jobName": ...,
    }


# GetEvaluationJobResponseTypeDef definition

class GetEvaluationJobResponseTypeDef(TypedDict):
    jobName: str,
    status: EvaluationJobStatusType,  # (1)
    jobArn: str,
    jobDescription: str,
    roleArn: str,
    customerEncryptionKeyId: str,
    jobType: EvaluationJobTypeType,  # (2)
    applicationType: ApplicationTypeType,  # (3)
    evaluationConfig: EvaluationConfigOutputTypeDef,  # (4)
    inferenceConfig: EvaluationInferenceConfigOutputTypeDef,  # (5)
    outputDataConfig: EvaluationOutputDataConfigTypeDef,  # (6)
    creationTime: datetime,
    lastModifiedTime: datetime,
    failureMessages: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-brackets: EvaluationJobStatusType](./literals.md#evaluationjobstatustype) 
2. See [:material-code-brackets: EvaluationJobTypeType](./literals.md#evaluationjobtypetype) 
3. See [:material-code-brackets: ApplicationTypeType](./literals.md#applicationtypetype) 
4. See [:material-code-braces: EvaluationConfigOutputTypeDef](./type_defs.md#evaluationconfigoutputtypedef) 
5. See [:material-code-braces: EvaluationInferenceConfigOutputTypeDef](./type_defs.md#evaluationinferenceconfigoutputtypedef) 
6. See [:material-code-braces: EvaluationOutputDataConfigTypeDef](./type_defs.md#evaluationoutputdataconfigtypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEvaluationJobRequestTypeDef

```python
# CreateEvaluationJobRequestTypeDef TypedDict usage example

from types_aiobotocore_bedrock.type_defs import CreateEvaluationJobRequestTypeDef


def get_value() -> CreateEvaluationJobRequestTypeDef:
    return {
        "jobName": ...,
    }


# CreateEvaluationJobRequestTypeDef definition

class CreateEvaluationJobRequestTypeDef(TypedDict):
    jobName: str,
    roleArn: str,
    evaluationConfig: EvaluationConfigUnionTypeDef,  # (1)
    inferenceConfig: EvaluationInferenceConfigUnionTypeDef,  # (2)
    outputDataConfig: EvaluationOutputDataConfigTypeDef,  # (3)
    jobDescription: NotRequired[str],
    clientRequestToken: NotRequired[str],
    customerEncryptionKeyId: NotRequired[str],
    jobTags: NotRequired[Sequence[TagTypeDef]],  # (4)
    applicationType: NotRequired[ApplicationTypeType],  # (5)
```

1. See [:material-code-braces: EvaluationConfigTypeDef](./type_defs.md#evaluationconfigtypedef) [:material-code-braces: EvaluationConfigOutputTypeDef](./type_defs.md#evaluationconfigoutputtypedef) 
2. See [:material-code-braces: EvaluationInferenceConfigTypeDef](./type_defs.md#evaluationinferenceconfigtypedef) [:material-code-braces: EvaluationInferenceConfigOutputTypeDef](./type_defs.md#evaluationinferenceconfigoutputtypedef) 
3. See [:material-code-braces: EvaluationOutputDataConfigTypeDef](./type_defs.md#evaluationoutputdataconfigtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-brackets: ApplicationTypeType](./literals.md#applicationtypetype) 
