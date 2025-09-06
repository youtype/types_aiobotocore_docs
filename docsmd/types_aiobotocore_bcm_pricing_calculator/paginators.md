# Paginators

> [Index](../README.md) > [BillingandCostManagementPricingCalculator](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [BillingandCostManagementPricingCalculator](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-pricing-calculator.html#billingandcostmanagementpricingcalculator)
    type annotations stubs module [types-aiobotocore-bcm-pricing-calculator](https://pypi.org/project/types-aiobotocore-bcm-pricing-calculator/).

## ListBillEstimateCommitmentsPaginator

Type annotations and code completion for `#!python session.create_client("bcm-pricing-calculator").get_paginator("list_bill_estimate_commitments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-pricing-calculator/paginator/ListBillEstimateCommitments.html#BillingandCostManagementPricingCalculator.Paginator.ListBillEstimateCommitments)

```python
# ListBillEstimateCommitmentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bcm_pricing_calculator.paginator import ListBillEstimateCommitmentsPaginator

session = get_session()
async with session.create_client("bcm-pricing-calculator") as client:  # (1)
    paginator: ListBillEstimateCommitmentsPaginator = client.get_paginator("list_bill_estimate_commitments")  # (2)
    async for item in paginator.paginate(...):
        item: ListBillEstimateCommitmentsResponseTypeDef
        print(item)  # (3)
```

1. client: [BillingandCostManagementPricingCalculatorClient](./client.md)
2. paginator: [ListBillEstimateCommitmentsPaginator](./paginators.md#listbillestimatecommitmentspaginator)
3. item: `AioPageIterator[ListBillEstimateCommitmentsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBillEstimateCommitmentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    billEstimateId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListBillEstimateCommitmentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListBillEstimateCommitmentsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBillEstimateCommitmentsRequestPaginateTypeDef = {  # (1)
    "billEstimateId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBillEstimateCommitmentsRequestPaginateTypeDef](./type_defs.md#listbillestimatecommitmentsrequestpaginatetypedef)
## ListBillEstimateInputCommitmentModificationsPaginator

Type annotations and code completion for `#!python session.create_client("bcm-pricing-calculator").get_paginator("list_bill_estimate_input_commitment_modifications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-pricing-calculator/paginator/ListBillEstimateInputCommitmentModifications.html#BillingandCostManagementPricingCalculator.Paginator.ListBillEstimateInputCommitmentModifications)

```python
# ListBillEstimateInputCommitmentModificationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bcm_pricing_calculator.paginator import ListBillEstimateInputCommitmentModificationsPaginator

session = get_session()
async with session.create_client("bcm-pricing-calculator") as client:  # (1)
    paginator: ListBillEstimateInputCommitmentModificationsPaginator = client.get_paginator("list_bill_estimate_input_commitment_modifications")  # (2)
    async for item in paginator.paginate(...):
        item: ListBillEstimateInputCommitmentModificationsResponseTypeDef
        print(item)  # (3)
```

1. client: [BillingandCostManagementPricingCalculatorClient](./client.md)
2. paginator: [ListBillEstimateInputCommitmentModificationsPaginator](./paginators.md#listbillestimateinputcommitmentmodificationspaginator)
3. item: `AioPageIterator[ListBillEstimateInputCommitmentModificationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBillEstimateInputCommitmentModificationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    billEstimateId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListBillEstimateInputCommitmentModificationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListBillEstimateInputCommitmentModificationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBillEstimateInputCommitmentModificationsRequestPaginateTypeDef = {  # (1)
    "billEstimateId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBillEstimateInputCommitmentModificationsRequestPaginateTypeDef](./type_defs.md#listbillestimateinputcommitmentmodificationsrequestpaginatetypedef)
## ListBillEstimateInputUsageModificationsPaginator

Type annotations and code completion for `#!python session.create_client("bcm-pricing-calculator").get_paginator("list_bill_estimate_input_usage_modifications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-pricing-calculator/paginator/ListBillEstimateInputUsageModifications.html#BillingandCostManagementPricingCalculator.Paginator.ListBillEstimateInputUsageModifications)

```python
# ListBillEstimateInputUsageModificationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bcm_pricing_calculator.paginator import ListBillEstimateInputUsageModificationsPaginator

session = get_session()
async with session.create_client("bcm-pricing-calculator") as client:  # (1)
    paginator: ListBillEstimateInputUsageModificationsPaginator = client.get_paginator("list_bill_estimate_input_usage_modifications")  # (2)
    async for item in paginator.paginate(...):
        item: ListBillEstimateInputUsageModificationsResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [BillingandCostManagementPricingCalculatorClient](./client.md)
2. paginator: [ListBillEstimateInputUsageModificationsPaginator](./paginators.md#listbillestimateinputusagemodificationspaginator)
3. item: `AioPageIterator[ListBillEstimateInputUsageModificationsResponsePaginatorTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBillEstimateInputUsageModificationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    billEstimateId: str,
    filters: Sequence[ListUsageFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListBillEstimateInputUsageModificationsResponsePaginatorTypeDef]:  # (3)
    ...
```

1. See `Sequence[ListUsageFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListBillEstimateInputUsageModificationsResponsePaginatorTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBillEstimateInputUsageModificationsRequestPaginateTypeDef = {  # (1)
    "billEstimateId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBillEstimateInputUsageModificationsRequestPaginateTypeDef](./type_defs.md#listbillestimateinputusagemodificationsrequestpaginatetypedef)
## ListBillEstimateLineItemsPaginator

Type annotations and code completion for `#!python session.create_client("bcm-pricing-calculator").get_paginator("list_bill_estimate_line_items")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-pricing-calculator/paginator/ListBillEstimateLineItems.html#BillingandCostManagementPricingCalculator.Paginator.ListBillEstimateLineItems)

```python
# ListBillEstimateLineItemsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bcm_pricing_calculator.paginator import ListBillEstimateLineItemsPaginator

session = get_session()
async with session.create_client("bcm-pricing-calculator") as client:  # (1)
    paginator: ListBillEstimateLineItemsPaginator = client.get_paginator("list_bill_estimate_line_items")  # (2)
    async for item in paginator.paginate(...):
        item: ListBillEstimateLineItemsResponseTypeDef
        print(item)  # (3)
```

1. client: [BillingandCostManagementPricingCalculatorClient](./client.md)
2. paginator: [ListBillEstimateLineItemsPaginator](./paginators.md#listbillestimatelineitemspaginator)
3. item: `AioPageIterator[ListBillEstimateLineItemsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBillEstimateLineItemsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    billEstimateId: str,
    filters: Sequence[ListBillEstimateLineItemsFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListBillEstimateLineItemsResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[ListBillEstimateLineItemsFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListBillEstimateLineItemsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBillEstimateLineItemsRequestPaginateTypeDef = {  # (1)
    "billEstimateId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBillEstimateLineItemsRequestPaginateTypeDef](./type_defs.md#listbillestimatelineitemsrequestpaginatetypedef)
## ListBillEstimatesPaginator

Type annotations and code completion for `#!python session.create_client("bcm-pricing-calculator").get_paginator("list_bill_estimates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-pricing-calculator/paginator/ListBillEstimates.html#BillingandCostManagementPricingCalculator.Paginator.ListBillEstimates)

```python
# ListBillEstimatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bcm_pricing_calculator.paginator import ListBillEstimatesPaginator

session = get_session()
async with session.create_client("bcm-pricing-calculator") as client:  # (1)
    paginator: ListBillEstimatesPaginator = client.get_paginator("list_bill_estimates")  # (2)
    async for item in paginator.paginate(...):
        item: ListBillEstimatesResponseTypeDef
        print(item)  # (3)
```

1. client: [BillingandCostManagementPricingCalculatorClient](./client.md)
2. paginator: [ListBillEstimatesPaginator](./paginators.md#listbillestimatespaginator)
3. item: `AioPageIterator[ListBillEstimatesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBillEstimatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Sequence[ListBillEstimatesFilterTypeDef] = ...,  # (1)
    createdAtFilter: FilterTimestampTypeDef = ...,  # (2)
    expiresAtFilter: FilterTimestampTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[ListBillEstimatesResponseTypeDef]:  # (5)
    ...
```

1. See `Sequence[ListBillEstimatesFilterTypeDef]`
2. See [:material-code-braces: FilterTimestampTypeDef](./type_defs.md#filtertimestamptypedef)
3. See [:material-code-braces: FilterTimestampTypeDef](./type_defs.md#filtertimestamptypedef)
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[ListBillEstimatesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBillEstimatesRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBillEstimatesRequestPaginateTypeDef](./type_defs.md#listbillestimatesrequestpaginatetypedef)
## ListBillScenarioCommitmentModificationsPaginator

Type annotations and code completion for `#!python session.create_client("bcm-pricing-calculator").get_paginator("list_bill_scenario_commitment_modifications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-pricing-calculator/paginator/ListBillScenarioCommitmentModifications.html#BillingandCostManagementPricingCalculator.Paginator.ListBillScenarioCommitmentModifications)

```python
# ListBillScenarioCommitmentModificationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bcm_pricing_calculator.paginator import ListBillScenarioCommitmentModificationsPaginator

session = get_session()
async with session.create_client("bcm-pricing-calculator") as client:  # (1)
    paginator: ListBillScenarioCommitmentModificationsPaginator = client.get_paginator("list_bill_scenario_commitment_modifications")  # (2)
    async for item in paginator.paginate(...):
        item: ListBillScenarioCommitmentModificationsResponseTypeDef
        print(item)  # (3)
```

1. client: [BillingandCostManagementPricingCalculatorClient](./client.md)
2. paginator: [ListBillScenarioCommitmentModificationsPaginator](./paginators.md#listbillscenariocommitmentmodificationspaginator)
3. item: `AioPageIterator[ListBillScenarioCommitmentModificationsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBillScenarioCommitmentModificationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    billScenarioId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListBillScenarioCommitmentModificationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListBillScenarioCommitmentModificationsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBillScenarioCommitmentModificationsRequestPaginateTypeDef = {  # (1)
    "billScenarioId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBillScenarioCommitmentModificationsRequestPaginateTypeDef](./type_defs.md#listbillscenariocommitmentmodificationsrequestpaginatetypedef)
## ListBillScenarioUsageModificationsPaginator

Type annotations and code completion for `#!python session.create_client("bcm-pricing-calculator").get_paginator("list_bill_scenario_usage_modifications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-pricing-calculator/paginator/ListBillScenarioUsageModifications.html#BillingandCostManagementPricingCalculator.Paginator.ListBillScenarioUsageModifications)

```python
# ListBillScenarioUsageModificationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bcm_pricing_calculator.paginator import ListBillScenarioUsageModificationsPaginator

session = get_session()
async with session.create_client("bcm-pricing-calculator") as client:  # (1)
    paginator: ListBillScenarioUsageModificationsPaginator = client.get_paginator("list_bill_scenario_usage_modifications")  # (2)
    async for item in paginator.paginate(...):
        item: ListBillScenarioUsageModificationsResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [BillingandCostManagementPricingCalculatorClient](./client.md)
2. paginator: [ListBillScenarioUsageModificationsPaginator](./paginators.md#listbillscenariousagemodificationspaginator)
3. item: `AioPageIterator[ListBillScenarioUsageModificationsResponsePaginatorTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBillScenarioUsageModificationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    billScenarioId: str,
    filters: Sequence[ListUsageFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListBillScenarioUsageModificationsResponsePaginatorTypeDef]:  # (3)
    ...
```

1. See `Sequence[ListUsageFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListBillScenarioUsageModificationsResponsePaginatorTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBillScenarioUsageModificationsRequestPaginateTypeDef = {  # (1)
    "billScenarioId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBillScenarioUsageModificationsRequestPaginateTypeDef](./type_defs.md#listbillscenariousagemodificationsrequestpaginatetypedef)
## ListBillScenariosPaginator

Type annotations and code completion for `#!python session.create_client("bcm-pricing-calculator").get_paginator("list_bill_scenarios")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-pricing-calculator/paginator/ListBillScenarios.html#BillingandCostManagementPricingCalculator.Paginator.ListBillScenarios)

```python
# ListBillScenariosPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bcm_pricing_calculator.paginator import ListBillScenariosPaginator

session = get_session()
async with session.create_client("bcm-pricing-calculator") as client:  # (1)
    paginator: ListBillScenariosPaginator = client.get_paginator("list_bill_scenarios")  # (2)
    async for item in paginator.paginate(...):
        item: ListBillScenariosResponseTypeDef
        print(item)  # (3)
```

1. client: [BillingandCostManagementPricingCalculatorClient](./client.md)
2. paginator: [ListBillScenariosPaginator](./paginators.md#listbillscenariospaginator)
3. item: `AioPageIterator[ListBillScenariosResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBillScenariosPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Sequence[ListBillScenariosFilterTypeDef] = ...,  # (1)
    createdAtFilter: FilterTimestampTypeDef = ...,  # (2)
    expiresAtFilter: FilterTimestampTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[ListBillScenariosResponseTypeDef]:  # (5)
    ...
```

1. See `Sequence[ListBillScenariosFilterTypeDef]`
2. See [:material-code-braces: FilterTimestampTypeDef](./type_defs.md#filtertimestamptypedef)
3. See [:material-code-braces: FilterTimestampTypeDef](./type_defs.md#filtertimestamptypedef)
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[ListBillScenariosResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBillScenariosRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBillScenariosRequestPaginateTypeDef](./type_defs.md#listbillscenariosrequestpaginatetypedef)
## ListWorkloadEstimateUsagePaginator

Type annotations and code completion for `#!python session.create_client("bcm-pricing-calculator").get_paginator("list_workload_estimate_usage")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-pricing-calculator/paginator/ListWorkloadEstimateUsage.html#BillingandCostManagementPricingCalculator.Paginator.ListWorkloadEstimateUsage)

```python
# ListWorkloadEstimateUsagePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bcm_pricing_calculator.paginator import ListWorkloadEstimateUsagePaginator

session = get_session()
async with session.create_client("bcm-pricing-calculator") as client:  # (1)
    paginator: ListWorkloadEstimateUsagePaginator = client.get_paginator("list_workload_estimate_usage")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkloadEstimateUsageResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [BillingandCostManagementPricingCalculatorClient](./client.md)
2. paginator: [ListWorkloadEstimateUsagePaginator](./paginators.md#listworkloadestimateusagepaginator)
3. item: `AioPageIterator[ListWorkloadEstimateUsageResponsePaginatorTypeDef]`


### paginate

Type annotations and code completion for `#!python ListWorkloadEstimateUsagePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    workloadEstimateId: str,
    filters: Sequence[ListUsageFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListWorkloadEstimateUsageResponsePaginatorTypeDef]:  # (3)
    ...
```

1. See `Sequence[ListUsageFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListWorkloadEstimateUsageResponsePaginatorTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkloadEstimateUsageRequestPaginateTypeDef = {  # (1)
    "workloadEstimateId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkloadEstimateUsageRequestPaginateTypeDef](./type_defs.md#listworkloadestimateusagerequestpaginatetypedef)
## ListWorkloadEstimatesPaginator

Type annotations and code completion for `#!python session.create_client("bcm-pricing-calculator").get_paginator("list_workload_estimates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-pricing-calculator/paginator/ListWorkloadEstimates.html#BillingandCostManagementPricingCalculator.Paginator.ListWorkloadEstimates)

```python
# ListWorkloadEstimatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_bcm_pricing_calculator.paginator import ListWorkloadEstimatesPaginator

session = get_session()
async with session.create_client("bcm-pricing-calculator") as client:  # (1)
    paginator: ListWorkloadEstimatesPaginator = client.get_paginator("list_workload_estimates")  # (2)
    async for item in paginator.paginate(...):
        item: ListWorkloadEstimatesResponseTypeDef
        print(item)  # (3)
```

1. client: [BillingandCostManagementPricingCalculatorClient](./client.md)
2. paginator: [ListWorkloadEstimatesPaginator](./paginators.md#listworkloadestimatespaginator)
3. item: `AioPageIterator[ListWorkloadEstimatesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListWorkloadEstimatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    createdAtFilter: FilterTimestampTypeDef = ...,  # (1)
    expiresAtFilter: FilterTimestampTypeDef = ...,  # (1)
    filters: Sequence[ListWorkloadEstimatesFilterTypeDef] = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[ListWorkloadEstimatesResponseTypeDef]:  # (5)
    ...
```

1. See [:material-code-braces: FilterTimestampTypeDef](./type_defs.md#filtertimestamptypedef)
2. See [:material-code-braces: FilterTimestampTypeDef](./type_defs.md#filtertimestamptypedef)
3. See `Sequence[ListWorkloadEstimatesFilterTypeDef]`
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[ListWorkloadEstimatesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListWorkloadEstimatesRequestPaginateTypeDef = {  # (1)
    "createdAtFilter": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListWorkloadEstimatesRequestPaginateTypeDef](./type_defs.md#listworkloadestimatesrequestpaginatetypedef)
