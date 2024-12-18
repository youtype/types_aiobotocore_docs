# BillingConductorClient

> [Index](../README.md) > [BillingConductor](./README.md) > BillingConductorClient

!!! note ""

    Auto-generated documentation for [BillingConductor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#billingconductor)
    type annotations stubs module [types-aiobotocore-billingconductor](https://pypi.org/project/types-aiobotocore-billingconductor/).

## BillingConductorClient

Type annotations and code completion for `#!python session.create_client("billingconductor")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client)

```python
# BillingConductorClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_billingconductor.client import BillingConductorClient

session = get_session()
async with session.create_client("billingconductor") as client:
    client: BillingConductorClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("billingconductor").exceptions` structure.

```python
# BillingConductorClient.exceptions usage example

async with session.create_client("billingconductor") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceLimitExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# BillingConductorClient usage type checking example

from types_aiobotocore_billingconductor.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("billingconductor").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("billingconductor").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### close



Type annotations and code completion for `#!python session.create_client("billingconductor").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### associate\_accounts

Connects an array of account IDs in a consolidated billing family to a
predefined billing group.

Type annotations and code completion for `#!python session.create_client("billingconductor").associate_accounts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/associate_accounts.html)

```python
# associate_accounts method definition

await def associate_accounts(
    self,
    *,
    Arn: str,
    AccountIds: Sequence[str],
) -> AssociateAccountsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssociateAccountsOutputTypeDef](./type_defs.md#associateaccountsoutputtypedef) 


```python
# associate_accounts method usage example with argument unpacking

kwargs: AssociateAccountsInputRequestTypeDef = {  # (1)
    "Arn": ...,
    "AccountIds": ...,
}

parent.associate_accounts(**kwargs)
```

1. See [:material-code-braces: AssociateAccountsInputRequestTypeDef](./type_defs.md#associateaccountsinputrequesttypedef) 

### associate\_pricing\_rules

Connects an array of <code>PricingRuleArns</code> to a defined
<code>PricingPlan</code>.

Type annotations and code completion for `#!python session.create_client("billingconductor").associate_pricing_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/associate_pricing_rules.html)

```python
# associate_pricing_rules method definition

await def associate_pricing_rules(
    self,
    *,
    Arn: str,
    PricingRuleArns: Sequence[str],
) -> AssociatePricingRulesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssociatePricingRulesOutputTypeDef](./type_defs.md#associatepricingrulesoutputtypedef) 


```python
# associate_pricing_rules method usage example with argument unpacking

kwargs: AssociatePricingRulesInputRequestTypeDef = {  # (1)
    "Arn": ...,
    "PricingRuleArns": ...,
}

parent.associate_pricing_rules(**kwargs)
```

1. See [:material-code-braces: AssociatePricingRulesInputRequestTypeDef](./type_defs.md#associatepricingrulesinputrequesttypedef) 

### batch\_associate\_resources\_to\_custom\_line\_item

Associates a batch of resources to a percentage custom line item.

Type annotations and code completion for `#!python session.create_client("billingconductor").batch_associate_resources_to_custom_line_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/batch_associate_resources_to_custom_line_item.html)

```python
# batch_associate_resources_to_custom_line_item method definition

await def batch_associate_resources_to_custom_line_item(
    self,
    *,
    TargetArn: str,
    ResourceArns: Sequence[str],
    BillingPeriodRange: CustomLineItemBillingPeriodRangeTypeDef = ...,  # (1)
) -> BatchAssociateResourcesToCustomLineItemOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CustomLineItemBillingPeriodRangeTypeDef](./type_defs.md#customlineitembillingperiodrangetypedef) 
2. See [:material-code-braces: BatchAssociateResourcesToCustomLineItemOutputTypeDef](./type_defs.md#batchassociateresourcestocustomlineitemoutputtypedef) 


```python
# batch_associate_resources_to_custom_line_item method usage example with argument unpacking

kwargs: BatchAssociateResourcesToCustomLineItemInputRequestTypeDef = {  # (1)
    "TargetArn": ...,
    "ResourceArns": ...,
}

parent.batch_associate_resources_to_custom_line_item(**kwargs)
```

1. See [:material-code-braces: BatchAssociateResourcesToCustomLineItemInputRequestTypeDef](./type_defs.md#batchassociateresourcestocustomlineiteminputrequesttypedef) 

### batch\_disassociate\_resources\_from\_custom\_line\_item

Disassociates a batch of resources from a percentage custom line item.

Type annotations and code completion for `#!python session.create_client("billingconductor").batch_disassociate_resources_from_custom_line_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/batch_disassociate_resources_from_custom_line_item.html)

```python
# batch_disassociate_resources_from_custom_line_item method definition

await def batch_disassociate_resources_from_custom_line_item(
    self,
    *,
    TargetArn: str,
    ResourceArns: Sequence[str],
    BillingPeriodRange: CustomLineItemBillingPeriodRangeTypeDef = ...,  # (1)
) -> BatchDisassociateResourcesFromCustomLineItemOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CustomLineItemBillingPeriodRangeTypeDef](./type_defs.md#customlineitembillingperiodrangetypedef) 
2. See [:material-code-braces: BatchDisassociateResourcesFromCustomLineItemOutputTypeDef](./type_defs.md#batchdisassociateresourcesfromcustomlineitemoutputtypedef) 


```python
# batch_disassociate_resources_from_custom_line_item method usage example with argument unpacking

kwargs: BatchDisassociateResourcesFromCustomLineItemInputRequestTypeDef = {  # (1)
    "TargetArn": ...,
    "ResourceArns": ...,
}

parent.batch_disassociate_resources_from_custom_line_item(**kwargs)
```

1. See [:material-code-braces: BatchDisassociateResourcesFromCustomLineItemInputRequestTypeDef](./type_defs.md#batchdisassociateresourcesfromcustomlineiteminputrequesttypedef) 

### create\_billing\_group

Creates a billing group that resembles a consolidated billing family that
Amazon Web Services charges, based off of the predefined pricing plan
computation.

Type annotations and code completion for `#!python session.create_client("billingconductor").create_billing_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/create_billing_group.html)

```python
# create_billing_group method definition

await def create_billing_group(
    self,
    *,
    Name: str,
    AccountGrouping: AccountGroupingTypeDef,  # (1)
    ComputationPreference: ComputationPreferenceTypeDef,  # (2)
    ClientToken: str = ...,
    PrimaryAccountId: str = ...,
    Description: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateBillingGroupOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AccountGroupingTypeDef](./type_defs.md#accountgroupingtypedef) 
2. See [:material-code-braces: ComputationPreferenceTypeDef](./type_defs.md#computationpreferencetypedef) 
3. See [:material-code-braces: CreateBillingGroupOutputTypeDef](./type_defs.md#createbillinggroupoutputtypedef) 


```python
# create_billing_group method usage example with argument unpacking

kwargs: CreateBillingGroupInputRequestTypeDef = {  # (1)
    "Name": ...,
    "AccountGrouping": ...,
    "ComputationPreference": ...,
}

parent.create_billing_group(**kwargs)
```

1. See [:material-code-braces: CreateBillingGroupInputRequestTypeDef](./type_defs.md#createbillinggroupinputrequesttypedef) 

### create\_custom\_line\_item

Creates a custom line item that can be used to create a one-time fixed charge
that can be applied to a single billing group for the current or previous
billing period.

Type annotations and code completion for `#!python session.create_client("billingconductor").create_custom_line_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/create_custom_line_item.html)

```python
# create_custom_line_item method definition

await def create_custom_line_item(
    self,
    *,
    Name: str,
    Description: str,
    BillingGroupArn: str,
    ChargeDetails: CustomLineItemChargeDetailsTypeDef,  # (1)
    ClientToken: str = ...,
    BillingPeriodRange: CustomLineItemBillingPeriodRangeTypeDef = ...,  # (2)
    Tags: Mapping[str, str] = ...,
    AccountId: str = ...,
) -> CreateCustomLineItemOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: CustomLineItemChargeDetailsTypeDef](./type_defs.md#customlineitemchargedetailstypedef) 
2. See [:material-code-braces: CustomLineItemBillingPeriodRangeTypeDef](./type_defs.md#customlineitembillingperiodrangetypedef) 
3. See [:material-code-braces: CreateCustomLineItemOutputTypeDef](./type_defs.md#createcustomlineitemoutputtypedef) 


```python
# create_custom_line_item method usage example with argument unpacking

kwargs: CreateCustomLineItemInputRequestTypeDef = {  # (1)
    "Name": ...,
    "Description": ...,
    "BillingGroupArn": ...,
    "ChargeDetails": ...,
}

parent.create_custom_line_item(**kwargs)
```

1. See [:material-code-braces: CreateCustomLineItemInputRequestTypeDef](./type_defs.md#createcustomlineiteminputrequesttypedef) 

### create\_pricing\_plan

Creates a pricing plan that is used for computing Amazon Web Services charges
for billing groups.

Type annotations and code completion for `#!python session.create_client("billingconductor").create_pricing_plan` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/create_pricing_plan.html)

```python
# create_pricing_plan method definition

await def create_pricing_plan(
    self,
    *,
    Name: str,
    ClientToken: str = ...,
    Description: str = ...,
    PricingRuleArns: Sequence[str] = ...,
    Tags: Mapping[str, str] = ...,
) -> CreatePricingPlanOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreatePricingPlanOutputTypeDef](./type_defs.md#createpricingplanoutputtypedef) 


```python
# create_pricing_plan method usage example with argument unpacking

kwargs: CreatePricingPlanInputRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.create_pricing_plan(**kwargs)
```

1. See [:material-code-braces: CreatePricingPlanInputRequestTypeDef](./type_defs.md#createpricingplaninputrequesttypedef) 

### create\_pricing\_rule

Creates a pricing rule can be associated to a pricing plan, or a set of pricing
plans.

Type annotations and code completion for `#!python session.create_client("billingconductor").create_pricing_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/create_pricing_rule.html)

```python
# create_pricing_rule method definition

await def create_pricing_rule(
    self,
    *,
    Name: str,
    Scope: PricingRuleScopeType,  # (1)
    Type: PricingRuleTypeType,  # (2)
    ClientToken: str = ...,
    Description: str = ...,
    ModifierPercentage: float = ...,
    Service: str = ...,
    Tags: Mapping[str, str] = ...,
    BillingEntity: str = ...,
    Tiering: CreateTieringInputTypeDef = ...,  # (3)
    UsageType: str = ...,
    Operation: str = ...,
) -> CreatePricingRuleOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: PricingRuleScopeType](./literals.md#pricingrulescopetype) 
2. See [:material-code-brackets: PricingRuleTypeType](./literals.md#pricingruletypetype) 
3. See [:material-code-braces: CreateTieringInputTypeDef](./type_defs.md#createtieringinputtypedef) 
4. See [:material-code-braces: CreatePricingRuleOutputTypeDef](./type_defs.md#createpricingruleoutputtypedef) 


```python
# create_pricing_rule method usage example with argument unpacking

kwargs: CreatePricingRuleInputRequestTypeDef = {  # (1)
    "Name": ...,
    "Scope": ...,
    "Type": ...,
}

parent.create_pricing_rule(**kwargs)
```

1. See [:material-code-braces: CreatePricingRuleInputRequestTypeDef](./type_defs.md#createpricingruleinputrequesttypedef) 

### delete\_billing\_group

Deletes a billing group.

Type annotations and code completion for `#!python session.create_client("billingconductor").delete_billing_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/delete_billing_group.html)

```python
# delete_billing_group method definition

await def delete_billing_group(
    self,
    *,
    Arn: str,
) -> DeleteBillingGroupOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteBillingGroupOutputTypeDef](./type_defs.md#deletebillinggroupoutputtypedef) 


```python
# delete_billing_group method usage example with argument unpacking

kwargs: DeleteBillingGroupInputRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.delete_billing_group(**kwargs)
```

1. See [:material-code-braces: DeleteBillingGroupInputRequestTypeDef](./type_defs.md#deletebillinggroupinputrequesttypedef) 

### delete\_custom\_line\_item

Deletes the custom line item identified by the given ARN in the current, or
previous billing period.

Type annotations and code completion for `#!python session.create_client("billingconductor").delete_custom_line_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/delete_custom_line_item.html)

```python
# delete_custom_line_item method definition

await def delete_custom_line_item(
    self,
    *,
    Arn: str,
    BillingPeriodRange: CustomLineItemBillingPeriodRangeTypeDef = ...,  # (1)
) -> DeleteCustomLineItemOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CustomLineItemBillingPeriodRangeTypeDef](./type_defs.md#customlineitembillingperiodrangetypedef) 
2. See [:material-code-braces: DeleteCustomLineItemOutputTypeDef](./type_defs.md#deletecustomlineitemoutputtypedef) 


```python
# delete_custom_line_item method usage example with argument unpacking

kwargs: DeleteCustomLineItemInputRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.delete_custom_line_item(**kwargs)
```

1. See [:material-code-braces: DeleteCustomLineItemInputRequestTypeDef](./type_defs.md#deletecustomlineiteminputrequesttypedef) 

### delete\_pricing\_plan

Deletes a pricing plan.

Type annotations and code completion for `#!python session.create_client("billingconductor").delete_pricing_plan` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/delete_pricing_plan.html)

```python
# delete_pricing_plan method definition

await def delete_pricing_plan(
    self,
    *,
    Arn: str,
) -> DeletePricingPlanOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeletePricingPlanOutputTypeDef](./type_defs.md#deletepricingplanoutputtypedef) 


```python
# delete_pricing_plan method usage example with argument unpacking

kwargs: DeletePricingPlanInputRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.delete_pricing_plan(**kwargs)
```

1. See [:material-code-braces: DeletePricingPlanInputRequestTypeDef](./type_defs.md#deletepricingplaninputrequesttypedef) 

### delete\_pricing\_rule

Deletes the pricing rule that's identified by the input Amazon Resource Name
(ARN).

Type annotations and code completion for `#!python session.create_client("billingconductor").delete_pricing_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/delete_pricing_rule.html)

```python
# delete_pricing_rule method definition

await def delete_pricing_rule(
    self,
    *,
    Arn: str,
) -> DeletePricingRuleOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeletePricingRuleOutputTypeDef](./type_defs.md#deletepricingruleoutputtypedef) 


```python
# delete_pricing_rule method usage example with argument unpacking

kwargs: DeletePricingRuleInputRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.delete_pricing_rule(**kwargs)
```

1. See [:material-code-braces: DeletePricingRuleInputRequestTypeDef](./type_defs.md#deletepricingruleinputrequesttypedef) 

### disassociate\_accounts

Removes the specified list of account IDs from the given billing group.

Type annotations and code completion for `#!python session.create_client("billingconductor").disassociate_accounts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/disassociate_accounts.html)

```python
# disassociate_accounts method definition

await def disassociate_accounts(
    self,
    *,
    Arn: str,
    AccountIds: Sequence[str],
) -> DisassociateAccountsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DisassociateAccountsOutputTypeDef](./type_defs.md#disassociateaccountsoutputtypedef) 


```python
# disassociate_accounts method usage example with argument unpacking

kwargs: DisassociateAccountsInputRequestTypeDef = {  # (1)
    "Arn": ...,
    "AccountIds": ...,
}

parent.disassociate_accounts(**kwargs)
```

1. See [:material-code-braces: DisassociateAccountsInputRequestTypeDef](./type_defs.md#disassociateaccountsinputrequesttypedef) 

### disassociate\_pricing\_rules

Disassociates a list of pricing rules from a pricing plan.

Type annotations and code completion for `#!python session.create_client("billingconductor").disassociate_pricing_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/disassociate_pricing_rules.html)

```python
# disassociate_pricing_rules method definition

await def disassociate_pricing_rules(
    self,
    *,
    Arn: str,
    PricingRuleArns: Sequence[str],
) -> DisassociatePricingRulesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DisassociatePricingRulesOutputTypeDef](./type_defs.md#disassociatepricingrulesoutputtypedef) 


```python
# disassociate_pricing_rules method usage example with argument unpacking

kwargs: DisassociatePricingRulesInputRequestTypeDef = {  # (1)
    "Arn": ...,
    "PricingRuleArns": ...,
}

parent.disassociate_pricing_rules(**kwargs)
```

1. See [:material-code-braces: DisassociatePricingRulesInputRequestTypeDef](./type_defs.md#disassociatepricingrulesinputrequesttypedef) 

### get\_billing\_group\_cost\_report

Retrieves the margin summary report, which includes the Amazon Web Services
cost and charged amount (pro forma cost) by Amazon Web Service for a specific
billing group.

Type annotations and code completion for `#!python session.create_client("billingconductor").get_billing_group_cost_report` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/get_billing_group_cost_report.html)

```python
# get_billing_group_cost_report method definition

await def get_billing_group_cost_report(
    self,
    *,
    Arn: str,
    BillingPeriodRange: BillingPeriodRangeTypeDef = ...,  # (1)
    GroupBy: Sequence[GroupByAttributeNameType] = ...,  # (2)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> GetBillingGroupCostReportOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: BillingPeriodRangeTypeDef](./type_defs.md#billingperiodrangetypedef) 
2. See [:material-code-brackets: GroupByAttributeNameType](./literals.md#groupbyattributenametype) 
3. See [:material-code-braces: GetBillingGroupCostReportOutputTypeDef](./type_defs.md#getbillinggroupcostreportoutputtypedef) 


```python
# get_billing_group_cost_report method usage example with argument unpacking

kwargs: GetBillingGroupCostReportInputRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.get_billing_group_cost_report(**kwargs)
```

1. See [:material-code-braces: GetBillingGroupCostReportInputRequestTypeDef](./type_defs.md#getbillinggroupcostreportinputrequesttypedef) 

### list\_account\_associations

This is a paginated call to list linked accounts that are linked to the payer
account for the specified time period.

Type annotations and code completion for `#!python session.create_client("billingconductor").list_account_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/list_account_associations.html)

```python
# list_account_associations method definition

await def list_account_associations(
    self,
    *,
    BillingPeriod: str = ...,
    Filters: ListAccountAssociationsFilterTypeDef = ...,  # (1)
    NextToken: str = ...,
) -> ListAccountAssociationsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ListAccountAssociationsFilterTypeDef](./type_defs.md#listaccountassociationsfiltertypedef) 
2. See [:material-code-braces: ListAccountAssociationsOutputTypeDef](./type_defs.md#listaccountassociationsoutputtypedef) 


```python
# list_account_associations method usage example with argument unpacking

kwargs: ListAccountAssociationsInputRequestTypeDef = {  # (1)
    "BillingPeriod": ...,
}

parent.list_account_associations(**kwargs)
```

1. See [:material-code-braces: ListAccountAssociationsInputRequestTypeDef](./type_defs.md#listaccountassociationsinputrequesttypedef) 

### list\_billing\_group\_cost\_reports

A paginated call to retrieve a summary report of actual Amazon Web Services
charges and the calculated Amazon Web Services charges based on the associated
pricing plan of a billing group.

Type annotations and code completion for `#!python session.create_client("billingconductor").list_billing_group_cost_reports` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/list_billing_group_cost_reports.html)

```python
# list_billing_group_cost_reports method definition

await def list_billing_group_cost_reports(
    self,
    *,
    BillingPeriod: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    Filters: ListBillingGroupCostReportsFilterTypeDef = ...,  # (1)
) -> ListBillingGroupCostReportsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ListBillingGroupCostReportsFilterTypeDef](./type_defs.md#listbillinggroupcostreportsfiltertypedef) 
2. See [:material-code-braces: ListBillingGroupCostReportsOutputTypeDef](./type_defs.md#listbillinggroupcostreportsoutputtypedef) 


```python
# list_billing_group_cost_reports method usage example with argument unpacking

kwargs: ListBillingGroupCostReportsInputRequestTypeDef = {  # (1)
    "BillingPeriod": ...,
}

parent.list_billing_group_cost_reports(**kwargs)
```

1. See [:material-code-braces: ListBillingGroupCostReportsInputRequestTypeDef](./type_defs.md#listbillinggroupcostreportsinputrequesttypedef) 

### list\_billing\_groups

A paginated call to retrieve a list of billing groups for the given billing
period.

Type annotations and code completion for `#!python session.create_client("billingconductor").list_billing_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/list_billing_groups.html)

```python
# list_billing_groups method definition

await def list_billing_groups(
    self,
    *,
    BillingPeriod: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    Filters: ListBillingGroupsFilterTypeDef = ...,  # (1)
) -> ListBillingGroupsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ListBillingGroupsFilterTypeDef](./type_defs.md#listbillinggroupsfiltertypedef) 
2. See [:material-code-braces: ListBillingGroupsOutputTypeDef](./type_defs.md#listbillinggroupsoutputtypedef) 


```python
# list_billing_groups method usage example with argument unpacking

kwargs: ListBillingGroupsInputRequestTypeDef = {  # (1)
    "BillingPeriod": ...,
}

parent.list_billing_groups(**kwargs)
```

1. See [:material-code-braces: ListBillingGroupsInputRequestTypeDef](./type_defs.md#listbillinggroupsinputrequesttypedef) 

### list\_custom\_line\_item\_versions

A paginated call to get a list of all custom line item versions.

Type annotations and code completion for `#!python session.create_client("billingconductor").list_custom_line_item_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/list_custom_line_item_versions.html)

```python
# list_custom_line_item_versions method definition

await def list_custom_line_item_versions(
    self,
    *,
    Arn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
    Filters: ListCustomLineItemVersionsFilterTypeDef = ...,  # (1)
) -> ListCustomLineItemVersionsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ListCustomLineItemVersionsFilterTypeDef](./type_defs.md#listcustomlineitemversionsfiltertypedef) 
2. See [:material-code-braces: ListCustomLineItemVersionsOutputTypeDef](./type_defs.md#listcustomlineitemversionsoutputtypedef) 


```python
# list_custom_line_item_versions method usage example with argument unpacking

kwargs: ListCustomLineItemVersionsInputRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.list_custom_line_item_versions(**kwargs)
```

1. See [:material-code-braces: ListCustomLineItemVersionsInputRequestTypeDef](./type_defs.md#listcustomlineitemversionsinputrequesttypedef) 

### list\_custom\_line\_items

A paginated call to get a list of all custom line items (FFLIs) for the given
billing period.

Type annotations and code completion for `#!python session.create_client("billingconductor").list_custom_line_items` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/list_custom_line_items.html)

```python
# list_custom_line_items method definition

await def list_custom_line_items(
    self,
    *,
    BillingPeriod: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    Filters: ListCustomLineItemsFilterTypeDef = ...,  # (1)
) -> ListCustomLineItemsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ListCustomLineItemsFilterTypeDef](./type_defs.md#listcustomlineitemsfiltertypedef) 
2. See [:material-code-braces: ListCustomLineItemsOutputTypeDef](./type_defs.md#listcustomlineitemsoutputtypedef) 


```python
# list_custom_line_items method usage example with argument unpacking

kwargs: ListCustomLineItemsInputRequestTypeDef = {  # (1)
    "BillingPeriod": ...,
}

parent.list_custom_line_items(**kwargs)
```

1. See [:material-code-braces: ListCustomLineItemsInputRequestTypeDef](./type_defs.md#listcustomlineitemsinputrequesttypedef) 

### list\_pricing\_plans

A paginated call to get pricing plans for the given billing period.

Type annotations and code completion for `#!python session.create_client("billingconductor").list_pricing_plans` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/list_pricing_plans.html)

```python
# list_pricing_plans method definition

await def list_pricing_plans(
    self,
    *,
    BillingPeriod: str = ...,
    Filters: ListPricingPlansFilterTypeDef = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListPricingPlansOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ListPricingPlansFilterTypeDef](./type_defs.md#listpricingplansfiltertypedef) 
2. See [:material-code-braces: ListPricingPlansOutputTypeDef](./type_defs.md#listpricingplansoutputtypedef) 


```python
# list_pricing_plans method usage example with argument unpacking

kwargs: ListPricingPlansInputRequestTypeDef = {  # (1)
    "BillingPeriod": ...,
}

parent.list_pricing_plans(**kwargs)
```

1. See [:material-code-braces: ListPricingPlansInputRequestTypeDef](./type_defs.md#listpricingplansinputrequesttypedef) 

### list\_pricing\_plans\_associated\_with\_pricing\_rule

A list of the pricing plans that are associated with a pricing rule.

Type annotations and code completion for `#!python session.create_client("billingconductor").list_pricing_plans_associated_with_pricing_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/list_pricing_plans_associated_with_pricing_rule.html)

```python
# list_pricing_plans_associated_with_pricing_rule method definition

await def list_pricing_plans_associated_with_pricing_rule(
    self,
    *,
    PricingRuleArn: str,
    BillingPeriod: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListPricingPlansAssociatedWithPricingRuleOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPricingPlansAssociatedWithPricingRuleOutputTypeDef](./type_defs.md#listpricingplansassociatedwithpricingruleoutputtypedef) 


```python
# list_pricing_plans_associated_with_pricing_rule method usage example with argument unpacking

kwargs: ListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef = {  # (1)
    "PricingRuleArn": ...,
}

parent.list_pricing_plans_associated_with_pricing_rule(**kwargs)
```

1. See [:material-code-braces: ListPricingPlansAssociatedWithPricingRuleInputRequestTypeDef](./type_defs.md#listpricingplansassociatedwithpricingruleinputrequesttypedef) 

### list\_pricing\_rules

Describes a pricing rule that can be associated to a pricing plan, or set of
pricing plans.

Type annotations and code completion for `#!python session.create_client("billingconductor").list_pricing_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/list_pricing_rules.html)

```python
# list_pricing_rules method definition

await def list_pricing_rules(
    self,
    *,
    BillingPeriod: str = ...,
    Filters: ListPricingRulesFilterTypeDef = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListPricingRulesOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ListPricingRulesFilterTypeDef](./type_defs.md#listpricingrulesfiltertypedef) 
2. See [:material-code-braces: ListPricingRulesOutputTypeDef](./type_defs.md#listpricingrulesoutputtypedef) 


```python
# list_pricing_rules method usage example with argument unpacking

kwargs: ListPricingRulesInputRequestTypeDef = {  # (1)
    "BillingPeriod": ...,
}

parent.list_pricing_rules(**kwargs)
```

1. See [:material-code-braces: ListPricingRulesInputRequestTypeDef](./type_defs.md#listpricingrulesinputrequesttypedef) 

### list\_pricing\_rules\_associated\_to\_pricing\_plan

Lists the pricing rules that are associated with a pricing plan.

Type annotations and code completion for `#!python session.create_client("billingconductor").list_pricing_rules_associated_to_pricing_plan` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/list_pricing_rules_associated_to_pricing_plan.html)

```python
# list_pricing_rules_associated_to_pricing_plan method definition

await def list_pricing_rules_associated_to_pricing_plan(
    self,
    *,
    PricingPlanArn: str,
    BillingPeriod: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListPricingRulesAssociatedToPricingPlanOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPricingRulesAssociatedToPricingPlanOutputTypeDef](./type_defs.md#listpricingrulesassociatedtopricingplanoutputtypedef) 


```python
# list_pricing_rules_associated_to_pricing_plan method usage example with argument unpacking

kwargs: ListPricingRulesAssociatedToPricingPlanInputRequestTypeDef = {  # (1)
    "PricingPlanArn": ...,
}

parent.list_pricing_rules_associated_to_pricing_plan(**kwargs)
```

1. See [:material-code-braces: ListPricingRulesAssociatedToPricingPlanInputRequestTypeDef](./type_defs.md#listpricingrulesassociatedtopricingplaninputrequesttypedef) 

### list\_resources\_associated\_to\_custom\_line\_item

List the resources that are associated to a custom line item.

Type annotations and code completion for `#!python session.create_client("billingconductor").list_resources_associated_to_custom_line_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/list_resources_associated_to_custom_line_item.html)

```python
# list_resources_associated_to_custom_line_item method definition

await def list_resources_associated_to_custom_line_item(
    self,
    *,
    Arn: str,
    BillingPeriod: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    Filters: ListResourcesAssociatedToCustomLineItemFilterTypeDef = ...,  # (1)
) -> ListResourcesAssociatedToCustomLineItemOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ListResourcesAssociatedToCustomLineItemFilterTypeDef](./type_defs.md#listresourcesassociatedtocustomlineitemfiltertypedef) 
2. See [:material-code-braces: ListResourcesAssociatedToCustomLineItemOutputTypeDef](./type_defs.md#listresourcesassociatedtocustomlineitemoutputtypedef) 


```python
# list_resources_associated_to_custom_line_item method usage example with argument unpacking

kwargs: ListResourcesAssociatedToCustomLineItemInputRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.list_resources_associated_to_custom_line_item(**kwargs)
```

1. See [:material-code-braces: ListResourcesAssociatedToCustomLineItemInputRequestTypeDef](./type_defs.md#listresourcesassociatedtocustomlineiteminputrequesttypedef) 

### list\_tags\_for\_resource

A list the tags for a resource.

Type annotations and code completion for `#!python session.create_client("billingconductor").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### tag\_resource

Associates the specified tags to a resource with the specified
<code>resourceArn</code>.

Type annotations and code completion for `#!python session.create_client("billingconductor").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Deletes specified tags from a resource.

Type annotations and code completion for `#!python session.create_client("billingconductor").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_billing\_group

This updates an existing billing group.

Type annotations and code completion for `#!python session.create_client("billingconductor").update_billing_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/update_billing_group.html)

```python
# update_billing_group method definition

await def update_billing_group(
    self,
    *,
    Arn: str,
    Name: str = ...,
    Status: BillingGroupStatusType = ...,  # (1)
    ComputationPreference: ComputationPreferenceTypeDef = ...,  # (2)
    Description: str = ...,
    AccountGrouping: UpdateBillingGroupAccountGroupingTypeDef = ...,  # (3)
) -> UpdateBillingGroupOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: BillingGroupStatusType](./literals.md#billinggroupstatustype) 
2. See [:material-code-braces: ComputationPreferenceTypeDef](./type_defs.md#computationpreferencetypedef) 
3. See [:material-code-braces: UpdateBillingGroupAccountGroupingTypeDef](./type_defs.md#updatebillinggroupaccountgroupingtypedef) 
4. See [:material-code-braces: UpdateBillingGroupOutputTypeDef](./type_defs.md#updatebillinggroupoutputtypedef) 


```python
# update_billing_group method usage example with argument unpacking

kwargs: UpdateBillingGroupInputRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.update_billing_group(**kwargs)
```

1. See [:material-code-braces: UpdateBillingGroupInputRequestTypeDef](./type_defs.md#updatebillinggroupinputrequesttypedef) 

### update\_custom\_line\_item

Update an existing custom line item in the current or previous billing period.

Type annotations and code completion for `#!python session.create_client("billingconductor").update_custom_line_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/update_custom_line_item.html)

```python
# update_custom_line_item method definition

await def update_custom_line_item(
    self,
    *,
    Arn: str,
    Name: str = ...,
    Description: str = ...,
    ChargeDetails: UpdateCustomLineItemChargeDetailsTypeDef = ...,  # (1)
    BillingPeriodRange: CustomLineItemBillingPeriodRangeTypeDef = ...,  # (2)
) -> UpdateCustomLineItemOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: UpdateCustomLineItemChargeDetailsTypeDef](./type_defs.md#updatecustomlineitemchargedetailstypedef) 
2. See [:material-code-braces: CustomLineItemBillingPeriodRangeTypeDef](./type_defs.md#customlineitembillingperiodrangetypedef) 
3. See [:material-code-braces: UpdateCustomLineItemOutputTypeDef](./type_defs.md#updatecustomlineitemoutputtypedef) 


```python
# update_custom_line_item method usage example with argument unpacking

kwargs: UpdateCustomLineItemInputRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.update_custom_line_item(**kwargs)
```

1. See [:material-code-braces: UpdateCustomLineItemInputRequestTypeDef](./type_defs.md#updatecustomlineiteminputrequesttypedef) 

### update\_pricing\_plan

This updates an existing pricing plan.

Type annotations and code completion for `#!python session.create_client("billingconductor").update_pricing_plan` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/update_pricing_plan.html)

```python
# update_pricing_plan method definition

await def update_pricing_plan(
    self,
    *,
    Arn: str,
    Name: str = ...,
    Description: str = ...,
) -> UpdatePricingPlanOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdatePricingPlanOutputTypeDef](./type_defs.md#updatepricingplanoutputtypedef) 


```python
# update_pricing_plan method usage example with argument unpacking

kwargs: UpdatePricingPlanInputRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.update_pricing_plan(**kwargs)
```

1. See [:material-code-braces: UpdatePricingPlanInputRequestTypeDef](./type_defs.md#updatepricingplaninputrequesttypedef) 

### update\_pricing\_rule

Updates an existing pricing rule.

Type annotations and code completion for `#!python session.create_client("billingconductor").update_pricing_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor/client/update_pricing_rule.html)

```python
# update_pricing_rule method definition

await def update_pricing_rule(
    self,
    *,
    Arn: str,
    Name: str = ...,
    Description: str = ...,
    Type: PricingRuleTypeType = ...,  # (1)
    ModifierPercentage: float = ...,
    Tiering: UpdateTieringInputTypeDef = ...,  # (2)
) -> UpdatePricingRuleOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: PricingRuleTypeType](./literals.md#pricingruletypetype) 
2. See [:material-code-braces: UpdateTieringInputTypeDef](./type_defs.md#updatetieringinputtypedef) 
3. See [:material-code-braces: UpdatePricingRuleOutputTypeDef](./type_defs.md#updatepricingruleoutputtypedef) 


```python
# update_pricing_rule method usage example with argument unpacking

kwargs: UpdatePricingRuleInputRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.update_pricing_rule(**kwargs)
```

1. See [:material-code-braces: UpdatePricingRuleInputRequestTypeDef](./type_defs.md#updatepricingruleinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("billingconductor").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "BillingConductorClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("billingconductor").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#BillingConductor.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("billingconductor").get_paginator` method with overloads.

- `client.get_paginator("list_account_associations")` -> [ListAccountAssociationsPaginator](./paginators.md#listaccountassociationspaginator)
- `client.get_paginator("list_billing_group_cost_reports")` -> [ListBillingGroupCostReportsPaginator](./paginators.md#listbillinggroupcostreportspaginator)
- `client.get_paginator("list_billing_groups")` -> [ListBillingGroupsPaginator](./paginators.md#listbillinggroupspaginator)
- `client.get_paginator("list_custom_line_item_versions")` -> [ListCustomLineItemVersionsPaginator](./paginators.md#listcustomlineitemversionspaginator)
- `client.get_paginator("list_custom_line_items")` -> [ListCustomLineItemsPaginator](./paginators.md#listcustomlineitemspaginator)
- `client.get_paginator("list_pricing_plans_associated_with_pricing_rule")` -> [ListPricingPlansAssociatedWithPricingRulePaginator](./paginators.md#listpricingplansassociatedwithpricingrulepaginator)
- `client.get_paginator("list_pricing_plans")` -> [ListPricingPlansPaginator](./paginators.md#listpricingplanspaginator)
- `client.get_paginator("list_pricing_rules_associated_to_pricing_plan")` -> [ListPricingRulesAssociatedToPricingPlanPaginator](./paginators.md#listpricingrulesassociatedtopricingplanpaginator)
- `client.get_paginator("list_pricing_rules")` -> [ListPricingRulesPaginator](./paginators.md#listpricingrulespaginator)
- `client.get_paginator("list_resources_associated_to_custom_line_item")` -> [ListResourcesAssociatedToCustomLineItemPaginator](./paginators.md#listresourcesassociatedtocustomlineitempaginator)



