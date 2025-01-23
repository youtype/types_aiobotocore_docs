# Type definitions

> [Index](../README.md) > [SagemakerEdgeManager](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SagemakerEdgeManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#sagemakeredgemanager)
    type annotations stubs module [types-aiobotocore-sagemaker-edge](https://pypi.org/project/types-aiobotocore-sagemaker-edge/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## ChecksumTypeDef

```python
# ChecksumTypeDef definition

class ChecksumTypeDef(TypedDict):
    Type: NotRequired[ChecksumTypeType],  # (1)
    Sum: NotRequired[str],
```

1. See [:material-code-brackets: ChecksumTypeType](./literals.md#checksumtypetype) 
## DeploymentModelTypeDef

```python
# DeploymentModelTypeDef definition

class DeploymentModelTypeDef(TypedDict):
    ModelHandle: NotRequired[str],
    ModelName: NotRequired[str],
    ModelVersion: NotRequired[str],
    DesiredState: NotRequired[ModelStateType],  # (1)
    State: NotRequired[ModelStateType],  # (1)
    Status: NotRequired[DeploymentStatusType],  # (3)
    StatusReason: NotRequired[str],
    RollbackFailureReason: NotRequired[str],
```

1. See [:material-code-brackets: ModelStateType](./literals.md#modelstatetype) 
2. See [:material-code-brackets: ModelStateType](./literals.md#modelstatetype) 
3. See [:material-code-brackets: DeploymentStatusType](./literals.md#deploymentstatustype) 
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

## GetDeploymentsRequestRequestTypeDef

```python
# GetDeploymentsRequestRequestTypeDef definition

class GetDeploymentsRequestRequestTypeDef(TypedDict):
    DeviceName: str,
    DeviceFleetName: str,
```

## GetDeviceRegistrationRequestRequestTypeDef

```python
# GetDeviceRegistrationRequestRequestTypeDef definition

class GetDeviceRegistrationRequestRequestTypeDef(TypedDict):
    DeviceName: str,
    DeviceFleetName: str,
```

## DefinitionTypeDef

```python
# DefinitionTypeDef definition

class DefinitionTypeDef(TypedDict):
    ModelHandle: NotRequired[str],
    S3Url: NotRequired[str],
    Checksum: NotRequired[ChecksumTypeDef],  # (1)
    State: NotRequired[ModelStateType],  # (2)
```

1. See [:material-code-braces: ChecksumTypeDef](./type_defs.md#checksumtypedef) 
2. See [:material-code-brackets: ModelStateType](./literals.md#modelstatetype) 
## DeploymentResultTypeDef

```python
# DeploymentResultTypeDef definition

class DeploymentResultTypeDef(TypedDict):
    DeploymentName: NotRequired[str],
    DeploymentStatus: NotRequired[str],
    DeploymentStatusMessage: NotRequired[str],
    DeploymentStartTime: NotRequired[TimestampTypeDef],
    DeploymentEndTime: NotRequired[TimestampTypeDef],
    DeploymentModels: NotRequired[Sequence[DeploymentModelTypeDef]],  # (1)
```

1. See [:material-code-braces: DeploymentModelTypeDef](./type_defs.md#deploymentmodeltypedef) 
## EdgeMetricTypeDef

```python
# EdgeMetricTypeDef definition

class EdgeMetricTypeDef(TypedDict):
    Dimension: NotRequired[str],
    MetricName: NotRequired[str],
    Value: NotRequired[float],
    Timestamp: NotRequired[TimestampTypeDef],
```

## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDeviceRegistrationResultTypeDef

```python
# GetDeviceRegistrationResultTypeDef definition

class GetDeviceRegistrationResultTypeDef(TypedDict):
    DeviceRegistration: str,
    CacheTTL: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EdgeDeploymentTypeDef

```python
# EdgeDeploymentTypeDef definition

class EdgeDeploymentTypeDef(TypedDict):
    DeploymentName: NotRequired[str],
    Type: NotRequired[DeploymentTypeType],  # (1)
    FailureHandlingPolicy: NotRequired[FailureHandlingPolicyType],  # (2)
    Definitions: NotRequired[List[DefinitionTypeDef]],  # (3)
```

1. See [:material-code-brackets: DeploymentTypeType](./literals.md#deploymenttypetype) 
2. See [:material-code-brackets: FailureHandlingPolicyType](./literals.md#failurehandlingpolicytype) 
3. See [:material-code-braces: DefinitionTypeDef](./type_defs.md#definitiontypedef) 
## ModelTypeDef

```python
# ModelTypeDef definition

class ModelTypeDef(TypedDict):
    ModelName: NotRequired[str],
    ModelVersion: NotRequired[str],
    LatestSampleTime: NotRequired[TimestampTypeDef],
    LatestInference: NotRequired[TimestampTypeDef],
    ModelMetrics: NotRequired[Sequence[EdgeMetricTypeDef]],  # (1)
```

1. See [:material-code-braces: EdgeMetricTypeDef](./type_defs.md#edgemetrictypedef) 
## GetDeploymentsResultTypeDef

```python
# GetDeploymentsResultTypeDef definition

class GetDeploymentsResultTypeDef(TypedDict):
    Deployments: List[EdgeDeploymentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EdgeDeploymentTypeDef](./type_defs.md#edgedeploymenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendHeartbeatRequestRequestTypeDef

```python
# SendHeartbeatRequestRequestTypeDef definition

class SendHeartbeatRequestRequestTypeDef(TypedDict):
    AgentVersion: str,
    DeviceName: str,
    DeviceFleetName: str,
    AgentMetrics: NotRequired[Sequence[EdgeMetricTypeDef]],  # (1)
    Models: NotRequired[Sequence[ModelTypeDef]],  # (2)
    DeploymentResult: NotRequired[DeploymentResultTypeDef],  # (3)
```

1. See [:material-code-braces: EdgeMetricTypeDef](./type_defs.md#edgemetrictypedef) 
2. See [:material-code-braces: ModelTypeDef](./type_defs.md#modeltypedef) 
3. See [:material-code-braces: DeploymentResultTypeDef](./type_defs.md#deploymentresulttypedef) 
