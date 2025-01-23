# BillingandCostManagementPricingCalculator module

> [Index](../README.md) > BillingandCostManagementPricingCalculator


!!! note ""

    Auto-generated documentation for [BillingandCostManagementPricingCalculator](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-pricing-calculator.html#billingandcostmanagementpricingcalculator)
    type annotations stubs module [types-aiobotocore-bcm-pricing-calculator](https://pypi.org/project/types-aiobotocore-bcm-pricing-calculator/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `BillingandCostManagementPricingCalculator` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `BillingandCostManagementPricingCalculator` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[bcm-pricing-calculator]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[bcm-pricing-calculator]'

# standalone installation
python -m pip install types-aiobotocore-bcm-pricing-calculator
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-bcm-pricing-calculator
```

## Usage

Code samples can be found in [Examples](./usage.md).

## BillingandCostManagementPricingCalculatorClient

Type annotations and code completion for  `#!python session.create_client("bcm-pricing-calculator")` as [BillingandCostManagementPricingCalculatorClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-pricing-calculator.html#BillingandCostManagementPricingCalculator.Client)

```python
# BillingandCostManagementPricingCalculatorClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_bcm_pricing_calculator.client import BillingandCostManagementPricingCalculatorClient


session = get_session()
async with session.create_client("bcm-pricing-calculator") as client:
    client: BillingandCostManagementPricingCalculatorClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("bcm-pricing-calculator").get_paginator("...")`.

```python
# ListBillEstimateCommitmentsPaginator usage example

from types_aiobotocore_bcm_pricing_calculator.paginator import ListBillEstimateCommitmentsPaginator

def get_list_bill_estimate_commitments_paginator() -> ListBillEstimateCommitmentsPaginator:
    return client.get_paginator("list_bill_estimate_commitments"))
```

- [ListBillEstimateCommitmentsPaginator](./paginators.md#listbillestimatecommitmentspaginator)
- [ListBillEstimateInputCommitmentModificationsPaginator](./paginators.md#listbillestimateinputcommitmentmodificationspaginator)
- [ListBillEstimateInputUsageModificationsPaginator](./paginators.md#listbillestimateinputusagemodificationspaginator)
- [ListBillEstimateLineItemsPaginator](./paginators.md#listbillestimatelineitemspaginator)
- [ListBillEstimatesPaginator](./paginators.md#listbillestimatespaginator)
- [ListBillScenarioCommitmentModificationsPaginator](./paginators.md#listbillscenariocommitmentmodificationspaginator)
- [ListBillScenarioUsageModificationsPaginator](./paginators.md#listbillscenariousagemodificationspaginator)
- [ListBillScenariosPaginator](./paginators.md#listbillscenariospaginator)
- [ListWorkloadEstimateUsagePaginator](./paginators.md#listworkloadestimateusagepaginator)
- [ListWorkloadEstimatesPaginator](./paginators.md#listworkloadestimatespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# BatchCreateBillScenarioCommitmentModificationErrorCodeType usage example

from types_aiobotocore_bcm_pricing_calculator.literals import BatchCreateBillScenarioCommitmentModificationErrorCodeType

def get_value() -> BatchCreateBillScenarioCommitmentModificationErrorCodeType:
    return "CONFLICT"
```

- [BatchCreateBillScenarioCommitmentModificationErrorCodeType](./literals.md#batchcreatebillscenariocommitmentmodificationerrorcodetype)
- [BatchCreateBillScenarioUsageModificationErrorCodeType](./literals.md#batchcreatebillscenariousagemodificationerrorcodetype)
- [BatchCreateWorkloadEstimateUsageCodeType](./literals.md#batchcreateworkloadestimateusagecodetype)
- [BatchDeleteBillScenarioCommitmentModificationErrorCodeType](./literals.md#batchdeletebillscenariocommitmentmodificationerrorcodetype)
- [BatchDeleteBillScenarioUsageModificationErrorCodeType](./literals.md#batchdeletebillscenariousagemodificationerrorcodetype)
- [BatchUpdateBillScenarioCommitmentModificationErrorCodeType](./literals.md#batchupdatebillscenariocommitmentmodificationerrorcodetype)
- [BatchUpdateBillScenarioUsageModificationErrorCodeType](./literals.md#batchupdatebillscenariousagemodificationerrorcodetype)
- [BillEstimateStatusType](./literals.md#billestimatestatustype)
- [BillScenarioStatusType](./literals.md#billscenariostatustype)
- [CurrencyCodeType](./literals.md#currencycodetype)
- [ListBillEstimateCommitmentsPaginatorName](./literals.md#listbillestimatecommitmentspaginatorname)
- [ListBillEstimateInputCommitmentModificationsPaginatorName](./literals.md#listbillestimateinputcommitmentmodificationspaginatorname)
- [ListBillEstimateInputUsageModificationsPaginatorName](./literals.md#listbillestimateinputusagemodificationspaginatorname)
- [ListBillEstimateLineItemsFilterNameType](./literals.md#listbillestimatelineitemsfilternametype)
- [ListBillEstimateLineItemsPaginatorName](./literals.md#listbillestimatelineitemspaginatorname)
- [ListBillEstimatesFilterNameType](./literals.md#listbillestimatesfilternametype)
- [ListBillEstimatesPaginatorName](./literals.md#listbillestimatespaginatorname)
- [ListBillScenarioCommitmentModificationsPaginatorName](./literals.md#listbillscenariocommitmentmodificationspaginatorname)
- [ListBillScenarioUsageModificationsPaginatorName](./literals.md#listbillscenariousagemodificationspaginatorname)
- [ListBillScenariosFilterNameType](./literals.md#listbillscenariosfilternametype)
- [ListBillScenariosPaginatorName](./literals.md#listbillscenariospaginatorname)
- [ListUsageFilterNameType](./literals.md#listusagefilternametype)
- [ListWorkloadEstimateUsagePaginatorName](./literals.md#listworkloadestimateusagepaginatorname)
- [ListWorkloadEstimatesFilterNameType](./literals.md#listworkloadestimatesfilternametype)
- [ListWorkloadEstimatesPaginatorName](./literals.md#listworkloadestimatespaginatorname)
- [MatchOptionType](./literals.md#matchoptiontype)
- [PurchaseAgreementTypeType](./literals.md#purchaseagreementtypetype)
- [RateTypeType](./literals.md#ratetypetype)
- [WorkloadEstimateCostStatusType](./literals.md#workloadestimatecoststatustype)
- [WorkloadEstimateRateTypeType](./literals.md#workloadestimateratetypetype)
- [WorkloadEstimateStatusType](./literals.md#workloadestimatestatustype)
- [WorkloadEstimateUpdateUsageErrorCodeType](./literals.md#workloadestimateupdateusageerrorcodetype)
- [BillingandCostManagementPricingCalculatorServiceName](./literals.md#billingandcostmanagementpricingcalculatorservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AddReservedInstanceActionTypeDef](./type_defs.md#addreservedinstanceactiontypedef)
- [AddSavingsPlanActionTypeDef](./type_defs.md#addsavingsplanactiontypedef)
- [BatchCreateBillScenarioCommitmentModificationErrorTypeDef](./type_defs.md#batchcreatebillscenariocommitmentmodificationerrortypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BatchCreateBillScenarioUsageModificationErrorTypeDef](./type_defs.md#batchcreatebillscenariousagemodificationerrortypedef)
- [UsageQuantityTypeDef](./type_defs.md#usagequantitytypedef)
- [BatchCreateWorkloadEstimateUsageErrorTypeDef](./type_defs.md#batchcreateworkloadestimateusageerrortypedef)
- [WorkloadEstimateUsageQuantityTypeDef](./type_defs.md#workloadestimateusagequantitytypedef)
- [BatchDeleteBillScenarioCommitmentModificationErrorTypeDef](./type_defs.md#batchdeletebillscenariocommitmentmodificationerrortypedef)
- [BatchDeleteBillScenarioCommitmentModificationRequestRequestTypeDef](./type_defs.md#batchdeletebillscenariocommitmentmodificationrequestrequesttypedef)
- [BatchDeleteBillScenarioUsageModificationErrorTypeDef](./type_defs.md#batchdeletebillscenariousagemodificationerrortypedef)
- [BatchDeleteBillScenarioUsageModificationRequestRequestTypeDef](./type_defs.md#batchdeletebillscenariousagemodificationrequestrequesttypedef)
- [BatchDeleteWorkloadEstimateUsageErrorTypeDef](./type_defs.md#batchdeleteworkloadestimateusageerrortypedef)
- [BatchDeleteWorkloadEstimateUsageRequestRequestTypeDef](./type_defs.md#batchdeleteworkloadestimateusagerequestrequesttypedef)
- [BatchUpdateBillScenarioCommitmentModificationEntryTypeDef](./type_defs.md#batchupdatebillscenariocommitmentmodificationentrytypedef)
- [BatchUpdateBillScenarioCommitmentModificationErrorTypeDef](./type_defs.md#batchupdatebillscenariocommitmentmodificationerrortypedef)
- [BatchUpdateBillScenarioUsageModificationErrorTypeDef](./type_defs.md#batchupdatebillscenariousagemodificationerrortypedef)
- [BatchUpdateWorkloadEstimateUsageEntryTypeDef](./type_defs.md#batchupdateworkloadestimateusageentrytypedef)
- [BatchUpdateWorkloadEstimateUsageErrorTypeDef](./type_defs.md#batchupdateworkloadestimateusageerrortypedef)
- [CostAmountTypeDef](./type_defs.md#costamounttypedef)
- [UsageQuantityResultTypeDef](./type_defs.md#usagequantityresulttypedef)
- [BillIntervalOutputTypeDef](./type_defs.md#billintervaloutputtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [NegateReservedInstanceActionTypeDef](./type_defs.md#negatereservedinstanceactiontypedef)
- [NegateSavingsPlanActionTypeDef](./type_defs.md#negatesavingsplanactiontypedef)
- [CreateBillEstimateRequestRequestTypeDef](./type_defs.md#createbillestimaterequestrequesttypedef)
- [CreateBillScenarioRequestRequestTypeDef](./type_defs.md#createbillscenariorequestrequesttypedef)
- [CreateWorkloadEstimateRequestRequestTypeDef](./type_defs.md#createworkloadestimaterequestrequesttypedef)
- [DeleteBillEstimateRequestRequestTypeDef](./type_defs.md#deletebillestimaterequestrequesttypedef)
- [DeleteBillScenarioRequestRequestTypeDef](./type_defs.md#deletebillscenariorequestrequesttypedef)
- [DeleteWorkloadEstimateRequestRequestTypeDef](./type_defs.md#deleteworkloadestimaterequestrequesttypedef)
- [ExpressionFilterOutputTypeDef](./type_defs.md#expressionfilteroutputtypedef)
- [ExpressionFilterTypeDef](./type_defs.md#expressionfiltertypedef)
- [GetBillEstimateRequestRequestTypeDef](./type_defs.md#getbillestimaterequestrequesttypedef)
- [GetBillScenarioRequestRequestTypeDef](./type_defs.md#getbillscenariorequestrequesttypedef)
- [GetWorkloadEstimateRequestRequestTypeDef](./type_defs.md#getworkloadestimaterequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListBillEstimateCommitmentsRequestRequestTypeDef](./type_defs.md#listbillestimatecommitmentsrequestrequesttypedef)
- [ListBillEstimateInputCommitmentModificationsRequestRequestTypeDef](./type_defs.md#listbillestimateinputcommitmentmodificationsrequestrequesttypedef)
- [ListUsageFilterTypeDef](./type_defs.md#listusagefiltertypedef)
- [ListBillEstimateLineItemsFilterTypeDef](./type_defs.md#listbillestimatelineitemsfiltertypedef)
- [ListBillEstimatesFilterTypeDef](./type_defs.md#listbillestimatesfiltertypedef)
- [ListBillScenarioCommitmentModificationsRequestRequestTypeDef](./type_defs.md#listbillscenariocommitmentmodificationsrequestrequesttypedef)
- [ListBillScenariosFilterTypeDef](./type_defs.md#listbillscenariosfiltertypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListWorkloadEstimatesFilterTypeDef](./type_defs.md#listworkloadestimatesfiltertypedef)
- [WorkloadEstimateSummaryTypeDef](./type_defs.md#workloadestimatesummarytypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdatePreferencesRequestRequestTypeDef](./type_defs.md#updatepreferencesrequestrequesttypedef)
- [CreateWorkloadEstimateResponseTypeDef](./type_defs.md#createworkloadestimateresponsetypedef)
- [GetPreferencesResponseTypeDef](./type_defs.md#getpreferencesresponsetypedef)
- [GetWorkloadEstimateResponseTypeDef](./type_defs.md#getworkloadestimateresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [UpdatePreferencesResponseTypeDef](./type_defs.md#updatepreferencesresponsetypedef)
- [UpdateWorkloadEstimateResponseTypeDef](./type_defs.md#updateworkloadestimateresponsetypedef)
- [BatchDeleteBillScenarioCommitmentModificationResponseTypeDef](./type_defs.md#batchdeletebillscenariocommitmentmodificationresponsetypedef)
- [BatchDeleteBillScenarioUsageModificationResponseTypeDef](./type_defs.md#batchdeletebillscenariousagemodificationresponsetypedef)
- [BatchDeleteWorkloadEstimateUsageResponseTypeDef](./type_defs.md#batchdeleteworkloadestimateusageresponsetypedef)
- [BatchUpdateBillScenarioCommitmentModificationRequestRequestTypeDef](./type_defs.md#batchupdatebillscenariocommitmentmodificationrequestrequesttypedef)
- [BatchUpdateWorkloadEstimateUsageRequestRequestTypeDef](./type_defs.md#batchupdateworkloadestimateusagerequestrequesttypedef)
- [BillEstimateCommitmentSummaryTypeDef](./type_defs.md#billestimatecommitmentsummarytypedef)
- [CostDifferenceTypeDef](./type_defs.md#costdifferencetypedef)
- [BillEstimateLineItemSummaryTypeDef](./type_defs.md#billestimatelineitemsummarytypedef)
- [BillEstimateSummaryTypeDef](./type_defs.md#billestimatesummarytypedef)
- [BillScenarioSummaryTypeDef](./type_defs.md#billscenariosummarytypedef)
- [CreateBillScenarioResponseTypeDef](./type_defs.md#createbillscenarioresponsetypedef)
- [GetBillScenarioResponseTypeDef](./type_defs.md#getbillscenarioresponsetypedef)
- [UpdateBillScenarioResponseTypeDef](./type_defs.md#updatebillscenarioresponsetypedef)
- [BillIntervalTypeDef](./type_defs.md#billintervaltypedef)
- [FilterTimestampTypeDef](./type_defs.md#filtertimestamptypedef)
- [UpdateBillEstimateRequestRequestTypeDef](./type_defs.md#updatebillestimaterequestrequesttypedef)
- [UpdateBillScenarioRequestRequestTypeDef](./type_defs.md#updatebillscenariorequestrequesttypedef)
- [UpdateWorkloadEstimateRequestRequestTypeDef](./type_defs.md#updateworkloadestimaterequestrequesttypedef)
- [UsageAmountTypeDef](./type_defs.md#usageamounttypedef)
- [BillScenarioCommitmentModificationActionTypeDef](./type_defs.md#billscenariocommitmentmodificationactiontypedef)
- [ExpressionOutputTypeDef](./type_defs.md#expressionoutputtypedef)
- [ExpressionPaginatorTypeDef](./type_defs.md#expressionpaginatortypedef)
- [ExpressionFilterUnionTypeDef](./type_defs.md#expressionfilteruniontypedef)
- [ListBillEstimateCommitmentsRequestPaginateTypeDef](./type_defs.md#listbillestimatecommitmentsrequestpaginatetypedef)
- [ListBillEstimateInputCommitmentModificationsRequestPaginateTypeDef](./type_defs.md#listbillestimateinputcommitmentmodificationsrequestpaginatetypedef)
- [ListBillScenarioCommitmentModificationsRequestPaginateTypeDef](./type_defs.md#listbillscenariocommitmentmodificationsrequestpaginatetypedef)
- [ListBillEstimateInputUsageModificationsRequestPaginateTypeDef](./type_defs.md#listbillestimateinputusagemodificationsrequestpaginatetypedef)
- [ListBillEstimateInputUsageModificationsRequestRequestTypeDef](./type_defs.md#listbillestimateinputusagemodificationsrequestrequesttypedef)
- [ListBillScenarioUsageModificationsRequestPaginateTypeDef](./type_defs.md#listbillscenariousagemodificationsrequestpaginatetypedef)
- [ListBillScenarioUsageModificationsRequestRequestTypeDef](./type_defs.md#listbillscenariousagemodificationsrequestrequesttypedef)
- [ListWorkloadEstimateUsageRequestPaginateTypeDef](./type_defs.md#listworkloadestimateusagerequestpaginatetypedef)
- [ListWorkloadEstimateUsageRequestRequestTypeDef](./type_defs.md#listworkloadestimateusagerequestrequesttypedef)
- [ListBillEstimateLineItemsRequestPaginateTypeDef](./type_defs.md#listbillestimatelineitemsrequestpaginatetypedef)
- [ListBillEstimateLineItemsRequestRequestTypeDef](./type_defs.md#listbillestimatelineitemsrequestrequesttypedef)
- [ListWorkloadEstimatesResponseTypeDef](./type_defs.md#listworkloadestimatesresponsetypedef)
- [ListBillEstimateCommitmentsResponseTypeDef](./type_defs.md#listbillestimatecommitmentsresponsetypedef)
- [BillEstimateCostSummaryTypeDef](./type_defs.md#billestimatecostsummarytypedef)
- [ListBillEstimateLineItemsResponseTypeDef](./type_defs.md#listbillestimatelineitemsresponsetypedef)
- [ListBillEstimatesResponseTypeDef](./type_defs.md#listbillestimatesresponsetypedef)
- [ListBillScenariosResponseTypeDef](./type_defs.md#listbillscenariosresponsetypedef)
- [BillIntervalUnionTypeDef](./type_defs.md#billintervaluniontypedef)
- [ListBillEstimatesRequestPaginateTypeDef](./type_defs.md#listbillestimatesrequestpaginatetypedef)
- [ListBillEstimatesRequestRequestTypeDef](./type_defs.md#listbillestimatesrequestrequesttypedef)
- [ListBillScenariosRequestPaginateTypeDef](./type_defs.md#listbillscenariosrequestpaginatetypedef)
- [ListBillScenariosRequestRequestTypeDef](./type_defs.md#listbillscenariosrequestrequesttypedef)
- [ListWorkloadEstimatesRequestPaginateTypeDef](./type_defs.md#listworkloadestimatesrequestpaginatetypedef)
- [ListWorkloadEstimatesRequestRequestTypeDef](./type_defs.md#listworkloadestimatesrequestrequesttypedef)
- [BatchUpdateBillScenarioUsageModificationEntryTypeDef](./type_defs.md#batchupdatebillscenariousagemodificationentrytypedef)
- [BatchCreateBillScenarioCommitmentModificationEntryTypeDef](./type_defs.md#batchcreatebillscenariocommitmentmodificationentrytypedef)
- [BatchCreateBillScenarioCommitmentModificationItemTypeDef](./type_defs.md#batchcreatebillscenariocommitmentmodificationitemtypedef)
- [BillEstimateInputCommitmentModificationSummaryTypeDef](./type_defs.md#billestimateinputcommitmentmodificationsummarytypedef)
- [BillScenarioCommitmentModificationItemTypeDef](./type_defs.md#billscenariocommitmentmodificationitemtypedef)
- [HistoricalUsageEntityOutputTypeDef](./type_defs.md#historicalusageentityoutputtypedef)
- [HistoricalUsageEntityPaginatorTypeDef](./type_defs.md#historicalusageentitypaginatortypedef)
- [ExpressionTypeDef](./type_defs.md#expressiontypedef)
- [CreateBillEstimateResponseTypeDef](./type_defs.md#createbillestimateresponsetypedef)
- [GetBillEstimateResponseTypeDef](./type_defs.md#getbillestimateresponsetypedef)
- [UpdateBillEstimateResponseTypeDef](./type_defs.md#updatebillestimateresponsetypedef)
- [BatchUpdateBillScenarioUsageModificationRequestRequestTypeDef](./type_defs.md#batchupdatebillscenariousagemodificationrequestrequesttypedef)
- [BatchCreateBillScenarioCommitmentModificationRequestRequestTypeDef](./type_defs.md#batchcreatebillscenariocommitmentmodificationrequestrequesttypedef)
- [BatchCreateBillScenarioCommitmentModificationResponseTypeDef](./type_defs.md#batchcreatebillscenariocommitmentmodificationresponsetypedef)
- [ListBillEstimateInputCommitmentModificationsResponseTypeDef](./type_defs.md#listbillestimateinputcommitmentmodificationsresponsetypedef)
- [BatchUpdateBillScenarioCommitmentModificationResponseTypeDef](./type_defs.md#batchupdatebillscenariocommitmentmodificationresponsetypedef)
- [ListBillScenarioCommitmentModificationsResponseTypeDef](./type_defs.md#listbillscenariocommitmentmodificationsresponsetypedef)
- [BatchCreateBillScenarioUsageModificationItemTypeDef](./type_defs.md#batchcreatebillscenariousagemodificationitemtypedef)
- [BatchCreateWorkloadEstimateUsageItemTypeDef](./type_defs.md#batchcreateworkloadestimateusageitemtypedef)
- [BillEstimateInputUsageModificationSummaryTypeDef](./type_defs.md#billestimateinputusagemodificationsummarytypedef)
- [BillScenarioUsageModificationItemTypeDef](./type_defs.md#billscenariousagemodificationitemtypedef)
- [WorkloadEstimateUsageItemTypeDef](./type_defs.md#workloadestimateusageitemtypedef)
- [BillEstimateInputUsageModificationSummaryPaginatorTypeDef](./type_defs.md#billestimateinputusagemodificationsummarypaginatortypedef)
- [BillScenarioUsageModificationItemPaginatorTypeDef](./type_defs.md#billscenariousagemodificationitempaginatortypedef)
- [WorkloadEstimateUsageItemPaginatorTypeDef](./type_defs.md#workloadestimateusageitempaginatortypedef)
- [ExpressionUnionTypeDef](./type_defs.md#expressionuniontypedef)
- [BatchCreateBillScenarioUsageModificationResponseTypeDef](./type_defs.md#batchcreatebillscenariousagemodificationresponsetypedef)
- [BatchCreateWorkloadEstimateUsageResponseTypeDef](./type_defs.md#batchcreateworkloadestimateusageresponsetypedef)
- [ListBillEstimateInputUsageModificationsResponseTypeDef](./type_defs.md#listbillestimateinputusagemodificationsresponsetypedef)
- [BatchUpdateBillScenarioUsageModificationResponseTypeDef](./type_defs.md#batchupdatebillscenariousagemodificationresponsetypedef)
- [ListBillScenarioUsageModificationsResponseTypeDef](./type_defs.md#listbillscenariousagemodificationsresponsetypedef)
- [BatchUpdateWorkloadEstimateUsageResponseTypeDef](./type_defs.md#batchupdateworkloadestimateusageresponsetypedef)
- [ListWorkloadEstimateUsageResponseTypeDef](./type_defs.md#listworkloadestimateusageresponsetypedef)
- [ListBillEstimateInputUsageModificationsResponsePaginatorTypeDef](./type_defs.md#listbillestimateinputusagemodificationsresponsepaginatortypedef)
- [ListBillScenarioUsageModificationsResponsePaginatorTypeDef](./type_defs.md#listbillscenariousagemodificationsresponsepaginatortypedef)
- [ListWorkloadEstimateUsageResponsePaginatorTypeDef](./type_defs.md#listworkloadestimateusageresponsepaginatortypedef)
- [HistoricalUsageEntityTypeDef](./type_defs.md#historicalusageentitytypedef)
- [HistoricalUsageEntityUnionTypeDef](./type_defs.md#historicalusageentityuniontypedef)
- [BatchCreateBillScenarioUsageModificationEntryTypeDef](./type_defs.md#batchcreatebillscenariousagemodificationentrytypedef)
- [BatchCreateWorkloadEstimateUsageEntryTypeDef](./type_defs.md#batchcreateworkloadestimateusageentrytypedef)
- [BatchCreateBillScenarioUsageModificationRequestRequestTypeDef](./type_defs.md#batchcreatebillscenariousagemodificationrequestrequesttypedef)
- [BatchCreateWorkloadEstimateUsageRequestRequestTypeDef](./type_defs.md#batchcreateworkloadestimateusagerequestrequesttypedef)

