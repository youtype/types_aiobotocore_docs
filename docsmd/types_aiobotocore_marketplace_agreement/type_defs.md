# Type definitions

> [Index](../README.md) > [AgreementService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [AgreementService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-agreement.html#agreementservice)
    type annotations stubs module [types-aiobotocore-marketplace-agreement](https://pypi.org/project/types-aiobotocore-marketplace-agreement/).



## ByolPricingTermTypeDef

```python
# ByolPricingTermTypeDef definition

class ByolPricingTermTypeDef(TypedDict):
    type: NotRequired[str],
```

## RecurringPaymentTermTypeDef

```python
# RecurringPaymentTermTypeDef definition

class RecurringPaymentTermTypeDef(TypedDict):
    billingPeriod: NotRequired[str],
    currencyCode: NotRequired[str],
    price: NotRequired[str],
    type: NotRequired[str],
```

## SupportTermTypeDef

```python
# SupportTermTypeDef definition

class SupportTermTypeDef(TypedDict):
    refundPolicy: NotRequired[str],
    type: NotRequired[str],
```

## ValidityTermTypeDef

```python
# ValidityTermTypeDef definition

class ValidityTermTypeDef(TypedDict):
    agreementDuration: NotRequired[str],
    agreementEndDate: NotRequired[datetime],
    agreementStartDate: NotRequired[datetime],
    type: NotRequired[str],
```

## AcceptorTypeDef

```python
# AcceptorTypeDef definition

class AcceptorTypeDef(TypedDict):
    accountId: NotRequired[str],
```

## ProposerTypeDef

```python
# ProposerTypeDef definition

class ProposerTypeDef(TypedDict):
    accountId: NotRequired[str],
```

## DimensionTypeDef

```python
# DimensionTypeDef definition

class DimensionTypeDef(TypedDict):
    dimensionKey: str,
    dimensionValue: int,
```

## ConstraintsTypeDef

```python
# ConstraintsTypeDef definition

class ConstraintsTypeDef(TypedDict):
    multipleDimensionSelection: NotRequired[str],
    quantityConfiguration: NotRequired[str],
```

## RateCardItemTypeDef

```python
# RateCardItemTypeDef definition

class RateCardItemTypeDef(TypedDict):
    dimensionKey: NotRequired[str],
    price: NotRequired[str],
```

## SelectorTypeDef

```python
# SelectorTypeDef definition

class SelectorTypeDef(TypedDict):
    type: NotRequired[str],
    value: NotRequired[str],
```

## DescribeAgreementInputRequestTypeDef

```python
# DescribeAgreementInputRequestTypeDef definition

class DescribeAgreementInputRequestTypeDef(TypedDict):
    agreementId: str,
```

## EstimatedChargesTypeDef

```python
# EstimatedChargesTypeDef definition

class EstimatedChargesTypeDef(TypedDict):
    agreementValue: NotRequired[str],
    currencyCode: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## DocumentItemTypeDef

```python
# DocumentItemTypeDef definition

class DocumentItemTypeDef(TypedDict):
    type: NotRequired[str],
    url: NotRequired[str],
    version: NotRequired[str],
```

## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    name: NotRequired[str],
    values: NotRequired[Sequence[str]],
```

## GrantItemTypeDef

```python
# GrantItemTypeDef definition

class GrantItemTypeDef(TypedDict):
    dimensionKey: NotRequired[str],
    maxQuantity: NotRequired[int],
```

## GetAgreementTermsInputRequestTypeDef

```python
# GetAgreementTermsInputRequestTypeDef definition

class GetAgreementTermsInputRequestTypeDef(TypedDict):
    agreementId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ScheduleItemTypeDef

```python
# ScheduleItemTypeDef definition

class ScheduleItemTypeDef(TypedDict):
    chargeAmount: NotRequired[str],
    chargeDate: NotRequired[datetime],
```

## ResourceTypeDef

```python
# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    id: NotRequired[str],
    type: NotRequired[str],
```

## RenewalTermConfigurationTypeDef

```python
# RenewalTermConfigurationTypeDef definition

class RenewalTermConfigurationTypeDef(TypedDict):
    enableAutoRenew: bool,
```

## SortTypeDef

```python
# SortTypeDef definition

class SortTypeDef(TypedDict):
    sortBy: NotRequired[str],
    sortOrder: NotRequired[SortOrderType],  # (1)
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ConfigurableUpfrontPricingTermConfigurationTypeDef

```python
# ConfigurableUpfrontPricingTermConfigurationTypeDef definition

class ConfigurableUpfrontPricingTermConfigurationTypeDef(TypedDict):
    dimensions: List[DimensionTypeDef],  # (1)
    selectorValue: str,
```

1. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
## UsageBasedRateCardItemTypeDef

```python
# UsageBasedRateCardItemTypeDef definition

class UsageBasedRateCardItemTypeDef(TypedDict):
    rateCard: NotRequired[List[RateCardItemTypeDef]],  # (1)
```

1. See [:material-code-braces: RateCardItemTypeDef](./type_defs.md#ratecarditemtypedef) 
## ConfigurableUpfrontRateCardItemTypeDef

```python
# ConfigurableUpfrontRateCardItemTypeDef definition

class ConfigurableUpfrontRateCardItemTypeDef(TypedDict):
    constraints: NotRequired[ConstraintsTypeDef],  # (1)
    rateCard: NotRequired[List[RateCardItemTypeDef]],  # (2)
    selector: NotRequired[SelectorTypeDef],  # (3)
```

1. See [:material-code-braces: ConstraintsTypeDef](./type_defs.md#constraintstypedef) 
2. See [:material-code-braces: RateCardItemTypeDef](./type_defs.md#ratecarditemtypedef) 
3. See [:material-code-braces: SelectorTypeDef](./type_defs.md#selectortypedef) 
## LegalTermTypeDef

```python
# LegalTermTypeDef definition

class LegalTermTypeDef(TypedDict):
    documents: NotRequired[List[DocumentItemTypeDef]],  # (1)
    type: NotRequired[str],
```

1. See [:material-code-braces: DocumentItemTypeDef](./type_defs.md#documentitemtypedef) 
## FixedUpfrontPricingTermTypeDef

```python
# FixedUpfrontPricingTermTypeDef definition

class FixedUpfrontPricingTermTypeDef(TypedDict):
    currencyCode: NotRequired[str],
    duration: NotRequired[str],
    grants: NotRequired[List[GrantItemTypeDef]],  # (1)
    price: NotRequired[str],
    type: NotRequired[str],
```

1. See [:material-code-braces: GrantItemTypeDef](./type_defs.md#grantitemtypedef) 
## FreeTrialPricingTermTypeDef

```python
# FreeTrialPricingTermTypeDef definition

class FreeTrialPricingTermTypeDef(TypedDict):
    duration: NotRequired[str],
    grants: NotRequired[List[GrantItemTypeDef]],  # (1)
    type: NotRequired[str],
```

1. See [:material-code-braces: GrantItemTypeDef](./type_defs.md#grantitemtypedef) 
## PaymentScheduleTermTypeDef

```python
# PaymentScheduleTermTypeDef definition

class PaymentScheduleTermTypeDef(TypedDict):
    currencyCode: NotRequired[str],
    schedule: NotRequired[List[ScheduleItemTypeDef]],  # (1)
    type: NotRequired[str],
```

1. See [:material-code-braces: ScheduleItemTypeDef](./type_defs.md#scheduleitemtypedef) 
## ProposalSummaryTypeDef

```python
# ProposalSummaryTypeDef definition

class ProposalSummaryTypeDef(TypedDict):
    offerId: NotRequired[str],
    resources: NotRequired[List[ResourceTypeDef]],  # (1)
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
## RenewalTermTypeDef

```python
# RenewalTermTypeDef definition

class RenewalTermTypeDef(TypedDict):
    configuration: NotRequired[RenewalTermConfigurationTypeDef],  # (1)
    type: NotRequired[str],
```

1. See [:material-code-braces: RenewalTermConfigurationTypeDef](./type_defs.md#renewaltermconfigurationtypedef) 
## SearchAgreementsInputRequestTypeDef

```python
# SearchAgreementsInputRequestTypeDef definition

class SearchAgreementsInputRequestTypeDef(TypedDict):
    catalog: NotRequired[str],
    filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    sort: NotRequired[SortTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
## UsageBasedPricingTermTypeDef

```python
# UsageBasedPricingTermTypeDef definition

class UsageBasedPricingTermTypeDef(TypedDict):
    currencyCode: NotRequired[str],
    rateCards: NotRequired[List[UsageBasedRateCardItemTypeDef]],  # (1)
    type: NotRequired[str],
```

1. See [:material-code-braces: UsageBasedRateCardItemTypeDef](./type_defs.md#usagebasedratecarditemtypedef) 
## ConfigurableUpfrontPricingTermTypeDef

```python
# ConfigurableUpfrontPricingTermTypeDef definition

class ConfigurableUpfrontPricingTermTypeDef(TypedDict):
    configuration: NotRequired[ConfigurableUpfrontPricingTermConfigurationTypeDef],  # (1)
    currencyCode: NotRequired[str],
    rateCards: NotRequired[List[ConfigurableUpfrontRateCardItemTypeDef]],  # (2)
    type: NotRequired[str],
```

1. See [:material-code-braces: ConfigurableUpfrontPricingTermConfigurationTypeDef](./type_defs.md#configurableupfrontpricingtermconfigurationtypedef) 
2. See [:material-code-braces: ConfigurableUpfrontRateCardItemTypeDef](./type_defs.md#configurableupfrontratecarditemtypedef) 
## AgreementViewSummaryTypeDef

```python
# AgreementViewSummaryTypeDef definition

class AgreementViewSummaryTypeDef(TypedDict):
    acceptanceTime: NotRequired[datetime],
    acceptor: NotRequired[AcceptorTypeDef],  # (1)
    agreementId: NotRequired[str],
    agreementType: NotRequired[str],
    endTime: NotRequired[datetime],
    proposalSummary: NotRequired[ProposalSummaryTypeDef],  # (2)
    proposer: NotRequired[ProposerTypeDef],  # (3)
    startTime: NotRequired[datetime],
    status: NotRequired[AgreementStatusType],  # (4)
```

1. See [:material-code-braces: AcceptorTypeDef](./type_defs.md#acceptortypedef) 
2. See [:material-code-braces: ProposalSummaryTypeDef](./type_defs.md#proposalsummarytypedef) 
3. See [:material-code-braces: ProposerTypeDef](./type_defs.md#proposertypedef) 
4. See [:material-code-brackets: AgreementStatusType](./literals.md#agreementstatustype) 
## DescribeAgreementOutputTypeDef

```python
# DescribeAgreementOutputTypeDef definition

class DescribeAgreementOutputTypeDef(TypedDict):
    acceptanceTime: datetime,
    acceptor: AcceptorTypeDef,  # (1)
    agreementId: str,
    agreementType: str,
    endTime: datetime,
    estimatedCharges: EstimatedChargesTypeDef,  # (2)
    proposalSummary: ProposalSummaryTypeDef,  # (3)
    proposer: ProposerTypeDef,  # (4)
    startTime: datetime,
    status: AgreementStatusType,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: AcceptorTypeDef](./type_defs.md#acceptortypedef) 
2. See [:material-code-braces: EstimatedChargesTypeDef](./type_defs.md#estimatedchargestypedef) 
3. See [:material-code-braces: ProposalSummaryTypeDef](./type_defs.md#proposalsummarytypedef) 
4. See [:material-code-braces: ProposerTypeDef](./type_defs.md#proposertypedef) 
5. See [:material-code-brackets: AgreementStatusType](./literals.md#agreementstatustype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AcceptedTermTypeDef

```python
# AcceptedTermTypeDef definition

class AcceptedTermTypeDef(TypedDict):
    byolPricingTerm: NotRequired[ByolPricingTermTypeDef],  # (1)
    configurableUpfrontPricingTerm: NotRequired[ConfigurableUpfrontPricingTermTypeDef],  # (2)
    fixedUpfrontPricingTerm: NotRequired[FixedUpfrontPricingTermTypeDef],  # (3)
    freeTrialPricingTerm: NotRequired[FreeTrialPricingTermTypeDef],  # (4)
    legalTerm: NotRequired[LegalTermTypeDef],  # (5)
    paymentScheduleTerm: NotRequired[PaymentScheduleTermTypeDef],  # (6)
    recurringPaymentTerm: NotRequired[RecurringPaymentTermTypeDef],  # (7)
    renewalTerm: NotRequired[RenewalTermTypeDef],  # (8)
    supportTerm: NotRequired[SupportTermTypeDef],  # (9)
    usageBasedPricingTerm: NotRequired[UsageBasedPricingTermTypeDef],  # (10)
    validityTerm: NotRequired[ValidityTermTypeDef],  # (11)
```

1. See [:material-code-braces: ByolPricingTermTypeDef](./type_defs.md#byolpricingtermtypedef) 
2. See [:material-code-braces: ConfigurableUpfrontPricingTermTypeDef](./type_defs.md#configurableupfrontpricingtermtypedef) 
3. See [:material-code-braces: FixedUpfrontPricingTermTypeDef](./type_defs.md#fixedupfrontpricingtermtypedef) 
4. See [:material-code-braces: FreeTrialPricingTermTypeDef](./type_defs.md#freetrialpricingtermtypedef) 
5. See [:material-code-braces: LegalTermTypeDef](./type_defs.md#legaltermtypedef) 
6. See [:material-code-braces: PaymentScheduleTermTypeDef](./type_defs.md#paymentscheduletermtypedef) 
7. See [:material-code-braces: RecurringPaymentTermTypeDef](./type_defs.md#recurringpaymenttermtypedef) 
8. See [:material-code-braces: RenewalTermTypeDef](./type_defs.md#renewaltermtypedef) 
9. See [:material-code-braces: SupportTermTypeDef](./type_defs.md#supporttermtypedef) 
10. See [:material-code-braces: UsageBasedPricingTermTypeDef](./type_defs.md#usagebasedpricingtermtypedef) 
11. See [:material-code-braces: ValidityTermTypeDef](./type_defs.md#validitytermtypedef) 
## SearchAgreementsOutputTypeDef

```python
# SearchAgreementsOutputTypeDef definition

class SearchAgreementsOutputTypeDef(TypedDict):
    agreementViewSummaries: List[AgreementViewSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AgreementViewSummaryTypeDef](./type_defs.md#agreementviewsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAgreementTermsOutputTypeDef

```python
# GetAgreementTermsOutputTypeDef definition

class GetAgreementTermsOutputTypeDef(TypedDict):
    acceptedTerms: List[AcceptedTermTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AcceptedTermTypeDef](./type_defs.md#acceptedtermtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
