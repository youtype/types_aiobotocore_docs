# PI module

> [Index](../README.md) > PI


!!! note ""

    Auto-generated documentation for [PI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
    type annotations stubs module [types-aiobotocore-pi](https://pypi.org/project/types-aiobotocore-pi/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `PI` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[pi]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[pi]'


# standalone installation
python -m pip install types-aiobotocore-pi
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-pi
```

## Usage

Code samples can be found in [Examples](./usage.md).

## PIClient

Type annotations and code completion for  `#!python session.create_client("pi")` as [PIClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_pi.client import PIClient


session = get_session()
async with session.create_client("pi") as client:
    client: PIClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_pi.literals import DetailStatusType

def get_value() -> DetailStatusType:
    return "AVAILABLE"
```

- [DetailStatusType](./literals.md#detailstatustype)
- [FeatureStatusType](./literals.md#featurestatustype)
- [ServiceTypeType](./literals.md#servicetypetype)
- [PIServiceName](./literals.md#piservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_pi.type_defs import DataPointTypeDef

def get_value() -> DataPointTypeDef:
    return {
        "Timestamp": ...,
        "Value": ...,
    }
```

- [DataPointTypeDef](./type_defs.md#datapointtypedef)
- [DimensionGroupTypeDef](./type_defs.md#dimensiongrouptypedef)
- [DimensionKeyDescriptionTypeDef](./type_defs.md#dimensionkeydescriptiontypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ResponsePartitionKeyTypeDef](./type_defs.md#responsepartitionkeytypedef)
- [DimensionDetailTypeDef](./type_defs.md#dimensiondetailtypedef)
- [DimensionKeyDetailTypeDef](./type_defs.md#dimensionkeydetailtypedef)
- [FeatureMetadataTypeDef](./type_defs.md#featuremetadatatypedef)
- [GetDimensionKeyDetailsRequestRequestTypeDef](./type_defs.md#getdimensionkeydetailsrequestrequesttypedef)
- [GetResourceMetadataRequestRequestTypeDef](./type_defs.md#getresourcemetadatarequestrequesttypedef)
- [ListAvailableResourceDimensionsRequestRequestTypeDef](./type_defs.md#listavailableresourcedimensionsrequestrequesttypedef)
- [ListAvailableResourceMetricsRequestRequestTypeDef](./type_defs.md#listavailableresourcemetricsrequestrequesttypedef)
- [ResponseResourceMetricTypeDef](./type_defs.md#responseresourcemetrictypedef)
- [ResponseResourceMetricKeyTypeDef](./type_defs.md#responseresourcemetrickeytypedef)
- [DescribeDimensionKeysRequestRequestTypeDef](./type_defs.md#describedimensionkeysrequestrequesttypedef)
- [MetricQueryTypeDef](./type_defs.md#metricquerytypedef)
- [DescribeDimensionKeysResponseTypeDef](./type_defs.md#describedimensionkeysresponsetypedef)
- [DimensionGroupDetailTypeDef](./type_defs.md#dimensiongroupdetailtypedef)
- [GetDimensionKeyDetailsResponseTypeDef](./type_defs.md#getdimensionkeydetailsresponsetypedef)
- [GetResourceMetadataResponseTypeDef](./type_defs.md#getresourcemetadataresponsetypedef)
- [ListAvailableResourceMetricsResponseTypeDef](./type_defs.md#listavailableresourcemetricsresponsetypedef)
- [MetricKeyDataPointsTypeDef](./type_defs.md#metrickeydatapointstypedef)
- [GetResourceMetricsRequestRequestTypeDef](./type_defs.md#getresourcemetricsrequestrequesttypedef)
- [MetricDimensionGroupsTypeDef](./type_defs.md#metricdimensiongroupstypedef)
- [GetResourceMetricsResponseTypeDef](./type_defs.md#getresourcemetricsresponsetypedef)
- [ListAvailableResourceDimensionsResponseTypeDef](./type_defs.md#listavailableresourcedimensionsresponsetypedef)

