# SavingsPlans module

> [Index](../README.md) > SavingsPlans


!!! note ""

    Auto-generated documentation for [SavingsPlans](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans)
    type annotations stubs module [types-aiobotocore-savingsplans](https://pypi.org/project/types-aiobotocore-savingsplans/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `SavingsPlans`.

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

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_savingsplans.client import SavingsPlansClient


session = get_session()
async with session.create_client("savingsplans") as client:
    client: SavingsPlansClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
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




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_savingsplans.type_defs import CreateSavingsPlanRequestRequestTypeDef

def get_value() -> CreateSavingsPlanRequestRequestTypeDef:
    return {
        "savingsPlanOfferingId": ...,
        "commitment": ...,
    }
```

- [CreateSavingsPlanRequestRequestTypeDef](./type_defs.md#createsavingsplanrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteQueuedSavingsPlanRequestRequestTypeDef](./type_defs.md#deletequeuedsavingsplanrequestrequesttypedef)
- [SavingsPlanRateFilterTypeDef](./type_defs.md#savingsplanratefiltertypedef)
- [SavingsPlanOfferingRateFilterElementTypeDef](./type_defs.md#savingsplanofferingratefilterelementtypedef)
- [SavingsPlanOfferingFilterElementTypeDef](./type_defs.md#savingsplanofferingfilterelementtypedef)
- [SavingsPlanFilterTypeDef](./type_defs.md#savingsplanfiltertypedef)
- [SavingsPlanTypeDef](./type_defs.md#savingsplantypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ParentSavingsPlanOfferingTypeDef](./type_defs.md#parentsavingsplanofferingtypedef)
- [SavingsPlanOfferingPropertyTypeDef](./type_defs.md#savingsplanofferingpropertytypedef)
- [SavingsPlanOfferingRatePropertyTypeDef](./type_defs.md#savingsplanofferingratepropertytypedef)
- [SavingsPlanRatePropertyTypeDef](./type_defs.md#savingsplanratepropertytypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [CreateSavingsPlanResponseTypeDef](./type_defs.md#createsavingsplanresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [DescribeSavingsPlanRatesRequestRequestTypeDef](./type_defs.md#describesavingsplanratesrequestrequesttypedef)
- [DescribeSavingsPlansOfferingRatesRequestRequestTypeDef](./type_defs.md#describesavingsplansofferingratesrequestrequesttypedef)
- [DescribeSavingsPlansOfferingsRequestRequestTypeDef](./type_defs.md#describesavingsplansofferingsrequestrequesttypedef)
- [DescribeSavingsPlansRequestRequestTypeDef](./type_defs.md#describesavingsplansrequestrequesttypedef)
- [DescribeSavingsPlansResponseTypeDef](./type_defs.md#describesavingsplansresponsetypedef)
- [SavingsPlanOfferingTypeDef](./type_defs.md#savingsplanofferingtypedef)
- [SavingsPlanOfferingRateTypeDef](./type_defs.md#savingsplanofferingratetypedef)
- [SavingsPlanRateTypeDef](./type_defs.md#savingsplanratetypedef)
- [DescribeSavingsPlansOfferingsResponseTypeDef](./type_defs.md#describesavingsplansofferingsresponsetypedef)
- [DescribeSavingsPlansOfferingRatesResponseTypeDef](./type_defs.md#describesavingsplansofferingratesresponsetypedef)
- [DescribeSavingsPlanRatesResponseTypeDef](./type_defs.md#describesavingsplanratesresponsetypedef)

