<a id="type-annotations-for-aiobotocore-sagemakerruntime-module"></a>

# Type annotations for aiobotocore SageMakerRuntime module

> [Index](..) > SageMakerRuntime

Auto-generated documentation for
[SageMakerRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#SageMakerRuntime)
type annotations stubs module
[types-aiobotocore-sagemaker-runtime](https://pypi.org/project/types-aiobotocore-sagemaker-runtime/).

- [Type annotations for aiobotocore SageMakerRuntime module](#type-annotations-for-aiobotocore-sagemakerruntime-module)
  - [How to install](#how-to-install)
    - [VSCode extension](#vscode-extension)
    - [From PyPI with pip](#from-pypi-with-pip)
  - [How to uninstall](#how-to-uninstall)
  - [SageMakerRuntimeClient](#sagemakerruntimeclient)
    - [Methods](#methods)
    - [Exceptions](#exceptions)
  - [Literals](#literals)
  - [Typed dictionaries](#typed-dictionaries)

<a id="how-to-install"></a>

## How to install

<a id="vscode-extension"></a>

### VSCode extension

Add
[AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `SageMakerRuntime`.

<a id="from-pypi-with-pip"></a>

### From PyPI with pip

Install `types-aiobotocore` for `SageMakerRuntime` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[sagemaker-runtime]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[sagemaker-runtime]'

# standalone installation
python -m pip install types-aiobotocore-sagemaker-runtime
```

<a id="how-to-uninstall"></a>

## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-sagemaker-runtime
```

<a id="sagemakerruntimeclient"></a>

## SageMakerRuntimeClient

Type annotations for `session.create_client("sagemaker-runtime")` as
[SageMakerRuntimeClient](./client.md)

Can be used directly:

```python
from types_aiobotocore_sagemaker_runtime.client import SageMakerRuntimeClient
```

<a id="methods"></a>

### Methods

- [__aenter__](./client.md#__aenter__)
- [__aexit__](./client.md#__aexit__)
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
