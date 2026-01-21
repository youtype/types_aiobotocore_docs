# SavingsPlans module

> [Index](../README.md) > SavingsPlans


!!! note ""

    Auto-generated documentation for [SavingsPlans](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#savingsplans)
    type annotations stubs module [types-aiobotocore-savingsplans](https://pypi.org/project/types-aiobotocore-savingsplans/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `SavingsPlans` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `SavingsPlans` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[savingsplans]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[savingsplans]'

# standalone installation
python -m pip install types-aiobotocore-savingsplans
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-savingsplans
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SavingsPlansClient

Type annotations and code completion for  `#!python session.create_client("savingsplans")` as [SavingsPlansClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans.Client)

```python
# SavingsPlansClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_savingsplans.client import SavingsPlansClient


session = get_session()
async with session.create_client("savingsplans") as client:
    client: SavingsPlansClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# CurrencyCodeType usage example

from types_aiobotocore_savingsplans.literals import CurrencyCodeType

def get_value() -> CurrencyCodeType:
    return "CNY"
```

- [CurrencyCodeType](./literals.md#currencycodetype)
- [SavingsPlanOfferingFilterAttributeType](./literals.md#savingsplanofferingfilterattributetype)
- [SavingsPlanOfferingPropertyKeyType](./literals.md#savingsplanofferingpropertykeytype)
- [SavingsPlanPaymentOptionType](./literals.md#savingsplanpaymentoptiontype)
- [SavingsPlanProductTypeType](./literals.md#savingsplanproducttypetype)
- [SavingsPlanRateFilterAttributeType](./literals.md#savingsplanratefilterattributetype)
- [SavingsPlanRateFilterNameType](./literals.md#savingsplanratefilternametype)
- [SavingsPlanRatePropertyKeyType](./literals.md#savingsplanratepropertykeytype)
- [SavingsPlanRateServiceCodeType](./literals.md#savingsplanrateservicecodetype)
- [SavingsPlanRateUnitType](./literals.md#savingsplanrateunittype)
- [SavingsPlanStateType](./literals.md#savingsplanstatetype)
- [SavingsPlanTypeType](./literals.md#savingsplantypetype)
- [SavingsPlansFilterNameType](./literals.md#savingsplansfilternametype)
- [SavingsPlansServiceName](./literals.md#savingsplansservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteQueuedSavingsPlanRequestTypeDef](./type_defs.md#deletequeuedsavingsplanrequesttypedef)
- [SavingsPlanRateFilterTypeDef](./type_defs.md#savingsplanratefiltertypedef)
- [SavingsPlanOfferingRateFilterElementTypeDef](./type_defs.md#savingsplanofferingratefilterelementtypedef)
- [SavingsPlanOfferingFilterElementTypeDef](./type_defs.md#savingsplanofferingfilterelementtypedef)
- [SavingsPlanFilterTypeDef](./type_defs.md#savingsplanfiltertypedef)
- [SavingsPlanTypeDef](./type_defs.md#savingsplantypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [ParentSavingsPlanOfferingTypeDef](./type_defs.md#parentsavingsplanofferingtypedef)
- [ReturnSavingsPlanRequestTypeDef](./type_defs.md#returnsavingsplanrequesttypedef)
- [SavingsPlanOfferingPropertyTypeDef](./type_defs.md#savingsplanofferingpropertytypedef)
- [SavingsPlanOfferingRatePropertyTypeDef](./type_defs.md#savingsplanofferingratepropertytypedef)
- [SavingsPlanRatePropertyTypeDef](./type_defs.md#savingsplanratepropertytypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [CreateSavingsPlanRequestTypeDef](./type_defs.md#createsavingsplanrequesttypedef)
- [CreateSavingsPlanResponseTypeDef](./type_defs.md#createsavingsplanresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ReturnSavingsPlanResponseTypeDef](./type_defs.md#returnsavingsplanresponsetypedef)
- [DescribeSavingsPlanRatesRequestTypeDef](./type_defs.md#describesavingsplanratesrequesttypedef)
- [DescribeSavingsPlansOfferingRatesRequestTypeDef](./type_defs.md#describesavingsplansofferingratesrequesttypedef)
- [DescribeSavingsPlansOfferingsRequestTypeDef](./type_defs.md#describesavingsplansofferingsrequesttypedef)
- [DescribeSavingsPlansRequestTypeDef](./type_defs.md#describesavingsplansrequesttypedef)
- [DescribeSavingsPlansResponseTypeDef](./type_defs.md#describesavingsplansresponsetypedef)
- [SavingsPlanOfferingTypeDef](./type_defs.md#savingsplanofferingtypedef)
- [SavingsPlanOfferingRateTypeDef](./type_defs.md#savingsplanofferingratetypedef)
- [SavingsPlanRateTypeDef](./type_defs.md#savingsplanratetypedef)
- [DescribeSavingsPlansOfferingsResponseTypeDef](./type_defs.md#describesavingsplansofferingsresponsetypedef)
- [DescribeSavingsPlansOfferingRatesResponseTypeDef](./type_defs.md#describesavingsplansofferingratesresponsetypedef)
- [DescribeSavingsPlanRatesResponseTypeDef](./type_defs.md#describesavingsplanratesresponsetypedef)

