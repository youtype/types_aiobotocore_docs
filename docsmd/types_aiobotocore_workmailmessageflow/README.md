# WorkMailMessageFlow module

> [Index](../README.md) > WorkMailMessageFlow


!!! note ""

    Auto-generated documentation for [WorkMailMessageFlow](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#workmailmessageflow)
    type annotations stubs module [types-aiobotocore-workmailmessageflow](https://pypi.org/project/types-aiobotocore-workmailmessageflow/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `WorkMailMessageFlow` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `WorkMailMessageFlow` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[workmailmessageflow]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[workmailmessageflow]'

# standalone installation
python -m pip install types-aiobotocore-workmailmessageflow
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-workmailmessageflow
```

## Usage

Code samples can be found in [Examples](./usage.md).

## WorkMailMessageFlowClient

Type annotations and code completion for  `#!python session.create_client("workmailmessageflow")` as [WorkMailMessageFlowClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow.Client)

```python
# WorkMailMessageFlowClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_workmailmessageflow.client import WorkMailMessageFlowClient


session = get_session()
async with session.create_client("workmailmessageflow") as client:
    client: WorkMailMessageFlowClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# WorkMailMessageFlowServiceName usage example

from types_aiobotocore_workmailmessageflow.literals import WorkMailMessageFlowServiceName

def get_value() -> WorkMailMessageFlowServiceName:
    return "workmailmessageflow"
```

- [WorkMailMessageFlowServiceName](./literals.md#workmailmessageflowservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [GetRawMessageContentRequestTypeDef](./type_defs.md#getrawmessagecontentrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [S3ReferenceTypeDef](./type_defs.md#s3referencetypedef)
- [GetRawMessageContentResponseTypeDef](./type_defs.md#getrawmessagecontentresponsetypedef)
- [RawMessageContentTypeDef](./type_defs.md#rawmessagecontenttypedef)
- [PutRawMessageContentRequestTypeDef](./type_defs.md#putrawmessagecontentrequesttypedef)

