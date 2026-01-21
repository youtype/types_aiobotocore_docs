# SageMakerMetrics module

> [Index](../README.md) > SageMakerMetrics


!!! note ""

    Auto-generated documentation for [SageMakerMetrics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#sagemakermetrics)
    type annotations stubs module [types-aiobotocore-sagemaker-metrics](https://pypi.org/project/types-aiobotocore-sagemaker-metrics/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `SageMakerMetrics` service.
1. Use provided commands to install generated packages.



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
# MetricQueryResultStatusType usage example

from types_aiobotocore_sagemaker_metrics.literals import MetricQueryResultStatusType

def get_value() -> MetricQueryResultStatusType:
    return "Complete"
```

- [MetricQueryResultStatusType](./literals.md#metricqueryresultstatustype)
- [MetricStatisticType](./literals.md#metricstatistictype)
- [PeriodType](./literals.md#periodtype)
- [PutMetricsErrorCodeType](./literals.md#putmetricserrorcodetype)
- [XAxisTypeType](./literals.md#xaxistypetype)
- [SageMakerMetricsServiceName](./literals.md#sagemakermetricsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [MetricQueryTypeDef](./type_defs.md#metricquerytypedef)
- [MetricQueryResultTypeDef](./type_defs.md#metricqueryresulttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BatchPutMetricsErrorTypeDef](./type_defs.md#batchputmetricserrortypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [BatchGetMetricsRequestTypeDef](./type_defs.md#batchgetmetricsrequesttypedef)
- [BatchGetMetricsResponseTypeDef](./type_defs.md#batchgetmetricsresponsetypedef)
- [BatchPutMetricsResponseTypeDef](./type_defs.md#batchputmetricsresponsetypedef)
- [RawMetricDataTypeDef](./type_defs.md#rawmetricdatatypedef)
- [BatchPutMetricsRequestTypeDef](./type_defs.md#batchputmetricsrequesttypedef)

