<a id="type-annotations-for-aiobotocore-sagemakerruntime-module"></a>

# Type annotations for aiobotocore SageMakerRuntime module

> [Index](..) > SageMakerRuntime

Auto-generated documentation for
[SageMakerRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime)
type annotations stubs module
[types-aiobotocore-sagemaker-runtime](https://pypi.org/project/types-aiobotocore-sagemaker-runtime/).

```bash
# install with types-aiobotocore
pip install 'types-aiobotocore[sagemaker-runtime]'

# install as a standalone
pip install types-aiobotocore-sagemaker-runtime
```

- [Type annotations for aiobotocore SageMakerRuntime module](#type-annotations-for-aiobotocore-sagemakerruntime-module)
  - [SageMakerRuntimeClient](#sagemakerruntimeclient)
    - [Methods](#methods)
    - [Exceptions](#exceptions)
  - [Literals](#literals)
  - [Typed dictionaries](#typed-dictionaries)

<a id="sagemakerruntimeclient"></a>

## SageMakerRuntimeClient

Type annotations for `aiobotocore.create_client("sagemaker-runtime")` as
[SageMakerRuntimeClient](./client.md)

Can be used directly:

```python
from types_aiobotocore_sagemaker_runtime.client import SageMakerRuntimeClient
```

<a id="methods"></a>

### Methods

- [can_paginate](./client.md#can_paginate)
- [exceptions](./client.md#exceptions)
- [generate_presigned_url](./client.md#generate_presigned_url)
- [invoke_endpoint](./client.md#invoke_endpoint)
- [invoke_endpoint_async](./client.md#invoke_endpoint_async)

<a id="exceptions"></a>

### Exceptions

SageMakerRuntimeClient [exceptions](./client.md#exceptions)

- ClientError
- InternalDependencyException
- InternalFailure
- ModelError
- ModelNotReadyException
- ServiceUnavailable
- ValidationError

<a id="literals"></a>

## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

Can be used directly:

```python
from types_aiobotocore_sagemaker_runtime.literals import ServiceName, ...
```

- [ServiceName](./literals.md#servicename)

<a id="typed-dictionaries"></a>

## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and
schema.

Can be used directly:

```python
from mypy_boto3_sagemaker_runtime.type_defs import InvokeEndpointAsyncInputRequestTypeDef, ...
```

- [InvokeEndpointAsyncInputRequestTypeDef](./type_defs.md#invokeendpointasyncinputrequesttypedef)
- [InvokeEndpointAsyncOutputTypeDef](./type_defs.md#invokeendpointasyncoutputtypedef)
- [InvokeEndpointInputRequestTypeDef](./type_defs.md#invokeendpointinputrequesttypedef)
- [InvokeEndpointOutputTypeDef](./type_defs.md#invokeendpointoutputtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
