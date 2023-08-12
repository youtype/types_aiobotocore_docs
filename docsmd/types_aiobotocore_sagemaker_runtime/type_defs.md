# Type definitions

> [Index](../README.md) > [SageMakerRuntime](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SageMakerRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime)
    type annotations stubs module [types-aiobotocore-sagemaker-runtime](https://pypi.org/project/types-aiobotocore-sagemaker-runtime/).

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




## InvokeEndpointAsyncInputRequestTypeDef

```python
# InvokeEndpointAsyncInputRequestTypeDef definition

class InvokeEndpointAsyncInputRequestTypeDef(TypedDict):
    EndpointName: str,
    InputLocation: str,
    ContentType: NotRequired[str],
    Accept: NotRequired[str],
    CustomAttributes: NotRequired[str],
    InferenceId: NotRequired[str],
    RequestTTLSeconds: NotRequired[int],
    InvocationTimeoutSeconds: NotRequired[int],
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

## InvokeEndpointInputRequestTypeDef

```python
# InvokeEndpointInputRequestTypeDef definition

class InvokeEndpointInputRequestTypeDef(TypedDict):
    EndpointName: str,
    Body: Union[str, bytes, IO[Any], StreamingBody],
    ContentType: NotRequired[str],
    Accept: NotRequired[str],
    CustomAttributes: NotRequired[str],
    TargetModel: NotRequired[str],
    TargetVariant: NotRequired[str],
    TargetContainerHostname: NotRequired[str],
    InferenceId: NotRequired[str],
    EnableExplanations: NotRequired[str],
```

## InvokeEndpointAsyncOutputTypeDef

```python
# InvokeEndpointAsyncOutputTypeDef definition

class InvokeEndpointAsyncOutputTypeDef(TypedDict):
    InferenceId: str,
    OutputLocation: str,
    FailureLocation: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InvokeEndpointOutputTypeDef

```python
# InvokeEndpointOutputTypeDef definition

class InvokeEndpointOutputTypeDef(TypedDict):
    Body: StreamingBody,
    ContentType: str,
    InvokedProductionVariant: str,
    CustomAttributes: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
