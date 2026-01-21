# Type definitions

> [Index](../README.md) > [AgreementService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [AgreementService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-agreement.html#agreementservice)
    type annotations stubs module [types-aiobotocore-marketplace-agreement](https://pypi.org/project/types-aiobotocore-marketplace-agreement/).



## ByolPricingTermTypeDef

```python
# ByolPricingTermTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import ByolPricingTermTypeDef


def get_value() -> ByolPricingTermTypeDef:
    return {
        "type": ...,
    }


# ByolPricingTermTypeDef definition

class ByolPricingTermTypeDef(TypedDict):
    type: NotRequired[str],
```


## RecurringPaymentTermTypeDef

```python
# RecurringPaymentTermTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import RecurringPaymentTermTypeDef


def get_value() -> RecurringPaymentTermTypeDef:
    return {
        "type": ...,
    }


# RecurringPaymentTermTypeDef definition

class RecurringPaymentTermTypeDef(TypedDict):
    type: NotRequired[str],
    currencyCode: NotRequired[str],
    billingPeriod: NotRequired[str],
    price: NotRequired[str],
```


## SupportTermTypeDef

```python
# SupportTermTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import SupportTermTypeDef


def get_value() -> SupportTermTypeDef:
    return {
        "type": ...,
    }


# SupportTermTypeDef definition

class SupportTermTypeDef(TypedDict):
    type: NotRequired[str],
    refundPolicy: NotRequired[str],
```


## ValidityTermTypeDef

```python
# ValidityTermTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import ValidityTermTypeDef


def get_value() -> ValidityTermTypeDef:
    return {
        "type": ...,
    }


# ValidityTermTypeDef definition

class ValidityTermTypeDef(TypedDict):
    type: NotRequired[str],
    agreementDuration: NotRequired[str],
    agreementStartDate: NotRequired[datetime.datetime],
    agreementEndDate: NotRequired[datetime.datetime],
```


## AcceptorTypeDef

```python
# AcceptorTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import AcceptorTypeDef


def get_value() -> AcceptorTypeDef:
    return {
        "accountId": ...,
    }


# AcceptorTypeDef definition

class AcceptorTypeDef(TypedDict):
    accountId: NotRequired[str],
```


## ProposerTypeDef

```python
# ProposerTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import ProposerTypeDef


def get_value() -> ProposerTypeDef:
    return {
        "accountId": ...,
    }


# ProposerTypeDef definition

class ProposerTypeDef(TypedDict):
    accountId: NotRequired[str],
```


## DimensionTypeDef

```python
# DimensionTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import DimensionTypeDef


def get_value() -> DimensionTypeDef:
    return {
        "dimensionKey": ...,
    }


# DimensionTypeDef definition

class DimensionTypeDef(TypedDict):
    dimensionKey: str,
    dimensionValue: int,
```


## ConstraintsTypeDef

```python
# ConstraintsTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import ConstraintsTypeDef


def get_value() -> ConstraintsTypeDef:
    return {
        "multipleDimensionSelection": ...,
    }


# ConstraintsTypeDef definition

class ConstraintsTypeDef(TypedDict):
    multipleDimensionSelection: NotRequired[str],
    quantityConfiguration: NotRequired[str],
```


## RateCardItemTypeDef

```python
# RateCardItemTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import RateCardItemTypeDef


def get_value() -> RateCardItemTypeDef:
    return {
        "dimensionKey": ...,
    }


# RateCardItemTypeDef definition

class RateCardItemTypeDef(TypedDict):
    dimensionKey: NotRequired[str],
    price: NotRequired[str],
```


## SelectorTypeDef

```python
# SelectorTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import SelectorTypeDef


def get_value() -> SelectorTypeDef:
    return {
        "type": ...,
    }


# SelectorTypeDef definition

class SelectorTypeDef(TypedDict):
    type: NotRequired[str],
    value: NotRequired[str],
```


## DescribeAgreementInputTypeDef

```python
# DescribeAgreementInputTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import DescribeAgreementInputTypeDef


def get_value() -> DescribeAgreementInputTypeDef:
    return {
        "agreementId": ...,
    }


# DescribeAgreementInputTypeDef definition

class DescribeAgreementInputTypeDef(TypedDict):
    agreementId: str,
```


## EstimatedChargesTypeDef

```python
# EstimatedChargesTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import EstimatedChargesTypeDef


def get_value() -> EstimatedChargesTypeDef:
    return {
        "currencyCode": ...,
    }


# EstimatedChargesTypeDef definition

class EstimatedChargesTypeDef(TypedDict):
    currencyCode: NotRequired[str],
    agreementValue: NotRequired[str],
```


## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```


## DocumentItemTypeDef

```python
# DocumentItemTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import DocumentItemTypeDef


def get_value() -> DocumentItemTypeDef:
    return {
        "type": ...,
    }


# DocumentItemTypeDef definition

class DocumentItemTypeDef(TypedDict):
    type: NotRequired[str],
    url: NotRequired[str],
    version: NotRequired[str],
```


## FilterTypeDef

```python
# FilterTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import FilterTypeDef


def get_value() -> FilterTypeDef:
    return {
        "name": ...,
    }


# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    name: NotRequired[str],
    values: NotRequired[Sequence[str]],
```


## GrantItemTypeDef

```python
# GrantItemTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import GrantItemTypeDef


def get_value() -> GrantItemTypeDef:
    return {
        "dimensionKey": ...,
    }


# GrantItemTypeDef definition

class GrantItemTypeDef(TypedDict):
    dimensionKey: NotRequired[str],
    maxQuantity: NotRequired[int],
```


## GetAgreementTermsInputTypeDef

```python
# GetAgreementTermsInputTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import GetAgreementTermsInputTypeDef


def get_value() -> GetAgreementTermsInputTypeDef:
    return {
        "agreementId": ...,
    }


# GetAgreementTermsInputTypeDef definition

class GetAgreementTermsInputTypeDef(TypedDict):
    agreementId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```


## ScheduleItemTypeDef

```python
# ScheduleItemTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import ScheduleItemTypeDef


def get_value() -> ScheduleItemTypeDef:
    return {
        "chargeDate": ...,
    }


# ScheduleItemTypeDef definition

class ScheduleItemTypeDef(TypedDict):
    chargeDate: NotRequired[datetime.datetime],
    chargeAmount: NotRequired[str],
```


## ResourceTypeDef

```python
# ResourceTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import ResourceTypeDef


def get_value() -> ResourceTypeDef:
    return {
        "id": ...,
    }


# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    id: NotRequired[str],
    type: NotRequired[str],
```


## RenewalTermConfigurationTypeDef

```python
# RenewalTermConfigurationTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import RenewalTermConfigurationTypeDef


def get_value() -> RenewalTermConfigurationTypeDef:
    return {
        "enableAutoRenew": ...,
    }


# RenewalTermConfigurationTypeDef definition

class RenewalTermConfigurationTypeDef(TypedDict):
    enableAutoRenew: bool,
```


## SortTypeDef

```python
# SortTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import SortTypeDef


def get_value() -> SortTypeDef:
    return {
        "sortBy": ...,
    }


# SortTypeDef definition

class SortTypeDef(TypedDict):
    sortBy: NotRequired[str],
    sortOrder: NotRequired[SortOrderType],  # (1)
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype)

## VariablePaymentTermConfigurationTypeDef

```python
# VariablePaymentTermConfigurationTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import VariablePaymentTermConfigurationTypeDef


def get_value() -> VariablePaymentTermConfigurationTypeDef:
    return {
        "paymentRequestApprovalStrategy": ...,
    }


# VariablePaymentTermConfigurationTypeDef definition

class VariablePaymentTermConfigurationTypeDef(TypedDict):
    paymentRequestApprovalStrategy: PaymentRequestApprovalStrategyType,  # (1)
    expirationDuration: NotRequired[str],
```

1. See [:material-code-brackets: PaymentRequestApprovalStrategyType](./literals.md#paymentrequestapprovalstrategytype)

## ConfigurableUpfrontPricingTermConfigurationTypeDef

```python
# ConfigurableUpfrontPricingTermConfigurationTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import ConfigurableUpfrontPricingTermConfigurationTypeDef


def get_value() -> ConfigurableUpfrontPricingTermConfigurationTypeDef:
    return {
        "selectorValue": ...,
    }


# ConfigurableUpfrontPricingTermConfigurationTypeDef definition

class ConfigurableUpfrontPricingTermConfigurationTypeDef(TypedDict):
    selectorValue: str,
    dimensions: list[DimensionTypeDef],  # (1)
```

1. See `list[DimensionTypeDef]`

## UsageBasedRateCardItemTypeDef

```python
# UsageBasedRateCardItemTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import UsageBasedRateCardItemTypeDef


def get_value() -> UsageBasedRateCardItemTypeDef:
    return {
        "rateCard": ...,
    }


# UsageBasedRateCardItemTypeDef definition

class UsageBasedRateCardItemTypeDef(TypedDict):
    rateCard: NotRequired[list[RateCardItemTypeDef]],  # (1)
```

1. See `list[RateCardItemTypeDef]`

## ConfigurableUpfrontRateCardItemTypeDef

```python
# ConfigurableUpfrontRateCardItemTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import ConfigurableUpfrontRateCardItemTypeDef


def get_value() -> ConfigurableUpfrontRateCardItemTypeDef:
    return {
        "selector": ...,
    }


# ConfigurableUpfrontRateCardItemTypeDef definition

class ConfigurableUpfrontRateCardItemTypeDef(TypedDict):
    selector: NotRequired[SelectorTypeDef],  # (1)
    constraints: NotRequired[ConstraintsTypeDef],  # (2)
    rateCard: NotRequired[list[RateCardItemTypeDef]],  # (3)
```

1. See [:material-code-braces: SelectorTypeDef](./type_defs.md#selectortypedef)
2. See [:material-code-braces: ConstraintsTypeDef](./type_defs.md#constraintstypedef)
3. See `list[RateCardItemTypeDef]`

## LegalTermTypeDef

```python
# LegalTermTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import LegalTermTypeDef


def get_value() -> LegalTermTypeDef:
    return {
        "type": ...,
    }


# LegalTermTypeDef definition

class LegalTermTypeDef(TypedDict):
    type: NotRequired[str],
    documents: NotRequired[list[DocumentItemTypeDef]],  # (1)
```

1. See `list[DocumentItemTypeDef]`

## FixedUpfrontPricingTermTypeDef

```python
# FixedUpfrontPricingTermTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import FixedUpfrontPricingTermTypeDef


def get_value() -> FixedUpfrontPricingTermTypeDef:
    return {
        "type": ...,
    }


# FixedUpfrontPricingTermTypeDef definition

class FixedUpfrontPricingTermTypeDef(TypedDict):
    type: NotRequired[str],
    currencyCode: NotRequired[str],
    duration: NotRequired[str],
    price: NotRequired[str],
    grants: NotRequired[list[GrantItemTypeDef]],  # (1)
```

1. See `list[GrantItemTypeDef]`

## FreeTrialPricingTermTypeDef

```python
# FreeTrialPricingTermTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import FreeTrialPricingTermTypeDef


def get_value() -> FreeTrialPricingTermTypeDef:
    return {
        "type": ...,
    }


# FreeTrialPricingTermTypeDef definition

class FreeTrialPricingTermTypeDef(TypedDict):
    type: NotRequired[str],
    duration: NotRequired[str],
    grants: NotRequired[list[GrantItemTypeDef]],  # (1)
```

1. See `list[GrantItemTypeDef]`

## PaymentScheduleTermTypeDef

```python
# PaymentScheduleTermTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import PaymentScheduleTermTypeDef


def get_value() -> PaymentScheduleTermTypeDef:
    return {
        "type": ...,
    }


# PaymentScheduleTermTypeDef definition

class PaymentScheduleTermTypeDef(TypedDict):
    type: NotRequired[str],
    currencyCode: NotRequired[str],
    schedule: NotRequired[list[ScheduleItemTypeDef]],  # (1)
```

1. See `list[ScheduleItemTypeDef]`

## ProposalSummaryTypeDef

```python
# ProposalSummaryTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import ProposalSummaryTypeDef


def get_value() -> ProposalSummaryTypeDef:
    return {
        "resources": ...,
    }


# ProposalSummaryTypeDef definition

class ProposalSummaryTypeDef(TypedDict):
    resources: NotRequired[list[ResourceTypeDef]],  # (1)
    offerId: NotRequired[str],
    offerSetId: NotRequired[str],
```

1. See `list[ResourceTypeDef]`

## RenewalTermTypeDef

```python
# RenewalTermTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import RenewalTermTypeDef


def get_value() -> RenewalTermTypeDef:
    return {
        "type": ...,
    }


# RenewalTermTypeDef definition

class RenewalTermTypeDef(TypedDict):
    type: NotRequired[str],
    configuration: NotRequired[RenewalTermConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: RenewalTermConfigurationTypeDef](./type_defs.md#renewaltermconfigurationtypedef)

## SearchAgreementsInputTypeDef

```python
# SearchAgreementsInputTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import SearchAgreementsInputTypeDef


def get_value() -> SearchAgreementsInputTypeDef:
    return {
        "catalog": ...,
    }


# SearchAgreementsInputTypeDef definition

class SearchAgreementsInputTypeDef(TypedDict):
    catalog: NotRequired[str],
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    sort: NotRequired[SortTypeDef],  # (2)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef)

## VariablePaymentTermTypeDef

```python
# VariablePaymentTermTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import VariablePaymentTermTypeDef


def get_value() -> VariablePaymentTermTypeDef:
    return {
        "type": ...,
    }


# VariablePaymentTermTypeDef definition

class VariablePaymentTermTypeDef(TypedDict):
    type: NotRequired[str],
    currencyCode: NotRequired[str],
    maxTotalChargeAmount: NotRequired[str],
    configuration: NotRequired[VariablePaymentTermConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: VariablePaymentTermConfigurationTypeDef](./type_defs.md#variablepaymenttermconfigurationtypedef)

## UsageBasedPricingTermTypeDef

```python
# UsageBasedPricingTermTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import UsageBasedPricingTermTypeDef


def get_value() -> UsageBasedPricingTermTypeDef:
    return {
        "type": ...,
    }


# UsageBasedPricingTermTypeDef definition

class UsageBasedPricingTermTypeDef(TypedDict):
    type: NotRequired[str],
    currencyCode: NotRequired[str],
    rateCards: NotRequired[list[UsageBasedRateCardItemTypeDef]],  # (1)
```

1. See `list[UsageBasedRateCardItemTypeDef]`

## ConfigurableUpfrontPricingTermTypeDef

```python
# ConfigurableUpfrontPricingTermTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import ConfigurableUpfrontPricingTermTypeDef


def get_value() -> ConfigurableUpfrontPricingTermTypeDef:
    return {
        "type": ...,
    }


# ConfigurableUpfrontPricingTermTypeDef definition

class ConfigurableUpfrontPricingTermTypeDef(TypedDict):
    type: NotRequired[str],
    currencyCode: NotRequired[str],
    rateCards: NotRequired[list[ConfigurableUpfrontRateCardItemTypeDef]],  # (1)
    configuration: NotRequired[ConfigurableUpfrontPricingTermConfigurationTypeDef],  # (2)
```

1. See `list[ConfigurableUpfrontRateCardItemTypeDef]`
2. See [:material-code-braces: ConfigurableUpfrontPricingTermConfigurationTypeDef](./type_defs.md#configurableupfrontpricingtermconfigurationtypedef)

## AgreementViewSummaryTypeDef

```python
# AgreementViewSummaryTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import AgreementViewSummaryTypeDef


def get_value() -> AgreementViewSummaryTypeDef:
    return {
        "agreementId": ...,
    }


# AgreementViewSummaryTypeDef definition

class AgreementViewSummaryTypeDef(TypedDict):
    agreementId: NotRequired[str],
    acceptanceTime: NotRequired[datetime.datetime],
    startTime: NotRequired[datetime.datetime],
    endTime: NotRequired[datetime.datetime],
    agreementType: NotRequired[str],
    acceptor: NotRequired[AcceptorTypeDef],  # (1)
    proposer: NotRequired[ProposerTypeDef],  # (2)
    proposalSummary: NotRequired[ProposalSummaryTypeDef],  # (3)
    status: NotRequired[AgreementStatusType],  # (4)
```

1. See [:material-code-braces: AcceptorTypeDef](./type_defs.md#acceptortypedef)
2. See [:material-code-braces: ProposerTypeDef](./type_defs.md#proposertypedef)
3. See [:material-code-braces: ProposalSummaryTypeDef](./type_defs.md#proposalsummarytypedef)
4. See [:material-code-brackets: AgreementStatusType](./literals.md#agreementstatustype)

## DescribeAgreementOutputTypeDef

```python
# DescribeAgreementOutputTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import DescribeAgreementOutputTypeDef


def get_value() -> DescribeAgreementOutputTypeDef:
    return {
        "agreementId": ...,
    }


# DescribeAgreementOutputTypeDef definition

class DescribeAgreementOutputTypeDef(TypedDict):
    agreementId: str,
    acceptor: AcceptorTypeDef,  # (1)
    proposer: ProposerTypeDef,  # (2)
    startTime: datetime.datetime,
    endTime: datetime.datetime,
    acceptanceTime: datetime.datetime,
    agreementType: str,
    estimatedCharges: EstimatedChargesTypeDef,  # (3)
    proposalSummary: ProposalSummaryTypeDef,  # (4)
    status: AgreementStatusType,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: AcceptorTypeDef](./type_defs.md#acceptortypedef)
2. See [:material-code-braces: ProposerTypeDef](./type_defs.md#proposertypedef)
3. See [:material-code-braces: EstimatedChargesTypeDef](./type_defs.md#estimatedchargestypedef)
4. See [:material-code-braces: ProposalSummaryTypeDef](./type_defs.md#proposalsummarytypedef)
5. See [:material-code-brackets: AgreementStatusType](./literals.md#agreementstatustype)
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## AcceptedTermTypeDef

```python
# AcceptedTermTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import AcceptedTermTypeDef


def get_value() -> AcceptedTermTypeDef:
    return {
        "legalTerm": ...,
    }


# AcceptedTermTypeDef definition

class AcceptedTermTypeDef(TypedDict):
    legalTerm: NotRequired[LegalTermTypeDef],  # (1)
    supportTerm: NotRequired[SupportTermTypeDef],  # (2)
    renewalTerm: NotRequired[RenewalTermTypeDef],  # (3)
    usageBasedPricingTerm: NotRequired[UsageBasedPricingTermTypeDef],  # (4)
    configurableUpfrontPricingTerm: NotRequired[ConfigurableUpfrontPricingTermTypeDef],  # (5)
    byolPricingTerm: NotRequired[ByolPricingTermTypeDef],  # (6)
    recurringPaymentTerm: NotRequired[RecurringPaymentTermTypeDef],  # (7)
    validityTerm: NotRequired[ValidityTermTypeDef],  # (8)
    paymentScheduleTerm: NotRequired[PaymentScheduleTermTypeDef],  # (9)
    freeTrialPricingTerm: NotRequired[FreeTrialPricingTermTypeDef],  # (10)
    fixedUpfrontPricingTerm: NotRequired[FixedUpfrontPricingTermTypeDef],  # (11)
    variablePaymentTerm: NotRequired[VariablePaymentTermTypeDef],  # (12)
```

1. See [:material-code-braces: LegalTermTypeDef](./type_defs.md#legaltermtypedef)
2. See [:material-code-braces: SupportTermTypeDef](./type_defs.md#supporttermtypedef)
3. See [:material-code-braces: RenewalTermTypeDef](./type_defs.md#renewaltermtypedef)
4. See [:material-code-braces: UsageBasedPricingTermTypeDef](./type_defs.md#usagebasedpricingtermtypedef)
5. See [:material-code-braces: ConfigurableUpfrontPricingTermTypeDef](./type_defs.md#configurableupfrontpricingtermtypedef)
6. See [:material-code-braces: ByolPricingTermTypeDef](./type_defs.md#byolpricingtermtypedef)
7. See [:material-code-braces: RecurringPaymentTermTypeDef](./type_defs.md#recurringpaymenttermtypedef)
8. See [:material-code-braces: ValidityTermTypeDef](./type_defs.md#validitytermtypedef)
9. See [:material-code-braces: PaymentScheduleTermTypeDef](./type_defs.md#paymentscheduletermtypedef)
10. See [:material-code-braces: FreeTrialPricingTermTypeDef](./type_defs.md#freetrialpricingtermtypedef)
11. See [:material-code-braces: FixedUpfrontPricingTermTypeDef](./type_defs.md#fixedupfrontpricingtermtypedef)
12. See [:material-code-braces: VariablePaymentTermTypeDef](./type_defs.md#variablepaymenttermtypedef)

## SearchAgreementsOutputTypeDef

```python
# SearchAgreementsOutputTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import SearchAgreementsOutputTypeDef


def get_value() -> SearchAgreementsOutputTypeDef:
    return {
        "agreementViewSummaries": ...,
    }


# SearchAgreementsOutputTypeDef definition

class SearchAgreementsOutputTypeDef(TypedDict):
    agreementViewSummaries: list[AgreementViewSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[AgreementViewSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetAgreementTermsOutputTypeDef

```python
# GetAgreementTermsOutputTypeDef TypedDict usage example

from types_aiobotocore_marketplace_agreement.type_defs import GetAgreementTermsOutputTypeDef


def get_value() -> GetAgreementTermsOutputTypeDef:
    return {
        "acceptedTerms": ...,
    }


# GetAgreementTermsOutputTypeDef definition

class GetAgreementTermsOutputTypeDef(TypedDict):
    acceptedTerms: list[AcceptedTermTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[AcceptedTermTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

