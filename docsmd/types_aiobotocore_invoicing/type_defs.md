# Type definitions

> [Index](../README.md) > [Invoicing](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Invoicing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/invoicing.html#invoicing)
    type annotations stubs module [types-aiobotocore-invoicing](https://pypi.org/project/types-aiobotocore-invoicing/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## BatchGetInvoiceProfileRequestRequestTypeDef

```python
# BatchGetInvoiceProfileRequestRequestTypeDef definition

class BatchGetInvoiceProfileRequestRequestTypeDef(TypedDict):
    AccountIds: Sequence[str],
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

## InvoiceUnitRuleTypeDef

```python
# InvoiceUnitRuleTypeDef definition

class InvoiceUnitRuleTypeDef(TypedDict):
    LinkedAccounts: NotRequired[Sequence[str]],
```

## ResourceTagTypeDef

```python
# ResourceTagTypeDef definition

class ResourceTagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## DeleteInvoiceUnitRequestRequestTypeDef

```python
# DeleteInvoiceUnitRequestRequestTypeDef definition

class DeleteInvoiceUnitRequestRequestTypeDef(TypedDict):
    InvoiceUnitArn: str,
```

## FiltersTypeDef

```python
# FiltersTypeDef definition

class FiltersTypeDef(TypedDict):
    Names: NotRequired[Sequence[str]],
    InvoiceReceivers: NotRequired[Sequence[str]],
    Accounts: NotRequired[Sequence[str]],
```

## InvoiceUnitRuleOutputTypeDef

```python
# InvoiceUnitRuleOutputTypeDef definition

class InvoiceUnitRuleOutputTypeDef(TypedDict):
    LinkedAccounts: NotRequired[List[str]],
```

## ReceiverAddressTypeDef

```python
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

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    ResourceTagKeys: Sequence[str],
```

## CreateInvoiceUnitResponseTypeDef

```python
# CreateInvoiceUnitResponseTypeDef definition

class CreateInvoiceUnitResponseTypeDef(TypedDict):
    InvoiceUnitArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteInvoiceUnitResponseTypeDef

```python
# DeleteInvoiceUnitResponseTypeDef definition

class DeleteInvoiceUnitResponseTypeDef(TypedDict):
    InvoiceUnitArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateInvoiceUnitResponseTypeDef

```python
# UpdateInvoiceUnitResponseTypeDef definition

class UpdateInvoiceUnitResponseTypeDef(TypedDict):
    InvoiceUnitArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateInvoiceUnitRequestRequestTypeDef

```python
# UpdateInvoiceUnitRequestRequestTypeDef definition

class UpdateInvoiceUnitRequestRequestTypeDef(TypedDict):
    InvoiceUnitArn: str,
    Description: NotRequired[str],
    TaxInheritanceDisabled: NotRequired[bool],
    Rule: NotRequired[InvoiceUnitRuleTypeDef],  # (1)
```

1. See [:material-code-braces: InvoiceUnitRuleTypeDef](./type_defs.md#invoiceunitruletypedef) 
## CreateInvoiceUnitRequestRequestTypeDef

```python
# CreateInvoiceUnitRequestRequestTypeDef definition

class CreateInvoiceUnitRequestRequestTypeDef(TypedDict):
    Name: str,
    InvoiceReceiver: str,
    Rule: InvoiceUnitRuleTypeDef,  # (1)
    Description: NotRequired[str],
    TaxInheritanceDisabled: NotRequired[bool],
    ResourceTags: NotRequired[Sequence[ResourceTagTypeDef]],  # (2)
```

1. See [:material-code-braces: InvoiceUnitRuleTypeDef](./type_defs.md#invoiceunitruletypedef) 
2. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    ResourceTags: List[ResourceTagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    ResourceTags: Sequence[ResourceTagTypeDef],  # (1)
```

1. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
## GetInvoiceUnitRequestRequestTypeDef

```python
# GetInvoiceUnitRequestRequestTypeDef definition

class GetInvoiceUnitRequestRequestTypeDef(TypedDict):
    InvoiceUnitArn: str,
    AsOf: NotRequired[TimestampTypeDef],
```

## ListInvoiceUnitsRequestRequestTypeDef

```python
# ListInvoiceUnitsRequestRequestTypeDef definition

class ListInvoiceUnitsRequestRequestTypeDef(TypedDict):
    Filters: NotRequired[FiltersTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    AsOf: NotRequired[TimestampTypeDef],
```

1. See [:material-code-braces: FiltersTypeDef](./type_defs.md#filterstypedef) 
## GetInvoiceUnitResponseTypeDef

```python
# GetInvoiceUnitResponseTypeDef definition

class GetInvoiceUnitResponseTypeDef(TypedDict):
    InvoiceUnitArn: str,
    InvoiceReceiver: str,
    Name: str,
    Description: str,
    TaxInheritanceDisabled: bool,
    Rule: InvoiceUnitRuleOutputTypeDef,  # (1)
    LastModified: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InvoiceUnitRuleOutputTypeDef](./type_defs.md#invoiceunitruleoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InvoiceUnitTypeDef

```python
# InvoiceUnitTypeDef definition

class InvoiceUnitTypeDef(TypedDict):
    InvoiceUnitArn: NotRequired[str],
    InvoiceReceiver: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    TaxInheritanceDisabled: NotRequired[bool],
    Rule: NotRequired[InvoiceUnitRuleOutputTypeDef],  # (1)
    LastModified: NotRequired[datetime],
```

1. See [:material-code-braces: InvoiceUnitRuleOutputTypeDef](./type_defs.md#invoiceunitruleoutputtypedef) 
## InvoiceProfileTypeDef

```python
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
# ListInvoiceUnitsRequestPaginateTypeDef definition

class ListInvoiceUnitsRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[FiltersTypeDef],  # (1)
    AsOf: NotRequired[TimestampTypeDef],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FiltersTypeDef](./type_defs.md#filterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListInvoiceUnitsResponseTypeDef

```python
# ListInvoiceUnitsResponseTypeDef definition

class ListInvoiceUnitsResponseTypeDef(TypedDict):
    InvoiceUnits: List[InvoiceUnitTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: InvoiceUnitTypeDef](./type_defs.md#invoiceunittypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetInvoiceProfileResponseTypeDef

```python
# BatchGetInvoiceProfileResponseTypeDef definition

class BatchGetInvoiceProfileResponseTypeDef(TypedDict):
    Profiles: List[InvoiceProfileTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InvoiceProfileTypeDef](./type_defs.md#invoiceprofiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
