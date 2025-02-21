# Examples

> [Index](../README.md) > [BillingandCostManagementPricingCalculator](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [BillingandCostManagementPricingCalculator](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-pricing-calculator.html#billingandcostmanagementpricingcalculator)
    type annotations stubs module [types-aiobotocore-bcm-pricing-calculator](https://pypi.org/project/types-aiobotocore-bcm-pricing-calculator/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[bcm-pricing-calculator]` package installed.

Write your `BillingandCostManagementPricingCalculator` code as usual,
type checking and code completion should work out of the box.



```python
# BillingandCostManagementPricingCalculatorClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("bcm-pricing-calculator") as client:  # (1)
    result = await client.batch_create_bill_scenario_commitment_modification()  # (2)
```

1. client: [BillingandCostManagementPricingCalculatorClient](./client.md)
2. result: [:material-code-braces: BatchCreateBillScenarioCommitmentModificationResponseTypeDef](./type_defs.md#batchcreatebillscenariocommitmentmodificationresponsetypedef) 



```python
# ListBillEstimateCommitmentsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("bcm-pricing-calculator") as client:  # (1)
    paginator = client.get_paginator("list_bill_estimate_commitments")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [BillingandCostManagementPricingCalculatorClient](./client.md)
2. paginator: [ListBillEstimateCommitmentsPaginator](./paginators.md#listbillestimatecommitmentspaginator)
3. item: [:material-code-braces: ListBillEstimateCommitmentsResponseTypeDef](./type_defs.md#listbillestimatecommitmentsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[bcm-pricing-calculator]`
or a standalone `types_aiobotocore_bcm_pricing_calculator` package, you have to explicitly specify
`client: BillingandCostManagementPricingCalculatorClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# BillingandCostManagementPricingCalculatorClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_bcm_pricing_calculator.client import BillingandCostManagementPricingCalculatorClient
from types_aiobotocore_bcm_pricing_calculator.type_defs import BatchCreateBillScenarioCommitmentModificationResponseTypeDef
from types_aiobotocore_bcm_pricing_calculator.type_defs import BatchCreateBillScenarioCommitmentModificationRequestTypeDef


session = get_session()

async with session.create_client("bcm-pricing-calculator") as client:
    client: BillingandCostManagementPricingCalculatorClient
    kwargs: BatchCreateBillScenarioCommitmentModificationRequestTypeDef = {...}
    result: BatchCreateBillScenarioCommitmentModificationResponseTypeDef = await client.batch_create_bill_scenario_commitment_modification(**kwargs)
```



```python
# ListBillEstimateCommitmentsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_bcm_pricing_calculator.client import BillingandCostManagementPricingCalculatorClient
from types_aiobotocore_bcm_pricing_calculator.paginator import ListBillEstimateCommitmentsPaginator
from types_aiobotocore_bcm_pricing_calculator.type_defs import ListBillEstimateCommitmentsResponseTypeDef


session = get_session()

async with session.create_client("bcm-pricing-calculator") as client:
    client: BillingandCostManagementPricingCalculatorClient
    paginator: ListBillEstimateCommitmentsPaginator = client.get_paginator("list_bill_estimate_commitments")
    async for item in paginator.paginate(...):
        item: ListBillEstimateCommitmentsResponseTypeDef
        print(item)
```


