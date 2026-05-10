# Sustainability module

> [Index](../README.md) > Sustainability


!!! note ""

    Auto-generated documentation for [Sustainability](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sustainability.html#sustainability)
    type annotations stubs module [types-aiobotocore-sustainability](https://pypi.org/project/types-aiobotocore-sustainability/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.7.0' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `Sustainability` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `Sustainability` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[sustainability]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[sustainability]'

# standalone installation
python -m pip install types-aiobotocore-sustainability
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-sustainability
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SustainabilityClient

Type annotations and code completion for  `#!python session.create_client("sustainability")` as [SustainabilityClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sustainability.html#Sustainability.Client)

```python
# SustainabilityClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_sustainability.client import SustainabilityClient


session = get_session()
async with session.create_client("sustainability") as client:
    client: SustainabilityClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("sustainability").get_paginator("...")`.

```python
# GetEstimatedCarbonEmissionsDimensionValuesPaginator usage example

from types_aiobotocore_sustainability.paginator import GetEstimatedCarbonEmissionsDimensionValuesPaginator

def get_get_estimated_carbon_emissions_dimension_values_paginator() -> GetEstimatedCarbonEmissionsDimensionValuesPaginator:
    return client.get_paginator("get_estimated_carbon_emissions_dimension_values"))
```

- [GetEstimatedCarbonEmissionsDimensionValuesPaginator](./paginators.md#getestimatedcarbonemissionsdimensionvaluespaginator)
- [GetEstimatedCarbonEmissionsPaginator](./paginators.md#getestimatedcarbonemissionspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# DimensionType usage example

from types_aiobotocore_sustainability.literals import DimensionType

def get_value() -> DimensionType:
    return "REGION"
```

- [DimensionType](./literals.md#dimensiontype)
- [EmissionsTypeType](./literals.md#emissionstypetype)
- [EmissionsUnitType](./literals.md#emissionsunittype)
- [GetEstimatedCarbonEmissionsDimensionValuesPaginatorName](./literals.md#getestimatedcarbonemissionsdimensionvaluespaginatorname)
- [GetEstimatedCarbonEmissionsPaginatorName](./literals.md#getestimatedcarbonemissionspaginatorname)
- [TimeGranularityType](./literals.md#timegranularitytype)
- [SustainabilityServiceName](./literals.md#sustainabilityservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [DimensionEntryTypeDef](./type_defs.md#dimensionentrytypedef)
- [EmissionsTypeDef](./type_defs.md#emissionstypedef)
- [TimePeriodOutputTypeDef](./type_defs.md#timeperiodoutputtypedef)
- [FilterExpressionTypeDef](./type_defs.md#filterexpressiontypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [GranularityConfigurationTypeDef](./type_defs.md#granularityconfigurationtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [EstimatedCarbonEmissionsTypeDef](./type_defs.md#estimatedcarbonemissionstypedef)
- [GetEstimatedCarbonEmissionsDimensionValuesResponseTypeDef](./type_defs.md#getestimatedcarbonemissionsdimensionvaluesresponsetypedef)
- [TimePeriodTypeDef](./type_defs.md#timeperiodtypedef)
- [GetEstimatedCarbonEmissionsResponseTypeDef](./type_defs.md#getestimatedcarbonemissionsresponsetypedef)
- [TimePeriodUnionTypeDef](./type_defs.md#timeperioduniontypedef)
- [GetEstimatedCarbonEmissionsDimensionValuesRequestPaginateTypeDef](./type_defs.md#getestimatedcarbonemissionsdimensionvaluesrequestpaginatetypedef)
- [GetEstimatedCarbonEmissionsDimensionValuesRequestTypeDef](./type_defs.md#getestimatedcarbonemissionsdimensionvaluesrequesttypedef)
- [GetEstimatedCarbonEmissionsRequestPaginateTypeDef](./type_defs.md#getestimatedcarbonemissionsrequestpaginatetypedef)
- [GetEstimatedCarbonEmissionsRequestTypeDef](./type_defs.md#getestimatedcarbonemissionsrequesttypedef)

