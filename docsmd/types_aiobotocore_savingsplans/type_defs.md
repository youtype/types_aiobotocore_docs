# Type definitions

> [Index](../README.md) > [SavingsPlans](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SavingsPlans](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans)
    type annotations stubs module [types-aiobotocore-savingsplans](https://pypi.org/project/types-aiobotocore-savingsplans/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
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

## DeleteQueuedSavingsPlanRequestRequestTypeDef

```python
# DeleteQueuedSavingsPlanRequestRequestTypeDef definition

class DeleteQueuedSavingsPlanRequestRequestTypeDef(TypedDict):
    savingsPlanId: str,
```

## SavingsPlanRateFilterTypeDef

```python
# SavingsPlanRateFilterTypeDef definition

class SavingsPlanRateFilterTypeDef(TypedDict):
    name: NotRequired[SavingsPlanRateFilterNameType],  # (1)
    values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: SavingsPlanRateFilterNameType](./literals.md#savingsplanratefilternametype) 
## SavingsPlanOfferingRateFilterElementTypeDef

```python
# SavingsPlanOfferingRateFilterElementTypeDef definition

class SavingsPlanOfferingRateFilterElementTypeDef(TypedDict):
    name: NotRequired[SavingsPlanRateFilterAttributeType],  # (1)
    values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: SavingsPlanRateFilterAttributeType](./literals.md#savingsplanratefilterattributetype) 
## SavingsPlanOfferingFilterElementTypeDef

```python
# SavingsPlanOfferingFilterElementTypeDef definition

class SavingsPlanOfferingFilterElementTypeDef(TypedDict):
    name: NotRequired[SavingsPlanOfferingFilterAttributeType],  # (1)
    values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: SavingsPlanOfferingFilterAttributeType](./literals.md#savingsplanofferingfilterattributetype) 
## SavingsPlanFilterTypeDef

```python
# SavingsPlanFilterTypeDef definition

class SavingsPlanFilterTypeDef(TypedDict):
    name: NotRequired[SavingsPlansFilterNameType],  # (1)
    values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: SavingsPlansFilterNameType](./literals.md#savingsplansfilternametype) 
## SavingsPlanTypeDef

```python
# SavingsPlanTypeDef definition

class SavingsPlanTypeDef(TypedDict):
    offeringId: NotRequired[str],
    savingsPlanId: NotRequired[str],
    savingsPlanArn: NotRequired[str],
    description: NotRequired[str],
    start: NotRequired[str],
    end: NotRequired[str],
    state: NotRequired[SavingsPlanStateType],  # (1)
    region: NotRequired[str],
    ec2InstanceFamily: NotRequired[str],
    savingsPlanType: NotRequired[SavingsPlanTypeType],  # (2)
    paymentOption: NotRequired[SavingsPlanPaymentOptionType],  # (3)
    productTypes: NotRequired[List[SavingsPlanProductTypeType]],  # (4)
    currency: NotRequired[CurrencyCodeType],  # (5)
    commitment: NotRequired[str],
    upfrontPaymentAmount: NotRequired[str],
    recurringPaymentAmount: NotRequired[str],
    termDurationInSeconds: NotRequired[int],
    tags: NotRequired[Dict[str, str]],
    returnableUntil: NotRequired[str],
```

1. See [:material-code-brackets: SavingsPlanStateType](./literals.md#savingsplanstatetype) 
2. See [:material-code-brackets: SavingsPlanTypeType](./literals.md#savingsplantypetype) 
3. See [:material-code-brackets: SavingsPlanPaymentOptionType](./literals.md#savingsplanpaymentoptiontype) 
4. See [:material-code-brackets: SavingsPlanProductTypeType](./literals.md#savingsplanproducttypetype) 
5. See [:material-code-brackets: CurrencyCodeType](./literals.md#currencycodetype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ParentSavingsPlanOfferingTypeDef

```python
# ParentSavingsPlanOfferingTypeDef definition

class ParentSavingsPlanOfferingTypeDef(TypedDict):
    offeringId: NotRequired[str],
    paymentOption: NotRequired[SavingsPlanPaymentOptionType],  # (1)
    planType: NotRequired[SavingsPlanTypeType],  # (2)
    durationSeconds: NotRequired[int],
    currency: NotRequired[CurrencyCodeType],  # (3)
    planDescription: NotRequired[str],
```

1. See [:material-code-brackets: SavingsPlanPaymentOptionType](./literals.md#savingsplanpaymentoptiontype) 
2. See [:material-code-brackets: SavingsPlanTypeType](./literals.md#savingsplantypetype) 
3. See [:material-code-brackets: CurrencyCodeType](./literals.md#currencycodetype) 
## ReturnSavingsPlanRequestRequestTypeDef

```python
# ReturnSavingsPlanRequestRequestTypeDef definition

class ReturnSavingsPlanRequestRequestTypeDef(TypedDict):
    savingsPlanId: str,
    clientToken: NotRequired[str],
```

## SavingsPlanOfferingPropertyTypeDef

```python
# SavingsPlanOfferingPropertyTypeDef definition

class SavingsPlanOfferingPropertyTypeDef(TypedDict):
    name: NotRequired[SavingsPlanOfferingPropertyKeyType],  # (1)
    value: NotRequired[str],
```

1. See [:material-code-brackets: SavingsPlanOfferingPropertyKeyType](./literals.md#savingsplanofferingpropertykeytype) 
## SavingsPlanOfferingRatePropertyTypeDef

```python
# SavingsPlanOfferingRatePropertyTypeDef definition

class SavingsPlanOfferingRatePropertyTypeDef(TypedDict):
    name: NotRequired[str],
    value: NotRequired[str],
```

## SavingsPlanRatePropertyTypeDef

```python
# SavingsPlanRatePropertyTypeDef definition

class SavingsPlanRatePropertyTypeDef(TypedDict):
    name: NotRequired[SavingsPlanRatePropertyKeyType],  # (1)
    value: NotRequired[str],
```

1. See [:material-code-brackets: SavingsPlanRatePropertyKeyType](./literals.md#savingsplanratepropertykeytype) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## CreateSavingsPlanRequestRequestTypeDef

```python
# CreateSavingsPlanRequestRequestTypeDef definition

class CreateSavingsPlanRequestRequestTypeDef(TypedDict):
    savingsPlanOfferingId: str,
    commitment: str,
    upfrontPaymentAmount: NotRequired[str],
    purchaseTime: NotRequired[TimestampTypeDef],
    clientToken: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## CreateSavingsPlanResponseTypeDef

```python
# CreateSavingsPlanResponseTypeDef definition

class CreateSavingsPlanResponseTypeDef(TypedDict):
    savingsPlanId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReturnSavingsPlanResponseTypeDef

```python
# ReturnSavingsPlanResponseTypeDef definition

class ReturnSavingsPlanResponseTypeDef(TypedDict):
    savingsPlanId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSavingsPlanRatesRequestRequestTypeDef

```python
# DescribeSavingsPlanRatesRequestRequestTypeDef definition

class DescribeSavingsPlanRatesRequestRequestTypeDef(TypedDict):
    savingsPlanId: str,
    filters: NotRequired[Sequence[SavingsPlanRateFilterTypeDef]],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-braces: SavingsPlanRateFilterTypeDef](./type_defs.md#savingsplanratefiltertypedef) 
## DescribeSavingsPlansOfferingRatesRequestRequestTypeDef

```python
# DescribeSavingsPlansOfferingRatesRequestRequestTypeDef definition

class DescribeSavingsPlansOfferingRatesRequestRequestTypeDef(TypedDict):
    savingsPlanOfferingIds: NotRequired[Sequence[str]],
    savingsPlanPaymentOptions: NotRequired[Sequence[SavingsPlanPaymentOptionType]],  # (1)
    savingsPlanTypes: NotRequired[Sequence[SavingsPlanTypeType]],  # (2)
    products: NotRequired[Sequence[SavingsPlanProductTypeType]],  # (3)
    serviceCodes: NotRequired[Sequence[SavingsPlanRateServiceCodeType]],  # (4)
    usageTypes: NotRequired[Sequence[str]],
    operations: NotRequired[Sequence[str]],
    filters: NotRequired[Sequence[SavingsPlanOfferingRateFilterElementTypeDef]],  # (5)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: SavingsPlanPaymentOptionType](./literals.md#savingsplanpaymentoptiontype) 
2. See [:material-code-brackets: SavingsPlanTypeType](./literals.md#savingsplantypetype) 
3. See [:material-code-brackets: SavingsPlanProductTypeType](./literals.md#savingsplanproducttypetype) 
4. See [:material-code-brackets: SavingsPlanRateServiceCodeType](./literals.md#savingsplanrateservicecodetype) 
5. See [:material-code-braces: SavingsPlanOfferingRateFilterElementTypeDef](./type_defs.md#savingsplanofferingratefilterelementtypedef) 
## DescribeSavingsPlansOfferingsRequestRequestTypeDef

```python
# DescribeSavingsPlansOfferingsRequestRequestTypeDef definition

class DescribeSavingsPlansOfferingsRequestRequestTypeDef(TypedDict):
    offeringIds: NotRequired[Sequence[str]],
    paymentOptions: NotRequired[Sequence[SavingsPlanPaymentOptionType]],  # (1)
    productType: NotRequired[SavingsPlanProductTypeType],  # (2)
    planTypes: NotRequired[Sequence[SavingsPlanTypeType]],  # (3)
    durations: NotRequired[Sequence[int]],
    currencies: NotRequired[Sequence[CurrencyCodeType]],  # (4)
    descriptions: NotRequired[Sequence[str]],
    serviceCodes: NotRequired[Sequence[str]],
    usageTypes: NotRequired[Sequence[str]],
    operations: NotRequired[Sequence[str]],
    filters: NotRequired[Sequence[SavingsPlanOfferingFilterElementTypeDef]],  # (5)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: SavingsPlanPaymentOptionType](./literals.md#savingsplanpaymentoptiontype) 
2. See [:material-code-brackets: SavingsPlanProductTypeType](./literals.md#savingsplanproducttypetype) 
3. See [:material-code-brackets: SavingsPlanTypeType](./literals.md#savingsplantypetype) 
4. See [:material-code-brackets: CurrencyCodeType](./literals.md#currencycodetype) 
5. See [:material-code-braces: SavingsPlanOfferingFilterElementTypeDef](./type_defs.md#savingsplanofferingfilterelementtypedef) 
## DescribeSavingsPlansRequestRequestTypeDef

```python
# DescribeSavingsPlansRequestRequestTypeDef definition

class DescribeSavingsPlansRequestRequestTypeDef(TypedDict):
    savingsPlanArns: NotRequired[Sequence[str]],
    savingsPlanIds: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    states: NotRequired[Sequence[SavingsPlanStateType]],  # (1)
    filters: NotRequired[Sequence[SavingsPlanFilterTypeDef]],  # (2)
```

1. See [:material-code-brackets: SavingsPlanStateType](./literals.md#savingsplanstatetype) 
2. See [:material-code-braces: SavingsPlanFilterTypeDef](./type_defs.md#savingsplanfiltertypedef) 
## DescribeSavingsPlansResponseTypeDef

```python
# DescribeSavingsPlansResponseTypeDef definition

class DescribeSavingsPlansResponseTypeDef(TypedDict):
    savingsPlans: List[SavingsPlanTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SavingsPlanTypeDef](./type_defs.md#savingsplantypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SavingsPlanOfferingTypeDef

```python
# SavingsPlanOfferingTypeDef definition

class SavingsPlanOfferingTypeDef(TypedDict):
    offeringId: NotRequired[str],
    productTypes: NotRequired[List[SavingsPlanProductTypeType]],  # (1)
    planType: NotRequired[SavingsPlanTypeType],  # (2)
    description: NotRequired[str],
    paymentOption: NotRequired[SavingsPlanPaymentOptionType],  # (3)
    durationSeconds: NotRequired[int],
    currency: NotRequired[CurrencyCodeType],  # (4)
    serviceCode: NotRequired[str],
    usageType: NotRequired[str],
    operation: NotRequired[str],
    properties: NotRequired[List[SavingsPlanOfferingPropertyTypeDef]],  # (5)
```

1. See [:material-code-brackets: SavingsPlanProductTypeType](./literals.md#savingsplanproducttypetype) 
2. See [:material-code-brackets: SavingsPlanTypeType](./literals.md#savingsplantypetype) 
3. See [:material-code-brackets: SavingsPlanPaymentOptionType](./literals.md#savingsplanpaymentoptiontype) 
4. See [:material-code-brackets: CurrencyCodeType](./literals.md#currencycodetype) 
5. See [:material-code-braces: SavingsPlanOfferingPropertyTypeDef](./type_defs.md#savingsplanofferingpropertytypedef) 
## SavingsPlanOfferingRateTypeDef

```python
# SavingsPlanOfferingRateTypeDef definition

class SavingsPlanOfferingRateTypeDef(TypedDict):
    savingsPlanOffering: NotRequired[ParentSavingsPlanOfferingTypeDef],  # (1)
    rate: NotRequired[str],
    unit: NotRequired[SavingsPlanRateUnitType],  # (2)
    productType: NotRequired[SavingsPlanProductTypeType],  # (3)
    serviceCode: NotRequired[SavingsPlanRateServiceCodeType],  # (4)
    usageType: NotRequired[str],
    operation: NotRequired[str],
    properties: NotRequired[List[SavingsPlanOfferingRatePropertyTypeDef]],  # (5)
```

1. See [:material-code-braces: ParentSavingsPlanOfferingTypeDef](./type_defs.md#parentsavingsplanofferingtypedef) 
2. See [:material-code-brackets: SavingsPlanRateUnitType](./literals.md#savingsplanrateunittype) 
3. See [:material-code-brackets: SavingsPlanProductTypeType](./literals.md#savingsplanproducttypetype) 
4. See [:material-code-brackets: SavingsPlanRateServiceCodeType](./literals.md#savingsplanrateservicecodetype) 
5. See [:material-code-braces: SavingsPlanOfferingRatePropertyTypeDef](./type_defs.md#savingsplanofferingratepropertytypedef) 
## SavingsPlanRateTypeDef

```python
# SavingsPlanRateTypeDef definition

class SavingsPlanRateTypeDef(TypedDict):
    rate: NotRequired[str],
    currency: NotRequired[CurrencyCodeType],  # (1)
    unit: NotRequired[SavingsPlanRateUnitType],  # (2)
    productType: NotRequired[SavingsPlanProductTypeType],  # (3)
    serviceCode: NotRequired[SavingsPlanRateServiceCodeType],  # (4)
    usageType: NotRequired[str],
    operation: NotRequired[str],
    properties: NotRequired[List[SavingsPlanRatePropertyTypeDef]],  # (5)
```

1. See [:material-code-brackets: CurrencyCodeType](./literals.md#currencycodetype) 
2. See [:material-code-brackets: SavingsPlanRateUnitType](./literals.md#savingsplanrateunittype) 
3. See [:material-code-brackets: SavingsPlanProductTypeType](./literals.md#savingsplanproducttypetype) 
4. See [:material-code-brackets: SavingsPlanRateServiceCodeType](./literals.md#savingsplanrateservicecodetype) 
5. See [:material-code-braces: SavingsPlanRatePropertyTypeDef](./type_defs.md#savingsplanratepropertytypedef) 
## DescribeSavingsPlansOfferingsResponseTypeDef

```python
# DescribeSavingsPlansOfferingsResponseTypeDef definition

class DescribeSavingsPlansOfferingsResponseTypeDef(TypedDict):
    searchResults: List[SavingsPlanOfferingTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SavingsPlanOfferingTypeDef](./type_defs.md#savingsplanofferingtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSavingsPlansOfferingRatesResponseTypeDef

```python
# DescribeSavingsPlansOfferingRatesResponseTypeDef definition

class DescribeSavingsPlansOfferingRatesResponseTypeDef(TypedDict):
    searchResults: List[SavingsPlanOfferingRateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SavingsPlanOfferingRateTypeDef](./type_defs.md#savingsplanofferingratetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSavingsPlanRatesResponseTypeDef

```python
# DescribeSavingsPlanRatesResponseTypeDef definition

class DescribeSavingsPlanRatesResponseTypeDef(TypedDict):
    savingsPlanId: str,
    searchResults: List[SavingsPlanRateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SavingsPlanRateTypeDef](./type_defs.md#savingsplanratetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
