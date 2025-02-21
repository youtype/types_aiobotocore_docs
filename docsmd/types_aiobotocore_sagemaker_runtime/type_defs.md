# Type definitions

> [Index](../README.md) > [SageMakerRuntime](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SageMakerRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#sagemakerruntime)
    type annotations stubs module [types-aiobotocore-sagemaker-runtime](https://pypi.org/project/types-aiobotocore-sagemaker-runtime/).

## BlobTypeDef

```python
# BlobTypeDef Union usage example

from types_aiobotocore_sagemaker_runtime.type_defs import BlobTypeDef


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




## InternalStreamFailureTypeDef

```python
# InternalStreamFailureTypeDef TypedDict usage example

from types_aiobotocore_sagemaker_runtime.type_defs import InternalStreamFailureTypeDef


def get_value() -> InternalStreamFailureTypeDef:
    return {
        "Message": ...,
    }


# InternalStreamFailureTypeDef definition

class InternalStreamFailureTypeDef(TypedDict):
    Message: NotRequired[str],
```

## InvokeEndpointAsyncInputTypeDef

```python
# InvokeEndpointAsyncInputTypeDef TypedDict usage example

from types_aiobotocore_sagemaker_runtime.type_defs import InvokeEndpointAsyncInputTypeDef


def get_value() -> InvokeEndpointAsyncInputTypeDef:
    return {
        "EndpointName": ...,
    }


# InvokeEndpointAsyncInputTypeDef definition

class InvokeEndpointAsyncInputTypeDef(TypedDict):
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
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_sagemaker_runtime.type_defs import ResponseMetadataTypeDef


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

## ModelStreamErrorTypeDef

```python
# ModelStreamErrorTypeDef TypedDict usage example

from types_aiobotocore_sagemaker_runtime.type_defs import ModelStreamErrorTypeDef


def get_value() -> ModelStreamErrorTypeDef:
    return {
        "Message": ...,
    }


# ModelStreamErrorTypeDef definition

class ModelStreamErrorTypeDef(TypedDict):
    Message: NotRequired[str],
    ErrorCode: NotRequired[str],
```

## PayloadPartTypeDef

```python
# PayloadPartTypeDef TypedDict usage example

from types_aiobotocore_sagemaker_runtime.type_defs import PayloadPartTypeDef


def get_value() -> PayloadPartTypeDef:
    return {
        "Bytes": ...,
    }


# PayloadPartTypeDef definition

class PayloadPartTypeDef(TypedDict):
    Bytes: NotRequired[bytes],
```

## InvokeEndpointInputTypeDef

```python
# InvokeEndpointInputTypeDef TypedDict usage example

from types_aiobotocore_sagemaker_runtime.type_defs import InvokeEndpointInputTypeDef


def get_value() -> InvokeEndpointInputTypeDef:
    return {
        "EndpointName": ...,
    }


# InvokeEndpointInputTypeDef definition

class InvokeEndpointInputTypeDef(TypedDict):
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

## InvokeEndpointWithResponseStreamInputTypeDef

```python
# InvokeEndpointWithResponseStreamInputTypeDef TypedDict usage example

from types_aiobotocore_sagemaker_runtime.type_defs import InvokeEndpointWithResponseStreamInputTypeDef


def get_value() -> InvokeEndpointWithResponseStreamInputTypeDef:
    return {
        "EndpointName": ...,
    }


# InvokeEndpointWithResponseStreamInputTypeDef definition

class InvokeEndpointWithResponseStreamInputTypeDef(TypedDict):
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
# InvokeEndpointAsyncOutputTypeDef TypedDict usage example

from types_aiobotocore_sagemaker_runtime.type_defs import InvokeEndpointAsyncOutputTypeDef


def get_value() -> InvokeEndpointAsyncOutputTypeDef:
    return {
        "InferenceId": ...,
    }


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
# InvokeEndpointOutputTypeDef TypedDict usage example

from types_aiobotocore_sagemaker_runtime.type_defs import InvokeEndpointOutputTypeDef


def get_value() -> InvokeEndpointOutputTypeDef:
    return {
        "Body": ...,
    }


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
# ResponseStreamTypeDef TypedDict usage example

from types_aiobotocore_sagemaker_runtime.type_defs import ResponseStreamTypeDef


def get_value() -> ResponseStreamTypeDef:
    return {
        "PayloadPart": ...,
    }


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
# InvokeEndpointWithResponseStreamOutputTypeDef TypedDict usage example

from types_aiobotocore_sagemaker_runtime.type_defs import InvokeEndpointWithResponseStreamOutputTypeDef


def get_value() -> InvokeEndpointWithResponseStreamOutputTypeDef:
    return {
        "Body": ...,
    }


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
