# SageMakerFeatureStoreRuntime module

> [Index](../README.md) > SageMakerFeatureStoreRuntime


!!! note ""

    Auto-generated documentation for [SageMakerFeatureStoreRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#SageMakerFeatureStoreRuntime)
    type annotations stubs module [types-aiobotocore-sagemaker-featurestore-runtime](https://pypi.org/project/types-aiobotocore-sagemaker-featurestore-runtime/).

## How to install



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

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_sagemaker_featurestore_runtime.client import SageMakerFeatureStoreRuntimeClient


session = get_session()
async with session.create_client("sagemaker-featurestore-runtime") as client:
    client: SageMakerFeatureStoreRuntimeClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_sagemaker_featurestore_runtime.literals import SageMakerFeatureStoreRuntimeServiceName

def get_value() -> SageMakerFeatureStoreRuntimeServiceName:
    return "sagemaker-featurestore-runtime"
```

- [SageMakerFeatureStoreRuntimeServiceName](./literals.md#sagemakerfeaturestoreruntimeservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_sagemaker_featurestore_runtime.type_defs import BatchGetRecordErrorTypeDef

def get_value() -> BatchGetRecordErrorTypeDef:
    return {
        "FeatureGroupName": ...,
        "RecordIdentifierValueAsString": ...,
        "ErrorCode": ...,
        "ErrorMessage": ...,
    }
```

- [BatchGetRecordErrorTypeDef](./type_defs.md#batchgetrecorderrortypedef)
- [BatchGetRecordIdentifierTypeDef](./type_defs.md#batchgetrecordidentifiertypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [FeatureValueTypeDef](./type_defs.md#featurevaluetypedef)
- [DeleteRecordRequestRequestTypeDef](./type_defs.md#deleterecordrequestrequesttypedef)
- [GetRecordRequestRequestTypeDef](./type_defs.md#getrecordrequestrequesttypedef)
- [BatchGetRecordRequestRequestTypeDef](./type_defs.md#batchgetrecordrequestrequesttypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [BatchGetRecordResultDetailTypeDef](./type_defs.md#batchgetrecordresultdetailtypedef)
- [GetRecordResponseTypeDef](./type_defs.md#getrecordresponsetypedef)
- [PutRecordRequestRequestTypeDef](./type_defs.md#putrecordrequestrequesttypedef)
- [BatchGetRecordResponseTypeDef](./type_defs.md#batchgetrecordresponsetypedef)

