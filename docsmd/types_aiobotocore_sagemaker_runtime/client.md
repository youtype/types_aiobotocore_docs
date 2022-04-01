# SageMakerRuntimeClient

> [Index](../README.md) > [SageMakerRuntime](./README.md) > SageMakerRuntimeClient

!!! note ""

    Auto-generated documentation for [SageMakerRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime)
    type annotations stubs module [types-aiobotocore-sagemaker-runtime](https://pypi.org/project/types-aiobotocore-sagemaker-runtime/).

## SageMakerRuntimeClient

Type annotations and code completion for `#!python session.create_client("sagemaker-runtime")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime.Client)

```python title="Usage example"
from aiobotocore.session import get_session
from types_aiobotocore_sagemaker_runtime.client import SageMakerRuntimeClient

session = get_session()
async with session.create_client("sagemaker-runtime") as client:
    client: SageMakerRuntimeClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("sagemaker-runtime").exceptions` structure.

```python title="Usage example"
async with session.create_client("sagemaker-runtime") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.InternalDependencyException,
        client.InternalFailure,
        client.ModelError,
        client.ModelNotReadyException,
        client.ServiceUnavailable,
        client.ValidationError,
    ) as e:
        print(e)
```

```python title="Type checking example"
from types_aiobotocore_sagemaker_runtime.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("sagemaker-runtime").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime.Client.can_paginate)

```python title="Method definition"
def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("sagemaker-runtime").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime.Client.generate_presigned_url)

```python title="Method definition"
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
services, your client applications use this API to get inferences from the model
hosted at the specified endpoint.

Type annotations and code completion for `#!python session.create_client("sagemaker-runtime").invoke_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime.Client.invoke_endpoint)

```python title="Method definition"
await def invoke_endpoint(
    self,
    *,
    EndpointName: str,
    Body: Union[bytes, IO[bytes], StreamingBody],
    ContentType: str = ...,
    Accept: str = ...,
    CustomAttributes: str = ...,
    TargetModel: str = ...,
    TargetVariant: str = ...,
    TargetContainerHostname: str = ...,
    InferenceId: str = ...,
) -> InvokeEndpointOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: InvokeEndpointOutputTypeDef](./type_defs.md#invokeendpointoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: InvokeEndpointInputRequestTypeDef = {  # (1)
    "EndpointName": ...,
    "Body": ...,
}

parent.invoke_endpoint(**kwargs)
```

1. See [:material-code-braces: InvokeEndpointInputRequestTypeDef](./type_defs.md#invokeendpointinputrequesttypedef) 

### invoke\_endpoint\_async

.

Type annotations and code completion for `#!python session.create_client("sagemaker-runtime").invoke_endpoint_async` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime.Client.invoke_endpoint_async)

```python title="Method definition"
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
) -> InvokeEndpointAsyncOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: InvokeEndpointAsyncOutputTypeDef](./type_defs.md#invokeendpointasyncoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: InvokeEndpointAsyncInputRequestTypeDef = {  # (1)
    "EndpointName": ...,
    "InputLocation": ...,
}

parent.invoke_endpoint_async(**kwargs)
```

1. See [:material-code-braces: InvokeEndpointAsyncInputRequestTypeDef](./type_defs.md#invokeendpointasyncinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("sagemaker-runtime").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime.Client.__aenter__)

```python title="Method definition"
await def __aenter__(
    self,
) -> SageMakerRuntimeClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("sagemaker-runtime").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime.Client.__aexit__)

```python title="Method definition"
await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```





