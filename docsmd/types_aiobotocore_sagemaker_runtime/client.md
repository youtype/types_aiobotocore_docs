# SageMakerRuntimeClient

> [Index](../README.md) > [SageMakerRuntime](./README.md) > SageMakerRuntimeClient

!!! note ""

    Auto-generated documentation for [SageMakerRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#sagemakerruntime)
    type annotations stubs module [types-aiobotocore-sagemaker-runtime](https://pypi.org/project/types-aiobotocore-sagemaker-runtime/).

## SageMakerRuntimeClient

Type annotations and code completion for `#!python session.create_client("sagemaker-runtime")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime.Client)

```python
# SageMakerRuntimeClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_sagemaker_runtime.client import SageMakerRuntimeClient

session = get_session()
async with session.create_client("sagemaker-runtime") as client:
    client: SageMakerRuntimeClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("sagemaker-runtime").exceptions` structure.

```python
# SageMakerRuntimeClient.exceptions usage example

async with session.create_client("sagemaker-runtime") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.InternalDependencyException,
        client.InternalFailure,
        client.InternalStreamFailure,
        client.ModelError,
        client.ModelNotReadyException,
        client.ModelStreamError,
        client.ServiceUnavailable,
        client.ValidationError,
    ) as e:
        print(e)
```

```python
# SageMakerRuntimeClient usage type checking example

from types_aiobotocore_sagemaker_runtime.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("sagemaker-runtime").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("sagemaker-runtime").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### invoke\_endpoint

After you deploy a model into production using Amazon SageMaker hosting
services, your client applications use this API to get inferences from the
model hosted at the specified endpoint.

Type annotations and code completion for `#!python session.create_client("sagemaker-runtime").invoke_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime/client/invoke_endpoint.html)

```python
# invoke_endpoint method definition

await def invoke_endpoint(
    self,
    *,
    EndpointName: str,
    Body: BlobTypeDef,
    ContentType: str = ...,
    Accept: str = ...,
    CustomAttributes: str = ...,
    TargetModel: str = ...,
    TargetVariant: str = ...,
    TargetContainerHostname: str = ...,
    InferenceId: str = ...,
    EnableExplanations: str = ...,
    InferenceComponentName: str = ...,
    SessionId: str = ...,
) -> InvokeEndpointOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: InvokeEndpointOutputTypeDef](./type_defs.md#invokeendpointoutputtypedef) 


```python
# invoke_endpoint method usage example with argument unpacking

kwargs: InvokeEndpointInputTypeDef = {  # (1)
    "EndpointName": ...,
    "Body": ...,
}

parent.invoke_endpoint(**kwargs)
```

1. See [:material-code-braces: InvokeEndpointInputTypeDef](./type_defs.md#invokeendpointinputtypedef) 

### invoke\_endpoint\_async

After you deploy a model into production using Amazon SageMaker hosting
services, your client applications use this API to get inferences from the
model hosted at the specified endpoint in an asynchronous manner.

Type annotations and code completion for `#!python session.create_client("sagemaker-runtime").invoke_endpoint_async` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime/client/invoke_endpoint_async.html)

```python
# invoke_endpoint_async method definition

await def invoke_endpoint_async(
    self,
    *,
    EndpointName: str,
    InputLocation: str,
    ContentType: str = ...,
    Accept: str = ...,
    CustomAttributes: str = ...,
    InferenceId: str = ...,
    RequestTTLSeconds: int = ...,
    InvocationTimeoutSeconds: int = ...,
) -> InvokeEndpointAsyncOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: InvokeEndpointAsyncOutputTypeDef](./type_defs.md#invokeendpointasyncoutputtypedef) 


```python
# invoke_endpoint_async method usage example with argument unpacking

kwargs: InvokeEndpointAsyncInputTypeDef = {  # (1)
    "EndpointName": ...,
    "InputLocation": ...,
}

parent.invoke_endpoint_async(**kwargs)
```

1. See [:material-code-braces: InvokeEndpointAsyncInputTypeDef](./type_defs.md#invokeendpointasyncinputtypedef) 

### invoke\_endpoint\_with\_response\_stream

Invokes a model at the specified endpoint to return the inference response as a
stream.

Type annotations and code completion for `#!python session.create_client("sagemaker-runtime").invoke_endpoint_with_response_stream` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime/client/invoke_endpoint_with_response_stream.html)

```python
# invoke_endpoint_with_response_stream method definition

await def invoke_endpoint_with_response_stream(
    self,
    *,
    EndpointName: str,
    Body: BlobTypeDef,
    ContentType: str = ...,
    Accept: str = ...,
    CustomAttributes: str = ...,
    TargetVariant: str = ...,
    TargetContainerHostname: str = ...,
    InferenceId: str = ...,
    InferenceComponentName: str = ...,
    SessionId: str = ...,
) -> InvokeEndpointWithResponseStreamOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: InvokeEndpointWithResponseStreamOutputTypeDef](./type_defs.md#invokeendpointwithresponsestreamoutputtypedef) 


```python
# invoke_endpoint_with_response_stream method usage example with argument unpacking

kwargs: InvokeEndpointWithResponseStreamInputTypeDef = {  # (1)
    "EndpointName": ...,
    "Body": ...,
}

parent.invoke_endpoint_with_response_stream(**kwargs)
```

1. See [:material-code-braces: InvokeEndpointWithResponseStreamInputTypeDef](./type_defs.md#invokeendpointwithresponsestreaminputtypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("sagemaker-runtime").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("sagemaker-runtime").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```





