<a id="type-annotations-for-aiobotocore-pi-module"></a>

# Type annotations for aiobotocore PI module

> [Index](..) > PI

Auto-generated documentation for
[PI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI)
type annotations stubs module
[types-aiobotocore-pi](https://pypi.org/project/types-aiobotocore-pi/).

```bash
# install with types-aiobotocore
pip install 'types-aiobotocore[pi]'

# Lite version does not provide session.create_client overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[pi]'

# standalone installation
pip install types-aiobotocore-pi
```

- [Type annotations for aiobotocore PI module](#type-annotations-for-aiobotocore-pi-module)
  - [PIClient](#piclient)
    - [Methods](#methods)
    - [Exceptions](#exceptions)
  - [Literals](#literals)
  - [Typed dictionaries](#typed-dictionaries)

<a id="piclient"></a>

## PIClient

Type annotations for `session.create_client("pi")` as [PIClient](./client.md)

Can be used directly:

```python
from types_aiobotocore_pi.client import PIClient
```

<a id="methods"></a>

### Methods

- [__aenter__](./client.md#__aenter__)
- [__aexit__](./client.md#__aexit__)
- [can_paginate](./client.md#can_paginate)
- [describe_dimension_keys](./client.md#describe_dimension_keys)
- [exceptions](./client.md#exceptions)
- [generate_presigned_url](./client.md#generate_presigned_url)
- [get_dimension_key_details](./client.md#get_dimension_key_details)
- [get_resource_metrics](./client.md#get_resource_metrics)

<a id="exceptions"></a>

### Exceptions

PIClient [exceptions](./client.md#exceptions)

- ClientError
- InternalServiceError
- InvalidArgumentException
- NotAuthorizedException

<a id="literals"></a>

## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

Can be used directly:

```python
from types_aiobotocore_pi.literals import DetailStatusType, ...
```

- [DetailStatusType](./literals.md#detailstatustype)
- [ServiceTypeType](./literals.md#servicetypetype)
- [ServiceName](./literals.md#servicename)

<a id="typed-dictionaries"></a>

## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and
schema.

Can be used directly:

```python
from mypy_boto3_pi.type_defs import DataPointTypeDef, ...
```

- [DataPointTypeDef](./type_defs.md#datapointtypedef)
- [DescribeDimensionKeysRequestRequestTypeDef](./type_defs.md#describedimensionkeysrequestrequesttypedef)
- [DescribeDimensionKeysResponseTypeDef](./type_defs.md#describedimensionkeysresponsetypedef)
- [DimensionGroupTypeDef](./type_defs.md#dimensiongrouptypedef)
- [DimensionKeyDescriptionTypeDef](./type_defs.md#dimensionkeydescriptiontypedef)
- [DimensionKeyDetailTypeDef](./type_defs.md#dimensionkeydetailtypedef)
- [GetDimensionKeyDetailsRequestRequestTypeDef](./type_defs.md#getdimensionkeydetailsrequestrequesttypedef)
- [GetDimensionKeyDetailsResponseTypeDef](./type_defs.md#getdimensionkeydetailsresponsetypedef)
- [GetResourceMetricsRequestRequestTypeDef](./type_defs.md#getresourcemetricsrequestrequesttypedef)
- [GetResourceMetricsResponseTypeDef](./type_defs.md#getresourcemetricsresponsetypedef)
- [MetricKeyDataPointsTypeDef](./type_defs.md#metrickeydatapointstypedef)
- [MetricQueryTypeDef](./type_defs.md#metricquerytypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ResponsePartitionKeyTypeDef](./type_defs.md#responsepartitionkeytypedef)
- [ResponseResourceMetricKeyTypeDef](./type_defs.md#responseresourcemetrickeytypedef)
