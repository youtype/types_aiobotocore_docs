# MarketplaceMetering module

> [Index](../README.md) > MarketplaceMetering


!!! note ""

    Auto-generated documentation for [MarketplaceMetering](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#marketplacemetering)
    type annotations stubs module [types-aiobotocore-meteringmarketplace](https://pypi.org/project/types-aiobotocore-meteringmarketplace/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.24.2' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `MarketplaceMetering` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `MarketplaceMetering` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[meteringmarketplace]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[meteringmarketplace]'

# standalone installation
python -m pip install types-aiobotocore-meteringmarketplace
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-meteringmarketplace
```

## Usage

Code samples can be found in [Examples](./usage.md).

## MarketplaceMeteringClient

Type annotations and code completion for  `#!python session.create_client("meteringmarketplace")` as [MarketplaceMeteringClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering.Client)

```python
# MarketplaceMeteringClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_meteringmarketplace.client import MarketplaceMeteringClient


session = get_session()
async with session.create_client("meteringmarketplace") as client:
    client: MarketplaceMeteringClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# UsageRecordResultStatusType usage example

from types_aiobotocore_meteringmarketplace.literals import UsageRecordResultStatusType

def get_value() -> UsageRecordResultStatusType:
    return "CustomerNotSubscribed"
```

- [UsageRecordResultStatusType](./literals.md#usagerecordresultstatustype)
- [MarketplaceMeteringServiceName](./literals.md#marketplacemeteringservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [RegisterUsageRequestTypeDef](./type_defs.md#registerusagerequesttypedef)
- [ResolveCustomerRequestTypeDef](./type_defs.md#resolvecustomerrequesttypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [MeterUsageResultTypeDef](./type_defs.md#meterusageresulttypedef)
- [RegisterUsageResultTypeDef](./type_defs.md#registerusageresulttypedef)
- [ResolveCustomerResultTypeDef](./type_defs.md#resolvecustomerresulttypedef)
- [UsageAllocationOutputTypeDef](./type_defs.md#usageallocationoutputtypedef)
- [UsageAllocationTypeDef](./type_defs.md#usageallocationtypedef)
- [UsageRecordOutputTypeDef](./type_defs.md#usagerecordoutputtypedef)
- [UsageAllocationUnionTypeDef](./type_defs.md#usageallocationuniontypedef)
- [UsageRecordResultTypeDef](./type_defs.md#usagerecordresulttypedef)
- [MeterUsageRequestTypeDef](./type_defs.md#meterusagerequesttypedef)
- [UsageRecordTypeDef](./type_defs.md#usagerecordtypedef)
- [BatchMeterUsageResultTypeDef](./type_defs.md#batchmeterusageresulttypedef)
- [UsageRecordUnionTypeDef](./type_defs.md#usagerecorduniontypedef)
- [BatchMeterUsageRequestTypeDef](./type_defs.md#batchmeterusagerequesttypedef)

