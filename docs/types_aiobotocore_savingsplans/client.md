<a id="savingsplansclient-for-aiobotocore-savingsplans-module"></a>

# SavingsPlansClient for aiobotocore SavingsPlans module

> [Index](../README.md) > [SavingsPlans](./README.md) > SavingsPlansClient

Auto-generated documentation for
[SavingsPlans](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans)
type annotations stubs module
[types-aiobotocore-savingsplans](https://pypi.org/project/types-aiobotocore-savingsplans/).

- [SavingsPlansClient for aiobotocore SavingsPlans module](#savingsplansclient-for-aiobotocore-savingsplans-module)
  - [SavingsPlansClient](#savingsplansclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_savings_plan](#create_savings_plan)
    - [delete_queued_savings_plan](#delete_queued_savings_plan)
    - [describe_savings_plan_rates](#describe_savings_plan_rates)
    - [describe_savings_plans](#describe_savings_plans)
    - [describe_savings_plans_offering_rates](#describe_savings_plans_offering_rates)
    - [describe_savings_plans_offerings](#describe_savings_plans_offerings)
    - [generate_presigned_url](#generate_presigned_url)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)

<a id="savingsplansclient"></a>

## SavingsPlansClient

Type annotations for `session.create_client("savingsplans")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_savingsplans.client import SavingsPlansClient

session = get_session()
async with session.create_client("savingsplans") as client:
    client: SavingsPlansClient
```

Boto3 documentation:
[SavingsPlans.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_savingsplans.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.InternalServerException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ServiceQuotaExceededException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

SavingsPlansClient exceptions.

Type annotations for `session.create_client("savingsplans").exceptions` method.

Boto3 documentation:
[SavingsPlans.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("savingsplans").can_paginate`
method.

Boto3 documentation:
[SavingsPlans.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create\_savings\_plan"></a>

### create_savings_plan

Creates a Savings Plan.

Type annotations for
`session.create_client("savingsplans").create_savings_plan` method.

Boto3 documentation:
[SavingsPlans.Client.create_savings_plan](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans.Client.create_savings_plan)

Asynchronous method. Use `await create_savings_plan(...)` for a synchronous
call.

Arguments mapping described in
[CreateSavingsPlanRequestRequestTypeDef](./type_defs.md#createsavingsplanrequestrequesttypedef).

Keyword-only arguments:

- `savingsPlanOfferingId`: `str` *(required)*
- `commitment`: `str` *(required)*
- `upfrontPaymentAmount`: `str`
- `purchaseTime`: `Union`\[`datetime`, `str`\]
- `clientToken`: `str`
- `tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateSavingsPlanResponseTypeDef](./type_defs.md#createsavingsplanresponsetypedef).

<a id="delete\_queued\_savings\_plan"></a>

### delete_queued_savings_plan

Deletes the queued purchase for the specified Savings Plan.

Type annotations for
`session.create_client("savingsplans").delete_queued_savings_plan` method.

Boto3 documentation:
[SavingsPlans.Client.delete_queued_savings_plan](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans.Client.delete_queued_savings_plan)

Asynchronous method. Use `await delete_queued_savings_plan(...)` for a
synchronous call.

Arguments mapping described in
[DeleteQueuedSavingsPlanRequestRequestTypeDef](./type_defs.md#deletequeuedsavingsplanrequestrequesttypedef).

Keyword-only arguments:

- `savingsPlanId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="describe\_savings\_plan\_rates"></a>

### describe_savings_plan_rates

Describes the specified Savings Plans rates.

Type annotations for
`session.create_client("savingsplans").describe_savings_plan_rates` method.

Boto3 documentation:
[SavingsPlans.Client.describe_savings_plan_rates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans.Client.describe_savings_plan_rates)

Asynchronous method. Use `await describe_savings_plan_rates(...)` for a
synchronous call.

Arguments mapping described in
[DescribeSavingsPlanRatesRequestRequestTypeDef](./type_defs.md#describesavingsplanratesrequestrequesttypedef).

Keyword-only arguments:

- `savingsPlanId`: `str` *(required)*
- `filters`:
  `Sequence`\[[SavingsPlanRateFilterTypeDef](./type_defs.md#savingsplanratefiltertypedef)\]
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[DescribeSavingsPlanRatesResponseTypeDef](./type_defs.md#describesavingsplanratesresponsetypedef).

<a id="describe\_savings\_plans"></a>

### describe_savings_plans

Describes the specified Savings Plans.

Type annotations for
`session.create_client("savingsplans").describe_savings_plans` method.

Boto3 documentation:
[SavingsPlans.Client.describe_savings_plans](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans.Client.describe_savings_plans)

Asynchronous method. Use `await describe_savings_plans(...)` for a synchronous
call.

Arguments mapping described in
[DescribeSavingsPlansRequestRequestTypeDef](./type_defs.md#describesavingsplansrequestrequesttypedef).

Keyword-only arguments:

- `savingsPlanArns`: `Sequence`\[`str`\]
- `savingsPlanIds`: `Sequence`\[`str`\]
- `nextToken`: `str`
- `maxResults`: `int`
- `states`:
  `Sequence`\[[SavingsPlanStateType](./literals.md#savingsplanstatetype)\]
- `filters`:
  `Sequence`\[[SavingsPlanFilterTypeDef](./type_defs.md#savingsplanfiltertypedef)\]

Returns a `Coroutine` for
[DescribeSavingsPlansResponseTypeDef](./type_defs.md#describesavingsplansresponsetypedef).

<a id="describe\_savings\_plans\_offering\_rates"></a>

### describe_savings_plans_offering_rates

Describes the specified Savings Plans offering rates.

Type annotations for
`session.create_client("savingsplans").describe_savings_plans_offering_rates`
method.

Boto3 documentation:
[SavingsPlans.Client.describe_savings_plans_offering_rates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans.Client.describe_savings_plans_offering_rates)

Asynchronous method. Use `await describe_savings_plans_offering_rates(...)` for
a synchronous call.

Arguments mapping described in
[DescribeSavingsPlansOfferingRatesRequestRequestTypeDef](./type_defs.md#describesavingsplansofferingratesrequestrequesttypedef).

Keyword-only arguments:

- `savingsPlanOfferingIds`: `Sequence`\[`str`\]
- `savingsPlanPaymentOptions`:
  `Sequence`\[[SavingsPlanPaymentOptionType](./literals.md#savingsplanpaymentoptiontype)\]
- `savingsPlanTypes`:
  `Sequence`\[[SavingsPlanTypeType](./literals.md#savingsplantypetype)\]
- `products`:
  `Sequence`\[[SavingsPlanProductTypeType](./literals.md#savingsplanproducttypetype)\]
- `serviceCodes`:
  `Sequence`\[[SavingsPlanRateServiceCodeType](./literals.md#savingsplanrateservicecodetype)\]
- `usageTypes`: `Sequence`\[`str`\]
- `operations`: `Sequence`\[`str`\]
- `filters`:
  `Sequence`\[[SavingsPlanOfferingRateFilterElementTypeDef](./type_defs.md#savingsplanofferingratefilterelementtypedef)\]
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[DescribeSavingsPlansOfferingRatesResponseTypeDef](./type_defs.md#describesavingsplansofferingratesresponsetypedef).

<a id="describe\_savings\_plans\_offerings"></a>

### describe_savings_plans_offerings

Describes the specified Savings Plans offerings.

Type annotations for
`session.create_client("savingsplans").describe_savings_plans_offerings`
method.

Boto3 documentation:
[SavingsPlans.Client.describe_savings_plans_offerings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans.Client.describe_savings_plans_offerings)

Asynchronous method. Use `await describe_savings_plans_offerings(...)` for a
synchronous call.

Arguments mapping described in
[DescribeSavingsPlansOfferingsRequestRequestTypeDef](./type_defs.md#describesavingsplansofferingsrequestrequesttypedef).

Keyword-only arguments:

- `offeringIds`: `Sequence`\[`str`\]
- `paymentOptions`:
  `Sequence`\[[SavingsPlanPaymentOptionType](./literals.md#savingsplanpaymentoptiontype)\]
- `productType`:
  [SavingsPlanProductTypeType](./literals.md#savingsplanproducttypetype)
- `planTypes`:
  `Sequence`\[[SavingsPlanTypeType](./literals.md#savingsplantypetype)\]
- `durations`: `Sequence`\[`int`\]
- `currencies`:
  `Sequence`\[[CurrencyCodeType](./literals.md#currencycodetype)\]
- `descriptions`: `Sequence`\[`str`\]
- `serviceCodes`: `Sequence`\[`str`\]
- `usageTypes`: `Sequence`\[`str`\]
- `operations`: `Sequence`\[`str`\]
- `filters`:
  `Sequence`\[[SavingsPlanOfferingFilterElementTypeDef](./type_defs.md#savingsplanofferingfilterelementtypedef)\]
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[DescribeSavingsPlansOfferingsResponseTypeDef](./type_defs.md#describesavingsplansofferingsresponsetypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("savingsplans").generate_presigned_url` method.

Boto3 documentation:
[SavingsPlans.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="list\_tags\_for\_resource"></a>

### list_tags_for_resource

Lists the tags for the specified resource.

Type annotations for
`session.create_client("savingsplans").list_tags_for_resource` method.

Boto3 documentation:
[SavingsPlans.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="tag\_resource"></a>

### tag_resource

Adds the specified tags to the specified resource.

Type annotations for `session.create_client("savingsplans").tag_resource`
method.

Boto3 documentation:
[SavingsPlans.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tags`: `Mapping`\[`str`, `str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag\_resource"></a>

### untag_resource

Removes the specified tags from the specified resource.

Type annotations for `session.create_client("savingsplans").untag_resource`
method.

Boto3 documentation:
[SavingsPlans.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `resourceArn`: `str` *(required)*
- `tagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("savingsplans").__aenter__` method.

Boto3 documentation:
[SavingsPlans.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [SavingsPlansClient](#savingsplansclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("savingsplans").__aexit__` method.

Boto3 documentation:
[SavingsPlans.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.
