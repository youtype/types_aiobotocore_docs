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




## InternalStreamFailureTypeDef

```python
# InternalStreamFailureTypeDef definition

class InternalStreamFailureTypeDef(TypedDict):
    Message: NotRequired[str],
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
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## ModelStreamErrorTypeDef

```python
# ModelStreamErrorTypeDef definition

class ModelStreamErrorTypeDef(TypedDict):
    Message: NotRequired[str],
    ErrorCode: NotRequired[str],
```

## PayloadPartTypeDef

```python
# PayloadPartTypeDef definition

class PayloadPartTypeDef(TypedDict):
    Bytes: NotRequired[bytes],
```

## InvokeEndpointInputRequestTypeDef

```python
# InvokeEndpointInputRequestTypeDef definition

class InvokeEndpointInputRequestTypeDef(TypedDict):
    EndpointName: str,
    Body: BlobTypeDef,
    ContentType: NotRequired[str],
    Accept: NotRequired[str],
    CustomAttributes: NotRequired[str],
    TargetModel: NotRequired[str],
    TargetVariant: NotRequired[str],
    TargetContainerHostname: NotRequired[str],
    InferenceId: NotRequired[str],
    EnableExplanations: NotRequired[str],
    InferenceComponentName: NotRequired[str],
    SessionId: NotRequired[str],
```

## InvokeEndpointWithResponseStreamInputRequestTypeDef

```python
# InvokeEndpointWithResponseStreamInputRequestTypeDef definition

class InvokeEndpointWithResponseStreamInputRequestTypeDef(TypedDict):
    EndpointName: str,
    Body: BlobTypeDef,
    ContentType: NotRequired[str],
    Accept: NotRequired[str],
    CustomAttributes: NotRequired[str],
    TargetVariant: NotRequired[str],
    TargetContainerHostname: NotRequired[str],
    InferenceId: NotRequired[str],
    InferenceComponentName: NotRequired[str],
    SessionId: NotRequired[str],
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
    NewSessionId: str,
    ClosedSessionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResponseStreamTypeDef

```python
# ResponseStreamTypeDef definition

class ResponseStreamTypeDef(TypedDict):
    PayloadPart: NotRequired[PayloadPartTypeDef],  # (1)
    ModelStreamError: NotRequired[ModelStreamErrorTypeDef],  # (2)
    InternalStreamFailure: NotRequired[InternalStreamFailureTypeDef],  # (3)
```

1. See [:material-code-braces: PayloadPartTypeDef](./type_defs.md#payloadparttypedef) 
2. See [:material-code-braces: ModelStreamErrorTypeDef](./type_defs.md#modelstreamerrortypedef) 
3. See [:material-code-braces: InternalStreamFailureTypeDef](./type_defs.md#internalstreamfailuretypedef) 
## InvokeEndpointWithResponseStreamOutputTypeDef

```python
# InvokeEndpointWithResponseStreamOutputTypeDef definition

class InvokeEndpointWithResponseStreamOutputTypeDef(TypedDict):
    Body: AioEventStream[ResponseStreamTypeDef],  # (1)
    ContentType: str,
    InvokedProductionVariant: str,
    CustomAttributes: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResponseStreamTypeDef](./type_defs.md#responsestreamtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
