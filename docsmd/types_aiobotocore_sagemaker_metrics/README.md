# SageMakerMetrics module

> [Index](../README.md) > SageMakerMetrics


!!! note ""

    Auto-generated documentation for [SageMakerMetrics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics)
    type annotations stubs module [types-aiobotocore-sagemaker-metrics](https://pypi.org/project/types-aiobotocore-sagemaker-metrics/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `SageMakerMetrics` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[sagemaker-metrics]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[sagemaker-metrics]'


# standalone installation
python -m pip install types-aiobotocore-sagemaker-metrics
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-sagemaker-metrics
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SageMakerMetricsClient

Type annotations and code completion for  `#!python session.create_client("sagemaker-metrics")` as [SageMakerMetricsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics.Client)

```python
# SageMakerMetricsClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_sagemaker_metrics.client import SageMakerMetricsClient


session = get_session()
async with session.create_client("sagemaker-metrics") as client:
    client: SageMakerMetricsClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# PutMetricsErrorCodeType usage example

from types_aiobotocore_sagemaker_metrics.literals import PutMetricsErrorCodeType

def get_value() -> PutMetricsErrorCodeType:
    return "CONFLICT_ERROR"
```

- [PutMetricsErrorCodeType](./literals.md#putmetricserrorcodetype)
- [SageMakerMetricsServiceName](./literals.md#sagemakermetricsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [BatchPutMetricsErrorTypeDef](./type_defs.md#batchputmetricserrortypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [BatchPutMetricsResponseTypeDef](./type_defs.md#batchputmetricsresponsetypedef)
- [RawMetricDataTypeDef](./type_defs.md#rawmetricdatatypedef)
- [BatchPutMetricsRequestRequestTypeDef](./type_defs.md#batchputmetricsrequestrequesttypedef)

