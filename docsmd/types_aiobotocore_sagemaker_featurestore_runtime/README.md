# SageMakerFeatureStoreRuntime module

> [Index](../README.md) > SageMakerFeatureStoreRuntime


!!! note ""

    Auto-generated documentation for [SageMakerFeatureStoreRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#sagemakerfeaturestoreruntime)
    type annotations stubs module [types-aiobotocore-sagemaker-featurestore-runtime](https://pypi.org/project/types-aiobotocore-sagemaker-featurestore-runtime/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `SageMakerFeatureStoreRuntime` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `SageMakerFeatureStoreRuntime` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[sagemaker-featurestore-runtime]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[sagemaker-featurestore-runtime]'

# standalone installation
python -m pip install types-aiobotocore-sagemaker-featurestore-runtime
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-sagemaker-featurestore-runtime
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SageMakerFeatureStoreRuntimeClient

Type annotations and code completion for  `#!python session.create_client("sagemaker-featurestore-runtime")` as [SageMakerFeatureStoreRuntimeClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime.Client)

```python
# SageMakerFeatureStoreRuntimeClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_sagemaker_featurestore_runtime.client import SageMakerFeatureStoreRuntimeClient


session = get_session()
async with session.create_client("sagemaker-featurestore-runtime") as client:
    client: SageMakerFeatureStoreRuntimeClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# DeletionModeType usage example

from types_aiobotocore_sagemaker_featurestore_runtime.literals import DeletionModeType

def get_value() -> DeletionModeType:
    return "HardDelete"
```

- [DeletionModeType](./literals.md#deletionmodetype)
- [ExpirationTimeResponseType](./literals.md#expirationtimeresponsetype)
- [TargetStoreType](./literals.md#targetstoretype)
- [TtlDurationUnitType](./literals.md#ttldurationunittype)
- [SageMakerFeatureStoreRuntimeServiceName](./literals.md#sagemakerfeaturestoreruntimeservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [BatchGetRecordErrorTypeDef](./type_defs.md#batchgetrecorderrortypedef)
- [BatchGetRecordIdentifierOutputTypeDef](./type_defs.md#batchgetrecordidentifieroutputtypedef)
- [BatchGetRecordIdentifierTypeDef](./type_defs.md#batchgetrecordidentifiertypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [FeatureValueOutputTypeDef](./type_defs.md#featurevalueoutputtypedef)
- [DeleteRecordRequestTypeDef](./type_defs.md#deleterecordrequesttypedef)
- [FeatureValueTypeDef](./type_defs.md#featurevaluetypedef)
- [GetRecordRequestTypeDef](./type_defs.md#getrecordrequesttypedef)
- [TtlDurationTypeDef](./type_defs.md#ttldurationtypedef)
- [BatchGetRecordIdentifierUnionTypeDef](./type_defs.md#batchgetrecordidentifieruniontypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [BatchGetRecordResultDetailTypeDef](./type_defs.md#batchgetrecordresultdetailtypedef)
- [GetRecordResponseTypeDef](./type_defs.md#getrecordresponsetypedef)
- [FeatureValueUnionTypeDef](./type_defs.md#featurevalueuniontypedef)
- [BatchGetRecordRequestTypeDef](./type_defs.md#batchgetrecordrequesttypedef)
- [BatchGetRecordResponseTypeDef](./type_defs.md#batchgetrecordresponsetypedef)
- [PutRecordRequestTypeDef](./type_defs.md#putrecordrequesttypedef)

