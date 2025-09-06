# Type definitions

> [Index](../README.md) > [Invoicing](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Invoicing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/invoicing.html#invoicing)
    type annotations stubs module [types-aiobotocore-invoicing](https://pypi.org/project/types-aiobotocore-invoicing/).

## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_invoicing.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime.datetime,
    str,
]
```


## InvoiceUnitRuleUnionTypeDef

```python
# InvoiceUnitRuleUnionTypeDef Union usage example

from types_aiobotocore_invoicing.type_defs import InvoiceUnitRuleUnionTypeDef


def get_value() -> InvoiceUnitRuleUnionTypeDef:
    return ...


# InvoiceUnitRuleUnionTypeDef definition

InvoiceUnitRuleUnionTypeDef = Union[
    InvoiceUnitRuleTypeDef,  # (1)
    InvoiceUnitRuleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: InvoiceUnitRuleTypeDef](./type_defs.md#invoiceunitruletypedef)
2. See [:material-code-braces: InvoiceUnitRuleOutputTypeDef](./type_defs.md#invoiceunitruleoutputtypedef)



## BatchGetInvoiceProfileRequestTypeDef

```python
# BatchGetInvoiceProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import BatchGetInvoiceProfileRequestTypeDef


def get_value() -> BatchGetInvoiceProfileRequestTypeDef:
    return {
        "AccountIds": ...,
    }


# BatchGetInvoiceProfileRequestTypeDef definition

class BatchGetInvoiceProfileRequestTypeDef(TypedDict):
    AccountIds: Sequence[str],
```


## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```


## BillingPeriodTypeDef

```python
# BillingPeriodTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import BillingPeriodTypeDef


def get_value() -> BillingPeriodTypeDef:
    return {
        "Month": ...,
    }


# BillingPeriodTypeDef definition

class BillingPeriodTypeDef(TypedDict):
    Month: int,
    Year: int,
```


## ResourceTagTypeDef

```python
# ResourceTagTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import ResourceTagTypeDef


def get_value() -> ResourceTagTypeDef:
    return {
        "Key": ...,
    }


# ResourceTagTypeDef definition

class ResourceTagTypeDef(TypedDict):
    Key: str,
    Value: str,
```


## CurrencyExchangeDetailsTypeDef

```python
# CurrencyExchangeDetailsTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import CurrencyExchangeDetailsTypeDef


def get_value() -> CurrencyExchangeDetailsTypeDef:
    return {
        "SourceCurrencyCode": ...,
    }


# CurrencyExchangeDetailsTypeDef definition

class CurrencyExchangeDetailsTypeDef(TypedDict):
    SourceCurrencyCode: NotRequired[str],
    TargetCurrencyCode: NotRequired[str],
    Rate: NotRequired[str],
```


## DeleteInvoiceUnitRequestTypeDef

```python
# DeleteInvoiceUnitRequestTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import DeleteInvoiceUnitRequestTypeDef


def get_value() -> DeleteInvoiceUnitRequestTypeDef:
    return {
        "InvoiceUnitArn": ...,
    }


# DeleteInvoiceUnitRequestTypeDef definition

class DeleteInvoiceUnitRequestTypeDef(TypedDict):
    InvoiceUnitArn: str,
```


## DiscountsBreakdownAmountTypeDef

```python
# DiscountsBreakdownAmountTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import DiscountsBreakdownAmountTypeDef


def get_value() -> DiscountsBreakdownAmountTypeDef:
    return {
        "Description": ...,
    }


# DiscountsBreakdownAmountTypeDef definition

class DiscountsBreakdownAmountTypeDef(TypedDict):
    Description: NotRequired[str],
    Amount: NotRequired[str],
    Rate: NotRequired[str],
```


## EntityTypeDef

```python
# EntityTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import EntityTypeDef


def get_value() -> EntityTypeDef:
    return {
        "InvoicingEntity": ...,
    }


# EntityTypeDef definition

class EntityTypeDef(TypedDict):
    InvoicingEntity: NotRequired[str],
```


## FeesBreakdownAmountTypeDef

```python
# FeesBreakdownAmountTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import FeesBreakdownAmountTypeDef


def get_value() -> FeesBreakdownAmountTypeDef:
    return {
        "Description": ...,
    }


# FeesBreakdownAmountTypeDef definition

class FeesBreakdownAmountTypeDef(TypedDict):
    Description: NotRequired[str],
    Amount: NotRequired[str],
    Rate: NotRequired[str],
```


## FiltersTypeDef

```python
# FiltersTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import FiltersTypeDef


def get_value() -> FiltersTypeDef:
    return {
        "Names": ...,
    }


# FiltersTypeDef definition

class FiltersTypeDef(TypedDict):
    Names: NotRequired[Sequence[str]],
    InvoiceReceivers: NotRequired[Sequence[str]],
    Accounts: NotRequired[Sequence[str]],
```


## InvoiceUnitRuleOutputTypeDef

```python
# InvoiceUnitRuleOutputTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import InvoiceUnitRuleOutputTypeDef


def get_value() -> InvoiceUnitRuleOutputTypeDef:
    return {
        "LinkedAccounts": ...,
    }


# InvoiceUnitRuleOutputTypeDef definition

class InvoiceUnitRuleOutputTypeDef(TypedDict):
    LinkedAccounts: NotRequired[List[str]],
```


## ReceiverAddressTypeDef

```python
# ReceiverAddressTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import ReceiverAddressTypeDef


def get_value() -> ReceiverAddressTypeDef:
    return {
        "AddressLine1": ...,
    }


# ReceiverAddressTypeDef definition

class ReceiverAddressTypeDef(TypedDict):
    AddressLine1: NotRequired[str],
    AddressLine2: NotRequired[str],
    AddressLine3: NotRequired[str],
    DistrictOrCounty: NotRequired[str],
    City: NotRequired[str],
    StateOrRegion: NotRequired[str],
    CountryCode: NotRequired[str],
    CompanyName: NotRequired[str],
    PostalCode: NotRequired[str],
```


## InvoiceSummariesSelectorTypeDef

```python
# InvoiceSummariesSelectorTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import InvoiceSummariesSelectorTypeDef


def get_value() -> InvoiceSummariesSelectorTypeDef:
    return {
        "ResourceType": ...,
    }


# InvoiceSummariesSelectorTypeDef definition

class InvoiceSummariesSelectorTypeDef(TypedDict):
    ResourceType: ListInvoiceSummariesResourceTypeType,  # (1)
    Value: str,
```

1. See [:material-code-brackets: ListInvoiceSummariesResourceTypeType](./literals.md#listinvoicesummariesresourcetypetype)

## InvoiceUnitRuleTypeDef

```python
# InvoiceUnitRuleTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import InvoiceUnitRuleTypeDef


def get_value() -> InvoiceUnitRuleTypeDef:
    return {
        "LinkedAccounts": ...,
    }


# InvoiceUnitRuleTypeDef definition

class InvoiceUnitRuleTypeDef(TypedDict):
    LinkedAccounts: NotRequired[Sequence[str]],
```


## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```


## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
```


## TaxesBreakdownAmountTypeDef

```python
# TaxesBreakdownAmountTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import TaxesBreakdownAmountTypeDef


def get_value() -> TaxesBreakdownAmountTypeDef:
    return {
        "Description": ...,
    }


# TaxesBreakdownAmountTypeDef definition

class TaxesBreakdownAmountTypeDef(TypedDict):
    Description: NotRequired[str],
    Amount: NotRequired[str],
    Rate: NotRequired[str],
```


## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    ResourceTagKeys: Sequence[str],
```


## CreateInvoiceUnitResponseTypeDef

```python
# CreateInvoiceUnitResponseTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import CreateInvoiceUnitResponseTypeDef


def get_value() -> CreateInvoiceUnitResponseTypeDef:
    return {
        "InvoiceUnitArn": ...,
    }


# CreateInvoiceUnitResponseTypeDef definition

class CreateInvoiceUnitResponseTypeDef(TypedDict):
    InvoiceUnitArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## DeleteInvoiceUnitResponseTypeDef

```python
# DeleteInvoiceUnitResponseTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import DeleteInvoiceUnitResponseTypeDef


def get_value() -> DeleteInvoiceUnitResponseTypeDef:
    return {
        "InvoiceUnitArn": ...,
    }


# DeleteInvoiceUnitResponseTypeDef definition

class DeleteInvoiceUnitResponseTypeDef(TypedDict):
    InvoiceUnitArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## UpdateInvoiceUnitResponseTypeDef

```python
# UpdateInvoiceUnitResponseTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import UpdateInvoiceUnitResponseTypeDef


def get_value() -> UpdateInvoiceUnitResponseTypeDef:
    return {
        "InvoiceUnitArn": ...,
    }


# UpdateInvoiceUnitResponseTypeDef definition

class UpdateInvoiceUnitResponseTypeDef(TypedDict):
    InvoiceUnitArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "ResourceTags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    ResourceTags: List[ResourceTagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See `List[ResourceTagTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    ResourceTags: Sequence[ResourceTagTypeDef],  # (1)
```

1. See `Sequence[ResourceTagTypeDef]`

## DateIntervalTypeDef

```python
# DateIntervalTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import DateIntervalTypeDef


def get_value() -> DateIntervalTypeDef:
    return {
        "StartDate": ...,
    }


# DateIntervalTypeDef definition

class DateIntervalTypeDef(TypedDict):
    StartDate: TimestampTypeDef,
    EndDate: TimestampTypeDef,
```


## GetInvoiceUnitRequestTypeDef

```python
# GetInvoiceUnitRequestTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import GetInvoiceUnitRequestTypeDef


def get_value() -> GetInvoiceUnitRequestTypeDef:
    return {
        "InvoiceUnitArn": ...,
    }


# GetInvoiceUnitRequestTypeDef definition

class GetInvoiceUnitRequestTypeDef(TypedDict):
    InvoiceUnitArn: str,
    AsOf: NotRequired[TimestampTypeDef],
```


## DiscountsBreakdownTypeDef

```python
# DiscountsBreakdownTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import DiscountsBreakdownTypeDef


def get_value() -> DiscountsBreakdownTypeDef:
    return {
        "Breakdown": ...,
    }


# DiscountsBreakdownTypeDef definition

class DiscountsBreakdownTypeDef(TypedDict):
    Breakdown: NotRequired[List[DiscountsBreakdownAmountTypeDef]],  # (1)
    TotalAmount: NotRequired[str],
```

1. See `List[DiscountsBreakdownAmountTypeDef]`

## FeesBreakdownTypeDef

```python
# FeesBreakdownTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import FeesBreakdownTypeDef


def get_value() -> FeesBreakdownTypeDef:
    return {
        "Breakdown": ...,
    }


# FeesBreakdownTypeDef definition

class FeesBreakdownTypeDef(TypedDict):
    Breakdown: NotRequired[List[FeesBreakdownAmountTypeDef]],  # (1)
    TotalAmount: NotRequired[str],
```

1. See `List[FeesBreakdownAmountTypeDef]`

## ListInvoiceUnitsRequestTypeDef

```python
# ListInvoiceUnitsRequestTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import ListInvoiceUnitsRequestTypeDef


def get_value() -> ListInvoiceUnitsRequestTypeDef:
    return {
        "Filters": ...,
    }


# ListInvoiceUnitsRequestTypeDef definition

class ListInvoiceUnitsRequestTypeDef(TypedDict):
    Filters: NotRequired[FiltersTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    AsOf: NotRequired[TimestampTypeDef],
```

1. See [:material-code-braces: FiltersTypeDef](./type_defs.md#filterstypedef)

## GetInvoiceUnitResponseTypeDef

```python
# GetInvoiceUnitResponseTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import GetInvoiceUnitResponseTypeDef


def get_value() -> GetInvoiceUnitResponseTypeDef:
    return {
        "InvoiceUnitArn": ...,
    }


# GetInvoiceUnitResponseTypeDef definition

class GetInvoiceUnitResponseTypeDef(TypedDict):
    InvoiceUnitArn: str,
    InvoiceReceiver: str,
    Name: str,
    Description: str,
    TaxInheritanceDisabled: bool,
    Rule: InvoiceUnitRuleOutputTypeDef,  # (1)
    LastModified: datetime.datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InvoiceUnitRuleOutputTypeDef](./type_defs.md#invoiceunitruleoutputtypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## InvoiceUnitTypeDef

```python
# InvoiceUnitTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import InvoiceUnitTypeDef


def get_value() -> InvoiceUnitTypeDef:
    return {
        "InvoiceUnitArn": ...,
    }


# InvoiceUnitTypeDef definition

class InvoiceUnitTypeDef(TypedDict):
    InvoiceUnitArn: NotRequired[str],
    InvoiceReceiver: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    TaxInheritanceDisabled: NotRequired[bool],
    Rule: NotRequired[InvoiceUnitRuleOutputTypeDef],  # (1)
    LastModified: NotRequired[datetime.datetime],
```

1. See [:material-code-braces: InvoiceUnitRuleOutputTypeDef](./type_defs.md#invoiceunitruleoutputtypedef)

## InvoiceProfileTypeDef

```python
# InvoiceProfileTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import InvoiceProfileTypeDef


def get_value() -> InvoiceProfileTypeDef:
    return {
        "AccountId": ...,
    }


# InvoiceProfileTypeDef definition

class InvoiceProfileTypeDef(TypedDict):
    AccountId: NotRequired[str],
    ReceiverName: NotRequired[str],
    ReceiverAddress: NotRequired[ReceiverAddressTypeDef],  # (1)
    ReceiverEmail: NotRequired[str],
    Issuer: NotRequired[str],
    TaxRegistrationNumber: NotRequired[str],
```

1. See [:material-code-braces: ReceiverAddressTypeDef](./type_defs.md#receiveraddresstypedef)

## ListInvoiceUnitsRequestPaginateTypeDef

```python
# ListInvoiceUnitsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import ListInvoiceUnitsRequestPaginateTypeDef


def get_value() -> ListInvoiceUnitsRequestPaginateTypeDef:
    return {
        "Filters": ...,
    }


# ListInvoiceUnitsRequestPaginateTypeDef definition

class ListInvoiceUnitsRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[FiltersTypeDef],  # (1)
    AsOf: NotRequired[TimestampTypeDef],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FiltersTypeDef](./type_defs.md#filterstypedef)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## TaxesBreakdownTypeDef

```python
# TaxesBreakdownTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import TaxesBreakdownTypeDef


def get_value() -> TaxesBreakdownTypeDef:
    return {
        "Breakdown": ...,
    }


# TaxesBreakdownTypeDef definition

class TaxesBreakdownTypeDef(TypedDict):
    Breakdown: NotRequired[List[TaxesBreakdownAmountTypeDef]],  # (1)
    TotalAmount: NotRequired[str],
```

1. See `List[TaxesBreakdownAmountTypeDef]`

## InvoiceSummariesFilterTypeDef

```python
# InvoiceSummariesFilterTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import InvoiceSummariesFilterTypeDef


def get_value() -> InvoiceSummariesFilterTypeDef:
    return {
        "TimeInterval": ...,
    }


# InvoiceSummariesFilterTypeDef definition

class InvoiceSummariesFilterTypeDef(TypedDict):
    TimeInterval: NotRequired[DateIntervalTypeDef],  # (1)
    BillingPeriod: NotRequired[BillingPeriodTypeDef],  # (2)
    InvoicingEntity: NotRequired[str],
```

1. See [:material-code-braces: DateIntervalTypeDef](./type_defs.md#dateintervaltypedef)
2. See [:material-code-braces: BillingPeriodTypeDef](./type_defs.md#billingperiodtypedef)

## ListInvoiceUnitsResponseTypeDef

```python
# ListInvoiceUnitsResponseTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import ListInvoiceUnitsResponseTypeDef


def get_value() -> ListInvoiceUnitsResponseTypeDef:
    return {
        "InvoiceUnits": ...,
    }


# ListInvoiceUnitsResponseTypeDef definition

class ListInvoiceUnitsResponseTypeDef(TypedDict):
    InvoiceUnits: List[InvoiceUnitTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See `List[InvoiceUnitTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## BatchGetInvoiceProfileResponseTypeDef

```python
# BatchGetInvoiceProfileResponseTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import BatchGetInvoiceProfileResponseTypeDef


def get_value() -> BatchGetInvoiceProfileResponseTypeDef:
    return {
        "Profiles": ...,
    }


# BatchGetInvoiceProfileResponseTypeDef definition

class BatchGetInvoiceProfileResponseTypeDef(TypedDict):
    Profiles: List[InvoiceProfileTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See `List[InvoiceProfileTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateInvoiceUnitRequestTypeDef

```python
# CreateInvoiceUnitRequestTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import CreateInvoiceUnitRequestTypeDef


def get_value() -> CreateInvoiceUnitRequestTypeDef:
    return {
        "Name": ...,
    }


# CreateInvoiceUnitRequestTypeDef definition

class CreateInvoiceUnitRequestTypeDef(TypedDict):
    Name: str,
    InvoiceReceiver: str,
    Rule: InvoiceUnitRuleUnionTypeDef,  # (1)
    Description: NotRequired[str],
    TaxInheritanceDisabled: NotRequired[bool],
    ResourceTags: NotRequired[Sequence[ResourceTagTypeDef]],  # (2)
```

1. See [:material-code-braces: InvoiceUnitRuleUnionTypeDef](#invoiceunitruleuniontypedef)
2. See `Sequence[ResourceTagTypeDef]`

## UpdateInvoiceUnitRequestTypeDef

```python
# UpdateInvoiceUnitRequestTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import UpdateInvoiceUnitRequestTypeDef


def get_value() -> UpdateInvoiceUnitRequestTypeDef:
    return {
        "InvoiceUnitArn": ...,
    }


# UpdateInvoiceUnitRequestTypeDef definition

class UpdateInvoiceUnitRequestTypeDef(TypedDict):
    InvoiceUnitArn: str,
    Description: NotRequired[str],
    TaxInheritanceDisabled: NotRequired[bool],
    Rule: NotRequired[InvoiceUnitRuleUnionTypeDef],  # (1)
```

1. See [:material-code-braces: InvoiceUnitRuleUnionTypeDef](#invoiceunitruleuniontypedef)

## AmountBreakdownTypeDef

```python
# AmountBreakdownTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import AmountBreakdownTypeDef


def get_value() -> AmountBreakdownTypeDef:
    return {
        "SubTotalAmount": ...,
    }


# AmountBreakdownTypeDef definition

class AmountBreakdownTypeDef(TypedDict):
    SubTotalAmount: NotRequired[str],
    Discounts: NotRequired[DiscountsBreakdownTypeDef],  # (1)
    Taxes: NotRequired[TaxesBreakdownTypeDef],  # (2)
    Fees: NotRequired[FeesBreakdownTypeDef],  # (3)
```

1. See [:material-code-braces: DiscountsBreakdownTypeDef](./type_defs.md#discountsbreakdowntypedef)
2. See [:material-code-braces: TaxesBreakdownTypeDef](./type_defs.md#taxesbreakdowntypedef)
3. See [:material-code-braces: FeesBreakdownTypeDef](./type_defs.md#feesbreakdowntypedef)

## ListInvoiceSummariesRequestPaginateTypeDef

```python
# ListInvoiceSummariesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import ListInvoiceSummariesRequestPaginateTypeDef


def get_value() -> ListInvoiceSummariesRequestPaginateTypeDef:
    return {
        "Selector": ...,
    }


# ListInvoiceSummariesRequestPaginateTypeDef definition

class ListInvoiceSummariesRequestPaginateTypeDef(TypedDict):
    Selector: InvoiceSummariesSelectorTypeDef,  # (1)
    Filter: NotRequired[InvoiceSummariesFilterTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: InvoiceSummariesSelectorTypeDef](./type_defs.md#invoicesummariesselectortypedef)
2. See [:material-code-braces: InvoiceSummariesFilterTypeDef](./type_defs.md#invoicesummariesfiltertypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListInvoiceSummariesRequestTypeDef

```python
# ListInvoiceSummariesRequestTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import ListInvoiceSummariesRequestTypeDef


def get_value() -> ListInvoiceSummariesRequestTypeDef:
    return {
        "Selector": ...,
    }


# ListInvoiceSummariesRequestTypeDef definition

class ListInvoiceSummariesRequestTypeDef(TypedDict):
    Selector: InvoiceSummariesSelectorTypeDef,  # (1)
    Filter: NotRequired[InvoiceSummariesFilterTypeDef],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: InvoiceSummariesSelectorTypeDef](./type_defs.md#invoicesummariesselectortypedef)
2. See [:material-code-braces: InvoiceSummariesFilterTypeDef](./type_defs.md#invoicesummariesfiltertypedef)

## InvoiceCurrencyAmountTypeDef

```python
# InvoiceCurrencyAmountTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import InvoiceCurrencyAmountTypeDef


def get_value() -> InvoiceCurrencyAmountTypeDef:
    return {
        "TotalAmount": ...,
    }


# InvoiceCurrencyAmountTypeDef definition

class InvoiceCurrencyAmountTypeDef(TypedDict):
    TotalAmount: NotRequired[str],
    TotalAmountBeforeTax: NotRequired[str],
    CurrencyCode: NotRequired[str],
    AmountBreakdown: NotRequired[AmountBreakdownTypeDef],  # (1)
    CurrencyExchangeDetails: NotRequired[CurrencyExchangeDetailsTypeDef],  # (2)
```

1. See [:material-code-braces: AmountBreakdownTypeDef](./type_defs.md#amountbreakdowntypedef)
2. See [:material-code-braces: CurrencyExchangeDetailsTypeDef](./type_defs.md#currencyexchangedetailstypedef)

## InvoiceSummaryTypeDef

```python
# InvoiceSummaryTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import InvoiceSummaryTypeDef


def get_value() -> InvoiceSummaryTypeDef:
    return {
        "AccountId": ...,
    }


# InvoiceSummaryTypeDef definition

class InvoiceSummaryTypeDef(TypedDict):
    AccountId: NotRequired[str],
    InvoiceId: NotRequired[str],
    IssuedDate: NotRequired[datetime.datetime],
    DueDate: NotRequired[datetime.datetime],
    Entity: NotRequired[EntityTypeDef],  # (1)
    BillingPeriod: NotRequired[BillingPeriodTypeDef],  # (2)
    InvoiceType: NotRequired[InvoiceTypeType],  # (3)
    OriginalInvoiceId: NotRequired[str],
    PurchaseOrderNumber: NotRequired[str],
    BaseCurrencyAmount: NotRequired[InvoiceCurrencyAmountTypeDef],  # (4)
    TaxCurrencyAmount: NotRequired[InvoiceCurrencyAmountTypeDef],  # (4)
    PaymentCurrencyAmount: NotRequired[InvoiceCurrencyAmountTypeDef],  # (4)
```

1. See [:material-code-braces: EntityTypeDef](./type_defs.md#entitytypedef)
2. See [:material-code-braces: BillingPeriodTypeDef](./type_defs.md#billingperiodtypedef)
3. See [:material-code-brackets: InvoiceTypeType](./literals.md#invoicetypetype)
4. See [:material-code-braces: InvoiceCurrencyAmountTypeDef](./type_defs.md#invoicecurrencyamounttypedef)
5. See [:material-code-braces: InvoiceCurrencyAmountTypeDef](./type_defs.md#invoicecurrencyamounttypedef)
6. See [:material-code-braces: InvoiceCurrencyAmountTypeDef](./type_defs.md#invoicecurrencyamounttypedef)

## ListInvoiceSummariesResponseTypeDef

```python
# ListInvoiceSummariesResponseTypeDef TypedDict usage example

from types_aiobotocore_invoicing.type_defs import ListInvoiceSummariesResponseTypeDef


def get_value() -> ListInvoiceSummariesResponseTypeDef:
    return {
        "InvoiceSummaries": ...,
    }


# ListInvoiceSummariesResponseTypeDef definition

class ListInvoiceSummariesResponseTypeDef(TypedDict):
    InvoiceSummaries: List[InvoiceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See `List[InvoiceSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

